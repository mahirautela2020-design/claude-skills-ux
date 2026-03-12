---
name: ui-design-tools-handoff
description: >
  Uses design tools effectively and prepares developer-ready handoff. Use when
  the user needs help structuring files, working with components, variants, and
  auto-layout, creating prototypes, and generating clear specs, annotations,
  and tokens for implementation and QA, aligned with the design system and
  atomic design.
metadata:
  domain: ui
  category: tools-handoff
  author: your-name
  version: 1.1.0
---

# UI Design Tools & Handoff

## Purpose

This skill helps designers use modern tools (such as Figma) effectively for components, layout, and prototyping, and then prepare developer-ready outputs.[web:347][web:350] It covers organizing files, using components, variants, and auto-layout, creating prototypes for flows, and producing clear specs, annotations, and tokens so implementation goes smoothly, in alignment with `ui-design-systems-components`, `ui-visual-design-layout`, `ux-interaction-design`, and `ux-accessibility-inclusive-design`.[web:210][web:296][web:240][web:293]

Use this skill when setting up or refining your design files, preparing work for dev handoff, or answering implementation questions.

---

## Instructions

### Step 1: Organize files, pages, and frames

Start by structuring the design workspace.[web:347][web:351]

Guidelines:

- Split work into clear pages or sections, for example:
  - `Foundations` (tokens, styles)
  - `Components` (atoms/molecules/organisms)
  - `Patterns`
  - `Flows` or `Screens` (by feature/area)
  - `Prototypes` or `Experiments` (optional)
- Name frames and top-level artboards meaningfully:
  - Include platform and state where useful (e.g., `Desktop / Dashboard / Default`, `Mobile / Onboarding / Step 1`).
- Avoid mixing exploratory work with finalized designs; use separate pages or areas for exploration vs production.

This makes it easier for teammates and developers to find what they need and supports atomic design and design-system organization.[web:332][web:361]

---

### Step 2: Use styles and tokens in the tool

Set up **styles** as a practical representation of your design tokens.[web:350][web:361]

- Create shared styles for:
  - Colors (e.g., primary, secondary, surface, text, semantic).
  - Text (e.g., heading levels, body text, captions).
  - Effects (e.g., shadows, blurs) and grid systems where supported.
- Name styles based on roles, not raw values (e.g., `Color / Primary / Default` instead of `Blue 500`).

Apply these styles consistently:

- Avoid manually setting colors and type wherever a style exists.
- Update styles instead of one-off changes when making system-wide adjustments.

Where possible, integrate with token tooling (e.g., Tokens Studio, Handoff-style pipelines, Style Dictionary) so tokens can be exported to code and kept in sync with implementation.[web:352][web:355][web:356] This ensures the design file stays in sync with the design system and tokens defined in `ui-design-systems-components`.

---

### Step 3: Build and use components and variants

Turn reusable UI pieces into components, following an atomic design approach.[web:357][web:361]

For each candidate component (buttons, inputs, cards, navigation, etc.):

- Create a **base component (atom or molecule)**:
  - With appropriate auto-layout settings.
  - Using token-based styles for color, type, and spacing.
- Create **variants** for:
  - States (default, hover, focus, active, disabled, loading).
  - Style types (primary, secondary, ghost, destructive).
  - Sizes (small, medium, large) if needed.

Guidelines:

- Keep component property names clear (e.g., `State`, `Variant`, `Size`, `Platform`).
- Ensure content (labels, icons) is editable via component properties where possible.
- Use these components in screens instead of drawing from scratch.

Map Figma components and variants directly to the components defined in `ui-design-systems-components` so handoff reflects the system, not one-off designs.[web:210][web:361] This improves consistency and speeds up updates.

---

### Step 4: Use auto-layout and constraints effectively

Use auto-layout to create flexible, resilient layouts inside the design tool.[web:351][web:349]

For groups of elements (e.g., buttons in a row, cards in a list, form fields):

- Apply auto-layout:
  - Set direction (horizontal/vertical).
  - Define spacing between items.
  - Define padding around content.
- Use alignment and resizing options:
  - Fixed vs fill container.
  - Hug contents where appropriate.

For frames representing screens:

- Set **constraints** or responsive resizing rules so elements behave correctly when the frame resizes (e.g., sticky headers, pinned actions).

The goal is to reflect how layouts should behave at different sizes (per `ui-platform-patterns-responsive` and `ui-visual-design-layout`) and make it easy to adjust designs later.[web:296][web:351]

---

### Step 5: Create prototypes to express flows

Use the prototyping features of your tool to represent interactions and flows.[web:347]

- Link screens using interactions:
  - Tap/click → navigate to another screen.
  - Overlays for menus, dialogs, tooltips (where relevant).
- For key flows, create dedicated prototype flows or starting points with names (e.g., `Onboarding flow`, `Checkout flow`).
- Use transitions sparingly and purposefully; prioritize clarity over flashy animations, aligning with motion guidance in `ux-design-principles`.[web:295]

Ensure prototypes:

