# Network Planes

| Plane | Range | Purpose |
|-------|-------|---------|
| LAN | 192.168.4.x | Local network (Pi fleet + Mac) |
| Mesh/Tailscale | 100.x.x.x | WireGuard/Headscale overlay |
| Docker | 172.17.x.x | Container networking |
| K3s | 10.42.x.x | Kubernetes pod networking |
| Public | 159.x.x.x | DigitalOcean droplets |
| IPv6 Global | 2001: | Public IPv6 |
| IPv6 Private | fdxx: | Private IPv6 |
| Loopback | 127.0.0.1 | Local services |

**Rule:** IPs change. PLANES do not.

→ [Fleet nodes](../infrastructure/fleet/)
→ [WireGuard mesh](../infrastructure/network/)
