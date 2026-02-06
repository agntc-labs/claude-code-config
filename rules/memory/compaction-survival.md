# Compaction Survival Protocol

## When Context Feels Fuzzy (After Compaction)
Immediately run:
```bash
# 1. Check recent work
git status && git log --oneline -5 && git diff HEAD~1 --stat

# 2. Check plan files
ls ~/.claude/plans/*.md 2>/dev/null

# 3. Recover from memory
~/.claude/universal/realtime-memory.py recover

# 4. Query MCP memory for context
# Use mcp__memory__read_graph
```

## Before Compaction (Proactive)
When conversation is getting long:
```bash
~/.claude/universal/realtime-memory.py snapshot "Working on X, completed Y, next is Z"
```

## What Gets Lost
- Exact code you wrote (git has it)
- Specific error messages
- Intermediate reasoning
- File contents read (read again)

## What Survives
- Conversation summary
- Major decisions
- Files modified (git)
- MCP memory saves

## Post-Compaction Checklist
□ Read git status + recent commits
□ Check for .bak files
□ Re-read files you were editing
□ Check ~/.claude/plans/
□ Query MCP memory
□ Ask user if truly lost
