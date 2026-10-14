# Engineering Operating Principles

**A practical operating guide for autonomous AI coding agents.**

A reusable `AGENTS.md` for individual maintainers, teams, and multi-team organizations. It helps coding agents act like thoughtful engineering collaborators: inspect before changing, challenge assumptions, keep changes scoped, test claims, and communicate risks.

## Why this exists

Coding agents can generate code quickly. Reliable engineering requires more: understanding existing systems, making proportionate decisions, preserving boundaries, and validating outcomes.

These principles provide a starting point—not a substitute for project documentation, permission controls, code review, or CI.

## Quick start

1. Copy [AGENTS.md](./AGENTS.md) into the root of your repository.
2. Add project-specific architecture, commands, tests, and approval requirements.
3. Give the agent a concrete task with scope and acceptance criteria.
4. Enforce permissions and CI outside the prompt.

For a lightweight project-specific supplement, see [examples/project-agents.md](./examples/project-agents.md). For a reusable task brief, see [examples/task-instructions.md](./examples/task-instructions.md).

## Adapting this to your organization

Whether working as an individual maintainer, a team, or multiple teams across one or several technology stacks, keep the common principles here and put commands, invariants, ownership, and approval rules in each project's supplement. Assign accountable owners and qualified independent reviewers according to the project's risk and approval requirements, not a fixed headcount. Start with one real task; use its existing issue or pull request to record assumptions, evidence, and review outcomes. A separate process document is optional.

When independent human review is required, an individual maintainer may need an external qualified reviewer. An unavailable reviewer does not remove the approval requirement.

The working loop is: define the outcome and invariants, inspect evidence, test an explicit hypothesis when uncertainty warrants it using the smallest useful change, then review the result and record what remains unknown. Use deeper independent review for consequential changes; routine edits need no standing review committee.

Keep Git and existing pre-merge checks. Changes to engineering infrastructure need a measured local problem, a bounded experiment, and human agreement—not another organization's scale as justification. See [sources and adaptation](./docs/sources-and-adaptation.md) for the distinction between source findings, analogies, and our recommendations.

## Operating modes

| Mode | When to use |
| --- | --- |
| Explore | Investigate options and validate hypotheses |
| Architect | Audit existing systems and compare structural options |
| Execute | Implement and test within approved boundaries |
| Review | Critically assess diffs and risks |

## Design philosophy

**Think before building. Challenge assumptions. Reuse before recreating. Validate before declaring success.**

## Scope and limitations

This repository is agent-agnostic. Support for `AGENTS.md` and instruction precedence varies by coding agent; check the documentation for your tool. Prompt instructions do not enforce security boundaries or guarantee agent behavior.

## Contributing

Issues and pull requests are welcome. Propose changes with a concrete problem, examples, and trade-offs. Keep guidance actionable and proportional.

Use English for this repository's canonical guide, documentation, examples, commit messages, and pull requests. Projects adopting the guide may choose their own language conventions.

## License

MIT — see [LICENSE](./LICENSE).
