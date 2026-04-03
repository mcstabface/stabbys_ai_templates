Create a session continuity artifact for this conversation.

Purpose:
- capture the current verified system state
- preserve the architectural decisions made
- record what was completed
- record what remains
- make it easy to resume in a new chat without relying on conversation history

Requirements:
- treat this as a continuation artifact, not a narrative summary
- write in markdown
- be concrete and specific
- distinguish clearly between:
  - completed and verified
  - partially implemented
  - proposed but not implemented
- do not invent progress
- do not claim anything was tested unless it was actually tested
- do not omit important caveats, failures, or known issues
- preserve architectural invariants and ownership boundaries
- prefer explicit state over polished wording

Include these sections:

1. Title
2. Date
3. Status
4. Scope of this session
5. Objective of the session
6. What was completed
7. What was verified
8. Files/modules touched
9. Architectural decisions or invariants affected
10. Current system state
11. Known issues / risks / limitations
12. Exact next recommended step
13. Resume instruction for the next chat

Output requirements:
- provide a recommended filename
- make the artifact clean enough to save directly into the project
- end with a short resume prompt that can be pasted into a new conversation

Before finalizing:
- separate facts from interpretation
- remove fluff
- make sure the next step is the smallest safe next step
