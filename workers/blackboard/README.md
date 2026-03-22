# Worker: blackboard

**BlackRoad Analytics Engine**

Tracks pageviews, visitors, sessions, errors, conversions across all BlackRoad sites. The bb.js script is loaded on 32+ HTML templates.

| Detail | Value |
|--------|-------|
| URL | blackboard.amundsonalexa.workers.dev |
| Alias | bb.blackroad.io |
| Storage | D1 (bcc78f33-b052-4cb2-bcfb-db5cd3c08472) |
| Tables | events, errors, conversions |
| 30-day stats | 1,220 pageviews, 764 visitors, 906 sessions |

## Endpoints

- `/bb.js` — analytics tracking script
- `/api/stats` — aggregate stats
- `/api/pages` — per-page breakdown
- `/api/errors` — error log (grouped)
- `/api/referrers` — traffic sources

## Known Issues

- 756 errors in 30 days (98.7% are CORS — fixed with crossorigin="anonymous")
- 84% bounce rate

→ [Analytics](../../web/analytics/)
→ [Status](../../status/)
