# Talk Plan Review — Angular→React Migration (per CandleKeep library)

## TL;DR

Your 24-slide, six-bit plan is **strong and correctly on-genre** for a 30–40 min technical talk. It passes the hardest test (the slide titles alone tell the whole story), and your bit structure maps almost exactly onto the standard tech-talk time budget. The books mostly **confirm your instincts** — especially the restrained AI-fall and the disciplined code slides.

Three places to look, all near the **opening and the close**:

1. The "no ending" open withholds without promising a payoff — the audience may read it as "incomplete."
2. The close can recover narrative symmetry via a **spoken ship-question callback** — and this is _compatible_ with sending the React question ("would you move today?") to Q&A. They're two different questions; an earlier draft of this review conflated them.
3. The real spine issue is **not** a missing closing line. The talk's _intended_ spine (people/momentum, from the handoff) and its _enacted_ spine (refactor-not-translation, what bits 3–4 actually teach) have drifted apart. Fix by reconnecting bits 3–4 to the spine — enacted, not stated. **Don't add a throughline sentence.**

> **Caution this document forces but didn't originally name:** taken together, the fixes below rebuild the lean close you deliberately stripped this session (one slide, finale→Q&A, no number bookend). Pick the _subset_ that recovers symmetry without the victory lap. Recommended subset: **#1 (open promise) + enacted-#2 (ship close)**. Skip the stated throughline.

## Steps I'd take (in priority order)

**Do these two — they recover symmetry without rebuilding the victory lap:**

- [~] **#1 — Add a promise to the "no ending" open.** ⚠️ CONSIDERED, REJECTED. The suggested callback line is a slogan (announces its own cleverness) and half-answers the question Slide 1 deliberately leaves open. This is TED/Anderson polish imported into a non-TED talk. Handled instead by *delivery* — say "this is not a story with an ending" as a confident thesis, not an apology (`bit1.md` Slide 2 notes). No added line.
- [x] **#2 — Recover the ship-question callback at the close, _spoken and enacted_.** ✅ DONE in the ship session — the wordless half-green sailing closing card after Slide 24 *is* the enacted callback ("still sailing, still rebuilding"). React→Q&A kept. See `ship-visual-system.md`.

**Consider, but don't over-correct:**

- [ ] **Reconnect bits 3–4 to the spine (replaces old "state the throughline").** The craft (refactor-not-translation) should visibly serve people/momentum: it's _what let a 2–3-person spare-time effort sustain five years_. Enact this connection; **do not** add a throughline sentence or poster slide.
- [x] **#4 — Give Slide 24 a visual anchor.** ✅ RESOLVED in the ship session — chose reflection-stays + **separate wordless closing ship card** after it (the card, not the text, holds through Q&A). See `bit5.md` Finale + `ship-visual-system.md`.

**Trivial / mechanical:**

- [x] **Slide 13: pick the diagram, not the code** (`scope.$evalAsync`) — ✅ DONE in `bit3.md`: data-flow arrows (`data ⇄ view` vs `data → view`), code dropped.
- [ ] **Check the dwell-heavy text slides (14, 22, 24)** — at 24 slides / 35 min you're under 1/min, so these hold 2–3 min each. Make each earn it. *(Still open — a delivery/rehearsal check, not a fix.)*

---

# Full Review

Read all five bits and both reference threads (the 30-min tech-talk guide + the TED/StoryBrand storytelling books).

## The plan is strong and on-genre

Run Riederer's test (read slide titles in sequence — do they tell the whole story without the body?): yours do.

> Ship of Theseus question → 5 years / no ending → self-intro → the codebase before → why change → how decided → options → why incremental + r2a → foundations → decisions in a vacuum → mid-flight → two versions → two models → 50/50 → research → table choices → table implementation → migrating a view → the return → the fall (quote) → looked done / bugs / paused → the method → dashboard full-screen (50%) → what I'd do differently.

That coherence is the thing most decks fail, and you pass it.

Mapped to Ernst's five-phase budget for a 30-min talk:

| Phase               | Time      | Your bit |
| ------------------- | --------- | -------- |
| Hook / problem      | 0–3 min   | Bit 1    |
| Context / landscape | 3–8 min   | Bit 2    |
| Core content        | 8–22 min  | Bits 3–4 |
| Takeaways           | 22–27 min | Bit 5    |
| Q&A buffer          | 27–30 min | —        |

