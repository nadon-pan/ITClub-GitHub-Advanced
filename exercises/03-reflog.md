# Exercise 03: Reflog Recovery

## Goal
Recover a commit that appears to be lost after a hard reset.

This exercise demonstrates how Git remembers previous HEAD positions.

---

## Start here
```bash
git switch exercise/reflog-start
git switch -c student/<yourname>-reflog
```

## Tasks
1. Confirm the commit exists:
```
git log --oneline -3
```
2. Reset the branch back one commit:
```
git reset --hard HEAD~1
```
3. Verify the commit is no longer visible:
```
git log --oneline -3
```
4. View the reflog:
```
git reflog -n 10
```
5. Find the commit hash from before the reset and restore it:
```
git reset --hard <commit-hash>
```

## Expected result
- git log should show the recovered commit again.
