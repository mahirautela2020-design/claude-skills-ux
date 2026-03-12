---
name: ui-platform-patterns-responsive
description: >
  Applies platform-specific patterns and responsive/adaptive behavior. Use when
  the user needs help following or extending web, iOS, Android, or desktop
  conventions, choosing when to follow vs invent patterns, and designing
  responsive/adaptive layouts (grids, breakpoints, touch vs pointer) that
  align with shared UX principles and design system components.
metadata:
  domain: ui
  category: platform-patterns
  author: your-name
  version: 1.1.0
---

# UI Platform Patterns & Responsiveness

## Purpose

This skill helps design interfaces that feel native to their platforms while staying consistent across a product suite.[web:236][web:278] It covers understanding platform patterns (web, iOS, Android, desktop), deciding when to follow vs extend them, and designing responsive/adaptive behavior across screen sizes and input types (touch vs pointer), in alignment with `ux-design-principles`, `ui-visual-design-layout`, `ui-design-systems-components`, and `ux-accessibility-inclusive-design`.[web:260][web:293][web:210]

Use this skill when you’re designing multi-platform products, responsive layouts, or deciding how much to lean on native conventions versus custom patterns.

---

## Instructions

### Step 1: Clarify platforms, devices, and inputs

Start by listing where the interface will run and how people will interact.[web:236]

Ask:

- "Which platforms are we targeting (web, iOS, Android, desktop, others)?"
- "Which devices and orientations matter (phone, tablet, laptop, large monitor)?"
- "What input methods are primary (touch, mouse, trackpad, keyboard, stylus)?"

Summarize:

- Platform(s) and OS (e.g., responsive web app, iOS app, Android app).
- Device range and critical breakpoints.
- Primary input paradigms (touch-first vs pointer/keyboard first).

This context will guide layout, interaction patterns, and accessibility considerations from other skills.

---

### Step 2: Identify key platform conventions

For each platform, note the major conventions relevant to your product.[web:236][web:278]

Examples:

- **Web**:
  - Top navigation bars, sidebars, scroll-based layouts, browser controls.
  - Standard patterns for links, buttons, forms, modals, and tooltips.
- **iOS**:
  - Navigation bars, tab bars, segmented controls, swipe gestures.
  - Navigation stacks and modal presentation styles.
- **Android**:
  - Material guidelines: bottom navigation, Floating Action Button (FAB), drawers.
  - Back button behavior, system-level gestures.
- **Desktop apps**:
  - Menus, toolbars, resizable windows, keyboard shortcuts.

For your specific product, list:

- Which native patterns you intend to follow.
- Any platform-specific components you should use or mirror (e.g., date pickers, navigation models).

Refer back to `ux-design-principles` for platform-specific guidance (web, iOS, Android) and to your design system for existing cross-platform components.[web:236][web:260][web:210]

---

### Step 3: Decide when to follow vs invent patterns

Use platform patterns as the default, and only invent custom patterns when necessary.[web:236][web:260]

Guidelines:

- Follow platform conventions when:
  - They cover your use case well.
  - Users bring strong expectations (e.g., back navigation, tab behavior).
  - It reduces learning and friction (Jakob’s Law).
- Consider extending or carefully inventing patterns when:
  - Your product needs unique workflows or data representations.
  - You can’t achieve the experience with existing patterns.
  - You can still explain the pattern simply and keep it consistent.

When inventing or extending:

- Ensure the new pattern is internally consistent and codified in `ui-design-systems-components`.
- Avoid breaking core platform expectations (e.g., back button behaviour, standard gestures).
- Document why you diverged and how the pattern should be used.

---

### Step 4: Plan responsive breakpoints and layout strategies

Define how your layout adapts across screen sizes, in line with `ui-visual-design-layout`.[web:296][web:301]

Decide:

- Key breakpoints (e.g., small: <600px, medium: 600–1024px, large: >1024px).
- Layout strategy at each breakpoint:
  - Small: mostly single-column, stacked content, larger tap targets.
  - Medium: one or two columns where appropriate.
  - Large: multi-column layouts, sidebars, denser content grids.

For each breakpoint, specify:

- Which elements move, stack, or hide.
- How navigation changes (e.g., top bar → menu button + drawer; tabs → overflow).
- How content density and spacing adjust.

Use grids, spacing scales, and typography rules from `ui-visual-design-layout` and tokens from `ui-design-systems-components` so responsiveness remains systematic.[web:210][web:230]

---

### Step 5: Design adaptive patterns for key components

Define how important components adapt, not just resize.[web:296]

Examples:

- **Navigation**:
  - Desktop: persistent top and/or side navigation.
  - Mobile: tab bar, hamburger/drawer, or bottom nav as appropriate.
- **Tables and data-heavy views**:
  - Desktop: full table, multiple columns, inline actions.
  - Mobile: card-based representation, key fields only, expandable details.
- **Forms**:
  - Desktop: multi-column layouts where beneficial.
  - Mobile: single-column forms with clear labels and appropriate input types.

For each key component or pattern:

- Describe its behaviour on small, medium, and large screens.
- Specify any breakpoint-specific features (e.g., secondary content hidden on mobile, accessible through a dedicated screen).

