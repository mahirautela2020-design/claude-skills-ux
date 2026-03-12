---
name: ui-visual-design-layout
description: >
  Designs clear, consistent visual hierarchy and layouts across breakpoints.
  Use when the user needs help with hierarchy, spacing, grids, typography,
  color, and imagery to guide attention and meaning, or when adapting layouts
  across different screen sizes and densities while keeping visual consistency,
  aligned with shared UX principles and accessibility guidance.
metadata:
  domain: ui
  category: visual-layout
  author: your-name
  version: 1.1.0
---

# UI Visual Design & Layout

## Purpose

This skill helps create interfaces with clear visual hierarchy and well-structured layouts that guide attention and support comprehension.[web:230][web:296] It covers grids, spacing, typography, color, and imagery, and how to adapt these across different breakpoints and pixel densities while maintaining consistency and accessibility, drawing on `ux-design-principles` for visual foundations, accessibility, and platform guidance.[web:260][web:293][web:236]

Use this skill when designing or reviewing UI at any fidelity where visual structure, emphasis, and responsiveness matter.

---

## Instructions

### Step 1: Clarify content, priorities, and breakpoints

Start by understanding what the layout must support.

Ask:

- "What content and actions must appear on this screen?"
- "What is the primary goal or task for this screen?"
- "Which breakpoints or platforms are in scope (e.g., mobile, tablet, desktop)?"

Summarize:

- Primary and secondary actions.
- Key content blocks (e.g., hero, forms, lists, navigation, supporting info).
- Breakpoints to design for (e.g., 320–480, 768, 1024+).[web:296]

This will drive hierarchy and layout decisions and later link to key metrics like task success, time to find information, or conversion (via `ux-product-design-metrics`).[web:303]

---

### Step 2: Define visual hierarchy

Decide what should draw attention first, second, and third.[web:230]

Guidelines:

- Use size, weight, contrast, and position to indicate importance.
- Establish a clear hierarchy for:
  - Page or screen title.
  - Primary action(s).
  - Secondary actions and supporting information.
- Avoid competing focal points; ensure there is a clear “entry point” for the eye.

Check:

- Can users scan the screen and quickly understand what it’s for and what to do next?
- Are primary actions visually distinct from secondary or tertiary actions?

Align hierarchy decisions with laws and principles in `ux-design-principles` (e.g., Aesthetic–Usability Effect, Von Restorff effect, recognition over recall).[web:260][web:262]

---

### Step 3: Use grids and spacing for structure

Apply a grid and spacing system to keep the layout consistent and flexible.[web:296][web:301]

Decide:

- Grid type (e.g., 12-column grid for desktop, fewer columns for mobile).
- Margins and gutters appropriate to platform and screen size.
- Base spacing scale (e.g., 4/8 px scale) and how it applies to padding and gaps.

Apply:

- Align main content blocks to grid columns.
- Maintain consistent spacing between related elements and groups.
- Use spacing to indicate grouping and separation (more space between groups than within groups), reflecting Gestalt principles such as proximity and common region from `ux-design-principles`.[web:272][web:276]

Avoid:

- Arbitrary pixel values that don’t follow the spacing system.
- Misaligned content that breaks the implicit grid without a clear reason.

---

### Step 4: Set typography for readability and hierarchy

Choose and apply type styles that support readability and hierarchy.[web:230]

Decide:

- Type scale: sizes for headings, subheadings, body text, captions.
- Weights and styles for emphasis (regular, medium, bold).
- Line length and line height appropriate to screen size and content type.

Guidelines:

- Ensure sufficient contrast between text and background (see accessibility guidance in `ux-design-principles`).[web:293]
- Use heading levels consistently: H1 for screen title, then descending levels for sub-sections.
- Avoid using many different fonts or too many styles; keep the system simple and consistent.

Check:

- Can users quickly skim headings and find what they need?
- Is body text comfortable to read on target devices?

---

### Step 5: Use color intentionally and accessibly

Use color to support meaning and hierarchy, not as decoration only.[web:230][web:236]

Guidelines:

- Define roles for colors (e.g., primary action, secondary action, destructive, feedback states, backgrounds, borders) and map them to tokens if you use design systems.
- Use color to:
  - Highlight primary actions and key information.
  - Differentiate states (normal, hover, focus, error, success).
- Maintain sufficient contrast for text and important UI elements (align with WCAG contrast ratios).[web:293]

Avoid:

- Using color alone to convey important information; pair with text, icons, or patterns.
- Overloading the interface with many different, unrelated colors.

Ensure that color choices align with brand where applicable, but not at the expense of usability or accessibility, following color theory and semantic color guidance in `ux-design-principles`.[web:230][web:239]

---

### Step 6: Use imagery and iconography purposefully

When including images or icons:[web:233]

