---
name: collab-ux-engineering
description: >
  Strengthens cross-functional collaboration between UX and engineering. Use
  when the user needs help involving engineers early, discussing feasibility
  and constraints, aligning on trade-offs, and supporting implementation (code
  reviews, QA, design-debt tracking) while protecting UX intent and shared
  outcomes.
metadata:
  domain: collaboration
  category: ux-engineering
  author: your-name
  version: 1.1.0
---

# Cross-functional Collaboration with Engineering

## Purpose

This skill helps designers and engineers work as true partners instead of separate handoff stages.[web:186][web:188][web:190][web:191][web:194][web:198] It focuses on involving engineering early, making constraints explicit, aligning on trade-offs, and supporting implementation and QA so that scope changes don’t quietly erode critical UX quality, while staying grounded in design system, accessibility, and outcome/metrics practices from related skills.[web:189][web:191][web:194][web:196][web:192]

Use this skill when starting new projects, refining complex flows, or navigating delivery and scope decisions with engineering teams.

---

## Instructions

### Step 1: Align on shared goals and constraints

Begin by establishing a **shared picture** of what you’re building and under what constraints.[web:190][web:191][web:194][web:198]

In a joint kickoff with PM and engineering, clarify:

- Product and UX goals for this project or release (link to strategy and metrics where possible).
- Key user journeys and problems you’re solving.
- Constraints:
  - Technical (platforms, performance, legacy systems, APIs).
  - Design (brand, accessibility, patterns, design system).
  - Business (timelines, compliance, budget).[web:191][web:195][web:199]

Capture this in a short, shared document or board so everyone has the same reference, and connect it to opportunity/metrics artefacts from `product-ux-strategy-alignment` and `ux-product-design-metrics` where relevant.

---

### Step 2: Involve engineers early in discovery and ideation

Bring engineers into **discovery and early design**, not only at handoff.[web:186][web:187][web:190][web:191][web:194][web:198]

Examples:

- Invite engineers to:
  - Problem-framing sessions and workshops.
  - Key research readouts and synthesis sessions.
  - Early sketching/ideation (even simple whiteboard or FigJam sessions).
- Ask for:
  - Feasibility concerns.
  - Opportunities they see from a technical perspective.
  - Ideas for simpler implementations that still meet user needs.[web:190][web:191][web:194][web:195]

This builds shared ownership, surfaces constraints earlier, and prevents designs that are beautiful but impractical.

---

### Step 3: Make constraints explicit and design within them

Turn vague “constraints” into **explicit inputs** to design.[web:191][web:195][web:199]

Work with engineering to list:

- Technical constraints:
  - Performance budgets, API limits, legacy dependencies, security/privacy requirements.
- Platform constraints:
  - Supported devices/browsers, interaction modes, offline/online behaviour.[web:195][web:194]
- Implementation constraints:
  - Existing systems, component library capabilities, team capacity and skills.

Design within these guardrails where possible, and note where you’re intentionally pushing them so trade-offs can be discussed early.[web:189][web:191][web:199] Reflect relevant constraints back into `ui-design-systems-components`, `ui-platform-patterns-responsive`, and accessibility skills when they are systemic.

---

### Step 4: Co-develop solutions and trade-off options

When exploring solutions, **co-create options** with engineering instead of pushing a single proposal.[web:189][web:191][web:194]

For important flows or features:

- Present 2–3 options that vary in:
  - UX impact.
  - Technical complexity.
  - Time-to-deliver.
- Discuss:
  - What each option implies for performance, maintainability, and risk.
  - How each option affects user value and outcome metrics.

Capture trade-offs explicitly (e.g., “Option B reduces time-to-market but hides advanced controls behind an extra step”).[web:189][web:191][web:190][web:198] Tie these options back to opportunities and metrics from `product-discovery-opportunity` and `product-ux-strategy-alignment` so decisions stay outcome-focused.

---

### Step 5: Create implementation-ready specs with engineering input

Prepare **implementation-friendly** design specs and flows.[web:188][web:191][web:194]

With engineering input, ensure specs include:

- User flows and edge cases.
- Component usage and states (aligned with the design system and atomic components).
- Behaviour details (interactions, loading, error and empty states).
- Responsive or adaptive behaviour, where relevant.
- Accessibility expectations (focus order, keyboard interactions, semantics).[web:191][web:195]

Review specs with engineering before development begins to:

- Confirm shared understanding.
- Adjust where small changes can reduce complexity without harming UX intent.[web:186][web:188][web:191][web:194]

Connect specs to `ui-design-tools-handoff` practices and ensure mapping to code components is clear.

---

### Step 6: Stay involved during implementation and QA

Treat implementation as a **collaborative build phase**, not a one-time handoff.[web:186][web:188][web:190][web:194][web:196]

Practices:

- Join regular check-ins or standups to surface design/engineering questions early.
- Offer design pairing or “office hours” with engineers for complex parts.
- Participate in:
  - Design reviews of implemented UI (e.g., staging environments).
  - QA reviews focused on UX, accessibility, and interaction issues.[web:196][web:200]

