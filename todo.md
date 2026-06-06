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

- [x] Slide 24 split — **decided: one slide, two halves.** The two-half structure carries the at-a-glance contrast; splitting breaks it and pads the close.
- [x] **S2 on-slide lines** — I set them to _"לפני 5 שנים התחלנו לעבור ל-React"_ / _"זה לא סיפור עם סוף"_ to make the visual designer-ready. Confirm/adjust the wording — it's your hook. — **@you**
- [x] **S13 visual** — **decided: keep the data-flow diagram** (Angular ↔ 2-way vs React → 1-way). It read fine in take 2; the issue was pacing (spent too long on it), not the visual. A little natural dwell here is OK given the speaker runs fast.
- [x] **S9 title — decided: "While we were in there"** (understated, opportunistic; lets "TypeScript + Tailwind" carry the point without announcing the moral). Set in `bit2.md`; designer unblocked.
- [x] **On-slide text language** — decided: **all on-slide text in English** (S20 now English too — no exceptions). S2 + S10 converted. Tell the designer the deck is English text / Hebrew spoken. — **@you to brief designer**
- [x] **S20 language — decided: English** (translated). Deck is fully English on-slide now; no deliberate-Hebrew exception. Set in `bit4.md`. Wording: _"It makes you feel anything's possible — you just have to send one more message."_
- [x] **S20 floating quote — resolved by reshaping the fall** (2026-06-06). S20 is now "the ask," not "the quote": visual = prompt _"convert the stacks page to react"_ → huge diff (~+10k/−5k); **quote moves to spoken.** S19 keeps the small dashboard but its notes now end on the AI turn, so S20's ask is the immediate consequence. Dashboard shown twice = different facets (S19 tool · S23 cropped to X/Y-done). All set in `bit4.md`; rationale in `design-notes.md`.

## Designer handoff

- [x] Strip inline TODOs / "speaker provides" / alt-titles from `slides/bitN.md` — moved here / removed
- [x] Move per-bit design rationale out of slide files → `design-notes.md` (not for slides, not for speaker-notes pane)
- [x] Brief the designer on the split: **Visual** → design it · **Notes (beats / 🔒 / cues)** → speaker-notes pane · section titles → speaker-notes pane only, NOT on the slide · ignore `design-notes.md` — **@you**
- [x] Tell designer: corner progress-ship is on almost every slide (build once as a template) — see `ship-visual-system.md`; and RTL/Hebrew layout for any on-slide text — **@you**
- [x] **S12 — designer rename only** (snippet already generated): Angular component → `rdWidget`, React component → `Widget` — **@you to relay**

## Content fixes (still worth a session)

- [ ] S21 fear-attribution — text exists, didn't land in run 1; turn into a sharp delivery cue — **@me**
- [ ] S10 (old) "unclear" note resolved by reframe; S13 "unclear" flag addressed via diagram (see Open decisions) — **@me**
- [ ] Bit 1 concrete grab in first 30s — likely satisfied now by S4's giant-controller screenshot; confirm it reads as concrete and not vague — **@me/@you**
- [x] **Bit 1 ran ~1 min even with pauses** — diagnosis: open was short on _stake_, not silence. Added S4 audience-stake beat (🔒 "אולי יש לכם קוד כזה... אני לא בטוח שזה נכון") — lands the skeleton's מסר לקהל that was on no slide. Fixes thin open + seeds the spine. (`bit1.md`, rationale in `design-notes.md`) — **re-time on next run**

## Human story (take 2 — felt thin vs the skeleton)

> Take 2 ran ~25–26 min (target 40 + Q&A, OK to finish early — first talk). Speaker's read: enough _technical_ depth; the **human story from the skeleton is what's getting lost.** So the work here is quality, not length — don't pad. Discuss placement, then decide.

- [ ] **Audit where the human story can come back** — the skeleton's [אנושי] beats: CEO conversation (partly on S6), the AI fall (S20, strong), stolen time / 2–3 people in spare time (S24). What else got flattened in the compression to cue-cards? — **@me to draft, @you to react**
- [x] **Place the "first merge" moment** — **decided: S10→S11 seam, as the opening spoken beat of S11** (in `bit3.md` S11 Notes). Framed as the _payoff of the Bit 2 decisions_ (first React components shipped, another dev built on them = momentum), then pivots straight into the mixed-code pain — warm → hard in one move. Not on the slide, not a dwell; S11 visual stays wordless.
- [ ] Do NOT restore the beats cut for **tone** (silence asymmetry = read as complaint). Those were cut on merit, not length. — **@me note**

## Speaker-provided assets (@you)

- [ ] S4 — screenshot of a real giant AngularJS controller
- [x] S11 — engine-swapped-at-sea ship image
- [ ] S15 — screenshots of repeated copy-paste patterns (old code)
- [ ] S16 — annotated rich table screenshot
- [ ] S17 — composable-vs-Datatable code snippets
- [ ] S18 — annotated real Portainer page (library assembly + refactor bits)
- [ ] S19 — dashboard screenshot (small; the tool view — AJS count over time / prioritization)
- [ ] S23 — same dashboard, **cropped to the X/Y-components-done metric** (the ~50%), full-screen
- [ ] **S20 — two new assets:** (a) prompt-UI screenshot/mockup showing _"convert the stacks page to react"_ · (b) the git-diff screenshot from that PR (the real ~+10k/−5k numbers)

## Production / polish (separate stream, not content)

- [ ] Better ship graphics + code-snippet graphics
- [ ] pptx export quality
- [ ] Audio: kill the echo
- [ ] Camera framing / background
- [ ] Slide interactivity — **S7: progressive strike** (four options appear plain, strike one-by-one as rejected, `incremental` left standing; NOT pre-struck on load). Fallback if no animation: show all four plain, no strikethrough, end-state highlights `incremental`. Also S16 callouts.

## Rehearsal (@you)

- [ ] Memorize Bit 1 verbatim + the last line; improvise everything else
