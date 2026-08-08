# Platform Profiles

Platform and surface mode are independent.

## Web

Design for:

- semantic HTML and native behavior first
- fluid viewport and content-driven reflow
- keyboard, pointer, touch, zoom, and browser navigation
- URL state, deep links, history, refresh, and progressive loading
- reduced motion, forced colors, and user font/contrast preferences
- variable network, CPU, memory, and input capability

Do not make hover the only path. Do not infer a device from viewport width alone.

## iOS

Design with current Apple guidance and installed platform behavior:

- safe areas, Dynamic Type, VoiceOver, Reduce Motion, Increase Contrast
- navigation stacks, tabs, sheets, toolbars, alerts, and system gestures
- semantic colors, materials, SF Symbols where appropriate
- keyboard avoidance, orientation, and one-handed reach
- interruption, permission, background, and restoration states

Do not transplant web navigation or Android control behavior into an iOS shell.

## Android

Design with current Android and Material guidance:

- system bars, insets, predictive back, dynamic type, TalkBack
- navigation bars/rails/drawers selected by window class and task model
- app bars, sheets, dialogs, snackbars, and system permissions
- dynamic color only when brand and contrast survive
- foldables, resizable windows, keyboards, and diverse hardware

Do not assume one handset size or make snackbars carry durable critical information.

## Adaptive cross-platform

Share:

- information architecture
- content model
- semantic tokens
- state machine and business rules
- accessibility intent
- analytics and outcome definitions

Adapt:

- navigation shell
- control anatomy
- gestures and back behavior
- typography metrics
- spacing and target conventions
- modal/sheet behavior
- permissions and system integrations

Parity means equivalent capability and understanding, not pixel identity.

## Platform-agnostic artifacts

Flows, research plans, service blueprints, content models, and token schemas may be platform-agnostic. Mark the decisions that must be resolved before implementation.
