---
name: code-review-checklist
preamble-tier: 2
version: 1.0.0
description: |
  Review a pull request diff for correctness, security, and maintainability using a structured checklist.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write Bash
arguments: [pr_diff]
triggers:
  - "When a developer submits a pull request and needs a comprehensive review before merging."
metadata:
  source: korvai
  korvai_id: c117edf8-40c0-4245-a22c-6074adaa8b32
  social_hook: Never merge bad code again — run every PR through this AI-powered review checklist 🔍
  gallery_slug_key: code-review-checklist
---

# Code Review Checklist

> Produce a thorough, structured code review covering correctness, security vulnerabilities, and maintainability issues from a pull request diff.

**Trigger:** When a developer submits a pull request and needs a comprehensive review before merging.

**Variables:** `$pr_diff`

---

## Steps

### Step 1: Analyze the pull request diff below and identify the scope of changes — which files, modules, or systems are affected and what the PR is trying to accomplish:

Analyze the pull request diff below and identify the scope of changes — which files, modules, or systems are affected and what the PR is trying to accomplish:

$pr_diff

**Checklist:**
- [ ] Diff is fully read and understood
- [ ] Purpose of the PR is clearly identified

### Step 2: Check for correctness: verify the logic is sound, edge cases are handled, error handling is present, and the code does what it claims. Flag any bugs, off-by-one errors, null dereferences, or incorrect assumptions.

Check for correctness: verify the logic is sound, edge cases are handled, error handling is present, and the code does what it claims. Flag any bugs, off-by-one errors, null dereferences, or incorrect assumptions.

**Checklist:**
- [ ] Logic and control flow verified
- [ ] Edge cases and error paths identified
- [ ] No obvious bugs or incorrect behavior

### Step 3: Audit the diff for security issues: look for injection vulnerabilities (SQL, XSS, command), hardcoded secrets or credentials, insecure deserialization, improper authentication/authorization checks, and unsafe use of external input.

Audit the diff for security issues: look for injection vulnerabilities (SQL, XSS, command), hardcoded secrets or credentials, insecure deserialization, improper authentication/authorization checks, and unsafe use of external input.

**Checklist:**
- [ ] No hardcoded secrets or tokens
- [ ] All external inputs are validated or sanitized
- [ ] Auth and permission checks are correct

### Step 4: Evaluate maintainability: assess code readability, naming clarity, function/class size, duplication, test coverage, and whether the changes follow the existing patterns and conventions of the codebase.

Evaluate maintainability: assess code readability, naming clarity, function/class size, duplication, test coverage, and whether the changes follow the existing patterns and conventions of the codebase.

**Checklist:**
- [ ] Code is readable and well-named
- [ ] No unnecessary duplication introduced
- [ ] Tests are present and meaningful

### Step 5: Compile all findings into a structured review report. Categorize each issue as Blocker, Major, or Minor. Include a short explanation and a suggested fix or improvement for each item. End with an overall recommendation: Approve, Request Changes, or Needs Discussion.

Compile all findings into a structured review report. Categorize each issue as Blocker, Major, or Minor. Include a short explanation and a suggested fix or improvement for each item. End with an overall recommendation: Approve, Request Changes, or Needs Discussion.

**Checklist:**
- [ ] All issues are categorized by severity
- [ ] Each issue includes a suggested fix
- [ ] Overall recommendation is clearly stated

---

## Output Format

Return a structured report with four sections: 1) PR Summary (1–3 sentences on scope and intent), 2) Correctness Issues, 3) Security Issues, 4) Maintainability Issues. Each issue entry should include: severity label (Blocker / Major / Minor), file and line reference if applicable, description of the problem, and a suggested fix. Close with a final recommendation line: Approve / Request Changes / Needs Discussion, with a one-sentence rationale.

---

*Exported from Korvai · v1 · 2026-08-09*