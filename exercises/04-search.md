# Exercise 04: Search & Find

## Goal
Use Git to search files and commit history.

These commands help you understand when and why changes happened.

---

## Start here
```bash
git switch main
git switch -c student/<yourname>-search
```

## Tasks
1. Search for text in the repository:
```
git grep "beta"
```
2. Find commits where the number of occurrences of a string changed:
```
git log -S "beta feature" --oneline
```
3. View line-by-line history for a file:
```
git blame src/search.txt
```

## Expected result
You can identify:
- At least one file match using ```grep```
- A commit hash using ```-S```
- A commit/author per line using ```blame```
