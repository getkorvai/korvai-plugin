---
name: blog-post-outline
preamble-tier: 2
version: 1.0.0
description: |
  Generate a structured blog post outline from a topic and target audience in seconds.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [blog_request]
triggers:
  - "When a user needs to plan a blog post before writing and has a topic and audience in mind."
metadata:
  source: korvai
  korvai_id: 8776577d-b76f-44ce-9dae-b5d03196b516
  social_hook: Stop staring at a blank page — get a full blog outline in one shot. 🚀
  gallery_slug_key: blog-post-outline
---

# Blog Post Outline

> Produce a clear, structured blog post outline with sections, key points, and a logical narrative flow tailored to a specific topic and audience.

**Trigger:** When a user needs to plan a blog post before writing and has a topic and audience in mind.

**Variables:** `$blog_request`

---

## Steps

### Step 1: Analyze the blog request below and identify the core topic, the target audience, and the primary goal of the post (inform, persuade, entertain, convert):

Analyze the blog request below and identify the core topic, the target audience, and the primary goal of the post (inform, persuade, entertain, convert):

$blog_request

**Checklist:**
- [ ] Core topic is clearly identified
- [ ] Target audience is defined
- [ ] Post goal is determined

### Step 2: Determine the best content angle and narrative hook. Choose an angle that differentiates the post (e.g., contrarian take, step-by-step guide, case study, listicle) based on the audience's needs and the topic's competitive landscape.

Determine the best content angle and narrative hook. Choose an angle that differentiates the post (e.g., contrarian take, step-by-step guide, case study, listicle) based on the audience's needs and the topic's competitive landscape.

**Checklist:**
- [ ] Angle is specific and differentiated
- [ ] Hook will resonate with the target audience

### Step 3: Draft a compelling working title and a one-sentence meta description that captures the post's value proposition for the target audience.

Draft a compelling working title and a one-sentence meta description that captures the post's value proposition for the target audience.

**Checklist:**
- [ ] Title includes a clear benefit or curiosity gap
- [ ] Meta description is under 160 characters

### Step 4: Build the full section-by-section outline. Include an Introduction, 3–6 body sections each with a heading and 2–4 bullet-point sub-points, and a Conclusion with a clear call-to-action.

Build the full section-by-section outline. Include an Introduction, 3–6 body sections each with a heading and 2–4 bullet-point sub-points, and a Conclusion with a clear call-to-action.

**Checklist:**
- [ ] Each section has a descriptive heading
- [ ] Sub-points are specific, not generic
- [ ] Conclusion includes a CTA

### Step 5: Add a brief content notes section suggesting: one internal linking opportunity, one external source type to cite, and one content upgrade idea (e.g., checklist, template, video) that would add value for the audience.

Add a brief content notes section suggesting: one internal linking opportunity, one external source type to cite, and one content upgrade idea (e.g., checklist, template, video) that would add value for the audience.

**Checklist:**
- [ ] Internal link suggestion is relevant
- [ ] Content upgrade idea matches audience needs

---

## Output Format

Present the output in clearly labeled sections: (1) Post Goal & Angle, (2) Working Title & Meta Description, (3) Full Outline with nested headings and bullet-point sub-points, and (4) Content Notes. Use markdown headers and bullets for easy scanning.

---

*Exported from Korvai · v1 · 2026-08-09*