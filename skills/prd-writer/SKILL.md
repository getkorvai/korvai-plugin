---
name: prd-writer
preamble-tier: 2
version: 1.0.0
description: |
  Transform a rough feature idea into a structured, actionable Product Requirements Document ready for engineering and design.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [feature_idea]
triggers:
  - "When a product manager or team member has a new feature idea or initiative that needs to be formalized for engineering and design handoff."
metadata:
  source: korvai
  korvai_id: 049c8c95-fc9e-4c7b-bcbf-d6bb5c8c5c6e
  social_hook: Stop writing PRDs from scratch. Paste your feature idea and get a full PRD in seconds. 🚀
  gallery_slug_key: prd-writer
---

# PRD Writer

> Convert a rough feature idea into a complete PRD with clear objectives, user stories, requirements, and success metrics.

**Trigger:** When a product manager or team member has a new feature idea or initiative that needs to be formalized for engineering and design handoff.

**Variables:** `$feature_idea`

---

## Steps

### Step 1: Analyze the feature idea provided below and extract core intent, target users, and the problem being solved:

Analyze the feature idea provided below and extract core intent, target users, and the problem being solved:

$feature_idea

**Checklist:**
- [ ] Core problem is clearly identified
- [ ] Target user segment is defined
- [ ] Key value proposition is apparent

**Template:**
```
Analyze the feature idea provided below and extract core intent, target users, and the problem being solved:

$feature_idea
```

### Step 2: Write the PRD header section: include a one-line feature summary, problem statement (2–3 sentences), goals, and explicitly list what is out of scope.

Write the PRD header section: include a one-line feature summary, problem statement (2–3 sentences), goals, and explicitly list what is out of scope.

**Checklist:**
- [ ] Problem statement is user-centric, not solution-centric
- [ ] Goals are measurable or at least directional
- [ ] At least 2 out-of-scope items are listed

### Step 3: Generate 3–5 user stories in 'As a [user], I want to [action] so that [outcome]' format. Cover the primary happy path and at least one edge case or secondary persona.

Generate 3–5 user stories in 'As a [user], I want to [action] so that [outcome]' format. Cover the primary happy path and at least one edge case or secondary persona.

**Checklist:**
- [ ] Each story has a clear actor, action, and outcome
- [ ] At least one edge case or non-primary user is covered

### Step 4: List functional requirements as numbered acceptance criteria (what the system must do) and non-functional requirements (performance, security, accessibility). Be specific and testable.

List functional requirements as numbered acceptance criteria (what the system must do) and non-functional requirements (performance, security, accessibility). Be specific and testable.

**Checklist:**
- [ ] Each requirement is independently verifiable
- [ ] Non-functional requirements include at least one accessibility or performance item

### Step 5: Define success metrics: list 2–4 KPIs or measurable outcomes that indicate the feature is working, and describe how each would be tracked (e.g., event logging, surveys, funnel analysis).

Define success metrics: list 2–4 KPIs or measurable outcomes that indicate the feature is working, and describe how each would be tracked (e.g., event logging, surveys, funnel analysis).

**Checklist:**
- [ ] Each metric is quantifiable
- [ ] Tracking method is specified for each metric

### Step 6: Add an open questions and dependencies section: surface any unresolved decisions, technical unknowns, cross-team dependencies, or stakeholder approvals needed before build can begin.

Add an open questions and dependencies section: surface any unresolved decisions, technical unknowns, cross-team dependencies, or stakeholder approvals needed before build can begin.

**Checklist:**
- [ ] At least 2 open questions are raised
- [ ] Any external team dependencies are named

---

## Output Format

Return the PRD as a structured document with clearly labeled sections: Summary, Problem Statement, Goals & Non-Goals, User Stories, Functional & Non-Functional Requirements, Success Metrics, and Open Questions & Dependencies. Use headers, numbered lists, and bullet points for scannability.

---

*Exported from Korvai · v1 · 2026-08-09*