Sync these definitions with component specs in `ui-design-systems-components` so the library encodes responsive/adaptive behaviour by default.[web:210][web:253]

---

### Step 6: Account for touch vs pointer interactions

Design for the primary input method while respecting secondary ones.[web:278][web:293]

For **touch-first** contexts:

- Ensure tap targets are large enough and have enough spacing (follow touch target guidance from `ux-design-principles`).[web:278]
- Avoid hover-only interactions; provide visible, tap-accessible affordances.
- Consider gesture support where appropriate, but always provide visible alternatives.

For **pointer/keyboard-first** contexts:

- Support hover states to preview information or show extra controls.
- Ensure focus states are clear for keyboard navigation.
- Make fine-grained controls usable with mouse/trackpad.

Avoid designs that require hover or precise cursor actions in touch contexts without alternatives, and coordinate with `ux-accessibility-inclusive-design` to ensure operability across inputs.[web:293]

---

### Step 7: Maintain cross-platform consistency where it matters

Balance platform-native behaviour with product-wide consistency.[web:236][web:260]

- Keep core concepts, naming, and flows consistent across platforms (so users recognise the same product).
- Allow visual and interaction details to follow platform conventions (e.g., different switch or button styles), while preserving intent.
- For cross-platform features, ensure:
  - Similar information is findable in similar places.
  - Key tasks follow comparable sequences, even if UI elements differ.

Document any platform-specific differences so they are intentional, not accidental, and ensure they are reflected in your design system documentation.

---

### Step 8: Validate patterns across breakpoints and platforms

Review and, where possible, test designs across the full range of contexts.[web:296]

Check:

- Layout doesn’t break or become unusable at any common screen size.
- Navigation remains discoverable and understandable as it adapts.
- Critical tasks remain easy to perform on touch and pointer devices.
- Platform-specific behaviours (e.g., back navigation, system gestures) don’t conflict with your patterns.

If possible, run quick checks on real devices or emulators to catch real-world issues (e.g., keyboard overlap on mobile, viewport quirks), and use `ux-prototyping-validation` for structured usability tests when changes are risky.[web:325]

---

### Step 9: Document responsive and platform behaviour for implementation

Make platform patterns and responsive behaviour explicit in specs.[web:320]

For each screen or pattern, document:

- Supported platforms and breakpoints.
- Layout specifications at each breakpoint (e.g., number of columns, major structural changes).
- Platform-specific patterns where applicable (e.g., tabs vs drawers, bottom vs side nav).
- Input considerations (tap target sizes, hover behaviour, keyboard interactions).

Link this documentation to your design system (`ui-design-systems-components`) and layout guidance (`ui-visual-design-layout`) so the same components behave correctly across contexts, and to `ux-accessibility-inclusive-design` to highlight accessibility expectations.[web:210][web:293]

---

## Examples

### Example 1: Multi-platform navigation

- Web:
  - Desktop: top navigation with prominent links and a secondary side navigation on wider screens.
  - Mobile: hamburger menu that opens a full-height drawer, with key actions accessible via a bottom nav bar.
- Native apps:
  - iOS: tab bar for primary sections, navigation stacks for detail screens.
  - Android: bottom nav and drawer following Material patterns, with platform-consistent back behaviour.

### Example 2: Responsive data view

- Desktop:
  - Full table with sortable columns, bulk actions, and in-row actions.
- Tablet:
  - Table with fewer visible columns and actions grouped in an overflow menu.
- Mobile:
  - Cards showing key data points, with a “view details” pattern to access full information.

---

## Troubleshooting

### Design looks good on desktop but breaks on mobile

- Revisit breakpoints and layouts; simplify structure for small screens.
- Reduce non-essential content and patterns at small sizes.
- Ensure navigation remains easy to reach and understand, and that touch targets meet size guidelines.[web:278]

### Platform-specific expectations are violated

- Identify where your design conflicts with established platform patterns (e.g., back button behaviour, tab bar usage).
- Adjust to better align with user expectations unless there’s a very strong reason not to.
- Document any intentional deviations and make sure they’re consistently applied.

### Too many platform-specific variations

- Look for opportunities to share underlying patterns and logic across platforms.
- Limit platform-specific variations to places where they provide clear user value.
- Use tokens and components that adapt visually per platform while maintaining structure and meaning, leveraging `ui-design-systems-components`.[web:210][web:342]

---

## Notes for use with other skills

- Use this skill with:
  - `ui-visual-design-layout` to ensure responsive layouts maintain clear hierarchy and rhythm.[web:230][web:296]
  - `ui-design-systems-components` to codify platform-aware components and responsive/adaptive patterns using tokens and atomic design.[web:210][web:332]
  - `ux-interaction-design` to ensure platform-appropriate interactions, gestures, and feedback behaviours.[web:240][web:236]
  - `ux-accessibility-inclusive-design` to keep responsive and platform behaviour accessible for different input types and contexts.[web:293][web:280]
  - `ux-product-design-metrics` when platform and responsiveness decisions are expected to impact metrics such as task success, time to complete, engagement, or adoption.[web:303]
