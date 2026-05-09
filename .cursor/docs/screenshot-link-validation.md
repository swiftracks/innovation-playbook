# Screenshot Link Validation Report

## Scope

Validated screenshot references across:

- `start-here/30-minute-activation.md`
- `run-learning-cycles/README.md`
- `run-learning-cycles/01-idea-problem.md`
- `run-learning-cycles/02-identify-critical-assumptions.md`
- `run-learning-cycles/03-form-testable-hypotheses.md`
- `run-learning-cycles/04-design-run-experiments.md`
- `run-learning-cycles/05-extract-key-learnings.md`
- `.cursor/docs/run-learning-cycle-guide.md`

## Naming consistency status

All in-repo references now use the normalized naming set:

- `01-workspace-dashboard.png`
- `02-project-dashboard.png`
- `03-kickoff-conversation.png`
- `04-clarifying-questions-conversation.png`
- `05-select-assumptions.png`
- `06-select-hypothesis.png`
- `07-select-experiment.png`
- `07.1-selected-experiment.png`
- `08-experiment-draft-ems.png`
- `08.1-experiment-draft-coordination-ems.png`
- `08.2-experiment-draft-approval-ems.png`
- `08.3-experiment-data-tracker-ems.png`
- `08.4-experiment-data-tracker-inputs-ems.png`
- `08.5-experiment-data-tracker-lock-ems.png`
- `08.6-generate-learning-card-ems.png`
- `08.7-generate-learning-card-submit-ems.png`
- `09-learning-card-draft-ems.png`
- `09.1-insights-library-ems.png`
- `09.2-conversation-sources.png`

## Filesystem validation result

- Directory checked: `innovation-playbook/screenshots/`
- Current visible `.png` files: `0`

This means markdown references are normalized, but binary assets are currently missing or not visible in this workspace checkout.

## Remediation list

1. Confirm whether screenshots are tracked via Git LFS or external storage.
2. Restore or copy the 19 expected screenshot assets into `innovation-playbook/screenshots/`.
3. Re-run link validation after assets are restored.
4. If any filename differs from the canonical list above, update docs to match actual file names.

## Documentation fallback rule

Until image assets are restored, keep the references in place (do not remove) so pages remain ready for publication once files are available.
