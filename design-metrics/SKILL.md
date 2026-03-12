---
name: ux-product-design-metrics
description: >
  Choose and apply UX and product design metrics that matter: task performance,
  behavioral, attitudinal, and business metrics, plus HEART, GSM, AARRR, North
  Star, and PULSE frameworks.
metadata:
  domain: foundations
  category: metrics
  author: your-name
  version: 1.0.0
---

# UX & Product Design Metrics

## Purpose

Use this skill to define, explain, and select UX and product metrics that connect design work to real outcomes.[web:303][web:308][web:311] It covers task performance, behavioral, attitudinal, and business metrics, plus core frameworks (HEART, GSM, AARRR, North Star, PULSE).[web:303][web:306][web:310][web:313]

## When to use

Use this skill when:

- Designing or auditing a feature, flow, or product and you need **clear success metrics**.
- Translating business or product goals into **measurable UX and product metrics**.
- Explaining **why certain metrics matter** to stakeholders.
- Comparing or choosing between **metric frameworks** for an initiative.

---

## Step 1: Clarify goals before picking metrics

1. Ask what problem or opportunity the team is targeting.
   - Example: “Reduce abandonment in checkout” or “Increase activation for new workspaces.”
2. Identify the **user outcome** and the **business outcome**.
   - User outcome: easier, faster, less frustrating.
   - Business outcome: more conversions, higher retention, lower support.
3. Note the key flows or features involved.
   - Example: onboarding wizard, search, cart, dashboard.

Use this step to prevent “metrics shopping” and anchor everything in goals.[web:308][web:312]

---

## Step 2: Task performance metrics (can users do the thing?)

Use this step for **usability tests, critical flows, and before/after UX changes.**[web:288]

### 2.1 Task Success Rate

- Definition: Percentage of tasks users complete successfully without critical errors.
- Use when: You need to know if users can finish key tasks (checkout, booking, create shipment).
- Example metric: “90% of new users can complete onboarding within 5 minutes.”

### 2.2 Time on Task

- Definition: Time it takes to complete a specific task.
- Use when: You care about **efficiency** and friction.
- Notes:
  - Shorter is usually better, but watch that speed does not increase errors.
  - Use medians to reduce outlier impact.

### 2.3 Error Rate

- Definition: Frequency of mistakes while attempting a task (input errors, wrong paths, validation failures).[web:288]
- Use when: Errors have high risk (money, privacy, critical operations).
- Example metric: “Reduce failed form submissions from 18% to 8%.”

### 2.4 Learnability

- Definition: How quickly new users can learn to use the product effectively.
- Signals:
  - Improvement between first and second attempts.
  - Time or sessions until users complete key tasks without assistance.
- Use when: Redesigning IA, onboarding, or workflows aimed at new users.

---

## Step 3: Behavioral metrics (what users actually do)

Use this step for **live product behavior** and to evaluate ongoing engagement.[web:306][web:313]

### 3.1 Engagement Rate

- Definition: How actively users interact with the product or features.
- Examples:
  - Sessions per user, actions per session, meaningful actions per week.
- Guidance:
  - Focus on **meaningful engagement** (value‑creating actions), not just time spent.

### 3.2 Retention Rate

- Definition: Percentage of users who return and keep using the product over time.[web:311]
- Types:
  - D1 / D7 / D30 retention, weekly/monthly active retention, cohort retention.
- Use when: Measuring long‑term value and stickiness.

### 3.3 Feature Adoption Rate

- Definition: Users who use a feature ÷ eligible users in a time window.
- Use when: Launching or iterating on features.
- Track both:
  - Initial adoption (did they try it?).
  - Sustained usage (do they keep using it?).

### 3.4 Bounce Rate

- Definition: Percentage of visits where users leave after a single page or screen.[web:296]
- Use when: Evaluating landing pages, marketing pages, or entry screens.
- Caveat: A high bounce rate can mean quick success or poor relevance—interpret with context.

### 3.5 Pages (or Screens) per Session

- Definition: Average number of pages/screens viewed per session.[web:301]
- Use when: Understanding browsing depth and exploration.
- Interpret with task context:
  - More pages can mean curiosity or confusion; fewer can mean efficiency or lack of engagement.

---

## Step 4: Attitudinal metrics (what users say and feel)

Use this step for **perception, satisfaction, and loyalty.**[web:311]

### 4.1 System Usability Scale (SUS)

- Definition: Standardized 10‑item questionnaire producing a usability score (0–100).[web:288]
- Use when: You want a quick, comparable measure of perceived usability across releases.
- Interpretation: ~68 is often cited as “average”; higher scores indicate better perceived usability.

### 4.2 Net Promoter Score (NPS)

- Definition: “How likely are you to recommend this product to a friend or colleague?” on a 0–10 scale.
- Calculation:
  - Promoters (9–10), Passives (7–8), Detractors (0–6).
  - NPS = % Promoters − % Detractors.
- Use when: Measuring loyalty and long‑term relationship health.

### 4.3 Customer Satisfaction (CSAT)

- Definition: Satisfaction with a specific interaction or feature, usually on a 1–5 or 1–7 scale.
- Use when: Evaluating discrete experiences (support interaction, feature usage, checkout).
- Example: “How satisfied were you with [X]?” (Very dissatisfied → Very satisfied).

### 4.4 Customer Effort Score (CES)

- Definition: How easy it was to complete a task or resolve an issue.[web:293]
- Typical item: “It was easy for me to [do X]” with agreement scale.
- Use when: Reducing friction and support load; easier experiences correlate with loyalty.

