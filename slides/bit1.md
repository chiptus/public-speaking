# Bit 1 — Opening (Slides 1–4)

> ~3 min. Code-first: problem → ship → intro → room. Slow · full stops · let silence sit.
> 🔒 = say verbatim · **Speak** = say live (prompt, not script) · _Cue_ = staging, never spoken. Rationale → `design-notes.md`.

## title

- **Visual:** Title on slide: **"AngularJS to React: How to Move a Mountain Incrementally"**
- **Notes:**
  - 🔒 _"היום אני אראה לכם איך מעבירים מוצר גדול מ-פריימורק מת — בלי לכתוב אותו מחדש."_ → straight to S1.
    - _(EN, meaning-check: today I'll show you how you move a large product off a dead framework — without rewriting it.)_
  - _Cue:_ don't read the title — it's on the slide. One line, ~10s, memorize only this, then go to the code. Not an agenda; "5 years / still shipping" pays off at S1/S23, don't front-load.

## Slide 1 — The codebase (the problem)

- **Visual:** Screenshot of a real AngularJS controller — the feeling of scale, not reading code. One callout: **391 components**.
- **Notes:**
  - 🔒 ככה נראה הקוד שלנו באנגולר — קונטרולרים ענקיים, כמעט לא מפורקים לקומפוננטות, הרבה כפילויות. 391 קומפוננטות להגר. התחלנו להעביר את זה לריאקט לפני חמש שנים. זה עדיין לא נגמר
  - _Cue:_ 391 = stakes, not a metric · let "no ending" sit.

## Slide 2 — The ship (the question)

- **Visual:** Big red ship (all-red = 0% migrated), whole, sailing. No text.
- **Notes:**
  - 🔒 יש שאלה ישנה — אם מחליפים את כל הקרשים של ספינה, אחד אחד, האם זו עדיין אותה ספינה? זאת בדיוק השאלה ששאלתי על האפליקציה שלנו: איך בונים אותה מחדש בפריימוורק חדש — בלי לשנות אותה?
  - _Cue:_ never say "Ship of Theseus" · ask, then stop.

## Slide 3 — Self-intro + setup

- **Visual:** Chaim Lev-Ari / Software developer, Portainer.io
- **Notes:**
  - 🔒 שמי חיים, אני מפתח בפורטיינר מאז 2018 — פלטפורמה לניהול קונטיינרים.
  - **Speak** (flat, own lines): 3–4 devs then · ~10–15 now · "led it largely on my own" · "never the priority"
  - _Cue:_ slow, flat · "never the priority" pays off at S24.

## Slide 4 — To the room

- **Visual:** The Slide 1 codebase screenshot, brought back as a callback — so "code like this" has something to point at. The springboard into Bit 2.
- **Notes:**
  - Someone who was/is in this situation? Who had an old legacy code and wanted to migrate from it?
  - 🔒 אז רציתי לספר לכם שזה אפשרי.
  - _Cue:_ to the room, then stop.
  - **→ Bridge → Bit 2 (say live):** _"לא עברנו בגלל הבלגן בקוד — לקוד מבולגן עושים ריפקטור. אז למה כן עברנו?"_ → S5.
    - _(EN, meaning-check: we didn't move because of the messy code — messy code you refactor. so why did we move?)_
    - _Cue:_ pose the question, don't answer it — S5 is the payoff.

_(Rationale, build behavior, design history → `design-notes.md`.)_
