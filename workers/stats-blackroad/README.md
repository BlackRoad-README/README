# Worker: stats-blackroad

**Fleet Stats Aggregator**

Receives push data from fleet collector every 5 minutes. Stores in KV. Serves fleet/infra/github/analytics endpoints.

| Detail | Value |
|--------|-------|
| URL | stats-blackroad.amundsonalexa.workers.dev |
| Auth | Authorization: Bearer (STATS_KEY) |
| Collector | ~/stats-blackroad/collect.sh (cron */5) |

## Endpoints

- `/fleet` — live fleet node data
- `/infra` — infrastructure counts
- `/github` — GitHub org stats
- `/ecosystem` — aggregate ecosystem numbers
- `/health` — last update timestamp
- `/push` — POST endpoint for collectors (auth required)

## Recent Fix

Auth mismatch fixed 2026-03-22: script was sending key as query param, worker expected Bearer header. Fleet data was stale since March 16.

→ [Infrastructure](../../infrastructure/fleet/)
→ [Monitoring](../../infrastructure/monitoring/)
