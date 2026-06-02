# Bit 4 — Depth and AI (Slides 15–23)

> 8–10 min. The longest bit and the emotional peak. Two sub-arcs: the component library story, then the AI arc (beginning → fall → recovery → light moment).
> Tone: restrained. The fall is real — don't overdramatize, don't under-sell.
> Cards are beats + one cue, never rationale — the "why" lives in the Decisions/Design block below.

## Sub-arc A — The Component Library and the Practice (Slides 15–18)

### Slide 15 — Research

- **Visual:** Screenshots of recurring patterns in the old Angular code — copy-pasted raw tables, repeated form fields — speaker provides
- **Notes:**
  - the method that drove the migration
  - find duplicated patterns → a component for each
  - _Cue:_ general method — NOT one table

### Slide 16 — The table: making the choices

- **Visual:** Screenshot of one rich table from the app, with callouts pointing at each capability — settings/column toggle, sort, filter, pagination, row-select, expand. Pick the table that uses the most of these at once. Callouts ≤4–6 words each. Speaker provides.
- **Notes:**
  - table = worked example; screenshot shows the scope
  - patterns → pick TanStack (headless, we own markup) → design API
  - _Cue:_ "all these needs, one component" = pressure into S17; name TanStack aloud

### Slide 17 — The table: implementation evolution

- **Visual:** Two code blocks side by side — composable usage (left, several pieces assembled per table) vs. `<Datatable columns data />` with a variant like `<ExpandableTable>` (right). ~6–10 lines each, trimmed to show _shape_; the volume contrast is the message. Speaker provides snippets.
- **Notes:**
  - primitives only → copy-paste default = S15 pain, in React
  - ship `Datatable` · keep primitives · `ExpandableTable`
  - _Cue:_ callback to S15 aloud — refactor ≠ translate

### Slide 18 — Migrating a view

- **Visual:** A real Portainer page, with overlays/labels showing which library components it was assembled from (Datatable, form fields, etc.), plus arrows marking the bits that needed refactoring. Speaker picks the page. Speaker provides.
- **Notes:**
  - for years: decompose → refactor gaps → small PRs
  - Copilot later: line-level only; decisions stayed human
  - _Cue:_ enact "migration ≠ translation" — don't assert

## Sub-arc B — The AI Arc (Slides 19–23)

### Slide 19 — The return

- **Visual:** The dashboard screenshot, shown **small** — AJS component count over time, which components to migrate first. A tool. Speaker provides (confirmed available). Same artifact returns full-screen at Slide 23.
- **Notes:**
  - came back, wanted to resume
  - built a dashboard (AJS count, prioritization) — vibe-coded, just a tool
  - started figuring out AI → sets up the fall
  - _Cue:_ let it sit, don't call it "organized" — the fall lands harder

### Slide 20 — The fall (the quote)

- **Visual:** _"נותן להרגיש שהכל אפשרי, רק צריך לשלוח עוד הודעה"_ — full slide, Hebrew, no attribution
- **Notes:**
  - warm setup: rusty, "convert the stack page for me"
  - quote appears → why the ask felt fine
  - _Cue:_ the quote IS the fall; full stop after

### Slide 21 — Looked done. Bugs. Paused.

- **Visual:** "Looked done. Bugs. Paused." — minimal
- **Notes:**
  - looked done · bugs · paused (~2mo ago, now resumed)
  - every bug blamed on the migration → the *fear* paused it
  - boundary: often it genuinely *was* the migration
  - _Cue:_ state, don't dramatize — no victim

### Slide 22 — The method

- **Visual:** Framing line ("Working with AI emphasized the fundamentals — it didn't replace them"), with the principles small beneath: plan → tasks → small units · YAGNI · bottom-up. No diagram.
- **Notes:**
  - AI raises the stakes on the basics — volume wherever you point it
  - mirror of S18: AI executes the units you used to type
  - you plan/decompose one layer up; it does the unit
  - _Cue:_ not "magic," not "burned me"; let "bottom-up" resonate

### Slide 23 — The dashboard, full-screen (the 50%)

- **Visual:** The same dashboard from Slide 19, now **full-screen**, focused on the ~50%. Speaker provides. **No corner ship here** — the motif drops away so the dashboard goes full-bleed. The break is the signal: this slide is real, not metaphor. (Data-dense slides drop the corner ship generally; see `ship-visual-system.md`.)
- **Notes:**
  - the number lands here, with weight
  - still migrating · progressing · learning — ~50% ahead
  - _Cue:_ proof of Bit 1's "no ending" — let it sit
- **→ Bridge to Bit 5 (improvised):** _let the ~50% sit._ Then forward: half the road's still ahead → less about the path behind, more about how I walk the rest → S24.
  - _Cue:_ forward on purpose — pre-empts regret; don't name the two halves

---

## Decisions So Far (this session)

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

## Open / To Discuss

- **Slide 18 visual:** pick a real Portainer page that cleanly shows library-assembly + a refactored bit. Speaker provides.
- Gather speaker-provided visuals: 15 (patterns), 16 (annotated table), 17 (code snippets), 18 (annotated view), 19+23 (dashboard — small, then full-screen).
- **Bit 1:** keep a concrete grab in the first 30s now that the number's gone (messy old code / "started years ago, still going") so the lighter open doesn't go vague.
- Then: Bit 5 (closing) — lands on the honest answer (skeleton line 134–138). Still homeless: [אנושי] moments removed from Bit 3 (silence asymmetry, stolen time); freed-up "first merge" moment.
