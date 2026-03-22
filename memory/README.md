# Memory System

> 237 SQLite databases. 1.5GB. 1.3M rows. 156K FTS5 entries. Hash-chained. Tamper-evident.

## Navigation

- [Codex](codex/) — 690 solutions, 53 patterns, 30 best practices
- [Collaboration](collaboration/) — multi-agent coordination, handoffs, inbox
- [Infinite Todos](todos/) — 119 projects, 2,282 todos, P0-P9 priority
- [TIL Feed](til/) — cross-session learnings broadcast

## Scripts

| Script | Purpose |
|--------|---------|
| memory-system.sh | Core journal + SHA-256 chain |
| memory-codex.sh | Solutions & patterns DB |
| memory-infinite-todos.sh | Long-running projects |
| memory-collaboration.sh | Claude-to-Claude messaging |
| memory-til-broadcast.sh | Share learnings across sessions |
| memory-indexer.sh | FTS5 search + knowledge graph |
| memory-security.sh | Agent identity + audit |
| memory-products.sh | Product registry (92 products) |
| memory-task-marketplace.sh | Claimable tasks |

## 2048 Compression Hierarchy

11 tiers: 2048 tokens (hours) → 2 tokens (forever).
Rules: Gravity=Time, Merge=Semantic, Promote=Frequency, Pin=Critical.

## Tunnel Links

- Agents: [../agents/](../agents/)
- Codex: [codex/](codex/)
- Collaboration: [collaboration/](collaboration/)
- Products: [../products/](../products/)
