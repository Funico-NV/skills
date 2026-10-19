---
name: funico-archtecture
description: Apply the Swift architecture and naming conventions from NVMNovem/skills to Funico application code. Use when structuring, writing, refactoring, or reviewing Swift application code for Funico.
---

# Funico Architecture

Use [NVMNovem/skills](https://github.com/NVMNovem/skills) as the architecture reference for Funico Swift application work.

## Read the upstream guidance

Before making architecture decisions, read the current [Novem Architecture skill](https://github.com/NVMNovem/skills/blob/main/novem-architecture/SKILL.md). If raw Markdown is needed, use [the raw skill file](https://raw.githubusercontent.com/NVMNovem/skills/main/novem-architecture/SKILL.md).

Read only the supporting references relevant to the task. Resolve their relative links from the upstream `novem-architecture/` folder, keeping the same branch or revision as the skill file. The references cover state and dependencies, view modifiers, model extensions, settings, navigation, localization, and content builders.

Keep the upstream guidance as the maintained source of architecture conventions rather than copying it into this skill. If it cannot be accessed, report the limitation and use available project evidence without claiming upstream compliance.

## Apply it to Funico

Inspect the project's instructions, module layout, and representative code before applying the upstream conventions. Follow its guidance for folder structure, naming, and the responsibilities being changed.

- Preserve the project's existing Funico names and prefixes; upstream example identifiers are illustrative.
- Preserve persisted identifiers and settings keys when applying naming changes.
- Respect explicit user requirements and project instructions. When conflicting project patterns leave the intended architecture unclear, clarify the specific decision before establishing a new rule.
- Keep changes scoped to the requested work; applying this skill does not call for an unrelated architecture migration.

## Verify the result

Run the project's relevant build or checks when code changes warrant them. In the handoff, identify the upstream guidance used, explain material deviations, and state what was verified.
