---
name: product-discovery-opportunity
description: >
  Frames product discovery work into clear opportunity areas, problem
  definitions, and hypotheses. Use when the user needs to turn insights and
  stakeholder input into opportunities, and apply simple frameworks like JTBD,
  Opportunity Solution Trees, and light scoring to decide what to explore next,
  aligned with shared outcomes and metrics.
metadata:
  domain: product
  category: discovery-opportunity
  author: your-name
  version: 1.1.0
---

# Product Discovery & Opportunity Sizing

## Purpose

This skill helps turn research insights, data, and stakeholder ideas into well-defined opportunities and testable hypotheses.[web:372] It uses simple, industry-standard frameworks (Jobs to Be Done, opportunity mapping, Opportunity Solution Trees, light scoring models) to prioritize which problems and opportunities to explore in discovery work, and connects to `ux-mindset-problem-framing`, `ux-user-research`, and `ux-product-design-metrics` so outcomes and measurement stay aligned.[web:366][web:369][web:372]

Use this skill when you have a lot of inputs (feedback, ideas, pain points) and need to create a clear picture of the opportunity space and decide where to focus.

---

## Instructions

### Step 1: Clarify outcomes and constraints

Anchor discovery in the **outcomes** that matter.[web:365][web:366]

Ask:

- "What product or business outcome are we trying to move (e.g., activation, retention, revenue, NPS, HEART dimensions)?"[web:369]
- "What time horizon are we working with (e.g., this quarter, this year)?"
- "What constraints are non-negotiable (markets, platform, regulatory)?"

Summarize:

- Target outcome(s) (e.g., “Increase onboarding completion”, “Improve self-serve adoption”).
- Time horizon and any constraints.
- Key segments or journeys in scope.

You can frame outcomes and metrics using `ux-product-design-metrics` (e.g., HEART + GSM, AARRR) so each opportunity explicitly ties to measurable signals later.[web:369] This sits at the top of your opportunity thinking and, if you use one, your Opportunity Solution Tree.[web:366][web:374]

---

### Step 2: Gather and cluster inputs

Collect the **raw inputs** that hint at problems and opportunities.[web:372]

Sources may include:

- User research (interviews, JTBD-style interviews, usability tests).
- Analytics (drop-off points, low-engagement features).
- Support tickets and sales feedback.
- Stakeholder ideas and known pain points.[web:372]

Cluster similar items into themes, such as:

- Onboarding friction
- Pricing and packaging confusion
- Collaboration gaps
- Reporting and insight needs

Record each input with a short, neutral description and source. Where useful, tag inputs with affected outcomes/metrics (e.g., activation, task success, NPS) so you can see where evidence clusters.

---

### Step 3: Frame Jobs to Be Done and user problems

Translate raw inputs into **Jobs to Be Done** and problem statements.[web:367][web:371]

Use JTBD-style statements:

- “When [situation], [user] wants to [job] so they can [desired outcome].”[web:367]
- Example: “When starting a new project with a client, consultants want to quickly set up a shared workspace so they can appear organized and professional.”

For each job, identify:

- Context (when/where this happens).
- Desired outcome (what success looks like for the user).
- Current obstacles and frustrations (from research or data).[web:367]

These jobs and problems become the backbone of your opportunity space and connect back to problem statements from `ux-mindset-problem-framing`.

---

### Step 4: Map opportunities from jobs and pain points

From each job/problem, derive **opportunities**—places where you could create value.[web:372]

For each job/problem, ask:

- "Where in the process does the user struggle most?"
- "Which steps are slow, confusing, or error-prone?"
- "Where are existing solutions failing to meet expectations?"

Describe opportunities as unmet or underserved needs, for example:

- “Help new admins understand which steps are essential vs optional in onboarding.”
- “Make pricing and limits clear before users commit to a plan.”

You can represent this as a list or as part of an Opportunity Solution Tree:

- Outcome → Opportunities → (later) Solutions → Tests.[web:366][web:374]

---

### Step 5: Build a simple Opportunity Solution Tree (optional but recommended)

Use an **Opportunity Solution Tree (OST)** style structure to organize thinking.[web:362][web:365][web:366][web:374]

At minimum:

- Top level: Targeted outcome (from Step 1).
- Next level: Opportunities (from Step 4).
- Next level: Potential solution ideas for each opportunity.
- Last level: Assumption tests or experiments you could run.

The tree helps you:

- See all opportunities under a shared outcome.
- Avoid jumping straight from outcome to a single solution.
- Keep track of which opportunities and solutions you’ve explored or validated, and which assumptions you still need to test.[web:365][web:366]

Treat the OST as a living artefact that evolves as you learn (both from discovery research and from experiments).

---

### Step 6: Define hypotheses for key opportunities

Turn priority opportunities into **testable hypotheses**.[web:372][web:368]

Use simple patterns:

- Problem hypothesis:  
  - “We believe that [segment] struggles with [problem] when [context], which leads to [negative outcome/metric impact].”
- Solution hypothesis:  
  - “We believe that [solution idea] will help [segment] achieve [job/outcome] by [mechanism], resulting in [impact on outcome metric].”
- Assumption hypothesis:  
  - “We believe [specific assumption about behaviour, value, or feasibility] is true.”

For each opportunity, you may have multiple hypotheses about:

- The problem (is it real and important?).
- The solution (will this approach address it?).
- The value (will it move the outcome you care about, as defined via HEART/GSM, AARRR, or business KPIs?).[web:369][web:373]

---

### Step 7: Size and prioritize opportunities

Use simple criteria to **size** and prioritize opportunities before investing heavily.[web:372][web:368]

For each opportunity, consider:

