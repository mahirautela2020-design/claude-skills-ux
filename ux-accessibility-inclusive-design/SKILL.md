---
name: ux-accessibility-inclusive-design
description: >
  Designs experiences that are accessible and inclusive by default. Use when
  the user needs help applying accessibility best practices (contrast,
  keyboard, semantics) at design time, considering diverse abilities, devices,
  and contexts, and designing alternatives where needed. Focuses on practical
  guidance for designers to catch issues early and collaborate effectively
  with engineers, QA, and broader UX principles and metrics.
metadata:
  domain: ux
  category: accessibility-inclusive
  author: your-name
  version: 1.1.0
---

# UX Accessibility & Inclusive Design

## Purpose

This skill helps you design interfaces and flows that work for more people, by building accessibility and inclusion into design decisions instead of leaving them only to QA or compliance checks.[web:293][web:298] It focuses on practical considerations for contrast, keyboard use, semantics, copy, and context, and on designing alternatives where needed for different abilities, devices, and environments, aligned with WCAG’s POUR principles and inclusive design guidance captured in `ux-design-principles`.[web:280][web:283][web:293]

Use this skill whenever you design or review screens and flows, especially for core tasks, forms, navigation, and content-heavy experiences.

---

## Instructions

### Step 1: Clarify users, contexts, and risks

Start by understanding where accessibility and inclusion are most critical.[web:283]

Ask:

- "Who are the key users and what range of abilities, devices, and environments might they have?"
- "Are there regulatory or contractual accessibility requirements (e.g., WCAG level, region, industry)?"
- "Which tasks or flows are most critical if someone struggles or gets blocked?"

Summarize:

- Primary tasks and flows to focus on.
- Potential barriers (vision, motor, hearing, cognitive, language, environment).
- Any standards or guidelines the product aims to meet (e.g., WCAG 2.x AA, organizational standards).

Use `ux-mindset-problem-framing` and `ux-user-research` where available to ground this in real segments and contexts.[web:325]

---

### Step 2: Design for perceivability (contrast, typography, media)

Ensure that users can **perceive** information (WCAG’s “Perceivable”).[web:293][web:298]

For visual content:

- Use sufficient colour contrast between text and background, especially for body text and interactive elements (meet or exceed WCAG contrast ratios).[web:293]
- Avoid conveying meaning by colour alone (use text, icons, or patterns as well).
- Choose readable type:
  - Reasonable base font sizes.
  - Adequate line height and spacing.
  - Avoid long, dense blocks of text.

For images and media:

- Provide descriptive text for important images and icons where meaning is not obvious from context.
- Consider captions or transcripts for key video/audio content.
- Avoid auto-playing media with sound; if used, provide controls to pause/stop.[web:293]

Document any intentional exceptions and why (e.g., purely decorative elements) so implementation can set appropriate semantics (e.g., `aria-hidden`).

---

### Step 3: Support keyboard and alternative input

Design flows so users can navigate and operate them without a mouse (WCAG “Operable”).[web:293][web:298]

Consider:

- **Focus order**:
  - Ensure logical focus order follows the visual layout and task sequence.
- **Keyboard access**:
  - All major interactive elements (buttons, links, fields, menus, dialogs) should be reachable and operable via keyboard-equivalent inputs.
- **Focus indication**:
  - Ensure focus states are clearly visible; avoid removing outlines without a strong, accessible alternative.

Where you introduce custom components (e.g., custom dropdowns, modals, sliders), plan with engineering how they will be made keyboard- and screen-reader-friendly, referencing patterns and platform guidance from `ux-design-principles`.[web:236][web:260]

---

### Step 4: Use clear structure and semantics

Help assistive technologies and users understand the structure (WCAG “Robust”).[web:293][web:298]

- Use heading levels consistently to reflect hierarchy (H1, H2, H3, etc. at implementation time).
- Ensure forms have clear labels associated with their fields.
- Group related controls logically (e.g., within clearly labelled sections).
- Avoid layout that relies on visual positioning only; ensure the underlying structure makes sense linearly.

As a designer, specify:

- Which pieces of text should be headings vs body.
- Where landmarks/sections might be used (e.g., nav, main content, footer).
- Which elements are primary actions vs secondary.

Coordinate with `ux-information-architecture` so structural decisions and semantics tell a consistent story.[web:110]

---

### Step 5: Design inclusive interactions and flows

Anticipate diverse ways of interacting and thinking.[web:280][web:283]

Consider:

- **Motor constraints**:
  - Make hit areas reasonably large (align with touch target guidance in `ux-design-principles`).[web:278][web:284]
  - Avoid requiring precise gestures (e.g., tiny drag handles) for core tasks without alternatives.
- **Cognitive load**:
  - Simplify flows where possible; avoid unnecessary steps and choices.
  - Break complex tasks into smaller steps; provide clear context and progress indication.
- **Time**:
  - Avoid very short timeouts where possible, or provide ways to extend time.

For critical flows, check that there is a way to:

- Pause, stop, or adjust moving or auto-updating content where it might distract or overwhelm.
- Navigate back or recover from mistakes without starting from scratch (user control and freedom).[web:288]

