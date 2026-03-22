# Network

## Physical Topology

```
              INTERNET (Comcast)
                    |
              ROUTER 192.168.4.1
              SSID: asdfghjkl
              5GHz Channel: 100
              Subnet: 192.168.4.0/22
              |    |    |    |    |
          ~~~~WiFi (all nodes on 5GHz)~~~~
              |    |    |    |    |
           ALICE CECILIA OCTAVIA ARIA LUCIDIA
           .49   .96    .101   .98   .38
```

## Network Planes

| Plane | Range | Purpose |
|-------|-------|---------|
| LAN | 192.168.4.x | Local WiFi network |
| WireGuard | 10.8.0.x | Encrypted mesh |
| Tailscale | 100.x.x.x | Headscale overlay |
| Docker | 172.17.x.x | Container networks |
| RoadNet AP | 10.10.x.0/24 | Per-node access points |

## WireGuard Addresses

| Node | WG Address |
|------|-----------|
| Alice | 10.8.0.6 |
| Cecilia | 10.8.0.3 |
| Octavia | 10.8.0.4 |
| Aria | 10.8.0.7 |
| Lucidia | Tailscale 100.66.235.47 |

## WiFi Signal Strength

| Node | dBm | Quality |
|------|-----|---------|
| Alice | -58 | 52 |
| Cecilia | -64 | 46 |
| Octavia | -63 | 47 |
| Aria | -61 | 49 |
| Lucidia | -62 | 48 |

## Subnetworks

- [WireGuard](wireguard/) — 12 peer connections
- [DNS](dns/) — PowerDNS on Lucidia + Gematria
- [Tunnels](tunnels/) — 18 Cloudflare tunnels via Aria
- [Tor](tor/) — hidden services on Alice, Octavia, Lucidia
- [Headscale](headscale/) — mesh coordinator on Aria
- [NATS](nats/) — pub/sub on Octavia
- [IPFS](ipfs/) — planned

→ [Fleet](../fleet/)
→ [Wire Map source](~/roadnet/WIRE-MAP.md)
→ [Port Map source](~/roadnet/PORT-MAP.md)
