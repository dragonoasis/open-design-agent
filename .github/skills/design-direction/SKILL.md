---
name: design-direction
description: Frame ambiguous UI/UX briefs, classify surface and platform, decide what to preserve or change, explore materially different directions, and produce a testable direction contract.
---

# Design Direction

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use this skill for new products, major redesigns, expressive surfaces, conflicting references, or requests described only as “clean,” “premium,” “modern,” or “creative.”

Do not use a full direction exercise for a trivial local correction. Compress it to a short inference and preserve the established system.

## Input

Gather or infer:

- product, surface, and task
- primary audience and context
- user and organizational outcomes
- platform and implementation constraints
- existing brand/system assets
- real content and available evidence
- references and what the user values in them
- non-goals, risks, and deadline

Separate known facts from assumptions.

## Direction process

### 1. Diagnose the assignment

Classify:

- create, redesign, extend, migrate, or repair
- Persuade, Operate, Read, Experience, or mixed surface
- web, iOS, Android, adaptive, or artifact-only
- preserve, expand, or replace for:
  - brand
  - content
  - information architecture
  - interaction
  - tokens
  - components
  - motion

Name the current failure in behavioral terms. “Looks dated” is incomplete; identify whether hierarchy, trust, density, expression, affordance, or system coherence is failing.

### 2. Find the product truth

Choose one or more evidence anchors:

- actual product UI
- real task widget
- real data or calculation
- code or technical artifact
- product photography
- editorial photography
- illustration tied to the subject
- customer or service interaction
- authoritative content

Do not let generic decoration become the only source of specificity.

### 3. Set independent axes

For each direction, state:

- density
- variance
- motion
- temperature
- depth/material
- geometry
- type character by role
- color role strategy
- imagery treatment
- evidence intensity

Avoid named style bundles unless the user explicitly requests one. “Brutalist” or “luxury” still needs observable decisions.

### 4. Explore materially different directions

When exploration is justified, create three directions. Each must change at least four material axes, including composition or evidence anchor.

Bad variation:

- same centered hero in blue, green, and orange
- same cards with different radius
- light and dark versions of one layout

Useful variation:

- editorial type-led narrative with documentary imagery
- product-first technical proof with dense live UI
- restrained object gallery with material photography

For each direction, provide:

| Field | Required content |
|---|---|
| Thesis | one sentence describing the design's argument |
| Surface promise | what the user should understand or accomplish |
| Composition | reading path, grid tension, focal structure |
| Type | display, UI, reading, data, and technical roles |
| Color | neutral temperature, action domain, semantic separation |
| Material | flat, line, surface, shadow, image, texture, atmosphere |
| Evidence anchor | what makes the design truthful and specific |
| Motion | purpose and intensity; reduced path |
| Signature | one or two memorable, subject-specific devices |
| Risk | likely usability, accessibility, performance, or brand failure |
| Rejection | patterns explicitly excluded |

### 5. Select rather than average

Score directions against:

- user outcome
- content fit
- platform fit
- brand truth
- accessibility and performance risk
- implementation feasibility
- distinctiveness without imitation

Choose one. If evidence is insufficient, identify the prototype or test that would decide.

## Direction contract

Return:

```text
THESIS:
SURFACE:
PLATFORM:
USER OUTCOME:
ORGANIZATIONAL OUTCOME:
EVIDENCE ANCHOR:
COMPOSITION:
TYPOGRAPHY:
COLOR ROLES:
GEOMETRY:
DEPTH / MATERIAL:
DENSITY:
VARIANCE:
MOTION:
RESPONSIVE INTENT:
PRESERVE:
EXPAND:
REPLACE:
NON-GOALS:
RISKS:
VALIDATION:
```

Every field must contain an executable decision, not a mood adjective.

## Checks

- Directions differ structurally, not cosmetically.
- The selected direction can support real content extremes.
- Signature devices arise from product truth.
- Brand and semantic colors cannot be confused.
- Motion has a purpose and equivalent path.
- The direction does not copy a reference brand's expression.
- Unknowns that could invalidate the direction are visible.
