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

1. **No on-slide title by default.** Most slides are an image or one line — a title would compete with it. Only add a title when the `Visual:` line says so. (One slide, **S9**, is an open question — see below.)

2. **Don't print spoken lines on the slide.** Several slides are deliberately **wordless / image-only** — the speaker says the line aloud. Never copy a 🔒 line onto the slide face. Wordless or near-wordless slides: **S1, S11, finale ship card**, and the screenshot/diagram slides (S4, S15–S19, S23) carry only labels/callouts, not prose.

3. **On-slide text is English** (talk is spoken in Hebrew). **One exception, still open: S20** — a Hebrew quote may stay Hebrew. Treat S20 as TBD until the speaker confirms (see open items). No RTL layout needed for anything else.

4. **The recurring ship** — read `slides/ship-visual-system.md` first. A small **progress ship** sits in the top-right corner of *almost every slide*, its planks filling grey→green as the talk progresses (~half-green by the end). **Build it once as a master/template**, don't redraw per slide. It **drops away on data-dense slides** (notably S23, the full-bleed dashboard). The big ship appears large only on **Slide 1** (all-grey) and the **closing card** (~half-green). Never put words on any ship.

---

## Open decisions that affect your work (speaker to resolve — see `todo.md`)

- **S2** — the two hook lines are set ("5 years ago we started moving to React" / "This story has no ending") but the speaker may reword. Confirm before finalizing.
- **S9** — likely needs a **title** (the visual "TypeScript + Tailwind" is too thin alone). Candidate titles pending speaker pick. Don't finalize this slide yet.
- **S13** — visual resolved to a **data-flow diagram** (Angular 2-way vs React 1-way); a code-snippet alternative is still on the table. Confirm before building.
- **S20** — Hebrew vs English (above).

## Assets the speaker still owes you

Real screenshots / code snippets for **S4, S11, S12, S15, S16, S17, S18, S19/S23**. Full list in `todo.md` under "Speaker-provided assets." Don't block on these — design the layouts with placeholders.

---

## Status of the deck right now

The slide files were just cleaned for handoff: all inline TODOs, "speaker provides" notes, alt-titles, and per-bit design rationale were stripped out (rationale → `design-notes.md`, action items → `todo.md`). So what's left in `slides/*.md` is meant to be taken literally as spec — with the four open decisions above flagged.

---

## Suggested skills for the next agent

- **`frontend-design`** — if the next step is producing actual slide mockups / HTML prototypes rather than briefing a human designer.
- **`candlekeep-cloud:candlekeep`** — to ground any further slide-craft questions (titles, text density, visual/speech split) in the talk books. Primary refs: *Giving a 30-Minute Tech Talk*, Anderson's *TED Talks* (the "Working with Designers" section, pp. 100–101).
