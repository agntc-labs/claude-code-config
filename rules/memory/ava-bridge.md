# Ava Memory Bridge (In Development)

## Concept
Ava becomes the persistent memory layer for Claude Code.
She manages our memory, not the other way around.

## Architecture (When Implemented)
```
Claude Code → Ava's /memory/save → Markdown + Firestore
Claude Code ← Ava's /memory/recall ← Semantic search
```

## Planned Endpoints
| Endpoint | Purpose |
|----------|---------|
| `/memory/save` | Save context before compaction |
| `/memory/recall` | Get context for current project |
| `/memory/decision` | Log important decisions |
| `/memory/rules` | Get Ava-generated rules |

## Current Status
- [ ] Memory directory created: /opt/digital-justin/claude-memory/
- [ ] API endpoints added to Ava
- [ ] Session monitoring active
- [ ] Auto-save before compaction
- [ ] Rule generation from pain points

## Manual Save (Until Automated)
```bash
curl -X POST http://100.124.119.18:5050/coord/messages \
  -H "Content-Type: application/json" \
  -d '{"from": "claude-code", "to": "ava", "type": "context_save", "message": "SAVE THIS CONTEXT"}'
```

## See Also
- Full architecture: @~/projects/experiments/Agent Playground/AVA_CLAUDE_BRIDGE_ARCHITECTURE.md
