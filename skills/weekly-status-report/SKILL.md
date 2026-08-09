---
name: weekly-status-report
preamble-tier: 2
version: 1.0.0
description: |
  Transform raw work logs into a polished, stakeholder-ready weekly status report in minutes.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [work_logs]
triggers:
  - "Invoke at the end of each work week when the user is ready to compile and share progress with stakeholders."
metadata:
  source: korvai
  korvai_id: 8250f6de-0642-4c5c-95a4-da8b1a4bc48f
  social_hook: Turn your messy work notes into a crisp stakeholder report — in one paste. 📋
  gallery_slug_key: weekly-status-report
---

# Weekly Status Report

> Convert raw weekly work logs into a structured, professional status report highlighting accomplishments, blockers, and next steps for stakeholders.

**Trigger:** Invoke at the end of each work week when the user is ready to compile and share progress with stakeholders.

**Variables:** `$work_logs`

---

## Steps

### Step 1: Analyze the work logs provided below and extract all notable activities, completed tasks, in-progress items, blockers, and upcoming priorities:

Analyze the work logs provided below and extract all notable activities, completed tasks, in-progress items, blockers, and upcoming priorities:

$work_logs

**Checklist:**
- [ ] All days of the week are accounted for
- [ ] Blockers and risks are identified
- [ ] Upcoming tasks are noted

**Template:**
```
Paste your raw work logs here:

$work_logs
```

### Step 2: Group extracted items into four categories: Accomplishments (completed this week), In Progress (started but not finished), Blockers & Risks (anything slowing the team down), and Next Week Priorities (planned work).

Group extracted items into four categories: Accomplishments (completed this week), In Progress (started but not finished), Blockers & Risks (anything slowing the team down), and Next Week Priorities (planned work).

**Checklist:**
- [ ] Every extracted item is assigned to exactly one category
- [ ] No category is left empty without a note

### Step 3: Rewrite each item in stakeholder-friendly language: use action verbs, remove jargon, quantify impact where possible (e.g., 'Reduced load time by 40%' instead of 'fixed slow query'), and keep each bullet to one concise sentence.

Rewrite each item in stakeholder-friendly language: use action verbs, remove jargon, quantify impact where possible (e.g., 'Reduced load time by 40%' instead of 'fixed slow query'), and keep each bullet to one concise sentence.

**Checklist:**
- [ ] Jargon and internal shorthand are eliminated
- [ ] At least one metric or outcome is included where data was available

### Step 4: Write a 2–3 sentence executive summary that captures the week's overall theme, the most important achievement, and any critical blocker or risk that requires stakeholder attention.

Write a 2–3 sentence executive summary that captures the week's overall theme, the most important achievement, and any critical blocker or risk that requires stakeholder attention.

**Checklist:**
- [ ] Summary is self-contained and readable without the detail sections
- [ ] Critical risks are surfaced, not buried

### Step 5: Assemble the final report in order: Executive Summary, Accomplishments, In Progress, Blockers & Risks, Next Week Priorities. Add a header with the reporting week date range and the preparer's team or name if inferable from the logs.

Assemble the final report in order: Executive Summary, Accomplishments, In Progress, Blockers & Risks, Next Week Priorities. Add a header with the reporting week date range and the preparer's team or name if inferable from the logs.

**Checklist:**
- [ ] Sections appear in the correct order
- [ ] Date range is present in the header
- [ ] Report reads as a single cohesive document

---

## Output Format

Deliver the report as clearly labeled sections with a bold heading for each (Executive Summary, Accomplishments, In Progress, Blockers & Risks, Next Week Priorities). Use bullet points within each section. Keep the full report under 500 words. Use professional, confident tone suitable for senior stakeholders.

---

*Exported from Korvai · v1 · 2026-08-09*