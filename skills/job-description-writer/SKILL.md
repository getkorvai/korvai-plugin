---
name: job-description-writer
preamble-tier: 2
version: 1.0.0
description: |
  Turn a role title and requirements into a clear, inclusive, ready-to-post job description.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [role_and_requirements]
triggers:
  - "When a hiring manager or recruiter needs to draft a new job description from scratch or rewrite an existing one."
metadata:
  source: korvai
  korvai_id: ff25a4cc-c3a6-4208-b45b-9356a8046a56
  social_hook: Stop scaring off great candidates with bad job posts — write inclusive JDs in seconds.
  gallery_slug_key: job-description-writer
---

# Job Description Writer

> Generate a polished, bias-aware job description that attracts diverse, qualified candidates based on a role overview and its core requirements.

**Trigger:** When a hiring manager or recruiter needs to draft a new job description from scratch or rewrite an existing one.

**Variables:** `$role_and_requirements`

---

## Steps

### Step 1: Analyze the role input provided below and extract key signals: job title, team context, seniority level, core responsibilities, and must-have vs. nice-to-have qualifications.

Analyze the role input provided below and extract key signals: job title, team context, seniority level, core responsibilities, and must-have vs. nice-to-have qualifications.

$role_and_requirements

**Checklist:**
- [ ] Role title and seniority are identifiable
- [ ] At least 3 core responsibilities are present
- [ ] Required vs. preferred qualifications are distinguishable

**Template:**
```
Role & Requirements:

$role_and_requirements
```

### Step 2: Draft a compelling 3–4 sentence role summary that communicates the team mission, the impact of this role, and who thrives in it — without gendered or exclusionary language.

Draft a compelling 3–4 sentence role summary that communicates the team mission, the impact of this role, and who thrives in it — without gendered or exclusionary language.

**Checklist:**
- [ ] No jargon or gendered language used
- [ ] Impact of the role is clearly stated

### Step 3: Write a bulleted Responsibilities section with 5–8 action-verb-led bullets. Focus on outcomes and day-to-day work, not internal org-chart politics.

Write a bulleted Responsibilities section with 5–8 action-verb-led bullets. Focus on outcomes and day-to-day work, not internal org-chart politics.

**Checklist:**
- [ ] Each bullet starts with an action verb
- [ ] Bullets describe outcomes, not just tasks

### Step 4: Produce two separate lists: 'Required Qualifications' (hard minimums, 4–6 items) and 'Nice to Have' (3–4 items). Flag and remove any requirements that are proxy barriers — e.g., degree requirements where skills suffice, excessive years of experience.

Produce two separate lists: 'Required Qualifications' (hard minimums, 4–6 items) and 'Nice to Have' (3–4 items). Flag and remove any requirements that are proxy barriers — e.g., degree requirements where skills suffice, excessive years of experience.

**Checklist:**
- [ ] Required and preferred are clearly separated
- [ ] No proxy barriers or inflated experience demands remain

### Step 5: Write a 2–3 sentence inclusive closing that invites candidates from underrepresented groups to apply, mentions any flexibility (remote, hybrid, accommodations), and directs them on how to apply.

Write a 2–3 sentence inclusive closing that invites candidates from underrepresented groups to apply, mentions any flexibility (remote, hybrid, accommodations), and directs them on how to apply.

**Checklist:**
- [ ] Inclusivity and flexibility are mentioned
- [ ] A clear call-to-action for applying is included

### Step 6: Review the full draft for inclusive language using these checks: no gendered pronouns or coded words (e.g., 'rockstar', 'ninja'), requirements list is proportionate to role level, and tone is welcoming rather than gatekeeping.

Review the full draft for inclusive language using these checks: no gendered pronouns or coded words (e.g., 'rockstar', 'ninja'), requirements list is proportionate to role level, and tone is welcoming rather than gatekeeping.

**Checklist:**
- [ ] No coded or exclusionary language present
- [ ] Tone is professional and welcoming
- [ ] Requirement count matches role seniority

---

## Output Format

Return the final job description as a structured document with clearly labeled sections: Role Summary, Responsibilities, Required Qualifications, Nice to Have, and How to Apply. Use plain language, bullet points for lists, and a warm but professional tone throughout.

---

*Exported from Korvai · v1 · 2026-08-09*