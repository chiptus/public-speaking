# Bit 4 — Depth and AI (Slides 15–23)

> 8–10 min. The longest bit and the emotional peak. Two sub-arcs: the component library story, then the AI arc (beginning → fall → recovery → light moment).
> Tone: restrained. The fall is real — don't overdramatize, don't under-sell.
> Cards are beats + one cue, never rationale — the "why" lives in the Decisions/Design block below.

## Sub-arc A — The Component Library and the Practice (Slides 15–18)

### Slide 15 — Research

- **Visual:**
  - Title (on slide): **Research**
  - Screenshots of recurring patterns in the old Angular code — copy-pasted raw tables, repeated form fields
- **Notes:**
  - the method that drove the migration
  - find duplicated patterns → a component for each
  - _Cue:_ general method — NOT one table

### Slide 16 — The table: making the choices

- **Visual:** Screenshot of one rich table from the app, with callouts pointing at each capability — settings/column toggle, sort, filter, pagination, row-select, expand. Pick the table that uses the most of these at once. Callouts ≤4–6 words each.
- **Notes:**
  - table = worked example; screenshot shows the scope
  - patterns → pick TanStack (headless, we own markup) → design API
  - _Cue:_ say "TanStack" aloud → pressure into S17

### Slide 17 — The table: implementation evolution

- **Visual:** Two code blocks side by side — composable usage (left, several pieces assembled per table) vs. `<Datatable columns data />` with a variant like `<ExpandableTable>` (right). ~6–10 lines each, trimmed to show _shape_; the volume contrast is the message.
- **Notes:**
  - primitives only → copy-paste default = S15 pain, in React
  - ship `Datatable` · keep primitives · `ExpandableTable`
  - _Cue:_ callback to S15 aloud — refactor ≠ translate

### Slide 18 — Migrating a view

- **Visual:**
  - Title (on slide): **Migrating a view**
  - A real Portainer page, with overlays/labels showing which library components it was assembled from (Datatable, form fields, etc.), plus arrows marking the bits that needed refactoring.
- **Notes:**
  - for years: decompose → refactor gaps → small PRs
  - Copilot later: line-level only; decisions stayed human
  - _Cue:_ enact "migration ≠ translation" — don't assert

## Sub-arc B — The AI Arc (Slides 19–23)

### Slide 19 — The return

- **Visual:**
  - Title (on slide): **The return**
  - The dashboard screenshot, shown **small** — AJS component count over time, which components to migrate first. A tool. Same artifact returns full-screen at Slide 23.
- **Notes:**
  - came back, wanted to resume
  - built a dashboard (AJS count, prioritization) — vibe-coded, just a tool
  - started figuring out AI → sets up the fall
  - _Cue:_ let it sit — don't call it "organized"

### Slide 20 — The fall (the quote)

- **Visual:** _"It makes you feel anything's possible — you just have to send one more message."_ — full slide, English, no attribution
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
  - _Cue:_ not magic / not burned — land "bottom-up"

### Slide 23 — The dashboard, full-screen (the 50%)

- **Visual:** The same dashboard from Slide 19, now **full-screen**, focused on the ~50%. **No corner ship here** — the motif drops away so the dashboard goes full-bleed. The break is the signal: this slide is real, not metaphor. (Data-dense slides drop the corner ship generally; see `ship-visual-system.md`.)
- **Notes:**
  - the number lands here, with weight
  - still migrating · progressing · learning — ~50% ahead
  - _Cue:_ proof of Bit 1's "no ending" — let it sit
- **→ Bridge to Bit 5 (improvised):** _let the ~50% sit._ Then forward: half the road's still ahead → less about the path behind, more about how I walk the rest → S24.
  - _Cue:_ forward — don't name the two halves

---

_(Design rationale + session decisions for this bit → `design-notes.md`. Open action items → `todo.md`.)_
