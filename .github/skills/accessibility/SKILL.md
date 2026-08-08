---
name: accessibility
description: Integrate accessibility into structure, content, interaction, visuals, motion, media, and testing while preventing unsupported conformance claims.
---

# Accessibility

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Accessibility is a design input, not a final checklist. Use this skill for new work, audits, design systems, high-risk flows, media, data visualization, and remediation.

Identify the applicable platform, jurisdiction, standard, version, conformance target, and organizational policy before asserting numeric requirements.

## 1. Build the access model

Identify:

- users, disabilities, temporary limitations, and situational constraints relevant to the task
- supported input and assistive technologies
- critical content and operations
- failure consequences
- platform and legal requirements

Do not reduce accessibility to screen readers or color contrast.

## 2. Structure and semantics

Specify:

- landmarks and page title
- heading hierarchy
- native element choice
- lists, tables, forms, and groups
- accessible names and descriptions
- relationships, status, and live regions
- language and direction

Use ARIA only when native semantics cannot express the behavior. Custom widgets inherit full keyboard, focus, state, and announcement responsibility.

## 3. Keyboard and focus

Verify:

- logical tab and reading order
- visible focus in every state and theme
- no keyboard trap
- skip and bypass paths
- roving focus or composite-widget behavior where appropriate
- initial focus and return for overlays
- shortcuts that do not conflict and can be discovered or remapped

Focus should follow user intent, not visual animation.

## 4. Visual access

Check:

- text, icon, component, focus, and chart contrast under the applicable criterion
- meaning independent of color
- zoom, reflow, spacing overrides, and large text
- forced colors/high contrast
- light, dark, disabled, hover, selected, invalid, and focus states
- text over media

Low-contrast secondary text is still content.

## 5. Motor and input access

- Apply current target-size guidance for the platform and criterion.
- Provide spacing and alternatives for small or precise targets.
- Do not require path-based gestures, multipoint gestures, dragging, hover, or device motion without an alternative.
- Support cancellation and reversal where possible.
- Avoid time limits or provide control and extension.

## 6. Cognitive and content access

- Use clear labels and instructions.
- Keep navigation and component behavior consistent.
- Explain requirements before errors occur.
- Make errors specific and blame-free.
- Reduce memory burden through visible context and sensible defaults.
- Let users review and correct consequential submissions.
- Avoid unnecessary motion, interruption, and choice overload.

Plain language depends on audience and domain; do not remove necessary precision.

## 7. Media and motion

Specify:

- alt text or decorative treatment
- captions, transcripts, and audio description where applicable
- pause/stop/hide controls
- autoplay policy
- reduced-motion and reduced-transparency behavior
- static equivalent when motion communicates order or causality

Canvas, WebGL, and charts need meaningful equivalent content and controls.

## 8. Forms, errors, and status

- Associate labels, instructions, requirements, errors, and descriptions.
- Announce status without stealing focus unnecessarily.
- Preserve input after recoverable failure.
- Provide error summary and field errors when scope warrants.
- Distinguish invalid, incomplete, unavailable, and system failure.

## 9. Test in layers

Use:

1. design inspection
2. automated analysis
3. keyboard and manual behavior review
4. zoom, reflow, contrast, reduced-motion, and forced-color review
5. representative screen reader and assistive-technology testing
6. testing with disabled users for consequential products

Automation is coverage assistance, not conformance.

## Output

Provide:

- applicable standard and scope
- critical user/task matrix
- requirements by structure, input, visual, content, media, and state
- findings with impact, evidence, and remediation
- test matrix and untested conditions
- conformance statement only when justified

Severity should combine task impact, affected users, frequency, and recovery—not visual prominence.

## Checks

- Essential content and tasks have equivalent access.
- Focus, names, states, and status are explicit.
- Color and motion are not sole carriers of meaning.
- Remediation fixes the cause rather than adding an ARIA label to a broken pattern.
- Claims distinguish tested, inferred, and unknown.
