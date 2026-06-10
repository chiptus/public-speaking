# Design notes — rationale behind the slides

> **Not for the designer and not for the speaker-notes pane.** This is the editorial "why" behind each bit — kept out of the slide files so those stay clean handoff specs. The per-slide `Visual` + `Notes` (beats / 🔒 verbatim / cues) live in `slides/bitN.md`; the *reasoning* lives here.

---

## Bit 1 — Opening

- Ship is enacted, never named "Ship of Theseus" aloud — the verbatim carries the paradox without the label (`talk-review.md`).
- Stack is split across two slides: Slide 2 names the destination (React), Slide 4 names the source (AngularJS) on the actual old code. Neither slide carries the full "AngularJS → React".
- Slide 2 hook works on the mismatch — a React migration that's taken 5+ years and still has no end. That question is the talk's pull. No number (the ~50%) here; it's withheld until the Bit 4 close. Deliver "no ending" as thesis, not apology.
- Slide 3: "since 2018" replaces tenure math; the "left and came back" beat is deferred to the AI-fall section.
- Slide 4 carries no *thesis about the migration* — the old "didn't create it, exposed it" line was cut: at Slide 4 it's an unearned summary, and a rebuttal to a charge nobody's made yet, not a reason. The bridge into Bit 2 is a connective on Slide 5 ("it wasn't only the mess"), not a closing line here.
- **Slide 4 audience-stake beat** ("אולי יש לכם קוד כזה... אני לא בטוח שזה נכון"): the skeleton's מסר לקהל ("you're not trapped") was on no slide — the one line that earns a senior dev's attention was missing. It lands here, off the concrete mess, so it's a *promise on recognition*, not an assertion (distinct from the cut migration-thesis above: this addresses the room, not the migration). Hedged ("I'm not sure that's true") on purpose: states doubt, not a guarantee — the talk earns the answer instead of selling it. Also fixes the thin ~1-min open: the open was short on *stake*, not on silence — pauses alone couldn't fill it.
- The "don't blame the migration / it exposed what was already broken" idea isn't lost — it's the same thought as the S21 fear-attribution beat ("every bug gets blamed on the migration"), where it's earned. See `bit4.md` Slide 21.
- Slide 1 grey ship teaches the full silhouette so the corner progress meter reads later (`ship-visual-system.md`).

---

## Bit 2 — The Decisions

- **S5 seam:** opens on Bit 1's mess connective so it reads as escalation, not a fresh start (the seam from Slide 4; Bit 1 has no closing bridge).
- **S9 reframe:** the slide is the payoff of S5's legitimacy beat, not a "foundations first" principle. The TS-resistance line echoes S6 (decided together) — keep it an aside; don't announce a moral. _(alt titles: "While we were in there" · "מה שהמעבר אפשר")_
- **S10:** behavior-preserving-but-fully-refactored is what Bit 4 cashes ("migration ≠ translation"). The bridge springs straight into Bit 3 (engine at sea), no reach-back.
- **Bit 2 through-line:** S6 · S9 · S10 are a quiet trilogy of collective decisions the speaker didn't fully own (decided-together · overruled-and-glad · a-decision-not-a-regret).

### Decisions (2026-06-06 — S5 reasons + EOL timeline + S8 snippet)

