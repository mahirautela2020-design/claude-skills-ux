---
name: product-experimentation-data
description: >
  Brings experimentation and data literacy into UX and product work. Use when
  the user needs help defining measurable hypotheses, collaborating on A/B
  tests or experiments, reading basic results, and combining analytics with
  qualitative research to decide what to iterate next, aligned with shared
  outcome and metrics frameworks.
metadata:
  domain: product
  category: experimentation-data
  author: your-name
  version: 1.1.0
---

# Experimentation & Data Literacy

## Purpose

This skill helps designers and product teams make evidence‑informed decisions by framing measurable hypotheses, collaborating on A/B tests and experiments, and interpreting results at a practical level.[web:141][web:143][web:144][web:145][web:151][web:153][web:150] It also guides how to combine analytics (quant) and research (qual) in a mixed‑methods way to decide what to iterate next, and connects to `ux-product-design-metrics` so experiments are anchored in HEART/AARRR/GSM outcomes rather than ad‑hoc numbers.[web:146][web:149][web:155][web:154][web:148][web:369][web:373]

Use this skill when you’re considering experiments, need to interpret test results, or want to bring data into design iteration without becoming a full‑time data scientist.

---

## Instructions

### Step 1: Clarify the decision and outcome

Before talking about tests or metrics, clarify **what decision** you’re trying to make.[web:141][web:143][web:151][web:153]

Ask:

- "What decision will this experiment inform (e.g., choose between two designs, keep or roll back a change)?"
- "Which user and business outcome are we trying to move (e.g., conversion, task completion, engagement, satisfaction, retention)?"[web:141][web:143][web:151][web:153][web:369]
- "What behaviour change do we expect from users if the design works as intended?"[web:145][web:148]

Whenever possible, express outcomes using the shared frameworks from `ux-product-design-metrics` (e.g., HEART category, AARRR stage, GSM goal/signal/metric) so experiments fit into the broader measurement model.[web:369][web:373] This anchors experimentation in real decisions and outcomes, not curiosity alone.

---

### Step 2: Define clear, measurable hypotheses

Frame design ideas as **testable hypotheses**.[web:147][web:145][web:148][web:150]

Use patterns like:

- **Design hypothesis**:  
  - “If we [design change], then [segment] will be more likely to [target behaviour], resulting in [metric change].”

Example:

- “If we surface a progress bar in the onboarding flow, new users will be more likely to finish onboarding, increasing completion rate (HEART: Task Success/Adoption) by at least 10%.”[web:148][web:145][web:369]

Make sure hypotheses specify:

- The change (what you’re testing).
- The audience/segment.
- The expected direction and rough magnitude of effect (where possible).
- The metric(s) that will show the effect, ideally reusing metrics defined via `ux-product-design-metrics`.[web:147][web:141][web:143][web:153][web:369]

---

### Step 3: Choose experiment type and basic design

Work with PMs/data to choose an appropriate **experiment type**.[web:141][web:143][web:144][web:151][web:153]

For most design work, this will be:

- **A/B tests (split tests)**:
  - Compare two versions (A = control, B = variant) for a subset of users.
- Sometimes:
  - A/B/n tests (multiple variants).
  - Feature flags and staged rollouts with before/after comparisons.[web:145][web:148][web:150]

Design basics:

- Randomly assign users to variants where possible.
- Keep other conditions stable during the test (avoid major confounding changes).
- Define:
  - Duration (long enough to reach minimum sample and cover typical usage patterns).
  - Primary metric and any guardrail metrics (e.g., conversion is primary; error rate or drop-off is guardrail).[web:144][web:145][web:147][web:153]

Designers don’t need to do the statistics, but should understand the logic enough to collaborate effectively.[web:141][web:143][web:145][web:150]

---

### Step 4: Select metrics and events with data partners

Collaborate with data/analytics partners to decide **what to measure**, using your shared metrics language.[web:141][web:143][web:147][web:153][web:369]

