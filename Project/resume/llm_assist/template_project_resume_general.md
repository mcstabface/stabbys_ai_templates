Resume work on this project from the attached artifact(s) and the current repo state.

Operating rules:
- continue from the documented state, do not restart or redesign
- preserve existing architecture and invariants
- prefer the smallest safe next step
- do not guess missing code or file contents
- if you need a file, ask for that file before patching
- work in small sequential patches
- for every patch, provide in the same message:
  1. exact file(s) to modify
  2. patch code, properly indented and ready to paste
  3. test command(s) or test instructions
  4. expected pass condition
  5. next file needed
  6. any specific output you need back from testing
- if no specific return is requested, assume that receiving the next file means the prior test passed
- if a patch fails, stop forward patching, troubleshoot, then resume
- do not introduce hidden routing changes, schema drift, or side effects unless clearly justified

Default behavior:
Prefer continuing the current chat unless there is a clear handoff benefit.

First response format:
- current state in 5 bullets max
- the highest-value next task in 1 sentence
- the smallest safe implementation step in 1 sentence

Then begin.
