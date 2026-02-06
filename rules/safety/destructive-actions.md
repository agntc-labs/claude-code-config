# Destructive Action Protection

## NEVER Do Without Permission
- `rm -rf` anything
- `git reset --hard`, `git checkout .`, `git clean -f`
- `git push --force`
- Overwriting entire files with Write (use Edit instead)
- Deleting files with >10 lines
- `DROP TABLE` / `DELETE FROM` without WHERE
- Firebase/gcloud delete commands

## Before Destructive Actions
1. ASK FIRST - even with autonomy
2. Create backup: `cp file file.bak` or `git stash`
3. Explain what will be lost
4. Offer non-destructive alternatives

## File Edit Rules
- **Small edits (<20 lines)**: Use Edit tool - safe and reversible
- **Large edits (>20 lines)**: STOP. Do you really need this much change?
  - Read ENTIRE file first
  - Multiple small Edits, not one Write
  - Create .bak backup first
- **NEVER Write** to overwrite files you haven't read THIS session

## Git Safe Commands (no asking)
`git status`, `git diff`, `git log`, `git add <files>`, `git commit`, `git push` (feature branches), `git stash`

## Git ALWAYS ASK
`git reset`, `git checkout .`, `git clean`, `git push --force`, `git push` (main/master), `git rebase`, `git merge` (to main)

## Recovery Commands
```bash
git reset --soft HEAD~1  # Undo commit, keep changes
git checkout HEAD -- file  # Recover deleted file
git reflog  # Find lost commits
git stash list && git stash pop  # Recover stash
```
