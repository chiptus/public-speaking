# Bit 2 — The Decisions (Slides 5–10)

> Cards carry beats **plus a spoken cue** — the speaker voices the reasoning live, in his own words, shaped **constraint → tension → decision**.
> 🔒 = learned word-for-word. **Speak:** = the reasoning he says out loud (prompts, not a script — don't memorize). _Cue:_ = silent staging/delivery prompt. The editorial "why" still lives in `design-notes.md`.

## Slide 5 — Why it had to change

- **Visual:**
  - Title (on slide): **Why it had to change**
  - Three lines: _hard to hire · refactor needed anyway · EOL deadline (Dec 2021)_
  - **Build behavior (within-slide anchor — accumulate flavor):** items appear one at a time in order (hiring → refactor → EOL). The **current** line is lit (full weight/accent); already-spoken lines stay visible but drop to a resting dim; the not-yet-reached line is absent until its beat. All three visible (dim) by the end. Synced to delivery, never auto — advancing the light is the pacing brake. Sibling of S7's strike (eliminate flavor); spec in `design-notes.md`.
- **Notes:**
  - 🔒 seam from Bit 1: _"וזה לא נגמר בבלגן"_ (it wasn't only the mess)
  - hiring = the real trigger: no dev wants to start on a dead framework (CEO arg, S6)
  - EOL = a known deadline since 2018, not a surprise — we prepared, didn't react
  - _Dates (say cleanly — take-3 garbled these):_ known/announced **since 2018**, actual **EOL Dec 2021**. Don't flip them.
  - refactor we'd do anyway → migration legitimized it
  - _(bg ref:_ initial migration commit → https://github.com/portainer/portainer/commit/85a6a807226d9f3baf7ec265022f130aed1eddd1 _)_
  - _Cue:_ escalation off Bit 1 — not a restart

## Slide 6 — How it was decided

- **Visual:**
  - Title (on slide): **How it was decided**
  - Flow: Internal discussions → Frontend team meeting → React
- **Notes:**
  - leadership layer: "can't hire" for AngularJS
  - _human beat (don't flatten to process):_ a real conversation with the CEO — made the hiring argument in **his** language, not ours. This is the warm note of the bit; take-3 dissolved it into "talks → green light."
  - team layer: ecosystem · familiarity · ownership
  - _Cue:_ land "decided together, not top-down"

## Slide 7 — The options

- **Visual:**
  - Title (on slide): **The options**
  - Three items, each on its own line — this is the on-slide text:
    - rewrite from zero
    - micro-frontends
    - incremental
  - **Build behavior (NOT on-slide text — this is an instruction):** all three appear plain on load; strike each through one at a time as the speaker rejects it; `incremental` is the only one left unstruck. **Do not show any strikethrough on load** — the strike happens live, synced to delivery.
- **Notes:**
  - reqs: keep shipping · don't freeze dev · don't fragment state/nav
  - rewrite (as a separate team's parallel build) → freezes delivery / forces double-dev in AngularJS · micro-frontends → fragments state/nav · incremental → meets all
  - _Cue:_ strike each → name what it fails

## Slide 8 — Why incremental + r2a

- **Visual:** two small code blocks — **register** then **use** (no diagram; the snippet _is_ the diagram):
  ```ts
  // register a React component as an AngularJS one
  angular
    .module("portainer")
    .component("reactButton", r2a(Button, ["label", "onClick"]));
  ```
  ```html
  <!-- now use it inside any AngularJS template -->
  <react-button label="Save" on-click="$ctrl.save"></react-button>
  ```
- **Notes:**
  - r2a = simplest fit · new features in React from day one
  - the snippet shows the whole deal: _"I just need the component and its props"_ (take line — say it off the code)
  - one-way flow: React runs inside Angular → kills most dual-maintenance
  - _Cue:_ two blocks only, no API tour · don't open the pain yet (→ Bit 3)

## Slide 9 — What the migration justified

- **Visual:**
  - Title (on slide): **While we were in there**
  - "TypeScript + Tailwind" large, clean
- **Notes:**
  - migration = cover for improvements that couldn't justify themselves alone
  - TS + Tailwind, merged in the first PRs
  - grace note: I argued against TypeScript; we did it anyway; far easier now
  - _Cue:_ "I was against it" — aside, don't sell

## Slide 10 — Same surface, rebuilt underneath

- **Visual:** Title alone: "Same surface. Rebuilt underneath."
- **Notes:**
  - users don't know it's React, don't know it's Angular — **they don't need to know. Same app to them.**
  - **warm close (the payoff of the Bit 2 decisions — first merge):** another dev built on our React components → it felt real, the decisions paid off. _(Bit 2 ends up/warm.)_
  - a decision, not a regret
  - behavior-preserving, still a full refactor — not a translation

_(Design rationale for this bit → `design-notes.md`.)_
