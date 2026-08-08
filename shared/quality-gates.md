# Open Design Agent Quality Gates

Run the gates relevant to the artifact. A failed safety, accessibility, truth, or core-task gate blocks “done.”

## Product and content

- The primary user and outcome are explicit.
- The first reading path and primary action are unambiguous.
- Content is real, supplied, or labeled synthetic.
- Claims, prices, metrics, names, and social proof are not invented.
- Destructive, financial, health, privacy, and irreversible actions expose consequences.
- Empty and error states help the user continue.

## Information architecture

- Navigation reflects the content model and task frequency.
- Labels use user language and remain distinct.
- Search, browse, filter, sort, and recovery are designed as one system where applicable.
- No critical path depends on an undiscoverable gesture or hover.
- Deep links, back behavior, and return position are coherent.

## Interaction and state

- Valid states, events, transitions, guards, and side effects are explicit.
- Every state has a way forward, back, retry, cancel, or safe exit.
- Loading representations are honest and preserve orientation.
- Errors identify the source, preserve recoverable work, and offer a next step.
- Confirmation persistence matches consequence and duration.
- Streaming and live updates preserve user control and scroll position.

## Visual system

- Hierarchy survives a squint test and does not rely on color alone.
- Typography roles, line length, line height, and data numerals fit the content.
- Spacing and alignment reveal grouping before containers are added.
- Color roles are semantic; brand and status meanings do not collide.
- Radius, border, depth, imagery, and icon treatments form one intentional world.
- Repeated cards, pills, gradients, labels, and effects have a product reason.
- The result is not an imitation of a reference brand.

## Responsive and platform

- Layout changes occur where content or interaction fails.
- Reading order remains correct after reflow.
- Keyboard, pointer, touch, and assistive inputs have equivalent paths.
- Safe areas, virtual keyboards, dynamic text, orientation, and viewport height are handled where relevant.
- Localization, language expansion, bidirectionality, dates, numbers, and names are considered.
- Dense expert surfaces and narrow consumer surfaces are not forced into one composition.

## Accessibility

- Semantic structure and accessible names are present.
- Focus order, focus visibility, target acquisition, and keyboard operation are coherent.
- Contrast is checked against the current applicable requirement.
- Status and errors are announced appropriately.
- Zoom, reflow, high contrast, reduced motion, and dynamic type preserve content and tasks.
- Media has meaningful alternatives; decorative media is hidden appropriately.
- No conformance claim is made without the required audit evidence.

## Performance and resilience

- The primary content does not wait on decorative media.
- Motion suspends when hidden or offscreen where practical.
- Large assets, fonts, effects, and client code have explicit value.
- Layout stability and perceived response are protected.
- Slow, offline, failed, and partial responses have designed outcomes.

## System and delivery

- Components use semantic tokens and documented variants.
- Local exceptions are intentional and discoverable.
- Component anatomy, properties, states, content rules, and accessibility are documented.
- Handoff includes responsive behavior, state behavior, assets, and acceptance criteria.
- Implementation QA compares behavior and content, not only pixels.
- Durable changes update the design-system truth.

## Final disposition

- **Rebuild:** the direction, task model, topology, or accessibility foundation is wrong.
- **Fix:** the foundation holds but material defects remain.
- **Ship:** all applicable gates pass and remaining uncertainty is explicitly accepted.
