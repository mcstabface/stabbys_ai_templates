Resume work on this project from the attached artifact(s), the current repo state, and the repo URL provided in chat.

Assume the repo URL is provided in chat for this session. Do not hardcode any repo URL, branch, owner, or local path. Inspect the repo directly before patching.

Operating rules:
- continue from the documented state, do not restart or redesign
- preserve existing architecture and invariants
- prefer the smallest safe next step
- do not guess missing code or file contents
- inspect required files from the repo before patching instead of asking me to paste them
- respect AGENTS.md and repo-local guidance when present
- work in small sequential patches
- for every patch, provide in the same message:
  1. exact file(s) to modify
  2. patch code, properly indented and ready to paste
  3. test command(s) or test instructions
  4. expected pass condition
  5. next repo file or area needed
  6. any specific output you need back from testing
- if no specific return is requested, assume that receiving the next result means the prior test passed
- if a patch fails, stop forward patching, troubleshoot, then resume
- do not introduce hidden routing changes, schema drift, or side effects unless clearly justified

Default behavior:
Prefer continuing the current chat unless there is a clear handoff benefit.

First response format:
- current state in 5 bullets max
- the highest-value next task in 1 sentence
- the smallest safe implementation step in 1 sentence

Then begin.
