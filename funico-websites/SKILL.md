---
name: funico-websites
description: Create new Funico websites using the Funico visual direction, required website icon treatment, project architecture, and abstract Swift-style component conventions. Use when starting, scaffolding, or substantially redesigning a Funico website or web application.
---

# Funico Websites

Use this skill when creating or substantially redesigning a Funico website or web application.

The result should feel calm, precise, operational, and carefully branded. Prefer a real usable website or application screen over a generic landing page unless the user explicitly asks for a marketing page.

## Required Reading

Read only the references that are relevant to the current task:

- For visual direction, colors, header rules, and icon placement, read [references/design-system.md](references/design-system.md).
- For application and page architecture, read [references/architecture.md](references/architecture.md).
- For folder layout and naming conventions, read [references/project-structure.md](references/project-structure.md).
- For acceptable abstract example style, inspect files in [examples](examples).

## Core Requirements

All new Funico websites must:

- Build the design around `#006387` as the base tint.
- Use `#AABCC6` as the secondary tint.
- Include a required website icon as a prominent, polished part of the header or first viewport.
- Improve on the provided reference header: the header must feel intentional, balanced, and branded rather than a plain utility strip.
- Preserve the reference's calm operational feel: light workspace, clear panels, restrained borders, compact navigation, strong information hierarchy.
- Avoid generic template aesthetics, oversized marketing composition, decorative blobs, heavy gradients, and excessive card nesting.
- Keep example code abstract. Examples may show declarative component API style, but must not mention real Funico repositories, package names, internal APIs, or actual implementation details.

## Working Rules

When starting a new Funico website:

1. Decide whether the request is a public website, operational web app, dashboard, or hybrid.
2. Read the relevant references.
3. Create the project structure before filling in pages.
4. Define shared design tokens for color, typography, spacing, radius, borders, and component states.
5. Create a header system with a required website icon treatment before building page-specific sections.
6. Implement pages using reusable layout and component primitives.
7. Verify the result at desktop and mobile sizes.
8. Report any intentional deviations from this skill.

## Priority

The user's explicit request always wins. When a request conflicts with this skill, keep the deviation small and explain it briefly.
