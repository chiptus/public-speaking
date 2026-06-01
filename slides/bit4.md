# Bit 4 — Depth and AI (Slides 15–23)

> 8–10 min. The longest bit and the emotional peak. Two sub-arcs: the component library story, then the AI arc (beginning → fall → recovery → light moment).
> Tone: restrained. The fall is real — don't overdramatize, don't under-sell.

## Sub-arc A — The Component Library and the Practice (Slides 15–18)

### Slide 15 — Research

- **Visual:** Screenshots of recurring patterns in the old Angular code — copy-pasted raw tables, repeated form fields — speaker provides
- **Notes:** The method that drove the migration. Find the patterns developers were already duplicating, build a component for each. NOT about one table — about systematically finding patterns.

### Slide 16 — The table: making the choices

- **Visual:** Screenshot of one rich table from the app, with callouts pointing at each capability — settings/column toggle, sort, filter, pagination, row-select, expand. Pick the table that uses the most of these at once. Callouts ≤4–6 words each. Speaker provides.
- **Notes:** The table as the worked example. The screenshot _shows_ the scope of needs. Said verbally over it: this drove the choices — research which table patterns we had → choose the library (TanStack Table, headless, we own the markup) → design the right API. "All these needs in one component" is the pressure that sets up Slide 17. TanStack named verbally, not drawn.

### Slide 17 — The table: implementation evolution

- **Visual:** Two code blocks side by side — composable usage (left, several pieces assembled per table) vs. `<Datatable columns data />` with a variant like `<ExpandableTable>` (right). ~6–10 lines each, trimmed to show _shape_; the volume contrast is the message. Speaker provides snippets.
- **Notes:** The lesson, not "wrong → right": you need the primitives, but shipping _only_ primitives makes devs copy-paste the default composition every time — recreating the exact copy-paste pain from Slide 15, now in React. So you provide the default (`Datatable`) for them, keep primitives for the cases that need them, `ExpandableTable` as a variant. Say the Slide 15 callback out loud. This IS refactor-not-translate — sets up Slide 18.

### Slide 18 — Migrating a view

- **Visual:** A real Portainer page, with overlays/labels showing which library components it was assembled from (Datatable, form fields, etc.), plus arrows marking the bits that needed refactoring. Speaker picks the page. Speaker provides.
- **Notes:** The practical payoff of the library — and "migration ≠ translation" _enacted_, not asserted. The way for years: decompose the view into components → refactor the gaps → ship in small PRs. **Copilot was added later** and helped at the line level (the typing), but decomposition and refactor decisions stayed with the developer. This is the practice that the AI arc both abandons (the fall) and returns to (the method).

## Sub-arc B — The AI Arc (Slides 19–23)

### Slide 19 — The return

- **Visual:** The dashboard screenshot, shown **small** — AJS component count over time, which components to migrate first. A tool. Speaker provides (confirmed available). Same artifact returns full-screen at Slide 23.
- **Notes:** Came back after a break, wanted to resume the migration. Built a dashboard to track it (AJS components over time, prioritization) — mostly vibe-coded; it's a tool to know where things stand, NOT a disciplined "measurement" beat. Started figuring out how to work with the new AI capabilities. Ends on that — sets up the fall. (You're shown organized here — let the dashboard sit, don't say it; it makes the fall land harder. The small-now / full-screen-later contrast sets up the closing payoff.)

### Slide 20 — The fall (the quote)

- **Visual:** _"נותן להרגיש שהכל אפשרי, רק צריך לשלוח עוד הודעה"_ — full slide, Hebrew, no attribution
- **Notes:** The quote IS the fall — the feeling and the action are one moment. Warm verbal setup: came back rusty, just told it "convert the stack page for me." Then the slide appears; the quote explains why the ask felt fine. Full stop after it lands.

### Slide 21 — Looked done. Bugs. Paused.

- **Visual:** "Looked done. Bugs. Paused." — minimal
- **Notes:** Don't dramatize. It looked finished — it wasn't. Bugs → project paused (~2 months ago), recently resumed. State it. **The attribution beat (spoken, no taxonomy):** in a long migration every bug gets blamed on the migration, and a bug pinned on it carries more fear than the same bug would otherwise — that fear, not the bug alone, is what paused the project. Keep it honest with a boundary: there's no clean "they blamed us unfairly" story — when it broke, it was often genuinely the migration. Vulnerability with a limit, no victim narrative. _(This is the earned home for the "the migration didn't create the mess, it exposed it" idea that was cut from the Bit 1 open — same thought, lands here where the audience has lived it. Optional to voice; don't force it.)_

### Slide 22 — The method

- **Visual:** Framing line ("Working with AI emphasized the fundamentals — it didn't replace them"), with the principles small beneath: plan → tasks → small units · YAGNI · bottom-up. No diagram.
- **Notes:** The payoff of the arc, and the honest takeaway — not "AI is magic," not "AI burned me," but: AI raises the stakes on the basics, because it generates volume in whatever direction you point it. **Direct mirror of Slide 18:** same view-migration practice (decompose → refactor → small units), AI now executes the units you used to type. Apply the principles _one layer up_ — you plan and decompose, it does the unit. "Bottom-up" quietly echoes sub-arc A (primitives → `Datatable`) and the talk's central message; let it resonate, don't state it.

### Slide 23 — The dashboard, full-screen (the 50%)

- **Visual:** The same dashboard from Slide 19, now **full-screen**, focused on the ~50%. Speaker provides. **No corner ship here** — the motif drops away so the dashboard goes full-bleed. The break is the signal: this slide is real, not metaphor. (Data-dense slides drop the corner ship generally; 23 is the clearest case — see `ship-visual-system.md`.)
- **Notes:** The closing image of the bit — the number lands here, with weight, because the audience has earned it (met the dashboard small on the Return, now sees the verdict). Said over it: still migrating, still progressing, still learning, ~50% still ahead. This is the _proof_ of Bit 1's claim ("a story without an end") — theme planted at the open, evidence delivered here. The number now lives in Bit 4, NOT the opening and NOT Bit 5's close (Bit 5 lands on the honest answer instead).

---

## Decisions So Far (this session)

- Sub-arc A reframed from "the table story" → **"building a component library"** (table-only felt too lean). Research → find patterns (tables, form fields) → build components → shared library.
- Slide 15 titled "Research" — about the _general_ method, not one artifact. Visual = screenshots of old copy-pasted patterns.
- **The table is the worked example, split across two slides (option B):** 16 = the choices (pattern research → TanStack Table → API design), 17 = implementation evolution (composable components → `Datatable` + variants like `ExpandableTable`). "Migration ≠ translation" moved to 18.
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
