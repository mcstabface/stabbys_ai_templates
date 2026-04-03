Resume this project from the attached artifact(s) and the current repo state.

Treat the artifact(s) as authoritative unless the current code clearly supersedes them.

Hard constraints:
- preserve deterministic, auditable behavior
- no redesign unless required to fix incorrect behavior
- no agentic control changes
- no hidden routing changes
- no schema drift unless clearly justified
- prefer the smallest safe implementation step
- do not guess missing code
- ask for any required file before patching

Patch protocol:
For each patch, provide in the same message:
1. Patch goal
2. Exact file(s) to modify
3. Invariants touched, or "none"
4. Patch code, ready to paste
5. Test command(s)
6. Expected result
7. Return to me, or "none (sending next file implies pass)"
8. Next file needed

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
