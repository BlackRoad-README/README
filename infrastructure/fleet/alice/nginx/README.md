# Alice — nginx

Reverse proxy for 37+ sites. Cloudflare tunnel ingress on :8080.

| Port | Service | Description |
|------|---------|-------------|
| :8080 | nginx (4 workers) | Main proxy / CF tunnel ingress |
| :9000 | nginx | Secondary (metrics proxy) |

→ [Alice overview](../)
→ [All nginx configs](../../)
