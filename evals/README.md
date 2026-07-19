# Quality Checklists (Evals)

How do you know the assistant is doing its job well? This folder holds simple pass/fail checklists — one row per thing that should be true about a good research brief, fact-check, Did You Know list, illustration prompt, or session.

## Two ways to use these

### 1. As a printable checklist (no tech needed)

Open any file in the `rubrics/` folder, and as you read the assistant's output, tick each row off. Every row has a "What pass requires" column that tells you exactly what to look for. If a row fails, that's your cue to push back — e.g. *"Some of these facts don't have sources — can you add them or flag them?"*

### 2. As an automatic check (let an AI grade it)

You can ask a second AI conversation to grade the first one's work:

1. Copy the finished output (say, a research brief) into a new conversation.
2. Copy in the matching rubric file.
3. Paste this grading prompt:

> You are a careful editorial evaluator for a children's book project. You will receive a piece of assistant output and a rubric of criteria. For each criterion, decide pass or fail: pass means the criterion is clearly and fully met; fail means it is absent, incomplete, or only partially met. Respond with one line per criterion: the ID, PASS or FAIL, and a one-sentence explanation. Then give a short overall summary of what needs fixing.

4. Take the failures back to your writing session and ask the assistant to address them.

## What's here

| File | Checks the quality of… |
|------|------------------------|
| `rubrics/process.csv` | The session itself — did the assistant follow the workflow and respect the author's role? |
| `rubrics/research-brief.csv` | A research brief |
| `rubrics/fact-check.csv` | A fact-check pass |
| `rubrics/did-you-know.csv` | Did You Know candidates |
| `rubrics/illustration-prompt.csv` | An illustration prompt |

Each CSV has the same columns: **ID** (a short label), **Criterion** (what's being checked), **What pass requires** (the exact, checkable condition), and **Notes** (why it matters).

These checklists are a floor, not a ceiling — an output can pass every row and still deserve another draft. Your judgment as the author always wins.

<sub>Curious how this kind of checklist works elsewhere? [One example from the education world.](https://github.com/anthropics/k12-teacher-skills/tree/main/evals)</sub>
