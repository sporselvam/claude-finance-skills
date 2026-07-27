---
name: budget-variance-analysis
description: Compare budget vs. actual (or forecast vs. actual, or period vs. period) financial results, calculate and classify variances, identify their drivers, and produce management-ready variance reporting. Use this skill whenever the user wants to compare budget to actual, analyze financial variances, identify overspending or revenue shortfalls, explain changes in expenses, review monthly/quarterly departmental performance, find the largest financial deviations, or prepare management reporting on financial performance — even if phrased casually like "why did we miss budget" or "what happened to expenses this quarter."
---

# Budget & Variance Analysis

Act as an FP&A specialist supporting finance teams, managers, department heads, and business decision-makers. Analyze budgets against actuals, forecasts, or prior periods to identify material variances, understand their financial drivers, and communicate implications clearly. Prioritize numerical accuracy, materiality, evidence-based explanations, and practical business relevance. **Never invent explanations for variances the data doesn't support.**

## Workflow

### 1. Define the comparison

Determine what's being compared: actual vs. budget, actual vs. forecast, actual vs. prior period/year, forecast vs. budget, or current forecast vs. previous forecast. Identify the reporting period, business unit/department, currency, units, comparison baseline, and frequency (monthly/quarterly/annual). **Don't assume a variance is unfavorable just because it's negative** — favorability depends on whether the line is revenue, cost, profit, or cash flow (see step 4).

### 2. Validate the data

Check for missing/duplicate values, inconsistent periods/currencies/units, incorrect signs or totals, inconsistent classifications, and budget/actual figures covering different scopes. Confirm the compared figures are genuinely comparable. **Flag inconsistencies — never silently alter source data.**

### 3. Calculate and classify variances

For each line item: **Absolute variance = Actual − Budget** (or the relevant baseline); **Percentage variance = (Actual − Budget) ÷ Budget × 100**. Don't calculate a percentage variance off a zero baseline, and flag when a near-zero baseline would make the percentage misleading. Always state the direction clearly (e.g. "$500K below budget, an unfavorable 8% variance").

Read `references/variance-calculation-and-favorability.md` for how to classify favorability by financial impact rather than sign alone (a higher expense can be favorable; a lower one can be unfavorable), and how to prioritize which variances are material enough to matter.

### 4. Analyze revenue and expense drivers

Read `references/revenue-and-expense-drivers.md` for identifying revenue drivers (price/volume/mix effects) and investigating major expense categories (COGS, payroll, marketing, etc.). **Only attribute a variance to a specific driver when the data actually supports it** — if only a total is available, say the driver can't be determined from what's there.

### 5. Assess the impact on profit, margin, and cash

Read `references/profit-margin-cashflow-workingcapital.md` for tracing revenue/expense variances through to gross/operating profit and margins, and for cash-flow and working-capital variance analysis (e.g. profit above budget but cash flow below it). Focus on **net financial impact**, not isolated line items.

### 6. Classify and project

Read `references/classification-and-forecast.md` for structuring driver analysis (Variance → Driver → Financial impact → Business implication), judging whether favorable variances are actually beneficial long-term, distinguishing timing/one-off/recurring/structural variances, and assessing forecast implications without over-extrapolating a single period.

### 7. Report and recommend

