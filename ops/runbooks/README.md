# Operational Runbooks

## Node Down

1. Check: `ssh user@ip "true"` — timeout = node unreachable
2. Check power: `ssh user@ip "vcgencmd get_throttled"` — 0x50005 = undervoltage
3. Check temp: reading > 80C = thermal throttling
4. Recovery: power cycle, check SD card, verify WiFi

## Service Down

1. Check: `systemctl status <service>`
2. Restart: `systemctl restart <service>`
3. If container: `docker restart <name>`
4. If persistent: check logs `journalctl -u <service> -n 50`

## Fleet Stats Stale

1. Check: `curl stats-blackroad.amundsonalexa.workers.dev/health`
2. If old timestamp: run `bash ~/stats-blackroad/collect.sh` manually
3. If 401: check auth header in collect.sh (Bearer not query param)
4. Verify: `curl stats-blackroad.amundsonalexa.workers.dev/fleet`

## Disk Full (Alice — 68% and climbing)

1. Clear logs: `sudo journalctl --vacuum-time=3d`
2. Clear apt: `sudo apt clean`
3. Check: `du -sh /var/log/* | sort -rh | head`
4. Logrotate: verify `/etc/logrotate.d/` configs

## DNS Not Resolving

1. Check Pi-hole: `dig @192.168.4.49 blackroad.io`
2. Check PowerDNS: `dig @192.168.4.38 blackroad.io`
3. Check Cloudflare: `dig @1.1.1.1 blackroad.io`
4. If local only: Headscale DNS (100.100.100.100) may not resolve all subdomains — use `--resolve` to test

→ [Incident response](../incident-response/)
→ [Fleet](../../infrastructure/fleet/)
→ [Monitoring](../../infrastructure/monitoring/)
