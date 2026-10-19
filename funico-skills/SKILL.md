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
- Keep the README's skill listing, readiness, and copyable usage prompt consistent with the skill. Follow its existing organization unless restructuring is part of the requested work.
- Respect explicit user requirements and project instructions. Base shared conventions on established patterns, and keep subject-specific requirements in the relevant skill.
- Keep changes scoped to the requested skill and its supporting resources and README entries. Suggest broader improvements separately unless they are within the task's scope.

## Verify the result

Check frontmatter, naming, reference links, and README consistency. Run an available skill validator when possible and verify any added scripts. In the handoff, identify the upstream guidance used, explain material deviations, and state what was verified and any validation limits.
