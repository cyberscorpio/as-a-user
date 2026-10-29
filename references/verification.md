# Verify through real use

**Task and expected outcome → discover the entry → operate the interface → observe feedback → verify the final outcome → assess human difficulty.**

## Establish coverage

- Build a feature-to-task inventory from requirements, documentation, and the application. Include required but missing features; menus alone cannot establish completeness. State the scope and material assumptions.
- For each feature, define the user role, starting conditions, expected outcome, and evidence needed before execution. Exercise a complete normal path, plus relevant role differences, invalid input, interruption, or recovery based on consequences. Do not imply every combination was tested.
- Record the environment/version and test data needed to reproduce results. Prefer recoverable test environments and fixtures; stay within authorized actions and restore test state where appropriate. If an action requires authorization not already given, stop that action and continue unaffected tasks.

## Operate from the user's position

- Use available browser automation or computer-use tools to interact with the real interface. Start from a discoverable entry and use labels, instructions, and feedback available to the intended user. Check whether choices require guessing or remembering unavailable context.
- Code, APIs, and logs may help prepare fixtures or investigate outcomes; they cannot replace the UI path under test. Record hidden URLs, backend fixes, or other workarounds as bypasses. A bypass cannot turn the original failed path into a pass.
- Observe after meaningful actions and before dependent ones. Keep one operator per shared browser/desktop session; separate sessions and fixtures if independent tasks run concurrently.
- Stop and return evidence when the state or target is unclear, an unexpected consequence appears, or a bounded retry allowance is exhausted. Set step/time/retry limits appropriate to the task; report unfinished coverage instead of silently skipping it.

## Verify closure and retain evidence

- Check the actual outcome, not just a click, HTTP success, toast, or executor's completion claim. Reopen or refresh saved work where relevant; inspect generated artifacts and exercise the necessary downstream step. Distinguish accepted, pending, completed, and unknown results.
- Retain reproducible action traces and evidence at consequential checkpoints: screenshots, accessible page state, saved records, or output artifacts. Tie evidence to the task, test object, and run. Use authorized read-only system evidence when needed to corroborate the result; it does not excuse missing UI feedback.
- Separately assess discovery, understanding, effort, control, and recovery using the shared human reasoning chain. Distinguish observed friction from predicted human difficulty; automated execution does not establish how real users feel.

Example: create a record through the UI, recover from a relevant validation error, submit, reopen the record, check its values, and continue its intended next operation. A success toast alone leaves persistence and the task's continuation unverified.

## Allocate models without lowering accuracy

- The current model owns scope, acceptance criteria, scenario selection, anomaly analysis, and final judgment. A lower-cost model may execute bounded tasks and collect evidence only when the runtime supports delegation and the model can use the required tools.
- Give the executor the goal, role, starting state, expected checkpoints, evidence requirements, and stopping conditions. Avoid prescribing every click when discoverability itself is being tested.
- Qualify cheaper execution on representative tasks against a trusted baseline, checking missed failures and false passes as well as completion. Select the lowest-cost model that meets the same quality bar; include retries and review overhead in cost.
- The current model inspects underlying evidence for acceptance, not just the executor's summary. Missing or contradictory evidence requires more observation or a rerun. Escalate ambiguous states, unexpected behavior, and repeated failures to the current model; a stronger reviewer cannot reconstruct evidence that was never collected.
- If delegation or a qualified cheaper model is unavailable, execute with the current model and disclose the actual allocation. Never claim a model switch that did not occur, weaken acceptance criteria, or mark omitted work as passed to save cost.

## Report

Use a compact ledger: **feature/task | expected outcome | actual outcome and evidence | status | usability finding**.

- **Passed:** executed and supported by sufficient evidence for the stated criteria.
- **Failed:** observed behavior contradicts an acceptance criterion; retain reproduction evidence.
- **Blocked:** a prerequisite, tool limitation, or unresolved evidence gap prevents a conclusion.
- **Not run:** not executed; state why.

Report counts against the inventory, material scenario gaps, environment, and actual model allocation. Rank usability findings by impact separately from functional status. After a fix, rerun the affected path and relevant dependencies, preserving the original failure and the new evidence. Do not claim completeness beyond the verified scope.
