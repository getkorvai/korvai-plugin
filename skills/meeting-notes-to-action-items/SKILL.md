---
name: meeting-notes-to-action-items
preamble-tier: 2
version: 1.0.0
description: |
  Convert messy meeting notes into a clean list of owners, action items, and deadlines.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [meeting_notes]
triggers:
  - "Invoke after any meeting when raw notes need to be converted into assigned, trackable action items."
metadata:
  source: korvai
  korvai_id: a779758c-747e-47b6-8df6-abebdc7899db
  social_hook: Stop losing action items in messy meeting notes — this skill extracts every task, owner, and deadline instantly.
  gallery_slug_key: meeting-notes-to-action-items
---

# Meeting Notes to Action Items

> Transform raw meeting notes into a structured action item list with clear owners, tasks, and deadlines ready to share with the team.

**Trigger:** Invoke after any meeting when raw notes need to be converted into assigned, trackable action items.

**Variables:** `$meeting_notes`

---

## Steps

### Step 1: Analyze the meeting notes below and identify every commitment, task, or follow-up mentioned:

Analyze the meeting notes below and identify every commitment, task, or follow-up mentioned:

$meeting_notes

**Checklist:**
- [ ] All notes have been read in full
- [ ] No implicit commitments overlooked

### Step 2: Extract each action item as a discrete, verb-led task. Rewrite vague language into clear, specific actions (e.g. 'discuss pricing' → 'Send revised pricing proposal to client'). Flag any tasks that are ambiguous or need clarification.

Extract each action item as a discrete, verb-led task. Rewrite vague language into clear, specific actions (e.g. 'discuss pricing' → 'Send revised pricing proposal to client'). Flag any tasks that are ambiguous or need clarification.

**Checklist:**
- [ ] Each task starts with an action verb
- [ ] Vague items have been sharpened or flagged

### Step 3: Assign an owner to each action item based on who was mentioned or implied in the notes. If no owner is identifiable, mark it as 'Unassigned' and flag it for the meeting organizer to resolve.

Assign an owner to each action item based on who was mentioned or implied in the notes. If no owner is identifiable, mark it as 'Unassigned' and flag it for the meeting organizer to resolve.

**Checklist:**
- [ ] Every action item has an owner or is explicitly flagged Unassigned
- [ ] Owner names match those mentioned in the notes

### Step 4: Assign a deadline to each action item using dates mentioned in the notes. If no date was given, infer a reasonable deadline based on urgency cues (e.g. 'ASAP', 'before next meeting') or mark as 'No deadline specified'.

Assign a deadline to each action item using dates mentioned in the notes. If no date was given, infer a reasonable deadline based on urgency cues (e.g. 'ASAP', 'before next meeting') or mark as 'No deadline specified'.

**Checklist:**
- [ ] Explicit dates are used where stated
- [ ] Inferred deadlines are labeled as estimated

### Step 5: Group action items by owner so each person can see their full list at a glance. Sort each owner's items by deadline, earliest first.

Group action items by owner so each person can see their full list at a glance. Sort each owner's items by deadline, earliest first.

**Checklist:**
- [ ] Items are grouped by owner
- [ ] Items within each group are sorted by deadline

### Step 6: Produce a brief meeting summary (2–3 sentences) capturing the main decisions made, then present the full action item table below it. End with a flagged section listing any unassigned tasks or items needing clarification.

Produce a brief meeting summary (2–3 sentences) capturing the main decisions made, then present the full action item table below it. End with a flagged section listing any unassigned tasks or items needing clarification.

**Checklist:**
- [ ] Summary covers key decisions, not just tasks
- [ ] Flags section is present if any items are unresolved

---

## Output Format

Start with a 2–3 sentence meeting summary. Follow with a table grouped by owner, columns: Owner | Action Item | Deadline | Status (e.g. Confirmed / Inferred / Flagged). End with a separate 'Needs Clarification' section listing unassigned or ambiguous items.

---

*Exported from Korvai · v1 · 2026-08-09*