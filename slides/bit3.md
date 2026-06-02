# Bit 3 — Living with Mixed Code (Slides 11–14)

> Cards are beats + one cue, never rationale — the "why" lives in Design notes below.
> 🔒 = learned word-for-word. Cues are glance-only, never spoken.

## Slide 11 — Swapping the engine at sea

- **Visual:** A ship at sea with its engine being swapped mid-voyage — the PO leaning over the rail asking for a new deck. No text, or minimal. Speaker sources the image.
- **Notes:**
  - can't stop the running system
  - PO at the rail wants a new deck _(pun, EN only, optional)_
  - _Cue:_ image only — lines spoken, no text

## Slide 12 — Two versions of the same component

- **Visual:** Short code snippet: Angular version using `ng-transclude` next to React version using `children` prop
- **Notes:**
  - no children prop → ng-transclude keeps Angular alive
  - snippet = the structural divergence
  - _Cue:_ let the code carry it, don't narrate

## Slide 13 — Two models in your head

- **Visual:** Code snippet showing `scope.$evalAsync(() => ...)` wrapper, or a data flow diagram: Angular ↔ (2-way) vs React → (1-way)
- **Notes:**
  - 2-way + 1-way coexist = the cognitive cost
  - the wrapper is the symptom
  - _Cue:_ name the cost, don't teach the API

## Slide 14 — 50/50

- **Visual:** "This is not a transition phase." / "This is how it runs." / "For years." — three lines, large, centered
- **Notes:**
  - the key reframe — line is on the slide
  - _Cue:_ say as fact, not complaint — let it sit
- **→ Bridge to Bit 4 (improvised):** _silence first — let S14 land._ Then: if it's the state for years, the question isn't *whether* to migrate but *how* — well, again and again → S15.
  - _Cue:_ question only — don't pre-state "find the patterns"

## Design notes

- The ship is the talk's single unified metaphor (Bit 1, Ship of Theseus), now shown in its working state — no competing plane.
- S13 was flagged "unclear" in run 1 (`takes/take1/notes1.md`) — keep it concrete: one symptom (the wrapper), one cost (two mental models), no API tour.
- Bridge springs straight off S14, no reach-back into Bit 3.

---

## Decisions Made in This Session

- [אנושי] moments (silence asymmetry, stolen time) removed from Bit 3 — placement TBD in Bit 5 planning
- Slide 12: code snippet approved (ng-transclude vs children prop)
- Analogy: swapping the engine at sea — the ship is the talk's single metaphor (Bit 1 Ship of Theseus); the competing plane was removed
