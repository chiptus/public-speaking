# Public Speaking, Storytelling & Lectures — Topic Folder

Books on TED-style talks, storytelling frameworks, brand narrative, and delivering technical lectures.

## Rules

- no walls of text. if something isn't clear I'll ask
- criticize, think outside the box, tell me if I'm wrong.
- The talk is a 30–40 min technical talk, NOT a TED talk. Favor depth over cutting — teaching code/details is allowed. Primary reference: Giving a 30-Minute Tech Talk (not Anderson/Gallo). Story principles (one spine, real vulnerability, don't announce the moral) still apply; TED-specific rules (18-min cut, Rule of Three, no slides) do not.

---

## Books

| Book                                                            | CandleKeep ID               | Local File                                       | Focus                                                      |
| --------------------------------------------------------------- | --------------------------- | ------------------------------------------------ | ---------------------------------------------------------- |
| TED Talks: The Official TED Guide to Public Speaking (Anderson) | `cmppjqsiu22ljrt0zqki0zovq` | `ted-talks-official-guide-anderson.epub`         | TED methodology — idea delivery, structure, stage presence |
| Talk Like TED (Gallo)                                           | `cmppjr2qq22lvrt0zge89z2li` | `talk-like-ted-gallo.epub`                       | 9 public-speaking secrets of top TED speakers              |
| Giving a 30-Minute Tech Talk                                    | `cmppjr2w822lzrt0zl50fgpxy` | `giving-a-30-min-tech-talk.md`                   | Technical talk structure, slides, demos, timing            |
| Building a StoryBrand 2.0 (Donald Miller)                       | `cmppjr6h122m7rt0zz31nzlhc` | `Building a StoryBrand 2.0 - Donald Miller.epub` | 7-part narrative framework for messaging clarity           |
| Brand Storytelling 2nd ed (Rodriguez, 2023)                     | `cmppjr6ii22mfrt0zl1vhe853` | `rodriguez-brand-storytelling-2nd-ed-2023.pdf`   | How to use stories to grow a business                      |
| Launch Your Platform (Milligan, 2024)                           | `cmppjrb8s22mvrt0zn9lpruvv` | `milligan-launch-your-platform-2024.epub`        | Personal brand, writing, coaching, speaking as a creator   |

---

## Ask Claude to research

- "What's the TED framework for structuring a talk?" — Anderson, Gallo
- "How do I open a talk with a strong hook?" — Gallo, Anderson
- "How do I structure a 30-minute technical lecture?" — Giving a 30-Minute Tech Talk
- "What is the StoryBrand framework?" — Miller
- "How do I use storytelling in a business presentation?" — Rodriguez, Miller


---

# MANDATORY: Post-Task Documentation (SR-PTD)

**CRITICAL: After completing ANY task that modifies files, you MUST invoke this skill:**

```
Skill tool -> skill: "sr-ptd-skill"
```

**This is NOT optional. Skipping this skill means the task is INCOMPLETE.**

When planning ANY development task, add as the FINAL item in your task list:
```
[ ] Create SR-PTD documentation
```

### Before Starting Any Task:
1. Create your task plan as usual
2. Add SR-PTD documentation as the last task item
3. This step is MANDATORY for: features, bug fixes, refactors, maintenance, research

### When Completing the SR-PTD Task:
1. Read `~/.claude/skills/sr-ptd-skill/SKILL.md` for full instructions
2. Choose template: Full (complex tasks) or Quick (simple tasks)
3. Create file: `SR-PTD_YYYY-MM-DD_[task-id]_[description].md`
4. Save to: `C:/projects/Skills/Dev_doc_for_skills`
5. Fill all applicable sections thoroughly

### Task Completion Criteria:
A task is NOT complete until SR-PTD documentation exists.

### If Conversation Continues After Task:
Update the existing SR-PTD document instead of creating a new one.

---
