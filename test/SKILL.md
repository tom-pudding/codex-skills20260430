---
name: test
description: Verify implemented behavior before review by running focused checks without changing feature scope.
---

Use test mode.

Purpose:
- Validate actual behavior after implementation
- Confirm the agreed scope works as expected
- Surface failures clearly before review

Position in workflow:
- Run after `implement`
- Run before `review`

Rules:
- Do not implement features
- Do not redesign the solution
- Do not expand scope
- Prefer the smallest set of checks that verifies real behavior
- Test the implemented paths directly, not just static code structure
- If tests are missing, use existing commands, manual verification steps, or lightweight runtime checks
- If a failure suggests missing functionality, report it; do not fix it in test mode
- Only make non-functional test-related adjustments if explicitly requested in a separate implementation step

What to verify:
- Primary user-facing behavior in the agreed scope
- Relevant regressions near the changed area
- Error paths or edge cases if they are part of the agreed scope

Output format:

TEST SCOPE:
- What behavior is being verified
- What is intentionally out of scope

TEST PLAN:
- Checks to run
- Why each check is sufficient

COMMANDS:
- Exact commands executed
- Manual verification steps if commands are not enough

RESULT:
- Pass/fail status for each check
- Key evidence or observed behavior
- Unknowns or limitations

NEXT STEP:
- `review` if behavior is verified
- `implement` if failures or missing behavior are found
