---
name: design-systems
description: Define and govern semantic tokens, themes, components, patterns, documentation, migration, contribution, versioning, and adoption for scalable products.
---

# Design Systems

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use for token architecture, component libraries, themes, pattern governance, migrations, documentation, audits, and adoption.

A design system is a decision and delivery system, not a component gallery.

## 1. Define system boundaries

Record:

- products and platforms served
- teams and ownership
- shared versus product-specific decisions
- supported themes, locales, inputs, and accessibility targets
- source of truth and release mechanism
- adoption and deprecation policy

Do not centralize a one-off marketing expression merely because it uses CSS.

## 2. Architect tokens

Use layers:

1. **primitive:** raw palette, dimension, font, duration, easing
2. **semantic:** purpose such as surface, text, action, status, focus
3. **component:** controlled component-level decisions

Prefer aliasing:

```text
component -> semantic role -> primitive
```

Define:

- naming grammar
- mode/theme mapping
- platform overrides
- fallback and contrast pairs
- ownership and change policy
- deprecated and replacement tokens

Components should not consume raw palette values without a documented exception.

## 3. Design themes by role

For light, dark, high contrast, brand, or product themes:

- remap semantic roles
- verify every state
- preserve hierarchy and contrast
- keep status meaning stable
- test media, charts, shadows, borders, and overlays

Theme parity is semantic, not numeric.

## 4. Specify components

Each component specification includes:

- purpose and when not to use
- anatomy and semantic elements
- properties and variants
- size and density behavior
- content rules
- states and transitions
- keyboard, focus, announcement, and accessibility
- responsive/platform adaptation
- localization and direction
- tokens and extension points
- examples, anti-examples, and related patterns
- implementation status and version

Avoid variants that differ only because a page needed an unreviewed override.

## 5. Define patterns above components

Document task patterns such as:

- forms and validation
- search and filtering
- empty and error recovery
- navigation
- data tables
- onboarding
- destructive confirmation
- chat and streaming

Patterns explain component composition and behavior across a user outcome.

## 6. Govern exceptions

An exception record includes:

- product need
- why the system cannot satisfy it
- accessibility and maintenance impact
- owner
- expiration or review date
- whether it should become a contribution

Do not hide exceptions as arbitrary class overrides.

## 7. Migrate behavior-first

When changing libraries or versions, inventory:

- wrapper and composition anatomy
- consumer props and callbacks
- DOM element and semantics
- focus, dismissal, activation, and value behavior
- portal, positioning, collision, and layering
- data attributes, class selectors, and CSS variables
- defaults and unsupported capabilities

Classify:

- mechanical rewrite
- intentional behavior change
- unsupported behavior delta
- product decision required

Never claim parity from matching imports or screenshots.

## 8. Document and release

Use:

- versioned change records
- contribution and review criteria
- accessibility acceptance
- visual/behavior regression coverage
- migration guidance
- deprecation windows
- ownership and support

Document what ships. Do not canonize a defect or a token used once.

## 9. Drive adoption

Measure:

- product coverage
- component reuse with appropriate exceptions
- update latency
- accessibility defects
- duplicate patterns
- contribution throughput
- developer and designer task cost

Raw adoption percentage is not success if teams bypass behavior or accessibility.

## Output

- system boundary and ownership
- token schema
- theme contract
- component/pattern specification
- exception and contribution process
- release/migration plan
- adoption and health measures

## Checks

- Semantic contracts permit meaningful visual variation.
- States and accessibility are first-class.
- Platform overrides do not fragment product meaning.
- Unsupported migration deltas are explicit.
- Documentation matches implementation.
