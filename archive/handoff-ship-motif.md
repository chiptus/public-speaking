# Handoff — Ship motif decisions (recurring visual)

**Date:** 2026-05-30
**Talk:** Migrating Portainer's frontend from AngularJS to React (Hebrew, 32–35 min + Q&A)
**Source proposal:** `talk-review.md`, "Addendum — Ship motif as a recurring visual" (lines ~100–130).

## What this session is for

Decide whether (and how) the **ship** appears as a *recurring orientation visual* across the deck. The metaphor itself is settled — the open work is the visual treatment at the seams, the bookends, and two contested slides.

## Critical working style (the speaker corrects on this)

- Work **one slide/decision at a time.** Discuss, get agreement, move on. Do NOT batch-produce.
- Do NOT enter plan mode — this is a discussion, not a plan-and-execute task.
- When you change a title/visual/note, say **why.**
- Speaker is **allergic to slogan slides** ("selling the story back"). Default: *enact* the idea via a concrete artifact, don't assert it.
- Slides in English, speaker presents in Hebrew, notes in English. Per-slide section format (`### Slide N — Title` + `**Visual:**` / `**Notes:**`).

## Already decided this session (do NOT reopen)

- **The ship is the talk's single unified metaphor.** Bit 1's analogy is Ship of Theseus; Bit 3's "engine swap" is the *same ship*, not a separate plane.
- **Plane → ship fix applied** in both places: `slides/bit3.md` Slide 11 (now "Swapping the engine at sea") and `migration-talk-sekelton.md` Bit 3 analogy ("החלפת מנוע בלב ים … סיפון חדש"). The competing plane metaphor is gone.
- **Close is deliberately lean.** This session stripped Bit 5 to a single forward slide (Slide 24), finale → none, the React question and the first-merge moment → Q&A. The ship work must not silently rebuild a victory-lap close.

## Open decisions (the actual task)

1. **Does the ship recur as an orientation visual at all?** The addendum proposes it at the seams (bit boundaries) + the two bookends. Ernst endorses a recurring orientation visual for 30+ min talks. Confirm the speaker wants this before placing any states.
2. **Which ship states, and how many?** Addendum lists 7 appearances (Slides 1, 2, 11, boundary 2→3, boundary 3→4, 23, 24) but calls it "5 states." Distinct *states* are ~3 (whole / few planks / half). **Tighten the claim** and confirm the real count. Also: do bit-boundary **transition cards** even exist in this deck, or is that a new device being introduced?
3. **Slide 23 — keep the ship OFF (my recommendation).** Slide 23 is the deck's earned emotional peak: the ~50% dashboard full-screen, weight the audience earned (see `slides/bit4.md` Slide 23 + its design notes). The addendum wants to pair/alternate a half-ship there. Risk: trades documentary weight for cleverness — exactly what the addendum's own principle says to avoid. The boundary 3→4 half-ship already establishes the image right before it. **Recommendation: 23 stays pure dashboard; the ship's *meaning* pays off at the close, not here.**
4. **Slide 24 collision — must resolve.** Slide 24 is LOCKED as a two-half **text reflection** ("Starting now" / "What I'd want" — see `slides/bit5.md`). The addendum wants the half-rebuilt ship as Slide 24's visual anchor. **You cannot have both** the two columns of phrases and the ship as the anchor. Options:
   - (a) Ship becomes 24's only visual; the two halves go fully spoken. (We rejected an empty/title-only 24 earlier for exactly this reason — revisit only if the ship changes that calculus.)
   - (b) Reflection stays as 24; the ship is a **separate wordless closing card after it** — the literal last image, which also sits through Q&A. This adds one slide (speaker resisted a 2nd *content* slide, but a wordless image isn't content). **My lean.**
   - Note: two independent analyses (the review's recency/dwell point + the addendum) both flag 24 as needing a visual anchor. The ship may be the fix — but the content has to go somewhere.
5. **Two ship "languages."** The *progress* ship (whole → few planks → half = "where are we") and the *scene* ship at Slide 11 (engine-swap-at-sea = the operational constraint) do different jobs and look different. If the audience reads planks as a progress meter, Slide 11's scene isn't "more planks." Fine to use one metaphor two ways, but the Slide 11 image should visibly be *the same ship*, just in action — don't assume the orientation reading carries automatically.

## Compatible with the review (already cross-checked)

- The review's **narrative-symmetry close** (recommendation #2) is about the **ship question** (Slide 1: "rebuild it in a different language without changing it?"), NOT the React question. So a spoken ship-callback close is compatible with React → Q&A. The ship addendum's Slide 24 note implements exactly this.
- The review's **#1 (promise at the open)** pairs with the Slide 2 whole-ship state. Cheap, no rule broken — worth doing alongside the ship work.

## Authoritative artifacts (read first)

- `talk-review.md` — the addendum (lines ~100–130) and the book-grounded review above it.
- `slides/bit1.md`, `bit3.md` (Slide 11, just changed), `bit4.md` (Slide 23 — the peak), `bit5.md` (Slide 24 — the locked reflection).
- `migration-talk-sekelton.md` — canonical skeleton. Top block has the spine + tone guardrail ("don't announce the moral"; enact, don't assert).

## Suggested first move

Confirm decision #1 (does the ship recur at all), then walk 23 and 24 — the two contested slides — one at a time. Leave the open/bookend promise (#1 above) for last since it's low-risk.
