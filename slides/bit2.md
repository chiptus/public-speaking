# Bit 2 — The Decisions (Slides 5–10)

| # | Title | Visual | Notes |
|---|-------|--------|-------|
| 5 | Why it had to change | Three lines: *dead library · refactor needed anyway · new features coming* | EOL is the trigger, not the full case. Migration gave legitimacy to refactoring that couldn't justify itself alone. |
| 6 | How it was decided | Flow: Internal discussions → Frontend team meeting → React | Two layers: "can't hire" for leadership. Ecosystem + team familiarity + ownership for the team. Decision made together, not top-down. |
| 7 | The options | Four options listed, three ruled out, one standing: rewrite from zero · micro-frontends · do nothing · incremental | Do nothing was real. Rewrite = freeze. Micro-frontends = split state/nav/components. Incremental was the only fit. |
| 8 | Why incremental + r2a | Angular box ← r2a → React box, arrow labeled "new components flow one way" | r2a is the simplest solution. New features in React from day one. React components usable inside Angular. Mostly eliminates dual-maintenance — exceptions are Bit 3's story. |
| 9 | Foundations first | "TypeScript + Tailwind" large, clean | Merged in first PRs. Deferring foundations is compounding debt. |
| 10 | Decisions in a vacuum | Title alone: "When you don't know what stays — everything becomes sacred" | The vacuum defaults to conservatism. Decide early what you're NOT keeping. One of the things Chaim would do differently. |