For your 40-min slot, stretch the core band (Bits 3–4); the proportions hold.

## Where the books say you're off

### 1. The opening "no ending" has no promise attached — clearest miss

Anderson: a rhetorical question works because it opens a knowledge gap "the brain fights to close" — but "tease, but don't give it away" still requires **mapping**: the audience must know **why** there's no ending, or they read it as "no payoff," i.e. incompleteness.

Right now Slide 2 withholds without promising. You _do_ pay it off structurally (Slide 23 = the proof), but nothing up front tells them a payoff is coming. Consider a half-line that turns the open-endedness into the point:

> "We started five years ago. This is not a story with an ending — and that's the right answer to the question I just asked you."

Good news: Slide 1 doesn't name "Ship of Theseus" on screen — keep it that way. The name-drop (reading as learned rather than visceral) is the one risk Anderson flags, and you've already dodged it.

### 2. The close can recover narrative symmetry — and it's compatible with React→Q&A

**First, untangle two questions an earlier draft of this review conflated:**

- **The ship question** (Slide 1): _rebuild it in a different language without changing it?_
- **The React question**: _would you move to React today?_ — sent to Q&A, correctly.

The narrative-symmetry close is about the **ship** question, which you did _not_ send to Q&A. So there's no conflict: keep React→Q&A and still do a ship callback. Anderson names _narrative symmetry_ (reframe the opening question with what the audience now knows) as "the most technically sophisticated ending available to you." Do it **enacted, not restated** — the half-rebuilt ship ("still sailing, still rebuilding") _is_ the callback; you don't re-ask the question as text. This fits your anti-slogan instinct better than the prose first implied.

**Recency weighting (Kahneman, via Anderson):** the final moment is what's remembered. Your _peak_ is Slide 23 (the 50%, full-screen), then you step down to a quiet text slide for the actual ending. That can work as a forward reframe — but it means Slide 24 has to carry disproportionate weight with no visual. Ernst: it sits on screen the entire Q&A; "make it worth staring at." Two columns of ≤5-word phrases may be too thin for that job (see Slide 24 in step #4).

### 3. The real spine issue: intended vs. enacted throughline have drifted (don't fix with a sentence)

An earlier draft of this review told you to "state the throughline once." That was the wrong fix, and it's the one most likely to produce the slogan slide you keep cutting. Here's the actual problem.

**Your _intended_ spine is documented** — handoff lines 3, 25–26: _"you can lead deep technical change from the bottom — the hard part is not the technology but holding momentum and recruiting people over years. A story of ownership and initiative."_ People/momentum. Not invented by this review; lifted from your own document.

**But the talk now _enacts_ a different spine.** Bits 3–4 (13 of 24 slides) teach _refactor-not-translation_ craft for its own sake. The restructuring this session moved weight off the human arc (human moments pulled from Bit 3; Bit 5 — which the handoff calls "the heart, and the longest" — is now a single forward slide) and onto the craft. Center of gravity slid toward craft; the close still pleads people (dedicated team, "what I'd want"). That's the mismatch.

**They are not co-equal rivals — one is the rope, one is the payload.** Run Anderson's rope test (the throughline ties together _every_ element). Ask which spine explains the AI fall, the spare-time pockets, the CEO conversation, the VP, "would you do it again":

- **People/momentum** explains all of them.
- **Refactor-not-translation** explains _none_ of them — only the table and the AI method, both inside bits 3–4.

So refactor-not-translation is not a second throughline; it's the **largest single lesson hanging on the people/momentum rope** — the evidence, not the point. If you switched the spine _to_ it, the AI fall and the whole human arc lose their rope and become loose anecdotes.

**The fix is a connection, not a sentence.** Make bits 3–4 visibly serve the spine: _refactor-not-translation is what let a 2–3-person, under-prioritized, spare-time effort sustain momentum for five years._ That link is currently missing — the craft is taught in isolation. Enact it (the half-rebuilt ship says "still going" without a line of moral). Then you never need the poster sentence, and Anderson's "leave enough to connect the dots" is satisfied by the structure, not by narration.

## Where the books confirm your instincts

