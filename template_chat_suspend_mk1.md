Create a continuation-ready session artifact for this conversation.

The artifact must be suitable for saving into the project and using as the authoritative starting point for the next chat.

Instructions:
- write in markdown
- prioritize accuracy over completeness theater
- do not guess
- do not smooth over uncertainty
- explicitly label:
  - completed
  - verified
  - in progress
  - deferred
- include only work that actually happened in this session
- if something was discussed but not implemented, say so plainly
- if something was implemented but not tested, say so plainly
- preserve architecture, invariants, ownership, and boundaries exactly as established
- keep the artifact useful for continuation, not presentation

Required sections:
1. Title
2. Date
3. Status
4. Session scope
5. Objective
6. Completed work
7. Verified behavior
8. Files or modules touched
9. Important implementation details
10. Current system state
11. Known issues / remaining work
12. Recommended next step
13. Safe stopping point
14. Resume instruction

Also include:
- recommended filename
- a final one-paragraph “bottom line”
- a copy-paste continuation prompt for the next chat
