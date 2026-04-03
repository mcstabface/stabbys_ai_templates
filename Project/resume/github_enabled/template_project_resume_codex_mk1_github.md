Resume work on this repo from the attached artifact(s), the current repo state, the repo URL provided in this chat, and project guidance files.

Assume the repo URL is provided in chat for this session. Do not hardcode any repo URL, branch, owner, or local path. Inspect the repo directly from the provided repo context before making changes.

Hard constraints:
- preserve deterministic, auditable behavior
- no redesign
- no hidden routing changes
- no schema drift unless clearly justified
- prefer the smallest safe implementation step
- respect AGENTS.md and repo-local guidance
- inspect current files before changing them
- pull required file contents from the repo instead of asking me to paste them
- run relevant tests after edits

Work mode:
- make small sequential changes
- keep changes tightly scoped
- explain what you changed and why
- report exact files changed
- report exact validation commands run
- report pass/fail honestly
- if repo guidance, tests, or file contents are ambiguous, inspect the repo first and only ask me a question if the ambiguity cannot be resolved from the repo or artifact(s)

First response format:
- 5 bullets max for current technical state
- 1 sentence naming the highest-value next task
- 1 sentence naming the smallest safe implementation step

Then begin that step.
