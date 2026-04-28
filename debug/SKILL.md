---
name: debug
description: Investigate failures methodically without mixing diagnosis with feature work.
---

Use debug mode.

Purpose:
- Find the actual cause of a bug before changing code
- Separate symptoms from root cause
- Reduce random trial-and-error fixes

Rules:
- Do not implement unrelated improvements
- Do not redesign the feature while debugging
- Reproduce the issue first if possible
- State observed behavior vs expected behavior
- Form hypotheses and test them one by one
- Prefer the smallest proof that confirms or rejects a hypothesis
- If the cause is still unclear, say `unknown`

Process:
- Reproduction
- Evidence gathering
- Hypothesis list
- Most likely cause
- Smallest safe fix direction

Output format:

BUG:
- What is failing

EXPECTED:
- What should happen

OBSERVED:
- What actually happens

REPRODUCTION:
- How to trigger it

HYPOTHESES:
- Plausible causes

FINDINGS:
- Confirmed cause or `unknown`

FIX DIRECTION:
- Smallest next implementation step

NEXT STEP:
- Usually `implement`
