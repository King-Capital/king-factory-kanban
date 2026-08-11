# Done-Means Checks — king-factory-kanban

Executable checks that prove a claim class holds. Written BEFORE the work,
proven able to fail (RED), authored by a different actor than the impl.

## Exit-code grammar
- `0` — pass (the thing under test holds)
- `1` — the thing under test FAILED (the signal, not an error)
- `3` — harness error (the check could not run; not a verdict)

## Rules
- A failure-signal check needs a control clause proving the healthy path stays
  healthy. A control that has only ever been green is unproven.
- Re-prove RED after ANY edit to a check.

_(No checks yet — created per claim class as lanes need them.)_
