# Evidence and Numeric Authority

## Evidence ladder

Use the strongest relevant evidence available:

1. current standards, safety constraints, and legal requirements
2. verified product behavior, user data, and outcome research
3. platform human-interface guidance and technical contracts
4. implemented design-system behavior and component tests
5. directly observed interfaces and content
6. expert guidance and established methods
7. inferred patterns and award recognition
8. stylistic preference

Lower levels can inspire a direction. They cannot silently overrule higher levels.

## Evidence record

For a material decision, capture:

| Field | Meaning |
|---|---|
| Claim | The proposed rule or conclusion |
| Evidence | Source, product artifact, observation, or test |
| Evidence type | measured, observed, implemented, documented, inferred, preferred |
| Scope | mode, platform, audience, scenario, content |
| Counterexample | Where the claim fails or changes |
| Confidence | high, medium, low |
| Validation need | what would raise confidence |

File counts, popularity, awards, stars, and repeated wording are discovery signals, not outcome evidence.

## Numeric classes

Classify every number:

- **Standard constraint:** tied to a current named standard and criterion.
- **External production constraint:** supplied by a current platform, publisher, printer, or device contract.
- **Platform baseline:** a convention that still requires current verification.
- **System default:** inherited from the product's selected toolkit.
- **Research-planning heuristic:** useful for planning but not statistical proof.
- **Design heuristic:** a starting range that must be tested in context.
- **Style parameter:** intentionally creates a visual world.
- **Measured product value:** observed in the current product or research.

Record:

```text
value:
unit:
class:
source_or_rationale:
platform:
conditions:
confidence:
last_verified:
```

## Common traps

- A contrast ratio is meaningless without the applicable criterion and element.
- A touch-target number is not universal across platforms and input modes.
- A breakpoint is not a device truth.
- A motion duration does not prove perceived speed or comfort.
- A participant count does not prove saturation or representativeness.
- A spacing base does not dictate every component gap.
- An award score is not an accessibility audit.

When authority is uncertain, state the number as a hypothesis or remove it.
