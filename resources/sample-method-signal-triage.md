# Sample Method — Signal Triage Before Learning Finalization

This is a dry-run sample page authored using the new contributor rules and skills.
It demonstrates expected structure and decision-ready methodology language.

## Purpose

Prevent weak or mixed-quality evidence from entering learning synthesis as if all evidence had equal weight.

## Outcome

A triaged evidence set with explicit confidence labels that supports a stronger learning statement.

## Inputs

- One completed experiment record
- Raw evidence artifacts (notes, metrics, transcripts, screenshots)
- Pre-declared success and invalidation criteria

## Steps in SwiftCNS

1. Gather evidence artifacts linked to the experiment.
2. Separate direct evidence from inferred interpretation.
3. Label each artifact as:
   - strong signal,
   - partial signal,
   - noise or confounder.
4. Record known constraints and anomalies that may distort interpretation.
5. Draft one confidence-shift statement tied to strongest signals.

## Quality Gates

Before moving to learning extraction:

1. Criteria alignment: each key signal maps to a declared criterion.
2. Traceability: each claim references a concrete artifact.
3. Ambiguity disclosure: unresolved contradictions are documented.
4. Confidence integrity: confidence increase/decrease is explicit and justified.

## Outputs

- Evidence triage note
- Confidence-shift statement
- List of unresolved uncertainties for next experiment iteration

## Definition of Done

- The team can explain what changed in confidence and why.
- The team can explain what remains uncertain.
- The triaged output can support a clear decision path (go, iterate, pivot, stop).

## If Blocked

If evidence quality is too weak to classify:

- mark the experiment as inconclusive,
- define the smallest next experiment needed to remove the highest uncertainty,
- avoid promoting the current result into high-confidence learning language.

## Next Step

Continue to learning extraction only when triage quality gates are satisfied.
