# Talk TODO — AngularJS→React migration talk

Tracking for both of us. **@me** = Claude, **@you** = Chaim. Keep it current.

## Done

- [x] Bit 1 open — verbatim lines + Visual/Notes/cue format, Design notes block (`bit1.md`)
- [x] Close last line as verbatim on finale ship card (`bit5.md`)
- [x] Seam 1→2 — "it wasn't only the mess" connective on Bit 2 Slide 5
- [x] Cut "didn't create the mess, exposed it" from open; parked at S21 (`bit4.md`)
- [x] Slide 10 reframed: regret → "same surface, new engine" decision (`bit2.md`, commit `e1580b4`)
- [x] Seam 2→3 — straight flow S10 → S11 (engine at sea), no reach-back
- [x] Seam 3→4 — question-bridge off S14 (silence first), opens S15 Research (`bit3.md`)
- [x] Seam 4→5 — forward-turn off S23 ~50%, opens S24, pre-empts regret (`bit4.md`)
- [x] Slide 9 reframed: "Foundations first" moral → "what the migration justified" (opportunity + TS-resistance grace note), `bit2.md`
- [x] Compress notes to cue-card style (beats + one Cue, rationale → Design notes) across bits 2–5, matching bit 1 — grounded in CandleKeep delivery research

## In progress

- _(nothing active — all four bit seams done)_

## Open decisions

- [ ] Slide 24 split — "what stays / what goes" as two halves vs one? (from original handoff) — **@you to call**
- [x] **S2 on-slide lines** — I set them to _"לפני 5 שנים התחלנו לעבור ל-React"_ / _"זה לא סיפור עם סוף"_ to make the visual designer-ready. Confirm/adjust the wording — it's your hook. — **@you**
- [x] **S13 visual** — **decided: keep the data-flow diagram** (Angular ↔ 2-way vs React → 1-way). It read fine in take 2; the issue was pacing (spent too long on it), not the visual. A little natural dwell here is OK given the speaker runs fast.
- [ ] **S9 needs a title** — "TypeScript + Tailwind" alone is a label, doesn't state the point. Add a title that carries the idea (the visual can't). This is the one slide where a title clearly earns its place. **Slide file marks the title TBD; designer is blocked on this.** — **@you to pick**
  - Constraint from the beat: the notes say _"don't announce the moral / don't sell it."_ So lean understated — let "TypeScript + Tailwind" do the work under the title.
  - Candidates: _"While we were in there"_ (understated, opportunistic — recommended) · _"Since we were rebuilding anyway"_ · _"What the migration justified"_ (= section name, but "justified" states the takeaway aloud) · _"What we added to the mix"_ · or **no title** (treat like the statement slides).
- [x] **On-slide text language** — decided: **all on-slide text in English**, except the S20 quote (see below). S2 + S10 converted. Tell the designer the deck is English text / Hebrew spoken. — **@you to brief designer**
- [ ] **S20 — two open questions on the fall quote:**
  - **Language** — keep it Hebrew? Leaning yes: it's a verbatim quote actually said in Hebrew, and the emotional low point — translating it weakens it and misrepresents it. Would be the one deliberate Hebrew slide (a visual break, like the corner-ship dropping on S23). — **@you to call**
  - **Floating quote (take 2)** — the quote feels disconnected from S19 (the return); "everything is just behind another prompt" takes a full slide but doesn't flow from S19. Root cause: S19 does two jobs (built-a-dashboard + started-using-AI) and emphasizes the dashboard, so the quote lands from nowhere. Candidate fix: end S19 on the **AI re-entry** (make it the last beat), demote the dashboard to a small aside (its real payoff is S23), so S20's quote is the immediate consequence. Keep the quote a full slide once connected. — **@you to call**

## Designer handoff

- [x] Strip inline TODOs / "speaker provides" / alt-titles from `slides/bitN.md` — moved here / removed
- [x] Move per-bit design rationale out of slide files → `design-notes.md` (not for slides, not for speaker-notes pane)
- [ ] Brief the designer on the split: **Visual** → design it · **Notes (beats / 🔒 / cues)** → speaker-notes pane · section titles → speaker-notes pane only, NOT on the slide · ignore `design-notes.md` — **@you**
- [ ] Tell designer: corner progress-ship is on almost every slide (build once as a template) — see `ship-visual-system.md`; and RTL/Hebrew layout for any on-slide text — **@you**
- [ ] **S12 — designer rename only** (snippet already generated): Angular component → `rdWidget`, React component → `Widget` — **@you to relay**

## Content fixes (still worth a session)

- [ ] S21 fear-attribution — text exists, didn't land in run 1; turn into a sharp delivery cue — **@me**
- [ ] S10 (old) "unclear" note resolved by reframe; S13 "unclear" flag addressed via diagram (see Open decisions) — **@me**
- [ ] Bit 1 concrete grab in first 30s — likely satisfied now by S4's giant-controller screenshot; confirm it reads as concrete and not vague — **@me/@you**
- [x] **Bit 1 ran ~1 min even with pauses** — diagnosis: open was short on *stake*, not silence. Added S4 audience-stake beat (🔒 "אולי יש לכם קוד כזה... אני לא בטוח שזה נכון") — lands the skeleton's מסר לקהל that was on no slide. Fixes thin open + seeds the spine. (`bit1.md`, rationale in `design-notes.md`) — **re-time on next run**
## Human story (take 2 — felt thin vs the skeleton)

> Take 2 ran ~25–26 min (target 40 + Q&A, OK to finish early — first talk). Speaker's read: enough *technical* depth; the **human story from the skeleton is what's getting lost.** So the work here is quality, not length — don't pad. Discuss placement, then decide.

- [ ] **Audit where the human story can come back** — the skeleton's [אנושי] beats: CEO conversation (partly on S6), the AI fall (S20, strong), stolen time / 2–3 people in spare time (S24). What else got flattened in the compression to cue-cards? — **@me to draft, @you to react**
- [ ] **Place the "first merge" moment** — currently parked as a Q&A answer in `design-notes.md`. It's warm + on-spine ("seeing other devs use what you built" = momentum/adoption). Chronologically early (~5 yrs ago), so it can't sit in the Bit 4 AI arc. Candidate homes: (a) end of Bit 2 / into Bit 3 — first React components actually shipping; (b) **inside Bit 3** as the warm counterpoint to the mixed-code pain (Bit 3 currently has no human beat). Leaning (b). — **@you to call**
- [ ] Do NOT restore the beats cut for **tone** (silence asymmetry = read as complaint). Those were cut on merit, not length. — **@me note**

## Speaker-provided assets (@you)

- [ ] S4 — screenshot of a real giant AngularJS controller
- [x] S11 — engine-swapped-at-sea ship image
- [ ] S15 — screenshots of repeated copy-paste patterns (old code)
- [ ] S16 — annotated rich table screenshot
- [ ] S17 — composable-vs-Datatable code snippets
- [ ] S18 — annotated real Portainer page (library assembly + refactor bits)
- [ ] S19 / S23 — dashboard screenshot (small, then full-screen)

## Production / polish (separate stream, not content)

- [ ] Better ship graphics + code-snippet graphics
- [ ] pptx export quality
- [ ] Audio: kill the echo
- [ ] Camera framing / background
- [ ] Slide interactivity — **S7: progressive strike** (four options appear plain, strike one-by-one as rejected, `incremental` left standing; NOT pre-struck on load). Fallback if no animation: show all four plain, no strikethrough, end-state highlights `incremental`. Also S16 callouts.

## Rehearsal (@you)

- [ ] Memorize Bit 1 verbatim + the last line; improvise everything else
