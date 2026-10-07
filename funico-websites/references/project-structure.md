# Funico Project Structure

Use this structure as a starting point for new Funico websites. Adapt names to the host framework or language while preserving responsibilities.

```text
funico-website/
|-- README.md
|-- Package or project manifest
|-- Sources/
|   `-- Website/
|       |-- App/
|       |   |-- Website
|       |   `-- Routes
|       |-- Layout/
|       |   |-- SiteHeader
|       |   |-- BrandLockup
|       |   |-- PrimaryNavigation
|       |   |-- PageShell
|       |   `-- Footer
|       |-- Components/
|       |   |-- SiteIcon
|       |   |-- Button
|       |   |-- Tabs
|       |   |-- MetricCard
|       |   |-- Panel
|       |   |-- FormField
|       |   `-- DataTable
|       |-- Features/
|       |   |-- Home/
|       |   |-- Dashboard/
|       |   `-- Shared/
|       |-- Models/
|       |-- Services/
|       `-- Styles/
|           |-- Colors
|           |-- Typography
|           |-- Spacing
|           |-- Components
|           `-- Responsive
|-- Public/
|   |-- favicon
|   |-- app-icon
|   `-- social-preview
`-- Tests/
```

## Required Areas

Every new project should include:

- A dedicated place for the website icon and favicon assets.
- Shared style tokens.
- A reusable site header.
- Shared layout primitives.
- Feature folders for page-specific code.

## Naming

Use clear names that describe responsibility:

- Prefer `SiteHeader` over `Header` when multiple header-like components may exist.
- Prefer `SiteIcon` over `Logo` when the project has not yet defined a full logo system.
- Prefer `BrandLockup` for icon + name + optional descriptor.
- Prefer `MetricCard`, `DataTable`, and `Panel` for operational UI.

## Examples

Example files in this skill are intentionally abstract. They show component shape and design intent only. Do not copy their API names as if they were real project dependencies.
