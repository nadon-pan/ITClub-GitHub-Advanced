# Exercise 01: Interactive Rebase

## Goal
Clean up a messy commit history into a small number of clear, meaningful commits.

This exercise simulates a real development workflow where commits were made quickly and now need cleanup before sharing.

---

## Start here
```bash
git switch exercise/rebase-start
git switch -c student/<yourname>-rebase
```

## Tasks

1. View the recent commit history:
```
git log --oneline -5
```
2. Start an interactive rebase on the last 4 commits:
```
git rebase -i HEAD~4
```
3. In the rebase editor:
- pick
- reword
- squash
- drop

## Expected results:
- git log should show a clean history.
- There should be no wip, fix, etc.
