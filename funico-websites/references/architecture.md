# Funico Website Architecture

## Architecture Goal

Funico websites should be easy to grow from a focused site into a richer operational web application. Use a feature-oriented structure with shared layout, design tokens, and components.

Prefer clear composition over clever abstraction. Add abstractions only when they remove repeated layout or behavior that already exists in at least two places.

## Layers

Use these conceptual layers:

- App: entry point, routing, page registration, global configuration.
- Layout: shell, header, navigation, footer, page containers.
- Components: reusable interface elements such as buttons, tabs, metric cards, input groups, icon marks, and table primitives.
- Features: page-specific sections and workflows.
- Models: plain data structures used by pages and features.
- Services: integration or data-loading boundaries.
- Styles: shared tokens and style helpers.

## Page Composition

Build pages from sections. A page should read as a deliberate product surface, not a sequence of unrelated cards.

Recommended page shape:

1. Header or app shell with required icon treatment.
2. Primary page context: title, status, tabs, or short task summary.
3. Main work area: metrics, forms, data views, or content sections.
4. Supporting content: tables, details, secondary actions.
5. Footer only when it adds real value.

## Header Architecture

Create the header as a reusable system:

- `SiteIcon` or equivalent icon component.
- `BrandLockup` or equivalent icon + name composition.
- `PrimaryNavigation` for major areas.
- `UtilityNavigation` for secondary actions.
- `SiteHeader` or equivalent wrapper.

The exact names can change by project, but keep these responsibilities distinct.

## Design Tokens

Define shared tokens before styling individual pages:

- Colors.
- Typography.
- Spacing.
- Radii.
- Borders.
- Shadows.
- Component states.

Use tokens consistently. Avoid one-off values unless the local design truly needs them.

## Data and Content

Keep sample data separate from layout components. Components may receive data, but should not hard-code realistic business records unless the user asks for a static mockup.

For public websites, keep copy direct and practical. For operational apps, prioritize labels, values, and workflows over promotional text.

## JavaScript and Interactivity

Use the project's normal stack and keep interaction as simple as the task allows. Do not add a JavaScript framework or large client-side architecture unless the user explicitly asks or the requirement genuinely needs it.

## Quality Bar

Before finishing, check:

- Header and icon are visible, polished, and responsive.
- Color use follows the Funico palette.
- Layout is usable at desktop and mobile sizes.
- Components do not overlap.
- Example or generated code does not expose private implementation names.