- **The AI fall.** Brené Brown's test (via Anderson) is the cleanest check: _"a story is only ready to share when the presenter's growth is not dependent on the audience's response."_ Your handoff already enforces restraint and the "no wrongly-blamed bug" honesty — that's vulnerability _with_ boundaries. Aligned. Gallo adds: don't stop at "AI made a mistake" (the audience assumes that's possible) — land on what it revealed about human accountability vs. delegation. Your Slide 22 does exactly this.
- **Code slides.** Ernst: "elide everything that does not support your key points… show the one telling line." Slides 12 / 17 are disciplined (shape, not volume). One flag: **Slide 13** (`scope.$evalAsync`) — you left it as "code or diagram, speaker's choice." Ernst's "prioritize intuitions over technical minutiae" pushes you to the diagram. Pick the diagram.
- **Slide density.** 24 slides / 35 min is _under_ Ernst's ~1/min (he suggests ~25–28 for 30 min). Not wrong, but it means slides 14, 22, 24 hold for 2–3 min each — those are your text slides. That's exactly where under-density bites. Make sure each earns the dwell time.

## The moves I'd actually make (a deliberate subset — don't do all of them)

The fixes above, taken together, would rebuild the lean close you stripped this session. Recover symmetry without the victory lap:

1. **Add a promise to the "no ending" open** (one half-line). Cheap, no downside.
2. **Recover the ship-question callback at the close — spoken and enacted**, via the half-rebuilt ship. Compatible with React→Q&A; they're different questions.

Then, separately and carefully:

3. **Reconnect bits 3–4 to the spine** (craft serves people/momentum) — _enacted, not stated_. **Skip** any throughline sentence.
4. **Give Slide 24 a visual anchor** (the ship) — but resolve the collision with the two-half text first.

Trivial: Slide 13 → diagram; check dwell on slides 14/22/24.

---

## Sources

- **Giving a 30-Minute Tech Talk** (Witowski / Riederer / Ernst) — primary reference. Time budget, ~1 slide/min, code-on-slides, openings/closings, Q&A protocol.
- **TED Talks: The Official Guide** (Anderson) — throughline, vulnerability, knowledge-gap questions, narrative-symmetry close, "connect the dots."
- **Talk Like TED** (Gallo) — emotional arc, "unexpected result" stories, stating the moral at most once.
- **Building a StoryBrand 2.0** (Miller) — guide-not-hero framing (the audience are the heroes who borrow your lessons).

> "We need to have owned our stories before sharing them is experienced as a gift. A story is only ready to share when the presenter's healing and growth is not dependent on the audience's response to it." — _TED Talks: The Official Guide_, p. 322

> "A lighter treatment that leaves audiences wanting more beats rushing through too much." — Ernst, _Giving a 30-Minute Tech Talk_, p. 2

---

# Addendum — Ship motif as a recurring visual

