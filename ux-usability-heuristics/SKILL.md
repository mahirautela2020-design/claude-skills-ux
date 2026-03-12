---
name: ux-usability-heuristics
description: >
  Plans and performs usability evaluations using heuristics, UX audits, and
  basic accessibility checks, then prioritizes issues and communicates them to
  product and engineering. Use when the user needs to review an experience for
  usability problems, structure findings, score severity, and propose actions
  based on impact and effort, aligned with shared UX principles and metrics.
metadata:
  domain: ux
  category: evaluation
  author: your-name
  version: 1.1.0
---

# UX Usability Evaluation & Heuristics

## Purpose

This skill helps systematically evaluate interfaces for usability and basic accessibility issues, using heuristic reviews and UX audits.[web:288][web:292] It guides you through defining scope, using a checklist or heuristics set, documenting issues clearly, prioritizing them by impact and effort, and communicating them effectively to product and engineering, while connecting to `ux-design-principles` for the canonical principles set and `ux-product-design-metrics` when findings tie to metrics.[web:260][web:303]

Use this skill when you want to assess an existing flow, prototype, or product area without running a full user study, or as a complement to user testing and analytics.

---

## Instructions

### Step 1: Define scope and context of the evaluation

Clarify what you are evaluating and why.[web:292]

Ask:

- "Which product, flow, or area do you want to evaluate?"
- "What are the most important tasks or journeys here?"
- "Are there specific issues or user complaints you already know about?"

Define:

- Scope (e.g., “checkout flow”, “billing settings”, “mobile onboarding”).
- Platforms/devices (web, mobile web, native apps).
- Primary user segments and tasks to focus on.

This keeps the evaluation focused and avoids trying to audit everything at once, and provides context for which metrics from `ux-product-design-metrics` are most relevant (e.g., task success, drop-off, CSAT, CES).[web:288][web:293]

---

### Step 2: Choose heuristic set and criteria

Select a **heuristic framework** and key criteria you will use.[web:288][web:297]

Use Nielsen’s 10 usability heuristics (referenced in `ux-design-principles`) as your core set:

- **Visibility of system status**  
  - The system keeps users informed about what’s happening (loading, saving, errors, success) in a timely, understandable way.
- **Match between system and the real world**  
  - Language, concepts, and formats match users’ mental models and domain language; avoid internal jargon.
- **User control and freedom**  
  - Users can easily undo or cancel actions, recover from mistakes, and navigate back without getting stuck.
- **Consistency and standards**  
  - Similar things look and behave similarly; patterns follow platform and product conventions.
- **Error prevention**  
  - Interfaces help users avoid mistakes (sensible defaults, constraints, confirmations for risky actions).
- **Recognition rather than recall**  
  - Users can see options and information when needed instead of remembering from previous screens.
- **Flexibility and efficiency of use**  
  - Frequent actions can be done efficiently (shortcuts, sensible defaults) without making first‑time use harder.
- **Aesthetic and minimalist design**  
  - Only relevant information is shown; screens are not overloaded or visually noisy.
- **Help users recognize, diagnose, and recover from errors**  
  - Error messages are clear, specific, and actionable; they appear close to where the problem happened.
- **Help and documentation (when needed)**  
  - Additional guidance is available for complex tasks, without forcing everyone to read long docs.[web:288][web:292]

Include basic accessibility considerations at this level:

- Sufficient colour contrast for text and important controls.
- Visible focus states and logical focus order for keyboard users.
- Descriptive text for links, buttons, and important icons.
- No reliance solely on colour to convey meaning.[web:293][web:298]

You can treat the heuristics, Gestalt principles, UX laws, and WCAG POUR in `ux-design-principles` as your extended checklist for deeper reviews when needed.[web:260][web:272][web:293]

Write down the list of heuristics and accessibility criteria you will apply so you can reference it consistently in your findings.

---

### Step 3: Walk through critical tasks and flows

Perform the evaluation **task by task**, not just page by page.[web:292]

For each key task (e.g., “create project”, “complete purchase”, “update password”):

- Start from the natural entry point for that task.
- Walk through the experience step by step as a user would.
- Interact with controls as intended:
  - Try primary paths.
  - Try some alternative paths where plausible.
