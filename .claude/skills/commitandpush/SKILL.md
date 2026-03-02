---
name: commitandpush
description: Stage all changed files, create a commit with a descriptive message, then ask whether to push to origin.
disable-model-invocation: true
---

Stage all changed files, create a commit with a descriptive message, then ask whether to push.

1. Run `git status` to see what files have changed.
2. Run `git add -A` to stage all changes.
3. Run `git diff --cached` to understand what changed.
4. Write a concise commit message summarising the changes (imperative mood, e.g. "Add user authentication feature").
5. Run `git commit -m "<message>"`.
6. Ask the user: "Push to origin? (yes/no)"
   - If yes: run `git push`
   - If no: stop here and confirm the commit was created locally.
