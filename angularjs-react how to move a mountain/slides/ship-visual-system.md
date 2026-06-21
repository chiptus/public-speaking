# Ship visual system (recurring)

**Decided 2026-05-30** (colors revised 2026-06-02). Source of truth for how the Ship-of-Theseus motif appears across the deck. Per-slide files reference it. The *why* lives in `../design-notes.md`.

## The one metaphor, two scales

| | Corner progress ship | Big bookend ships |
|---|---|---|
| **Job** | Ambient orientation — "how far are we" | The emotional / identity beats |
| **Size** | Small, top-right corner | Large |
| **Where** | Almost every slide | Slide 2 (open) + closing card (after Slide 24) |

Both use the **same visual language**: a whole, sailing ship whose planks color-fill from **Angular-red → React-blue** (their real brand colors — AngularJS red, React blue). They differ only in size and how many planks have turned.

## Color-fill, not build-up

- Ship is **always whole and sailing.** Progress = planks changing **color** (red → blue), never planks *added* to an empty frame.
- Fill is **chunky, per-bit** (5 bits = ~5 perceptible steps), not plank-by-plank — a 30px icon can't show fine change.
- Always fill *within a fixed full silhouette* (like a battery icon) so each slide reads e.g. "~40% blue" on its own, without comparing to a slide seen minutes ago.

## States across the deck

- **Slide 2 — big, whole, all-red (0% migrated), sailing. No text.** Establishes the silhouette so the corner meter reads later. _(Slide 1 is now the codebase/problem; code-first open, revised 2026-06-09.)_
- **Corner, every slide — fills red→blue bit by bit**, advancing toward the finale state by the close. Exact fraction is **symbolic, not a literal meter** — no one counts planks. Wordless.
- **Closing card after Slide 24 — big, well-progressed (more blue than red), sailing, wordless.** Literal last image; holds through Q&A. **Not all-blue / finished** — it shouldn't read as *done*.

## When the corner ship drops away

Data-dense slides drop it — clearest case **Slide 23** (full-bleed ~50% dashboard, the deck's peak). The break is the signal: *this slide is real, not metaphor.*

## Don'ts

- **No words on any ship**, ever — every appearance wordless.
- **No full/finished (all-blue) ship** anywhere.
- **No seam / transition cards** — the corner meter does the bit-to-bit orientation.

## Cross-references

- `bit1.md` Slide 2 — big establishing red ship.
- `bit4.md` Slide 23 — corner ship dropped, full-bleed dashboard.
- `bit5.md` Finale — wordless closing ship card after Slide 24.
- `bit3.md` Slide 11 — the *scene* ship (engine-swap-at-sea): same ship in action, a separate job from the meter. Must visibly be the same ship.
