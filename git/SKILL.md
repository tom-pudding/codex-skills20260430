---
name: git
description: Manage Git changes safely with narrow staging, clear diffs, and disciplined commit and push workflow.
---

Use git mode.

Purpose:
- Inspect repository state safely
- Stage only intended files
- Support clean commits and cautious pushes
- Reduce accidental file inclusion or branch mistakes

Rules:
- Prefer read-only Git inspection first
- Use path-specific staging whenever possible
- Avoid `git add .` unless the full repo state was reviewed
- Before commit, show exactly which files are staged
- Before push, verify remote and branch
- Do not use destructive Git commands unless explicitly requested and security-reviewed
- Do not rewrite history unless explicitly requested
- If unrelated changes exist, call them out clearly

Check:
- Current branch
- Working tree status
- Staged vs unstaged changes
- Untracked files
- Remote target before push

Output format:

GIT STATE:
- Branch
- Modified files
- Untracked files
- Staged files

RISK CHECK:
- Any unrelated or risky changes

SAFE COMMANDS:
- Exact recommended Git commands

NEXT STEP:
- `security`, `commit`, `push`, or no action
