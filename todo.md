# Talk revision — handoff (after dry-run 1 + Sagit's feedback)

**Status:** dry run ran **15 min** against a **32–35 min** target. Diagnosis below. Source feedback: `takes/dryrun1/sagit-feedback`. Grounded in CandleKeep books (Tech Talk ref, Anderson, Gallo, Miller, Rodriguez).

---

## Core diagnosis

The short runtime is **structural, not pace**. A short talk isn't a fast long talk — it's missing whole phases.

Time budget for 30 min (Witowski/Riederer/Ernst):

| Phase | Time | State |
|---|---|---|
| Hook / problem | 0–3 | ✅ strong (Sagit agrees) |
| **Context / landscape** | **3–8** | ❌ mostly collapsed |
| Core content | 8–22 | ✅ present as beats |
| **Explicit takeaways (recap)** | **22–27** | ❌ none — S24 is forward-looking, not a recap |
| Q&A | 27–30 | ✅ |

The missing **context** + **takeaway** phases ≈ the lost ~17 min.

**Mechanical cause:** cards are built as *"beats only, rationale glance-only, never spoken."* Riederer says each topic sentence needs **2–3 spoken subpoints** (constraint → tension → decision). We have ~24 topic sentences and **zero spoken subpoints** under them. The reasoning was written into design-notes and marked do-not-speak. That design *is* the 15-min talk.

---

## Two framing decisions

- **Spine: KEEP.** Don't rethink it. *"If you're stuck with legacy code, you're not trapped"* is **audience-as-hero**, which the books call the one correct choice (Miller p.68). The audience-message line already does this. The speaker is the **guide**, not the hero — tilt each decision beat toward "here's what *you* can take," but the facts/spine don't change.
- **Restraint rule: REVISE.** *"Don't announce the moral"* has bled into *"don't speak the reasoning."* Different things. Speak the **constraints**; cut the **editorial** ("and that's why this was right"). The well-structured why *is* the argument (Anderson p.61).

---

## The four moves

1. **Build the missing phases** — a context/landscape beat early; an explicit takeaway/recap beat near the end (distinct from S24's forward look).
2. **Add spoken constraint-reasoning** under each decision card — expose constraint → let tension build → decision lands (Anderson's explanation order). Flagship: the TypeScript beat (what I feared / did it anyway / now glad).
3. **Front-load frame-story stakes** — StoryBrand *hero-in-a-hole*: open with the hole (calcifying code, no mandate, leadership unconvinced, solo, for years) **before** any climb. Solo/scale/resistance are stakes amplifiers — pull the *fact* forward; **keep the *feeling* at S24** so the close Sagit loved isn't defused.
4. **Progressive disclosure + spoken transitions** throughout — staged bullets (highlight current, dim rest); speak the transition *before* the click. Write the missing 1→2 and 2→3 bridges.

---

## Sagit's notes → mapped

- **Frame story (her #1)** → move 3.
- **"Detail considerations" (TypeScript example)** → move 2.
- **Cognitive anchor** — clarified: *within-slide markers showing which point I'm on* (generalize the S7 strike pattern) → move 4. Backed by Anderson p.98 (builds, one idea at a time). Doubles as a pacing brake.
- **Transitions / flow** → move 4.
- **Praise (keep):** opening, ending, the "insights between," the breaks.

## Push-back on Sagit (one point)

She suggested *"maybe add the central message up front."* Books say **don't** (Anderson p.128: tease, don't give it away). Reconciliation: add title + roadmap (*"three decisions that surprised us"*) + the central **question** — **not** the message. Ship of Theseus is already a *question*, not a moral. Map the journey, hide the destination (Anderson p.130).

---

## Context/landscape phase — DECIDED (2026-06-08)

The villain is **indifference, not resistance** — nobody opposed the migration, nobody prioritized it ("even one screen per release doesn't really happen"). That's the honest difficulty and the universal the room shares. Frame-story stakes go up front; the indifference theme **pays off again at S24** (the "real priority" ask), so it's planted, not dumped.

- [x] **S4.5 drafted** (new slide, `bit1.md`) — the condition: I pushed it · nobody opposed · never priority · that's the hard part → "you have one too." Mostly spoken; ~1.5–2 min recovered here.
- [ ] **S3** — fold in the scale arc as one spoken line (2018: 3–4 devs → today ~10–15; migration outlived people who joined/left). No extra slide.
- [ ] **S4** — relocate its closing room-turn to S4.5; S4 ends on the mess. Pick one room-line.
- [ ] Render S4.5's spoken lines to Hebrew (isolated lines — avoid inline RTL mixing).
- [ ] Renumber Bit 1→5 once S4.5 is locked (currently a .5 insert).

## Open / next

- [ ] Title + roadmap + central **question** up front (not the message — Anderson p.128)
- [ ] Add takeaway/recap phase before S24
- [ ] Write spoken constraint-reasoning per decision card (start: TypeScript)
- [ ] Progressive-disclosure spec across multi-point slides
- [ ] Write 1→2 and 2→3 transitions
- [ ] (carried from skeleton) self-intro phrasing · dashboard screenshot for S23
