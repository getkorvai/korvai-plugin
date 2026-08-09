---
name: customer-interview-synthesis
preamble-tier: 2
version: 1.0.0
description: |
  Transform raw customer interview notes into structured themes, standout quotes, and actionable product decisions.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [interview_notes]
triggers:
  - "After completing one or more customer interviews and collecting raw notes or transcripts that need to be analyzed and shared with a team."
metadata:
  source: korvai
  korvai_id: 6b5a1545-85ba-4043-a0f8-abe5ae9c0e3b
  social_hook: Stop drowning in interview notes — turn raw customer conversations into clear themes and decisions in minutes.
  gallery_slug_key: customer-interview-synthesis
---

# Customer Interview Synthesis

> Synthesize raw customer interview notes into prioritized themes, representative quotes, and concrete product or strategy decisions.

**Trigger:** After completing one or more customer interviews and collecting raw notes or transcripts that need to be analyzed and shared with a team.

**Variables:** `$interview_notes`

---

## Steps

### Step 1: Analyze the raw interview notes below and identify the core topics and recurring pain points mentioned across responses:

Analyze the raw interview notes below and identify the core topics and recurring pain points mentioned across responses:

$interview_notes

**Checklist:**
- [ ] All interviews or respondents are represented
- [ ] No major topic from the notes is overlooked

**Template:**
```
Analyze the raw interview notes below and identify the core topics and recurring pain points mentioned across responses:

$interview_notes
```

### Step 2: Group related observations into 3–6 distinct themes. For each theme, write a one-sentence label and a 2–3 sentence explanation of what customers are expressing and why it matters.

Group related observations into 3–6 distinct themes. For each theme, write a one-sentence label and a 2–3 sentence explanation of what customers are expressing and why it matters.

**Checklist:**
- [ ] Each theme is distinct with no major overlap
- [ ] Theme labels are jargon-free and team-readable

### Step 3: Select 1–2 verbatim or near-verbatim quotes per theme that best illustrate the customer sentiment. Attribute each quote to an anonymous respondent identifier (e.g. Participant A) if names are present.

Select 1–2 verbatim or near-verbatim quotes per theme that best illustrate the customer sentiment. Attribute each quote to an anonymous respondent identifier (e.g. Participant A) if names are present.

**Checklist:**
- [ ] Quotes are specific and vivid, not generic
- [ ] No identifying personal information is exposed

### Step 4: Assess the frequency and intensity of each theme — note how many respondents mentioned it and whether it was a mild frustration or a critical blocker.

Assess the frequency and intensity of each theme — note how many respondents mentioned it and whether it was a mild frustration or a critical blocker.

**Checklist:**
- [ ] Frequency count or estimate is included per theme
- [ ] Severity or emotional weight is noted

### Step 5: Translate each theme into one concrete decision or recommendation — a product change, a hypothesis to test, or a gap to investigate further. Frame each as an actionable next step for a product or strategy team.

Translate each theme into one concrete decision or recommendation — a product change, a hypothesis to test, or a gap to investigate further. Frame each as an actionable next step for a product or strategy team.

**Checklist:**
- [ ] Every theme maps to at least one decision or action
- [ ] Decisions are specific enough to assign or prioritize

### Step 6: Write a 3–5 sentence executive summary that captures the single biggest insight from the interviews, the top 2–3 themes, and the most urgent recommended action.

Write a 3–5 sentence executive summary that captures the single biggest insight from the interviews, the top 2–3 themes, and the most urgent recommended action.

**Checklist:**
- [ ] Summary is understandable without reading the full synthesis
- [ ] Urgency or priority is clearly communicated

---

## Output Format

Structure the response with clearly labeled sections in this order: (1) Executive Summary, (2) Themes — each with a label, explanation, frequency/intensity note, and supporting quotes, (3) Decisions & Recommendations — a numbered list mapping each theme to an action. Use plain language suitable for a cross-functional team audience.

---

*Exported from Korvai · v1 · 2026-08-09*