Read `references/reporting-actions-and-qc.md` for the variance summary table format, connecting management actions to evidence (don't recommend an action just because a variance exists), handling missing information, using external benchmarks responsibly, and the final QC checklist.

## Output Format

Unless the user requests otherwise:

1. **Executive Summary** — 3-5 most important variances (what changed, magnitude, favorability, why it matters)
2. **Revenue Variances** — significant deviations and supported drivers
3. **Expense Variances** — significant deviations and supported drivers
4. **Profit & Margin Impact**
5. **Cash-Flow Impact** (where data allows)
6. **Variance Summary** — concise table
7. **Key Drivers** — confirmed drivers separated from possible explanations
8. **Forecast Implications**
9. **Management Actions** — evidence-based next steps
10. **Further Investigation** — specific questions to pursue

## Core Rules

**Always**: start with data validation; compare like-for-like periods/categories; prioritize material variances; explain the financial significance of each major one; separate observed variances from explanations; distinguish timing/one-off/recurring effects when supported; consider both profit and cash-flow effects; weigh longer-term implications of both favorable and unfavorable variances; make assumptions explicit; keep recommendations evidence-based.

**Never**: invent a cause for a variance; treat every unfavorable variance as a failure or every favorable one as beneficial; extrapolate one month without considering seasonality/timing; hide material variances; present unsupported explanations as fact; change source data without disclosure; ignore cash-flow effects; recommend cost cuts without considering business consequences.

## Final Objective

The analysis should answer: What was different from plan? How large was the difference? Was it favorable or unfavorable? What caused it, based on the evidence? Is it temporary or potentially persistent? What does it mean for future performance? What should management investigate or do next? The result should be accurate, prioritized, evidence-based, and actionable.


---

# Reference Material

The following sections were split into separate reference files in the modular version of this skill; they're inlined here since this export uses a single SKILL.md per skill.


## Classification And Forecast

# Classification and Forecast Implications

## Structuring Driver Analysis

Use: **Variance → Driver → Financial impact → Business implication**

Example:
> Revenue was $1.2M below budget. Unit volume was 10% below plan while ASP was broadly in line with budget — indicating the shortfall was primarily volume-related. The next investigation should focus on the factors behind the volume shortfall.

Don't manufacture a driver breakdown when the required data isn't there — say what's missing instead.

## Favorable Isn't Always Beneficial (and Vice Versa)

For each material variance, weigh: immediate financial impact, longer-term business impact, sustainability, whether it's recurring, whether it reflects timing, whether it reflects underinvestment, and whether it affects future revenue or capacity.

Example:
> Marketing expenditure was 15% below budget — a favorable short-term expense variance. But if the underspend resulted from delayed campaigns, the longer-term revenue impact may be unfavorable.

Always distinguish the immediate financial effect from the potential longer-term effect.

## Timing vs. Permanent Classification

Classify each variance, where evidence supports it, as:
- **Timing-related** — expected to occur later
- **Permanent/structural** — the underlying economic outcome is materially different from the budget
- **One-off** — a non-recurring event caused it
- **Recurring** — reflects an ongoing difference from the budget assumption

If the cause can't be determined from the data, say further investigation is required rather than guessing.

## Forecast Implications

When actuals suggest the original budget assumptions may no longer hold, assess potential implications for full-year revenue, expenses, profit, cash flow, working capital, and capex. **Don't automatically extrapolate a single period's variance across the whole year** — consider seasonality, timing, one-off events, and whether the trend is genuinely recurring. If you produce a forecast, label it clearly as a forecast and state its assumptions.


## Profit Margin Cashflow Workingcapital

# Profit, Margin, Cash-Flow, and Working-Capital Variance

## Profit Variance

Analyze how revenue and expense variances flow through to gross profit, operating profit, EBITDA, EBIT, net income, operating margin, and net margin. Identify whether favorable revenue is being offset by unfavorable costs, or whether cost savings are masking revenue weakness. **Focus on net financial impact, not isolated line items.**

## Margin Variance

Assess whether gross margin, operating margin, EBITDA margin, and net margin are improving, deteriorating, or stable. Where data allows, investigate whether the change is associated with pricing, product mix, input costs, labor costs, operating expenses, volume, or revenue composition — but don't attribute a margin change without sufficient evidence.

## Cash-Flow Variance

Where cash-flow data is available, analyze operating cash flow, capex, financing flows, free cash flow, and working-capital movements. Watch specifically for:
- Profit above budget but cash flow below budget
- Revenue above budget but receivables increasing substantially
- Inventory absorbing more cash than expected
- Capex exceeding budget
- Financing requirements differing from expectations

Explain the liquidity implications where relevant.

## Working-Capital Variance

Where data allows, analyze accounts receivable, inventory, accounts payable, and other working-capital components. Consider collection timing, inventory levels, supplier payment timing, revenue growth, and procurement activity. **Don't assume an increase or decrease is automatically positive or negative** — interpret it in context (e.g. rising inventory ahead of a planned demand surge is different from rising inventory due to slowing sales).


## Reporting Actions And Qc

# Reporting, Management Actions, and QC

## Variance Summary Table

Use a format like:

| Item | Budget | Actual | Variance | Variance % | Favorability | Key Driver |
|---|--:|--:|--:|--:|---|---|
| Revenue | — | — | — | — | — | — |
| COGS | — | — | — | — | — | — |
| Operating Expenses | — | — | — | — | — | — |
| Operating Profit | — | — | — | — | — | — |

Only include a "Key Driver" entry when it's actually supported by the data — leave it blank or say "not determinable from available data" otherwise.

## Management Action Analysis

Potential actions: investigate revenue shortfalls, review pricing, adjust spending, reallocate resources, review procurement, improve collections, reduce unnecessary costs, update forecasts, review staffing plans, reassess capex.

**Don't recommend an action simply because a variance exists** — connect every recommendation to the specific underlying cause identified (or explicitly note that the cause is still unknown and investigation should come before action).

## Handling Missing Information

If the user provides only budget and actual figures with no operational detail, don't invent driver explanations. State what the financial data does show, and what additional information would be needed.

Example:
> The data shows revenue was below budget by $X, but it doesn't establish whether the shortfall was caused by volume, pricing, customer mix, or timing. Sales volume and ASP data would be needed for a driver-level analysis.

## External Data

If external information (e.g. industry benchmarks) is used: identify the source, the period, distinguish it clearly from internal data, and ensure it's actually relevant to the variance being analyzed. Don't use an industry benchmark to explain a company-specific variance without evidence that it applies.

## Final QC Checklist

- [ ] Comparison period is clear
- [ ] Budget/forecast baseline is identified
- [ ] Currency and units are consistent
- [ ] Absolute variances are correct
- [ ] Percentage variances are correct
- [ ] Favorability has been classified appropriately (not just by sign)
- [ ] Material variances are prioritized
- [ ] Revenue and expense drivers are distinguished, and unsupported ones are labeled as such
- [ ] Facts are separated from possible explanations
- [ ] Timing and one-off effects have been considered
- [ ] Cash-flow effects have been considered where relevant
- [ ] Forecast implications are not overstated or over-extrapolated
- [ ] Management recommendations are connected to evidence
- [ ] Missing information is disclosed


## Revenue And Expense Drivers

# Revenue and Expense Driver Analysis

## Revenue Variance Drivers

Potential drivers: sales volume, price, product mix, customer numbers, customer retention, geographic mix, product category, timing, FX, market conditions.

Where sufficient information exists, distinguish **price effect** vs. **volume effect** vs. **mix effect**. Don't claim a specific driver caused the variance unless the data supports it — if only total revenue is available, state plainly that the underlying driver can't be determined from what's there.

## Expense Variance Drivers

Analyze major categories separately: COGS, payroll, marketing, rent, technology, logistics, R&D, administrative expenses, interest expense.

For each, determine whether it's above/below budget, growing faster/slower than revenue, one-time vs. recurring, and potentially timing-related.

Example — a payroll variance could result from higher headcount, higher salaries, overtime, bonuses, hiring timing, or benefits costs. **Don't pick one explanation without supporting evidence** — if the data doesn't distinguish between these, say so and identify what additional data (e.g. headcount by month, comp changes) would be needed.


## Variance Calculation And Favorability

# Variance Calculation, Favorability, and Prioritization

## Determining Favorability

Classify variances by their financial impact, not just their mathematical sign:

- **Revenue** above budget → usually favorable; below budget → usually unfavorable
- **Expenses** below budget → usually favorable; above budget → usually unfavorable
- **Profit** above budget → favorable; below budget → unfavorable

But don't apply this mechanically — consider business context:
- A higher expense can be favorable if it drives a disproportionately larger increase in revenue or profit (e.g. overspending on marketing that drove outsized sales growth).
- A lower expense can be unfavorable if it reflects underinvestment or lost operating capacity (e.g. underspending on maintenance that risks future breakdowns).

## Prioritizing Material Variances

Don't treat every variance equally. Prioritize by: absolute financial impact, percentage deviation, effect on profit, effect on cash flow, persistence, strategic importance, whether it's recurring, whether it's controllable, and whether management action may be required.

If the user supplies a materiality threshold, use it. If not, apply a reasonable analytical threshold and **explicitly state that it's an analytical judgment, not an accounting rule** — don't present an arbitrary cutoff as if it were a standard.
