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
| Core content | 8–22 | ❌ present as beats, but reasoning unspoken — see mechanical cause |
| Takeaway (spoken line) | ~26 | ❌ never said aloud — fix = one spoken line at the S23→S24 bridge, **NOT** a new slide |
| Q&A | 27–30 | ✅ |

The missing **context** phase + the **unspoken reasoning** under every card ≈ the lost ~17 min. (The takeaway is one spoken line, ~30s — not a phase; revised 2026-06-09, see below.)

**Mechanical cause:** cards are built as *"beats only, rationale glance-only, never spoken."* Riederer says each topic sentence needs **2–3 spoken subpoints** (constraint → tension → decision). We have ~24 topic sentences and **zero spoken subpoints** under them. The reasoning was written into design-notes and marked do-not-speak. That design *is* the 15-min talk.

---

## LOCKED — direction, takeaway, strategy (2026-06-09)

- **Subject vs. tension:** the **migration is the subject**; the **5 years (indifference) is the tension that earns attention** — not a competing thesis. Promoting "5 years" to *the problem* tips into "why won't my org prioritize me" (grievance). Confirms the kept spine; just names the relationship. (Library agrees: open with the concrete puzzle, not the cost.)
- **The takeaway — LOCKED, one sentence:**
  > **You're not stuck with legacy code — you can migrate it incrementally while you keep shipping, as long as you're honest that it's a multi-year campaign, not a sprint.**
  Carries all three: audience-as-hero (*"you can"*) · the subject (incremental, keep shipping) · the tension (multi-year, baked in — not a complaint). Rejected alternatives: *"the hard part is momentum, not tech"* (= the 5-years-as-subject talk we ruled out) and *"go view by view"* (a *how*, not a belief).
- **Takeaway delivery:** a **spoken line at the S23→S24 bridge**, **not a recap slide.** A separate recap slide = two endings competing with S24 (which is reflection + ask, different content). Sequence: restate thesis (spoken) → S24 personal lessons/ask → finale ship. Supersedes the earlier "add a takeaway/recap *phase/beat*."
- **Fill strategy:** **deepen existing slides first.** Add spoken reasoning + the context phase onto current slides; reach for a new slide only when a beat genuinely needs its own visual. (Headroom exists — book says ~25–28 slides for 30 min — but bloat is the risk, so deepen before adding.)
- **The open:** fuse B+C — the concrete problem (the code) + *"5 years, no ending"* in one breath; self-intro **after**. Front-load the *fact* of the stakes; keep the *feeling* at S24.

---

## Two framing decisions

- **Spine: KEEP.** Don't rethink it. *"If you're stuck with legacy code, you're not trapped"* is **audience-as-hero**, which the books call the one correct choice (Miller p.68). The audience-message line already does this. The speaker is the **guide**, not the hero — tilt each decision beat toward "here's what *you* can take," but the facts/spine don't change.
- **Restraint rule: REVISE.** *"Don't announce the moral"* has bled into *"don't speak the reasoning."* Different things. Speak the **constraints**; cut the **editorial** ("and that's why this was right"). The well-structured why *is* the argument (Anderson p.61).

---

## The four moves

1. **Build the missing context phase** — a context/landscape beat early (indifference stakes), folded into S3/S4 as flat spoken beats. (The takeaway is now a single spoken line at the S23→S24 bridge — see LOCKED 2026-06-09 — *not* a separate phase.)
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

**S4.5 dropped** — a dedicated "condition" slide read too big/dramatic (it was announcing the moral). The fix: keep the facts, kill the drama, fold into S3 as flat spoken beats. No new slide.

- [x] **S3 → "Self-intro + setup"** (done, `bit1.md`) — name/role + size arc (3–4 → ~10–15) + "led it largely on my own" + "never the priority," all spoken flat over the existing name card. S3 loses its "brisk" cue. "Never the priority" plants here, pays off at S24.
- [x] S4 unchanged (it stays *reasons to move + the mess*; conditions are not its theme).
- [ ] Render S3's new spoken lines to Hebrew (isolated lines — avoid inline RTL mixing).

## Open / next

- [ ] **Write spoken constraint-reasoning per decision card — START HERE, flagship: TypeScript** (constraint → tension → decision); then replicate the shape across r2a, incremental-vs-rewrite, behavior-preserving
- [ ] Fuse the open (S1–S4): code + "5 years, no ending" in one breath, self-intro after
- [ ] Land the takeaway as a spoken line at the S23→S24 bridge (no new slide)
- [ ] Title + roadmap + central **question** up front (not the message — Anderson p.128)
- [ ] Progressive-disclosure spec across a *few* multi-point slides (not all)
- [ ] Write 1→2 and 2→3 transitions
- [ ] Q&A prep — why migrate · how long · how many to convince · why so slow
- [ ] (carried from skeleton) self-intro phrasing · dashboard screenshot for S23
