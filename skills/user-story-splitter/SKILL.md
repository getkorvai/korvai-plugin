---
name: user-story-splitter
preamble-tier: 2
version: 1.0.0
description: |
  Break a large user story into small, independently shippable stories with clear acceptance criteria.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [user_story]
triggers:
  - "When a user story is too large to complete in a single sprint or has multiple distinct behaviors bundled together."
metadata:
  source: korvai
  korvai_id: e5bb6aa9-1097-4c29-93b6-0693376be88c
  social_hook: Stop shipping monoliths. Split any bloated user story into lean, deployable slices in seconds. 🔪
  gallery_slug_key: user-story-splitter
---

# User Story Splitter

> Transform a single large user story into a set of small, independently shippable stories, each with a clear title, narrative, and acceptance criteria.

**Trigger:** When a user story is too large to complete in a single sprint or has multiple distinct behaviors bundled together.

**Variables:** `$user_story`

---

## Steps

### Step 1: Analyze the user story below and identify all the distinct behaviors, edge cases, and implicit sub-features bundled inside it:

Analyze the user story below and identify all the distinct behaviors, edge cases, and implicit sub-features bundled inside it:

$user_story

**Checklist:**
- [ ] Story contains multiple acceptance criteria or scenarios
- [ ] Story touches more than one user action or system boundary

### Step 2: Identify the single thinnest vertical slice — the smallest piece that delivers real user value end-to-end. Label it as the 'Walking Skeleton' story that all other slices can build on.

Identify the single thinnest vertical slice — the smallest piece that delivers real user value end-to-end. Label it as the 'Walking Skeleton' story that all other slices can build on.

**Checklist:**
- [ ] Slice touches UI, logic, and data if applicable
- [ ] Slice is deployable and testable on its own

### Step 3: Generate the remaining split stories using recognized splitting patterns: by workflow step, by data variation, by user role, by happy/error path, or by CRUD operation. Aim for 3–7 total stories from the original.

Generate the remaining split stories using recognized splitting patterns: by workflow step, by data variation, by user role, by happy/error path, or by CRUD operation. Aim for 3–7 total stories from the original.

**Checklist:**
- [ ] Each story is independent and not blocked by another split story
- [ ] No story duplicates the scope of another
- [ ] Each story fits comfortably within a single sprint

### Step 4: Write each split story in standard 'As a [role], I want [action], so that [benefit]' format. Include 2–4 acceptance criteria per story written as Given/When/Then scenarios.

Write each split story in standard 'As a [role], I want [action], so that [benefit]' format. Include 2–4 acceptance criteria per story written as Given/When/Then scenarios.

**Checklist:**
- [ ] Every story has a role, action, and benefit
- [ ] Every story has at least one Given/When/Then criterion

### Step 5: Flag any stories that carry significant unknowns or technical risk and recommend them as spikes. Note which stories are optional enhancements that could be deferred to the backlog.

Flag any stories that carry significant unknowns or technical risk and recommend them as spikes. Note which stories are optional enhancements that could be deferred to the backlog.

**Checklist:**
- [ ] Spikes are clearly labeled and time-boxed
- [ ] Deferred stories are marked as backlog candidates

### Step 6: Produce a final summary table listing each story's title, the splitting pattern used, its relative size (S/M/L), and its recommended priority (Now / Next / Later).

Produce a final summary table listing each story's title, the splitting pattern used, its relative size (S/M/L), and its recommended priority (Now / Next / Later).

**Checklist:**
- [ ] All split stories are represented in the table
- [ ] At least one story is marked Now/highest priority

---

## Output Format

Present the Walking Skeleton story first, followed by numbered split stories in 'As a / I want / So that' format with Given/When/Then acceptance criteria. End with a markdown summary table: Story Title | Split Pattern | Size | Priority. Use clear headings for each section.

---

*Exported from Korvai · v1 · 2026-08-09*