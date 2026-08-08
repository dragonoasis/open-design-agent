---
name: prototyping-validation
description: Select prototype fidelity, define scenarios and success criteria, plan usability, accessibility, heuristic, click, and experiment validation, and turn findings into decisions.
---

# Prototyping and Validation

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use when a design decision remains uncertain or when evidence is needed before implementation or release.

## 1. Name the question

Examples:

- Can users find the right destination?
- Do users understand the value proposition?
- Can users recover from a failed payment?
- Does the interaction model remain understandable without motion?
- Which of two supplied alternatives changes completion?

Do not prototype the entire product when one focused artifact can answer the question.

## 2. Select fidelity

| Question | Suitable fidelity |
|---|---|
| terminology, grouping, sequence | content model, cards, flow |
| navigation and task structure | wireframe or clickable flow |
| control behavior and state | interactive component prototype |
| visual hierarchy and brand fit | high-fidelity static or coded surface |
| motion, gesture, input, responsive behavior | coded or device-capable prototype |
| performance or assistive technology | production-like implementation |

Fidelity is cost in service of a question, not a maturity badge.

## 3. Define realistic scenarios

Scenarios include:

- participant context and motivation
- information they would realistically have
- task without revealing the interface path
- success, partial success, and failure criteria
- observation targets
- risk and stop conditions

Avoid instructions that use the exact navigation labels being tested.

## 4. Select validation layers

### Heuristic review

Use for broad expert diagnosis. Record evidence, affected task, severity, and recommendation. It does not replace user behavior.

### First-click or navigation test

Use for information scent and path choice. Track first choice, path, confidence, and recovery.

### Moderated or unmoderated usability

Measure task outcome, critical errors, recovery, time where meaningful, confidence, and qualitative explanation.

### Accessibility validation

Combine automated, manual, assistive-technology, and disabled-user testing according to risk.

### Experiment

Define:

- hypothesis and mechanism
- isolated difference
- randomization unit
- primary metric
- guardrails
- sample and duration rationale
- stopping and novelty risks
- analysis plan

Do not run an experiment to choose among fundamentally underdesigned alternatives.

## 5. Pilot

Pilot the prototype, instructions, data capture, timing, and technical setup. Fix study defects before participant sessions.

## 6. Analyze against decisions

Separate:

- observation
- task outcome
- severity
- pattern
- explanation
- recommendation
- confidence

Prioritize by task impact, affected population, frequency, consequence, and recovery—not number of comments alone.

## 7. Decide

For each research question:

- supported
- contradicted
- mixed/segment-specific
- unanswered

Then choose:

- proceed
- revise and retest
- investigate
- stop

Do not declare success from preference ratings alone.

## Output

- question and decision
- prototype scope and fidelity rationale
- participant/sample rationale
- scenarios and metrics
- test protocol
- accessibility and ethics considerations
- analysis structure
- decision rule
- limitations

## Checks

- Prototype fidelity can answer the question.
- Task wording does not teach the solution.
- Metrics connect to outcome and include guardrails.
- Findings retain evidence and uncertainty.
- Validation does not claim more than it tested.
