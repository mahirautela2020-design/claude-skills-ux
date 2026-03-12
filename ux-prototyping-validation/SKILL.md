---
name: ux-prototyping-validation
description: >
  Plans and creates prototypes at the right fidelity, then validates concepts
  and flows through user testing. Use when the user needs help deciding
  prototype fidelity (low, mid, high), planning concept or usability tests,
  creating test tasks and scripts, and turning findings into design changes and
  next steps, aligned with shared UX principles and metrics.
metadata:
  domain: ux
  category: prototyping-validation
  author: your-name
  version: 1.1.0
---

# UX Prototyping & Validation

## Purpose

This skill helps teams choose the right level of prototype fidelity and run structured validation activities so that design decisions are tested with users before full implementation.[web:325] It covers low-, mid-, and high-fidelity prototypes and the setup of concept tests and usability tests that lead to concrete design improvements, and it works alongside `ux-design-principles` (for heuristics, patterns, accessibility) and `ux-product-design-metrics` (for task and outcome metrics).[web:260][web:303]

Use this skill when you want to explore ideas quickly, test flows or interactions, or de-risk design decisions with real user feedback.

---

## Instructions

### Step 1: Clarify goals, risks, and constraints

Before prototyping, clarify **what you are trying to learn** and **what is at risk**.[web:325]

Ask:

- "What decision do you want this prototype to help you make?"
- "What are the riskiest assumptions about this idea or flow?"
- "What constraints do you have (time, tools, recruiting, devices)?"

Summarize:

- Validation goals (e.g., “Does this concept solve the right problem?”, “Can users complete this flow without help?”).
- Key risks and unknowns.
- Practical constraints (timeframe, team, tools).

When possible, connect goals to categories from `ux-product-design-metrics` (task performance, behavioral, attitudinal, business) so you already know what you’ll measure (e.g., task success rate, time on task, CSAT, conversion).[web:288][web:303]

This will guide fidelity and test type.

---

### Step 2: Choose prototype fidelity (low, mid, high)

Select prototype fidelity based on stage and risk.[web:325]

- **Low-fidelity** (sketches, wireframes, basic clickable flows):
  - Use early, when exploring multiple ideas or structures.
  - Good for checking concepts, flows, and IA without getting stuck on visual details.

- **Mid-fidelity** (structured wireframes with clearer layout and basic interactions):
  - Use when you have a direction and need to test flows and layout.
  - Good for usability testing of tasks without final visual polish.

- **High-fidelity** (realistic UI, interactions, and content):
  - Use when you need to test detailed interactions, visual hierarchy, and nuanced content.
  - Good for late-stage validation and stakeholder buy-in.

Recommend a fidelity and explain why it fits the current goals and risks. Note what can be simplified versus what must be realistic, and reference `ux-design-principles` when you specifically want to validate visual hierarchy, motion, or platform conventions.[web:230][web:236][web:295]

---

### Step 3: Define scenarios and tasks for the prototype

Design around **realistic user scenarios and tasks**.[web:325]

Define:

- Scenario: a short narrative that sets context (who the user is, what they’re trying to do, and why).
- Tasks: specific actions the participant will attempt using the prototype.

Guidelines:

- Use tasks that align with the critical flows and success metrics (e.g., “Sign up and create your first project”, “Compare two plans and choose one”).[web:288][web:303]
- Avoid telling participants exactly how to complete the task (“Click X, then Y”); focus on goals, not instructions.
- Include a mix of primary tasks (core flows) and secondary tasks (settings, error recovery, etc.) if time allows.

Document scenarios and tasks clearly so they can be reused in test scripts and later linked to metrics definitions from `ux-product-design-metrics` (e.g., task success, time on task, error rate, CES).[web:288][web:293]

---

### Step 4: Prepare the prototype for testing

Ensure the prototype supports the planned tasks smoothly.[web:325]

Check:

- All screens and states needed for each task are present.
- Links and hotspots cover the expected paths (and key alternate paths).
- Error and empty states are approximated where they matter, even if simplified.
- Navigation behaves consistently enough for testing.

For low- and mid-fidelity prototypes:

- Focus on flow logic and information placement.
- Use simple labels and placeholders where detailed UI is not necessary.

