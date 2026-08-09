---
name: standup-summary
preamble-tier: 2
version: 1.0.0
description: |
  Summarize a team standup meeting into clear blockers, progress highlights, and next steps.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [standup_notes]
triggers:
  - "Invoke after a daily standup meeting when notes or a transcript need to be distilled into a shared summary."
metadata:
  source: korvai
  korvai_id: ccb4258e-564a-4950-9cbd-237b80b6dc7a
  social_hook: Turn messy standup notes into a clean, actionable summary in seconds. 🚀
  gallery_slug_key: standup-summary
---

# Standup Summary

> Transform raw standup notes into a structured summary with blockers, progress, and next steps for easy team reference.

**Trigger:** Invoke after a daily standup meeting when notes or a transcript need to be distilled into a shared summary.

**Variables:** `$standup_notes`

---

## Steps

### Step 1: Analyze the standup notes or transcript provided below:

Analyze the standup notes or transcript provided below:

$standup_notes

**Checklist:**
- [ ] Raw notes or transcript are present
- [ ] Content covers at least one team member's update

**Template:**
```
Analyze the standup notes or transcript provided below:

$standup_notes
```

### Step 2: Identify and list all blockers mentioned. For each blocker, note who owns it and what is preventing progress. If no blockers were mentioned, explicitly state 'No blockers reported.'

Identify and list all blockers mentioned. For each blocker, note who owns it and what is preventing progress. If no blockers were mentioned, explicitly state 'No blockers reported.'

**Checklist:**
- [ ] Every mentioned blocker is captured
- [ ] Owner is attributed to each blocker

### Step 3: Extract progress updates for each team member. Summarize what was completed or meaningfully advanced since the last standup in one to two sentences per person.

Extract progress updates for each team member. Summarize what was completed or meaningfully advanced since the last standup in one to two sentences per person.

**Checklist:**
- [ ] Each speaking team member has a progress entry
- [ ] Summaries are concise and jargon-free

### Step 4: Compile next steps: list the concrete tasks or goals each team member committed to completing before the next standup. Flag any items that depend on resolving a blocker.

Compile next steps: list the concrete tasks or goals each team member committed to completing before the next standup. Flag any items that depend on resolving a blocker.

**Checklist:**
- [ ] Next steps are specific and actionable
- [ ] Blocker-dependent tasks are flagged

### Step 5: Write a one-sentence executive summary of the overall team status (e.g., on track, at risk, blocked) suitable for sharing with a manager or stakeholder who did not attend.

Write a one-sentence executive summary of the overall team status (e.g., on track, at risk, blocked) suitable for sharing with a manager or stakeholder who did not attend.

**Checklist:**
- [ ] Summary reflects the overall tone of the standup
- [ ] Fits in a single sentence

---

## Output Format

Return four labeled sections: 1) Executive Summary — one sentence on overall team status. 2) Blockers — bulleted list with owner names. 3) Progress — bulleted list grouped by team member. 4) Next Steps — bulleted list with owner names and any blocker dependencies noted inline.

---

*Exported from Korvai · v1 · 2026-08-09*