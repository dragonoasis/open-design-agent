---
name: content-design
description: Design product language, labels, instructions, errors, empty states, onboarding, voice, content models, and localization-ready UX copy grounded in user tasks and product truth.
---

# Content Design

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use when language affects understanding, action, trust, recovery, onboarding, navigation, or brand voice. Content design is part of the interaction model, not text added after layout.

## 1. Define the content job

For each message, identify:

- audience and context
- user question
- action or decision
- product/system truth
- consequence
- persistence and urgency
- next step

Do not optimize wording before the underlying action or policy is coherent.

## 2. Build a content hierarchy

Separate:

- page or task purpose
- section orientation
- control label
- instruction
- supporting explanation
- status or feedback
- legal/policy detail
- next action

Use progressive disclosure. Critical requirements and consequences must not be hidden behind tooltips or legal links.

## 3. Name by user meaning

Labels should:

- use the audience's vocabulary
- distinguish sibling choices
- describe the object or outcome
- remain stable across navigation, heading, and action where meaning is shared

Avoid internal team names, implementation terms, vague nouns, and clever labels that lose information scent.

## 4. Write actions as outcomes

Buttons and links should indicate what will happen:

- “Save draft”
- “Send invitation”
- “Delete workspace”

Use generic “Continue” only when the next step is obvious from context. Distinguish cancel, close, back, skip, and undo by actual behavior.

## 5. Design state-specific language

### Loading

State what is happening when useful. Do not promise a duration that is unknown.

### Empty

Distinguish:

- first use
- no results
- filtered-out results
- unavailable data
- permission limitation
- cleared or completed state

Explain what belongs here and offer the relevant next action.

### Error

- identify the failed action or affected field
- avoid blame
- preserve context
- explain what the user can do
- state when support or waiting is the only path
- avoid raw codes unless they help support

### Success

Confirm the consequential result and any next step. Do not celebrate routine actions so heavily that the interface slows down.

### Destructive or consequential action

Name the object, scope, permanence, dependent effects, and recovery. The confirmation action must not be ambiguous.

## 6. Create voice as behavior

Define voice dimensions such as:

- direct versus conversational
- calm versus energetic
- formal versus informal
- expert versus explanatory

Then adapt tone to state. Errors, health, finance, privacy, and crisis contexts require restraint even when the brand is playful.

Do not use personality to obscure responsibility.

## 7. Design onboarding content

- lead with the real value and next task
- explain permissions in context
- teach concepts when they become relevant
- make optional education skippable
- avoid feature dumps and repeated motivational filler
- support return and replay

## 8. Prepare for localization

- avoid concatenated sentences and UI-dependent word order
- provide translator context
- support expansion and script differences
- use locale-aware dates, numbers, names, addresses, and plurals
- avoid idioms, puns, and culture-bound metaphors when they obstruct translation
- keep text out of images

Test bidirectional meaning and mixed-script content.

## 9. Govern content

For reusable content patterns, define:

- owner
- source of truth
- variables and allowable values
- review and expiry
- legal/regulated review
- localization status
- measurement

Dynamic messages must handle missing, long, and unsafe values.

## Output

- content purpose and audience
- hierarchy/content model
- proposed copy by state
- voice/tone rationale
- localization notes
- truth, legal, or policy dependencies
- content acceptance criteria

## Checks

- Every message helps understanding, action, trust, or recovery.
- Labels and outcomes are distinct.
- Errors own system failure and give a path.
- Empty states reflect the actual cause.
- Voice adapts to consequence.
- Copy is truthful, localizable, and resilient to dynamic content.