For each experiment:

- **Primary metric**:
  - The main outcome tied to your hypothesis (e.g., click‑through rate, conversion, onboarding completion, a proxy for task success or engagement).[web:141][web:143][web:147][web:153]
- **Secondary metrics**:
  - Supporting behaviours (scroll depth, feature usage, time on task).
  - Quality/safety metrics (error rates, bounce, drop‑off further in the funnel).[web:145][web:148][web:144]
- **Guardrails**:
  - Metrics that should not degrade beyond acceptable bounds (e.g., overall conversion, latency, retention).[web:145][web:147][web:153]

Ensure:

- Events are well‑defined (what counts as “success” or “activation”).
- Tracking exists or will be implemented correctly before running the test.[web:141][web:153][web:150]

Where possible, align these metrics with HEART/AARRR/GSM definitions from `ux-product-design-metrics` so experiments roll up cleanly into overall health views.[web:369][web:373]

---

### Step 5: Run the experiment and ensure integrity

Support a **clean run** of the experiment.[web:144][web:147][web:153]

Key points:

- Users should consistently see the same variant once assigned (no flipping between A and B).
- Avoid running overlapping tests on the same audience and metrics when possible.
- Let the test run until:
  - Minimum sample size is reached.
  - Pre‑defined test window is complete (e.g., at least one or more typical usage cycles).[web:144][web:145][web:153]

Designers can help monitor:

- Obvious UX issues in variants.
- Any surprising qualitative signals from support, research, or user feedback during the test.[web:144][web:146][web:148]

---

### Step 6: Read basic experiment results

When results are ready, interpret them at a **practical** level (in collaboration with data partners).[web:141][web:143][web:145][web:147][web:150][web:153]

Look for:

- Direction and magnitude of change in primary metric (did B outperform A? by how much?).
- Confidence/statistical significance as explained by analysts:
  - Is the observed difference likely to be real versus random noise?
- Impact on secondary and guardrail metrics:
  - Did improvements in one area cause harm elsewhere?[web:144][web:145][web:147][web:153]

Designers should focus on:

- Whether the hypothesis is supported, partially supported, or not supported.
- What user behaviour changed in practice.

Avoid over‑interpreting small or inconclusive differences without enough data.[web:141][web:143][web:147][web:153] Feed learnings back into hypotheses and the opportunity space (`product-discovery-opportunity`).

---

### Step 7: Combine analytics with qualitative research (mixed methods)

Use a **mixed‑methods** approach: analytics and experiments show “what” and “how much”; research shows “why”.[web:146][web:149][web:155][web:154][web:148]

Practices:

- Before experiments:
  - Use qualitative research (interviews, usability tests) to generate strong hypotheses and variants.[web:154][web:146][web:149][web:148]
- During/after experiments:
  - Use analytics and A/B results to quantify impact.
  - Use follow‑up research (e.g., targeted usability sessions, surveys) to understand why a variant worked or failed.[web:146][web:149][web:155][web:148]

When both data streams point in the same direction (e.g., users say something is confusing and A/B tests show lower engagement), treat it as a strong signal to prioritize changes.[web:146][web:149][web:155]

Connect this with `ux-user-research` and `ux-prototyping-validation` so experiment design and interpretation benefit from deep qualitative context.

---

### Step 8: Decide iteration and rollout based on evidence

Use experiment results and qualitative insights to decide **what to do next**.[web:141][web:144][web:145][web:153]

Options:

- **Roll out winning variant**:
  - When it clearly improves primary metrics without harming guardrails.
- **Iterate and re‑test**:
  - When results are mixed, unclear, or show local improvements with trade‑offs.
- **Roll back**:
  - When the variant clearly hurts key metrics or reveals UX regressions.

For each iteration, update:

- Hypotheses (based on what you’ve learned).
- UX and product metrics you care about (potentially refining GSM/HEART definitions).[web:369][web:373]
- The opportunity or roadmap items this work supports (`product-discovery-opportunity`, `product-ux-strategy-alignment`).

