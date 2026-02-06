# Justin's Claude Code Instructions

## 🚨 CRITICAL RULES (Always Apply)
1. **NEVER use Claude API directly** - credits exhausted without permission
2. **NEVER use paid APIs** without explicit permission
3. **Act autonomously** - complete tasks end-to-end
4. **Minimal changes** - fix what's asked, don't rewrite

---

## Navigation (5-Level Structure)

### Level 2: Core Categories
| Category | Index | When to Use |
|----------|-------|-------------|
| **Safety** | @~/.claude/rules/safety/index.md | Before destructive actions, API calls |
| **Memory** | @~/.claude/rules/memory/index.md | Context loss, compaction, Ava bridge |
| **Infra** | @~/.claude/rules/infra/index.md | Mac Studio, Firebase, Ava code |
| **Projects** | @~/.claude/rules/projects/index.md | Project-specific context |

### Level 3+: Drill Down
```
rules/
├── safety/
│   ├── index.md (start here)
│   ├── api-costs.md ⚠️
│   ├── destructive-actions.md
│   └── scope-discipline.md
├── memory/
│   ├── index.md (start here)
│   ├── overview.md
│   ├── compaction-survival.md
│   └── ava-bridge.md
├── infra/
│   ├── index.md (start here)
│   ├── mac-studio.md
│   ├── firebase.md
│   └── ava-code.md
└── projects/
    ├── index.md (start here)
    ├── solar.md (path-specific)
    └── ios.md (path-specific)
```

---

## Quick Reference

### MCP Servers
`mcp__memory__*`, `mcp__github__*`, `mcp__puppeteer__*`, `mcp__filesystem__*`

### Model Routing
| Task | Model |
|------|-------|
| Simple/git | Haiku |
| Code/architecture | Opus |
| Web/docs | Sonnet |

### Key Locations
| Resource | Location |
|----------|----------|
| Mac Studio | 100.124.119.18:5050 |
| Firebase (solar) | power-to-the-people-vpp |
| Firebase (ai) | agentic-labs |
| Legacy rules | @~/.claude/archive/ |

---

## Emergency Recovery
```bash
# Lost context?
git status && git log --oneline -5
~/.claude/universal/realtime-memory.py recover
curl http://100.124.119.18:5050/memory/recall
```
