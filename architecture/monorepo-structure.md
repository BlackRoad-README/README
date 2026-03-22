# RoadCode Monorepo Structure

```
BlackRoad-OS-Inc/RoadCode/
  Agents/          # Agent identities, prompts, memory, coordination
  Api/             # API servers, endpoints, middleware
  Archive/         # Backup, DR, historical data
  Cli/             # br command, CLI tools, shell scripts
  Config/          # System config, env templates, secrets management
  Core/            # Kernel, runtime, OS primitives
  Data/            # Databases, migrations, seeds, schemas
  Docs/            # Documentation, guides, papers
  Infrastructure/  # Terraform, Docker, nginx, Caddy, WireGuard
  Models/          # AI models, Modelfiles, training data
  Nodes/           # Per-node configs (Alice, Cecilia, Octavia, Aria, Lucidia, Gematria, Anastasia)
  Runtime/         # Process management, cron, daemons, supervisors
  Scripts/         # Memory system, collectors, deployers, fleet tools
  Services/        # Workers, microservices, background jobs
  System/          # Boot, init, health checks, watchdogs
  Tests/           # Integration, unit, e2e, load testing
  Web/             # Frontend templates, static sites, design system
```

→ [Agents folder details](../agents/)
→ [Infrastructure details](../infrastructure/)
→ [Memory scripts](../memory/)
