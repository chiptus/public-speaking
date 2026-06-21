# Public Speaking & Storytelling

A working repo for building conference/meetup talks — slides, scripts, rehearsal notes, and the reference material behind them. One folder per talk, past and future.

## Layout

```
.
├── ck/                                  # reference library (talk-craft books)
├── angularjs-react how to move a mountain/   # a talk (see its own README)
└── .claude/                             # Claude Code config for this repo
```

- **Each talk gets its own top-level folder.** It holds the slides, the speaker notes, design rationale, rehearsal sheet, and any assets (screenshots, video takes, exports).
- **`ck/`** is the shared reference shelf — books on tech-talk structure and storytelling that inform every talk:
  - `giving-a-30-min-tech-talk.md` — primary reference for technical talks (structure, slides, demos, timing)
  - `ted-talks-official-guide-anderson.epub` · `talk-like-ted-gallo.epub` — TED methodology (story principles; TED-specific rules don't all apply to long tech talks)
  - `Building a StoryBrand 2.0 - Donald Miller.epub` · `rodriguez-brand-storytelling-2nd-ed-2023.pdf` · `milligan-launch-your-platform-2024.epub` — narrative & brand storytelling

## Conventions

- Slide content lives in plain markdown, split into "bits" (sections), so it diffs cleanly and stays designer-/speaker-readable.
- The *why* behind editorial choices is kept in a separate `design-notes.md`, so slide files stay clean handoff specs.
- Video takes (`*.mp4`) are git-ignored; transcripts (`.txt`) are tracked.

## Talks

| Talk | Status | Folder |
| --- | --- | --- |
| AngularJS to React: How to Move a Mountain Incrementally | in rehearsal | [`angularjs-react how to move a mountain/`](./angularjs-react%20how%20to%20move%20a%20mountain/) |
