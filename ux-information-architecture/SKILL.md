---
name: ux-information-architecture
description: >
  Designs and documents information architecture and flows. Use when the user
  needs help structuring content and functionality (sitemaps, navigation,
  taxonomies, tagging) or mapping user/task flows, journeys, and service
  blueprints across channels. Covers IA concepts, practical modelling, and
  clear deliverables for product and engineering, aligned to shared UX
  principles and metrics.
metadata:
  domain: ux
  category: structure-and-flows
  author: your-name
  version: 1.1.0
---

# UX Information Architecture & Flows

## Purpose

This skill helps design clear, user-centred structures and flows so people can find, understand, and complete tasks efficiently.[web:110][web:272] It covers information architecture (sitemaps, navigation models, taxonomies, labels, metadata) and flow mapping (task/user flows, journeys, and service blueprints) as used in modern UX practice, and connects to `ux-design-principles` for underlying UX laws and patterns and to `ux-product-design-metrics` for measuring IA/flow success.[web:260][web:303]

Use this skill when you need to organize content or functionality, design or refine navigation, or map how users and systems move through a product or service across screens and channels.

---

## Instructions

### Step 1: Clarify scope and primary tasks

Before designing IA or flows, clarify **what** you’re structuring.

Ask:

- "What kind of product or experience is this (site, app, platform, service)?"
- "What are the top 3–7 tasks users come here to accomplish?"
- "Which parts of the experience are currently confusing, hard to find, or causing drop-off?"

Summarize:

- Product / context
- Primary user tasks / goals
- Known problem areas in navigation or flows

This keeps IA focused on real user and business priorities, not just internal org charts.[web:110]

---

### Step 2: Inventory and cluster content and functionality

Create a **content and functionality inventory** as a foundation for IA.[web:110]

- List pages, sections, tools, and key features that exist or are planned.
- Include important metadata where known (e.g., audience, frequency of use, owner).

Then:

- Cluster related items into groups that make sense from a user perspective (not internal team names).
- Note potential **organization schemes**:
  - By task (things users want to do)
  - By topic or category
  - By audience/role
  - By lifecycle (onboarding, everyday use, advanced, support)

Capture clusters as rough groups that will become top-level sections and sub-sections.

You can refer to `ux-design-principles` for Gestalt principles (proximity, similarity, common region) when deciding how items should be grouped visually and conceptually.[web:272][web:276]

---

### Step 3: Design high-level structure, navigation, and sitemap

Use the inventory and clusters to design a user-centred **structure and navigation model**.[web:110]

Decide:

- **Top-level areas** (e.g., Home, Dashboard, Projects, Reports, Settings).
- **Sub-sections** under each area.
- Whether structure will be:
  - Mostly **hierarchical** (parent → child)
  - Hub-and-spoke
  - Wizard/step-based for key tasks

Draft a **sitemap-style outline**:

- Show levels (top-level, second-level, sometimes third-level).
- Indicate which sections are global nav vs local nav.
- Keep hierarchy as shallow as possible while remaining clear (avoid very deep nesting where users must click through many levels).

Ensure:

- Every important user task has a clear “home”.
- There are no orphaned pages without clear parent/context.

Where relevant, align structure and navigation patterns with platform guidelines covered in `ux-design-principles` (e.g., web, iOS, Android navigation norms).[web:236]

---

### Step 4: Define labels, taxonomies, and metadata

Design **names and vocabularies** that match user language and mental models.[web:110]

For navigation and IA:

- Propose clear, concise labels for:
  - Main navigation items
  - Sub-navigation
  - Categories and filters
- Avoid internal jargon where possible; prefer user-facing terms.

For taxonomies and tagging:

- Identify key dimensions users use to find content (e.g., topic, format, audience, time, status).
- Propose:
  - A small set of controlled categories for each dimension.
  - Tagging rules (what gets tagged with what, and how consistently).

Document:

- Label name → meaning/description
- Category or tag lists
- Any important synonyms or “see also” relationships

You can use findings from `ux-user-research` (user language, mental models) and principles from `ux-design-principles` (match with the real world, recognition over recall) to justify naming decisions.[web:288][web:238]

---

### Step 5: Map task and user flows

Create **task flows** and **user flows** for critical journeys.

Clarify:

- **Task flows** – linear steps required to complete a specific task (e.g., “Create a project”, “Complete checkout”).
- **User flows** – paths users can take through the product, including branches and alternate routes.

For each critical task:

- Define start and end points (entry and successful completion).
- List main steps and decision points in logical order.
- Note variations:
  - New vs existing users
  - Error paths and recovery
  - Optional branches (e.g., skip, save for later)

Represent flows in a way devs and stakeholders can follow (even if you’re not drawing the diagram here):

- Step name
- Screen or area
- Decision rules / conditions
- Expected user/system actions

Focus on reducing unnecessary steps, circular paths, and dead ends. Where relevant, use laws from `ux-design-principles` (e.g., Hick’s Law, Fitts’s Law, error prevention) to simplify flows and improve wayfinding.[web:260][web:288]

