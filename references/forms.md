# Forms

Connect field and validation choices to the task, likely misunderstandings, and the effort already invested.

## Deciding what to show

- Use task relevance, frequency, and consequences of omission to decide visibility. Optional does not mean unimportant; required does not automatically mean visually dominant.
- Fold away rarely needed detail only when people can discover it and understand whether it applies. Keep consequential choices and active errors discoverable.
- Make required status clear through a consistent convention and accessible semantics. Explain symbols if used.

## Supporting correct input

- Use familiar labels and place rules or examples where they inform entry. Improve an unclear label before adding more helper text.
- Distinguish typing slips from misunderstanding: a format hint may fix the former, while the latter needs an explanation of meaning or consequences.
- Choose validation timing that helps correction without interrupting unfinished input. Explain any automatic correction that changes meaning.

## Recovering from errors

- Identify what failed, associate the explanation with the field, and give an actionable correction when known. Technical codes may supplement, but cannot replace, that explanation.
- Keep errors available while correcting them. Use inline messages, a navigable summary, and appropriate focus management for the form; a transient toast alone does not ensure discovery or recovery.
- Make errors perceivable to assistive technology and avoid color-only signals. Preserve valid input and explain any information that cannot be retained.

## Verify the response

Try a relevant omission or invalid value: can the person locate and understand the problem, correct it using their input method, and continue without repeating completed work? Check folded fields in both the common task and the task that needs them.