For high-fidelity prototypes:

- Align UI and interactions with your design system and platform patterns.
- Ensure content, visual hierarchy, and microinteractions are realistic enough for evaluation, drawing from `ux-design-principles` for heuristics, motion, and accessibility.[web:260][web:295][web:293]

---

### Step 5: Choose validation approach and test type

Select the **validation approach** and **test type** based on what you need to learn and your constraints.[web:325]

#### 5.1 Concept vs usability focus

- **Concept testing**:
  - Focus: overall desirability, comprehension, and perceived value of an idea or direction.
  - Questions: Do users understand what this is? Does it solve the right problem? How does it fit into their current behaviour?
  - Prototype: low- to mid-fidelity is often enough to communicate the idea.

- **Usability testing**:
  - Focus: ease of use, efficiency, and errors when completing tasks.
  - Questions: Can users complete key tasks? Where do they get stuck? What confuses them?
  - Prototype: mid- to high-fidelity, with realistic flows and interactions.

You can combine both in one session (short concept discussion, then task-based usability tasks) if time allows.

#### 5.2 Moderated vs unmoderated

Decide how sessions will run:

- **Moderated (live)**:
  - Researcher facilitates in real time (remote or in-person).
  - Best for complex flows, early concepts, and when you need to probe “why”.
  - Requires more time per session but gives richer insight.

- **Unmoderated (self-guided)**:
  - Participants complete tasks on their own using a script or testing platform.
  - Best for simpler flows and when you need more participants or quick feedback.
  - Less ability to probe in the moment; rely on careful task design and follow-up questions.

#### 5.3 In-person vs remote

- **In-person**:
  - Useful when physical context, devices, or environment matter (e.g., retail, hardware, multi-screen setups).
  - Easier to observe non-verbal cues, but harder to scale.

- **Remote**:
  - Easier to recruit diverse participants.
  - Works well for most digital product testing when using screen sharing or remote testing tools.

#### 5.4 Think‑aloud vs silent observation

- **Think‑aloud**:
  - Ask participants to verbalize what they’re trying to do and what they expect.
  - Great for understanding mental models and misunderstandings.
- **Silent with retrospective interview**:
  - Let participants work naturally, then ask them afterward about key moments.
  - Useful when talk‑aloud would interfere with realistic behaviour.

Choose the combination (moderated/unmoderated, in‑person/remote, think‑aloud/retrospective) that best matches your goals, context, and available resources.

---

### Step 6: Plan sessions and scripts

Create a simple **session plan** and **moderation script**.[web:325]

Session structure:

1. Introduction and consent (brief explanation, recording consent if applicable).
2. Background questions (role, experience, current tools).
3. Concept exploration (if relevant) – show the idea and discuss first impressions.
4. Task-based usability testing – ask participants to perform predefined tasks using the prototype.
5. Wrap-up – overall impressions, likes/dislikes, suggestions, and closing.

For the script:

- Write simple prompts for each task (e.g., “Imagine you want to… Please show me how you would do that here.”).
- Note any follow-up questions you will use when participants struggle or succeed (“What were you expecting here?”).
- Plan not to lead participants to the “right” answer; stay neutral.

Align key questions with constructs you may measure later (e.g., satisfaction, perceived effort, understanding) to complement metrics like CSAT, CES, or SUS from `ux-product-design-metrics`.[web:311][web:293]

---

### Step 7: Run tests and capture observations

During sessions:

- Encourage think-aloud (participants narrate what they’re trying to do and what they expect).
- Observe:
  - Where they hesitate or get stuck.
  - Misunderstandings about labels, layout, or interactions.
  - Workarounds or unexpected paths they take.
- Capture:
  - Success/failure for each task.
  - Time to complete (roughly, if useful).
  - Severity of issues (e.g., cosmetic, minor, major, blocker).

Use structured notes per participant and per task to make synthesis easier later, and align behavioural metrics (task success, time on task, error patterns) with definitions from `ux-product-design-metrics`.[web:288][web:303]

---

### Step 8: Analyze results and identify issues

After sessions, synthesize findings.[web:325]

- Aggregate observations across participants:
  - Where did multiple people struggle?
  - Which paths worked smoothly?
