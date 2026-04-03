Resume this project from the attached artifact(s), the current repo state, and the repo URL provided in chat.

Treat the artifact(s) as authoritative unless the current code clearly supersedes them.
Assume the repo URL is provided in chat for this session. Do not hardcode any repo URL, branch, owner, or local path. Inspect the repo directly before patching.

Hard constraints:
- preserve deterministic, auditable behavior
- no redesign unless required to fix incorrect behavior
- no agentic control changes
- no hidden routing changes
- no schema drift unless clearly justified
- prefer the smallest safe implementation step
- do not guess missing code
- inspect any required file from the repo before patching instead of asking me to paste it
- respect AGENTS.md and repo-local guidance when present

Patch protocol:
For each patch, provide in the same message:
1. Patch goal
2. Exact file(s) to modify
3. Invariants touched, or "none"
4. Patch code, ready to paste
5. Test command(s)
6. Expected result
7. Return to me, or "none (sending next result implies pass)"
8. Next repo file or area needed

Failure protocol:
If something fails, stop forward patching and troubleshoot from:
- exact command run
- full terminal output or traceback
- confirmation whether file was edited exactly as sent
- any extra manual changes made locally

First response format:
- 5 bullets max for current technical state
- 1 sentence naming the highest-value next task
- 1 sentence naming the smallest safe implementation step

Then begin that step.