- **S5 reasons rewritten — hiring leads, EOL is a deadline not a trigger.** Take-1 (`takes/take 3 - bit 2/take1.txt`) framed it as "a month after we started, AngularJS was declared dead" — death-as-surprise-cause. That's false: AngularJS LTS was announced **2018**, EOL date **Dec 31 2021** (verified — [Angular blog](https://blog.angular.dev/stable-angularjs-and-long-term-support-7e077635ee9c), extended for COVID, [InfoQ](https://www.infoq.com/news/2022/01/angularjs-lts-end/)). So the end date was public for **years**; they prepared, didn't react. The honest trigger was **hiring** (the CEO argument), not EOL. New three lines: _hard to hire · refactor needed anyway · EOL deadline_. **"new features coming" dropped from S5** — it's a constraint that argues for _incremental_, not a reason to _change_; it already lives in S7 reqs ("keep shipping"). Speaker's internal "since 2018" (S3) ≈ the same year the public clock started — a real alignment to lean on, but **not** the same event (don't sell a tidy-but-false coincidence; tone rule).
- **Hiring sits on both S5 and S6 on purpose (setup→payoff, not redundancy).** S5 names it flat as a _reason_; S6 is the _scene_ where that argument lands with the CEO ("spoke his language"). S6's old standalone "can't hire" line was rewritten to point back at S5 so it reads as the payoff, not a fresh introduction.
- **S8 = code snippet, diagram dropped.** Per take-1 review: the box-arrow r2a diagram was replaced with two tiny code blocks (**register** a React component as an Angular one, then **use** it in a template). The snippet _is_ the diagram — more concrete, and it makes the take's clearest line ("I just need the component and its props") show rather than assert. Kept to two blocks (no API tour) so it doesn't front-load Bit 4's code budget (S12/S17). **Sets up S12**: S8 shows r2a clean, S12 shows where it breaks (`children`/`ng-transclude`) — a real cross-bit setup→payoff. Snippet reconciled against the real r2a signature (confirmed 2026-06-06).
- **S7 "do nothing" dropped — level separation.** S7 is a _how to migrate_ list (rewrite · micro-frontends · incremental — three real strategies); "do nothing" is a _whether_ question, already settled by S5's three reasons. Striking it on S7 ("→ lib dead") just restated S5. It's also where take-1 went circular (not a distinct beat, a restatement). Clean split now: **S5 = whether (must change), S7 = how (three strategies).** Build drops 4→3 (two rejected, incremental stands).

### Within-slide anchor — Sagit's "cognitive anchor" (2026-06-10)

One mechanic, generalized from S7's strike: exactly one unit is **active** (lit / full weight), the rest de-emphasized; the marker advances **synced to delivery, never auto**. Job: orient the room (_where am I inside this slide_) **and** brake pacing (can't advance until the current unit lands). Two flavors:

- **Eliminate (S7):** all points shown; strike each as it's rejected; the survivor stands. For knocking options down.
- **Accumulate (S5):** points build in one at a time; current lit, prior ones dim but kept, next absent. For building a case.

**Grain is the real choice, not whether to anchor.** S5/S7 anchor at the **item** level (one line at a time). S22 and S24 already anchor at the **group** level — S22: framing line → the four principles (2 beats); S24: "mine" row → "need" row (2 beats). That coarser grain is correct for them: going finer (lighting each principle / each mine-item individually) would fight S22's _cluster_ read ("back to basics" lands as one thing) and S24's _band_ asymmetry (mine vs. not-mine is the point, not the individual items). So: new work was S5 only; S7/S22/S24 were already anchored at the grain that fits them. Sparing by design — match the grain to what the slide is doing.

---

## Bit 3 — Living with Mixed Code

- The ship is the talk's single unified metaphor (Bit 1, Ship of Theseus), now shown in its working state — no competing plane.
- S13 was flagged "unclear" in run 1 (`takes/take1/notes1.md`) — keep it concrete: one symptom (the wrapper), one cost (two mental models), no API tour.
- Bridge springs straight off S14, no reach-back into Bit 3.
- **2→3 seam = a question on S11, not a bridge line on S10 (2026-06-10).** Sagit's "seams as questions" → only 2→3 needed it (1→2 and 3→4 were already questions; 4→5 stays the thesis, not a question). The question — _"how do you swap an engine while the ship's still sailing?"_ — is asked **as S11's engine-at-sea image reveals**, not as a spoken bridge over S10. A seam line that describes the image would narrate/deflate the visual (and S10 "new engine underneath" + S11 already share the metaphor). S10→S11 run quick (<1 min) on purpose — pivot beats, not teaching beats; Bit 3's weight is S14's "for years" pause.

### Decisions made (Bit 3 session)

- [אנושי] moments (silence asymmetry, stolen time) removed from Bit 3 — placement TBD in Bit 5 planning
- Slide 12: code snippet approved (ng-transclude vs children prop)
- Analogy: swapping the engine at sea — the ship is the talk's single metaphor (Bit 1 Ship of Theseus); the competing plane was removed

---

## Bit 4 — Depth and AI

### Decisions so far (this session)

