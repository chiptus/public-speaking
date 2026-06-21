# AngularJS to React: How to Move a Mountain Incrementally

A 30–40 min technical talk (spoken in Hebrew) on migrating a large product (Portainer) off AngularJS to React incrementally — over five years, while still shipping features.

**Spine:** you're not stuck with legacy code — you can migrate it incrementally while you keep shipping, as long as you're honest that it's a multi-year campaign, not a sprint.

## Where the talk lives

The canonical source is the per-slide files in `slides/`, **not** the original skeleton.

```
slides/
├── bit1.md … bit5.md        # the deck, one file per section ("bit")
│                            #   each slide = Visual (for designer) + Notes (🔒 verbatim / Speak / Cue)
└── ship-visual-system.md    # the recurring Ship-of-Theseus motif (color-fill progress)

design-notes.md      # the editorial "why" behind each bit — kept out of slide files
designer-handoff.md  # brief for the graphic designer (how to read a slide file)
rehearsal.md         # what to memorize verbatim vs. improv off cues; time budget
todo.md              # revision log + open items (locked direction, takeaway, strategy)
migration-talk-skeleton.md   # ⚠️ FROZEN original outline — do NOT rehearse from it
```

### Reading order for a newcomer

1. `slides/bit1.md`–`bit5.md` — the actual talk, content + visual per slide
2. `slides/ship-visual-system.md` — the recurring visual metaphor
3. `design-notes.md` — the reasoning behind the choices
4. `rehearsal.md` — how to practice it

> ⚠️ `migration-talk-skeleton.md` is a **frozen** snapshot of the first outline. It no longer matches the current deck (code-first open, the takeaway, components-not-lines, etc.). Kept for history only.

## Assets

- `slides/` — markdown source of the deck
- `ships/` — the Ship-of-Theseus illustrations (progress states + engine + diff)
- `screenshots/` — real product screenshots used in slides (e.g. the migration dashboard)
- `takes/` — rehearsal recordings and transcripts (`.mp4` git-ignored, `.txt` tracked)
- `final slideshow/` — the built deck (standalone HTML) + the design-system PPTX

## The five bits

1. **Opening** — the codebase, the ship paradox, the stakes ("5 years, still not done")
2. **The decisions** — why leave AngularJS, why incremental, r2a, what went in early
3. **Living with mixed code** — Angular and React side by side, for years
4. **Depth + AI** — the table story, the AI fall, the dashboard (the 50%)
5. **What's next** — what I'd do differently, and what I'd need

## Working rules (see `CLAUDE.md`)

- No walls of text; depth over cutting (it's a tech talk, not a TED talk).
- Speak the constraints/reasoning; don't announce the moral.
- Primary craft reference: *Giving a 30-Minute Tech Talk* (in `../ck/`).
