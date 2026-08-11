# Repo Agent Instructions

<!-- CODEX-AGENTS-WRAPPER v1 -->

Startup order: first read and follow
`/Volumes/ThunderBolt/Development/AGENTS.md`, then read the required SOPs for
the task, then read this repo's `_AGENTS.md` when present.

You MUST follow the relevant SOPs in `/Volumes/ThunderBolt/Development/_DOCS/`
based on the task:

- coding: `CODING_STANDARDS.md`
- git, issues, PRs, or boards: `GIT_STANDARDS.md`
- goal runs, workers, swarms, or long-running work: `AGENT_WORKFLOW.md`
- infra, hosts, runners, LXC, SSH, DNS, or deploy work: `INFRASTRUCTURE_SOP.md`
- terminology or repo shorthand: `GLOSSARY.md`

If this repo contains `_AGENTS.md`, you MUST read it before making changes.
`_AGENTS.md` contains repo-local facts and stricter local overrides.

Do not proceed with code, git, PR, board, infra, deploy, or destructive work
until the required global and local instructions are read.

## Specialized Agents (Graph Mode)

This repo is converted to **Graph Mode** (PRE-CANON:
`/Volumes/ThunderBolt/Development/_DOCS/RLVR_LANES_SEED_v2-draft.md`, graduating as
`_DOCS/GRAPH_MODE_SOP.md`; operated by `_ob/skills/graph-mode/`).

**Agents in `.claude/agents/`** (derived copies, process shape only, zero repo
facts — conventions discovered fresh, absent ones ANNOUNCED not skipped):

- `verifier` — classify a change against known classes, run their done-means, report exit codes.
- `pr-scribe` — compose a PR body and prove it passes the repo's validator (falls back to `_DOCS/GIT_STANDARDS.md` shape).
- `harvest-scribe` — turn an accepted lane report into drafted Tightenings.
- `done-means-author` — turn a claim class into an executable check with its RED transcript.

None gates — agent produces, script judges, hook enforces. Derived from
`/Volumes/ThunderBolt/Development/_DOCS/agents/`; improvements flow project → Development canon → sync out.

**Conventions:** lane contract + Tightenings → `docs/lane-contract.md`; done-means + exit grammar
(`0`/`1`/`3`) → `scripts/done-means/`; class vocabulary → the Tightenings
(unclassified work → `verifier` tier 3).
