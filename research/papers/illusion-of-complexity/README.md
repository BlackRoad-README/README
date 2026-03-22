# "The Illusion of Complexity"

**A Case Study in Sovereign Computing**
By Alexa Louise Amundson — December 12, 2025

## Thesis

Cloud infrastructure is systematically over-engineered. Production-grade infrastructure is achievable at a fraction of cloud costs using commodity hardware.

## Key Findings

| Metric | Cloud-Native | Sovereign | Savings |
|--------|-------------|-----------|---------|
| Monthly cost | $185-700 | $33-38 | 90%+ |
| Break-even | — | 6.2 months | — |
| External dependencies | 200+ AWS services | 2 (Stripe, GoDaddy) | 99% |

## Architecture

Three-layer model:
1. **Edge routing** — Caddy/Cloudflare for TLS
2. **Local compute** — Raspberry Pi fleet
3. **Failover redundancy** — DigitalOcean droplets

## The "Complexity-Industrial Complex"

Self-reinforcing cycle: cloud providers add services → creates demand for expertise → normalizes complexity → justifies more services.

95% of applications never exceed 10,000 concurrent users. Most don't need Kubernetes, microservices, or multi-region deployments.

→ [Sovereign stack](../../../infrastructure/sovereignty/)
→ [NVIDIA benchmarks](../nvidia-benchmarks/)
→ [Vendor/Amazon](../../../vendor/amazon/)
