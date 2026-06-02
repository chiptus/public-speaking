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
- [ ] **S2 on-slide lines** — I set them to _"לפני 5 שנים התחלנו לעבור ל-React"_ / _"זה לא סיפור עם סוף"_ to make the visual designer-ready. Confirm/adjust the wording — it's your hook. — **@you**
- [ ] **S13 visual** — resolved the old "or" to a **data-flow diagram** (Angular ↔ 2-way vs React → 1-way). Alternative was the `scope.$evalAsync` wrapper snippet. Pick one. — **@you to call**
- [ ] **S9 needs a title** — "TypeScript + Tailwind" alone is a label, doesn't state the point. Add a title that carries the idea (the visual can't): candidates _"What we added to the mix"_ / _"What we got from the migration"_ / _"What the migration justified"_ (= the section name). This is the one slide where a title clearly earns its place. — **@you to pick**
- [x] **On-slide text language** — decided: **all on-slide text in English**, except the S20 quote (see below). S2 + S10 converted. Tell the designer the deck is English text / Hebrew spoken. — **@you to brief designer**
- [ ] **S20 — keep the fall quote Hebrew?** Leaning yes: it's a verbatim quote actually said in Hebrew, and the emotional low point — translating it weakens it and misrepresents it. Would be the one deliberate Hebrew slide (a visual break, like the corner-ship dropping on S23). Needs more thought. — **@you to call**

## Designer handoff

- [x] Strip inline TODOs / "speaker provides" / alt-titles from `slides/bitN.md` — moved here / removed
- [x] Move per-bit design rationale out of slide files → `design-notes.md` (not for slides, not for speaker-notes pane)
- [ ] Brief the designer on the split: **Visual** → design it · **Notes (beats / 🔒 / cues)** → speaker-notes pane · section titles → speaker-notes pane only, NOT on the slide · ignore `design-notes.md` — **@you**
- [ ] Tell designer: corner progress-ship is on almost every slide (build once as a template) — see `ship-visual-system.md`; and RTL/Hebrew layout for any on-slide text — **@you**

## Content fixes (still worth a session)

- [ ] S21 fear-attribution — text exists, didn't land in run 1; turn into a sharp delivery cue — **@me**
- [ ] S10 (old) "unclear" note resolved by reframe; S13 "unclear" flag addressed via diagram (see Open decisions) — **@me**
- [ ] Bit 1 concrete grab in first 30s — likely satisfied now by S4's giant-controller screenshot; confirm it reads as concrete and not vague — **@me/@you**
- [x] Homeless beats (from old Bit 4 notes): [אנושי] moments cut from Bit 3 (silence asymmetry, stolen time) + freed-up "first merge" moment — find a home or retire. "First merge" currently parked as a Q&A answer in `design-notes.md` — **@me**

## Speaker-provided assets (@you)

- [ ] S4 — screenshot of a real giant AngularJS controller
- [x] S11 — engine-swapped-at-sea ship image
- [ ] S12 — ng-transclude vs children-prop snippet
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
- [ ] Slide interactivity (e.g. S7 strike-through options, S16)

## Rehearsal (@you)

- [ ] Memorize Bit 1 verbatim + the last line; improvise everything else
