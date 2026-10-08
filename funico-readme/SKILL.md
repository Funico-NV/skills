---
name: funico-readme
description: Create or revise README.md files for Funico software projects. Use when documenting a repository, package, service, library, or app, or when aligning an existing README with Funico's practical documentation style.
---

# Funico README

Create a README that helps a new contributor or consumer understand the project and complete its ordinary first task without guessing. Keep it factual, compact, and grounded in the repository.

## Establish what is true

Before writing, inspect the relevant source, manifests, configuration examples, scripts, tests, and existing documentation. Treat implemented behavior as the source of truth. Preserve useful, correct material already in the README and resolve contradictions rather than repeating them.

Identify:

- what the project is and who uses it;
- its main products, components, or responsibilities;
- the supported setup and normal usage path;
- important constraints, security boundaries, compatibility requirements, and known limitations;
- commands and examples that can be verified locally.

Do not invent setup steps, environment variables, endpoints, version numbers, support claims, or links. When a detail cannot be verified, omit it or label it clearly as unverified.

## Shape the README around the reader

Put a basic description near the top. In one short paragraph, say what the project provides, who or what consumes it, and the boundary that distinguishes it from adjacent projects.

Include only sections that help this project. Typical priorities are:

1. project description and status or compatibility information;
2. installation or dependency setup;
3. the smallest useful example;
4. products, key concepts, or architecture when readers must choose among them;
5. configuration and normal operating commands;
6. known limitations, security considerations, migration notes, or troubleshooting when they affect real use;
7. testing and contribution guidance when this repository supports contributors.

Do not add empty boilerplate sections. For a new README or a substantial restructure, read [references/patterns.md](references/patterns.md) and adapt its patterns rather than copying every heading.

## Include useful code examples

Every README needs at least one fenced example showing the ordinary path: the first useful thing a reader should type or integrate. Prefer complete, copyable examples over fragments that hide essential context.

- Use the correct language identifier on every code fence.
- Introduce the purpose of an example before the block and explain non-obvious choices after it.
- Keep examples short enough to scan, but include required imports, setup, and error handling when omitting them would mislead.
- Use realistic placeholders and never include real credentials, tokens, private hosts, or customer data.
- When the project exposes several independently consumed products, give each product a basic example unless the repository's own instructions define a different standard.
- Test examples against the current API whenever practical. Run the relevant compiler, test, formatter, documentation checker, or command. If an example cannot be executed in the available environment, say so in the handoff instead of claiming it works.

Examples should demonstrate supported behavior, not merely show type names. Prefer the stable public interface and the simplest production-appropriate path.

## Use the Funico writing style

- Write direct, specific prose without marketing language.
- Explain important design decisions in terms of their consequence for the reader.
- Use short descriptive headings and compact paragraphs.
- Put identifiers, commands, paths, configuration keys, routes, and literal values in backticks.
- Use tables for genuine comparisons or mappings, not decoration.
- Use bullets for parallel facts and numbered lists for ordered work.
- Use GitHub admonitions sparingly: `NOTE` for context, `TIP` for an actionable shortcut or workaround, and `WARNING` for a meaningful risk.
- Put lengthy implementation evidence, queries, payloads, or diagnostics in a `<details>` block when readers need access but not immediate visibility.
- State limitations plainly: describe the boundary, when it matters, the observable effect, and the workaround if one exists.

Match established repository conventions for heading capitalization, line wrapping, badges, and link style. Repository instructions take precedence over this skill.

## Finish carefully

Check the final README against the code and remove stale claims. Verify internal links, commands, examples, product names, and versions. Keep unrelated README content intact unless the user asked for a broader rewrite.

Summarize what was documented and report which examples or commands were actually verified.
