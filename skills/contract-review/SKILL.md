---
name: contract-review
preamble-tier: 2
version: 1.0.0
description: |
  Review a contract for risky clauses, missing obligations, and renewal traps to surface legal and business risks fast.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [contract_text]
triggers:
  - "When a contract is received and needs review before signing or negotiation."
metadata:
  source: korvai
  korvai_id: b6fa19e9-035a-4bf5-852d-234df984eb3e
  social_hook: Stop signing blind. Let AI flag every risky clause, silent obligation, and auto-renewal trap in your contract. 🔍
  gallery_slug_key: contract-review
---

# Contract Review

> Analyze a contract to identify risky clauses, missing obligations, and renewal traps, and deliver a structured risk report with recommended actions.

**Trigger:** When a contract is received and needs review before signing or negotiation.

**Variables:** `$contract_text`

---

## Steps

### Step 1: Analyze the full contract text below and identify all parties, the contract type, effective dates, and governing law before proceeding:

Analyze the full contract text below and identify all parties, the contract type, effective dates, and governing law before proceeding:

$contract_text

**Checklist:**
- [ ] All parties clearly identified
- [ ] Contract type and purpose understood
- [ ] Governing law and jurisdiction noted

### Step 2: Scan for risky clauses including indemnification, limitation of liability, exclusivity, non-compete, and IP assignment provisions. Note which party bears disproportionate risk in each.

Scan for risky clauses including indemnification, limitation of liability, exclusivity, non-compete, and IP assignment provisions. Note which party bears disproportionate risk in each.

**Checklist:**
- [ ] Indemnification scope assessed
- [ ] Liability caps (or absence) flagged
- [ ] IP and exclusivity terms reviewed

### Step 3: Identify missing or vague obligations: deliverables without deadlines, payment terms without amounts, SLAs without penalties, or dispute resolution procedures that are absent or unclear.

Identify missing or vague obligations: deliverables without deadlines, payment terms without amounts, SLAs without penalties, or dispute resolution procedures that are absent or unclear.

**Checklist:**
- [ ] All obligations have clear owners and deadlines
- [ ] Payment terms are specific and complete
- [ ] Dispute resolution process is defined

### Step 4: Flag all renewal, termination, and notice clauses. Highlight auto-renewal traps, short notice windows (under 30 days), evergreen clauses, and any termination-for-convenience restrictions.

Flag all renewal, termination, and notice clauses. Highlight auto-renewal traps, short notice windows (under 30 days), evergreen clauses, and any termination-for-convenience restrictions.

**Checklist:**
- [ ] Auto-renewal terms surfaced with exact notice deadlines
- [ ] Termination-for-convenience rights confirmed
- [ ] Notice periods flagged as adequate or risky

### Step 5: Produce a structured risk report: list each finding with a severity rating (High / Medium / Low), the relevant clause or section reference, a plain-language explanation of the risk, and a specific recommended action or redline suggestion.

Produce a structured risk report: list each finding with a severity rating (High / Medium / Low), the relevant clause or section reference, a plain-language explanation of the risk, and a specific recommended action or redline suggestion.

**Checklist:**
- [ ] Every finding has a severity rating
- [ ] Clause location is cited for each issue
- [ ] Each risk includes a concrete recommended action

### Step 6: Write a concise executive summary (5–8 sentences) covering overall contract risk level, the top 3 issues requiring immediate attention, and a clear go / negotiate / reject recommendation.

Write a concise executive summary (5–8 sentences) covering overall contract risk level, the top 3 issues requiring immediate attention, and a clear go / negotiate / reject recommendation.

**Checklist:**
- [ ] Overall risk level stated
- [ ] Top 3 issues called out explicitly
- [ ] Clear recommendation provided

---

## Output Format

Start with an Executive Summary section, followed by a Risk Report table with columns: Severity, Section Reference, Risk Description, and Recommended Action. End with a numbered list of Priority Negotiation Points. Use plain language throughout — no unexplained legal jargon.

---

*Exported from Korvai · v1 · 2026-08-09*