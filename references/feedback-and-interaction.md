# Feedback and interaction

The user cannot see behind the page. Every action must produce a visible result.

## Action feedback

- Buttons need **pressed / released** states — the user must feel the click.
- Any action that changes state (save, submit, delete, sync) must surface a visible result: success, failure, or progress.
- Silence reads as "nothing happened" or "it broke."

## States to design

- Default
- Loading / in-progress
- Empty
- Error
- Success

If a state can occur, it must be designed — not left to chance.

## Simplicity

- Internal complexity is acceptable; **surface complexity is not**.
- Present the shortest correct path. No detours, no unnecessary steps.
- Design from first principles: what does the user actually need to accomplish here?
- If a flow needs explanation, it's too complex.

## Checks

- Does every button show pressed/released?
- Does every state-changing action show a result?
- Can the user tell, at all times, what just happened and what's next?
- Is there any step that exists for the system's convenience, not the user's?