# as-a-user

**Design and review UI by connecting human characteristics to concrete decisions.**

People bring goals, experience, abilities, and expectations to an interface. Their attention and working memory are limited; they can be interrupted, make mistakes, learn, and develop expertise. `as-a-user` helps an agent reason from those characteristics in a specific task, without assuming every user has the same needs.

## One reasoning chain, two modes

**User and context → task → relevant human characteristic → likely difficulty → design response → verification.**

- **`as-a-user · design`** uses the chain to choose structure, actions, and relevant states and recovery paths.
- **`as-a-user · review`** uses it to connect observed interface behavior to likely task difficulties and actionable improvements.

For example, someone interrupted during order entry may lose track of the current order. Retaining their draft and keeping order identity in context supports resumption. Verify whether they can continue the correct order without re-entering data.

The aim is successful task completion with reasonable understanding, effort, and recovery cost. Fewer fields or clicks are useful only when they serve that goal. Necessary information, learning, and deliberate choices remain part of good design.

## Usage

### Design

> Use `as-a-user` to design this screen. Establish the user, task, and context; state material assumptions. Connect key choices to relevant human characteristics, include the states and recovery paths this task needs, and explain how to verify the choices.

### Review

> Use `as-a-user` to review this flow. Select relevant usage and recovery scenarios. For each actionable finding, give the location and evidence, human characteristic and likely impact, fix, and verification. Rank severity separately from evidence confidence and report material coverage gaps.

Review distinguishes observation, inference, and untested assumptions. A screenshot cannot establish runtime behavior, and an agent's prediction of a feeling is not user research. Heuristic review supports, but does not replace, testing with real users.

## Contents

- [SKILL.md](SKILL.md) — purpose, shared reasoning chain, and mode instructions.
- [Human model](references/mental-model.md) — contextual characteristics and contrasting examples.
- [Layout and hierarchy](references/layout-and-hierarchy.md) — attention, orientation, and experience.
- [Forms](references/forms.md) — visibility, input guidance, and error correction.
- [Feedback and interaction](references/feedback-and-interaction.md) — truthful status, control, and recovery.

References load only when relevant. The skill is a lightweight human-centered design perspective, not a full research methodology or accessibility audit.

## License

MIT
