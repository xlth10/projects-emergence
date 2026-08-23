---
name: projects-emergence
description: Develop rough ideas into research-backed, reproducible, reflective, and publishable projects. Use when a project needs problem framing, evidence gathering, a research gate before implementation, iteration, or a public handoff; skip routine low-risk edits whose requirements are already clear.
---

# Projects Emergence

Turn an early idea into a project whose decisions, implementation, and claims can be inspected and revisited.

The default loop is:

```text
clarify → research → replicate or adapt → implement → reflect → research → revise
```

This is a decision loop, not a requirement to manufacture novelty. A well-supported replication or adaptation is a valid outcome.

## Start from the decision

Establish the smallest useful shared understanding before doing substantial work:

- Who experiences the problem?
- In what situation does it occur?
- What outcome would be useful?
- What would count as success?
- Which constraints or publication boundaries matter?

Ask only for information that cannot be safely inferred. Prefer one focused question at a time when the answer will change the project direction.

## Choose proportionate research

Do not turn every task into a research project.

- For a new idea, product direction, or core hypothesis, use a full research loop.
- For an unfamiliar mechanism, architecture choice, or competing design options, use focused research.
- For a bug with an unclear cause, use diagnosis and a minimal reproduction.
- For publishing, migration, data handling, cost, privacy, or another hard-to-reverse action, use a risk check.
- For familiar, low-risk mechanical work with clear acceptance criteria, proceed directly and verify the result.

When research is needed, read [references/research-loop.md](references/research-loop.md). Stop researching when the evidence can support the next concrete decision.

## Select an honest project path

Compare existing approaches before choosing what to build:

1. **Replicate** when an established solution already meets the goal.
2. **Adapt** when the mechanism works but the user, device, style, or workflow differs.
3. **Improve** when evidence reveals a specific weakness under the project's constraints.
4. **Redesign** only when existing approaches fail a central requirement.

Record what is reused, what changes, why the change is necessary, and which claims remain unverified. Check licenses before reusing code, data, copy, or assets.

## Pass the research gate

Before substantial implementation or a consequential direction change, replay the current state:

- the problem being solved;
- the mechanism that appears to work;
- the evidence that supports it;
- the strongest uncertainty or counterexample;
- the smallest implementation that can test the hypothesis;
- the intended public/private boundary.

Pause for user confirmation when this replay changes product direction, implementation scope, publication strategy, cost, or another material commitment. Approval to implement does not authorize commits, pushes, deployments, messages, purchases, or other external actions unless the user also requested them.

## Implement the smallest informative slice

After the gate passes:

1. Reproduce the critical mechanism or observable behavior.
2. Make the smallest change that tests the project hypothesis.
3. Verify behavior with a test, log, comparison, user check, or other relevant evidence.
4. Keep reference behavior and original contributions distinguishable.
5. Preserve uncertainties instead of presenting them as conclusions.

Use the templates in `assets/` only when persistent project records are useful. Do not create process files merely to satisfy the skill.

## Reflect and loop

After a meaningful implementation, assess:

- Did it solve the stated problem?
- Is the chosen path better than simply using the reference solution?
- Which conclusion still lacks evidence?
- What is the most fragile part of the result?
- What would change first if the project were repeated?

Choose reflection questions appropriate to the project:

- Product: user, context, value, usability, alternatives.
- Tool: interface, failure modes, boundaries, maintenance.
- Research: hypothesis, replication fidelity, experiment quality, evidence strength.
- Creative: expression, distinctiveness, audience response, finish.
- Data: provenance, bias, metrics, reproducibility.

If reflection exposes a material weakness, define the next decision and re-enter research with the smallest evidence budget that can resolve it.

## Coordinate larger workspaces only when needed

For a portfolio, multi-project repository, parallel Codex tasks, or Git worktrees, read [references/workspace-modes.md](references/workspace-modes.md). Keep each project isolated and give one place authority over shared indexes or public metadata.

## Publish with evidence

Before a public handoff:

- remove private paths, credentials, personal records, and internal-only sources;
- attribute external work and state relevant licenses;
- distinguish demonstrated results from hypotheses;
- include a minimal reproduction, example, or case study;
- state known limitations and the next validation needed;
- obtain explicit approval immediately before pushing, deploying, submitting, or announcing.

The public artifact should make the result understandable. The repository should make it reproducible. Private working notes can retain the fuller history.