- Sub-arc A reframed from "the table story" → **"building a component library"** (table-only felt too lean). Research → find patterns (tables, form fields) → build components → shared library.
- Slide 15 titled "Research" — about the _general_ method, not one artifact. Visual = screenshots of old copy-pasted patterns.
- **The table is the worked example, split across two slides (option B):** 16 = the choices (pattern research → TanStack Table → API design), 17 = implementation evolution (composable components → `Datatable` + variants like `ExpandableTable`). "Migration ≠ translation" moved to 18.
- **S21 is the earned home for the cut Bit 1 line** ("the migration didn't create the mess, it exposed it") — same thought, lands here where the audience has lived it. Optional to voice; don't force it.
- **Sub-arc B restructured to 6 slides (19–24); bit is now 10 slides (15–24):**
  - Dropped the "Skipping patience" slogan slide entirely — too neat / "selling the story back."
  - The quote IS the fall (feeling + action are one moment); collapsed into a single slide (21).
  - Dashboard moved _before_ the fall, to a new **Return** slide (20) — it's a tool built on re-entry, not the disciplined "measurement" beat it was miscast as.
  - Method slide (23) reframed: AI _emphasizes_ the fundamentals (plan → tasks → small units · YAGNI · bottom-up), doesn't replace them — the honest takeaway of the arc.
  - Quote intro resolved: **warm** verbal setup ("convert the stack page for me") → slide.
  - Dropped the "first merge" light-moment slide — it happened ~5 yrs ago (near the start), so it can't sit at the end of the AI arc chronologically. Freed up — possible reuse in Bit 5.
  - Copilot beginning dated ~4 yrs ago (mid-2022) — now folded into Slide 18 as a tool inside the human practice, not its own slide.
- **The number moved (skeleton updated, bits 1/4/5):** Bit 1 opens with the _theme_ only — "a story without an end," no number. The **dashboard carries the number**: small/tool on the Return (19), **full-screen at the bit close (23) where the ~50% lands with earned weight.** Bit 5 no longer closes on the number — it lands on the honest answer ("would you move to React today?"). Rationale: theme-then-proof beats a repeated bookend; an abstract stat at the open becomes a number the audience understands the cost of by the end.
- **Slides 18 + 19 (old) merged into Slide 18 "Migrating a view"** — both felt thin/asserted. The view-migration slide _enacts_ "migration ≠ translation" instead of stating it as a slogan, and absorbs the "Copilot worked" beat as a footnote (Copilot helped at the line level inside the practice). Slide 22 (the method) now mirrors 18 directly: same process, AI executes the units. Bit drops to 9 slides (15–23).

### Decisions (2026-06-06 — the fall reshape + first merge)

- **S20 reshaped: the fall is now "the ask," not "the quote."** Visual = the **real merged PR screenshot** (title _"refactor(stacks): migrate create view to react"_ → **74 files changed, +2,935/−714**). The PR title doubles as the ask, so no separate prompt-UI mockup is needed; **"74 files"** is the unreviewable signal (emphasize files over line count). The disproportion (one casual sentence → 74 files) carries "top-down migration = huge PRs you can't review" **visually**, so the speaker doesn't announce the moral. (Portainer's repo is public — PR #1538 — so no confidentiality issue.) The **quote moves off-slide → spoken** ("anything's possible, just send one more message"). Trade-off accepted: lose the stark quote-as-slide, gain a concrete, visceral fall that lands with senior devs. The explicit *bottom-up* payoff stays at S22 (setup → payoff).
- **S19 floating-quote problem fixed by reorder, not removal.** S19 keeps the small dashboard visual (it's itself a vibe-coded AI artifact, so it doubles as evidence of the AI re-entry), but its notes now **end on the AI turn** so S20's ask is the immediate consequence. Dashboard shown twice is fine because the two appearances are **different facets**: S19 = the _tool_; S23 = cropped to just the **X/Y-components-done** metric (the number). Not the same view repeated.
- **The "first merge" human beat placed: S10→S11 seam, opening spoken beat of S11** (`bit3.md`). Framed as the payoff of the Bit 2 decisions (another dev built on our React components → momentum), then pivots into the mixed-code pain — warm → hard in one move. Supersedes the earlier "dropped, reuse in Bit 5" note above.
- **On-slide text fully English** — S20's Hebrew quote is gone (now spoken); no deliberate-Hebrew slide remains. **S9 title = "While we were in there."** **S24 stays one slide, two halves.**
- **Numbers added, surgically — and the "no number in Bit 1" rule above is refined.** Two _different_ numbers now bracket the talk: **S4 = the starting magnitude** (**391** AngularJS components — mostly big, undecomposed views; the "mountain," stakes), and **S23 = the progress** (~50% of that same count). **LOC was rejected** — 391 components ÷ LOC implies a misleading ~average that undercuts the "giant controllers" screenshot (the distribution is skewed: a few monsters, a long tail of small ones). **Unit = components** (not views/LOC) across S4/S19/S23. The S4 🔒 line was tweaked from "almost no components" → "barely decomposed into components" so it doesn't surface-clash with "391 components" (the 391 exist; they're just not broken down). The old line 59 rule was aimed at a _progress/percentage_ stat at the open — that still doesn't go in Bit 1. A concrete _magnitude_ on S4, tied to the giant-controller screenshot, is stakes not decoration, so it earns its place. **Constraint:** S4 and S23 must use the **same unit/denominator** or "~50%" isn't traceable. Real N is speaker-provided (`todo.md`). AngularJS/React release dates were considered and **rejected** as trivia/history-lecture risk; EOL (Dec 2021) stays as the trigger on S5 only.
- **Human story thickened (surgical — take-2 read thin vs the skeleton).** Two beats expanded in _delivery_, no new slides: **S22 reframed "The method" → "The way out"** (internal header only) — now carries the lived recovery (stalled/scared → back to the fundamentals → moving again → "today I can plan anything with it"), with **e2e tests added** to the principles as the safety net that catches "looked done" bugs and verifies behavior-preserved (ties to S10 "same surface" + S23). **S24's stolen-time beat sharpened** — "2–3 people, spare time, for years" gets its own beat + a flat/slow delivery cue so it lands as the quiet truth, not a bullet. CEO-conversation beat left **improvised** (already in the talk, deliberately not on slides); S21 fear-attribution left as-is — a **rehearsal** item (text is fine, just needs practice), not a content gap.

