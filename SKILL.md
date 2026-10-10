---
name: as-a-user
description: Design and review UI from a real user's position. Use when generating or auditing interfaces — the same user-first logic applies to both. The bar is whether users can complete their goal, not whether features exist.
---

# as-a-user

Design and review UI as a real user would. Not as a system builder, not as a feature list.

## The human model (why this works)

A real user **assumes, errs, and has no patience**. They receive information far slower than an LLM, remember poorly, and can only understand the system through what is visible on the page. Sometimes they form muscle memory.

Design for that person — not for an idealized careful reader.

Core traits to design against:
- **Assumes** — fills gaps with guesses, often wrong.
- **Errs** — misclicks, mistypes, misreads.
- **Impatient** — won't read, won't hunt, won't wait.
- **Slow intake** — needs hierarchy to know what matters first.
- **Forgetful** — can't hold context across screens or steps.
- **Blind to internals** — only sees what's rendered; never knows what happened behind the page.
- **Muscle memory** — repeats familiar patterns; consistency beats cleverness.

## Principles

1. **Structure every page.** Group elements by content, order by importance, separate groups with clear boundaries, and use size/color so the eye catches the priority first.
2. **Tame forms.** Highlight what's required or business-critical. Hide the rest behind "Advanced". Mark required fields (*). Give explicit, visible error messages — never vague, never off-screen. Label any non-obvious field with small helper text.
3. **Always respond to action.** Buttons need pressed/released states. Any action that changes state must surface a visible result — the user cannot see behind the page.
4. **Keep interaction simple.** Internal complexity is fine; the surface must be obvious. Design from first principles, not from implementation convenience.

## Modes

**`as-a-user · design`** — while generating UI. State who the user is, the context, and the goal; then produce structure, primary action, and states (default / loading / empty / error / success). Justify each key choice from the user's side.

**`as-a-user · review`** — while auditing UI. Walk the main flow as a first-time user. Report friction as: symptom → user feeling → impact → fix. Rank by severity (blocker / major / minor / polish). Separate real problems from preferences.

## References

Load only what the task needs:
- `references/mental-model.md` — the human traits, expanded, with design implications.
- `references/layout-and-hierarchy.md` — grouping, ordering, boundaries, emphasis.
- `references/forms.md` — required fields, progressive disclosure, errors, helper text.
- `references/feedback-and-interaction.md` — action feedback, states, simplicity.

## Anti-patterns

- Treating "feature works" as "UI is good."
- Assuming the user reads instructions.
- Hiding errors where the user won't see them.
- Clever layouts that break muscle memory.
- Adding surface complexity to match internal complexity.