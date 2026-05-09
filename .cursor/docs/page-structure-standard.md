# Playbook Page Structure Standard

Use this standard for all rewrites in `innovation-playbook` except the frozen homepage (`README.md`).

## Global writing goals

1. Keep every page easy to skim and deep enough to execute.
2. Explain why each stage matters before telling people what to click.
3. Keep voice aligned to SwiftCNS: direct, evidence-grounded, coaching, sober.
4. Preserve canonical loop language: `assumptions -> hypotheses -> experiments -> learnings -> insights -> decisions`.

## Standard section order

Use this order unless a page type explicitly overrides it.

1. `Purpose`
2. `Who this is for`
3. `Outcome`
4. `Why this matters`
5. `Inputs` or `Prerequisites`
6. `How it works` or `Steps in SwiftCNS`
7. `Quality gates`
8. `Outputs`
9. `Definition of done`
10. `Next step`

## Page-type adaptations

### Walkthrough pages

- Include one primary UI transition per step.
- For each step: `screen context -> user action -> expected outcome -> common mistake`.
- Keep screenshot references deterministic and close to the relevant step.

### Method pages

- Explain stage logic and decision implications.
- Include weak-vs-strong patterns or anti-patterns.
- Link upstream/downstream stages explicitly.

### Checklist and rubric pages

- Keep concise structure.
- Add interpretation guidance so teams know how to act on results.
- Avoid compliance-only language.

### Internal skill/docs pages

- Keep instructions deterministic.
- Avoid decorative storytelling.
- Preserve tool contracts and sequence integrity.

## Readability rules

- Use one `#` heading per file.
- Prefer short paragraphs (2-4 sentences).
- Use bullets for criteria and checklists, not for entire narrative.
- Keep table usage purposeful and compact.
- Avoid duplicative headings with similar meaning.

## Brand and terminology guardrails

- Frame SwiftCNS as a learning system that resolves uncertainty.
- Avoid framing as backlog management or generic productivity tooling.
- Prefer terms: uncertainty, evidence, conviction, learning velocity, decision quality.
- Avoid hype and unsupported promises.

## Runtime alignment guardrails

- Present implemented behavior as current.
- Mark non-shipped behavior as planned.
- Do not invent entities, controls, or automation steps.
- For tutorial claims, require screenshot or capture-backed evidence.
