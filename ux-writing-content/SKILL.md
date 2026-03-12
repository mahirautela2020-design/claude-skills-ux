---
name: ux-writing-content
description: >
  Helps design clear, effective UX copy. Use when the user needs help writing
  or refining labels, microcopy, empty states, error messages, helper text, and
  onboarding flows, or when improving structure for scannability, tone, and
  comprehension. Focuses on practical UX writing guidance at an awareness
  level that works alongside visual, interaction, IA, principles, and metrics.
metadata:
  domain: ux
  category: content
  author: your-name
  version: 1.1.0
---

# UX Writing & Content Design (Awareness)

## Purpose

This skill supports creating clear, helpful interface copy that works with interaction and visual design.[web:233] It covers labels, microcopy, empty states, error and helper messages, and simple onboarding content, with an emphasis on scannability, appropriate tone, user comprehension, and alignment to shared principles (`ux-design-principles`) and metrics (`ux-product-design-metrics`).[web:260][web:303]

Use this skill whenever you need to refine UI text so that users understand what things are, what will happen, and what they should do next.

---

## Instructions

### Step 1: Clarify context, user, and action

Before writing any copy, clarify:

- **Context** – where the text appears (button, form, dialog, empty state, onboarding step).
- **User** – who is reading it (role/segment, expertise, emotional state).
- **Action or outcome** – what we need the user to understand or do.

Ask:

- "What is the user trying to do at this moment?"
- "What happens if they succeed or fail here?"
- "How experienced are they with this product or domain?"

Summarize this in 2–3 lines; use it to guide wording, tone, and the level of detail, and to connect to relevant metrics later (e.g., task success, CSAT, CES) via `ux-product-design-metrics`.[web:288][web:293]

---

### Step 2: Write clear, action-oriented labels

For buttons, links, and controls, prioritize **clarity over cleverness**.[web:233]

Guidelines:

- Use **verbs** that describe the action (e.g., “Save draft”, “Send invoice”, “Download report”) instead of vague labels (“OK”, “Submit”, “Next” where possible).
- Avoid jargon where a plain-language alternative exists.
- Keep labels short but specific enough that users know what will happen.

For pairs of actions (e.g., primary vs secondary):

- Make the primary action explicit (e.g., “Save changes” vs “Discard”).
- Avoid symmetrical ambiguity (two similar-sounding options that do very different things).

Document:

- Control → Label → Purpose
- Any important distinctions between similar labels.

Ensure labels are consistent with IA and navigation terminology from `ux-information-architecture`, and with the principles of match with real world and recognition over recall from `ux-design-principles`.[web:288][web:110][web:238]

---

### Step 3: Design helpful microcopy and helper text

Microcopy supports users in understanding fields, choices, and consequences.[web:233]

For fields and settings:

- Use **helper text** to clarify what is expected (format, examples, constraints).
- Place helper text close to the relevant control.
- Use concise, plain sentences or fragments (e.g., “Used for account recovery only”).

For sensitive or risky actions:

- Briefly explain **what will happen** and **whether it can be undone**.
- Example: “This will permanently delete the project and all associated data. This action cannot be undone.”

Avoid:

- Overly technical explanations unless necessary; translate into user terms.
- Wall-of-text helper sections; aim for the minimum needed to unblock users.

Tie helper text and microcopy to interaction behaviour defined in `ux-interaction-design` (states, constraints, feedback) so what you say matches what the system does.[web:240][web:243]

---

### Step 4: Craft empty states that guide next steps

Empty states are opportunities to orient and guide users, not just “no data” screens.[web:233]

For lists, dashboards, or features with no content yet:

- Explain **why** it’s empty (e.g., “You haven’t created any reports yet.”).
- Suggest **what to do next** (e.g., “Create your first report to track campaign performance.”).
- Provide a clear **primary action** (button) in the empty state when appropriate.

If data is empty due to filters or conditions:

- Clarify the condition (“No results match your filters.”).
- Suggest how to adjust filters or broaden criteria.

Keep empty states friendly but focused on helping users make progress, and ensure labels/actions align with IA and interaction patterns.

---

### Step 5: Write clear, actionable error messages

Error messages should reduce frustration and help users recover.[web:288][web:293]

Guidelines:

- Say **what went wrong** in simple terms.
- Say **why**, if known, without exposing raw technical details.
- Tell users **what to do next** or how to fix it.

Patterns:

- Field validation error: “Enter a valid email address, like name@example.com.”
- Limit error: “You can upload up to 5 files. Remove one to add another.”
- System error: “We couldn’t save your changes. Check your connection and try again.”

Avoid:

- Blaming language (“You did X wrong”); focus on the problem, not the user.
- Generic errors like “Something went wrong” without additional guidance, unless it’s truly unknown and you provide a next step (retry, contact support).

