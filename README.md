# Open Design Agent

Open Design Agent is a source-first UI/UX design system for AI-assisted product work. It combines one orchestrating agent with composable domain skills, shared quality contracts, and scenario profiles.

It is not a visual template library. It reasons from the user's task, content, audience, platform, evidence, and existing product before choosing a visual or interaction direction.

## Architecture

```text
open-design-agent/
|-- .github/
|   |-- agents/
|   |   |-- open-design-agent.agent.md
|   |   |-- design-researcher.agent.md
|   |   |-- design-critic.agent.md
|   |   `-- design-system-steward.agent.md
|   `-- skills/
|       |-- design-direction/
|       |-- ui-foundations/
|       |-- art-direction/
|       |-- content-design/
|       |-- ux-architecture/
|       |-- interaction-design/
|       |-- responsive-platform/
|       |-- accessibility/
|       |-- design-systems/
|       |-- research-insights/
|       |-- prototyping-validation/
|       |-- critique/
|       `-- delivery-governance/
|-- shared/
|   |-- operating-contract.md
|   |-- evidence-and-numbers.md
|   `-- quality-gates.md
|-- profiles/
|   |-- surfaces.md
|   |-- platforms.md
|   `-- scenarios.md
`-- LICENSE
```

## How the parts compose

1. The agent classifies the work and loads the shared contract.
2. A **surface profile** defines what success means: Persuade, Operate, Read, or Experience.
3. A **platform profile** supplies web, iOS, Android, or adaptive constraints.
4. One or more **scenario profiles** add domain-specific risks.
5. Only the domain skills needed for the task are activated.
6. Quality gates run across the combined result.

Specialized agents provide isolated contexts:

- `open-design-agent`: primary orchestrator and implementation partner
- `design-researcher`: read-only evidence and study specialist
- `design-critic`: read-only independent finishing review
- `design-system-steward`: token, component, migration, and governance specialist

Typical routes:

| Request | Skills |
|---|---|
| New marketing page | design-direction, art-direction, ui-foundations, responsive-platform, accessibility, critique |
| Product workflow | ux-architecture, interaction-design, ui-foundations, accessibility, prototyping-validation |
| Content, onboarding, or error language | content-design plus ux-architecture or interaction-design as needed |
| Design system | design-systems, ui-foundations, interaction-design, responsive-platform, accessibility, delivery-governance |
| UX research | research-insights, ux-architecture, prototyping-validation |
| Existing UI audit | critique plus the domain skills implicated by findings |
| Implementation handoff | delivery-governance plus interaction-design and design-systems as needed |

## Use with GitHub Copilot CLI

Use `open-design-agent` as the working directory, or copy its `.github`, `shared`, and `profiles` directories together into a project root so relative references remain valid.

- Run `/skills` to inspect the 13 project skills.
- Run `/agent open-design-agent` for the main orchestrator.
- Select `design-researcher`, `design-critic`, or `design-system-steward` for isolated specialist work.

Skills are stored in Copilot's native project discovery path: `.github/skills/<name>/SKILL.md`.

## Design guarantees

Open Design Agent must:

- distinguish facts, assumptions, hypotheses, and preferences
- classify surface mode and platform separately
- preserve existing product truth unless change is intentional
- design responsive behavior and states, not only ideal screenshots
- treat accessibility, semantics, and recovery as design inputs
- use real content or clearly labeled placeholders
- expose the authority and scope of numeric rules
- generate materially different directions when exploration is valuable
- reject brand imitation and unlicensed asset reuse
- report what was not validated

## License

Open Design Agent is released under the MIT License. See [LICENSE](LICENSE).
