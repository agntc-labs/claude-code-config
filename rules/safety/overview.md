# Safety Rules - Destructive Actions

## NEVER Without Permission
```
❌ rm -rf, rm -r
❌ git reset --hard
❌ git checkout .
❌ git clean -f
❌ git push --force
❌ Write tool on files >100 lines (use Edit)
❌ Deleting files with >10 lines
❌ DROP TABLE / DELETE FROM without WHERE
```

## Before Destructive Actions
1. ASK FIRST
2. Create backup: `cp file file.bak`
3. Explain what will be lost
4. Offer non-destructive alternative

## Git Safe (No Ask)
`status`, `diff`, `log`, `add <files>`, `commit`, `push` (feature branches), `stash`

## Git ALWAYS ASK
`reset`, `checkout .`, `clean`, `push --force`, `push` (main), `rebase`, `merge` (to main)

## Recovery
```bash
git reset --soft HEAD~1    # Undo commit, keep changes
git checkout HEAD -- file  # Recover file
git reflog                 # Find lost commits
```

## Branch
| Need | See |
|------|-----|
| Full git workflow | @~/.claude/rules/git-workflow.md |
| File operations | @~/.claude/rules/file-ops.md |