- Cover main happy paths and at least some key edge/error states.
- Reflect real interaction decisions (e.g., correct buttons, navigation paths) as defined in `ux-interaction-design`.

These prototypes serve both for testing (`ux-prototyping-validation`) and explaining behaviour to developers and stakeholders.[web:325]

---

### Step 6: Prepare developer-ready specs

When designs are ready for implementation, prepare **specs** that developers can rely on.[web:347][web:349][web:350]

Within the design tool (and Dev Mode if available):

- Ensure all elements use shared styles and components where possible.
- Label frames and components clearly (names that match code concepts when possible).
- Use built-in spec features (e.g., inspect/dev mode) so developers can see:
  - Measurements and spacing.
  - Fonts and sizes.
  - Colors and tokens.
  - Component names, variants, and properties.
- Mark frames explicitly as “Ready for Dev” where your process supports it.[web:356]

If needed, add:

- Redlines or explicit measurement callouts for complex areas.
- Notes where behaviour is not obvious from layout alone (e.g., responsive behaviour, scroll areas, conditional states).

---

### Step 7: Add annotations for behaviour and edge cases

Beyond visuals, clarify **behaviour**.[web:349][web:354]

For each critical screen or flow:

- Add annotation layers or sticky notes to capture:
  - Interaction behaviour (on click, on hover, on scroll; keyboard expectations).
  - Error and empty state conditions.
  - Responsiveness (how layout changes at breakpoints).
  - Performance or loading behaviour (e.g., skeletons vs spinners).
- Keep annotations succinct and structured, for example:
  - `Behavior:` …
  - `Errors:` …
  - `Responsive:` …
  - `Notes:` …

This bridges the gap between the interaction specs (`ux-interaction-design`) and visual design in one place and gives QA clear test scenarios.

---

### Step 8: Export tokens and assets when needed

When engineering uses design tokens or assets, support automation where possible.[web:350][web:352][web:355][web:360]

- Align token names with your design system (`color-primary`, `space-8`, etc.).
- Where tooling allows, export token definitions (colors, typography, spacing) from the design tool to code-friendly formats (e.g., JSON → Style Dictionary → CSS/JS variables).
- Prepare icons, illustrations, and other assets:
  - Proper export sizes and formats (SVG/PNG, etc.).
  - Naming conventions that make them easy to reference in code.

Minimize manual copying of values; aim for shared token pipelines and CI/CD workflows so design decisions flow into code automatically and stay in sync with the system.

---

### Step 9: Support implementation and QA

During build and QA, be available to clarify design intent and adjust where needed.[web:349][web:358]

- Join discussions when developers have questions about edge cases or behaviour not fully captured in the designs.
- Compare implemented views against the design:
  - Layout and spacing.
  - States and interactions.
  - Typography, colours, and accessibility.
- Help log and prioritize visual and interaction discrepancies that matter for UX, and accept minor differences where they don’t impact users.

Update the design system or specs when implementation uncovers better patterns or constraints you didn’t anticipate, and feed those back into `ui-design-systems-components` and `ux-design-principles` where appropriate.

---

## Examples

### Example 1: Handoff for new settings page

- Organized the page within a `Settings` section in the file, under a clear `Flows` page.
- Used existing form components (atoms/molecules) and auto-layout for fields and actions.
- Created a prototype flow showing navigation from main menu to settings and success/error states.
- Provided specs and annotations covering:
  - Field validations and error messages.
  - Save/cancel behaviour and loading states.
  - Responsive layout for desktop and mobile.

### Example 2: Component library setup

- Defined foundational styles for colors, type, and spacing as token-based styles.
- Created core components (buttons, inputs, cards) using those styles and variants, following atomic design in Figma.[web:357][web:361]
- Documented usage and properties in a dedicated components page, linking to system tokens and code names.
- Collaborated with engineering to align component names and properties with the code library and token pipeline.

---

## Troubleshooting

### Developers say designs are hard to build

- Check if components and layouts use consistent patterns and tokens.
- Simplify overly complex structures or rare variations.
- Align component properties and names with how the code is structured and the design system is implemented.

### Specs and reality drift apart

- Schedule regular check-ins during implementation to catch divergence early.
- Update designs or specs when the team makes intentional changes.
- Feed improvements and new patterns back into the design system and token pipeline.

### Files are messy and hard to navigate

- Consolidate variants into components instead of duplicating similar frames.
- Move old explorations to an archive page.
- Rename pages, frames, and components to follow a clear naming convention and atomic design structure.

---

## Notes for use with other skills

- Use this skill with:
  - `ui-design-systems-components` to ensure components in tools map cleanly to system components and atomic structure.[web:210][web:332]
  - `ui-visual-design-layout` to keep visual decisions consistent and responsive in implementation.[web:296]
  - `ux-interaction-design` so behaviour and states are correctly captured in prototypes and annotations.[web:240]
  - `ux-accessibility-inclusive-design` and `ux-usability-heuristics` to ensure what ships matches usability and inclusion goals.[web:293][web:288]
  - `ux-product-design-metrics` when handoff includes instrumentation or metric-related requirements (e.g., events, states to track).[web:303]
