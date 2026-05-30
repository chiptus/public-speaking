# Handoff — Slide Planning, Bit 3 Onwards

**Date:** 28/5/2026
**Speaker:** Chaim Lev-Ari
**Talk:** Migrating Portainer's frontend from AngularJS to React
**Next session goal:** Continue slide planning from Bit 3

---

## Source Material

The authoritative skeleton is at:
`/mnt/user-data/outputs/migration-talk-skeleton.md`

A previous "why React?" decision handoff is at:
`/mnt/user-data/outputs/handoff-why-react.md`
(resolved — no separate slide, answer lives inside Bit 2 Slide 6)

---

## Talk Overview

- **Length:** 32–35 minutes + Q&A
- **Audience:** Senior fullstack developers, professional-social weekly meetup, don't know the speaker
- **Language:** Slides in English. Speaker presents in Hebrew. Speaker notes in English.
- **Central message:** You can lead deep technical change from the bottom up, even when it's not an organizational priority. A story of ownership and initiative — not a clean success story.
- **[אנושי]** = human/personal moments woven throughout. Not concentrated in one beat.
- **א״מ** = agreed shorthand for AI.
- Style: minimalist. One idea per slide. Slides are background to the speaker, not standalone documents. No bullet-heavy slides.

---

## Bit Structure

| Bit | Topic | Minutes | Status |
|-----|-------|---------|--------|
| 1 | Opening | 4–5 | ✅ Signed off |
| 2 | The decisions | 4–5 | ✅ Signed off |
| 3 | Living with mixed code | 4–5 | ⬜ Not started |
| 4 | Depth and AI | 8–10 | ⬜ Not started |
| 5 | Closing | 4–5 | ⬜ Not started |

---

## Bit 1 — Final Slides (Slides 1–4)

| # | Title | Visual | Notes |
|---|-------|--------|-------|
| 1 | Ship of Theseus | "How do you rebuild an app in a different language — without changing it?" Large text, centered | Leave open. Don't answer here. It lands differently by the end. |
| 2 | Hook | "We started five years ago. We're not done. Fifty percent. This is not a story with an ending." Four large lines, centered, nothing else | Say it slow. Full stop after each sentence. Silence after the last line is part of the slide. |
| 3 | Self-intro | Chaim Lev-Ari / Software developer, Portainer.io / Leading the migration from the start — with breaks | One sentence on Portainer verbally: מוצר לניהול קונטיינרים. Don't linger. Not a Portainer talk. |
| 4 | The codebase before | Screenshot of a real controller — to be captured by speaker | Goal is the feeling of scale, not reading the code. The migration didn't create this mess — it exposed it. |

**Note on Slide 1:** The Ship of Theseus analogy opens more questions than stated — does the app need to stay the same? What are the requirements? These are spoken, not on the slide.

---

## Bit 2 — Final Slides (Slides 5–10)

| # | Title | Visual | Notes |
|---|-------|--------|-------|
| 5 | Why it had to change | Three lines: *dead library · refactor needed anyway · new features coming* | EOL is the trigger, not the full case. Migration gave legitimacy to refactoring that couldn't justify itself alone. |
| 6 | How it was decided | Flow: Internal discussions → Frontend team meeting → React | Two layers: "can't hire" for leadership. Ecosystem + team familiarity + ownership for the team. Decision made together, not top-down. |
| 7 | The options | Four options listed, three ruled out, one standing: rewrite from zero · micro-frontends · do nothing · incremental | Do nothing was real. Rewrite = freeze. Micro-frontends = split state/nav/components. Incremental was the only fit. |
| 8 | Why incremental + r2a | Angular box ← r2a → React box, arrow labeled "new components flow one way" | r2a is the simplest solution. New features in React from day one. React components usable inside Angular. Mostly eliminates dual-maintenance — exceptions are Bit 3's story. |
| 9 | Foundations first | "TypeScript + Tailwind" large, clean | Merged in first PRs. Deferring foundations is compounding debt. |
| 10 | Decisions in a vacuum | Title alone: "When you don't know what stays — everything becomes sacred" | The vacuum defaults to conservatism. Decide early what you're NOT keeping. One of the things Chaim would do differently. |

---

## Bit 3 — Not Started

**Topic:** Living with mixed code

**Skeleton content to cover:**
- Analogy: replacing the engine mid-flight — while someone asks for first class
- Concrete example 1: r2a doesn't support `children` prop → `ng-transclude` → two versions of the same component in parallel until the Angular one dies
- Concrete example 2: `scope.$evalAsync` — React calls a callback, Angular doesn't know, UI doesn't update. You learn to wrap everything. This is the cognitive cost — two mental models simultaneously.
- Key point: 50/50 is not a transition phase — it's a permanent operating mode for years
- **[אנושי]:** Silence asymmetry — nobody voices an opinion in planning, everyone's an expert when something breaks
- **[אנושי]:** Working in stolen time, no official prioritization

**Note:** The two concrete examples (ng-transclude + scope.$evalAsync) together tell a complete story — structural cost + cognitive cost. Both belong.

---

## Bit 4 — Not Started

**Topic:** Depth and AI

**Skeleton content to cover:**

*The table story:*
- Researching recurring patterns in old code
- Finding where developers already copy-paste
- Building where they're already going
- Migration = refactor, not line-by-line translation

*AI arc — three phases:*

1. **The beginning:** Copilot for technical conversion. Refactor decisions (break into small components, decide what's worth building) stay with the developer.

2. **The fall:**
   - Philosophy was known before: tests first, small units, merge with enough lead time before release
   - Came back rusty
   - Asked AI to convert a whole page
   - Quote to preserve verbatim: *"נותן להרגיש שהכל אפשרי, רק צריך לשלוח עוד הודעה"*
   - Didn't skip the technology — skipped the patience
   - Bugs → project pause

3. **The recovery:**
   - Dashboard built in October: count of remaining Angular components, lines of code
   - Measurement as a condition for continuing
   - Ask AI for a plan, break into tasks, plan each separately
   - Same small-units principle — now a layer above
   - Today: can plan everything with it

*The light moment:* First merge. Seeing other developers use what was built.

---

## Bit 5 — Not Started

**Topic:** Closing

**Skeleton content to cover:**
- What I'd do differently: recruit partners, prioritize as an engineering task from day one — not something that will sort itself out
- Looking forward: process change brought more organizational involvement. VP now more engaged than before.
- The prepared answer: "Would you migrate to React today?" — Still think the reasons were right. The path could have been different, but it doesn't depend only on me.
- Closing line (resolved in earlier session): If there's a team and prioritization — it looks different. If continuing alone, sometimes underground, in stolen time — it looks almost the same.

---

## Q&A Prep (Slides NOT needed — spoken only)

- Why not Vue / Svelte
- Why not micro-frontends
- Why not rewrite from zero
- Top-down or bottom-up → bottom-up
- Where to start → went with the busiest page everyone sees

---

## Working Decisions Log

- Slides in English, speaker in Hebrew, notes in English
- Minimalist style — one idea per slide, slides as backdrop
- No code on slides — screenshots of real code possible (speaker provides)
- [אנושי] moments woven into beats, not collected in one section
- "Why React?" — no separate slide. Answered inside Slide 6. Q&A prep handles follow-up.
- Bit 2 Slides 7+8 kept separate (decision vs solution — different energy)
- No Q&A slides — those are spoken

---

## Suggested Skills

- `/mnt/skills/public/pptx/SKILL.md` — required before building any file
- `/mnt/skills/user/portainer-virtual-se/SKILL.md` — only if Portainer context needed, use sparingly
