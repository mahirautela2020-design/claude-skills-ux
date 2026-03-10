---
name: ux-design-principles
description: >
  Foundations: UX laws and design principles. Use when you need to ground
  design, audits, and documentation in shared principles: 21 Laws of UX,
  usability heuristics, accessibility (POUR), Gestalt, cognitive, interaction,
  inclusive, atomic design, color, motion, web, and mobile/touch.
metadata:
  domain: foundations
  category: ux-principles
  author: your-name
  version: 1.0.0
---

# Foundations: UX Laws & Design Principles

This reference combines the 21 Laws of UX with core design, usability, accessibility, data visualization, motion, web, Gestalt, cognitive, interaction, inclusive, atomic, color, and mobile/touch principles.[web:260][web:288][web:293][web:294][web:295][web:296][web:272][web:280][web:210][web:230][web:278] Use it to ground design work, audits, and documentation in industry‑standard concepts.

---

## 1. Core Design Principles (Visual/UI)

High‑level principles for making interfaces clear, coherent, and effective.[web:230][web:301]

### 1.1 Hierarchy

Organize information so users can quickly see what matters most.

- Emphasize primary actions and content through size, weight, color, and placement.
- Use heading levels, grouping, and spacing to create clear levels of importance.

### 1.2 Contrast

Use contrast to differentiate elements and guide attention.[web:230]

- Apply contrast in color, size, weight, and shape to separate content and controls.
- Ensure contrast also meets accessibility requirements for legibility.[web:293]

### 1.3 Alignment & Grid

Align elements to an underlying grid for structure and order.[web:296][web:301]

- Use consistent margins, columns, and baselines.
- Avoid arbitrary alignment that creates visual noise.

### 1.4 Proximity & Grouping

Group related items together and separate the unrelated.

- Place related content near each other with smaller gaps.
- Use larger gaps and separators between distinct groups.

### 1.5 Consistency

Make similar things look and behave the same.[web:290][web:301]

- Standardize typography, colors, component styles, and interaction patterns.
- Keep patterns consistent across pages and platforms.

### 1.6 Simplicity & Minimalism

Remove anything that does not support user goals.[web:292]

- Avoid unnecessary decoration, redundant copy, and duplicate controls.
- Prefer one clear way to do something over many confusing options.

### 1.7 Feedback & Status

Make system status visible at all times.[web:288]

- Show loading, saving, errors, and success in context.
- Use subtle but noticeable feedback for interactions.

### 1.8 Responsiveness & Adaptability

Design for different screen sizes, densities, and contexts.[web:296][web:301]

- Use responsive layouts that reflow content gracefully.
- Optimize for both desktop and mobile, including touch interactions.

---

## 2. Usability Principles (Nielsen’s Heuristics)

Jakob Nielsen’s 10 heuristics are widely used usability principles.[web:288][web:289][web:302]

1. **Visibility of system status** – Keep users informed about what is happening.
2. **Match between system and the real world** – Use users’ language and familiar concepts.
3. **User control and freedom** – Provide undo, redo, cancel, and exits from unwanted states.
4. **Consistency and standards** – Follow platform conventions and internal consistency.
5. **Error prevention** – Design to avoid problems before they occur.
6. **Recognition rather than recall** – Keep options visible; avoid forcing memory.
7. **Flexibility and efficiency of use** – Support shortcuts and expert use without harming novices.
8. **Aesthetic and minimalist design** – Remove irrelevant information and clutter.
9. **Help users recognize, diagnose, and recover from errors** – Clear, specific, constructive error messages.
10. **Help and documentation** – Provide accessible, concise support for complex flows.

Use these as a default checklist in reviews and UX audits.[web:288][web:292]

---

## 3. Accessibility Principles (WCAG POUR)

Accessibility is organized around four WCAG principles: **Perceivable, Operable, Understandable, Robust (POUR)**.[web:298][web:293]

### 3.1 Perceivable

Information and UI components must be presented in ways that users can perceive.

- Provide text alternatives for non‑text content.
- Ensure sufficient color contrast and scalable text.[web:293]
- Do not rely on color alone to convey meaning.

### 3.2 Operable

Components and navigation must be usable via different input methods.[web:298]

- Make all functionality available via keyboard.
- Provide enough time for tasks; avoid unexpected timeouts.[web:293]
- Avoid content that causes seizures (e.g., fast flashing).[web:293]

### 3.3 Understandable

Content and operation must be easy to understand.[web:298]

- Use clear language and predictable navigation.
- Provide helpful, specific errors and instructions.
- Avoid unexpected context changes (e.g., navigation on focus).

