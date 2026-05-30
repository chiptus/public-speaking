# Bit 4 — Depth and AI (Slides 15–24)

> 8–10 min. The longest bit and the emotional peak. Two sub-arcs: the component library story, then the AI arc (beginning → fall → recovery → light moment).
> Tone: restrained. The fall is real — don't overdramatize, don't under-sell.

## Sub-arc A — The Component Library (Slides 15–18)

### Slide 15 — Research

- **Visual:** Screenshots of recurring patterns in the old Angular code — copy-pasted raw tables, repeated form fields — speaker provides
- **Notes:** The method that drove the migration. Find the patterns developers were already duplicating, build a component for each. NOT about one table — about systematically finding patterns.

### Slide 16 — The table: making the choices

- **Visual:** Screenshot of one rich table from the app, with callouts pointing at each capability — settings/column toggle, sort, filter, pagination, row-select, expand. Pick the table that uses the most of these at once. Callouts ≤4–6 words each. Speaker provides.
- **Notes:** The table as the worked example. The screenshot *shows* the scope of needs. Said verbally over it: this drove the choices — research which table patterns we had → choose the library (TanStack Table, headless, we own the markup) → design the right API. "All these needs in one component" is the pressure that sets up Slide 17. TanStack named verbally, not drawn.

### Slide 17 — The table: implementation evolution

- **Visual:** Two code blocks side by side — composable usage (left, several pieces assembled per table) vs. `<Datatable columns data />` with a variant like `<ExpandableTable>` (right). ~6–10 lines each, trimmed to show *shape*; the volume contrast is the message. Speaker provides snippets.
- **Notes:** The lesson, not "wrong → right": you need the primitives, but shipping *only* primitives makes devs copy-paste the default composition every time — recreating the exact copy-paste pain from Slide 15, now in React. So you provide the default (`Datatable`) for them, keep primitives for the cases that need them, `ExpandableTable` as a variant. Say the Slide 15 callback out loud. This IS refactor-not-translate — sets up Slide 18.

### Slide 18 — Migration ≠ translation

- **Visual:** "Migration is a refactor. Not a line-by-line translation." — large, centered
- **Notes:** The principle/payoff. Migrating a page = assembling from the library + refactoring, not translating Angular line-by-line. Seeds the AI arc (skipping this principle causes the fall).

## Sub-arc B — The AI Arc (Slides 19–24)

### Slide 19 — Copilot as converter

