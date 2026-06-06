# Designer brief — AngularJS→React migration talk deck

**For:** the graphic designer building the slide deck.
**Source files:** `slides/bit1.md … bit5.md` (one file per "bit" / section), plus `slides/ship-visual-system.md`.
**Talk:** 30–40 min technical talk, spoken in **Hebrew**, ~24 content slides + a wordless closing card.

---

## How to read a slide file

Each slide is one block:

```
## Slide N — <internal title>
- **Visual:** what goes on the slide   ← YOU design this
- **Notes:**
  - 🔒 <Hebrew line>   ← spoken word-for-word; goes in the speaker-notes pane
  - <beat / cue>       ← speaker reminders; speaker-notes pane
  - _Cue:_ <delivery>  ← speaker-notes pane
```

**Three buckets — please keep them separate:**

| In the file | What to do with it |
|---|---|
| **`Visual:`** | Design the slide from this. |
| **`Notes:`** (🔒 lines, beats, `Cue:`) | Drop into the **speaker-notes pane** of that slide. Do **not** put any of it on the slide face. |
| **The `## Slide N — title` header** | Speaker-notes pane only (as a label). **Do NOT render it as a slide title** unless the Visual explicitly asks for a title (most don't — see below). |
| **`design-notes.md`** (separate file) + anything in `todo.md` | Ignore entirely — that's editorial / speaker planning, not slide content. |

---

## Critical rules

1. **No on-slide title by default.** Most slides are an image or one line — a title would compete with it. Only add a title when the `Visual:` line says so.

2. **A `Visual:` line is a _description_, not text to typeset.** Put on the slide only what is **quoted** or marked **"on slide" / "Title (on slide)"**. Everything else in a Visual line is build spec + intent for you — e.g. S20's *"the disproportion is the point"* and S17's *"the volume contrast is the message"* are direction, **not** on-slide copy.

3. **Don't print spoken lines on the slide.** Several slides are deliberately **wordless / image-only** — the speaker says the line aloud. Never copy a 🔒 line onto the slide face. Wordless or near-wordless slides: **S1, S11, finale ship card**; the screenshot/diagram/mockup slides (S4, S15–S20, S23) carry only labels/callouts/the mockup's own content, not prose.

4. **On-slide text is English** (talk is spoken in Hebrew). **No exceptions** — the deck is fully English on-slide, so no RTL layout is needed anywhere. (S20's quote is now spoken aloud, not on the slide.)

5. **The recurring ship** — read `slides/ship-visual-system.md` first. A small **progress ship** sits in the top-right corner of *almost every slide*, its planks filling grey→green as the talk progresses (~half-green by the end). **Build it once as a master/template**, don't redraw per slide. It **drops away on data-dense slides** (notably S23, the full-bleed dashboard). The big ship appears large only on **Slide 1** (all-grey) and the **closing card** (~half-green). Never put words on any ship.

---

## Recently decided — build to these (previously open, now final)

- **S2** — hook lines confirmed: "5 years ago we started moving to React" / "This story has no ending."
- **S9** — **title decided: "While we were in there"**, with "TypeScript + Tailwind" large beneath it.
- **S13** — **data-flow diagram** confirmed (Angular 2-way vs React 1-way). The code-snippet alternative is dropped.
- **S20** — **reshaped, no longer a quote slide.** Two-part visual: a small chat-input mockup showing the prompt *"convert the stacks page to react"* → the resulting **huge git diff** (~+10k/−5k). Lay it out so the size contrast dominates (tiny ask → massive unreviewable PR). The reflective quote is spoken aloud, not on the slide.

## Assets the speaker still owes you

Real screenshots / code snippets for **S4, S15, S16, S17, S18, S19, S20, S23**. Note S20 needs **two** assets: the prompt-UI mockup ("convert the stacks page to react") and the git-diff screenshot (real ~+10k/−5k numbers). S19 = small dashboard (tool view); S23 = same dashboard cropped to the X/Y-components-done metric. (The S11 image and the S12 snippet are already in hand.) Full list in `todo.md` under "Speaker-provided assets." Don't block on these — design the layouts with placeholders.

---

## Status of the deck right now

The slide files were cleaned for handoff: all inline TODOs, "speaker provides" notes, alt-titles, and per-bit design rationale were stripped out (rationale → `design-notes.md`, action items → `todo.md`). So what's left in `slides/*.md` is meant to be taken literally as spec — **per Critical Rule 2, "literally" means the quoted/marked text, not the descriptive prose around it.** The previously-open decisions (S2, S9, S13, S20) are now resolved — see "Recently decided" above.

---

## Suggested skills for the next agent

- **`frontend-design`** — if the next step is producing actual slide mockups / HTML prototypes rather than briefing a human designer.
- **`candlekeep-cloud:candlekeep`** — to ground any further slide-craft questions (titles, text density, visual/speech split) in the talk books. Primary refs: *Giving a 30-Minute Tech Talk*, Anderson's *TED Talks* (the "Working with Designers" section, pp. 100–101).