- Observe:
  - Where you hesitate or feel unsure.
  - Where information is missing or unclear.
  - Where the design does not match expectations.

Take notes tied to specific screens and actions, and, where relevant, note which task-level metrics (task success, errors, time on task) from `ux-product-design-metrics` are likely affected.[web:288][web:303]

---

### Step 4: Identify and log usability and accessibility issues

As you walk through flows, **log issues** whenever a heuristic or criterion is violated.[web:292]

For each issue, capture:

- **Location** – screen, step, or component.
- **Description** – what happens and why it’s a problem from the user’s point of view.
- **Related heuristic(s)** – which principle(s) it violates.
- **Impact on users** – who is affected and how (confusion, slow-down, errors, inability to complete).
- **Accessibility note** (if applicable) – e.g., low contrast, missing labels, keyboard trap.

Example issue entry:

- Location: Checkout – payment step  
- Description: When card details are invalid, an error message appears at the top of the page only; fields with problems are not highlighted, so users must scan the entire form to guess what’s wrong.  
- Related heuristics: Visibility of system status; Help users recognize, diagnose, and recover from errors.  
- Impact: Major – likely to cause repeated failures and frustration for many users during a critical flow.  
- Accessibility: Error state relies on colour only; screen readers may not announce the issue clearly.

Keep descriptions factual and observable; avoid blaming users.

---

### Step 5: Include basic accessibility checks

Within the scope of this skill (awareness-level accessibility):[web:293][web:298]

- Check colour contrast visually and, if possible, with a basic tool.
- Check that:
  - Links and buttons have clear, descriptive labels.
  - Focus order follows a logical sequence.
  - Keyboard users can access major interactive elements and escape modals.
- Note any obvious problems with:
  - Text size and readability.
  - Reliance solely on colour to convey information.
  - Images/icons used without supporting text where meaning might be unclear.

Record accessibility issues alongside usability issues, marking them clearly so they can be routed appropriately, and consider using `ux-accessibility-inclusive-design` for deeper reviews.

---

### Step 6: Assess severity and impact

For each issue, assign a **severity rating** to help with prioritization.[web:292]

A simple scale:

- **Blocker** – prevents task completion or causes major errors.
- **Major** – often causes confusion, errors, or workarounds; significantly slows users.
- **Minor** – noticeable friction but users can still complete tasks.
- **Cosmetic** – mainly visual or polish issues; very low impact on task completion.

Also note:

- **Frequency** – how often the issue is likely to occur (for most users / some users / rare edge case).
- **Affected users** – which segments are most impacted (new users, power users, specific roles, assistive tech users, etc.).

Where possible, relate impact to metrics in `ux-product-design-metrics` (e.g., task success, error rate, abandonment, support tickets, CSAT) to help stakeholders see business relevance.[web:288][web:309][web:311]

This will be used later for impact × effort prioritization.

---

### Step 7: Propose fixes and patterns (at a high level)

For each issue, suggest **possible directions for improvement**, not final detailed designs.[web:292]

Examples:

- For unclear labels: propose clearer wording and alignment with IA terminology.
- For hidden actions: suggest moving actions to more standard positions or affordances.
- For over-cluttered screens: suggest reducing visual noise, grouping related elements, or using progressive disclosure.

Focus on:

- Simplifying and clarifying flows and interactions.
- Aligning with existing design system components and patterns.
- Reducing cognitive load and potential for errors.

Use `ux-design-principles` as the reference point for which laws, heuristics, or accessibility rules your proposed fix should satisfy (e.g., recognition over recall, error prevention, visibility of system status, inclusive design).[web:260][web:280][web:293]

You do not need to fully redesign; the aim is to give actionable guidance on what to explore in design.

---

### Step 8: Prioritize issues (impact × effort)

Help product and engineering decide what to tackle first using an **impact × effort** lens.[web:292]

For each issue:

- **Impact**: based on severity, frequency, and alignment with key tasks and business goals:
  - High / Medium / Low
- **Effort**: approximate relative implementation effort:
  - High / Medium / Low

Create a simple prioritization:

- **High impact, low/medium effort** → address first.
- **High impact, high effort** → consider as part of larger roadmap or redesign.
- **Medium impact, low effort** → quick wins when capacity allows.
- **Low impact, high effort** → likely de-prioritize.