### 3.4 Robust

Content must work reliably with a range of technologies.[web:298]

- Use semantic HTML and ARIA responsibly.
- Ensure compatibility with assistive technologies.
- Avoid patterns that break standard focus and reading order.

---

## 4. Twenty‑One Laws of UX

Laws of UX describe common patterns in behavior and perception applied to interfaces.[web:260][web:263][web:265]

### 4.1 Aesthetic–Usability Effect

People perceive attractive designs as more usable.[web:265]

- Use clean, coherent visual design to increase perceived ease of use.
- Do not let aesthetics hide serious usability or accessibility issues.

### 4.2 Doherty Threshold

Interaction feels fluid when response times are under ~400 ms.[web:265][web:262]

- Provide visible feedback or skeleton states if operations take longer.
- Prioritize performance on critical user journeys.

### 4.3 Fitts’s Law

Larger and closer targets are faster and easier to hit.[web:265][web:262]

- Increase size and spacing of primary targets, especially on touch devices.
- Separate destructive actions from primary actions.

### 4.4 Goal‑Gradient Effect

Users work harder as they feel closer to a goal.[web:265]

- Use clear progress indicators and show steps completed.
- Highlight how much is left to finish a task.

### 4.5 Hick’s Law

Decision time grows with number and complexity of choices.[web:265][web:262]

- Reduce or group options; use progressive disclosure.
- Provide defaults and recommended paths.

### 4.6 Jakob’s Law

People expect your product to behave like others they know.[web:265][web:262]

- Align with familiar web and app patterns.
- Only diverge when there is a clear, validated improvement.

### 4.7 Law of Common Region

Elements in the same bounded area are perceived as grouped.[web:265][web:272]

- Use cards and panels to group related content.
- Avoid mixing unrelated items in one region.

### 4.8 Law of Proximity

Items close together are perceived as related.[web:274][web:279]

- Group related labels, inputs, and messages.
- Use spacing to separate different groups.

### 4.9 Law of Prägnanz (Simplicity)

People prefer simpler, more regular shapes and organization.[web:272][web:275]

- Structure layouts to make the simplest interpretation obvious.
- Avoid unnecessary complexity in composition.

### 4.10 Law of Similarity

Visually similar elements appear related.[web:272][web:279]

- Style similar actions and statuses consistently.
- Differentiate elements that serve different purposes.

### 4.11 Law of Uniform Connectedness

Visually connected elements are seen as a group.[web:276][web:279]

- Connect related items using lines, backgrounds, or connectors.
- Avoid connecting unrelated items.

### 4.12 Miller’s Law

Working memory can hold only a limited number of items.[web:262][web:267]

- Chunk content into small groups.
- Avoid long, unstructured lists of options.

### 4.13 Occam’s Razor

Among equivalent solutions, the simplest is preferable.[web:262][web:265]

- Prefer fewer steps and fewer concepts when possible.
- Remove features that do not materially help users.

### 4.14 Pareto Principle (80/20 Rule)

Most value comes from a small portion of features.[web:265]

- Identify and optimize key journeys and functions.
- Avoid over‑engineering rarely used features.

### 4.15 Parkinson’s Law

Work expands to fill available time or space.[web:265][web:262]

- Use constraints (time, space, scope) to focus user input.
- Avoid unlimited, unstructured fields when more guidance is better.

### 4.16 Peak–End Rule

People judge experiences by their peak and ending moments.[web:265][web:263]

- Design for strong, positive peaks and clear, satisfying endings.
- Ensure confirmation and success states are especially clear and supportive.

### 4.17 Postel’s Law

Be lenient in what you accept; strict in what you output.[web:261][web:267]

- Accept varied input formats and normalize them.
- Output clean, consistent values in the UI.

### 4.18 Serial Position Effect

First and last items in a sequence are remembered best.[web:279][web:262]

- Place key options at the beginning or end of menus and lists.
- Avoid hiding critical actions in the middle.

### 4.19 Tesler’s Law (Conservation of Complexity)

Every system has irreducible complexity; you can only shift it.[web:265][web:267]

- Move complexity from users into smart defaults and system logic where possible.
- Provide advanced options without forcing everyone to use them.

### 4.20 Von Restorff Effect (Isolation Effect)

Distinct items are more likely to be noticed and remembered.[web:279][web:262]

- Make primary actions and warnings visually distinctive.
- Use contrast and uniqueness to highlight key information.

### 4.21 Zeigarnik Effect

Unfinished tasks are more memorable than completed ones.[web:262][web:263]

- Use visible “draft” or “incomplete” indicators.
- Provide cues and reminders to resume important tasks.

