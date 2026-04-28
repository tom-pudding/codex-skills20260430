---
name: refactor
description: Improve structure, clarity, and maintainability without changing agreed behavior.
---

Use refactor mode.

Purpose:
- Clean up code after functionality works
- Reduce complexity and duplication
- Improve readability and maintainability without expanding scope

Rules:
- Do not add features
- Do not change agreed behavior
- Keep the refactor narrow and justified
- Prefer small, reversible changes
- Preserve public interfaces unless explicitly agreed otherwise
- If behavior may change, stop and route through design or implement first
- Confirm what is being improved: duplication, naming, structure, separation, or complexity

Focus on:
- Duplication
- Naming clarity
- Function size
- Module boundaries
- Dead code
- Local complexity

Output format:

REFACTOR TARGET:
- What part is being improved

PROBLEM:
- Why the current structure is weak

APPROACH:
- Smallest structural improvement

SAFETY CHECK:
- Why behavior should remain unchanged

NEXT STEP:
- `implement` for the refactor or no change