If helpful, recommend grouping issues into **themes** (e.g., “error messaging”, “navigation clarity”, “form usability”) and prioritizing themes.

When prioritization needs to tie into product metrics, use `ux-product-design-metrics` (e.g., HEART, AARRR, GSM) to highlight which issues block or support key outcomes like activation, retention, or conversion.[web:303][web:308][web:313]

---

### Step 9: Produce a usability findings and recommendations summary

Create a concise, structured summary to share with stakeholders.[web:292][web:325]

Suggested structure:

1. **Overview**  
   - Scope and goals of the evaluation.  
   - Methods used (heuristic review, light accessibility check, flows covered).
2. **Key themes**  
   - 3–7 major categories of issues with short descriptions.
3. **Top issues**  
   - A table with: ID, location, description, severity, impact, suggested direction, and priority.
4. **Quick wins**  
   - Issues that are high impact and low effort.
5. **Larger opportunities**  
   - Issues or patterns that may require more significant design or technical work.
6. **Next steps**  
   - Recommended follow-up (e.g., design adjustments, further user testing, additional accessibility review).

Where relevant, explicitly note:

- Which **principles** from `ux-design-principles` are violated or addressed by recommended changes.
- Which **metrics** from `ux-product-design-metrics` should be monitored after fixes (e.g., improved task success, reduced abandonment, better CSAT/CSAT, fewer support tickets).[web:260][web:303][web:309]

Ensure the summary is understandable to non-design stakeholders and clearly links usability problems to user and business impact.

---

## Examples

### Example 1: Checkout flow heuristic review

- Scope: desktop checkout flow from cart to confirmation.
- Findings:
  - Several validation errors not clearly linked to fields.
  - Inconsistent naming of shipping options.
  - Low contrast for important price information.
- Prioritization:
  - High impact + low effort: improve error messaging and field highlighting (visibility of system status; error recovery).
  - Medium impact + medium effort: align shipping labels and restructure options (match with real world; consistency).
  - Medium/low impact + higher effort: colour contrast and typography adjustments in a future UI refactor (accessibility and visual hierarchy).

### Example 2: Settings area UX audit

- Scope: account and billing settings on web app.
- Findings:
  - Hard-to-find “cancel subscription” link buried in a non-obvious place.
  - Multiple similar pages with overlapping content; confusing IA.
  - No confirmation or clear feedback after major changes.
- Prioritization:
  - High impact, medium effort: restructure settings IA and surface important actions (findability; user control).
  - High impact, low effort: add clear success messages after saving important changes (visibility of status; feedback).

---

## Troubleshooting

### Too many issues, unclear where to start

- Group issues into themes (e.g., “forms and validation”, “navigation and labels”, “feedback and visibility of status”).
- Within each theme, highlight 1–3 highest-impact issues.
- Use impact × effort to create a short “must address next” list.

### Stakeholders disagree on severity

- Anchor severity in user and task impact, not personal preferences.
- Where disagreement persists, suggest a small, focused user test or A/B test to observe real behaviour and metrics (using `ux-prototyping-validation` and `ux-product-design-metrics`).[web:303][web:313]
- Be transparent about judgement calls and assumptions.

### Findings are ignored or lost

- Present summaries in a format that fits existing workflows (tickets, docs, slides).
- Link each issue to a concrete follow-up action (design task, engineering ticket, research question).
- Track whether issues are addressed over time and revisit major ones in later evaluations.

---

## Notes for use with other skills

- Use this skill:
  - Alongside `ux-prototyping-validation` to evaluate prototypes between design iterations.
  - With `ux-accessibility-inclusive-design` for deeper accessibility reviews beyond basic checks.[web:293][web:280]
  - Together with `ux-interaction-design` and UI skills to inform detailed changes to components and patterns.[web:240]
  - With `ux-design-principles` as the canonical source for heuristics, UX laws, and accessibility principles referenced in findings and recommendations.[web:260][web:272]
  - With `ux-product-design-metrics` and product experimentation skills when usability issues and fixes need to be tied to metrics like task success, conversion, retention, CSAT, CES, or NPS.[web:303][web:311][web:313]
