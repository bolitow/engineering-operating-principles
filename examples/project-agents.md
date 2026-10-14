# Example: project-specific agent instructions

> Adapt this example to your repository. Do not copy placeholder commands without checking them.

## Project context
- Purpose: [What the application does]
- Stack: [Languages, frameworks, runtime]
- Architecture: [Key modules and boundaries]
- Owners: [Accountable maintainer or team, required independent reviewers, and escalation when unavailable]
- Related projects: [Shared contracts and affected consumers; omit if none]

## Development commands
- Install: `[command]`
- Type check: `[command]`
- Test: `[command]`
- Build: `[command]`

## Invariants and verification
List only important properties. These examples are illustrative, not requirements for every project.

| Property | Owning boundary | Verification and counterexample |
| --- | --- | --- |
| [A retry does not create a second payment] | [Payment service] | [Repeat the request with the same key; reject duplicate records] |
| [A tenant cannot read another tenant's data] | [Authorization and storage] | [Cross-tenant integration request must fail] |

- Hermetic checks: [Commands and controlled clock, seed, fixtures, or dependencies]
- Integration checks: [Real boundaries, required environment, and remaining gaps]
- Required pre-merge / pre-deploy checks: [Keep existing controls explicit]
- Shared-contract verification: [Consumer versions, checks, and accountable owner]

## Approval boundaries
- Agent may autonomously: [Low-risk scoped changes]
- Human approval required: [Migrations, public APIs, production actions]

## Definition of done
- [Relevant tests and checks pass]
- [Diff reviewed]
- [Risks and unverified areas disclosed]
- [Required independent review completed; pending review means not ready for merge]

## Evidence and experiments
- Record location: [Existing issue, PR, or decision log; avoid a duplicate ledger]
- Repeatability: [Revision, environment, fixture or input, command, and result]
- Current delivery bottleneck: [Measured stage, baseline, or explicitly unknown]

Keep local facts in this supplement and general investigation and review rules in the root `AGENTS.md`; neither document overrides enforced permissions.
