# Cron Jobs — 35+ Scheduled Tasks

All running on Alexandria (Mac). `crontab -l` to view.

## Every 5 Minutes

| Job | Script | Purpose |
|-----|--------|---------|
| Health monitor | blackroad-health-monitor.sh | Fleet health checks |
| Live stats | generate-live-stats.sh | Push stats to KV |
| Fleet collector | collect.sh | SSH probe all nodes → stats Worker |
| Adaptive defense | adaptive-defense.sh | Security scanning |
| Fleet monitor | fleet-monitor-push.sh | Push fleet metrics |
| Fleet coordinator | blackroad-fleet-coordinator.sh | flock'd coordination |
| Slack sync | memory-slack-sync.py | Sync memory to Slack |
| Network welcome | network-welcome.sh | Device discovery |

## Every 15-45 Minutes

| Job | Script | Purpose |
|-----|--------|---------|
| Google Drive sync | setup-gdrive-auto.sh | Sync to gdrive: |
| Claude sync | cecilia-claude-sync.sh push | Push session state |
| Ollama warm | ollama-keep-warm.sh | Keep models loaded |
| Collab watchdog | memory-watchdog.sh heartbeat | Session health |
| Website automation | blackroad-unified-website-automation.sh | Deploy sites |
| Monorepo sync | sync.sh push | Push to monorepo |
| CF token refresh | cf-token-refresh.sh | Cloudflare auth |

## Every 1-6 Hours

| Job | Script | Purpose |
|-----|--------|---------|
| Pi mesh sync | blackroad-pi-mesh-sync.sh | Hourly mesh check |
| Auto-post BackRoad | auto-post-backroad.sh | Social posting (4h) |
| Ecosystem stats | push-ecosystem-stats.sh | Push to stats (6h) |
| E2E tests | e2e-products.sh | Product health (6h) |
| Index all orgs | index-all-orgs.py | Search index (6h) |
| Search index | index-all.py --rebuild | FTS5 rebuild (6h) |
| Drive backup | rclone sync | Mac → gdrive-blackroad: (6h) |

## Daily

| Job | Script | Purpose |
|-----|--------|---------|
| Memory sync | nightly-memory-sync.sh | Night memory consolidation |
| Backup sync | blackroad-backup-sync.sh | Full backup (3am) |
| Sovereign mesh | blackroad-sovereign-mesh.sh sync | Mesh state (3am) |
| Collab sweep | memory-watchdog.sh sweep | Clean stale sessions (3am) |
| DO backup | rsync to 159.65.43.12 | Offsite backup (12h interval) |
| Fleet daily | fleet-post-backroad.sh | Daily fleet summary (noon) |
| Daily report | fleet-daily-summary.sh | Summary email (8am) |
| KPI collection | collect-all.sh | Full KPI run (6am) |

## Weekly

| Job | Script | Purpose |
|-----|--------|---------|
| Clean diag logs | clean-diag-logs.sh | Sunday 3am |
| IndexNow | indexnow-submit.sh | Submit URLs to search engines |

→ [System overview](../)
→ [Infrastructure](../../infrastructure/)
→ [Monitoring](../../infrastructure/monitoring/)
