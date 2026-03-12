---
name: ux-user-research
description: >
  Plans and runs user and market research to inform UX and product decisions.
  Use when the user needs help choosing methods, planning studies, creating
  research materials, analyzing findings, or turning data into personas and
  opportunity areas. Covers qualitative research (interviews, contextual
  inquiry, diary studies, usability tests), basic quantitative research
  (surveys, simple analytics reads), and competitor/market scans as inputs
  to UX strategy, and connects findings to shared principles and metrics.
metadata:
  domain: ux
  category: research
  author: your-name
  version: 1.1.0
---

# UX User & Market Research

## Purpose

This skill guides the planning and synthesis of user and market research so that design decisions are grounded in real behaviour, needs, and market context.[web:319][web:325] It combines qualitative and quantitative UX methods with competitor and market analysis to create actionable insights, personas, and opportunity areas, and is designed to work alongside `ux-mindset-problem-framing`, `ux-design-principles`, and `ux-product-design-metrics`.[web:260][web:303]

Use this skill whenever you need to understand users, validate assumptions, or size opportunities before (or alongside) design and product decisions.

---

## Instructions

### Step 1: Clarify research goals and questions

Before choosing methods, clarify what the team really needs to learn.[web:325]

Ask:

- "What decisions do you need this research to support?"
- "What do you already know, and what are you unsure about?"
- "Which assumptions, if wrong, would cause the biggest problems?"

From this, write:

- 2–4 **research goals** (e.g., “understand why new users abandon onboarding at step 3”).
- 3–8 **research questions** (e.g., “What expectations do users have before onboarding?”, “What obstacles or confusions occur at step 3?”).

Ensure questions are answerable by user/market research (not solely “Will this feature increase revenue?”).

Also identify any **existing data sources** (analytics, support tickets, previous studies) that should be reviewed before or alongside new data collection, so you build on prior knowledge instead of starting from scratch.

If problem framing already exists (via `ux-mindset-problem-framing`), align goals and questions to the defined problem statements, assumptions, and success criteria.

---

### Step 2: Select methods (qual, quant, or mixed)

Select methods based on goals, timeline, and available data.[web:325]

- If the goal is to **explore needs/behaviours or generate ideas**, propose **qualitative** methods:
  - Generative interviews
  - Contextual inquiry / field studies
  - Diary studies
  - Open-ended surveys

- If the goal is to **measure or compare**, propose **quantitative** methods:
  - Structured surveys
  - Simple experiments / A/B tests (if infrastructure exists)
  - Analytics review (funnels, events, cohorts)
  - Task success metrics, completion rates, error rates (see `ux-product-design-metrics` for definitions).[web:288]

- If both exploration and measurement are needed, propose a **mixed-methods** approach:
  - Qual first to discover patterns, quant after to validate and size them.

Summarize your recommendation:

- Primary method(s)
- Why they fit the goal
- Rough sample size and timeline (e.g., “5–8 interviews over 1–2 weeks”; “survey with 100+ responses over 1–2 weeks”).

---

### Step 3: Define target participants and recruitment criteria

Clarify **who** you need to hear from for valid insights.

Ask:

- "Which user segments, roles, or customer types are most relevant?"
- "Are there specific behaviours we care about (e.g., people who abandoned, power users, people who never converted)?"
- "Any markets, platforms, or languages in/out of scope?"

Produce:

- 1–3 **primary segments** (e.g., “new B2B admins in their first 30 days”).
- **Inclusion criteria** (must-have traits or behaviours).
- **Exclusion criteria** (who should not be recruited).

If personas already exist (from previous research or `ux-design-principles`/foundations work), align recruitment to those personas; if not, note that this research can help define or refine them.

---

### Step 4: Plan qualitative research

Based on chosen methods, outline a concrete plan.

#### 4.1 Interviews / contextual inquiry

For interviews or contextual sessions:

- Define **session length** (e.g., 45–60 minutes).
- Draft a **discussion guide** structure:
  - Warm-up and background
  - Current workflows / behaviours
  - Specific journeys or tasks related to the problem
  - Pain points, needs, expectations
  - Reactions to existing flows or concepts (if evaluative)

Include example question patterns:

- “Tell me about the last time you [did relevant task].”
- “Walk me through what you did, step by step.”
- “What was hardest or most frustrating?”
- “What would ‘great’ look like in this situation?”

