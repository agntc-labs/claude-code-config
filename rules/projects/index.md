# Project-Specific Rules Index (Level 2)

## How Project Rules Work
Project rules use **path-specific loading** - they ONLY load when working on matching files.

```yaml
---
paths:
  - "**/*.swift"
---
# These rules only load for Swift files
```

## Available Project Rules

### Solar / SolarOS
- **File**: @~/.claude/rules/projects/solar.md
- **Paths**: `**/SOLAR*.md`, `**/solar/**`
- **Key context**: 2026 changes, compliance, Ava's research

### iOS Development
- **File**: @~/.claude/rules/projects/ios.md
- **Paths**: `**/*.swift`, `**/ios/**`
- **Key context**: SwiftUI patterns, Firebase iOS SDK

### Web / React
- **File**: @~/.claude/rules/projects/web.md
- **Paths**: `**/*.tsx`, `**/*.jsx`, `**/web/**`
- **Key context**: React patterns, Firebase web SDK

### Python / Backend
- **File**: @~/.claude/rules/projects/python.md
- **Paths**: `**/*.py`
- **Key context**: FastAPI, async patterns

## Adding New Project Rules
1. Create file in `~/.claude/rules/projects/`
2. Add frontmatter with `paths:` field
3. Add project-specific context
