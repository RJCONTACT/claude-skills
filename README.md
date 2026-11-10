# Design system migration — Claude skill

A Claude skill that moves a legacy Figma design system onto a base kit such as Untitled UI **without changing what users see**, adds a second product look as a variable mode, and proves the result by rebuilding real screens next to their sources.

**Get it:** the skill is sold as a bundle with the Figma agent version. Details and the buy link are on my [Tools page](https://rishik-jha.rishikrkjha.workers.dev/tools). How it was built: [case study](https://rishik-jha.rishikrkjha.workers.dev/case-study/design-system-migration).

## What it does

1. **Audit** the old system: styles, variables, components, icons, hard-coded values on real screens.
2. **Foundations**: the old values become variables; the kit's scales and semantic tokens point at them.
3. **Components**: base components restyled first so every variant inherits; new components where the kit has no match.
4. **Theme modes**: a second product as a variable mode plus number variables for size differences, with the default look unchanged.
5. **Validation screens**: inventory, rebuild from library instances only, compare by eye and by layer values, fix the library.
6. **Coverage tests**: more screens chosen for untested components, until every component type passes.
7. **Hand-off**: decisions, tokens, remaining differences and version checkpoints written up.

It includes a strict pass rule (colours exact, sizes and spacing within 1px, same weight, same icon and position) and the Figma limits found along the way, with workarounds.

## Works with

Claude and Claude Code, driving Figma through the Figma Desktop Bridge (figma-console MCP server).

## Also available

The same workflow as five slash commands for Figma's design agent: [figma-skills](https://github.com/RJCONTACT/figma-skills).

© 2026 Rishik Jha. The skill files are not in this repository.