Log implementation bugs and UX gaps with clear descriptions and priority based on user impact, using `ux-usability-heuristics` and `ux-accessibility-inclusive-design` as reference.

---

### Step 7: Track design debt alongside technical debt

Make **design debt** visible similar to technical debt.[web:192][web:196][web:200]

Examples of design debt:

- Inconsistent use of components or patterns across screens.
- Missing states or edge cases in implemented UI.
- UX shortcuts taken to meet deadlines.

Practices:

- Create design-debt items in the same issue tracker as dev/tech debt.
- Tag them clearly (e.g., `design-debt`) and note:
  - User impact.
  - Where and why the compromise was made.
- Periodically review and prioritize design-debt alongside tech debt in planning.[web:192][web:196][web:200]

Where debt is systemic, loop it back into `ui-design-systems-components` and roadmap discussions so it can be addressed intentionally.

---

### Step 8: Negotiate scope without losing core UX intent

When timelines or constraints force scope changes, negotiate around **scope, time, and quality**, not just saying “yes” or “no”.[web:189][web:191][web:195][web:193][web:197]

Strategies:

- Identify **MVP** UX:
  - What is the minimum acceptable experience that still meets core user needs?
  - What can be simplified or deferred without breaking key journeys?
- Offer structured options:
  - Swap: “If we add X, we can drop Y of similar effort.”
  - Phase: “Ship a simpler version now, plan a second pass for advanced controls.”
- Make user impact explicit:
  - Explain which user problems will or won’t be solved in v1 and how that affects outcomes.

Confirm decisions in writing (ticket descriptions, docs) so everyone knows what’s in/out and what is debt to revisit later.[web:193][web:197] Align with PMs using `product-ux-strategy-alignment` so compromises stay visible at roadmap level.

---

### Step 9: Build long-term trust and shared practice

Over time, aim for **ongoing partnership**, not project-by-project alignment.[web:186][web:190][web:191][web:194][web:198]

Behaviours:

- Invite engineers to research and usability sessions; share learnings that affect their work.
- Learn basics of the tech stack; be curious about performance, scalability, and code constraints.
- Celebrate joint wins where good collaboration produced better outcomes.
- Reflect together in retros:
  - What worked well in design/engineering collaboration?
  - What should we change for next time?

This shared practice increases speed, quality, and job satisfaction across both disciplines, and strengthens the link between UX, engineering, and measurable product outcomes.

---

## Examples

### Example 1: Complex new workflow

- Early collaboration:
  - Engineers joined discovery sessions and journey mapping.
- Co-designed options:
  - Three implementation options with different levels of automation and complexity, each with explicit trade-offs.
- Scope negotiation:
  - Team chose an MVP path that delivered key user value while planning a second phase for advanced automation.
- Implementation:
  - Designers joined dev reviews and QA passes to keep UX intent and accessibility intact.

### Example 2: Refactoring legacy UI with design system

- Goal:
  - Replace inconsistent legacy screens with design-system-based UI.
- Collaboration:
  - Designers and engineers audited existing patterns and agreed on target components.
- Debt tracking:
  - Items that couldn’t be updated due to time/tech constraints were logged as design and tech debt with clear rationale.
- Outcome:
  - Gradual improvement of UX and codebase, with shared understanding of remaining gaps and their user impact.

---

## Troubleshooting

### Engineers feel design is unrealistic

- Bring them into problem framing and ideation earlier.
- Ask for feasibility input before committing to high-fidelity solutions.
- Show willingness to adjust designs based on real constraints while protecting core user needs.[web:186][web:187][web:190][web:191][web:194]

### Designers feel UX is being compromised too often

- Make trade-offs explicit: document user impact and what is being deferred.
- Align with PM on which experiences are non-negotiable for users.
- Use experiments and metrics (`product-experimentation-data`, `ux-product-design-metrics`) to demonstrate where UX quality matters most.[web:189][web:191][web:195]

### Handoffs still cause confusion and rework

- Move from one-time handoffs to continuous collaboration:
  - Shared tools (Figma, Storybook, comments).
  - Regular syncs focused on open questions and edge cases.[web:188][web:190][web:194]
- Standardize specs and design system use so both sides speak the same component language (`ui-design-systems-components`, `ui-design-tools-handoff`).

---

## Notes for use with other skills

- Use this skill with:
  - `ui-design-systems-components` and `ui-design-tools-handoff` to align design and code components and improve handoff quality.
  - `ui-visual-design-layout`, `ux-accessibility-inclusive-design`, and `ux-usability-heuristics` when reviewing builds and logging UX issues.
  - `product-ux-strategy-alignment` and `product-discovery-opportunity` to ensure collaboration decisions stay tied to strategy, opportunities, and metrics.
  - `product-experimentation-data` when working with engineering on outcome-focused iterations and experiments.
