# Ship visual system (recurring)

**Decided 2026-05-30.** The ship is the talk's single unified metaphor (Ship of Theseus). This file is the source of truth for how it appears across the deck. Per-slide files reference it.

## The one metaphor, two scales

| | Corner progress ship | Big bookend ships |
|---|---|---|
| **Job** | Ambient orientation — "how far are we" | The emotional / identity beats |
| **Size** | Small, top-right corner | Large |
| **Where** | Almost every slide | Slide 1 (open) + closing card (after Slide 24) |

Both speak the **same visual language**: a whole, sailing ship whose planks color-fill from **Angular-grey → React-green**. They differ only in size and in how many planks have turned.

## Color-fill, not build-up (the rule that keeps it on-metaphor)

The ship is **always whole and sailing.** Progress = planks changing **color** (grey → green), never planks being *added* to an empty frame.

- **Why:** the app was never empty — it was a working AngularJS app. "Building from nothing" tells the wrong story. "Replacing planks on a ship that keeps sailing" *is* Ship of Theseus, and it's honest.
- Fill is **chunky, per-bit** (5 bits = ~5 perceptible steps), not subtle plank-by-plank — a 30px icon can't show fine change.
- Always fill *within a fixed full silhouette* (like a battery icon) so each slide reads "~40% green" on its own, without comparing to a slide seen minutes ago.

## States across the deck

- **Slide 1 — big, whole, all-grey (0%), sailing. No text.** Establishes the silhouette so the corner meter is legible. The Theseus question is **spoken, not printed** — the image poses it, the voice asks it.
- **Corner, every slide — fills grey→green bit by bit**, reaching **~half green by the close** (= the 50% from the Bit 4 dashboard). Wordless.
- **Closing card after Slide 24 — big, ~half-green, sailing, wordless.** Literal last image; holds through Q&A. NOT full/finished — a finished ship would claim a completion that didn't happen and restore the cut victory lap.

## When the corner ship drops away

The motif yields whenever a slide needs to breathe — **data-dense slides drop it.** Clearest case: **Slide 23** (the full-bleed ~50% dashboard, the deck's peak). The break is itself a signal: *this slide is real, not metaphor.*

## What we deliberately did NOT do

- **No seam / transition cards.** The corner meter does the bit-to-bit orientation; dedicated boundary slides aren't needed. (Earlier plan; dropped once the corner became the meter.)
- **No full/finished ship anywhere.** Max state is ~half-green — matches the honest 50%.
- **No words on any ship appearance.** All wordless — no slogan, no "selling the story back."

## Cross-references

- `bit1.md` Slide 1 — big establishing grey ship.
- `bit4.md` Slide 23 — corner ship dropped, full-bleed dashboard.
- `bit5.md` Finale — wordless closing ship card after Slide 24.
- `slides/bit3.md` Slide 11 — the *scene* ship (engine-swap-at-sea): same ship in action, a separate job from the progress meter. Should visibly be the same ship.