This builds a cycle of continuous improvement grounded in data and research.[web:145][web:146][web:149][web:155]

---

### Step 9: Communicate findings and learning

Summarize findings in a way that stakeholders can act on.[web:141][web:143][web:145][web:147][web:150][web:153]

Include:

- Hypothesis and why you tested this change (linked to outcomes/metrics).
- Experiment setup (variants, audience, duration, primary metrics).
- Key results:
  - Direction and size of change for main metrics.
  - Any important secondary/guardrail effects.
- Qualitative insights explaining the “why”.[web:146][web:149][web:155][web:154][web:148]
- Decision and next steps (rollout, iterate, or stop).

Capture these learnings in a shared place (e.g., experiment log) so future teams don’t re‑run the same tests without need and can see how experiments contribute to HEART/AARRR/GSM goals.[web:144][web:145][web:146][web:149][web:369]

---

## Examples

### Example 1: CTA placement A/B test

- Hypothesis:
  - “Moving the primary CTA above the fold and clarifying its label will increase click‑through by at least 8% without hurting overall conversion.”[web:145][web:148]
- Setup:
  - A/B test with variant B having new CTA placement and label.
  - Primary metric: CTA click‑through.
  - Secondary: downstream conversion to sign‑up.[web:141][web:143][web:153]
- Results:
  - CTR increased by ~10%, downstream conversion also improved.
- Mixed methods:
  - Follow‑up interviews confirmed users noticed and understood the CTA better.[web:146][web:149]
- Decision:
  - Roll out variant B, document pattern in `ui-design-systems-components` and note metric impact in the experiment log.

### Example 2: Onboarding step removal experiment

- Hypothesis:
  - “Removing a low‑value onboarding step will increase completion and not reduce long‑term engagement.”[web:144][web:145][web:148]
- Setup:
  - A/B test: A includes step; B skips it.
  - Primary metric: onboarding completion.
  - Guardrail: day‑7 retention, feature adoption.[web:141][web:143][web:153]
- Results:
  - Completion increased, but day‑7 retention in B dropped slightly.
- Mixed methods:
  - Qual interviews showed users missed essential context from the removed step.[web:146][web:154]
- Decision:
  - Iterate: reintroduce step in a simplified form; test again with better guidance rather than full removal, tied to HEART: Task Success + Retention.

---

## Troubleshooting

### Tests run, but results feel inconclusive

- Check whether:
  - Sample size and duration were sufficient.
  - Metrics were aligned with the hypothesis.
- Treat the test as learning, refine the hypothesis, and consider a follow‑up experiment with clearer design differences.[web:141][web:144][web:147][web:153]

### Team over‑relies on A/B tests alone

- Remind that tests show **what** happened, not always **why**.
- Pair experiments with research to avoid local optimizations that hurt long‑term experience.[web:146][web:149][web:155][web:154][web:148]
- Use A/B tests where stakes and traffic justify the overhead; use other methods (e.g., qualitative tests, prototypes) when they don’t.

### Designers feel intimidated by stats

- Focus on structuring strong hypotheses and understanding direction/magnitude of effects.
- Partner with data specialists for statistical details and validity checks.[web:141][web:143][web:145][web:150]
- Build familiarity gradually by reviewing a few experiments end‑to‑end.

---

## Notes for use with other skills

- Use this skill with:
  - `product-discovery-opportunity` to validate opportunities and solution ideas with experiments.[web:362][web:372]
  - `product-ux-strategy-alignment` to tie experiments to strategic outcomes and roadmap bets.[web:126][web:369]
  - `ux-product-design-metrics` to define HEART/AARRR/GSM metrics and guardrails before testing.[web:369][web:373]
  - `ux-prototyping-validation` and `ux-user-research` to generate strong hypotheses and interpret results via mixed methods.[web:146][web:149][web:325]
