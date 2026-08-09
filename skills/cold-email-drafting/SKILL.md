---
name: cold-email-drafting
preamble-tier: 2
version: 1.0.0
description: |
  Draft a personalized cold outreach email from a prospect profile and offer in minutes.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [prospect_profile_and_offer]
triggers:
  - "When you need to write a cold email to a new prospect and have their profile details plus your offer ready."
metadata:
  source: korvai
  korvai_id: ae0f036b-379a-46bc-bc00-d333b0262c36
  social_hook: Stop sending generic cold emails. This skill writes hyper-personalized outreach that actually gets replies. 🎯
  gallery_slug_key: cold-email-drafting
---

# Cold Email Drafting

> Produce a concise, personalized cold outreach email that connects the prospect's specific context to a compelling offer and drives a single clear call to action.

**Trigger:** When you need to write a cold email to a new prospect and have their profile details plus your offer ready.

**Variables:** `$prospect_profile_and_offer`

---

## Steps

### Step 1: Analyze the prospect profile and offer below. Extract key details: prospect's role, company, likely pain points, recent signals (funding, hiring, news), and the core value proposition of the offer.

Analyze the prospect profile and offer below. Extract key details: prospect's role, company, likely pain points, recent signals (funding, hiring, news), and the core value proposition of the offer.

$prospect_profile_and_offer

**Checklist:**
- [ ] Prospect role and company are identified
- [ ] At least one specific pain point or signal is noted
- [ ] Core offer value proposition is clear

### Step 2: Write a subject line that feels personal and curiosity-driven. It should reference something specific to the prospect (their company, role, or a recent signal) — not a generic pitch. Aim for under 8 words.

Write a subject line that feels personal and curiosity-driven. It should reference something specific to the prospect (their company, role, or a recent signal) — not a generic pitch. Aim for under 8 words.

**Checklist:**
- [ ] Subject line is under 8 words
- [ ] References something specific to the prospect
- [ ] Avoids spammy words like 'free', 'guaranteed', or excessive punctuation

### Step 3: Draft the opening line (1–2 sentences). Lead with a specific, genuine observation about the prospect or their company — not a compliment. Reference a real signal like a product launch, job posting, or published content to establish relevance.

Draft the opening line (1–2 sentences). Lead with a specific, genuine observation about the prospect or their company — not a compliment. Reference a real signal like a product launch, job posting, or published content to establish relevance.

**Checklist:**
- [ ] Opening references a specific, verifiable detail
- [ ] Does not open with 'I' or a generic compliment
- [ ] Feels human, not templated

### Step 4: Write the value bridge (2–3 sentences). Connect the observed pain point or signal directly to the offer. Be explicit about the outcome the prospect can expect — use a concrete result or metric if possible. Avoid feature-dumping.

Write the value bridge (2–3 sentences). Connect the observed pain point or signal directly to the offer. Be explicit about the outcome the prospect can expect — use a concrete result or metric if possible. Avoid feature-dumping.

**Checklist:**
- [ ] Pain point is explicitly connected to the offer
- [ ] At least one concrete outcome or result is mentioned
- [ ] No more than 3 sentences

### Step 5: Write a low-friction call to action (1 sentence). Ask for a specific, small commitment — a 15-minute call, a yes/no question, or permission to send more info. Avoid vague CTAs like 'let me know your thoughts'.

Write a low-friction call to action (1 sentence). Ask for a specific, small commitment — a 15-minute call, a yes/no question, or permission to send more info. Avoid vague CTAs like 'let me know your thoughts'.

**Checklist:**
- [ ] CTA asks for one specific action
- [ ] Commitment level is low (under 20 minutes or a simple reply)
- [ ] CTA is a single sentence

### Step 6: Assemble the full email and review it. Total length should be 100–150 words. Cut any sentence that doesn't directly serve the prospect. Flag any claims that need verification before sending.

Assemble the full email and review it. Total length should be 100–150 words. Cut any sentence that doesn't directly serve the prospect. Flag any claims that need verification before sending.

**Checklist:**
- [ ] Email is 100–150 words
- [ ] Every sentence serves the prospect, not the sender
- [ ] Any unverified claims are flagged for review

---

## Output Format

Present the output in three labeled sections: (1) Subject Line — the final subject line text; (2) Email Body — the complete ready-to-send email as plain prose; (3) Notes — a brief bullet list of any personalization assumptions made or claims that should be verified before sending.

---

*Exported from Korvai · v1 · 2026-08-09*