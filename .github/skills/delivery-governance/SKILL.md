---
name: delivery-governance
description: Produce implementation-ready handoff, design QA, decision records, system documentation, versioning, debt management, adoption plans, and outcome reporting.
---

# Delivery and Governance

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use when design moves into implementation, review, release, maintenance, or organizational adoption.

## 1. Handoff as an executable contract

Include:

- scope and user outcome
- links to source artifacts
- content and data requirements
- responsive/platform behavior
- component anatomy and variants
- state and transition behavior
- accessibility requirements
- assets and ownership
- analytics and outcome events
- acceptance criteria
- known risks and open decisions

Do not hand off only dimensions and colors.

## 2. Decision record

For material decisions:

```text
decision:
date:
owner:
context:
evidence:
alternatives:
choice:
tradeoff:
revisit_trigger:
```

Record why, not a transcript of discussion.

## 3. Design QA

Review the implemented artifact at:

- representative viewports/devices
- keyboard and touch
- loading, empty, success, error, disabled, permission, and offline states
- real and extreme content
- light, dark, high contrast, reduced motion
- localization and bidirectionality where supported
- slow network and constrained performance

Compare:

- task and information architecture
- behavior and state
- accessibility
- hierarchy and visual system
- approved direction

Do not reduce QA to pixel differences. An implementation adaptation is acceptable when it improves platform behavior or accessibility and is recorded.

## 4. Defect record

Each finding includes:

- evidence
- expected behavior
- actual behavior
- affected user/task
- severity
- owner
- acceptance check

Separate design defect, implementation defect, content defect, data/service defect, and accepted deviation.

## 5. Document the shipped truth

After implementation, update:

- tokens actually used
- component behavior
- pattern guidance
- responsive/platform decisions
- accessibility notes
- known exceptions
- examples and anti-examples

Do not promote a one-off value or workaround into the system. If the artifact contradicts an approved decision, resolve the contradiction rather than documenting both as truth.

## 6. Version and change

Define:

- semantic or product-appropriate versioning
- release notes
- migration path
- deprecation and removal dates
- compatibility and fallback
- communication channels
- ownership and support

Breaking visual change can be behavioral when it alters hierarchy, target location, or recognition.

## 7. Manage design debt

Classify:

- duplicated component or pattern
- token drift
- accessibility gap
- inconsistent behavior
- unsupported platform
- outdated content
- documentation drift
- research or truth drift

Prioritize by user impact, frequency, risk, system spread, and repair leverage. Do not use inconsistency count alone.

## 8. Adoption as behavior change

Plan:

- stakeholder and team needs
- pilot products
- training and examples
- contribution path
- migration support
- feedback and support
- incentives and governance

Measure appropriate use, update latency, defects, duplicate work, and task cost—not only component import counts.

## 9. Report impact honestly

Connect:

- design change
- intended mechanism
- user behavior or outcome
- organizational measure
- guardrails
- evidence confidence

Distinguish correlation, experiment, qualitative evidence, and anecdote. Do not attribute a business outcome entirely to design without evidence.

## Output

Depending on scope:

- implementation handoff
- acceptance matrix
- QA report
- decision record
- shipped design documentation
- release/migration plan
- debt register
- adoption plan
- impact report

## Checks

- Engineering can implement behavior without guessing.
- QA covers states and inputs, not only ideal screenshots.
- Documentation reflects shipped truth.
- Exceptions and debt have owners.
- Impact claims match evidence.
