# Memory & Context Index (Level 2)

## When Context Feels Fuzzy
- **Overview**: @~/.claude/rules/memory/overview.md
  - Quick recovery commands
  - What survives compaction
  - Post-compaction checklist

- **Compaction Survival**: @~/.claude/rules/memory/compaction-survival.md
  - Detailed recovery protocol
  - Proactive save commands

## Ava Memory Bridge (Coming Soon)
- **Ava Bridge**: @~/.claude/rules/memory/ava-bridge.md
  - Ava as persistent memory layer
  - API endpoints for save/recall
  - Auto-save before compaction

## Quick Commands
```bash
# Recovery
~/.claude/universal/realtime-memory.py recover

# Save decision
~/.claude/universal/realtime-memory.py decision "desc" "reason"

# Snapshot
~/.claude/universal/realtime-memory.py snapshot "state"

# Ask Ava
curl http://100.124.119.18:5050/memory/recall
```
