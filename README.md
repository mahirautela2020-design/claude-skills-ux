
# UX / UI / Product Design Skills for Claude

This repository contains a set of Claude skills that encode industry‑standard UX, UI, and Product Design workflows. Each skill is a standalone folder with its own `SKILL.md` file, instructions, and optional references.[web:318][web:319]

In addition to workflow‑specific skills (research, IA, interaction, etc.), this repo includes **two foundation skills**:

- `ux_design_principles` – canonical library of UX/UI principles and laws.
- `ux_product_design_metrics` – canonical library of UX/product metrics and frameworks.

Other skills should reference these foundations instead of redefining principles or metrics.

---

## Repository structure

```text
ux-ui-product-design-skills/
├── README.md
├── ux-mindset-problem-framing/
│   ├── SKILL.md
│   └── references/
├── ux-user-research/
│   ├── SKILL.md
│   └── references/
├── ux-information-architecture/
│   ├── SKILL.md
│   └── references/
├── ux-interaction-design/
│   ├── SKILL.md
│   └── references/
├── ux-writing-content/
│   ├── SKILL.md
│   └── references/
├── ux-prototyping-validation/
│   ├── SKILL.md
│   └── references/
├── ux-usability-heuristics/
│   ├── SKILL.md
│   └── references/
├── ux-accessibility-inclusive-design/
│   ├── SKILL.md
│   └── references/
├── ux-design-principles/
│   ├── SKILL.md
│   └── references/
├── ux-product-design-metrics/
│   ├── SKILL.md
│   └── references/
├── ui-visual-design-layout/
│   ├── SKILL.md
│   └── references/
├── ui-design-systems-components/
│   ├── SKILL.md
│   └── references/
├── ui-platform-patterns-responsive/
│   ├── SKILL.md
│   └── references/
├── ui-design-tools-handoff/
│   ├── SKILL.md
│   └── references/
├── product-discovery-opportunity-sizing/
│   ├── SKILL.md
│   └── references/
├── product-ux-strategy-alignment/
│   ├── SKILL.md
│   └── references/
├── product-experimentation-data-literacy/
│   ├── SKILL.md
│   └── references/
├── collab-stakeholder-communication/
│   ├── SKILL.md
│   └── references/
├── collab-workshop-facilitation/
│   ├── SKILL.md
│   └── references/
├── collab-eng-collaboration/
│   ├── SKILL.md
│   └── references/
├── collab-design-ops-process/
│   ├── SKILL.md
│   └── references/
└── collab-leadership-mentoring/
    ├── SKILL.md
    └── references/
```

> Note: `README.md` lives only at the repo root. Each skill folder contains its own `SKILL.md` but no README inside the skill folder.[web:318]

---

## Skill overview

### UX foundations

- **UX Mindset & Problem Framing**  
  Clarifying the “why”, problem statements, and constraints before jumping into solutions. Linking user problems, business goals, and technical reality; reframing vague asks into testable hypotheses.

- **User & Market Research**  
  Planning and running qualitative methods (interviews, contextual inquiry, diary studies) and basic quant (surveys, simple analytics reads). Competitor/market scans, benchmarking, UX audits, and synthesizing into personas, jobs‑to‑be‑done, and opportunity areas.

- **Information Architecture & Flows**  
  Structuring content and functionality (sitemaps, navigation models, taxonomies, tags). Designing task/user flows, service blueprints, and state diagrams across channels.

- **Interaction Design & Behavior**  
  Defining states, edge cases, error flows, and system feedback. Choosing appropriate patterns, anticipating user behavior, and balancing simplicity vs control.

- **UX Writing & Content Design (awareness)**  
  Writing or collaborating on clear labels, microcopy, empty states, error messages, and onboarding. Ensuring content structure supports scannability, tone, and comprehension.

- **Prototyping & Validation**  
  Low‑, mid‑, and high‑fidelity prototypes; choosing fidelity based on risk and stage. Setting up and running concept tests and usability tests with prototypes, translating findings into design changes.

- **Usability Evaluation & Heuristics**  
  Heuristic reviews, UX audits, and accessibility checks as part of regular practice. Prioritizing issues by impact and effort and communicating them to product and engineering.

- **Accessibility & Inclusive Design**  
  Applying accessibility standards (contrast, keyboard, semantics) at design time, not just in QA. Considering a range of devices, abilities, and contexts; designing alternatives where needed.

- **Design Principles (Foundations)** – `ux-design-principles`  
  Canonical reference for UX and UI principles: 21 Laws of UX, Gestalt principles, interaction design principles, inclusive design, accessibility (WCAG/POUR), cognitive psychology, ethical design and dark patterns, calm technology, design tokens & systems, UI patterns, luxury design, Atomic Design, color theory, data visualization basics, content design, IA, mobile & touch guidelines, motion design, iOS/Android guidelines, and web performance/Core Web Vitals.[web:260][web:272][web:280][web:230][web:295][web:239]

