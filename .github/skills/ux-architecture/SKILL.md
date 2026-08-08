---
name: ux-architecture
description: Define user outcomes, information architecture, task flows, navigation, search, forms, onboarding, content strategy, journeys, and service dependencies before polish.
---

# UX Architecture

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use for product structure, workflows, navigation, content, service design, or when visual problems may originate upstream.

## Input

- user and organizational outcomes
- evidence and research confidence
- content/data model
- platform and permissions
- existing IA, analytics, support findings, or service constraints
- high-risk or regulated context

Do not present unsupported personas, journeys, or jobs as research. Label them hypotheses.

## Workflow

### 1. Frame the job and outcome

Record:

- situation and trigger
- desired progress
- current alternative
- success from the user's perspective
- organizational outcome
- risks and unacceptable outcomes

Avoid demographic personas when behavior, context, expertise, access needs, or motivation is more relevant.

### 2. Model content and entities

Identify:

- core objects and relationships
- required attributes and states
- ownership, permissions, lifecycle, freshness, and source
- user language and ambiguous terms
- what can be searched, filtered, sorted, grouped, or compared

Interface architecture cannot compensate for a contradictory content model.

### 3. Define task flows

For each primary task:

- entry points
- prerequisites
- happy path
- alternate paths
- interruption and resume
- validation and error recovery
- cancel, undo, and exit
- confirmation and next step
- cross-device or cross-role handoff

Mark service or policy dependencies.

### 4. Design information architecture

Choose organizing principles:

- task
- object
- audience
- lifecycle
- topic
- location
- chronology
- frequency

Create a sitemap or object map, then validate labels and grouping. Do not use internal org structure unless it matches user expectations.

### 5. Select navigation

Decide:

- global, local, contextual, and utility navigation
- current location and hierarchy
- deep-link and back behavior
- persistent versus temporary destinations
- mobile and wide-screen adaptation
- keyboard and assistive traversal

Navigation follows structure and frequency, not a fashionable shell.

### 6. Design search and discovery as a system

Specify:

- query entry and scope
- suggestions and recent items
- filters, sort, and active constraints
- result anatomy and ranking cues
- result counts and freshness
- no-match, unavailable, and system-error states
- query persistence and return

Do not confuse no results with failed search.

### 7. Design forms around intent

- request only necessary information
- use persistent labels
- group by user intent
- provide defaults and examples where helpful
- expose requirements before submission
- time validation to help rather than interrupt
- preserve input on recoverable failure
- use field and summary errors according to scope
- explain why sensitive data is needed

The backend schema is not a form architecture.

### 8. Design onboarding toward value

Choose:

- immediate task
- contextual guidance
- sample content
- guided setup
- optional tour
- progressive permissions

Make optional education skippable and replayable. Do not front-load every feature.

### 9. Map service reality

When backstage processes affect the experience, record:

- frontstage action
- system response
- human or service dependency
- data source
- delay and failure mode
- support and escalation

Fix service failures upstream where possible rather than adding interface apology layers.

## Output

- outcome and scope statement
- object/content model
- primary and alternate task flows
- IA and navigation model
- search/form/onboarding specification as relevant
- service dependency map
- assumptions and research confidence
- measurable success and guardrails

## Checks

- Users can predict where to go and what happens next.
- Every primary task has recovery and exit.
- Labels use user language.
- Permission and data consequences are visible.
- The design does not rely on speculative research artifacts.
- Visual complexity is not masking structural complexity.
