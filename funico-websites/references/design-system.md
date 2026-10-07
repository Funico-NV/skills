# Funico Design System

## Visual Direction

Funico websites should feel like premium operational software: calm, clear, data-capable, and built around real work. The attached design reference is a useful direction for density, spacing, card treatment, and tabbed work areas, but the header should be significantly more refined.

Use the reference's strengths:

- Light gray-blue application background.
- White or near-white panels with subtle borders.
- Compact navigation tabs with clear active states.
- Strong numeric hierarchy for operational metrics.
- Dense but readable forms and tables.
- Restrained shadows, mostly for separation rather than decoration.

Avoid copying the weak parts:

- Do not use a flat full-width strip that makes the brand feel secondary.
- Do not leave the website icon as a small utility mark.
- Do not let the header become only a navigation container.

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

The header must be a branded composition, not a plain top bar.

Required header qualities:

- A prominent website icon appears in the header or first viewport.
- The icon sits in a deliberate mark container, such as a beveled square, soft tile, circular seal, or integrated brand lockup.
- The brand name and page/product context should align cleanly with the icon.
- Navigation should feel connected to the header but not crowd the icon.
- Header height should be generous enough for brand presence while staying efficient for operational apps.
- Utility items should be visually secondary.

Good header patterns:

- A dark base-tint header with an icon tile on the left, brand text beside it, and compact navigation below or to the right.
- A split header where a brand rail contains the icon and product name, while a lighter navigation band holds tabs.
- A first-viewport hero header where the icon appears as a large product mark, with navigation kept minimal and precise.

Avoid:

- Tiny favicon-style marks as the only icon usage.
- Generic logo placeholder squares.
- Header text that is larger than the icon treatment but less visually considered.
- Overcrowded nav bars.
- Glassmorphism, large gradients, or decorative background shapes.

## Required Website Icon

Every website must include a website icon concept. Treat it as a first-class design element.

The icon should:

- Be simple enough to work as a favicon.
- Be polished enough to appear at 40-64px in the header.
- Use the base tint and secondary tint, with white or near-white where useful.
- Be visually related to the website's domain or product purpose.
- Have a defined container and spacing rules.

Deliver at least one of these when creating a new site:

- A clear icon concept in the design notes.
- An implemented icon component.
- A generated or hand-built icon asset.

Do not finish a new Funico website without addressing the icon.

## Layout

Prefer dense but calm interfaces. A Funico website can be spacious, but it should still feel useful immediately.

Recommended layout values:

- Content max width: `1200px` to `1440px`, depending on app density.
- Desktop page padding: `32px`.
- Tablet page padding: `24px`.
- Mobile page padding: `16px`.
- Section gap: `32px` to `64px`.
- Panel gap: `12px` to `24px`.

For operational screens:

- Side panels may be used for inputs or filters.
- Main content should prioritize current result, metrics, tables, and task flow.
- Use tabs for peer-level views.
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

- Radius should usually be `8px` or less.
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
- Collapse navigation into a compact menu or horizontal scroll tabs.
- Stack side panels above main content when needed.
- Preserve data readability by prioritizing key metrics before detailed tables.

Do not allow text, tabs, buttons, metric cards, or icon lockups to overlap.