Where relevant, probe for aspects that connect to principles from `ux-design-principles` (e.g., clarity, feedback, trust, accessibility).

#### 4.2 Diary studies or longitudinal methods

If long-term behaviour is important, propose a **diary study**:

- Duration (e.g., 1–2 weeks).
- Prompt schedule (e.g., daily, event-based).
- Log template (what they record: context, task, feelings, outcome).

Define how you’ll check in (e.g., kickoff + midpoint + closing interview).

#### 4.3 Usability testing (if needed)

If the goal includes evaluating a specific flow or prototype, outline a **usability test**:

- Scope and tasks (e.g., “sign up and complete first project”).
- Success criteria (task completion, time on task, errors).[web:288]
- Think-aloud vs moderated script.

You can use metrics definitions from `ux-product-design-metrics` (task success rate, time on task, error rate, learnability) to structure the test and analysis.

---

### Step 5: Plan basic quantitative research

If quantitative or mixed methods are needed, plan simple, decision-focused quant.

#### 5.1 Surveys

- Define **survey goal** (e.g., measure prevalence of a behaviour, understand attitudes).
- Draft a high-level question structure:
  - Screening questions
  - Behaviour questions (what they do)
  - Attitude questions (how they feel)
  - Outcome questions (success, satisfaction, loyalty)

Recommend:

- Mostly closed-ended questions with carefully chosen scales.
- 1–2 open-ended questions for richer context.

Where appropriate, align items with standard attitudinal metrics from `ux-product-design-metrics` (e.g., SUS, NPS, CSAT, CES) so results can be compared over time.[web:311][web:293]

#### 5.2 Analytics / product data

If analytics exist, outline:

- Which **events or funnels** to inspect (e.g., onboarding, checkout, key task flows).
- Which basic metrics to examine:
  - Conversion or completion rate
  - Drop-off by step
  - Time on task or time to complete
  - Usage frequency and feature adoption

Specify how analytics will be used:

- To contextualize qualitative findings.
- To size the impact of observed issues.
- To connect to framework views like HEART, AARRR, or PULSE if the team already uses them.[web:303][web:313][web:310]

---

### Step 6: Plan competitor and market research

Add **competitor and market insights** to complement user research.

Define:

- **Direct competitors** – similar products in the same space.
- **Indirect / aspirational competitors** – adjacent or best-in-class experiences.

Suggest activities:

- UX competitor walkthroughs with a structured checklist (onboarding, navigation, key flows, messaging, pricing clarity, help/support).
- Screenshots and notes of patterns, strengths, weaknesses.
- Market-level review:
  - Industry reports, trend articles, relevant benchmarks.
  - Signals about expectations users bring from other products.

Where possible, define simple **benchmark metrics** (e.g., time to complete a core task, number of steps, clarity of pricing) to compare your experience against key competitors.

Summarize outputs:

- Table of competitors vs key UX dimensions.
- List of patterns to consider adopting, avoiding, or improving upon—grounding evaluation in concepts from `ux-design-principles` (e.g., Gestalt, heuristics, accessibility).

---

### Step 7: Capture and synthesize research data

Help structure notes and data for synthesis.

#### 7.1 Note structure

Recommend note structures such as:

- By participant (for qualitative): background + key quotes + behaviours + pain points + opportunities.
- By theme (for synthesis): recurring needs, obstacles, workarounds, mental models.

#### 7.2 Thematic analysis

Guide a basic thematic clustering:

- Extract key observations from each session or data source.
- Group observations into themes (e.g., “trust & transparency”, “learnability”, “efficiency”, “collaboration”).
- For each theme, capture:
  - Description
  - Supporting evidence (quotes, metrics)
  - Impact on users and business

Where appropriate, connect themes back to assumptions from the `ux-mindset-problem-framing` skill and highlight which themes map to principle areas in `ux-design-principles` (e.g., feedback, information architecture, motion, performance).

---

### Step 8: Produce personas, JTBD, and opportunity areas

From synthesized data, help create **personas, jobs-to-be-done, and opportunity areas**.

#### 8.1 Personas (lightweight)

- Identify distinct clusters of users based on goals, behaviours, contexts, and constraints.
- For each persona, define:
  - Name and role
  - Goals and motivations
  - Behaviours and workflows
  - Pain points and needs
  - Environment and constraints

