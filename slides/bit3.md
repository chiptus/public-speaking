# Bit 3 — Living with Mixed Code (Slides 11–14)

| # | Title | Visual | Notes |
|---|-------|--------|-------|
| 11 | Mid-flight | Image of a plane in flight — no text, or minimal: "mid-flight" | Engine mid-flight while someone asks for first class. Speaker delivers both lines verbally. Image only — no text duplication. |
| 12 | Two versions of the same component | Short code snippet: Angular version using `ng-transclude` next to React version using `children` prop | r2a has no children prop. ng-transclude keeps the Angular version alive. Code shows the structural divergence. Speaker provides snippet. |
| 13 | Two models in your head | Code snippet showing `scope.$evalAsync(() => ...)` wrapper, or a data flow diagram: Angular ↔ (2-way) vs React → (1-way) | Cognitive cost: 2-way and 1-way binding coexist. The wrapping pattern is the symptom. Code or diagram — speaker to choose the form that feels most concrete. |
| 14 | 50/50 | "This is not a transition phase." / "This is how it runs." / "For years." — three lines, large, centered | The key reframe. Say it as a fact. Not a complaint. Let it sit. Strong close for the bit. |

---

## Decisions Made in This Session

- [אנושי] moments (silence asymmetry, stolen time) removed from Bit 3 — placement TBD in Bit 5 planning
- Slide 12: code snippet approved (ng-transclude vs children prop)
- Slide 13: code or diagram — speaker to decide
- Analogy: engine mid-flight (not Ship of Theseus)
