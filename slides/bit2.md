# Bit 2 — The Decisions (Slides 5–10)

> 4–5 min. Cards are beats + one cue, never rationale — the "why" lives in Design notes below.
> 🔒 = learned word-for-word. Cues are glance-only, never spoken.

## Slide 5 — Why it had to change

- **Visual:**
  - Title (on slide): **Why it had to change**
  - Three lines: _dead library · refactor needed anyway · new features coming_
- **Notes:**
  - 🔒 seam from Bit 1: _"וזה לא נגמר בבלגן"_ (it wasn't only the mess)
  - EOL = the trigger, not the whole case (Dec 2021)
  - migration gave refactoring the legitimacy it couldn't earn alone
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
  - the requirements behind the cut — explicit: keep shipping features · implicit: don't freeze dev, don't fragment state/nav
  - strike each against a requirement: do-nothing = library is dead · rewrite = freezes feature delivery · micro-frontends = fragments state/nav/components · incremental = the only one that meets all
  - _Cue:_ strike each as you reject it — name the requirement it fails

## Slide 8 — Why incremental + r2a

- **Visual:** Angular box ← r2a → React box, arrow labeled "new components flow one way"
- **Notes:**
  - r2a = simplest fit · new features in React from day one
  - React components run inside Angular → kills most dual-maintenance
  - _Cue:_ exceptions belong to Bit 3 — don't open mixed-code pain here

## Slide 9 — What the migration justified

- **Visual:**
  - Title (on slide): **TBD** — slide needs a title, wording not yet decided (see `todo.md` → Open decisions, "S9 needs a title")
  - "TypeScript + Tailwind" large, clean
- **Notes:**
  - migration = cover for improvements that couldn't justify themselves alone
  - TS + Tailwind, merged in the first PRs
  - grace note: I argued against TypeScript; we did it anyway; far easier now
  - _Cue:_ "I was against it" = small aside, not a confession — don't sell it

## Slide 10 — Same surface, new engine

- **Visual:** Title alone: "Same surface. New engine underneath."
- **Notes:**
  - a decision, not a regret
  - held the UX identical, rebuilt the code beneath
  - why: no product mandate to change UX · changing the surface muddies attribution (can't tell regression from redesign)
  - behavior-preserving, still a full refactor — not a translation
  - _Cue / bridge → Bit 3:_ same ship, swap the engine

_(Design rationale for this bit → `design-notes.md`.)_