Ensure error copy supports the error-handling patterns defined in `ux-interaction-design` and respects accessibility guidance from `ux-design-principles` (e.g., where messages appear, how they are announced).[web:240][web:293]

---

### Step 6: Structure content for scannability

Ensure content is easy to scan and understand, especially in dense or important screens.[web:233]

Techniques:

- Use **meaningful headings** and subheadings.
- Use short paragraphs and bullet lists for multiple points.
- Front-load key information at the beginning of sentences or headings.
- Prefer simple sentence structures and avoid unnecessary qualifiers.

For onboarding or multi-step instructions:

- Break up complex tasks into numbered steps.
- Keep each step focused on a single action or decision.
- Use consistent phrasing and formatting across steps.

Check that users can skim the page or dialog and still understand:

- Where they are.
- What options exist.
- What the primary action is.

These principles connect back to hierarchy, visual design, and cognitive load in `ux-design-principles`.[web:230][web:238]

---

### Step 7: Maintain appropriate tone and voice

Align tone with context, brand, and user emotional state.[web:233]

Consider:

- **High-stress moments** (errors, payments, security) → clear, calm, direct; avoid jokes and slang.
- **Exploratory moments** (onboarding tips, success messages) → can be more encouraging or warm, but still concise.
- **Professional contexts** (B2B tools, enterprise workflows) → straightforward, respectful, minimal fluff.

Guidelines:

- Use “you” to address the user where natural.
- Avoid over-familiarity or forced humour, especially in error states.
- Keep terminology consistent across the product (choose one term for a concept and stick to it).

When tone and voice are closely tied to perceived usability and satisfaction, connect them to attitudinal metrics (CSAT, NPS, SUS) through `ux-product-design-metrics` when evaluating impact.[web:311][web:293]

---

### Step 8: Align copy with interaction and IA

Ensure UX text is consistent with the structure and behaviour defined in other skills.[web:110][web:240]

Check:

- Labels match IA and navigation names (no “Projects” in one place and “Jobs” in another for the same concept).
- Button and link labels match the actual action (and any subsequent screens).
- Empty states and messages reference the right flows and options (e.g., correct feature names, steps, or settings).

Where there is a mismatch, adjust either the copy or the underlying design so they tell a coherent story, guided by consistency and match-with-real-world principles in `ux-design-principles`.[web:288][web:260]

---

### Step 9: Provide examples and patterns for reuse

When possible, generalize examples into **patterns** the team can reuse.[web:233]

For example:

- Confirmation dialogs:
  - Title: “Are you sure you want to [action]?”
  - Body: brief impact statement.
  - Primary button: “[Action]”
  - Secondary: “Cancel”
- Error message pattern:
  - What happened + how to fix + optional extra detail.
- Empty state pattern:
  - Statement of state + reason + recommended next step + primary action.

Document these as small pattern snippets that can be applied across multiple features and link them to components or patterns in your design system and `ux-design-principles` so terminology and behaviour stay aligned.[web:210][web:260]

---

## Examples

### Example 1: Form field and error

- Field label: “Company name”
- Helper text: “Use your legal business name or trading name.”
- Error: “Enter a company name with at least 2 characters.”

### Example 2: Empty state

- Context: Reports page with no reports.
- Copy:
  - Title: “No reports yet”
  - Body: “Create your first report to track how your campaigns perform over time.”
  - Primary action: “Create report”

### Example 3: Onboarding tooltip

- Context: First time a user sees a complex dashboard.
- Copy:
  - “Pin your most important metrics here so they’re always at the top of your dashboard.”

---

## Troubleshooting

### Copy is too long or dense

- Break it into shorter sentences or bullets.
- Remove non-essential background; keep what users need now.
- Move details into helper text or a secondary area if necessary.

### Users misinterpret actions

- Check whether the label or message could be read in more than one way.
- Make the label more specific (“Delete project” vs “Delete”).
- Add a short explanatory line near risky actions.

### Tone feels off

- Revisit user context: are they stressed, busy, or exploring?
- Remove jokes or idioms in critical paths.
- Use neutral, respectful language, especially around errors and limitations.

---

## Notes for use with other skills

- Use this skill together with:
  - `ux-interaction-design` to ensure copy supports interaction behaviour, states, errors, and feedback.[web:240][web:243]
  - `ux-information-architecture` so labels and headings match the structure and navigation.[web:110]
  - `ux-design-principles` to align copy with heuristics, inclusive design, and content principles (e.g., clarity, recognition over recall, accessibility).[web:260][web:293]
  - `ux-product-design-metrics` when copy changes are part of experiments or need to be tied to metrics like task success, conversion, CSAT, CES, or NPS.[web:303][web:311]
  - Product and experimentation skills when messaging impacts trust, onboarding, and adoption.