### 4.5 User Sentiment Analysis

- Definition: Qualitative or automated analysis of user opinions and emotions.
- Sources:
  - Open‑ended survey responses, interviews, reviews, support tickets, social feedback.
- Use when: You need nuanced understanding behind metrics (e.g., “why NPS dropped”).

---

## Step 5: Business impact metrics (connect UX to outcomes)

Use this step to **show how UX work affects revenue, growth, and cost.**[web:309][web:317]

### 5.1 Conversion Rate

- Definition: % of users who complete a desired action (macro or micro conversions).
- Examples:
  - Account creation, checkout completion, upgrade to paid plan, feature enablement.
- Use when: Evaluating flows that end in a clear “yes/no” outcome.

### 5.2 Cart Abandonment Rate

- Definition: % of users who add items to cart but do not complete purchase.[web:301]
- Formula: (Carts with no purchase ÷ Carts with items) in a time period.
- Influence via:
  - Clear pricing, reduced friction, fewer surprises, trust and security signals.

### 5.3 Return on Investment (ROI) for UX

- Definition: Financial return from UX work relative to its cost.
- Simple framing: (Benefit − Cost) ÷ Cost.
- Benefits may include:
  - Increased conversion, higher retention, lower support cost, higher NPS/CSAT linked to revenue.

### 5.4 Revenue per User

- Variants: ARPU, ARPPU, LTV.
- Use when: Understanding how UX changes affect monetization (e.g., clearer upgrade flows, better packaging).
- Combine with retention and satisfaction to avoid revenue‑at‑all‑costs.

### 5.5 Support Ticket Reduction

- Definition: Reduction in support volume and severity after UX changes.
- Use when: You aim to remove confusion and prevent issues.
- Evidence:
  - Fewer tickets in specific categories.
  - Lower handling time or escalations.

---

## Step 6: Use metric frameworks to structure choices

Use this step to **pick the right metrics and avoid vanity metrics.**[web:303][web:308][web:310][web:313]

### 6.1 HEART Framework (Google)

Five UX dimensions:[web:303][web:311][web:315]

- **Happiness** – Attitudes and satisfaction (CSAT, NPS, SUS, qualitative feedback).
- **Engagement** – Frequency, intensity, and depth of use (actions per session, active days).
- **Adoption** – New users or feature uptake (new accounts, new feature usage).
- **Retention** – Continued use over time (cohort retention, churn rate).[web:311]
- **Task Success** – Effectiveness and efficiency (success rate, time on task, error rate).

Use HEART to ensure you cover subjective, behavioral, and task outcomes, not just one dimension.[web:303][web:306]

### 6.2 Goals–Signals–Metrics (GSM)

A process for translating goals into measurable outcomes.[web:308][web:312][web:316]

1. **Goals** – What are we trying to achieve for users and the business?
2. **Signals** – What behaviors or events would indicate we’re succeeding?
3. **Metrics** – How will we quantify those signals?

Example:
- Goal: “Onboarding feels effortless.”
- Signals: Fewer abandoned setups, fewer related support tickets.
- Metrics: Setup completion rate, time to first value, tickets about onboarding.

### 6.3 AARRR (Pirate Metrics)

A growth‑oriented funnel covering the user lifecycle.[web:309][web:313][web:317]

- **Acquisition** – How users find and sign up (visits, signups, CAC).
- **Activation** – First value moments (activation rate, time to activate).[web:317]
- **Retention** – Do they come back? (cohort retention, churn).
- **Revenue** – How value is monetized (ARPU, MRR, expansion revenue).[web:309]
- **Referral** – Do they bring others? (invite rate, referral conversion).

Use AARRR when framing product metrics across marketing, onboarding, and lifecycle.

### 6.4 North Star Metric

A single metric that captures the **core value delivered** to customers.

- Criteria:
  - Reflects customer value, not just internal activity.
  - Correlates with long‑term sustainable growth.
  - Can be influenced by product and UX changes.

Examples:
- Completed shipments per active customer.
- Weekly active collaborative documents.
- Songs or minutes listened per week.

### 6.5 PULSE Framework

Operational product health metrics.[web:310][web:314]

- **Page Views** – Overall activity volume.
- **Uptime** – Availability of the product (reliability).
- **Latency** – Response and load times (performance).
- **Seven‑Day Active Users** – Short‑term active usage.
- **Earnings** – Revenue generated.

Use PULSE alongside HEART and UX metrics so performance and reliability are tracked with experience quality.[web:310][web:314]

---

## Step 7: Putting it all together

When you need to define metrics for a project:

1. **Start with goals**  
   - Define user and business goals (Step 1).

2. **Choose a framework**  
   - HEART for UX quality and experience.
   - AARRR for lifecycle and growth.
   - PULSE for reliability and performance.
   - Use GSM to connect goals → signals → metrics.

3. **Select a minimal metric set**  
   - Pick 1–3 primary metrics from:
     - Task performance (Step 2),
     - Behavioral (Step 3),
     - Attitudinal (Step 4),
     - Business impact (Step 5).
   - Add a few guardrail metrics (e.g., error rate, support tickets) so improvements do not create new problems.

4. **Baseline, then measure change**  
   - Capture metrics before changes.
   - Measure after release or experiment.
   - Combine numbers with qualitative insights to explain “what” and “why”.

Use this skill to keep your metric choices intentional, minimal, and tightly aligned to user and business value.