Use `ux-interaction-design` to ensure interaction patterns remain accessible and do not rely solely on complex gestures or motion.

---

### Step 6: Write inclusive, clear copy

Ensure text does not create unnecessary barriers.[web:233][web:283]

Guidelines:

- Use clear, plain language where possible; explain domain-specific terms briefly when needed.
- Avoid idioms, sarcasm, or cultural references that may not translate or may confuse.
- Be respectful and people-focused in wording (people-first language where appropriate).
- Provide concrete instructions rather than vague guidance (“Enter a 6-digit code from your email” vs “Enter the code”).

Check that error messages and instructions are explicit enough to help users with different levels of literacy, experience, or language proficiency, and coordinate with `ux-writing-content` for patterns.[web:233]

---

### Step 7: Provide alternatives and fallbacks

Plan **alternative ways** to access content or complete tasks when standard interactions may not work for everyone.[web:283]

Examples:

- If complex charts or visualizations are critical, provide text summaries of key insights.
- For drag-and-drop interactions, provide equivalent “move up/down” or “add/remove” controls.
- For gesture-heavy mobile interactions, ensure there are visible controls that achieve the same outcomes.
- For time-based interactions, provide configurable durations or “remind me later” patterns.

Document the alternatives so that engineering and QA know what to implement and test, and so patterns can be codified into design systems (`ux-design-principles` / design-system skills).

---

### Step 8: Integrate accessibility checks into design reviews

Make accessibility a **regular part of design practice**, not a final checklist.[web:283]

For each design or flow review:

- Include a brief pass for:
  - Contrast and readability.
  - Clear focus and keyboard paths (at least conceptually).
  - Clear labels and instructions.
  - Obvious alternatives for custom interactions.
- Note any areas that require deeper engineering and QA checks.

Encourage team rituals where accessibility is a standing topic (e.g., a dedicated slide/section in design reviews) and use `ux-usability-heuristics` and `ux-design-principles` when a deeper heuristic or principles-based evaluation is needed.[web:288][web:260]

---

### Step 9: Capture issues and collaborate on fixes

When you spot accessibility or inclusivity issues:

- Log them with:
  - Location and context.
  - Description of the barrier.
  - Who is likely to be impacted.
  - Proposed design changes or alternatives.
- Work with:
  - Engineers to understand what is feasible and how patterns can be made more accessible.
  - QA to ensure accessible behaviours are covered by test plans.

Prioritize issues where:

- Core tasks are blocked.
- The impact on independence, dignity, or safety is high.
- Regulatory/compliance requirements apply.

Where appropriate, connect accessibility and inclusion work to metrics from `ux-product-design-metrics` (e.g., task success, error rate, support tickets, CSAT, CES) to demonstrate impact.[web:288][web:293][web:309]

---

## Examples

### Example 1: Accessible sign-up form

- Design decisions:
  - Clear labels for all fields, with helper text for tricky fields.
  - Sufficient contrast on text and buttons.[web:293]
  - Meaningful error messages placed near fields, with a summary at the top.
  - Focus order follows the visual layout; keyboard users can move through fields and submit.

### Example 2: Inclusive dashboard filters

- Design decisions:
  - Filters accessible via both mouse and keyboard, with clear focus states.[web:293]
  - Filter chips with text labels and icon + text combos instead of colour-only signals.
  - Complex data visualizations accompanied by short, plain-language summaries of key trends.

---

## Troubleshooting

### Design looks nice but is hard to read or use

- Check contrast and font sizes first; adjust to improve readability.[web:293]
- Reduce visual noise; simplify backgrounds behind text and controls.
- Revisit layout to ensure logical grouping and sufficient spacing.

### Accessibility feels overwhelming

- Start with critical flows and apply a small core checklist:
  - Can users see/read it?
  - Can users operate it without a mouse?
  - Is the structure and messaging clear?
- Add more detailed checks over time and rely on specialists or tools where needed.
- Use `ux-design-principles` as a reference for WCAG POUR and inclusive design principles.[web:280][web:293]

### Designers and engineers disagree on what’s “good enough”

- Anchor discussions in user impact and, where applicable, formal guidelines.
- Use simple examples or quick tests (e.g., try navigating only with a keyboard) to make issues concrete.
- Where trade-offs are necessary, document them and plan for future improvements.

---

## Notes for use with other skills

- Use this skill alongside:
  - `ux-interaction-design` to ensure patterns and behaviours are accessible (keyboard, focus, error handling).[web:240]
  - `ux-usability-heuristics` for deeper evaluation and prioritization of accessibility issues.[web:288][web:293]
  - UI and design system skills to update components and tokens for better accessibility by default.[web:210]
  - `ux-design-principles` as the foundation for inclusive design, WCAG POUR, platform guidelines, motion, and mobile accessibility.
  - `ux-product-design-metrics` to connect accessibility and inclusion improvements to metrics such as task success, error rate, support tickets, CSAT, CES, and retention.[web:303][web:288][web:309]
