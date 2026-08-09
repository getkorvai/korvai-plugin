---
name: sales-call-follow-up
preamble-tier: 2
version: 1.0.0
description: |
  Turn a raw sales call transcript into a polished follow-up email and structured CRM notes in minutes.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [transcript]
triggers:
  - "Invoke immediately after a sales call when you have a transcript or detailed notes ready to process."
metadata:
  source: korvai
  korvai_id: 244ed695-074c-4dac-9901-1c2f72181cf5
  social_hook: Stop spending 30 mins on post-call admin. Paste your transcript, get a follow-up email + CRM notes instantly. 🚀
  gallery_slug_key: sales-call-follow-up
---

# Sales Call Follow-up

> Transform a sales call transcript into a ready-to-send follow-up email and complete CRM notes capturing key details, next steps, and deal signals.

**Trigger:** Invoke immediately after a sales call when you have a transcript or detailed notes ready to process.

**Variables:** `$transcript`

---

## Steps

### Step 1: Analyze the sales call transcript below and extract all key information before drafting anything:

Analyze the sales call transcript below and extract all key information before drafting anything:

$transcript

**Checklist:**
- [ ] Transcript is fully pasted and readable
- [ ] Identify prospect name, company, and role

**Template:**
```
Analyze the sales call transcript below and extract all key information before drafting anything:

$transcript
```

### Step 2: Identify and list the following from the transcript: prospect's core pain points, stated goals, objections raised, budget or timeline signals, and any commitments made by either party.

Identify and list the following from the transcript: prospect's core pain points, stated goals, objections raised, budget or timeline signals, and any commitments made by either party.

**Checklist:**
- [ ] At least one pain point identified
- [ ] Objections and commitments both noted

### Step 3: Draft a concise, personalized follow-up email from the salesperson's perspective. Open with a reference to a specific moment from the call, summarize the value proposition tied to their pain points, list agreed next steps as bullet points, and close with a clear CTA.

Draft a concise, personalized follow-up email from the salesperson's perspective. Open with a reference to a specific moment from the call, summarize the value proposition tied to their pain points, list agreed next steps as bullet points, and close with a clear CTA.

**Checklist:**
- [ ] Email references a specific call detail
- [ ] Next steps are explicit and dated if mentioned
- [ ] CTA is singular and actionable

### Step 4: Write structured CRM notes covering: Contact details (name, title, company), Deal stage, Pain points, Objections, Budget/timeline signals, Agreed next steps with owner and due date, and an overall deal health score (Hot / Warm / Cold) with one-line rationale.

Write structured CRM notes covering: Contact details (name, title, company), Deal stage, Pain points, Objections, Budget/timeline signals, Agreed next steps with owner and due date, and an overall deal health score (Hot / Warm / Cold) with one-line rationale.

**Checklist:**
- [ ] All CRM fields are populated
- [ ] Deal health score includes a rationale

### Step 5: Review the follow-up email and CRM notes together for consistency. Ensure the next steps in both documents match exactly, the tone of the email fits the prospect's communication style observed in the call, and no sensitive pricing or internal commentary leaks into the email.

Review the follow-up email and CRM notes together for consistency. Ensure the next steps in both documents match exactly, the tone of the email fits the prospect's communication style observed in the call, and no sensitive pricing or internal commentary leaks into the email.

**Checklist:**
- [ ] Next steps are identical across email and CRM notes
- [ ] No internal-only information in the email draft

---

## Output Format

Return two clearly labeled sections: 1) FOLLOW-UP EMAIL — subject line, greeting, body paragraphs, and sign-off ready to copy-paste. 2) CRM NOTES — a structured list with labeled fields. Use plain text formatting with section headers in ALL CAPS.

---

*Exported from Korvai · v1 · 2026-08-09*