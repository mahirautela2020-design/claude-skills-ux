---
name: ui-design-systems-components
description: >
  Designs, documents, and evolves design systems. Use when the user needs help
  creating or refining tokens, components, and patterns, defining states and
  variants, writing usage guidelines, or working within a contribution and
  governance model for a design system, aligned with shared UX principles,
  accessibility, atomic design, and metrics.
metadata:
  domain: ui
  category: design-systems
  author: your-name
  version: 1.2.0
---

# UI Design Systems & Components

## Purpose

This skill helps create and maintain coherent design systems: the reusable tokens, components, and patterns that ensure consistent, scalable UI.[web:210][web:253] It assumes an **atomic design** mindset where smaller building blocks (tokens, atoms) combine into components and larger patterns (molecules, organisms, templates) to build whole experiences, rather than isolated pages.[web:332][web:342] It covers defining tokens, building components with states and variants, documenting usage guidelines, and understanding contribution and governance so the system can evolve sustainably, in alignment with `ux-design-principles` and `ux-product-design-metrics`.[web:260][web:293][web:303]

Use this skill when designing new components, refactoring screens into system pieces, or improving how your product team uses and maintains a design system.

---

## Instructions

### Step 1: Clarify product scope and system goals

Before working on the system, understand where it will be used and what it must support.[web:253]

Ask:

- "Which products or surfaces does this system need to cover (web, mobile, desktop)?"
- "What are the main UI patterns and components currently in use?"
- "What problems are we trying to solve with the design system (inconsistency, speed, quality, accessibility, handoff)?"

Summarize:

- Supported platforms and form factors.
- Key component families (e.g., inputs, buttons, navigation, cards, table patterns).
- System goals (e.g., reduce duplication, improve accessibility, speed up delivery, align with `ux-design-principles` and atomic design).[web:332][web:342]

---

### Step 2: Inventory existing UI and identify candidate components

Start from real product screens.[web:253]

- Gather representative screens across the product (core flows, onboarding, settings, dashboards).
- Identify repeated UI patterns:
  - Controls (buttons, inputs, toggles, dropdowns).
  - Content containers (cards, list items, table rows).
  - Navigation elements (tabs, sidebars, menus).
  - Feedback patterns (alerts, banners, toasts, inline status).

Group similar patterns and note variations. This forms the starting point for system components and helps you see how current UI naturally clusters into **atoms, molecules, and organisms** in an atomic design sense (e.g., input + label + helper text as a molecule, header as an organism).[web:332][web:342]

---

### Step 3: Define design tokens

Establish tokens as the smallest reusable design decisions.[web:210][web:339][web:342]

Common token categories:

- **Color tokens** – primary, secondary, background, surface, border, text, semantic (success, warning, error, info).
- **Typography tokens** – font families, sizes, weights, line heights for headings, body, captions.
- **Spacing tokens** – a spacing scale (e.g., 4/8/12/16 px) used for margins, paddings, and gaps.
- **Radius, border, shadow tokens** – consistent corners, strokes, and elevation levels.
- **Layout and motion tokens** – grid, breakpoints, density, durations, easing for key interactions.[web:339]

For each token:

- Define a name (e.g., `color-primary`, `space-4`, `radius-sm`, `motion-fast`).
- Provide value(s) and short description of intended use.

Treat tokens as the **subatomic layer** beneath atoms in your atomic design system (tokens → atoms → molecules → organisms → templates → pages).[web:339][web:342] Encourage components to consume tokens rather than hard-coded values so changes can propagate systematically, and ensure tokens meet accessibility guidance from `ux-design-principles` and `ux-accessibility-inclusive-design`.[web:293]

---

### Step 4: Design core components

Based on the inventory, design core components (atoms and molecules) for the system, following atomic design concepts from `ux-design-principles` and Brad Frost’s methodology.[web:210][web:332][web:342]

For each component (e.g., Button, Text Field, Card, Modal, Tag):

- Define structure:
  - Required elements (label, icon, helper text, etc.).
  - Optional elements (leading/trailing icons, supporting text).
- Apply tokens:
  - Colors, typography, spacing, radius, shadows drawn from tokens.
- Ensure alignment with accessibility and interaction requirements:
  - Size and hit area (e.g., touch-target guidance).[web:278]
  - Contrast and focus states (defined later in states).
  - Support for labels and error messaging patterns.

Consider how components will compose into larger patterns (e.g., search bar molecule, header organism, template) so they work well in composition, not just in isolation.[web:332][web:337]

Aim for components that are flexible enough for real use cases but not overloaded with unnecessary options.

---

### Step 5: Define states and variants

Specify how components behave in different situations.[web:253]

For each component, define:

- **States**:
  - Default
  - Hover / focus / active (where applicable)
  - Disabled
  - Loading
  - Error / success / warning (if relevant)
- **Variants**:
  - Style variants (e.g., primary, secondary, ghost, destructive).
  - Size variants (e.g., small, medium, large).
  - Layout variants (e.g., with icon, icon-only, text-only).

Document:

- Visual differences between states and variants (colors, borders, elevation, etc.).
- Behavioural differences (e.g., which states are interactive, which show specific feedback).

Ensure each state and variant has a clear purpose and is not duplicative, and that error/success/warning states align with semantics and accessibility guidance in `ux-design-principles`.[web:260][web:293]

---

### Step 6: Define component properties and constraints

Make components predictable and easier to use by specifying their properties and boundaries.[web:210][web:253]

For each component:

- List configurable properties (e.g., `label`, `icon`, `size`, `variant`, `isLoading`, `isDisabled`, `ariaLabel`).
- Define allowed combinations and constraints (e.g., destructive buttons must use specific variants; icon-only buttons require accessible labels).
- Clarify default values (e.g., default size, default variant, default layout).

