# Bit 3 — Living with Mixed Code (Slides 11–14)

> Cards are beats + one cue, never rationale — the "why" lives in Design notes below.
> 🔒 = learned word-for-word. Cues are glance-only, never spoken.

## Slide 11 — Swapping the engine at sea

- **Visual:** A ship at sea with its engine being swapped mid-voyage — the PO leaning over the rail asking for a new deck. No text, or minimal.
- **Notes:**
  - analogy: engine swap mid-sail · PO wants a new deck
  - **ask:** _"so — what's it like to live like this?"_
  - _Cue:_ once · no pause → S12

## Slide 12 — Two versions of the same component

- **Visual:**
  - Title (on slide): **Two versions of the same component**
  - Short code snippet: Angular `rdWidget` (using `ng-transclude`) next to React `Widget` (using `children` prop)
- **Notes:**
  - no children prop → ng-transclude keeps Angular alive
  - snippet = the structural divergence
  - _Cue:_ let the code carry it, don't narrate

## Slide 13 — Two models in your head

- **Visual:**
  - Title (on slide): **Two models in your head**
  - Data-flow diagram — Angular ↔ (2-way binding) vs React → (1-way binding), shown side by side.
- **Notes:**
  - 2-way + 1-way coexist = the cognitive cost
  - the wrapper is the symptom
  - digest cycle
  - _Cue:_ name the cost, don't teach the API

## Slide 14 — 50/50

- **Visual:** "This is not a transition phase." / "This is how it runs." / "For years." — three lines, large, centered
  - **Build behavior:** one line at a time, in order. Pause after each. The silence after "For years." is the point — don't rush it.
- **Notes:**
  - the key reframe — line is on the slide
  - _Cue:_ say as fact, not complaint — let it sit
- **→ Bridge to Bit 4 (improvised):** _silence first — let S14 land._ Then: if it's the state for years, the question isn't _whether_ to migrate but _how_ — well, again and again → S15.
  - _Cue:_ question only — don't pre-state "find the patterns"

_(Design rationale + session decisions for this bit → `design-notes.md`.)_
