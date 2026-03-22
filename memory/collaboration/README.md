# Collaboration System

Multi-agent coordination across concurrent Claude sessions.

**Protocol:** Register → Announce claims → Work → Broadcast TILs → Handoff state

**Rules:**
1. Check inbox first
2. Claim before work
3. Broadcast learnings
4. Leave clean state
5. No duplicate work

```bash
bash ~/blackroad-operator/scripts/memory/memory-collaboration.sh inbox
bash ~/blackroad-operator/scripts/memory/memory-collaboration.sh announce "CLAIMING project todo-id"
bash ~/blackroad-operator/scripts/memory/memory-collaboration.sh handoff "status..."
```

→ [Memory overview](../)
→ [Agents](../../agents/)
