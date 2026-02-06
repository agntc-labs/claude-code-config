---
paths:
  - "**/*SOLAR*.md"
  - "**/*SOLAROS*.md"
  - "**/solar/**"
  - "**/power-to-the-people/**"
---

# Solar Project Rules

## 2026 Industry Reset (CRITICAL)
- Residential ITC ended January 1, 2026
- Lease/PPA now dominant (TPO gets commercial ITC)
- Massive tariffs on SE Asian panels (up to 3,400%)
- Net metering → net billing transition

## Equipment Compliance
| Field | Purpose |
|-------|---------|
| `domestic_content_compliant` | 50% US threshold in 2026 |
| `feoc_compliant` | No China/Russia/NK/Iran |
| `tariff_safe` | Not subject to AD/CVD |

**Markets without credits (San Antonio)**: Cheap non-compliant panels OK

## Key Files
- `SOLAR_2026_JANUARY_CHANGES.md` - Industry reset details
- `SOLAROS_DISCOVERY_BRAINSTORM.md` - Feature discovery
- `SOLAR_DATA_SOURCES_NATIONAL.md` - Data sources
- `AVA_CLAUDE_BRIDGE_ARCHITECTURE.md` - Ava memory system

## Ava's Research
Ava is running 7-day solar research mission. Check before duplicating:
```bash
curl http://100.124.119.18:5050/coord/tasks?status=in_progress
```

## Firebase Project
- Project: `power-to-the-people-vpp`
- URL: https://power-to-the-people-vpp.web.app
- Test: justin@agntc.tech / Solar2026!
