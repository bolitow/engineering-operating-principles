# Sources and adaptation

This note records why the operating guide changed. It is background, not an additional approval process. Sources were read on 14 October 2026; no REA software or source-control prototype was run to validate their claims.

## Reported facts from Anthropic

[Redesigning source control at Anthropic](https://www.anthropic.com/engineering/redesigning-source-control), published 13 October 2026:

- **“Growing our monorepo” and “Contributing to the wider ecosystem”:** the workload is exceptional; Scion is not presented as a general Git replacement.
- **“Principles for agent-scale source control”:** APIs and sparse access reduce the repository data clients need.
- **“What we learned building Scion”:** engineers preserve system constraints, review change intent, and restrain overengineering from adversarial reviews. The team reports hermetic simulations and a shift toward post-merge and pre-deploy testing under extreme merge concurrency.

These are the authors' reports, not measurements reproduced here or evidence that our projects share their bottlenecks.

## Documented method from REA

References are pinned to revision `f75b1a416ba67b8421e7dbd248160afedb79581f`:

- [Repository guidelines — Product and Authority; Performance](https://github.com/morluto/rea/blob/f75b1a416ba67b8421e7dbd248160afedb79581f/AGENTS.md): distinguish kinds of evidence and unknowns; measure completed workflows with their limitations.
- [Reconstruction obligation ledgers — opening contract; Manifest and closure](https://github.com/morluto/rea/blob/f75b1a416ba67b8421e7dbd248160afedb79581f/docs/reconstruction-obligation-ledgers.md): link claims, implementation ownership, cases, and comparable verification; unresolved evidence prevents closure.
- [Touhou reconstruction method — Autonomy, oracles and the compounding flywheel; TH08's floating-literal oracle failure](https://github.com/morluto/rea/blob/f75b1a416ba67b8421e7dbd248160afedb79581f/website/evidence/touhou-reconstruction-method.md): preserve checked results and lessons, and test the verifier. A historical comparison missed incorrect referenced data despite matching instructions. The note attributes the historical work to its original projects, not exclusively to REA.

## Analogies and recommendations for our team

The following are our adaptations for two developers and multiple technology stacks, not instructions or measured results from either source.

| Analogy | Recommendation | Boundary |
| --- | --- | --- |
| A reconstruction claim resembles a feature acceptance claim | Link each consequential invariant to a check and a responsible component in the existing task record | No REA installation, formal ledger schema, or proof of equivalence required |
| An independent oracle resembles a regression or contract test | Use an expected result independent of the implementation, plus a known bad case for critical checks | Passing fixtures only establish the properties exercised |
| Constraining an agent resembles reviewing a design | Write invariants before implementation; review intent, evidence, and risky code with the other developer | Agent critique does not replace human ownership or required approval |
| Fetching only useful data resembles focused investigation | Start with relevant paths and consumers, expand as evidence requires | Do not hide dependencies or mistake search scope for completeness |
| Infrastructure changes follow observed pressure | Measure a local delivery bottleneck and run a small reversible trial | Retain Git and pre-merge controls; no migration or reduced protection by analogy |

Keep the rules in [AGENTS.md](../AGENTS.md), local commands and ownership in the [project supplement](../examples/project-agents.md), and task-specific evidence in the [task brief](../examples/task-instructions.md). Use existing issues, PRs, and decision records rather than creating parallel reporting systems.

Start adoption with one representative task. Record where time and rework occurred, whether the checks detected the intended failure, and whether the second developer could assess the decision from the evidence. Keep useful guidance and simplify friction; this is a proposed trial, not a claimed productivity gain.
