---
name: competitive-teardown
preamble-tier: 2
version: 1.0.0
description: |
  Analyze a competitor product and produce a structured teardown covering positioning, strengths, weaknesses, and strategic gaps.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [competitor_intel]
triggers:
  - "When preparing for a product launch, sales pitch, strategy review, or whenever a competitor releases a new product or update."
metadata:
  source: korvai
  korvai_id: 88bc955e-cd31-460c-b5a1-6a7845a89a33
  social_hook: Know your enemy. This skill tears apart any competitor product and hands you a strategic edge in minutes.
  gallery_slug_key: competitive-teardown
---

# Competitive Teardown

> Produce a comprehensive competitive teardown that reveals a rival product's positioning, strengths, weaknesses, and exploitable gaps to inform your strategy.

**Trigger:** When preparing for a product launch, sales pitch, strategy review, or whenever a competitor releases a new product or update.

**Variables:** `$competitor_intel`

---

## Steps

### Step 1: Ingest the competitor intelligence below and identify the product, its target market, and its core value proposition:

Ingest the competitor intelligence below and identify the product, its target market, and its core value proposition:

$competitor_intel

**Checklist:**
- [ ] Product name and category are clearly identified
- [ ] Target audience is defined
- [ ] Primary value proposition is extracted

### Step 2: Analyze the product's positioning: what category does it own, what narrative does it push, and how does it differentiate itself in messaging and branding?

Analyze the product's positioning: what category does it own, what narrative does it push, and how does it differentiate itself in messaging and branding?

**Checklist:**
- [ ] Category and narrative are named
- [ ] Key differentiators in messaging are listed

### Step 3: Identify the product's top 3–5 strengths — features, UX, pricing, distribution, brand equity, or network effects — with a one-line rationale for each.

Identify the product's top 3–5 strengths — features, UX, pricing, distribution, brand equity, or network effects — with a one-line rationale for each.

**Checklist:**
- [ ] Each strength has a concrete rationale
- [ ] At least one non-obvious strength is included

### Step 4: Identify the product's top 3–5 weaknesses or vulnerabilities — gaps in features, poor UX, pricing friction, support issues, or negative sentiment — with evidence where available.

Identify the product's top 3–5 weaknesses or vulnerabilities — gaps in features, poor UX, pricing friction, support issues, or negative sentiment — with evidence where available.

**Checklist:**
- [ ] Each weakness is grounded in observable evidence
- [ ] Customer pain points are referenced if available

### Step 5: Map the strategic gaps and opportunities: where is this competitor underserving users, ignoring segments, or leaving flanks open? Highlight the top 2–3 actionable openings.

Map the strategic gaps and opportunities: where is this competitor underserving users, ignoring segments, or leaving flanks open? Highlight the top 2–3 actionable openings.

**Checklist:**
- [ ] Each gap is tied to a concrete opportunity
- [ ] Opportunities are ranked by potential impact

### Step 6: Write a one-paragraph executive summary and a 'How to Beat Them' recommendation block with 3 specific tactical moves.

Write a one-paragraph executive summary and a 'How to Beat Them' recommendation block with 3 specific tactical moves.

**Checklist:**
- [ ] Executive summary is under 100 words
- [ ] Each tactical move is specific and actionable

---

## Output Format

Structure the response as clearly labeled sections: 1) Product Overview, 2) Positioning Analysis, 3) Strengths (bulleted), 4) Weaknesses (bulleted), 5) Strategic Gaps & Opportunities (ranked), 6) Executive Summary + How to Beat Them. Use concise, direct language throughout. No fluff.

---

*Exported from Korvai · v1 · 2026-08-09*