# The human mental model

Design targets a person who **assumes, errs, and has no patience**.

## Traits and design implications

| Trait | What it means | Design implication |
|---|---|---|
| Assumes | Fills missing info with guesses | Never rely on inference; make state and meaning explicit |
| Errs | Misclicks, mistypes, misreads | Make errors easy to prevent, easy to recover |
| Impatient | Won't read, hunt, or wait | Put the answer where the eye lands; no hidden paths |
| Slow intake | Processes far slower than an LLM | Use hierarchy: size, color, spacing to signal priority |
| Forgetful | Can't hold context across steps | Show context in place; don't make them remember |
| Blind to internals | Only sees the rendered page | Surface every result and state change visibly |
| Muscle memory | Repeats familiar patterns | Keep placement and behavior consistent |

## The visibility rule

The user knows the system **only through what is on the page**.
Anything happening behind it — saving, syncing, failing — is invisible unless you show it.

## The patience rule

Every moment spent thinking "what does this mean?", "where do I click?", "did it work?" is a defect.
Good UI removes those moments; it does not explain them away.