- **Visual:** Angular → React arrow, Copilot label
- **Notes:** The beginning, ~4 yrs ago (Copilot, ~mid-2022). AI handles the technical conversion; judgment (what to refactor, what's worth building) stays with the developer. This respected the principle from Slide 18 — and it worked.

### Slide 20 — The return

- **Visual:** The dashboard screenshot, shown **small** — AJS component count over time, which components to migrate first. A tool. Speaker provides (confirmed available). Same artifact returns full-screen at Slide 24.
- **Notes:** Came back after a break, wanted to resume the migration. Built a dashboard to track it (AJS components over time, prioritization) — mostly vibe-coded; it's a tool to know where things stand, NOT a disciplined "measurement" beat. Started figuring out how to work with the new AI capabilities. Ends on that — sets up the fall. (You're shown organized here — let the dashboard sit, don't say it; it makes the fall land harder. The small-now / full-screen-later contrast sets up the closing payoff.)

### Slide 21 — The fall (the quote)

- **Visual:** *"נותן להרגיש שהכל אפשרי, רק צריך לשלוח עוד הודעה"* — full slide, Hebrew, no attribution
- **Notes:** The quote IS the fall — the feeling and the action are one moment. Warm verbal setup: came back rusty, just told it "convert the stack page for me." Then the slide appears; the quote explains why the ask felt fine. Full stop after it lands.

### Slide 22 — Looked done. Bugs. Paused.

- **Visual:** "Looked done. Bugs. Paused." — minimal
- **Notes:** Don't dramatize. It looked finished — it wasn't. Bugs → project paused (~2 months ago), recently resumed. State it.

### Slide 23 — The method

- **Visual:** Framing line ("Working with AI emphasized the fundamentals — it didn't replace them"), with the principles small beneath: plan → tasks → small units · YAGNI · bottom-up. No diagram.
- **Notes:** The payoff of the arc, and the honest takeaway — not "AI is magic," not "AI burned me," but: AI raises the stakes on the basics, because it generates volume in whatever direction you point it. Apply the principles *one layer up* — you plan and decompose, it executes the small unit. "Bottom-up" quietly echoes sub-arc A (primitives → `Datatable`) and the talk's central message; let it resonate, don't state it.

### Slide 24 — The dashboard, full-screen (the 50%)

- **Visual:** The same dashboard from Slide 20, now **full-screen**, focused on the ~50%. Speaker provides.
- **Notes:** The closing image of the bit — the number lands here, with weight, because the audience has earned it (met the dashboard small on the Return, now sees the verdict). Said over it: still migrating, still progressing, still learning, ~50% still ahead. This is the *proof* of Bit 1's claim ("a story without an end") — theme planted at the open, evidence delivered here. The number now lives in Bit 4, NOT the opening and NOT Bit 5's close (Bit 5 lands on the honest answer instead).

---

## Decisions So Far (this session)

- Sub-arc A reframed from "the table story" → **"building a component library"** (table-only felt too lean). Research → find patterns (tables, form fields) → build components → shared library.
- Slide 15 titled "Research" — about the *general* method, not one artifact. Visual = screenshots of old copy-pasted patterns.
- **The table is the worked example, split across two slides (option B):** 16 = the choices (pattern research → TanStack Table → API design), 17 = implementation evolution (composable components → `Datatable` + variants like `ExpandableTable`). "Migration ≠ translation" moved to 18.
- **Sub-arc B restructured to 6 slides (19–24); bit is now 10 slides (15–24):**
  - Dropped the "Skipping patience" slogan slide entirely — too neat / "selling the story back."
  - The quote IS the fall (feeling + action are one moment); collapsed into a single slide (21).
  - Dashboard moved *before* the fall, to a new **Return** slide (20) — it's a tool built on re-entry, not the disciplined "measurement" beat it was miscast as.
  - Method slide (23) reframed: AI *emphasizes* the fundamentals (plan → tasks → small units · YAGNI · bottom-up), doesn't replace them — the honest takeaway of the arc.
  - Quote intro resolved: **warm** verbal setup ("convert the stack page for me") → slide.
  - Dropped the "first merge" light-moment slide — it happened ~5 yrs ago (near the start), so it can't sit at the end of the AI arc chronologically. Freed up — possible reuse in Bit 5.
  - Copilot beginning dated ~4 yrs ago (mid-2022), per Slide 19.
- **The number moved (skeleton updated, bits 1/4/5):** Bit 1 opens with the *theme* only — "a story without an end," no number. The **dashboard carries the number**: small/tool on the Return (20), **full-screen at the bit close (24) where the ~50% lands with earned weight.** Bit 5 no longer closes on the number — it lands on the honest answer ("would you move to React today?"). Rationale: theme-then-proof beats a repeated bookend; an abstract stat at the open becomes a number the audience understands the cost of by the end.

## Open / To Discuss

- Gather speaker-provided visuals: 15 (patterns), 16 (annotated table), 17 (code snippets), 20+24 (dashboard — small, then full-screen).
- **Bit 1:** keep a concrete grab in the first 30s now that the number's gone (messy old code / "started years ago, still going") so the lighter open doesn't go vague.
- Then: Bit 5 (closing) — lands on the honest answer (skeleton line 134–138). Still homeless: [אנושי] moments removed from Bit 3 (silence asymmetry, stolen time); freed-up "first merge" moment.
