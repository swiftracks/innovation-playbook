# Playbook Rewrite Matrix

This matrix defines rewrite depth, page type, and screenshot dependency for every markdown file in `innovation-playbook`.

## Legend

- **Depth**: `light`, `standard`, `deep`
- **Screenshots**: `required`, `optional`, `none`, `validate-links`
- **Status**: `planned`, `rewriting`, `done`

## Matrix

| File | Page type | Depth | Screenshots | Notes | Status |
| --- | --- | --- | --- | --- | --- |
| `README.md` | Homepage | light | none | Frozen by request; do not modify. | done |
| `GETTING-STARTED.md` | Entry guide | deep | optional | Onboarding narrative anchor. | planned |
| `SUMMARY.md` | Navigation | standard | none | Keep scannable hierarchy and naming consistency. | planned |
| `glossary.md` | Reference | standard | none | Canonical terms and anti-drift language. | planned |
| `roadmap-and-handoff.md` | Operating boundary | standard | none | Clarify handoff outside product loop. | planned |
| `start-here/30-minute-activation.md` | Walkthrough | deep | required | Expand to full screen-backed operator story. | planned |
| `start-here/role-lenses.md` | Role guidance | deep | optional | Keep one-path model with role interpretation. | planned |
| `concept-foundations/README.md` | Foundation index | standard | none | Bridge from onboarding to loop logic. | planned |
| `concept-foundations/core-definitions.md` | Definitions | deep | none | Keep artifact distinctions explicit. | planned |
| `concept-foundations/learning-system-overview.md` | System model | deep | optional | Preserve canonical loop and continuity model. | planned |
| `concept-foundations/decision-quality-model.md` | Decision model | deep | optional | Strengthen confidence and tradeoff framing. | planned |
| `learning-cycle/fundamentals/README.md` | Fundamentals index | standard | none | Emphasize cadence and compounding quality. | planned |
| `learning-cycle/fundamentals/cycle-anatomy.md` | Method page | deep | none | Checkpoint-level execution discipline. | planned |
| `learning-cycle/fundamentals/quality-standards.md` | Quality gates | deep | none | Stage criteria and weak/strong examples. | planned |
| `learning-cycle/fundamentals/common-failure-patterns.md` | Troubleshooting method | deep | none | Recovery from weak checkpoints. | planned |
| `run-learning-cycles/README.md` | Runbook index | deep | validate-links | Source-of-truth sequence + screenshot inventory. | planned |
| `run-learning-cycles/01-idea-problem.md` | Walkthrough step | deep | required | Project and conversation kickoff quality. | planned |
| `run-learning-cycles/02-identify-critical-assumptions.md` | Walkthrough step | deep | required | Importance/evidence triage and selection. | planned |
| `run-learning-cycles/03-form-testable-hypotheses.md` | Walkthrough step | deep | required | D/F/V hypothesis framing and signal clarity. | planned |
| `run-learning-cycles/04-design-run-experiments.md` | Walkthrough step | deep | required | EMS draft->approval->tracker->completion flow. | planned |
| `run-learning-cycles/05-extract-key-learnings.md` | Walkthrough step | deep | required | Learning draft, insight library, sources compounding. | planned |
| `resources/index.md` | Resource index | standard | none | Usage guidance for checklists and rubrics. | planned |
| `resources/decision-readiness-checklist.md` | Checklist | standard | none | Repair broken next-step link and keep decision focus. | planned |
| `resources/learning-quality-rubric.md` | Rubric | deep | none | Clarify score interpretation and usage behavior. | planned |
| `resources/sample-method-signal-triage.md` | Worked method sample | standard | none | Keep as model for contributors. | planned |
| `resources/adaptive-dry-run-brief.md` | Brief mode sample | standard | none | Preserve concise tactical format. | planned |
| `resources/adaptive-dry-run-standard.md` | Standard mode sample | standard | none | Preserve stage method shape. | planned |
| `resources/adaptive-dry-run-deep.md` | Deep mode sample | deep | none | Multi-cycle conflict handling and thresholds. | planned |
| `program-operations/index.md` | Operations index | standard | none | Program-layer purpose and navigation. | planned |
| `program-operations/cadence-and-stage-gates.md` | Program method | deep | none | Review rhythm, gates, and escalation clarity. | planned |
| `program-operations/mentor-collaboration-model.md` | Collaboration method | deep | none | Intervention timing and ownership boundaries. | planned |
| `metrics/index.md` | Metrics index | standard | none | Tie measures to system improvement outcomes. | planned |
| `metrics/north-star-and-supporting-metrics.md` | Metrics model | deep | none | Interpretation guidance and metric interactions. | planned |
| `metrics/cycle-improvement-playbook.md` | Improvement method | deep | none | Diagnose->intervene->validate->standardize loop. | planned |
| `troubleshooting/README.md` | Recovery guide | deep | none | Fast diagnosis and smallest-fix recovery strategy. | planned |
| `.cursor/docs/run-learning-cycle-guide.md` | Internal capture narrative | deep | required | Canonical UX sequence source and screenshot mapping. | planned |
| `.cursor/skills/author-cns-playbook/SKILL.md` | Internal skill | standard | none | Preserve method contract, improve clarity and examples. | planned |
| `.cursor/skills/capture-cns-workflow/SKILL.md` | Internal skill | standard | required | Capture fidelity and deterministic screenshot guidance. | planned |
| `.cursor/skills/map-content-to-cns-runtime/SKILL.md` | Internal skill | standard | none | Runtime claim validation method clarity. | planned |
| `.cursor/skills/review-cns-methodology/SKILL.md` | Internal skill | standard | none | Review lens, severity model, and pass criteria clarity. | planned |
| `.cursor/skills/write-cns-tutorial-from-capture/SKILL.md` | Internal skill | standard | required | Capture-backed tutorial conversion standards. | planned |
