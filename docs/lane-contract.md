# king-factory-kanban — Lane Contract

Status: **WRITTEN.** Standing rules every Graph Mode lane in this repo is
pointed at. The protocol is **PRE-CANON**
(`/Volumes/ThunderBolt/Development/_DOCS/RLVR_LANES_SEED_v2-draft.md`, graduating as `GRAPH_MODE_SOP.md`).

## Standing rules

- **Never on `main`.** Work on `feat/`/`fix/`/`wip/`/`refactor/` branches.
- **Stage by explicit path, never `git add -A`.** A lane commit is limited to
  the files that lane produced; verify with `git diff --cached --name-only`.
- **Red-first, checker is never the lane.** A done-means is executable, written
  BEFORE the work, proven able to fail, authored by a DIFFERENT actor. Re-prove
  RED after any edit to the check.
- **Harvest barrier.** Lanes may pipeline; harvest completes before the next
  dispatch. An un-harvested lesson is a defect of the accepting merge pass.
- **ABSENT is announced, never skipped.** Conventions are discovered, not
  hardcoded; a silent no-op in a non-conforming repo is the failure this closes.
- **No secrets** in git, logs, reports, PRs, or fixtures.

## Conventions a cold agent must discover

- **Lane contract:** this file (`docs/lane-contract.md`).
- **Done-means checks:** `scripts/done-means/` — exit grammar `0` pass /
  `1` under-test failed / `3` harness error.
- **Class vocabulary:** none registered yet — the Tightenings below ARE the
  vocabulary; unclassified work lands in `verifier` tier 3. Honest starting
  state, tailor per repo as classes earn entries.

## Tightenings

<!-- Dated log; harvest-scribe drafts here, the accepting merge pass lands it.
     Start empty — entries must be about THIS repo's lanes. -->

_(empty — no lanes have run under this contract yet)_
