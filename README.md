# King Factory Pipeline — Kanban Orchestration

Visual explainer for how AI agents run King Capital's nightly trading pipeline using Hermes Agent's Kanban system.

## Quick Start

Open `index.html` in a browser. No dependencies, no build step -- it's a single self-contained HTML file.

## What's In Here

- **Pipeline visualization** -- 6-stage dependency chain from FRD ingest to reconciliation
- **Kanban board mockup** -- how tasks flow through triage → ready → running → done
- **Key concepts** -- dependencies, agent profiles, heartbeats, structured handoffs, self-healing
- **Before/After comparison** -- cron+bash vs. Kanban agents
- **Data flow diagram** -- FRD API → PostgreSQL → Signals → QRT → CSV → SFTP → Reconciliation
- **Tech stack** -- Hermes Agent, OpenClaw, Open Brain

## Live Board

The actual Kanban board runs on Bilby (CT 271, 10.71.20.71):

```bash
ssh root@10.71.20.71 "hermes kanban list --board king-factory"
```

## Related

- [king-ops](https://github.com/King-Capital/king-ops) -- factory module backend
- [king-ingest](https://github.com/King-Capital/king-ingest) -- FRD data pipeline
- [king-signals](https://github.com/King-Capital/king-signals) -- signal generation
- [king-reconciliation](https://github.com/King-Capital/king-reconciliation) -- fill matching
