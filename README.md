# Funico Skills

A growing collection of reusable skills for working on Funico projects.

This repository brings together the conventions, workflows, and practical knowledge that guide our work. Each skill captures a specific area of expertise in a format an AI coding assistant can follow, helping turn shared knowledge into consistent results across projects.

## What is a skill?

A skill is a focused set of instructions for a particular type of task. Its `SKILL.md` explains when to use it, how to approach the work, and which requirements to follow. Supporting files can provide references, examples, assets, or scripts when needed.

Skills can cover different subjects, from design and development to documentation, project setup, and recurring workflows. This collection will expand as new needs and practices emerge.

## Available skills

| Skill | Purpose | Status |
| --- | --- | --- |
| [Funico Architecture](funico-archtecture/SKILL.md) | Apply the Swift architecture and naming conventions from NVMNovem/skills to Funico application code. | ![Ready to use](https://img.shields.io/badge/status-ready%20to%20use-2ea44f) |
| [Funico Mailings](funico-mailings/SKILL.md) | Reserved for guidance on Funico mailings. The workflow has not been documented yet. | ![Not ready](https://img.shields.io/badge/status-not%20ready-d97706) |
| [Funico README](funico-readme/SKILL.md) | Create or revise practical, repository-grounded README files for Funico software projects. | ![Ready to use](https://img.shields.io/badge/status-ready%20to%20use-2ea44f) |
| [Funico Skills](funico-skills/SKILL.md) | Create or update reusable Funico skills using guidance from NVMNovem/skills, including references and README usage prompts. | ![Not ready](https://img.shields.io/badge/status-not%20ready-d97706) |
| [Funico Websites](funico-websites/SKILL.md) | Create or redesign Funico websites and web applications with shared visual guidelines, architecture, and project structure. | ![Ready to use](https://img.shields.io/badge/status-ready%20to%20use-2ea44f) |

## Usage

Choose a skill below and copy its prompt into your AI assistant. Replace the bracketed task with your desired outcome, project context, and any specific constraints. Each skill has its own heading so you can link directly to its usage section on GitHub.

### Architecture

Use this prompt when writing or reviewing Swift application code with the Novem architecture and naming conventions used by Funico.

```text
Read and follow the Funico Architecture skill:
https://github.com/Funico-NV/skills/blob/main/funico-archtecture/SKILL.md

Also read the linked Novem Architecture skill and the reference files relevant to the task, resolving their paths relative to the owning skill's folder on GitHub. Apply the Swift architecture and naming conventions to the code you write or review, preserving Funico names and persisted identifiers. Ask for clarification when conflicting project patterns leave the intended convention unclear.

Task: [Describe what to build, change, or review in this project.]
```

### Mailings

This skill is a placeholder and is not ready for use. Use this prompt to document its workflow before applying it to mailing tasks.

```text
Inspect the Funico Mailings skill placeholder:
https://github.com/Funico-NV/skills/blob/main/funico-mailings/SKILL.md

Create useful skill instructions from the supplied Funico mailing requirements and established project examples. Link any supporting references from the skill, and keep its README listing and usage prompt in sync. Identify missing requirements rather than inventing mailing conventions.

Task: [Describe the mailing workflow and conventions this skill should capture.]
```

### README

Use this prompt when creating or updating a project's README with Funico's practical documentation style.

```text
Read and follow the Funico README skill:
https://github.com/Funico-NV/skills/blob/main/funico-readme/SKILL.md

Also read the linked reference files relevant to the task, resolving their paths relative to the skill's folder on GitHub. Ground the README in the repository's actual setup and usage, and preserve correct existing content.

Task: [Describe the project and what to create or update in its README.]
```

### Skills

This skill refers to starter guidance and is not ready for general use yet. Use this prompt to try it when creating or updating a skill in this repository.

```text
Read and follow the Funico Skills skill:
https://github.com/Funico-NV/skills/blob/main/funico-skills/SKILL.md

Also read the linked Novem Skills skill and the reference files relevant to the task, resolving their paths relative to the owning skill's folder on GitHub. Apply the guidance using Funico naming and repository links, and keep the README listing and alphabetical Usage sections in sync.

Task: [Describe the skill to create or update and the conventions it should capture.]
```

### Websites

Use this prompt when creating or substantially redesigning a Funico website or web application.

```text
Read and follow the Funico Websites skill:
https://github.com/Funico-NV/skills/blob/main/funico-websites/SKILL.md

Also read the linked reference files and examples relevant to the task, resolving their paths relative to the skill's folder on GitHub. Apply the Funico visual guidelines, website icon treatment, architecture, and project structure. Verify the result at desktop and mobile sizes.

Task: [Describe the website or application to create or redesign and its constraints.]
```

## Repository structure

Each skill lives in its own folder at the repository root:

```text
skills/
|-- README.md
`-- <skill-name>/
    |-- SKILL.md
    |-- references/    # Optional supporting documentation
    |-- examples/      # Optional examples
    |-- assets/        # Optional files used by the skill
    `-- scripts/       # Optional helper scripts
```

## Adding a skill

Create a folder with a descriptive name and add a `SKILL.md` that clearly states the skill's purpose, when it applies, and the steps or standards to follow. Keep the main instructions focused and place detailed supporting material in the appropriate subfolders.

Add the skill to the table above and give it a subsection under Usage with a copyable prompt that links to its `SKILL.md` on GitHub. Keep instructions actionable, examples relevant, and references up to date as the collection grows.
