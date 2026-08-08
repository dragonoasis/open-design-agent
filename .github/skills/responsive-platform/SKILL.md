---
name: responsive-platform
description: Adapt layouts, navigation, content, controls, and behavior across web, iOS, Android, window sizes, input methods, localization, and accessibility preferences.
---

# Responsive and Platform Design

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use for responsive web, native adaptation, cross-platform products, localization, dynamic text, or any interface whose available space and input change.

Select the [platform profile](../../../profiles/platforms.md) first.

## 1. Inventory adaptation pressures

Test:

- content length and language
- viewport width and height
- windowed, split, folded, and full-screen modes
- pointer, touch, keyboard, stylus, voice, and assistive input
- zoom and dynamic text
- orientation and safe areas
- virtual keyboard and system UI
- reduced motion, contrast, and transparency
- slow network and low-power hardware

Do not equate narrow width with mobile capability.

## 2. Define structural invariants

Record what must remain:

- task and content priority
- reading order
- semantic relationships
- primary and escape actions
- selected object and context
- user-entered state

Visual position may change; meaning must not.

## 3. Choose content-driven transitions

For each region, identify the failure condition:

- lines become unreadable
- controls wrap ambiguously
- comparison no longer fits
- target acquisition degrades
- navigation consumes content
- side-by-side context becomes illegible
- the virtual keyboard hides the active task

Introduce a layout transition at that failure, then document the observed threshold as a system value—not a universal device breakpoint.

## 4. Adapt composition

Use:

- reflow
- stacking
- priority disclosure
- scrollable comparison with anchors
- alternate navigation
- master-detail transformation
- sheet or full-screen task takeover
- density adjustment

Do not reorder the visual layout in a way that breaks DOM, focus, or reading order without an equivalent semantic solution.

## 5. Adapt navigation and controls

Share destinations and task logic where possible. Adapt:

- tab bar, navigation rail, drawer, sidebar, breadcrumb, or command palette
- modal, sheet, popover, or full-screen presentation
- hover affordance versus explicit disclosure
- back and history behavior
- keyboard shortcut visibility

Parity means equivalent outcome, not identical chrome.

## 6. Handle content extremes

Test:

- 200% and higher zoom where applicable
- largest supported dynamic text
- long German-like labels
- compact CJK text with different line metrics
- Arabic/Hebrew bidirectionality and mixed numbers
- long names, addresses, currencies, dates, and units
- unbroken URLs, code, tables, charts, and user content
- zero, one, many, and maximum items

Use truncation only when full content remains available.

## 7. Localization and direction

- Use logical properties and semantic start/end.
- Mirror directional layout and controls where meaning changes.
- Do not mirror logos, media, charts, clocks, or culturally fixed symbols automatically.
- Preserve reading and focus order in bidirectional content.
- Avoid text embedded in images.
- Define locale-sensitive formatting and pluralization.

## 8. Native platform adaptation

For iOS and Android, verify current platform guidance and installed APIs. Adapt navigation, controls, permissions, back behavior, typography, materials, and system integrations rather than wrapping a web layout.

For adaptive systems, share tokens by semantic role and permit platform-specific component values.

## Output

Create an adaptation matrix:

| Region/behavior | Failure condition | Compact/narrow | Regular | Expanded/wide | Input/platform notes |
|---|---|---|---|---|---|

Also include:

- structural invariants
- content-extreme results
- localization/RTL decisions
- platform-specific differences
- unverified device conditions

## Checks

- Breakpoints arise from observed failure.
- Visual and semantic order agree.
- No essential hover-only path.
- Virtual keyboard and safe areas are handled.
- Dynamic text and zoom preserve the task.
- Platform differences are intentional.
