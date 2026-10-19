---
name: funico-skills
description: Create or update reusable skills in the Funico skills repository using the guidance from NVMNovem/skills, including supporting references and README usage prompts.
---

# Funico Skills

Use [NVMNovem/skills](https://github.com/NVMNovem/skills) as the reference for creating and maintaining reusable Funico skills.

## Read the upstream guidance

Before creating or updating a skill, read the current [Novem Skills skill](https://github.com/NVMNovem/skills/blob/main/novem-skills/SKILL.md). If raw Markdown is needed, use [the raw skill file](https://raw.githubusercontent.com/NVMNovem/skills/main/novem-skills/SKILL.md).

Read only the supporting references relevant to the task. Resolve any relative links from the upstream `novem-skills/` folder, keeping the same branch or revision as the skill file.

Keep the upstream guidance as the maintained source of skill-authoring conventions rather than copying it into this skill. If it cannot be accessed, report the limitation and use available project evidence without claiming upstream compliance. The upstream skill currently describes itself as a starter; do not imply that it provides a complete standard.

## Apply it to Funico

Read this repository's README, the skill being changed, and nearby skills before applying the upstream conventions.

- Create skills in root-level `funico-<subject>/` folders, with a `SKILL.md` whose frontmatter name matches its folder.
- Use Funico headings, names, and examples instead of copying Novem branding. Preserve existing skill names unless a rename is requested.
- Use this repository's GitHub URL, `https://github.com/Funico-NV/skills`, when adapting upstream README usage links.
- Respect explicit user requirements and project instructions. Base shared conventions on established patterns, and keep subject-specific requirements in the relevant skill.
- Keep changes scoped to the requested skill and its supporting resources and README entries. Suggest broader improvements separately unless they are within the task's scope.

## Keep the repository README in sync

Apply the upstream section of this name to the root `README.md` in [Funico-NV/skills](https://github.com/Funico-NV/skills). Repository maintenance instructions from the upstream skill target this Funico repository; `NVMNovem/skills` remains the reference source.

- Add or update the skill's entry in the Available skills table using a relative link to its `SKILL.md`, a purpose matching its description, and a status badge. Use the existing Not ready badge for a new starter, and preserve existing readiness unless changing it is part of the task.
- Give the skill a subsection under Usage, keeping the subsection headings alphabetical. Include a brief explanation and a fenced `text` block containing a copyable prompt ending with a bracketed task placeholder.
- Link usage prompts to `https://github.com/Funico-NV/skills/blob/main/<skill-folder>/SKILL.md`, using the actual Funico folder name. Ask the assistant to read relevant linked references relative to the folder that owns them. Keep Novem links where they identify upstream guidance.
- Check that the Funico README's listing, readiness, and usage prompt agree with the skill being changed.

## Verify the result

Check frontmatter, naming, reference links, and README consistency. Run an available skill validator when possible and verify any added scripts. In the handoff, identify the upstream guidance used, explain material deviations, and state what was verified and any validation limits.
