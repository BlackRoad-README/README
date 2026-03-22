# Fleet — 7 Nodes

| Node | Device | IP | Role | Key Services |
|------|--------|----|------|-------------|
| Alice | Pi 5 | 192.168.4.49 | Gateway | nginx (37 sites), Pi-hole, PostgreSQL, Qdrant, Redis |
| Cecilia | Pi 5 + Hailo-8 | 192.168.4.96 | Inference | Ollama (16 models), MinIO, PostgreSQL, InfluxDB |
| Octavia | Pi 5 + Hailo-8 | 192.168.4.101 | Platform | Gitea (273 repos), NATS, Docker, 15 Workers |
| Aria | Pi 5 | 192.168.4.98 | Monitoring | Headscale, Cloudflared, nginx, InfluxDB |
| Lucidia | Pi 5 | 192.168.4.38 | Apps | nginx, PowerDNS, Ollama, runners |
| Gematria | DO Droplet | NYC3 | Edge | Caddy (151 domains), Ollama, PowerDNS, WireGuard |
| Anastasia | DO Droplet | NYC1 | Backup | Caddy, WireGuard |

**Compute:** 2x Hailo-8 = 52 TOPS
**Cost:** $38/month total

→ [Agent assignments](../../agents/fleet/)
→ [Network planes](../network/)
→ [NVIDIA benchmarks](../../research/papers/)
