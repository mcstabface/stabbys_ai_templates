Checkpoint rule:
Identify a stopping point only when the work has reached a stable, resumable state and enough meaningful progress has been completed to justify a session artifact.

Do not suggest a new chat for:
- trivial patches
- single small fixes
- momentary stability after one change
- minor decisions that do not affect future work

Do suggest a new chat only when one or more of the following is true:
- a meaningful feature slice is complete and verified
- a multi-step patch sequence is complete and verified
- a meaningful bugfix batch is complete and the system is stable
- an evaluation or validation cycle is complete and has produced results that shape the next step
- a significant architectural or process decision has been settled
- the conversation is becoming degraded and there is already enough completed work to create a clean handoff artifact

When identifying a checkpoint, provide:
1. why this is a clean stopping point
2. what should be captured in the session artifact
3. the exact next recommended step

Default behavior:
Prefer continuing the current chat unless there is a clear handoff benefit.
