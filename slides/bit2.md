# Bit 2 — The Decisions (Slides 5–10)

## Slide 5 — Why it had to change

- **Visual:** Three lines: _dead library · refactor needed anyway · new features coming_
- **Notes:** **Open with the connective from Bit 1's mess** — _"it wasn't only the mess" / "וזה לא נגמר בבלגן"_ — so this reads as escalation, not a restart (the seam from Slide 4; no closing bridge in Bit 1). EOL is the trigger, not the full case. Migration gave legitimacy to refactoring that couldn't justify itself alone.

## Slide 6 — How it was decided

- **Visual:** Flow: Internal discussions → Frontend team meeting → React
- **Notes:** Two layers: "can't hire" for leadership. Ecosystem + team familiarity + ownership for the team. Decision made together, not top-down.

## Slide 7 — The options

- **Visual:** Four options listed, three ruled out, one standing: rewrite from zero · micro-frontends · do nothing · incremental
- **Notes:** Do nothing was real. Rewrite = freeze. Micro-frontends = split state/nav/components. Incremental was the only fit.

## Slide 8 — Why incremental + r2a

- **Visual:** Angular box ← r2a → React box, arrow labeled "new components flow one way"
- **Notes:** r2a is the simplest solution. New features in React from day one. React components usable inside Angular. Mostly eliminates dual-maintenance — exceptions are Bit 3's story.

## Slide 9 — What the migration justified

_(alt titles: "While we were in there" · "מה שהמעבר אפשר")_

- **Visual:** "TypeScript + Tailwind" large, clean
- **Notes:** The opening, not a principle. The migration was cover for improvements that **couldn't justify themselves alone** (callback to S5's legitimacy beat) — TS + Tailwind, merged in the first PRs. We took the opportunity while we were already in there. **Grace note, don't sell it:** I argued against TypeScript; we did it anyway; changes are far easier now. Let "I was against it" land as a small aside — the room decided together (echoes S6), not a confession.

## Slide 10 — Same surface, new engine

- **Visual:** Title alone: "אותו ממשק. מנוע חדש מתחת." _(Same surface. New engine underneath.)_
- **Notes:** A decision, not a regret. We didn't redesign while migrating — held the UX identical and rebuilt the code beneath it. The migration wasn't product-driven, so there was no one to sanction UX changes; and changing the surface mid-migration would muddy attribution — you couldn't tell a regression from a redesign. Behavior-preserving, but still a full refactor underneath, not a translation (Bit 4 cashes this). Bridges to Bit 3: same ship, swap the engine.
