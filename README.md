# Engineering Operating Principles

**A practical operating guide for autonomous AI coding agents.**

A reusable `AGENTS.md` designed to help coding agents act like thoughtful engineering collaborators: inspect before changing, challenge assumptions, keep changes scoped, test claims, and communicate risks.

## Why this exists

Coding agents can generate code quickly. Reliable engineering requires more: understanding existing systems, making proportionate decisions, preserving boundaries, and validating outcomes.

These principles provide a starting point—not a substitute for project documentation, permission controls, code review, or CI.

## Quick start

1. Copy [AGENTS.md](./AGENTS.md) into the root of your repository.
2. Add project-specific architecture, commands, tests, and approval requirements.
3. Give the agent a concrete task with scope and acceptance criteria.
4. Enforce permissions and CI outside the prompt.

For a lightweight project-specific supplement, see [examples/project-agents.md](./examples/project-agents.md). For a reusable task brief, see [examples/task-instructions.md](./examples/task-instructions.md).

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

## License

MIT — see [LICENSE](./LICENSE).
