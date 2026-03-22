# Lucidia — Apps Node

**The Dreamer — Reasoning, Vision (kahuna model)**

| Spec | Value |
|------|-------|
| Device | Raspberry Pi 5 |
| IP | 192.168.4.38 |
| SSH | octavia@192.168.4.38 |
| Kernel | 6.12.62+rpt-rpi-2712 |
| Memory | 7.9 GB (5.5 GB used) |
| Disk | 235 GB (69 GB used, 31%) |
| CPU Temp | 61C (HIGH) |
| Listening Ports | 63 |
| Running Services | 49 |
| Load Average | 3.76+ |

## Docker Containers (16)

| Container | Image | Ports |
|-----------|-------|-------|
| eps | pi-eps | :50001 |
| bitcoind | ruimarinho/bitcoin-core | 8332-8333 (internal) |
| road-pdns | powerdns/pdns-auth-48 | .38:53 (DNS), :9053 (admin) |
| road-pdns-admin | powerdnsadmin/pda-legacy | :9192 |
| road-dns-db | postgres:15-alpine | 5432 (internal) |
| blackroad-gitea | gitea/gitea | :3100, :2222 (SSH) |
| roadauth | node:18-alpine | :4002→3002 |
| roadapi | node:18-alpine | :4001→3001 |
| blackroad-edge-agent | blackroad/edge-agent:v2 | :9090, :8082 |
| blackroad.systems | blackroad.systems | :3005→3000 |
| blackroadai.com | blackroadai.com | :3006→3000 |
| blackroad-auth-gateway | blackroad-auth-gateway | — |
| blackroad-metaverse | blackroad-metaverse | :3109→3000 |
| blackroad-os | blackroad-os-ultimate | — |
| blackroad-os-carpool | blackroad-os-carpool | :3002→3000 |
| pi-my-agent-1 | pi-my-agent | :8080 |

## Ollama Models (6)

blackroad-road, blackroad-lite, blackroad-master, tinyllama, qwen2.5:3b, nomic-embed-text

## Key Services

- [nginx](nginx/) — reverse proxy for apps
- [PowerDNS](powerdns/) — authoritative DNS (ns2)
- [Ollama](ollama/) — AI inference (6 models)
- [Runners](runners/) — GitHub/Gitea Actions runners

## Notes

- HOTTEST NODE (61C) — high load, needs attention
- Most Docker containers (16) — most apps hosted here
- Most listening ports (63) — highest service density
- Bitcoin node running (bitcoind)
- Runs self-hosted versions of blackroad.systems and blackroadai.com

→ [Agent](../../../agents/fleet/lucidia/)
→ [Network](../../network/)
→ [Fleet](../)