- Cluster issues into themes (e.g., navigation confusion, unclear labels, hidden actions, overloaded screens).

For each issue:

- Describe the problem in user terms (what they were trying to do and what happened).
- Link to evidence (which tasks, how many participants, severity).
- Identify likely root causes in the design (interaction pattern, content, visual hierarchy, IA), referencing `ux-design-principles` when helpful (e.g., violations of recognition over recall, visibility of system status, error prevention).[web:288][web:260]

Keep the analysis focused on patterns rather than individual anecdotes.

---

### Step 9: Turn findings into design changes and next steps

Translate validation results into **concrete actions**.[web:325]

For each major issue:

- Propose at least one design change (e.g., surface a control earlier, change label, reduce steps, change pattern).
- Prioritize:
  - Severity (how badly it affects users).
  - Frequency (how often it occurs).
  - Impact on key metrics (conversion, completion, satisfaction) as defined in `ux-product-design-metrics`.[web:303][web:309]

Summarize:

- Top issues and associated design changes.
- Changes that can be applied widely as patterns or guidelines.
- Open questions that need further research or testing.

Decide whether:

- Another iteration of prototype + testing is needed.
- It is ready to move into implementation with known trade-offs.

Where appropriate, propose a follow-up measurement plan (e.g., HEART + GSM) from `ux-product-design-metrics` to track impact after implementation.[web:303][web:308]

---

## Examples

### Example 1: Early concept test

- Context: New idea for a “guided setup” wizard.
- Fidelity: Low-fidelity wireframes showing main steps and screens.
- Validation:
  - Concept test with 5 participants to understand whether the concept makes sense and fits their workflow.
  - Questions around perceived value, clarity of steps, and missing pieces.
- Outcome:
  - Refined concept flow and messaging before investing in detailed UI.
  - Clearer hypotheses and HEART metrics (Happiness, Adoption) for later experiments via `ux-product-design-metrics`.[web:303]

### Example 2: Usability test on high-fidelity prototype

- Context: Redesigned billing settings area.
- Fidelity: High-fidelity prototype in design tool with realistic data and interactions.
- Validation:
  - Usability test with 6 participants focused on tasks like “update payment method” and “download last month’s invoice.”
  - Measured task success and observed confusion around nested navigation.
- Outcome:
  - Simplified navigation structure, clearer labels, improved error and confirmation messages.
  - Plan to track completion rate, time on task, and support tickets post-release using `ux-product-design-metrics` definitions.[web:288][web:309]

---

## Troubleshooting

### Prototype is too rough or too polished for the question

- If users focus on visual polish instead of the idea, consider stepping down fidelity for early exploration.
- If they can’t understand the flow because it’s too abstract, increase fidelity where needed for clarity.
- Use `ux-design-principles` to decide which aspects must be realistic (e.g., hierarchy, key interactions) at each stage.[web:230][web:240]

### Sessions turn into design critiques

- Gently redirect from “I don’t like this colour” to “Tell me what you expected here” and “What would help you complete this task more easily?”
- Focus on observable behaviour and needs, not personal preferences.
- Capture directional feedback but prioritize patterns rooted in behaviour and metrics.

### Findings are inconsistent

- Look for patterns across participants rather than expecting unanimity.
- Note differences by segment (e.g., new vs experienced users).
- If critical decisions hinge on unclear results, plan a follow-up study (possibly with adjusted tasks or different fidelity) and consider complementing with quant from `ux-product-design-metrics` (e.g., A/B tests, surveys).[web:303][web:313]

---

## Notes for use with other skills

- Use together with:
  - `ux-mindset-problem-framing` to ensure you’re validating the right problem and success criteria.
  - `ux-user-research` to complement generative/discovery work and analytics.
  - `ux-information-architecture` and `ux-interaction-design` to ensure prototypes reflect intended structure and behaviour.
  - `ux-design-principles` to check concepts and flows against UX laws, heuristics, accessibility, and platform guidelines during review.[web:260][web:272]
  - `ux-writing-content` so microcopy, labels, and messages in prototypes are realistic enough for evaluation.
  - `ux-product-design-metrics` and product experimentation skills to define HEART/GSM/AARRR metrics and measure impact after validated designs are implemented.[web:303][web:308][web:313]
