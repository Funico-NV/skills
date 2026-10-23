# Funico Design System

## Visual Direction

Funico websites should feel like premium operational software: calm, clear, data-capable, and built around real work. Use the [current design reference](../assets/design-reference.png) for the compact menu bar, icon placement, density, spacing, and panel treatment. The reference shows an operational app; adapt its content to the project.

Use the reference's strengths:

- Light gray-blue application background.
- White or near-white panels with subtle borders.
- Compact navigation tabs with clear active states.
- Strong numeric hierarchy for operational metrics.
- Dense but readable forms and tables.
- Restrained shadows, mostly for separation rather than decoration.

## Color System

Required tints:

- Base tint: `#006387`
- Secondary tint: `#AABCC6`

Suggested neutral palette:

- Page background: `#F3F7F9`
- Panel background: `#FFFFFF`
- Raised background: `#F8FBFC`
- Primary text: `#102232`
- Secondary text: `#557083`
- Muted text: `#718797`
- Border: `#D7E3EA`
- Soft border: `#E6EEF2`
- Positive background: `#E4F6EE`
- Positive text: `#14724D`
- Warning accent: `#D6A13D`

Use `#006387` for primary actions, active states, key brand surfaces, and the most important progress or data marks. Use `#AABCC6` for calm secondary surfaces, dividers, inactive UI structure, and icon support tones.

Do not make the entire interface monochrome teal. Combine the brand tint with neutrals, white space, and restrained status colors.

## Header

Use a single compact white menu bar above the light workspace. Keep the icon, product name, and primary navigation on the same row at desktop sizes, as in the current reference.

Desktop starting values (adapt to the product and available width):

- Header height: about `58px` to `60px`, with a subtle bottom border and no heavy shadow.
- Horizontal padding: `24px` to `40px`.
- Website icon: about `30px` to `32px` square, with gently rounded corners and its original proportions preserved.
- Icon-to-name gap: `10px` to `12px`; product name: about `16px`, semibold or bold, in primary text color.
- Brand-to-navigation gap: `24px` to `32px`; navigation labels: about `14px`, with `20px` to `24px` between them.
- Active navigation: darker text with a thin `2px` base-tint underline aligned to the header's bottom edge. Inactive labels use secondary text color.
- Push optional status, environment, or version text to the far right using flexible space; keep it small and muted.

Keep the brand lockup from shrinking and center the icon and text vertically. Place navigation directly after the brand so it reads as one coherent menu bar. Move product descriptors into page content when they would add an unnecessary second line to the header.

Use real navigation links with an accessible current-page state and visible keyboard focus. Keep hit areas comfortable even when the visual mark and labels are compact. Reserve segmented or filled tabs for local controls inside the workspace.

Avoid:

- A tall colored brand band with a separate row repeating the primary navigation.
- Enlarging the icon or adding a hero area just to give the brand more presence.
- Extra frames, padding, or tiles around an icon that already has its own container.
- Generic logo placeholders, crowded navigation, heavy gradients, or decorative header shapes.

## Required Website Icon

Every website must include a website icon concept. Treat it as a first-class design element.

The icon should:

- Be simple enough to work as a favicon.
- Remain clear at the reference header size of `30px` to `32px` and at favicon sizes.
- Use the base tint and secondary tint, with white or near-white where useful.
- Be visually related to the website's domain or product purpose.
- Use a compact rounded-square treatment when appropriate; preserve an existing supplied icon and its built-in container. Define spacing around the mark without adding an extra frame.

Deliver at least one of these when creating a new site:

- A clear icon concept in the design notes.
- An implemented icon component.
- A generated or hand-built icon asset.

Do not finish a new Funico website without addressing the icon.

## Layout

Prefer dense but calm interfaces. A Funico website can be spacious, but it should still feel useful immediately.

Recommended layout values:

- Content max width: `1200px` to `1440px`, depending on app density.
- Desktop page padding: `24px` to `32px`.
- Tablet page padding: `24px`.
- Mobile page padding: `16px`.
- Operational section gap: `20px` to `24px`; public content sections may use `32px` to `64px`.
- Panel gap: `12px` to `24px`.

For operational screens:

- Side panels may be used for inputs or filters; the reference uses an approximately `340px` settings panel with a `20px` to `24px` gap before the main workspace.
- Main content should prioritize current result, metrics, tables, and task flow.
- Keep primary peer-level views in the header; use local tabs only for views or controls within the current page.
- Use cards for metrics and repeated entities only; do not put cards inside cards.

## Typography

Use a restrained hierarchy:

- Product or page title: strong, compact, and clear.
- Data values: large and high contrast.
- Labels: small, slightly muted, and consistent.
- Body text: readable, direct, and never marketing-heavy unless the page is explicitly a public landing page.

Avoid viewport-scaled text. Do not use negative letter spacing.

## Components

Buttons:

- Primary buttons use `#006387`.
- Secondary buttons use white or pale blue-gray surfaces with clear borders.
- Destructive or warning actions should not reuse the primary tint.

Cards and panels:

- Use approximately `10px` to `12px` radii for main panels and `6px` to `8px` for controls, matching the reference.
- Borders should carry most separation.
- Shadows should be subtle and rare.
- Avoid nested cards.

Tabs:

- Use compact tabs with a clear active underline, border, or filled surface.
- Active tab color should connect to `#006387`.

Forms:

- Inputs should feel precise and utility-oriented.
- Use labels, units, and help text sparingly but clearly.
- Keep form controls aligned in predictable grids.

Tables and data rows:

- Use clear column labels.
- Use calm row separators.
- Highlight important bars, quantities, or statuses with brand and status colors.

## Responsive Behavior

On mobile:

- Keep the icon and brand visible.
- Move primary navigation into an accessible compact menu or its own horizontally scrollable row before it crowds the brand. Do not shrink the icon or clip navigation labels.
- Move or hide nonessential utility text first; retain access to any utility actions.
- Stack side panels above main content when needed.
- Preserve data readability by prioritizing key metrics before detailed tables.

Do not allow text, tabs, buttons, metric cards, or icon lockups to overlap.
