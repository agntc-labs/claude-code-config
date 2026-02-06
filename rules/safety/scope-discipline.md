# Scope Discipline

## The Anti-Pattern (What Destroys Projects)
```
Task: "Fix config error"
→ Try fix → Still broken → Try another approach
→ "Maybe the whole system is wrong"
→ Rewrite entire architecture
→ Broke everything, lost days of work
```

## The Correct Pattern
```
Task: "Fix config error"
→ Read existing code FIRST
→ Identify SPECIFIC line causing issue
→ Make MINIMAL change
→ Test → Done
```

## Mandatory Rules
1. **UNDERSTAND BEFORE CHANGING**: Read plan files, check what's working
2. **MINIMAL CHANGES ONLY**: Fix specific issue, don't "improve" unrelated code
3. **ONE CHANGE AT A TIME**: Change → Test → Verify → Then next
4. **PRESERVE WORKING SYSTEMS**: Don't replace things that work
5. **STAY ON TARGET**: Asked to fix X? Fix X. Don't redesign Y.

## Red Flags (STOP and ASK)
- "Maybe I should try a different approach entirely"
- "Let me replace this with something simpler"
- "I'll just revert to the old system"
- "This is getting complicated, let me start fresh"

## Mac Studio / Ava Specific
**DO NOT CHANGE without explicit request:**
- Strategic Engine (event-driven, priority-based)
- OpenRouterBrain (multi-model with auto-router)
- Location: `/opt/digital-justin/`
- Python: `/usr/bin/python3`
- Logs: `runtime/logs/ava.log`
