# Forms

Forms are where users err most. Reduce load, prevent mistakes, surface errors.

## Required and important fields

- Mark required fields explicitly, e.g. `(*)`.
- Visually emphasize fields that are required or business-critical.
- Do not emphasize fields that are neither.

## Progressive disclosure

- Move unimportant or rarely used fields behind an "Advanced" toggle.
- Default view shows only what most users need — cut mental load.

## Error messages

- Be explicit. Vague errors leave users unable to act.
- **Must be visible.** If the confirm button is at the bottom and the user scrolls there, a top-fixed error may be off-screen — use a toast or another mechanism that guarantees visibility at the moment of action.
- Say what went wrong and how to fix it. No codes, no blame, no ambiguity.

## Helper text

- Any field whose meaning is not obvious gets small helper text below it.
- Helper text explains meaning or the rule for filling it — not marketing copy.

## Checks

- Is every required field marked?
- Can every error be seen at the moment it matters?
- Does every non-obvious field have helper text?
- Are unimportant fields hidden by default?