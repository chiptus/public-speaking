# Bit 3 — Living with Mixed Code (Slides 11–14)

## Slide 11 — Swapping the engine at sea

- **Visual:** A ship at sea with its engine being swapped mid-voyage — the PO leaning over the rail asking for a new deck. No text, or minimal. Speaker sources the image.
- **Notes:** The operational constraint — you can't stop the running system. The ship is the talk's single unified metaphor (established in Bit 1, Ship of Theseus), now shown in its working state — no competing plane. Speaker delivers both lines verbally. ("new deck" = ship deck / slide deck pun — English only, optional.) Image only — no text duplication.

## Slide 12 — Two versions of the same component

- **Visual:** Short code snippet: Angular version using `ng-transclude` next to React version using `children` prop
- **Notes:** r2a has no children prop. ng-transclude keeps the Angular version alive. Code shows the structural divergence. Speaker provides snippet.

## Slide 13 — Two models in your head

- **Visual:** Code snippet showing `scope.$evalAsync(() => ...)` wrapper, or a data flow diagram: Angular ↔ (2-way) vs React → (1-way)
- **Notes:** Cognitive cost: 2-way and 1-way binding coexist. The wrapping pattern is the symptom. Code or diagram — speaker to choose the form that feels most concrete.

## Slide 14 — 50/50

- **Visual:** "This is not a transition phase." / "This is how it runs." / "For years." — three lines, large, centered
- **Notes:** The key reframe. Say it as a fact. Not a complaint. Let it sit. Strong close for the bit.

---

## Decisions Made in This Session

- [אנושי] moments (silence asymmetry, stolen time) removed from Bit 3 — placement TBD in Bit 5 planning
- Slide 12: code snippet approved (ng-transclude vs children prop)
- Analogy: swapping the engine at sea — the ship is the talk's single metaphor (Bit 1 Ship of Theseus); the competing plane was removed