- Ensure they support the content or task (e.g., illustrating a concept, providing recognition).
- Keep style consistent (illustration style, photography style, icon stroke/fill).
- Avoid images that distract from primary tasks or slow comprehension.

For icons:

- Use them to support labels, not to replace text for critical actions.
- Ensure that icons are legible at the sizes used.
- Use consistent meaning across the product (same icon → same function).

Consider accessibility implications (e.g., alt text, non-text alternatives) in collaboration with `ux-accessibility-inclusive-design` and `ux-design-principles`.[web:293]

---

### Step 7: Design for multiple breakpoints and densities

Adapt layouts responsively while preserving hierarchy and meaning.[web:296][web:301]

For each breakpoint:

- Identify which content is essential and must stay visible.
- Adjust grid and spacing:
  - Fewer columns and larger tap targets on smaller screens.
  - Reflow content vertically for narrow viewports; move from multi-column to single-column where needed.
- Consider reordering sections where appropriate to keep the most important content near the top.

Ensure:

- Primary actions remain easy to access (e.g., reachable thumbs on mobile, aligning with mobile guidelines in `ux-design-principles`).[web:278][web:284]
- Typography scales appropriately (not too small on small screens, not too large on large screens).
- Key patterns (e.g., cards, lists, forms) adapt gracefully without breaking.

---

### Step 8: Check alignment, consistency, and rhythm

Refine layouts for polish and coherence.[web:230]

Check:

- Alignment:
  - Text and elements line up to grid and each other where expected.
  - Forms and related controls are aligned for easy scanning.
- Consistency:
  - Similar elements (e.g., cards, list items, buttons) share spacing, corner radius, shadows, and other styling.
- Rhythm:
  - Vertical spacing between sections feels regular and intentional.
  - There are no random jumps or cramped areas.

Fix:

- Stray misalignments.
- Inconsistent paddings/margins.
- Overly tight or overly loose sections.

Align visual decisions with design system tokens and components where possible so they can be reused and enforced via `ux-design-principles` and design-system skills.[web:210]

---

### Step 9: Prepare visual specs for implementation

Document the visual design decisions so they can be implemented accurately.[web:320]

For each major screen or component, specify:

- Layout:
  - Grid usage (columns, gutters, margins).
  - Key spacing values between elements and sections.
- Typography:
  - Font styles (family, size, weight, line height) for each text role.
- Color:
  - Tokens or hex values for backgrounds, text, borders, actions, states.
- Responsive behavior:
  - How layout changes at specified breakpoints.
  - Any components that stack, collapse, or change behavior.

Where relevant, reference design system tokens and components so devs can reuse existing building blocks and so measurements (e.g., Core Web Vitals, readability, engagement) can be tied back to visual changes via `ux-product-design-metrics`.[web:239][web:303]

---

## Examples

### Example 1: Responsive marketing hero

- Desktop:
  - Two-column layout: messaging and CTA on the left, illustration on the right.
  - Clear hierarchy: headline, supporting copy, primary and secondary buttons.
- Mobile:
  - Single-column layout: illustration above or below copy as appropriate, CTA buttons stacked.
  - Typography and spacing scaled for comfortable mobile reading and tapping.

### Example 2: Data table layout

- Desktop:
  - Multi-column table aligned to grid, with clear column headers and consistent row height.
  - Primary actions available at row level and in a toolbar.
- Mobile:
  - Cards or responsive table pattern with key data surfaced and secondary data collapsed.
  - Actions accessible via a clear, consistent pattern (e.g., overflow menu on each card).

---

## Troubleshooting

### Layout feels cluttered or noisy

- Remove non-essential elements and decorative lines.
- Increase spacing between groups and simplify background treatments.
- Revisit color usage; reduce the number of competing accents.

### Users miss key information or actions

- Check whether the primary content and actions have enough visual weight and clear positioning.
- Adjust hierarchy with size, contrast, or placement.
- Reduce competing elements near critical areas.

### Designs don’t scale well to smaller screens

- Reevaluate what is essential at smaller breakpoints.
- Simplify layouts; move from multiple columns to one column.
- Ensure tap targets and text remain usable at touch sizes, following guidance in `ux-design-principles` and `ux-accessibility-inclusive-design`.[web:278][web:293]

---

## Notes for use with other skills

- Use this skill with:
  - `ux-interaction-design` to align visual treatments with interaction states and behaviors.[web:240]
  - `ux-accessibility-inclusive-design` to ensure contrast, size, and structure support accessibility.[web:293]
  - `ux-design-principles` as the foundation for hierarchy, color, motion, platform guidelines, and data visualization basics.[web:260][web:230]
  - Design system skills to codify visual decisions into reusable tokens and components.[web:210]
  - `ux-product-design-metrics` when visual/layout changes are expected to impact metrics such as task success, time to find key information, conversion, or engagement.[web:303]
