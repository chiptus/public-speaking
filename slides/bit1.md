# Bit 1 — Opening (Slides 1–4)

> ~3 min. Code-first: problem → ship → intro → room. Slow · full stops · let silence sit.
> 🔒 = say verbatim · **Speak** = say live (prompt, not script) · _Cue_ = staging, never spoken. Rationale → `design-notes.md`.

## title

- **Visual:** Title on slide: **"AngularJS to React: How to Move a Mountain Incrementally"**
- **Notes:**
  - **Speak:** _"how we've been moving a large product off a dead framework — incrementally, five years, still shipping."_
  - _Cue:_ ~10s, then go to the code. Not an agenda.

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
  - **→ Bridge → Bit 2 (say live):** _"לא עברנו בגלל הבלגן בקוד — לקוד מבולגן עושים ריפקטור. עברנו כי AngularJS עצמו הגיע לסוף הדרך."_ → S5.
    - _(EN, meaning-check: we didn't move because of the messy code — messy code you refactor. we moved because AngularJS itself had reached the end of the road.)_
    - _Cue:_ hand straight to S5's "why" — don't preview "one decision" (that's Bit 2's thesis → lives at S6/S8).

_(Rationale, build behavior, design history → `design-notes.md`.)_
