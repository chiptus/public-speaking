# Bit 3 — Living with Mixed Code (Slides 11–14)

## Slide 11 — Mid-flight

- **Visual:** Image of a plane in flight — no text, or minimal: "mid-flight"
- **Notes:** Engine mid-flight while someone asks for first class. Speaker delivers both lines verbally. Image only — no text duplication.

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
- Slide 13: code or diagram — speaker to decide
- Analogy: engine mid-flight (not Ship of Theseus)