- **User value**:
  - How important is the job to users?
  - How much friction or dissatisfaction exists today? (e.g., frequency × frustration).[web:367][web:371]
- **Business impact**:
  - How directly does this connect to your target outcome (activation, retention, revenue, NPS, HEART category)?[web:369][web:372]
- **Reach**:
  - How many users or accounts are affected?
- **Feasibility / effort**:
  - Rough estimation of implementation complexity and dependencies.
- **Confidence**:
  - How strong is the evidence behind your assumptions and impact estimates (e.g., using confidence meters or ICE/RICE-style thinking)?[web:368][web:376]

You can express this with:

- A simple High/Medium/Low rating per dimension, or
- A light scoring approach (e.g., impact × confidence ÷ effort, ICE, RICE), or
- A JTBD-style **opportunity score** that combines importance and satisfaction gaps for outcomes (e.g., Importance + max(Importance − Satisfaction, 0)).[web:367][web:375]

Identify:

- Top 3–5 opportunities to explore next.
- Lower-priority opportunities to park for later.

---

### Step 8: Select discovery bets and next actions

From prioritized opportunities, choose **discovery bets**—areas you’ll actively explore now.[web:372][web:368]

For each chosen opportunity:

- Confirm the main hypothesis you want to test first.
- Decide the next discovery action, such as:
  - JTBD-focused interviews or field visits.
  - Concept testing (sketches, prototypes).
  - Data deep-dive or quick analytics checks.
  - Small experiments or pilots (e.g., A/B tests, feature flags).[web:362][web:365]

Document:

- Opportunity name and description.
- Chosen hypothesis to test.
- Planned method(s) and time frame.
- How you’ll know if you should continue, pivot, or drop it (linked back to outcomes and metrics defined with `ux-product-design-metrics`).[web:369]

---

### Step 9: Keep the opportunity space and decisions visible

Maintain a living view of your **opportunity space**, not just a backlog of solutions.[web:366][web:370]

- Keep your opportunities list or OST up to date as you learn.
- Mark:
  - Opportunities validated as important.
  - Opportunities invalidated or deprioritized.
  - Solutions tested and their outcomes.
- When new ideas arrive, link them to existing opportunities or note if they imply a new opportunity.

Use this artefact to:

- Communicate with stakeholders about **why** you’re focusing where you are.
- Avoid repeatedly revisiting the same debates without new evidence.
- Ensure discovery work stays tied to outcomes, real jobs, and measurable metrics.[web:366][web:372]

---

## Examples

### Example 1: Improving onboarding completion

- Outcome:
  - Increase onboarding completion for new admins (Task Success and Adoption in HEART).[web:369]
- Inputs:
  - Drop-off at step 3, interview feedback about confusion, support tickets about setup.
- JTBD:
  - “When starting with a new tool, new admins want to quickly configure the basics so they can show value to their team without feeling overwhelmed.”[web:367]
- Opportunities:
  - Clarify which setup steps are required vs optional.
  - Provide better guidance and expectations about time and effort.
- Prioritization:
  - High user importance, high friction, large reach, medium effort, reasonable confidence → top discovery bet.[web:368][web:372]
- Next actions:
  - JTBD interviews with recent sign-ups.
  - Low-fidelity concept tests of a simplified onboarding flow, then A/B tests measured via completion and time to first value.[web:362][web:369]

### Example 2: Expanding usage in existing accounts

- Outcome:
  - Increase feature adoption in existing paying accounts (Engagement and Retention).[web:369]
- Inputs:
  - Analytics show low use of collaboration features, interviews reveal people work around them with external tools.
- JTBD:
  - “When coordinating work across teams, managers want everyone to see the same status without duplicating effort across tools.”[web:367]
- Opportunities:
  - Make collaboration entry points more obvious in core workflows.
  - Clarify value of shared views vs individual workspaces.
- Prioritization:
  - High business impact (retention, expansion), medium effort, moderate reach → strong candidate for exploration.[web:372]
- Next actions:
  - Concept tests of new collaboration affordances.
  - Small in-product experiments with clearer prompts and placement, measured with adoption and usage metrics.[web:365][web:369]

---

## Troubleshooting

### Too many opportunities, hard to choose

- Tighten scope by outcome and time horizon (e.g., focus only on activation this quarter).
- Apply simple impact × confidence ÷ effort or importance × satisfaction thinking to cut through the noise.[web:368][web:367]
- Limit immediate bets to a small number (e.g., 3–5), park the rest.

### Stakeholders jump straight to solutions

- Reframe their ideas as hypotheses tied to specific opportunities.
- Show how each idea fits under jobs and outcomes in your OST.
- Use your opportunity map or OST to discuss trade-offs and focus, not just features.[web:365][web:366]

### Discovery feels disconnected from delivery

- Link discovery outputs (opportunities, hypotheses) to backlog items, experiments, and OKRs.
- Use the same outcome metrics (HEART, AARRR, GSM) in both discovery and delivery discussions.[web:369][web:373]
- Update the opportunity space as you learn from experiments and launches, so it stays relevant.

---

## Notes for use with other skills

- Use this skill alongside:
  - `ux-mindset-problem-framing` to define sharp problem statements and assumptions.
  - `ux-user-research` to gather evidence for jobs, opportunities, and satisfaction/importance gaps.
  - `ux-prototyping-validation` to test solution hypotheses for prioritized opportunities.[web:362][web:370]
  - `ux-product-design-metrics` to define and track outcome metrics (HEART, AARRR, GSM) for opportunities and discovery bets.[web:369]
  - Product roadmapping and experimentation skills when turning validated opportunities into initiatives, bets, and experiments at scale.[web:372][web:368]
