---
name: as-a-user
description: Design, review, and verify user interfaces through human characteristics and task goals. Use when creating UI, evaluating usability, or exercising software through a browser or computer use to verify task completion and interaction quality.
---

# as-a-user

Help people complete their goals with an interface they can understand, operate, and recover from. Ground decisions in the user's task and circumstances.

## Human model

People have limited attention and working memory, use experience to form expectations, and can make slips or misunderstand rules. They also learn, develop expertise, and need control over consequential choices. Abilities, motivation, devices, and interruptions vary by situation; do not assume a universally impatient or inexperienced user.

## Shared reasoning chain

**User and context → task → relevant human characteristic → likely difficulty → design response → verification.**

Use this chain for consequential choices and findings, not for every element:

1. Establish the goal, experience level, and relevant conditions from available evidence. State material assumptions; ask only when missing context would change the decision.
2. Select the human characteristics that matter here. Explain how they affect this task before choosing a UI pattern.
3. Choose a response that reduces total effort and error cost, including understanding, action, and recovery. Preserve information, learning, and deliberation the task needs; fewer fields or clicks are not goals by themselves.
4. Specify an observable way to check whether the response helps. Distinguish a proposed check from one actually performed.

Example: interrupted order entry → limited working memory → returning to the wrong order → retain the draft and keep order identity in context → check that someone can resume the correct order without re-entering data.

## Modes

**`as-a-user · design`** — Use the chain to produce the requested design: structure, actions, and task-relevant states and recovery paths. Briefly explain key choices and tradeoffs. Make information perceivable and controls operable across relevant input methods and assistive technology; do not rely on color alone.

**`as-a-user · review`** — Walk relevant tasks using the available interface or artifacts. Select scenarios that matter: first use, practiced use, interruption, or failure recovery. Report actionable findings as:

**Scenario/location and evidence → relevant human characteristic and likely impact → fix → verification.**

- Separate observed facts, inferences, and untested assumptions. Do not present imagined feelings as user research. Screenshots support static observations, not claims about runtime behavior.
- Rank severity by task obstruction, error consequences, affected scope, and recovery difficulty: blocker / major / minor / polish. State evidence confidence separately; distinguish preferences from problems.
- Summarize coverage and material unknowns. Heuristic review does not replace testing with real users.

**`as-a-user · verify`** — Read [Verification](references/verification.md). Actually exercise each in-scope feature as a user task through the interface, then check the final outcome against explicit expectations. Report functional results separately from human-centered usability findings, with evidence and coverage gaps. Use the current model for planning and acceptance; delegate bounded execution to a qualified lower-cost model only when supported, without weakening evidence or acceptance standards.

## References

Load only what the task needs:

- [Human model](references/mental-model.md) — selecting relevant characteristics and applying the chain.
- [Layout and hierarchy](references/layout-and-hierarchy.md) — attention, grouping, orientation, and expertise.
- [Forms](references/forms.md) — field visibility, instructions, errors, and preserving effort.
- [Feedback and interaction](references/feedback-and-interaction.md) — truthful status, control, and recovery.
- [Verification](references/verification.md) — real operation, task closure, evidence, and model cost allocation.