---

## Bit 5 — What's Next (the close)

- **S24 cut on purpose:** no "recruit partners" slogan (can't recruit people who aren't there; risked implying the 50% was a personal failure to rally a team). The honest-answer beat moved off-deck (see below).
- **Why the half-built ship reopens the old "finale: none" without betraying it.** Finale-none guarded against (1) spending the ~50% number twice, and (2) ending triumphant. A wordless, half-built, still-sailing ship does neither — no number, not finished, and a ship mid-rebuild is _literally_ a story without an end. A full/finished ship would claim a completion that didn't happen and silently restore the victory lap. (See `ship-visual-system.md`.)
- **Single-forward-slide discipline holds:** the finale is a wordless image, not a second content slide.

### Decisions (2026-06-06 — S24 reshaped: columns → rows, want → need)

- **Two stacked rows, not two columns.** The content went asymmetric (several small things in my hands, one big thing that isn't) — a wide "mine" band over a single "need" band *shows* that asymmetry and kills the empty-dark-box imbalance the two-column version had.
- **"What I'd want" → "What I'd need"** (title too). "Need" is the honest register; "want" drifted toward wishlist.
- **The product trade-off moved from the mine side to the need side — and split in two.** "Explicit product trade-off (what stays/goes)" used to be a "do differently" bullet (skeleton:65). But that decision isn't the speaker's to make — it needs product. So it became *two distinct product asks* in the need band: (1) **rank** which views matter (forward — prioritize the queue), (2) **call what's dead** so dead old constraints stop being treated as sacred (backward — the vacuum lesson). Sharpens the spine: the mine/not-mine line runs right through the most concrete decision in the talk. The need band is still **one ask** ("make it a priority") shown concretely as people + product — not a list of demands.
- **e2e appears twice on purpose, at opposite ends of the timeline.** S22 = e2e as part of the *recovery* (how I got out). S24 = e2e as a *prevention* guardrail ("pin behavior before you migrate, not after the scare"). The "before" framing is what keeps S24 from echoing S22; it also absorbs the "looked done" lesson, so no separate bullet for that. Ties to S10 ("same surface, new engine").
- **Mine band final (4):** bottom-up small targets · guardrails-first e2e · document+revisit decisions · show the team the progress. **Need band final (2):** a real priority (dedicated team, 2 devs + 1 QA) · product in the loop (rank what matters, call what's dead).
- **Final layout tuning (from rendered passes).** (1) **Slide title removed** — it repeated the two band headers; the headers + white/navy contrast carry the split alone. (2) **Height asymmetry is the argument** — white "mine" band taller (2×2 grid), navy "need" band short, hugging its two items; equal-height bands muted the "many vs. one" point, so the navy band is deliberately shrunk to fit its content. (3) **`NOT MINE TO GRANT` label kept** on the need band (the phrase is what keeps it from reading as a complaint); **`MINE` dropped** (top band is self-evidently the speaker's).

### Off-deck → Q&A

- **"Would you move to React today?"** → answered in Q&A, not a slide. Verdict is _yes, but_ — and the "but" is already Slide 24. The "yes" is one spoken line.
- **"First merge" warm moment** → Q&A answer to "a moment that stuck" / "what made it worth it." It's about the _method_ working (Bit 4's story), not a forward-looking close.

---

## Ship visual system — rationale

> The spec is `slides/ship-visual-system.md` (kept tight for the designer). The *why* lives here.

- **Color-fill, not build-up.** The app was never empty — it was a working AngularJS app. "Building from nothing" tells the wrong story; "replacing planks on a ship that keeps sailing" *is* Ship of Theseus, and it's honest. So progress shows as planks changing color within a whole ship, never as a ship assembling from parts.
- **Colors are the real brand colors (revised 2026-06-02).** Original spec said Angular-grey → React-green; corrected to **AngularJS red → React blue** — their actual brand colors, so the fill maps to something the audience can decode. Art was already red→blue; the spec was the stale side.
- **The finale reads more than half on purpose.** Earlier rule capped it at ~half-green to mirror the honest 50%. Relaxed: the exact fraction is **symbolic — no one counts planks**. What still holds is *not all-blue / not finished* — a completed ship would claim an ending the talk explicitly denies (S2: "this story has no ending"). The corner meter loosely echoes the ~50% Bit 4 dashboard but isn't a literal gauge.
- **Never say "Ship of Theseus" aloud.** Slide 1 poses the paradox by image + spoken plank-question; naming it reads as learned/academic, not visceral (Anderson). The verbatim carries the paradox without the label.
- **No seam / transition cards.** Earlier plan; dropped once the corner meter became the bit-to-bit orientation device. Dedicated boundary slides became redundant.

---

## On-slide title decisions (2026-06-02)

> Rule (from the designer brief): **no on-slide title by default** — the `## Slide N — title` header is a speaker-notes label only. A title goes on the slide **only** where it acts as a functional label on a structured slide, or where the `Visual:` line mandates one.

**Titles KEPT on-slide** (functional label for a structured visual):

| Slide | On-slide title | Why kept |
|---|---|---|
| **S5** | Why it had to change | Labels the three-reason list |
| **S6** | How it was decided | Labels the decision flow |
| **S7** | The options | **Mandated** by the `Visual:` line itself |
| **S9** | **TBD — open decision** | Gets a title ("TypeScript + Tailwind" too thin alone), but the wording is unresolved — see `todo.md` |
| **S12** | Two versions of the same component | Labels the side-by-side code |
| **S13** | Two models in your head | Labels the data-flow diagram |
| **S15** | Research | Labels the pattern screenshots |
| **S18** | Migrating a view | Labels the annotated page |
| **S19** | The return | Labels the small dashboard |
| **S24** | _(no slide title)_ — band headers "What I'd do differently" / "What I'd need" | the slide-level title was dropped (it echoed the band headers 3×); the two headers + white/navy contrast carry the split. `NOT MINE TO GRANT` kept as a green label on the need band; `MINE` dropped (the top band is self-evidently the speaker's) |

**Titles REMOVED** (the visual is self-labelling, a title would compete):

- **S4** — screenshot only.
- **S8** — the r2a diagram is self-labelled.
- **S16** — table screenshot carries its own callouts.
- **S17** — code blocks are self-captioned.

**Not titles — these are wordless or text-as-content** (so the question doesn't apply):

- Wordless / image-only: **S1, S11, finale ship card**.
- The line *is* the slide (statement text, not a heading): **S2** (hook), **S3** (self-intro), **S10** ("Same surface. New engine underneath."), **S14** (50/50 lines), **S21** ("Looked done. Bugs. Paused."), **S22** (method framing line). _(S20 is no longer here — it's now a visual slide: prompt → diff.)_

_**S9 title — decided: "While we were in there"** (2026-06-06). Understated, opportunistic; lets "TypeScript + Tailwind" carry the point without announcing the moral._
