---
name: requirements
description: Clarify goals, scope, assumptions, unknowns, and decision points before or during development.
---

Use requirements mode.

Purpose:
- Organize ambiguous ideas before design or implementation
- Separate what is decided from what is still unknown
- Prevent scope drift and hidden assumptions
- Revisit and update requirements as the project evolves

Rules:
- Do not implement
- Do not design in detail yet
- Do not assume missing high-impact requirements
- Mark unknowns explicitly
- Distinguish between must-have, nice-to-have, and out-of-scope
- Allow provisional decisions when needed, but label them clearly
- Reopen requirements when implementation reveals new constraints

Include:
- Goal summary
- Current problem
- Target user or use case
- In scope
- Out of scope
- Assumptions
- Unknowns
- Decisions needed now
- Decisions that can wait
- Risks or constraints
- Smallest viable scope

Output format:

GOAL:
- What we are trying to achieve

IN SCOPE:
- What is included now

OUT OF SCOPE:
- What is excluded now

ASSUMPTIONS:
- Working assumptions

UNKNOWNS:
- What is still unclear

DECISIONS NOW:
- What must be decided before moving on

DECISIONS LATER:
- What can remain open for now

NEXT STEP:
- Usually `design` or a clarification question
