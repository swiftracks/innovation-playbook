# Deep Methodology Note — Handling Multi-Cycle Evidence Conflict

## Purpose

Define a rigorous method for resolving conflicting evidence across multiple cycles without defaulting to either paralysis or overreaction.

## Outcome

Teams produce a weighted, decision-ready interpretation with explicit confidence and residual uncertainty.

## Context and Problem Framing

Teams sometimes accumulate evidence across multiple cycles that points in different directions.
Without a method for weighting evidence quality, they either freeze decisions or overreact to the latest signal.

## Scope and Assumptions

- Scope: experiment-to-learning synthesis across two or more cycles.
- Assumption: core hypothesis remains stable while execution conditions vary.
- Constraint: decisions must still be made on cadence.

## Method Logic

1. Separate evidence by cycle and by signal reliability.
2. Score each signal for methodological quality (sample integrity, measurement validity, bias risk).
3. Compare confidence shifts by weighted signal class, not raw count.
4. Draft decision options with explicit tradeoffs:
   - go with bounded risk,
   - iterate test design,
   - pivot hypothesis branch,
   - stop current path.

## Evidence Model and Quality Thresholds

- Strong evidence: meets pre-declared criteria with acceptable reliability.
- Partial evidence: meets some criteria but has known constraints.
- Weak evidence: inconclusive or confounded.

Decision thresholds:

- Go requires dominant strong evidence and acceptable downside.
- Iterate requires meaningful but non-conclusive evidence.
- Pivot requires repeated failure against valid criteria.
- Stop requires high-confidence negative signal with weak recovery path.

## Decision Model and Tradeoffs

- Fast decision bias can improve speed but increase false positives.
- Conservative decision bias reduces false positives but risks slower learning velocity.
- Teams should pick bias consciously based on consequence severity.

## Failure Modes and Recovery

- Failure mode: latest-cycle bias overrides stronger historical evidence.
  - Recovery: use weighted evidence review before decision.
- Failure mode: teams call a pivot without falsification-quality proof.
  - Recovery: require explicit invalidation trace.

## Handoff Implications

When this method is used, downstream planning should include:

- explicit confidence level,
- known uncertainty debt,
- and one validation checkpoint in the next cycle.

## Next step

Apply [Decision Readiness Checklist](decision-readiness-checklist.md) before committing to `go`, `iterate`, `pivot`, or `stop`.