---

## 5. Gestalt Principles

Laws of visual perception that explain grouping and organization.[web:272][web:276][web:279]

- **Proximity** – Close items are perceived as a group.[web:274]
- **Similarity** – Similar items (color, shape, size) appear related.[web:272]
- **Closure** – People complete incomplete shapes mentally.[web:275]
- **Continuity** – The eye follows continuous lines and paths.[web:276]
- **Figure/Ground** – People distinguish foreground from background.[web:272]
- **Common Fate** – Elements moving together appear related.[web:276]
- **Symmetry & Order** – Symmetrical, ordered layouts feel stable and harmonious.[web:279]
- **Common Region** – Elements in the same bounded area are seen as grouped.[web:276]

Use combinations of these to create clear structure and scannable layouts.

---

## 6. Cognitive Psychology Principles

Behavioral principles that affect how users think, remember, and decide.[web:262][web:238]

- **Reduce cognitive load** – Limit simultaneous choices, chunk content, and sequence tasks.
- **Recognition over recall** – Keep options visible instead of requiring memory.[web:288]
- **Match mental models** – Mirror real‑world concepts and workflows.[web:238]
- **Externalize memory** – Use histories, breadcrumbs, saved filters, and visible context so users don’t have to remember everything.

(Effects like Von Restorff, Zeigarnik, Serial Position, Peak–End, and Doherty are covered in the Laws section.)

---

## 7. Interaction Design Principles

Fundamental principles of how users interact with interfaces.[web:240][web:243]

- **Affordances & Signifiers** – Controls suggest use; signifiers make interaction possibilities clear.
- **Feedback & Response** – Every action gets timely, perceivable feedback.[web:243]
- **Constraints & Forcing Functions** – Prevent invalid or dangerous actions.[web:240]
- **Natural Mapping** – Align controls with their effects intuitively.
- **Consistency & Standards** – Follow platform norms and internal patterns.[web:288]
- **Discoverability & Visibility** – Make important actions easy to find.
- **Error Prevention** – Design flows to avoid errors rather than just handling them.[web:288]
- **Direct Manipulation** – Let users act directly on objects where possible.[web:240]
- **Recognition Over Recall** – Present relevant options in context.[web:288]

---

## 8. Inclusive Design Principles

Design for diversity in ability, context, and situation.[web:280][web:283]

- **Recognize Exclusion** – Identify who is left out when designing from a narrow perspective.[web:280]
- **Learn from Diversity** – Treat people living with constraints as experts in adaptation.[web:280]
- **Solve for One, Extend to Many** – Solutions for specific disabilities often help everyone.[web:286]
- **Persona Spectrum** – Consider permanent, temporary, and situational disability.[web:277]
- **Provide Comparable Experience** – Ensure users can complete tasks in ways that work for them.[web:283]
- **Consider Situation & Context** – Design for varied environments (noise, light, bandwidth).[web:283]
- **Be Consistent & Predictable** – Reduce cognitive load with stable patterns.[web:283]
- **Give Users Control** – Respect preferences and provide adjustable experiences.[web:280]

---

## 9. Atomic Design & Component Principles

From Brad Frost’s atomic design to component APIs and documentation.[web:210]

- **Atoms** – Smallest units (buttons, inputs, labels, icons).
- **Molecules** – Simple combinations (search bar, labeled input with error).
- **Organisms** – Larger structures (headers, cards, comment threads).
- **Templates** – Page‑level layouts that place organisms.
- **Pages** – Templates with real content and data.

Component‑level principles:

- **Component API Design** – Design props, slots, and events that are clear, flexible, and hard to misuse.
- **Component Composition** – Build complex UIs by composing focused components, not monoliths.
- **Variants & Polymorphism** – Support size, style, and behavioral variants; allow semantic flexibility when needed.
- **Component Documentation** – Provide usage examples, props, accessibility guidance, and do’s/don’ts.

---

## 10. Color Theory & Application

Using color effectively in interfaces.[web:230][web:236][web:239]

- **Color Psychology & Emotion** – Align palette with brand personality and user expectations.
- **Color Harmonies & Relationships** – Use simple, coherent schemes for balance.[web:230]
- **Semantic Color Systems** – Define tokens for primary, neutral, and status colors.
- **Contrast & Accessibility** – Meet WCAG contrast ratios for text and key UI elements.[web:293]
- **Colorblindness Considerations** – Do not rely on color alone; pair with icons/labels.[web:239]
- **Brand Color & Identity** – Use brand colors consistently for recognition.[web:230]
- **Dark Mode & Theming** – Base themes on tokens; validate contrast and depth cues in each theme.
- **Cultural Color Meanings** – Check color choices against cultural contexts.
- **Scalable Color Systems** – Use systematic scales (e.g., 50–900) behind functional tokens.
- **Color in Data Visualization** – Use color to highlight data and categories, not as decoration.[web:294]

