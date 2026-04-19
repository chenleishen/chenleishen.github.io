---
name: commit
description: Create clean git commits. Use when the user asks to commit changes, write a commit message, stage changes for a commit, or commit and push work to a remote repository.
---

# Commit

When creating a commit:

1. Check the working tree with `git status --short --branch`.
2. Inspect changes with `git diff` and `git diff --staged` as needed.
3. Stage only the files that belong to the requested change. Do not stage unrelated user work.
4. Prefer this commit subject format:

   `type(scope): imperative summary`

   Use common types like `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, and `ci`.
5. Keep the subject under 72 characters when practical.
6. Add a commit body only when the reason, tradeoffs, or verification need explanation.
7. Run a relevant lightweight verification when appropriate. If none is run, say so.
8. Commit the staged changes, then report the commit hash and the files included.
9. Push only when the user asks to push or asks for the change to be on the remote.
