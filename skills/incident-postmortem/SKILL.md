---
name: incident-postmortem
preamble-tier: 2
version: 1.0.0
description: |
  Draft a blameless postmortem from an incident timeline and impact summary in minutes.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [incident_report]
triggers:
  - "Invoke after an incident has been resolved and a timeline with impact notes has been collected."
metadata:
  source: korvai
  korvai_id: a8b111ed-75ce-4b5c-a1a7-7daa8c28410c
  social_hook: Turn your incident chaos into clean, blameless postmortems — automatically. 🔥
  gallery_slug_key: incident-postmortem
---

# Incident Postmortem

> Generate a complete, blameless postmortem document including timeline, root cause analysis, impact assessment, and actionable follow-up items from a raw incident report.

**Trigger:** Invoke after an incident has been resolved and a timeline with impact notes has been collected.

**Variables:** `$incident_report`

---

## Steps

### Step 1: Analyze the incident report below and extract key facts: incident title, start/end times, affected systems, and a structured timeline of events.

Analyze the incident report below and extract key facts: incident title, start/end times, affected systems, and a structured timeline of events.

$incident_report

**Checklist:**
- [ ] Incident start and end timestamps are identified
- [ ] Affected systems or services are listed
- [ ] At least 3 timeline events are extracted

**Template:**
```
Incident Report:

$incident_report
```

### Step 2: Identify the root cause(s) using a blameless lens. Focus on systemic failures, process gaps, or environmental conditions — not individual errors. Distinguish between root causes and contributing factors.

Identify the root cause(s) using a blameless lens. Focus on systemic failures, process gaps, or environmental conditions — not individual errors. Distinguish between root causes and contributing factors.

**Checklist:**
- [ ] Root cause is systemic, not person-specific
- [ ] Contributing factors are separated from root cause

### Step 3: Quantify the impact: describe user-facing symptoms, estimate the number of users or systems affected, duration of degradation, and any data loss or SLA breaches.

Quantify the impact: describe user-facing symptoms, estimate the number of users or systems affected, duration of degradation, and any data loss or SLA breaches.

**Checklist:**
- [ ] Impact duration is stated in minutes or hours
- [ ] Affected user or system scope is estimated
- [ ] SLA breach or data loss is noted if applicable

### Step 4: Draft the Detection and Response section: describe how the incident was detected (alert, user report, etc.), who responded, and evaluate whether detection was timely or could be improved.

Draft the Detection and Response section: describe how the incident was detected (alert, user report, etc.), who responded, and evaluate whether detection was timely or could be improved.

**Checklist:**
- [ ] Detection method is clearly stated
- [ ] Response timeline is summarized
- [ ] Detection gap or improvement opportunity is noted

### Step 5: Generate a prioritized list of action items to prevent recurrence. Each item should include a description, suggested owner role (not a named individual), and a recommended priority (P1/P2/P3).

Generate a prioritized list of action items to prevent recurrence. Each item should include a description, suggested owner role (not a named individual), and a recommended priority (P1/P2/P3).

**Checklist:**
- [ ] Each action item maps to a root cause or contributing factor
- [ ] Owner roles are generic (e.g., 'On-call engineer'), not named people
- [ ] Priority level is assigned to each item

### Step 6: Assemble the full postmortem document in a clean, structured format. Use a professional but accessible tone. Ensure no language assigns personal blame — reframe any blame-implying phrases to systemic observations.

Assemble the full postmortem document in a clean, structured format. Use a professional but accessible tone. Ensure no language assigns personal blame — reframe any blame-implying phrases to systemic observations.

**Checklist:**
- [ ] All sections are present: Summary, Timeline, Root Cause, Impact, Detection & Response, Action Items
- [ ] No blame-assigning language is used
- [ ] Document reads as a complete, shareable artifact

---

## Output Format

Produce a structured postmortem document with clearly labeled sections: (1) Incident Summary, (2) Timeline, (3) Root Cause & Contributing Factors, (4) Impact, (5) Detection & Response, (6) Action Items table with columns for Description, Owner Role, and Priority. Use plain prose under each section. Keep the tone factual, blameless, and concise.

---

*Exported from Korvai · v1 · 2026-08-09*