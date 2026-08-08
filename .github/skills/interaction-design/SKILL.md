---
name: interaction-design
description: Specify state machines, transitions, feedback, loading, errors, motion, gestures, streaming, interruption, and recovery for components and product flows.
---

# Interaction Design

Follow the [operating contract](../../../shared/operating-contract.md), [evidence policy](../../../shared/evidence-and-numbers.md), and [quality gates](../../../shared/quality-gates.md).

Use whenever behavior changes over time or in response to input. A static mockup is not a complete interaction specification.

## 1. Model the state

For each component or flow, list:

- stable states
- transient states
- events
- guards
- transitions
- entry/exit actions
- side effects
- persistence
- cancellation and interruption

Separate independent concerns. Network state, validation state, selection state, and permission state should not become one impossible enum.

Use a table:

| Current state | Event | Guard | Next state | Feedback | Side effect | Recovery |
|---|---|---|---|---|---|---|

Every state needs an exit, retry, undo, cancel, or safe terminal outcome.

## 2. Map state to interface

Specify:

- visible content and controls
- enabled and disabled actions
- focus target and return
- accessible name, description, and announcement
- progress or status persistence
- responsive/platform variation

Do not hide a valid state because it is rare.

## 3. Feedback by consequence

Choose:

- local inline feedback for field or component scope
- persistent page/panel status for durable conditions
- transient confirmation for low-risk completed actions
- modal interruption only when immediate decision is necessary
- system notification for background completion when appropriate

Match prominence and persistence to consequence. Do not use a toast for a critical failure, unresolved permission, or information the user must act on later.

## 4. Loading and progress

Distinguish:

- immediate acknowledgment
- determinate progress
- indeterminate wait
- streaming or incremental content
- background operation
- stale or cached content
- partial success

Preserve layout and orientation. Skeletons should approximate real content and must not imply data that may never exist. Never fake a progress percentage.

Allow cancellation when the operation is long, expensive, or no longer useful.

## 5. Error and recovery

For every error:

- identify whether user, system, permission, data, network, conflict, or policy caused it
- own system failures in the copy
- state what happened without exposing irrelevant internals
- preserve recoverable input and context
- give one specific next step
- provide escalation or support when self-recovery is impossible

Design retry idempotency and duplicate-submission prevention.

## 6. Motion

Every animation must answer:

- what changed?
- what caused it?
- where did it come from or go?
- what needs attention?
- what can be interrupted?

Specify:

- trigger
- property
- duration or physical behavior
- easing
- sequencing
- interruption
- performance tier
- reduced/no-motion equivalent

Prefer transform and opacity where suitable, but do not animate merely because it is cheap. Reduced motion must preserve content, order, and causality.

## 7. Gestures and target acquisition

- Use visible controls for essential actions.
- Provide alternatives to swipe, drag, hover, long press, and device motion.
- Make drag start, valid drop, invalid drop, cancel, and keyboard movement visible.
- Separate dangerous adjacent targets and confirm proportional to risk.
- Apply current platform target guidance; do not treat one pixel value as universal.

## 8. Overlays and focus

For dialogs, sheets, menus, popovers, and tooltips, define:

- trigger and accessible relationship
- initial focus
- tab/focus containment where applicable
- escape, outside press, back, and close rules
- focus return
- scroll locking
- nested overlay behavior
- mobile substitution

A tooltip cannot contain essential or interactive content that has no other path.

## 9. Streaming, chat, and live updates

Specify:

- message/event types
- pending, streaming, complete, interrupted, retrying, and failed states
- attachment upload and processing
- user scroll interruption and jump-to-latest
- editing, regeneration, cancellation, and provenance
- rate limits, tool activity, and delayed background completion

Do not force-scroll a user who moved away from the latest content. Repeated content used for animation must not repeat for assistive technology.

## Output

- state inventory
- transition table or diagram
- feedback and recovery specification
- focus and announcement behavior
- motion and reduced-motion specification
- input/gesture alternatives
- edge-case acceptance criteria

## Checks

- No impossible or dead-end states.
- Pending actions cannot be submitted twice unintentionally.
- Failure preserves work where safe.
- Focus and announcements follow state.
- Motion is meaningful and interruptible.
- Essential behavior has keyboard/touch/assistive parity.
