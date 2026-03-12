---
name: ux-mindset-problem-framing
description: >
  Guides UX teams to frame the right problem before solutioning. Use when the
  user has a vague or solution-focused request like "redesign this page",
  "improve onboarding", "fix drop-off", or "increase conversion" and needs to
  clarify the real user problem, context, constraints, and success criteria.
  This skill helps pause solutioning, gather context, surface assumptions,
  draft user-centred problem statements, create How Might We questions, and
  define measurable outcomes aligned with design-thinking best practices.
metadata:
  domain: ux
  category: foundations
  author: your-name
  version: 1.1.0
---

# UX Mindset & Problem Framing

## Purpose

This skill ensures you are solving the **right** problem by deliberately framing the problem space before exploring solutions.[web:319][web:325] It draws on design thinking practices (Define stage, problem statements, How Might We questions), UX discovery guidance, and connects to shared foundations for principles and metrics via `ux-design-principles` and `ux-product-design-metrics`.[web:260][web:303]

Use this skill whenever a request is vague, solution-first, or business-metric-only, and you need a clear, user-centred problem definition and agreed success criteria before research, ideation, or UI work begins.

---

## Instructions

### Step 1: Pause solutions and clarify intent

1. If the request starts with a solution (e.g., "redesign checkout", "change the button", "add a new feature"), explicitly pause solutioning.  
2. Explain that you will first clarify the problem so that any later design work better targets real user needs and business outcomes.

Ask clarifying questions such as:

- "What motivated this request right now?"
- "What is not working today from your perspective?"
- "If this project is successful, what will be different for users and for the business?"

Write a short 2–3 sentence summary of the initial intent in plain language and confirm it with the user.

---

### Step 2: Understand context and constraints

Collect the minimum context needed to frame the problem well.

Ask about:

- **Product / service**: What it does, who it’s for, where this problem sits in the journey.
- **Target users**: Segments, roles, key tasks, environments.
- **Current experience**: Where and how the issue shows up (flows, touchpoints, channels).
- **Constraints**: Time, budget, tech stack, markets, compliance, legacy systems.
- **Existing inputs**: Any research, analytics, support tickets, prior experiments, or stakeholder opinions.

Summarize context in a compact structure, for example:

- Product / area:
- Users / segments:
- Journey stage / touchpoints:
- Existing evidence:
- Key constraints:

---

### Step 3: Surface assumptions and multiple perspectives

Good problem framing makes assumptions explicit and shows where different parties see the problem differently.[web:325]

Ask:

- "What do stakeholders currently believe is causing this problem?"
- "What are we assuming about user behaviour or needs that might be wrong?"
- "Who disagrees about the problem, and what is their view?"

Then:

- List assumptions grouped by **User**, **Business**, **Technology / Operations**.
- Mark each as **Fact**, **Assumption**, or **Unknown / needs validation**.

Highlight high-risk assumptions (high impact if wrong, currently unvalidated) as candidates for research later.

---

### Step 4: Describe symptoms and evidence

Separate symptoms from underlying problems.

Collect:

- **Symptoms** – observable issues (e.g., “users abandon basket at payment step”, “NPS for onboarding dropped in last quarter”).
- **Evidence** – supporting data: analytics, research findings, quotes, support logs, operational metrics.

Organize them in a small table-style structure:

- Symptom
- Evidence / source
- Severity (high / medium / low)
- Confidence (high / medium / low)

Call out where evidence is lacking and note “needs research or data pull”.

---

### Step 5: Draft user-centred problem statements

Use established UX/design-thinking patterns to turn observations into clear, human-centred problem statements.[web:325]

Offer at least one of these templates:

1. **User–job format**  
   - “[User/segment] needs to [goal] but [barrier] because [root cause], which leads to [impact].”

2. **Discovery problem statement**  
   - “We have observed [symptom] for [user/segment] in [context], which causes [impact]. We believe this happens because [suspected causes].”

3. **JTBD “struggling moment” format**  
   - “When [situation], [user] struggles to [goal] because [barrier]. As a result, [negative outcome].”

Create 1–3 candidate problem statements that:

- Focus on user needs and experience.
- Reference concrete evidence or acknowledged gaps.
- Avoid embedding specific solutions (no “redesign the page” or “add feature X” inside the statement).

Ask which statement (or combination) best reflects the challenge.

---

### Step 6: Create “How Might We” questions

Translate chosen problem statements into open, solution-agnostic opportunity questions.

Use the pattern:

- “How might we [enable positive change] for [specific users] so that [desired outcome]?”

Guidelines:

- Keep questions human-centred (focus on users, not only business KPI).
- Avoid locking into a specific solution or UI element.
- Aim for a scope that is neither too broad (“improve the entire experience”) nor too narrow (“change the colour of the button”).

Generate 3–6 HMW statements, then select 1–3 that are most important and actionable.

---

### Step 7: Define success metrics and signals

Clarify how the team will know if they solved the right problem.[web:303][web:308]

Use `ux-product-design-metrics` as the canonical source for metrics and frameworks, and pick from:

- **Task performance metrics** – task success rate, time on task, error rate, learnability for the key journeys.[web:288]
- **Behavioral metrics** – engagement, retention, feature adoption, bounce rate, pages/screens per session where relevant.[web:306]
- **Attitudinal metrics** – SUS, NPS, CSAT, CES, or targeted satisfaction questions.[web:311]
- **Business impact metrics** – conversion rate, cart abandonment, revenue per user, support ticket volume for this problem area.[web:309][web:301]

Optionally frame metrics using:

- **HEART** – Happiness, Engagement, Adoption, Retention, Task Success for the specific flow.[web:303][web:311]
- **GSM (Goals–Signals–Metrics)** – write 1–2 goals, list observable signals, then choose concrete metrics from the categories above.[web:308][web:316]

Ask questions like:

- “If we come back in 3–6 months, what would tell you this problem was solved well?”
- “Which existing metrics or dashboards can we align to this problem?”

Record 2–3 concrete, measurable success criteria aligned with the problem statement and HMW questions.

---

### Step 8: Capture scope, constraints, and risks

Frame the boundaries around the problem space.

Document:

- **In scope** – users, flows, platforms, and parts of the experience this work covers.
- **Out of scope** – what will not change, or will be handled separately.
- **Non-negotiables** – compliance, brand, technical/legal constraints that must be respected.
- **Risks and dependencies** – areas where timelines, resources, or other teams may impact the work.

Summarize in a simple list or table that can be pasted into a brief or ticket.

---

### Step 9: Produce a problem-framing summary and next steps

Produce a concise summary that can be used as a foundation for research, ideation, and prioritization.[web:325]

Suggested sections:

1. **Context** – product, users, journey stage.
2. **Symptoms & evidence** – key issues and supporting data.
3. **Assumptions to test** – especially high-risk ones.
4. **Problem statement(s)** – final agreed version(s).
5. **How Might We questions** – 1–3 selected HMW questions.
6. **Success metrics & signals** – what success looks like (linking to `ux-product-design-metrics` where needed).
7. **Scope, constraints, risks** – boundaries and dependencies.
8. **Recommended next steps** – what to do after framing.

Examples of recommended next steps:

- “Use the `ux-user-research` skill to plan discovery research to validate assumptions A, B, C.”
- “Use the `ux-information-architecture` skill to explore content and navigation issues revealed by this framing.”
- “Use the `ux-design-principles` skill to evaluate early solution ideas against UX laws, heuristics, accessibility, and platform guidelines.”
- “Use the `ux-product-design-metrics` skill to refine HEART/GSM metrics and set baselines for this problem.”

---

## Examples

### Example 1: Checkout abandonment

**Initial ask**  
“Redesign the checkout so people stop dropping. Our sales are down.”

**Problem framing outcome**

- Symptom: High drop-off on payment step; customers complain about “hidden fees”.
- Problem statement: “Price-sensitive customers need to understand total costs early in checkout but encounter surprise delivery fees at the final step, causing distrust and abandonment.”
- HMW: “How might we communicate total costs earlier in the checkout journey so that customers can make confident purchase decisions?”
- Success metrics: Reduced abandonment on payment step, fewer support complaints about pricing transparency, improved satisfaction/trust for checkout, stable or improved overall conversion.

### Example 2: Vague dashboard redesign

**Initial ask**  
“Our analytics dashboard looks bad. Please redesign it.”

**Problem framing outcome**

- Symptom: Users struggle to find key metrics quickly; frequent support questions on where to find basic numbers.
- Problem statement: “Time-pressed managers need to find 3–5 core KPIs in under a minute, but the current dashboard buries them among rarely used charts, leading to confusion and reliance on support.”
- HMW: “How might we make the most important KPIs immediately visible and interpretable for managers so they can make quick decisions without contacting support?”
- Success metrics: Time to first key metric, reduction in “where is X?” inquiries, increased self-reported confidence using the dashboard.

---

## Troubleshooting

### User has little or no data

- Acknowledge the lack of evidence and explain that you are framing a hypothesis problem to guide what data to collect.
- Emphasize assumptions vs facts and clearly label evidence gaps.
- Recommend specific next steps (e.g., “plan 5–7 interviews” or “review analytics for this funnel”) and hand off to the research skill.

### Stakeholder is fixated on a solution

- Reflect their desired solution respectfully while re-anchoring on user needs and outcomes.
- Show how framing the problem well increases the chance that their solution will work or reveal better options.
- Keep problem statements and HMW questions free of specific feature or UI decisions, but you can later explore their idea during ideation.

### Problem feels too broad

- Slice the problem by user segment, journey stage, or metric (e.g., focus first on new users in onboarding rather than “overall product experience”).
- Draft multiple narrower problem statements, then ask the user to pick the one with highest impact and feasibility for the current work.

---

## Notes for combination with other skills

- After running this skill, it is recommended to follow up with:
  - `ux-user-research` for discovery and validation.
  - `ux-information-architecture` if structural/content issues are suspected.
  - `ux-design-principles` to ground solution ideas in UX laws, heuristics, accessibility, and platform guidelines.
  - `ux-product-design-metrics` to select, refine, and track HEART/GSM/AARRR metrics for this problem.
  - Product or collaboration skills for prioritization and stakeholder alignment.

This ensures a consistent flow from problem framing → research → design → measurement across your UX practice.[web:325]
