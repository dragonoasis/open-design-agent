---
name: ui-foundations
description: Design coherent visual hierarchy, composition, layout, typography, color, spacing, imagery, iconography, and data presentation for interfaces and content surfaces.
---

# UI Foundations

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use after the task and direction are understood. This skill turns structure and content into a coherent visual system without imposing one visual style.

## Inputs

- direction contract or existing design system
- surface and platform profiles
- content hierarchy and real content samples
- state and responsive requirements
- brand assets and accessibility constraints

## Workflow

### 1. Establish reading order

Identify:

- first fixation and first meaningful statement
- primary action or decision
- secondary scan path
- supporting detail available on demand
- terminal or next-step region

Use size, weight, contrast, spacing, position, and density in combination. Do not make every section begin with an oversized heading or every action visually primary.

Check hierarchy in grayscale, at a distance, and with content replaced by blocks. Then restore semantic color and verify meaning.

### 2. Build composition from content

Choose the layout behavior from:

- narrative sequence
- comparison
- browse and filter
- monitor and respond
- edit and inspect
- read and reference
- spatial exploration

Define columns, margins, gutters, alignment anchors, max measures, and intentional breaks as relationships. Use proximity before borders and containers.

Avoid:

- equal-card grids when content importance differs
- nested panels without a grouping reason
- symmetry that hides priority
- arbitrary off-grid placement labeled as creativity

### 3. Define spacing roles

Create a compact scale, then map semantic roles:

- inline
- control internal
- related-item
- group
- section
- region

Optical adjustment is allowed when documented. Do not force every value onto a scale if the result is visibly wrong, and do not call arbitrary values “optical.”

### 4. Assign typography by job

Define:

- display or campaign role
- page and section hierarchy
- interface labels and controls
- reading body
- metadata and captions
- code or technical notation
- tabular and financial numerals

Tune size, weight, width, tracking, line height, and measure together. Test:

- long and short labels
- mixed case and all-caps use
- numbers, symbols, code, and units
- multilingual scripts and fallback fonts
- zoom and dynamic text

Do not use a display face for dense controls merely to preserve branding.

### 5. Build semantic color

Separate:

- background and surface roles
- text and icon hierarchy
- border and focus roles
- primary and secondary action
- interactive accent
- success, warning, error, and information
- data-series roles
- brand-only or campaign-only domains

Map light, dark, and high-contrast themes by role rather than inversion. Verify contrast under the current applicable standard and state.

Never let brand green double automatically as success, or brand red as error.

### 6. Define geometry and depth

Use radius, border, surface contrast, shadow, overlap, blur, and texture intentionally.

Choose a depth model:

- flat and ruled
- surface contrast
- restrained elevation
- layered material
- atmospheric

Depth must express grouping, interaction, or world—not decorate every card. Limit radius tiers and explain pill usage by behavior.

### 7. Direct imagery and icons

For imagery:

- choose documentary, product, editorial, illustrative, technical, or atmospheric roles
- define crop, aspect, focal point, grading, caption, and fallback
- protect text readability without muddy overlays
- provide meaningful alternatives

For icons:

- define stroke/fill logic, grid, optical size, and naming
- pair unfamiliar icons with labels
- keep decorative icons out of the accessibility tree
- never use emoji or arbitrary glyphs as system icons without intent

### 8. Design data visualization by question

State the analytical task:

- compare
- rank
- trend
- distribute
- relate
- compose
- locate

Then select a chart. Include:

- title and takeaway context
- units, source, freshness, and denominator
- labels or accessible data alternative
- color-independent encoding
- empty, partial, loading, and error states

Do not add charts merely to make a dashboard appear analytical.

## Output

Provide:

- composition and reading-order specification
- typography role table
- semantic color roles
- spacing and geometry rules
- depth/material rule
- imagery and icon direction
- data-visualization rules where relevant
- responsive implications
- content-extreme examples

## Checks

- Hierarchy reflects importance, not component size defaults.
- Grouping is visible without excessive containers.
- Typography remains readable in the target language and platform.
- Color meaning is semantic and redundant.
- Geometry and depth form one world.
- Real content still fits.
- The surface is distinct without resembling a reference brand.