---

## 11. Data Visualization Principles

Principles for clear, honest, and effective charts.[web:294][web:299]

- **Show the Data** – Above all else, make the data itself visible and legible.
- **Maximize Data‑Ink Ratio** – Prioritize marks that represent data; reduce non‑data ink.[web:299]
- **Minimize Chartjunk** – Avoid unnecessary 3D effects, gradients, and decoration.[web:294][web:299]
- **Graphical Integrity** – Ensure visuals faithfully represent the underlying data (no misleading axes).[web:299]
- **Choose the Right Chart** – Use chart types that match the question (trend, comparison, distribution).[web:294]
- **Consistent Scales & Encodings** – Keep axis scales and encodings consistent across related charts.
- **Highlight Signal** – Use color, annotation, and emphasis to draw attention to key points.
- **Context & Annotation** – Provide labels, units, and context so users can interpret correctly.
- **Accessibility** – Ensure color contrast, alternative descriptions, and readable text in visuals.[web:293]

---

## 12. Motion Design Principles

Motion as a tool for clarity, not decoration.[web:295][web:300]

- **Purposeful Motion** – Every animation should support usability (orientation, feedback, hierarchy).  
- **Expectation** – Motion should match what users expect when they interact.[web:300]
- **Continuity** – Animate transitions to preserve spatial and conceptual continuity.[web:300]
- **Timing & Duration** – Use brief, tuned durations; avoid slow, blocking animations.[web:295]
- **Easing** – Use natural easing curves (ease‑in‑out) that feel physical, not mechanical.[web:295]
- **Hierarchy & Focus** – Use motion to direct attention to the most important elements.[web:295]
- **Feedback & State Change** – Animate state changes (expand, collapse, loading, success) to make them clear.[web:300]
- **Interruptibility** – Let users interrupt or skip animations when they act again.[web:295]
- **System Coherence** – Maintain a consistent motion language across the product.[web:300]
- **Accessibility & Comfort** – Respect reduced‑motion preferences and avoid motion that can cause discomfort.[web:293]

---

## 13. Web Design Principles

Core principles for modern, responsive web experiences.[web:296][web:301]

- **Responsive Layouts** – Use fluid grids and flexible media so content adapts to device size.[web:296]
- **Mobile‑First** – Design from small screens up, then enhance for larger screens.[web:301]
- **Performance** – Optimize assets, minimize blocking scripts, and design for fast load times.[web:301]
- **Clear Navigation** – Provide predictable, consistent navigation structures.[web:301]
- **Content Priority** – Surface critical content and actions above the fold where possible.
- **Consistency & Branding** – Maintain a uniform visual language that aligns with brand identity.[web:301]
- **Readable Typography** – Use appropriate sizes, line lengths, and line heights for readability.[web:296]
- **Accessible Interactions** – Ensure keyboard, screen reader, and touch accessibility.[web:293]
- **Error Handling & Empty States** – Design informative, supportive states for errors and no‑content cases.
- **Security & Trust Cues** – Clearly show security, privacy, and trust indicators where relevant.

---

## 14. Mobile & Touch Design Guidelines

Guidelines for comfortable, accessible touch interfaces.[web:278][web:281][web:284]

- **Minimum Touch Target Size** – Aim for at least 44 × 44 pt on iOS and 48 × 48 dp on Android.[web:278][web:281]
- **Thumb Zones & Reachability** – Place frequent actions in reachable zones, especially lower areas.
- **Safe Areas & Notches** – Respect platform safe area insets to avoid obscured content.
- **Standard Gesture Patterns** – Use platform‑standard gestures; never block system gestures.
- **Contextual Keyboards** – Use input types that trigger the right keyboard (email, number, tel, URL).
- **Orientation & Screen Flexibility** – Support portrait and landscape where appropriate; adapt layouts.
- **Haptic Feedback** – Use subtle haptics to confirm key actions without overwhelming.[web:278]
- **Mobile Performance & Loading** – Optimize for variable network conditions; prioritize critical content.
- **Readable Text Sizes** – Use at least ~16 px body text; respect system text scaling.[web:278]
- **Mobile Navigation Patterns** – Use bottom tabs for primary destinations; use drawers/menus for secondary navigation.[web:236]

---

This document can serve as your canonical “Foundations: Principles” reference for tools, audits, and stakeholder education.
