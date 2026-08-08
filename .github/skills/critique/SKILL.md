---
name: critique
description: Audit designs and implementations across product truth, UX, interaction, visual craft, accessibility, responsiveness, systems, and evidence, then prioritize causal fixes.
---

# Design Critique

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use for design reviews, screenshot critiques, implementation audits, design-debt assessment, or a final quality pass.

Critique is diagnosis, not taste commentary. Do not edit while diagnosing unless the task explicitly combines review and repair.

## Inputs

Use the strongest available:

- original request and user decisions
- product/content requirements
- direction contract
- flows and state specification
- design-system source
- artifact or implementation
- representative screenshots/states/viewports
- validation evidence

Name missing evidence. A screenshot cannot prove semantics, keyboard behavior, loading, performance, or assistive-technology support.

## Review order

### 1. Truth and task

- Is the product promise accurate?
- Is the primary user outcome clear?
- Are content, metrics, people, and claims real or labeled?
- Can the primary task begin and finish?
- Are risk and consequence visible?

### 2. Structure

- Does IA match user language and object relationships?
- Is reading order intentional?
- Are navigation and location clear?
- Are forms, search, and workflows grouped by intent?

### 3. Behavior and state

- Are all plausible states represented?
- Are transitions, focus, feedback, persistence, and recovery coherent?
- Are loading and progress honest?
- Do overlays, gestures, streaming, and live updates preserve control?

### 4. Accessibility and platform

- Are structure, names, focus, input parity, contrast, zoom, reflow, media alternatives, and reduced motion accounted for?
- Does the design fit the chosen platform rather than imitate another?
- Are localization and direction risks visible?

### 5. Visual causality

Review together:

- hierarchy
- composition
- typography
- color
- spacing
- affordance
- information density
- imagery
- material and depth
- brand consistency

State what causes the problem. “Spacing is inconsistent” is weaker than “three unrelated gaps make the card title appear detached from its value and grouped with the next row.”

### 6. System and delivery

- Are semantic tokens and variants used?
- Are exceptions intentional?
- Does documentation match behavior?
- Does the implementation preserve the approved direction?
- Are performance and QA acceptance visible?

## Severity

Classify:

- **Blocker:** safety, accessibility, truth, data loss, or core task cannot proceed.
- **Major:** substantial misunderstanding, failure, exclusion, or direction contradiction.
- **Moderate:** repeated friction or system inconsistency with a workaround.
- **Minor:** localized craft defect with little task impact.

Do not derive severity from visual prominence.

## Prioritize causal fixes

Order:

1. foundation or direction
2. task/IA
3. state and recovery
4. accessibility/platform
5. hierarchy and composition
6. system consistency
7. polish

One upstream fix may resolve several symptoms. Do not output twelve disconnected lens checklists.

## Output

First line:

```text
disposition: rebuild | fix | ship
```

Then:

### Evidence limits

What was and was not inspectable.

### Keep

What is working and must not be diluted.

### Material findings

| Priority | Severity | Evidence | User impact | Cause | Fix | Validation |
|---|---|---|---|---|---|---|

### Systemic pattern

The smallest set of root causes explaining the findings.

### Acceptance

Observable conditions for the next disposition.

Use **rebuild** when the task model, direction, topology, or accessibility foundation is wrong; **fix** when the foundation holds but material defects remain; **ship** only when applicable gates pass.
