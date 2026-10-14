# Example: task brief for a coding agent

## Mode
[Explore | Architect | Execute | Review]

## Objective
[State the user outcome, not only a proposed implementation.]

## Current context
[Relevant architecture and constraints. Link observed facts to files/revisions or source sections. Label source-derived conclusions, hypotheses, and unknowns separately.]

## Authorized scope
[Repositories, directories, tools, environments, and allowed actions.]

## Out of scope
[What must not be changed.]

## Acceptance criteria
- [Observable outcome]
- [Tests or verification evidence]

## Invariants and experiment (when uncertainty matters)
- Must remain true: [Property and owning component]
- Hypothesis: [Expected explanation or improvement]
- Baseline and smallest experiment: [Comparable input, revision, environment, and command]
- Rejection case: [Counterexample or result that would disprove the hypothesis]
- Evidence to retain: [Result, fixture or seed, limitations; use the existing issue or PR]

For a straightforward edit, omit this section instead of inventing an experiment.

## Review
[Review intent and evidence, then risk-sensitive implementation details. Name the second developer when independent human review is required; record pending review explicitly.]

## Risk and approval gates
[Decisions requiring human approval.]

## Expected response
- Findings grounded in actual files
- Recommendation and trade-offs when relevant
- Changes made, if authorized
- Tests actually run and results
- Remaining risks and unknowns

Do not treat an architectural suggestion as authorization to refactor.
