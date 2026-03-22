# Sovereignty Stack

| Service | Cloud Version | BlackRoad Version | Runs On |
|---------|--------------|-------------------|---------|
| Git | GitHub | Gitea (273 repos) | Octavia |
| AI | OpenAI | Ollama (44 models, 52 TOPS) | 4 nodes |
| Storage | AWS S3 | MinIO | Cecilia |
| DNS | Cloudflare | PowerDNS | Lucidia + Gematria |
| Chat | Slack | RoundTrip (200 agents) | D1 + Workers AI |
| VPN | Tailscale | WireGuard (12 tunnels) | All nodes |
| TLS | Cloudflare | Caddy + Let's Encrypt | Gematria |
| Database | AWS RDS | PostgreSQL | 3 nodes |
| Cache | ElastiCache | Redis | Alice |
| CI/CD | GitHub Actions | Gitea Actions | Octavia |
| Search | Algolia | FTS5 + Workers AI | D1 |
| PaaS | Heroku | Deploy API | Octavia |

Only external deps: Stripe (cards), GoDaddy (registrar).

→ [Road Fleet forks](../infrastructure/sovereignty/)
→ [BlackBox Protocol](../infrastructure/sovereignty/)
