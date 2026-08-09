---
name: personal-finance-health-check
preamble-tier: 2
version: 1.0.0
description: |
  A repeatable intake-and-diagnosis SOP that gathers the financial context people usually leave out, then grades the resulting advice against life-cycle finance principles. Education, not regulated advice.
license: CC-BY-4.0
compatibility: Designed for Claude Code and compatible agent clients
allowed-tools: Read Write
triggers:
  - "When you want a structured, repeatable financial review from AI instead of a one-off chat — it collects the context you would forget and checks the advice against life-cycle principles."
metadata:
  source: korvai
  korvai_id: fa239fb3-2a64-4bb6-a2ab-6f62532d1ef8
  social_hook: The MIT Sloan study showed the gap between good and bad AI financial advice is mostly what you forget to tell it. This SOP asks for all of it, then grades the answer.
  gallery_slug_key: personal-finance-health-check
---

# Personal Finance Health Check

> Run a structured personal-finance review: collect the full financial picture (including the context people routinely omit), produce spending/saving/investing guidance grounded in life-cycle principles, then self-grade that guidance against a fixed set of diagnostic tests. This is educational analysis, not regulated financial advice.

**Trigger:** When you want a structured, repeatable financial review from AI instead of a one-off chat — it collects the context you would forget and checks the advice against life-cycle principles.

---

## Steps

### Step 1: Gather my complete financial picture. Ask for anything missing before advising — do NOT proceed on a partial picture, because the omitted context (not the model) is what produces generic advice.

Gather my complete financial picture. Ask for anything missing before advising — do NOT proceed on a partial picture, because the omitted context (not the model) is what produces generic advice.

**Checklist:**
- [ ] Age, target retirement age, household (dependents, partner income)
- [ ] Income: annual after-tax, stability, and any expected large changes
- [ ] Liquidity: cash / emergency buffer in months of essential expenses
- [ ] Debt: balances and interest rates, especially anything above ~7%
- [ ] Retirement access: employer match, tax-advantaged accounts available
- [ ] Current savings and how they are allocated (stocks / bonds / cash / other)
- [ ] Goal in my own words, and my honest risk comfort

### Step 2: State the baseline assumptions you will use, and flag every gap. For each missing number, say what you will assume and how sensitive the advice is to it. Use ~2% real return for safe savings and the long-run historical average for diversified stocks; never assume market timing or above-market returns.

State the baseline assumptions you will use, and flag every gap. For each missing number, say what you will assume and how sensitive the advice is to it. Use ~2% real return for safe savings and the long-run historical average for diversified stocks; never assume market timing or above-market returns.

**Checklist:**
- [ ] List each assumption with the biggest risk if it is wrong
- [ ] Name the 2-3 missing inputs that would most change the answer
- [ ] Assume current tax and Social Security rules unless told otherwise

### Step 3: Produce the core guidance: a spending/saving split for working years, an age-appropriate asset allocation with a glide path that reduces equity as I age, an explicit rebalancing rule (calendar + threshold), account priority (match first, then tax-advantaged, then taxable), and a high-interest-debt plan. Describe any product generically and disclose it is one option, not an endorsement.

Produce the core guidance: a spending/saving split for working years, an age-appropriate asset allocation with a glide path that reduces equity as I age, an explicit rebalancing rule (calendar + threshold), account priority (match first, then tax-advantaged, then taxable), and a high-interest-debt plan. Describe any product generically and disclose it is one option, not an endorsement.

**Checklist:**
- [ ] Savings rate + spending target
- [ ] Allocation + age glide path
- [ ] Rebalancing rule: calendar AND threshold trigger
- [ ] Account priority order
- [ ] High-interest debt payoff vs. invest decision

### Step 4: Self-grade the guidance you just gave against the diagnostic tests below (these are the life-cycle checks the research proposes). For each, mark PASS or FIX and, if FIX, correct the guidance before finishing. Do not skip a test to look decisive.

Self-grade the guidance you just gave against the diagnostic tests below (these are the life-cycle checks the research proposes). For each, mark PASS or FIX and, if FIX, correct the guidance before finishing. Do not skip a test to look decisive.

**Checklist:**
- [ ] Consumption smoothing: does the plan avoid wild year-to-year swings, and let me spend savings down in retirement rather than hoard?
- [ ] Shock response: on job loss, does it use my buffer proportionally instead of panic-cutting?
- [ ] Diversification: is risky money mostly in broad funds, with only small single-stock/crypto exposure?
- [ ] Active rebalancing: is there a concrete rule to correct drift, not "stay the course"?
- [ ] Bias check: is every risk/savings assumption tied to my stated numbers, not to inferred traits (gender, apparent literacy, tone)?

### Step 5: Hand off responsibly. Summarize what to do this week, what would change the recommendation, and exactly what to verify with a licensed professional. Reinforce that this is education, not regulated advice.

Hand off responsibly. Summarize what to do this week, what would change the recommendation, and exactly what to verify with a licensed professional. Reinforce that this is education, not regulated advice.

**Checklist:**
- [ ] Top 3 actions for this week
- [ ] The 2-3 inputs that most move the plan
- [ ] What to confirm with a human advisor before acting

---

## Output Format

Return five sections: (1) Intake summary — the picture you collected and what is still missing. (2) Assumptions — each with its biggest risk. (3) The plan — savings rate, allocation + glide path, rebalancing rule, account priority, debt plan. (4) Diagnostic scorecard — the five tests above, each PASS/FIX, with any fixes already applied. (5) Handoff — this week's actions, what would change the advice, and what to verify with a licensed professional. Keep it concrete and grounded only in my stated numbers.

---

*Exported from Korvai · v1 · 2026-08-09*