---
name: bug-triage
preamble-tier: 2
version: 1.0.0
description: |
  Transform a raw bug report into a prioritized, reproducible triage summary with severity, steps, and owner recommendations.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [bug_report]
triggers:
  - "When a new bug report is submitted and needs to be assessed, prioritized, and routed before entering a development sprint."
metadata:
  source: korvai
  korvai_id: cc17a4f9-3ae0-453d-b3f5-b34680687f70
  social_hook: Stop drowning in messy bug reports — turn chaos into a clean, actionable triage summary in seconds. 🐛
  gallery_slug_key: bug-triage
---

# Bug Triage

> Analyze a raw bug report and produce a structured triage summary including severity rating, clear reproduction steps, expected vs actual behavior, impact assessment, and recommended ownership.

**Trigger:** When a new bug report is submitted and needs to be assessed, prioritized, and routed before entering a development sprint.

**Variables:** `$bug_report`

---

## Steps

### Step 1: Analyze the raw bug report below and extract all available factual details — affected component, environment, user actions, and any error messages or logs:

Analyze the raw bug report below and extract all available factual details — affected component, environment, user actions, and any error messages or logs:

$bug_report

**Checklist:**
- [ ] Affected component or feature is identified
- [ ] Environment details (OS, browser, version) are noted
- [ ] Any error messages or stack traces are captured

### Step 2: Reconstruct a numbered, step-by-step reproduction sequence from the report. Fill in any implied steps based on typical user flows. Flag any steps that are ambiguous or missing information.

Reconstruct a numbered, step-by-step reproduction sequence from the report. Fill in any implied steps based on typical user flows. Flag any steps that are ambiguous or missing information.

**Checklist:**
- [ ] Steps begin from a clear starting state
- [ ] Ambiguous or missing steps are explicitly flagged

### Step 3: Define the expected behavior and the actual behavior observed, written as two distinct, concise statements. Base these strictly on what the report describes — do not infer intent beyond what is stated.

Define the expected behavior and the actual behavior observed, written as two distinct, concise statements. Base these strictly on what the report describes — do not infer intent beyond what is stated.

**Checklist:**
- [ ] Expected behavior is one clear sentence
- [ ] Actual behavior matches what the report describes

### Step 4: Assign a severity level (Critical / High / Medium / Low) and a priority level (P0–P3). Justify each rating in one sentence based on user impact, data risk, frequency of occurrence, and whether a workaround exists.

Assign a severity level (Critical / High / Medium / Low) and a priority level (P0–P3). Justify each rating in one sentence based on user impact, data risk, frequency of occurrence, and whether a workaround exists.

**Checklist:**
- [ ] Severity and priority are both assigned
- [ ] Justification references at least one impact factor
- [ ] Workaround availability is noted

### Step 5: Recommend an owner team or role (e.g., Frontend, Backend, DevOps, QA) and suggest any immediate mitigation actions that could reduce user impact before a fix is deployed.

Recommend an owner team or role (e.g., Frontend, Backend, DevOps, QA) and suggest any immediate mitigation actions that could reduce user impact before a fix is deployed.

**Checklist:**
- [ ] Owner team or role is specified
- [ ] At least one mitigation action is suggested if applicable

### Step 6: Compile all outputs into a final triage summary. Present it as a clean, scannable document with labeled sections: Summary, Environment, Reproduction Steps, Expected vs Actual, Severity & Priority, Impact, Owner, and Mitigation.

Compile all outputs into a final triage summary. Present it as a clean, scannable document with labeled sections: Summary, Environment, Reproduction Steps, Expected vs Actual, Severity & Priority, Impact, Owner, and Mitigation.

**Checklist:**
- [ ] All eight sections are present
- [ ] Summary is two sentences or fewer
- [ ] Document is ready to paste into a ticket tracker

---

## Output Format

A structured triage document with clearly labeled sections in this order: (1) One-line Summary, (2) Environment, (3) Numbered Reproduction Steps with flagged gaps, (4) Expected Behavior vs Actual Behavior, (5) Severity and Priority with justification, (6) User Impact scope, (7) Recommended Owner, (8) Mitigation Actions. Use plain text suitable for pasting into Jira, Linear, or GitHub Issues.

---

*Exported from Korvai · v1 · 2026-08-09*