---

### Step 6: Map journeys and service blueprints (if cross-channel)

When experiences span multiple touchpoints or teams, create **journey maps** and **service blueprints**.[web:110]

For a key journey (e.g., “Onboard to paid plan”, “File and track a support case”):

- Outline customer/user actions step by step.
- Identify:
  - Frontstage touchpoints (what the user sees: UI, emails, calls).
  - Backstage actions (systems, internal teams, processes).
  - Supporting processes and dependencies.

If documenting a service blueprint, capture:

- Customer actions
- Frontstage (visible) actions
- Backstage (invisible) actions
- Support processes and systems
- Evidence (screens, messages, artifacts)

Use this to spot:

- Gaps where user flows break due to internal processes.
- Handoffs or silos causing delays or confusion.

---

### Step 7: Align IA and flows with research and mental models

Check IA and flows against what you know from research and analytics.[web:325]

- Compare structure and labels to:
  - Words users actually use.
  - How they expect content to be grouped.
  - Where they naturally look for things.
- Confirm that top tasks are easy to start and finish without unnecessary detours.

Where you need to **discover** how users naturally group and name content, plan a **card sorting** study (open, closed, or hybrid) and use the results to refine groupings and labels. Where you need to **validate** a proposed structure, plan **tree testing** to check if users can quickly find items in your IA without the UI “chrome”.[web:110]

Use any existing card sorting or tree-testing results to refine categories and labels where possible.

If you see mismatches (e.g., users think about tasks by “project phase”, but IA is organized “by team”), suggest adjustments to structure or labels and check them against principles in `ux-design-principles` (e.g., recognition over recall, consistency, match with real world).[web:288]

---

### Step 8: Produce clear IA and flow deliverables

Create **clear, shareable artifacts** so product and engineering can implement and test.

Recommended deliverables:

- **IA overview**:
  - Short narrative describing the structure and how it supports key tasks.
- **Sitemap outline**:
  - Hierarchical list of key sections and pages.
- **Navigation spec**:
  - Global nav, local nav, footer, search, and cross-links.
- **Flow specs**:
  - Bullet-based step-by-step descriptions for each key task/user flow.
- **Diagrams** (optional references):
  - Sitemaps, user-flow diagrams, journey maps, service blueprints.

Include:

- IDs or names for each node/step (to reference in tickets and design files).
- Notes about edge cases and future extensibility (how IA can grow without breaking).

Where appropriate, note which success metrics from `ux-product-design-metrics` will be used to evaluate IA changes (e.g., navigation success rate, time to find key content, drop-off on specific steps).[web:303][web:308]

---

## Examples

### Example 1: SaaS dashboard IA and flows

- Context: B2B analytics dashboard where users struggle to find core KPIs.
- IA outcome:
  - Top-level nav: Home, Dashboards, Reports, Alerts, Settings.
  - Dashboards grouped by “My dashboards”, “Team dashboards”, “Templates”.
- Flow outcome:
  - Task flow: “Create a dashboard from a template” with clearly documented steps from entry to first saved dashboard.
- Service blueprint:
  - Shows how data ingestion, processing, and alerting connect to user-facing screens and notifications.

### Example 2: Marketing site sitemap and navigation

- Context: Marketing site has grown organically and navigation is cluttered.
- IA outcome:
  - Content inventory, removal/merge decisions.
  - New sitemap with fewer top-level items and clearer categorization by solutions, industries, resources, and company.
- Navigation outcome:
  - Simplified global nav with labels tested to match user expectations.
  - Footer IA that surfaces key support and legal pages.

---

## Troubleshooting

### Structure mirrors org chart instead of user needs

- Identify where navigation categories are team names or internal systems.
- Propose user-centred alternatives based on tasks, topics, or user segments.
- Use examples of how users would phrase their goals to justify the change.

### Too many levels or pages

- Look for opportunities to merge or flatten sections.
- Prioritize content based on task frequency and importance.
- Keep sitemap as simple as possible while still scalable.

### Competing navigation patterns

- Clarify the **primary navigation model** (e.g., global top nav + contextual side nav).
- Reduce redundant entry points that cause confusion.
- Ensure labels are consistent across menus, breadcrumbs, and headings.

---

## Notes for use with other skills

- Use this skill **after**:
  - `ux-mindset-problem-framing` to understand problem and scope.
  - `ux-user-research` to align IA and flows with actual user mental models and language.
- Combine with:
  - `ux-design-principles` to apply relevant laws, heuristics, accessibility, and platform guidelines when evaluating IA and flows.
  - `ux-product-design-metrics` to define and track navigation and flow success metrics (e.g., findability, task success, time to task, drop-off).[web:260][web:303]
- Feed outputs into:
  - Interaction design and UI skills (for detailed screens and components).
  - Product and engineering planning (for epics/stories aligned to IA and flows).
