# Bit 2 — The Decisions (Slides 5–10)

> 4–5 min. Cards are beats + one cue, never rationale — the "why" lives in Design notes below.
> 🔒 = learned word-for-word. Cues are glance-only, never spoken.

## Slide 5 — Why it had to change

- **Visual:**
  - Title (on slide): **Why it had to change**
  - Three lines: _dead library · refactor needed anyway · new features coming_
- **Notes:**
  - 🔒 seam from Bit 1: _"וזה לא נגמר בבלגן"_ (it wasn't only the mess)
  - EOL = trigger, not the whole case (Dec 2021)
  - migration legitimized the refactor (couldn't earn it alone)
  - _Cue:_ escalation off Bit 1 — not a restart

## Slide 6 — How it was decided

- **Visual:**
  - Title (on slide): **How it was decided**
  - Flow: Internal discussions → Frontend team meeting → React
- **Notes:**
  - leadership layer: "can't hire" for AngularJS
  - team layer: ecosystem · familiarity · ownership
  - _Cue:_ land "decided together, not top-down"

## Slide 7 — The options

- **Visual:**
  - Title (on slide): **The options**
  - Four items, each on its own line — this is the on-slide text:
    - rewrite from zero
    - micro-frontends
    - do nothing
    - incremental
  - **Build behavior (NOT on-slide text — this is an instruction):** all four appear plain on load; strike each through one at a time as the speaker rejects it; `incremental` is the only one left unstruck. **Do not show any strikethrough on load** — the strike happens live, synced to delivery.
- **Notes:**
  - reqs: keep shipping · don't freeze dev · don't fragment state/nav
  - do-nothing → lib dead · rewrite → freezes delivery · micro-frontends → fragments state/nav · incremental → meets all
  - _Cue:_ strike each → name what it fails

## Slide 8 — Why incremental + r2a

- **Visual:** Angular box ← r2a → React box, arrow labeled "new components flow one way"
- **Notes:**
  - r2a = simplest fit · new features in React from day one
  - React components run inside Angular → kills most dual-maintenance
  - _Cue:_ don't open the pain yet (→ Bit 3)

## Slide 9 — What the migration justified

- **Visual:**
  - Title (on slide): **While we were in there**
  - "TypeScript + Tailwind" large, clean
- **Notes:**
  - migration = cover for improvements that couldn't justify themselves alone
  - TS + Tailwind, merged in the first PRs
  - grace note: I argued against TypeScript; we did it anyway; far easier now
  - _Cue:_ "I was against it" — aside, don't sell

## Slide 10 — Same surface, new engine

- **Visual:** Title alone: "Same surface. New engine underneath."
- **Notes:**
  - a decision, not a regret
  - same UX, rebuilt underneath
  - why: no mandate to change UX · new surface muddies attribution (regression vs redesign)
  - behavior-preserving, still a full refactor — not a translation
  - _Cue / bridge → Bit 3:_ same ship, swap the engine

_(Design rationale for this bit → `design-notes.md`.)_
