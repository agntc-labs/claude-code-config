---
paths:
  - "**/digital-justin/**"
  - "**/ava/**"
  - "**/*ava*.py"
---

# Ava Code Rules (Only loads when working on Ava files)

## DO NOT CHANGE Without Explicit Permission
- Strategic Engine architecture
- OpenRouterBrain multi-model logic
- ClaudeCodeAgent integration
- Task queue system

## Locations
- Mac Studio: `/opt/digital-justin/`
- Python: `/usr/bin/python3`
- Logs: `runtime/logs/ava.log`
- State: `runtime/state/`

## Before Editing Ava
1. Check she's not running: `ps aux | grep ava`
2. Check her current task: `curl http://100.124.119.18:5050/coord/tasks`
3. Create backup: `cp file.py file.py.bak`
4. After edit: restart if needed

## Testing Changes
```bash
ssh admin@100.124.119.18
cd /opt/digital-justin
/usr/bin/python3 -c "from ava.module import X; print(X)"
```