- **UX & Product Design Metrics (Foundations)** – `ux-product-design-metrics`  
  Metrics and frameworks for measuring design success: task performance (task success, time on task, error rate, learnability), behavioral metrics (engagement, retention, feature adoption, bounce rate, pages/screens per session), attitudinal metrics (SUS, NPS, CSAT, CES, sentiment), and business metrics (conversion, cart abandonment, revenue per user, support ticket reduction, UX ROI). Includes HEART, Goals‑Signals‑Metrics (GSM), AARRR (pirate metrics), North Star Metric, and PULSE frameworks.[web:288][web:303][web:308][web:310][web:313]

---

### UI / visual and systems skills

- **Visual Design & Layout**  
  Using hierarchy, spacing, grids, typography, color, and imagery to guide attention and meaning. Designing for different breakpoints/densities while keeping visual consistency.

- **Design Systems & Components**  
  Creating, documenting, and evolving tokens, components, and patterns. Covering component states, variants, usage guidelines, and contribution/governance models.

- **Platform Patterns & Responsiveness**  
  Applying platform conventions (web, iOS, Android, desktop) and deciding when to follow vs invent. Designing responsive/adaptive behavior: grids, breakpoints, touch vs pointer paradigms.

- **Design Tools & Handoff**  
  Proficiency with Figma and related tools for components, auto‑layout, prototyping, and design specs. Preparing developer‑ready outputs (specs, annotations, tokens) and answering implementation questions.

---

### Product thinking & strategy

- **Product Discovery & Opportunity Sizing**  
  Turning insights and stakeholder input into opportunity areas, problem definitions, and hypotheses. Using simple frameworks (JTBD, opportunity trees, etc.) to prioritize what to explore.

- **Product & UX Strategy Alignment**  
  Connecting design work to product strategy, roadmaps, and success metrics. Identifying where design can move key metrics (activation, retention, satisfaction) and quantifying impact.

- **Experimentation & Data Literacy**  
  Defining measurable hypotheses, collaborating on A/B tests or experiments, and reading basic experiment results. Using analytics and research together (mixed methods) to decide what to iterate next.

---

### Collaboration, leadership & ops

- **Stakeholder Management & Communication**  
  Clear storytelling in reviews, documenting rationale, and managing feedback loops. Adapting communication for PMs, engineers, executives, and non‑design stakeholders.

- **Workshop Design & Facilitation**  
  Planning and facilitating discovery, ideation, prioritization, and alignment sessions. Using collaborative tools (FigJam, Miro) and methods (crazy 8s, mapping, prioritization) effectively.

- **Cross‑functional Collaboration with Engineering**  
  Involving engineers early, discussing feasibility/constraints, and aligning on trade‑offs. Supporting implementation (reviews, QA, design debt tracking) and negotiating scope without losing UX intent.

- **Design Operations & Process**  
  Contributing to team rituals (crits, design reviews, retros), templates, and documentation. Helping maintain the skills matrix, mentoring, and improving ways of working.

- **Leadership, Mentoring & Influence**  
  Mentoring others, shaping standards, influencing product direction, and driving cross‑team initiatives. Setting quality bars, giving/receiving feedback, and representing design in strategic forums.

---

## How these skills work together

- For **principle‑driven questions** (“Is this a good design?”, “Which law applies here?”) Claude leans on `ux-design-principles` and then applies specific workflow skills (e.g., interaction, IA, accessibility) as needed.[web:260][web:272]
- For **metric and outcome questions** (“How should we measure success?”, “What’s the HEART setup for this flow?”) Claude uses `ux-product-design-metrics` and combines it with product/experiment skills.[web:303][web:308][web:310][web:313]

Other skills assume these two are the **single source of truth** for principles and metrics and reference them instead of duplicating content.

---

## Using these skills with Claude

### In Claude.ai

1. Zip each skill folder individually (for example, `ux-mindset-problem-framing` → `ux-mindset-problem-framing.zip`).  
2. In Claude.ai, go to **Settings → Capabilities → Skills**.  
3. Click **Upload skill** and select the zipped folder.  
4. Enable the skill and start a chat. Claude will auto‑load it when your query matches its description.[web:318]

### In Claude Code

For project‑local skills:

```text
your-project/
└── .claude/
    └── skills/
        ├── ux-mindset-problem-framing/
        ├── ux-user-research/
        └── ux-information-architecture/
```

For global skills (all projects), place the folders in:

```text
~/.claude/skills/
```

Claude Code will automatically discover and use skills from these directories.[web:318][web:331]

---

## Customizing

- Duplicate an existing skill folder to create a new skill.  
- Update the YAML frontmatter in `SKILL.md` (`name`, `description`, `metadata`) and adjust the instructions to match your own UX processes.[web:319]  
- Keep skill folder and `name` fields in kebab‑case, avoid `claude` or `anthropic` in names, and don’t use `<` or `>` in descriptions.[web:319][web:331]
```
