---
name: ux-interaction-design
description: >
  Designs interaction behaviour for digital products. Use when the user needs
  help defining states, edge cases, error and empty flows, microinteractions,
  and system feedback, or when choosing appropriate interaction patterns and
  balancing simplicity vs control. Covers task-focused interaction design
  grounded in user needs, platform conventions, and usability best practices,
  and aligned with shared UX principles and metrics.
metadata:
  domain: ux
  category: interaction
  author: your-name
  version: 1.1.0
---

# UX Interaction Design & Behavior

## Purpose

This skill helps define how users and the system interact over time: what happens on each step, how controls behave, how states change, and how feedback is communicated.[web:240][web:243] It focuses on task-centric interaction design, including states, edge cases, errors, and patterns that match user expectations while keeping complexity manageable, and leverages `ux-design-principles` for heuristics, laws, and platform guidance plus `ux-product-design-metrics` when interaction changes need to be measured.[web:260][web:303]

Use this skill when you need to design or refine flows and screens beyond static layouts: deciding interactions, handling edge cases, and specifying detailed behaviour for implementation.

---

## Instructions

### Step 1: Clarify the core task and context

Before specifying interactions, clarify the **task**, **context**, and **constraints**.

Ask:

- "What is the primary task or set of tasks this flow must support?"
- "Who is the user in this scenario (persona/segment) and what are they trying to achieve?"
- "On which platforms/devices will this interaction run (web, mobile, desktop)?"

Summarize:

- Core task(s) and success criteria
- Target users and context (frequency, urgency, risk)
- Platforms and any major technical or policy constraints

This anchors interaction decisions in actual user goals and environment, and sets up later metric choices from `ux-product-design-metrics` (e.g., task success, time on task, error rate).[web:288][web:303]

---

### Step 2: Identify key steps and decision points

Outline the **logical steps** and decisions in the flow (building on IA and user flows if available).[web:110]

For the chosen task:

- List steps from start to completion.
- Note decision points (e.g., “user chooses plan type”, “system validates payment”).
- Mark where user input is required vs where the system acts automatically.

Represent it as a simple sequence, for example:

- Step 1: User lands on [entry screen]
- Step 2: User chooses [option A/B/C]
- Step 3: System [validates / fetches / calculates]
- Step 4: User confirms / edits
- Step 5: System finalizes and shows result

This will guide which interactions need detailed behaviour and states and can later be tied to metrics like completion rate and drop-off as defined in `ux-product-design-metrics`.[web:303][web:308]

---

### Step 3: Define control types and interaction patterns

Choose interaction patterns and controls that are appropriate for the task, platform, and mental model.[web:240][web:243]

For each step or decision:

- Decide how users will act:
  - Click/tap vs drag-and-drop vs keyboard input vs gestures
  - Single primary action vs multiple secondary actions
- Choose control types:
  - Buttons vs links vs icons (and when each is appropriate)
  - Radio buttons vs checkboxes vs dropdowns vs segmented controls
  - Steppers, sliders, toggles, date pickers, etc.

Apply guidelines (drawing from `ux-design-principles`):

- Prefer simple, well-known patterns and platform conventions before inventing custom interactions (Jakob’s Law, consistency).[web:260][web:288]
- Avoid overloading a single control with many meanings.
- Ensure there is a clear primary action on each screen and that destructive or risky actions are clearly differentiated (e.g., styling, confirmation, Von Restorff effect).[web:260]

Document for each control:

- Purpose (what it does)
- Type and label
- When it is enabled/disabled
- Any shortcuts or accelerators (e.g., keyboard, bulk actions) if relevant

---

### Step 4: Specify states for key components and screens

Interaction design requires clear handling of **states**.[web:240]

For important components and screens, define:

- **Idle / default** – initial state before user interaction
- **Hover / focus / active** (where applicable)
- **Loading / in-progress**
- **Success / done**
- **Empty states** – when there is no data yet
- **Error states** – when something goes wrong
- **Disabled / unavailable**

For each state:

- Describe what the user sees (visual cues, text, icons).
- Describe what the user can and cannot do.
- Note transitions: what triggers entry and exit from the state.

Example:

- Button “Submit”:
  - Default: enabled, label “Submit”.
  - Loading: disabled, spinner shown, label “Submitting…”.
  - Success: reverts to default or navigates to confirmation view.
  - Error: remains visible; error message shown near field or at top.

Ensure states respect accessibility and inclusive design guidance from `ux-design-principles` (e.g., clear focus states, non-color-only cues).[web:293][web:280]

---

### Step 5: Design error handling and recovery flows

Define how the system handles **errors and failures**, not just the happy path.[web:288]

Consider:

- **Validation errors** (user input issues):
  - What is validated on change vs on submit.
  - How errors are surfaced (inline messages, summaries, field highlights).
  - How to phrase messages (clear, specific, actionable).
- **System errors** (network, server, unknown):
  - What users see if a request fails or times out.
  - Whether and how they can retry.
  - Fallback behaviour if data is partially available.

For each likely error scenario:

- Describe the error condition.
- Describe what the user sees (message, visual cues).
- Describe how they recover:
  - Fix input and retry
  - Try again later
  - Contact support / follow alternative path

Follow heuristics from `ux-design-principles` around error prevention, error messages, and help & documentation.[web:288]

Make sure error handling doesn’t trap users; there should be clear paths back to safety or alternatives.

---

### Step 6: Account for edge cases and constraints

Consider **edge cases** and less common scenarios that might break the experience.[web:243]

Ask:

- "What happens if there is no data yet?"
- "What if there is a very large amount of data?"
- "What if the user loses connectivity mid-flow?"
- "What if the user has partial permissions or restricted access?"

For each edge case:

- Define what is shown (e.g., empty state with guidance, truncated lists with “show more”, permission messages).
- Specify which actions are hidden vs shown but disabled, and why.
- Ensure that the interaction remains understandable and doesn’t leak technical complexity unnecessarily.

Balance simplicity with control:

- Hide complexity by default but provide advanced options where needed for power users, clearly separated and explained (Tesler’s Law).[web:260]
- Avoid forcing all users into complex flows just to support rare edge cases.

---

### Step 7: Define system feedback and microinteractions

Specify how the system **responds** to user actions to communicate status and outcomes.[web:240][web:295]

For each key interaction (submit, save, upload, navigation change, destructive action):

- Define feedback type:
  - Immediate inline feedback (e.g., field turns valid/invalid).
  - Toasters/snackbars or banners for transient messages.
  - Dialogs for confirmations or critical errors.
  - Progress indicators (spinners, skeletons, progress bars).
- Define timing:
  - How quickly feedback appears after an action (consider the Doherty Threshold).[web:260]
  - How long transient messages remain visible.
- Define motion/animation (if any):
  - Simple, purposeful transitions (e.g., expanding/collapsing sections, sliding panels).
  - Avoid overly flashy or long animations that slow down tasks or conflict with reduced-motion preferences (see `ux-design-principles` motion and accessibility sections).[web:295][web:293]

Ensure feedback answers the user’s key questions:

- Did my action work?
- What is happening now?
- What should I do next?

---

### Step 8: Pattern selection and consistency

Choose and document patterns so similar problems are solved in similar ways.[web:243]

For recurring needs:

- Selection patterns (radio vs checkbox vs dropdown).
- Navigation patterns (tabs vs side nav vs breadcrumbs).
- Data manipulation patterns (inline edit vs edit forms vs modals).
- Confirmation patterns (inline messages vs dialogs vs undo).

For each pattern, note:

- When to use it.
- When **not** to use it.
- How it behaves across breakpoints or platforms.

Aim to reuse patterns from your design system and the platform guidelines captured in `ux-design-principles` (web, iOS, Android) before inventing new ones.[web:236][web:260] Only introduce new patterns when they provide clear, user-centred benefits and can be explained simply.

---

### Step 9: Create interaction specs for delivery

Produce clear interaction specifications that development and QA can use.

For each key flow or screen:

- Provide:
  - Step-by-step description of interactions (what user does, what system does).
  - State definitions for important components.
  - Error and edge-case handling.
  - Feedback and transitions.

You can express this as:

- Annotated screenshots or wireframes.
- A table listing:
  - Trigger (user/system action)
  - Condition (if any)
  - Result (state change, navigation, feedback)
- References to reusable patterns or components in your design system.

Where interaction changes are tied to outcomes, reference `ux-product-design-metrics` for relevant measures (e.g., task success rate, time on task, error rate, CES, engagement).[web:288][web:303]

Ensure that specs are easy to scan and update; avoid burying critical behaviour in long paragraphs.

---

## Examples

### Example 1: Form submission flow

- Core task: submit a multi-step application form.
- Interaction design:
  - Progressive disclosure: show sections step by step to reduce cognitive load.
  - Inline validation: validate required fields on blur and show errors with actionable messages.
  - States:
    - Draft, In progress, Submitted, Needs attention (if partial data).
    - Button states: Default, Loading, Disabled (when invalid).
  - Errors:
    - Network failure: non-blocking banner with retry.
    - Validation errors: field-level messages plus summary at top.
  - Feedback:
    - Success screen summarizing submitted data and next steps.
    - Email confirmation sent asynchronously.

### Example 2: Table with bulk actions

- Core task: manage many items at once (e.g., select and archive multiple records).
- Interaction design:
  - Pattern: checkbox selection column with “select all” and bulk action bar appearing when items selected.
  - States:
    - No selection: bulk bar hidden.
    - Some selected: bulk bar visible, actions enabled.
    - All selected: “select all” reflects state.
  - Edge cases:
    - Large datasets: selection persists across pages with clear messaging.
    - Limited permissions: some bulk actions disabled with explanations.
  - Feedback:
    - After actions, show status message (e.g., “12 items archived”) with an optional undo.

---

## Troubleshooting

### Interaction is too complex

- Identify unnecessary steps or controls and remove them (Occam’s Razor).[web:260]
- Group related actions into simple flows.
- Defer advanced options behind clear affordances (“Advanced settings”).

### Users miss key actions

- Check visual hierarchy and placement of primary actions (coordinate with layout skill and `ux-design-principles` on hierarchy and contrast).[web:230]
- Improve affordances (button styling, labels, icon + text).
- Consider progressive disclosure: only show some actions when relevant.

### Inconsistent behaviour across screens

- Audit flows for similar interactions implemented differently.
- Choose a single pattern and update specs to align.
- Link interaction decisions to design system components and platform guidelines where possible.[web:236]

---

## Notes for use with other skills

- Use this skill in combination with:
  - `ux-information-architecture` to ensure interactions align with structure and navigation.
  - `ux-design-principles` to ground decisions in laws of UX, heuristics, inclusive design, motion, and platform patterns.[web:260][web:272]
  - UI and design system skills to ensure visual treatments support the intended interactions.
  - `ux-product-design-metrics` and product experimentation skills when interaction changes are tested for impact on key metrics (e.g., task success, conversion, retention, satisfaction).[web:303][web:313]