Keep them grounded in recurring patterns, not single anecdotes.

#### 8.2 Jobs-to-be-done

Translate insights into jobs:

- “When [situation], [user] wants to [goal] so they can [bigger outcome].”

Capture desired outcomes and functional, social, and emotional aspects where relevant.

#### 8.3 Opportunity areas

For each major theme, derive opportunities, for example:

- “Opportunity: simplify and clarify onboarding steps for new admins to reduce confusion and time to first value.”
- “Opportunity: improve transparency and control around pricing and billing to build trust.”

Link each opportunity to evidence, potential impact, and, where useful, to relevant principles from `ux-design-principles` (e.g., visibility of system status, match with real world, error prevention).[web:288][web:260]

---

### Step 9: Create a research summary and recommendations

Produce a concise, stakeholder-ready summary that can flow into design and product work.[web:325]

Suggested sections:

1. **Background and goals** – context, goals, research questions.
2. **Methods** – what you did and with whom (segments, sample sizes).
3. **Key findings / themes** – top 4–7 insights with evidence.
4. **Personas or segments** – if relevant.
5. **Jobs / opportunity areas** – what to focus on next.
6. **Recommendations** – design, product, and research recommendations.
7. **Risks and limitations** – sample caveats, what this research cannot answer.

Align recommendations back to:

- Problem framing and assumptions from `ux-mindset-problem-framing`.
- Principles from `ux-design-principles` (e.g., heuristics, accessibility, motion, IA) when suggesting design changes.
- Metrics from `ux-product-design-metrics` (e.g., HEART/GSM setups) when suggesting how to track impact.[web:303][web:308]

---

## Examples

### Example 1: Onboarding drop-off study

- Goals: understand why new users abandon during step 3 of onboarding; identify opportunities to improve completion.
- Methods: 6 remote interviews with recent sign-ups, analytics review of onboarding funnel, small competitive scan of 3 similar tools.
- Findings: unclear value proposition at step 2, unexpected required fields at step 3, low perceived payoff for completing setup.
- Outputs:
  - Persona: “Time-poor team lead” with specific goals and constraints.
  - Opportunities: clarify value earlier, reduce required fields, delay advanced setup to later moments.
  - Recommendations: prototype a simplified onboarding path; validate via usability tests; track task success, time on task, and early retention using `ux-product-design-metrics` definitions.[web:288][web:303]

### Example 2: Market and UX competitive analysis

- Goals: understand how competitors handle pricing and feature packaging; identify gaps.
- Methods: 5 competitor UX walkthroughs, analysis of public documentation and pricing pages, light market-trend review.
- Findings: competitors use clearer tier names, upfront pricing, and better empty states during trial.
- Outputs:
  - UX patterns to emulate or improve on, mapped to principles (clarity, transparency, feedback).
  - Opportunity areas linked to user expectations and differentiators.
  - Recommendations: revise pricing flows guided by `ux-design-principles`; measure impact via conversion and support ticket metrics as defined in `ux-product-design-metrics`.[web:260][web:309]

---

## Troubleshooting

### No research capacity or very tight timelines

- Suggest lightweight methods:
  - 3–5 quick user interviews.
  - Simple short survey with existing users.
  - Rapid review of support tickets and analytics.
- Emphasize that even small, focused studies are more reliable than assumptions.

### Data conflict between qualitative and quantitative findings

- Highlight differences rather than forcing agreement.
- Use mixed-method reasoning:
  - Quant shows “what” and “how often” at scale.
  - Qual explains “why” with depth.
- Recommend follow-up where gaps are critical.

### Stakeholders want “proof” from small samples

- Clearly describe limitations of small qualitative samples.
- Focus on patterns and directionality, not statistical proof.
- Suggest ways to follow up with larger quantitative studies if needed.

---

## Notes for use with other skills

- Use this skill **after** `ux-mindset-problem-framing` to validate assumptions and deepen understanding.
- Feed outputs into:
  - `ux-information-architecture` (if structural or content issues are discovered).
  - Interaction and UI skills (for detailed design decisions guided by `ux-design-principles`).
  - Product thinking skills (for opportunity sizing and prioritization).
  - `ux-product-design-metrics` to define or refine HEART/GSM/AARRR metrics and measurement plans tied to the research findings.[web:303][web:308][web:313]
