# Memory & Context Preservation

## When Context Feels Fuzzy
```bash
# 1. Check recent work
git status && git log --oneline -5

# 2. Check Ava's memory (when available)
curl http://100.124.119.18:5050/memory/recall

# 3. Use realtime-memory
~/.claude/universal/realtime-memory.py recover
```

## Proactive Saves (Do Often)
```bash
# Save decision
~/.claude/universal/realtime-memory.py decision "description" "reason"

# Save learning
~/.claude/universal/realtime-memory.py learn "topic" "content"

# Snapshot before complex work
~/.claude/universal/realtime-memory.py snapshot "current state"
```

## What Survives Compaction
- Git commits/history ✅
- MCP memory saves ✅
- Ava's memory (when implemented) ✅
- Realtime-memory saves ✅

## What Gets Lost
- Exact code written (but git has it)
- Intermediate reasoning
- File contents read

## Post-Compaction Checklist
□ `git status` + recent commits
□ Check .bak files
□ Re-read active files
□ Query Ava: `curl http://100.124.119.18:5050/memory/recall`

## Branch
| Need | See |
|------|-----|
| MCP memory usage | @~/.claude/rules/mcp-memory.md |
| Ava integration | @~/.claude/rules/ava-bridge.md |
