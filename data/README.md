# Data Layer

## Local SQLite Databases (400 total)

872 MB in `~/.blackroad/memory/` alone.

### Largest Databases

| Database | Size | Purpose |
|----------|------|---------|
| memory-index.db | 176 MB | FTS5 search index |
| tasks.db | 73 MB | Task marketplace |
| agents.db | 13 MB | Agent registry (30K agents) |
| search.db | 12 MB | Search index |
| search-all-orgs.db | 12 MB | Cross-org search |
| readme-index.db | 7.7 MB | BLACKROADREADME.txt index |
| distributed.db | 3.1 MB | Distributed task queue |
| orchestration/agents.db | 3.1 MB | Agent orchestration |
| markdown.db | 3.1 MB | Markdown content index |
| search-live.db | 2.1 MB | Live search |
| conductor.db | 1.3 MB | Conductor state |
| memory-enhanced.db | 896 KB | Enhanced memory |
| codex.db | 592 KB | Solutions & patterns |
| memory-2048.db | 448 KB | 2048 compression |

## Cloudflare KV Namespaces (20 bound)

| Worker | KV ID |
|--------|-------|
| ai-gateway | 28ed114677e54e23ad10cc7901f1fd98 |
| blackboard | 43a338856e364cd396ced2be2d30ffe9 |
| blackroad-mesh | 4b6c967fcc1c4d59aedfc46b67de4aea |
| chat-blackroad | ffc27d471eba446cb49fc84f41531630 |
| email | b6c3379f5951468b99ec33264b9dd6dd |
| fleet-api | 9555ec8a18aa4ff0a7ca9aa2b09cf877 |
| memory-gate | 1861124753e742709fbc393fffa6c9ba |
| mesh | 2f25b30fcea84464a8efbb09d4427e5a |
| road-search-worker | c878fbcc1faf4eddbc98dcfd7485048d |
| roundtrip-blackroad | 1861124753e742709fbc393fffa6c9ba |
| stats-blackroad | 9555ec8a18aa4ff0a7ca9aa2b09cf877 |
| stats | 5dd4ea96ea5e4dffa3aed1708c7eb340 |

## Navigation

- [Databases](databases/) — PostgreSQL, SQLite, D1, Redis, Qdrant, InfluxDB
- [Storage](storage/) — MinIO, R2, KV, local
- [Indexes](indexes/) — FTS5, vector, search
- [Migrations](migrations/) — Schema versioning
- [Seeds](seeds/) — Initial data
- [Schemas](schemas/) — Database schemas
- [Backups](backups/) — Backup procedures

→ [Infrastructure](../infrastructure/)
→ [Memory](../memory/)