This helps designers and engineers use components correctly and avoids pattern drift, and supports metric-friendly consistency (e.g., consistent primary button usage across flows) that ties into `ux-product-design-metrics`.[web:303]

---

### Step 7: Document usage guidelines and examples

Create simple, practical guidance for how and when to use each component.[web:253]

For each component, document:

- **When to use**:
  - Typical use cases.
  - When **not** to use it (e.g., don’t use this component for navigation, use tabs instead).
- **Behaviour guidance**:
  - How it behaves with long text, empty values, or unusual data.
  - How it responds across breakpoints (e.g., stack vs inline).
- **Examples**:
  - Good use examples with context.
  - Common pitfalls or anti-patterns.

Where relevant, reference specific principles from `ux-design-principles` (e.g., recognition over recall, error prevention, Fitts’s Law, inclusive design) and clarify how components combine into molecules/organisms/templates in your atomic system.[web:260][web:332][web:342]

This documentation can live as part of your design system site or references inside your skill.

---

### Step 8: Plan contribution and governance

Ensure the design system can evolve without chaos.[web:253][web:320]

Define:

- **Who can propose changes or new components** (e.g., any product team designer, through a defined process).
- **Review process**:
  - How proposals are reviewed (design review, accessibility review, technical feasibility).
  - Who approves changes (design system council, leads).
- **Versioning and communication**:
  - How changes are versioned and communicated to teams (changelog, release notes, announcements).

Encourage:

- Adding new variants and components only when needed and when they serve multiple use cases.
- Deprecating components and variants when they cause confusion or are replaced by better patterns.
- Using `ux-product-design-metrics` when appropriate to justify larger system investments (e.g., measuring impact on speed, quality, task success, or support tickets).[web:303][web:309]

Maintain an atomic perspective: changes at token or atom level will cascade into molecules, organisms, templates, and pages, so governance must consider system-wide impact.[web:337][web:342]

---

### Step 9: Align implementation and ongoing maintenance

Make sure the **code implementation** of the design system matches the design.[web:253]

Work with engineering to:

- Map design components to code components and tokens (e.g., in a component library or design tokens system).
- Maintain one source of truth for component behaviour and styling.
- Plan regression checks when changes are made to core components (e.g., via visual regression testing and automated accessibility checks).

For ongoing maintenance:

- Periodically audit product screens to find divergence from the system.
- Capture useful “product-only” patterns that should be considered for upstream inclusion.
- Update documentation when behaviour or visual decisions change.

Use `ux-usability-heuristics` and `ux-accessibility-inclusive-design` to evaluate system components themselves, ensuring the design system encodes good usability and accessibility by default.[web:288][web:293][web:280]

---

## Examples

### Example 1: Button component

- Tokens:
  - Colors: primary, secondary, destructive, disabled.
  - Typography: label style.
  - Spacing: padding tokens around text.
- Variants:
  - Primary, secondary, ghost, destructive.
  - Sizes: small, medium, large.
- States:
  - Default, hover, focus, active, loading, disabled.
- Usage guidelines:
  - Primary for main actions; one per view where possible.
  - Secondary for less prominent actions.
  - Destructive reserved for irreversible actions with confirmation.
  - Icon-only buttons require accessible labels and clear focus states.

In atomic terms, the button is an **atom** that appears inside molecules (e.g., search bar) and organisms (e.g., header, card actions) and is reused in templates and pages.[web:332][web:342]

### Example 2: Card pattern

- Structure:
  - Container with title, metadata, primary action, optional summary or image.
- Tokens:
  - Elevation levels (e.g., default vs hover shadow).
  - Spacing and radius.
- Variants:
  - Simple card (title + text).
  - Card with media.
  - Selectable card.
- Usage guidelines:
  - Use cards to represent discrete items (e.g., projects, products).
  - Avoid mixing multiple interaction patterns within a single card (e.g., entire card clickable plus internal buttons) without clear rules documented in `ux-interaction-design`.

A card is typically a **molecule** or **organism**, composed of atoms (text, icons, buttons) and molecules (e.g., media + text) assembled in line with atomic design.[web:332][web:342]

---

## Troubleshooting

### Too many similar components

- Identify overlap and redundancy.
- Merge components or reduce variants to a smaller, more focused set.
- Prefer extending existing components over creating entirely new ones where possible.

### Components are misused in product teams

- Check whether documentation and examples are clear enough.
- Add more guidance on “when not to use” and common mistakes.
- Provide design reviews or office hours to help teams adopt patterns correctly.

### System is hard to keep up to date

- Establish clearer governance: who owns what, and how often the system is reviewed.
- Ensure changes are communicated via regular updates and are easy to apply (e.g., through tokens and component libraries).
- Track system adoption and gaps, and prioritize improvements based on real use and impact on metrics where available (e.g., speed of delivery, defects, support tickets).

---

## Notes for use with other skills

- Use this skill together with:
  - `ui-visual-design-layout` to ensure components follow visual hierarchy and layout rules.[web:230]
  - `ux-interaction-design` so component behaviour, states, and feedback match interaction principles and platform conventions.[web:240][web:236]
  - `ux-accessibility-inclusive-design` to bake accessibility into tokens and components (contrast, hit areas, semantics, motion).[web:293][web:280]
  - `ux-design-principles` as the canonical reference for atomic design, tokens, patterns, and UX laws applied at system level.[web:210][web:260][web:332][web:342]
  - `ux-product-design-metrics` and product skills when aligning system changes with product roadmaps and demonstrating impact on metrics like speed, consistency, and UX quality.[web:303][web:309]