> ⚠️ **SUPERSEDED (2026-05-30) by `slides/ship-visual-system.md`.** This addendum is kept for history; the ship session deliberately diverged from it in three places:
> - **No seam/transition cards** (this addendum's 2→3, 3→4 cards) — a *corner color-fill progress meter* (grey→green) on most slides does the orientation instead.
> - **Ship OFF Slide 23** — the dashboard peak stays pure documentary; this addendum's "pair the ship with the dashboard" was rejected.
> - **Slide 1 is wordless** — the Theseus question is spoken, not printed over the ship.
> Read `ship-visual-system.md` for the live system; treat the per-state notes below as non-authoritative.

**Decision context:** the ship is one _unified_ metaphor across the talk, not decoration. Bit 3's analogy is the ship itself (replace the engine at sea while the PO asks for a new deck) — so there's no competing "plane" metaphor. Fix needed: `bit3.md` Slide 11 currently says "plane in flight / engine mid-flight / first class" and "(not Ship of Theseus)" — change it to the ship.

**Principle:** Ernst endorses a recurring orientation visual for 30+ min talks. Use the ship at the **seams (bit boundaries) + the two bookends** — 5 states, not 24. Keep it **off** the real-artifact slides (4, 16, 18, 23) so the screenshots keep their documentary weight; the only exception is the ship's own _meaning_ slide at the 50% (see Slide 23 note).

## Ship states — copy-ready slide notes

**Slide 1 (open) — whole original ship**

> Ship visual: the original ship, intact, whole. The question sits over it ("rebuild it in a different language without changing it?"). Plant the metaphor without naming "Ship of Theseus" on screen.

**Slide 2 (hook) — same whole ship, "no ending" promise**

> Keep the whole ship behind the two lines. Add the spoken promise so the open-endedness reads as the point, not as incompleteness: "…and that's the right answer to the question I just asked."

**Slide 11 (Bit 3 — the ship scene, NOT a plane)**

> Replace the current plane/engine visual with the ship: engine being swapped _while at sea_, PO leaning over asking for a new deck. This is the operational constraint (can't stop the running system) — a content slide, the ship's working appearance. Two lines delivered verbally. ("new deck" = ship deck / slide deck pun, optional.)

**Bit boundary 2→3** _(if you use a transition card)_ **— a few planks swapped**

> Ship with a handful of new planks visibly different from the old — migration just underway.

**Bit boundary 3→4 — roughly half rebuilt**

> Ship clearly part-old, part-new. Mirrors the 50/50 reframe of Slide 14.

**Slide 23 (the 50%) — ship visibly ~half, old + new planks both showing**

> This is the one real-artifact slide where the ship's _meaning_ belongs: pair (or alternate) the full-screen dashboard with the half-rebuilt ship. Old and new planks both visible = the ~50%, earned. The ship makes the number a metaphor-payoff, not just a stat.

**Slide 24 (close) — same half-rebuilt ship, "still sailing, still rebuilding"**

> Reuse the Slide 23 ship as the visual anchor Slide 24 was missing. Spoken narrative-symmetry callback to the opening question (don't restate the question as text). "Still sailing, still rebuilding" = the no-ending payoff + the symmetry close in one image. This also lets the ship — not bullet text — be what sits on screen through Q&A.

**Do NOT put a ship on:** Slide 4 (real controller), 16 (annotated table), 18 (annotated view). Let the artifacts carry those.

---

# Addendum — Skeleton (`migration-talk-sekelton.md`) vs. deck: reconcile

The prose skeleton (the script) is **more book-aligned than the deck in its instincts** — its tone rules already encode what the books preach — but it exposes the spine drift more plainly and disagrees with the deck in three spots. The work here is consistency, not new ideas.

## What the books praise in the skeleton

- **Tone rules (lines 12–16) are already the books' position.** Line 15 — _"don't announce the moral — the spine is enacted, not declared; enough that the audience connects the dots"_ — is almost verbatim Anderson, p. 561: _"You don't want to... force-feed the conclusion... but you absolutely do want enough there for your listeners to connect the dots."_ This **vindicates the "don't add a throughline sentence" call** in §3 above. Your own skeleton forbids it.
- **Cutting silence-asymmetry (line 168)** for "sounds like a complaint, not an insight" = Brené Brown via Anderson: _"vulnerability minus boundaries is not vulnerability."_ Venting filtered from insight. Right call.
- **The spine (line 9) is documented and singular** — people/momentum. Confirms §3: the intended throughline is not the review guessing.

## Five things to reconcile (book-grounded)

1. ~~**The ship/plane clash is still in the script — unresolved.**~~ ✅ **RESOLVED (review was stale).** Skeleton Bit 3 analogy now reads "החלפת מנוע בלב ים … סיפון חדש … אותה ספינה … בלי מטוס מתחרה"; `bit3.md` Slide 11 is "Swapping the engine at sea." Both files carry the ship; no plane remains.

2. ~~**Naming "Ship of Theseus" aloud (line 40).**~~ ✅ **RESOLVED — decided: say the paradox, not the name.** Speak the plank question and bridge to the app; do not say "Ship of Theseus" aloud. Applied to `bit1.md` Slide 1, skeleton Bit 1 analogy, and `ship-visual-system.md`.

3. ~~**Skeleton vs. deck disagree on the dashboard.**~~ ✅ **RESOLVED.** Skeleton's _"מדידה כתנאי להמשך"_ (measurement as a condition) replaced with the deck's honest version — _"כלי לדעת איפה הדברים עומדים — לא מדידה ממושמעת, רובו vibe-coded."_ Skeleton and `bit4.md` Slide 19 now agree.

4. **Timing under-runs the target.** Per-bit budgets sum to **24–30 min** (4–5 ×4 + 8–10); stated target is 32–35 min content. You're 2–5 min light on paper. Either bits expand in delivery (likely) or there's room to deepen the **core (Bit 4)**, not the framing. Use Ernst's 10/20/25-min rehearsal checkpoints to calibrate.

5. **The hook has no promise (same as the deck).** ⚠️ Same call as #1 — the added-line fix was **rejected** as a slogan; handled via delivery (confident thesis, not apology). No script change.
