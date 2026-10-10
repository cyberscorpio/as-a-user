# as-a-user

**Design and review UI as a real user would.**

`as-a-user` is a skill that makes AI think and judge interfaces like a real person — not like a system builder, and not like a feature list.

It shares **one logic** across two modes:

- **`as-a-user · design`** — while generating UI, make choices *for* the user.
- **`as-a-user · review`** — while auditing UI, find friction *for* the user.

The bar is always the same: **can users complete their goal?** — not whether the features exist.

---

## Why

AI writes UI that works but doesn't feel good to use. Features are all there; the experience isn't.

The reason is simple: AI reasons like a machine, not like a person. A real user:

- **assumes** — fills gaps with guesses, often wrong
- **errs** — misclicks, mistypes, misreads
- **has no patience** — won't read, won't hunt, won't wait
- **takes in information slowly** — needs hierarchy to know what matters first
- **forgets** — can't hold context across screens or steps
- **is blind to internals** — only sees what's rendered, never what happens behind the page
- **forms muscle memory** — repeats familiar patterns; consistency beats cleverness

`as-a-user` encodes that model so AI designs and audits against it.

---

## What it does

Four principles, applied in both modes:

1. **Structure every page.** Group by content, order by importance, separate groups clearly, use size and color so the eye catches priority first.
2. **Tame forms.** Mark required fields (*), hide the rest behind "Advanced", give explicit and visible errors, add helper text to any non-obvious field.
3. **Always respond to action.** Buttons need pressed/released states; any state change must surface a visible result.
4. **Keep interaction simple.** Internal complexity is fine; the surface must be obvious. Design from first principles.

---

## Usage

### Design mode

> Design this screen with `as-a-user`. First state who the user is, the context, and their goal. Then give the structure, the primary action, and the key states (default / loading / empty / error / success). Justify each key choice from the user's side.

### Review mode

> Review this UI with `as-a-user`. Walk the main flow as a first-time user. Point out where I'd be confused, stuck, or unsure whether it worked. Report each issue as symptom → user feeling → impact → fix, ranked by severity.

---

## How the two modes relate

as-a-user (one principle: stand in the real user's position)
├── design → make choices for the user
└── review → find friction for the user


Same logic, two outputs. Because the criteria are identical, design and review never contradict each other.

---

## Structure

as-a-user/
├── SKILL.md # compact: model, principles, modes, index
└── references/
├── mental-model.md # the human traits, expanded
├── layout-and-hierarchy.md # grouping, ordering, boundaries, emphasis
├── forms.md # required fields, disclosure, errors, helper text
└── feedback-and-interaction.md # action feedback, states, simplicity


`SKILL.md` stays short. Details load on demand from `references/`.

---

## Anti-patterns

- Treating "the feature works" as "the UI is good."
- Assuming the user reads instructions.
- Hiding errors where the user won't see them.
- Clever layouts that break muscle memory.
- Matching surface complexity to internal complexity.

---

## Background

`as-a-user` follows the spirit of **human-centered design** — but as a lightweight, callable perspective rather than a full methodology. It's the "stand in the user's shoes" layer, made available at both generation time and review time.

---

## License

MIT