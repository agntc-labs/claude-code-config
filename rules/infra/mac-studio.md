# Infrastructure Reference

## Mac Studio (24/7 Server)
- **Tailscale IP**: 100.124.119.18
- **API**: http://100.124.119.18:5050
- **Location**: `/opt/digital-justin/`
- **Python**: `/usr/bin/python3`

### Key Endpoints
| Endpoint | Purpose |
|----------|---------|
| `/health` | Health check |
| `/think` | Generate response as Justin |
| `/coord/register` | Register this session |
| `/coord/agents` | List active agents |
| `/coord/tasks` | Shared task queue |
| `/coord/messages` | Inter-agent messaging |
| `/coord/onboard` | Full system briefing |

### Register This Session
```bash
curl -X POST http://100.124.119.18:5050/coord/register \
  -H "Content-Type: application/json" \
  -d '{"agent_id": "claude-macbook", "agent_type": "claude-code"}'
```

## Firebase / GCP
- **Org**: agntc.tech (ID: 600894054507)
- **Owner**: justin@agntc.tech

### Projects
| Project | Purpose |
|---------|---------|
| power-to-the-people-vpp | Solar CRM |
| agentic-labs | Digital Justin, AI apps |

### Service Accounts
- MacBook: `~/Projects/power-to-the-people/firebase-service-account.json`
- Mac Studio: `/opt/digital-justin/firebase-service-account.json`

## VaultDev (API Keys)
- Location: `~/Documents/VaultDev/`
- 136+ keys managed
- `vault_list_keys` / `vault_test_key KEY_NAME`
