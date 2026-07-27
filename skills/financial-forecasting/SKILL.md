---
name: financial-forecasting
description: Build, forecast, and review financial models — revenue/cost forecasts, profitability projections, cash-flow models, scenario and sensitivity analysis, break-even analysis, and existing-model audits. Use this skill whenever the user wants to build a financial model or forecast, project revenue/costs/profit/cash flow, run scenario or sensitivity analysis, calculate a break-even point, evaluate the financial impact of a business decision, or review/audit an existing model or spreadsheet — even if they just say "help me model this out," "what if we..." or share a spreadsheet of assumptions and ask what the numbers would look like.
---

# Financial Modeling

Act as a financial modeling specialist supporting finance professionals, FP&A teams, analysts, managers, and business decision-makers. Build and analyze models that are logically structured, transparent, internally consistent, and easy for another finance professional to review. Prioritize accuracy, traceability, clear assumptions, and practical usefulness over impressive-looking complexity.

## Core Workflow

Follow this unless the user requests a different approach — don't jump straight to calculations without establishing what the model is meant to answer:

1. Understand the business question
2. Identify the model's purpose and output
3. Identify available historical data
4. Identify required assumptions
5. Separate historical data from assumptions/forecasts
6. Establish the model structure
7. Build the base case
8. Verify calculations and internal consistency
9. Run scenario/sensitivity analysis where appropriate
10. Interpret the results
11. Identify key risks and assumptions
12. Present the model and conclusions clearly

### 1. Define the objective

Establish: what decision the model supports, what's being forecast, the relevant time horizon, required level of detail, which outputs matter most, and the intended audience. If the objective is unclear, make a reasonable interpretation and state it explicitly rather than inventing business context.

### 2. Identify and label inputs

Separate every input into one of three categories, and never blur them together:

- **Historical data** — things that already happened (historical revenue, expenses, margins, headcount, capex, cash flows, working capital)
- **Assumptions** — inputs that drive the forecast (growth, pricing, volume, cost inflation, headcount growth, tax rates, capex, working-capital assumptions, interest rates)
- **Outputs** — the metrics the model produces (revenue, gross/operating profit, net income, operating/free cash flow, ending cash, break-even, ROI)

**Never present an assumption as a historical fact.**

### 3. Establish model structure

Use a logical flow: **Inputs → Assumptions → Calculations → Outputs**. Where appropriate, structure into: Assumptions, Historical financials, Revenue build, Cost build, P&L, Working capital, Capex, Cash flow, Financing, Scenarios, Summary/output. Avoid unnecessary complexity — a model should be understandable and auditable by another person, not just by its builder.

### 4. Build revenue, cost, and profitability

Read `references/revenue-and-cost-modeling.md` for driver-based revenue forecasting, fixed/variable/semi-variable cost classification, and profitability modeling (gross profit → EBITDA → EBIT → net income) with margin checks.

### 5. Model cash flow and working capital

Read `references/cashflow-and-working-capital.md`. Never assume rising profit automatically means rising cash — identify cases where the business is profitable but cash-constrained.

### 6. Scenario, sensitivity, and break-even analysis

Read `references/scenario-sensitivity-breakeven.md` for how to build base/upside/downside scenarios, run sensitivity analysis on the assumptions that matter most, and calculate break-even points with operational meaning (not just a number).

### 7. Validate — or, if reviewing an existing model, audit first

Read `references/model-review-and-validation.md`. If the user hands you an existing model, **do not immediately rebuild it** — assess its structure, formulas, and assumptions first, and separate genuine model errors from business assumptions that are simply aggressive or conservative (don't call an assumption "wrong" just because it differs from your expectation).

### 8. Manage assumptions and handle uncertainty

Read `references/assumptions-and-qc.md` for how to handle missing assumptions (explain why it's needed, ask if essential, otherwise use a clearly labeled illustrative assumption), how to talk about uncertainty ("under the stated assumptions...", "the model indicates...", "the result is sensitive to..."), how to handle external data and spreadsheets, and the final QC checklist to run before presenting results.

## Output Format

Unless the user requests otherwise:

1. **Executive Summary** — most important results and business implications
2. **Objective** — what the model is designed to answer
3. **Key Inputs and Assumptions**
4. **Model Structure** — major relationships driving it
5. **Base Case Results**
6. **Scenario Analysis** (where appropriate)
7. **Sensitivity Analysis** — assumptions with the greatest impact
8. **Key Risks** — assumptions/conditions that could materially change the result
9. **Model Limitations** — missing information, simplifying assumptions
10. **Business Implications** — what it means for the decision at hand

## Core Rules

**Always**: build from clearly defined assumptions; keep historical data separate from forecasts; show the logic behind important calculations; verify calculations; prefer driver-based modeling when the data supports it; make assumptions transparent; test material uncertainty; explain business meaning; flag limitations; prioritize transparency and auditability.

**Never**: invent historical financial data; hide assumptions; present forecasts as guaranteed outcomes; treat model output as more reliable than its assumptions; ignore cash-flow implications; silently alter source data; present unsupported estimates as facts; claim a model is "accurate" merely because the arithmetic works.

## Final Objective

The model should help answer: What assumptions are driving the outcome? What's the expected result under the base case? What happens if key assumptions change? Which assumptions create the greatest risk? What does this imply for the business decision?


---

# Reference Material

The following sections were split into separate reference files in the modular version of this skill; they're inlined here since this export uses a single SKILL.md per skill.


## Assumptions And Qc

# Assumption Management, Uncertainty, and QC

## Assumption Management

Every important assumption should be explicit, traceable, reasonable, time-specific where appropriate, and clearly distinguished from historical data.

If an assumption materially affects the output, flag it as a **key assumption**. When the user hasn't supplied one that's needed:

1. Explain why it's needed.
2. Ask for it if it's essential to proceeding.
3. Otherwise, use a clearly labeled illustrative assumption.
4. Show how sensitive the result is to that assumption where appropriate.

Never disguise an estimate as a known fact.

## Talking About Uncertainty

Don't present a forecast as a prediction with certainty. Use language like:
- "Under the stated assumptions..."
- "The model indicates..."
- "The result is sensitive to..."
- "This scenario assumes..."
- "The available information does not establish..."

Consider and flag the assumptions most likely to affect the model: revenue uncertainty, cost inflation, demand changes, pricing pressure, interest rates, FX (where relevant), capital requirements, working-capital requirements, financing availability.

## External Data

If external information is used: identify the source, identify the relevant period, distinguish it clearly from user-provided data, ensure units/currencies are compatible, and explain any adjustments made. Don't combine incompatible datasets without warning, and don't treat external forecasts or market assumptions as though they were company-specific facts.

## Spreadsheet and Data Handling

When working with spreadsheets or structured data: preserve source data separately from calculated outputs; avoid overwriting original values; identify formulas vs. hard-coded inputs where possible; use consistent units; label assumptions clearly; maintain logical input→output relationships; check for missing/duplicated data; verify important calculations independently. If generating a spreadsheet model, make it understandable to another finance professional without requiring them to infer the structure.

## Final QC Checklist

Before finalizing:
- [ ] Objective is clearly defined
- [ ] Historical data is separated from assumptions
- [ ] Units and currencies are consistent
- [ ] Forecast period is clear
- [ ] Revenue assumptions are explicit
- [ ] Cost assumptions are explicit
- [ ] Cash-flow implications are considered
- [ ] Key formulas have been checked
- [ ] Major outputs reconcile
- [ ] Scenarios are logically constructed
- [ ] Important sensitivities are identified
- [ ] Missing information is disclosed
- [ ] Unsupported assumptions are not presented as facts
- [ ] Results are clearly connected to the business decision


## Cashflow And Working Capital

# Cash-Flow and Working-Capital Modeling

## Cash-Flow Modeling

When cash flow is relevant, distinguish accounting profitability from actual cash movement. Consider: operating cash flow, capital expenditure, working-capital changes, financing flows, debt repayments, equity financing, dividends, and ending cash.

**Do not assume that increasing profit automatically means increasing cash.** Explicitly identify situations where the business may be profitable but experience cash-flow pressure (e.g. rapid receivables/inventory growth consuming cash even as net income rises).

## Working Capital

Where relevant, consider accounts receivable, inventory, accounts payable, and other operating working-capital items, and how changes in each affect cash flow.

Use historical relationships (e.g. days sales outstanding, days inventory outstanding, days payable outstanding) where sufficient data exists to derive them. Where an assumption is required instead (e.g. no historical data to derive DSO), identify it explicitly as an assumption rather than presenting it as derived from the business's own history.


## Model Review And Validation

# Model Validation and Existing-Model Review

## Model Validation (for models you build)

Before presenting results, check:

**Arithmetic**: formulas calculate correctly; totals reconcile; percentages are correct; units are consistent; signs are correct.

**Financial logic**: revenue drivers produce reasonable revenue; costs behave consistently with their stated assumptions; profit changes appropriately when revenue or costs change; cash flow reflects the working-capital and investment assumptions used; debt/financing flows reconcile.

**Internal consistency** — check these relationships specifically:
- Revenue → gross profit
- Gross profit → operating profit
- Operating profit → net income
- Net income → cash flow (where appropriate)
- Capex → investing cash flow
- Debt changes → financing cash flow
- Opening cash + net cash movement → ending cash

Flag inconsistencies rather than silently correcting them.

## Existing Model Review

If the user provides an existing financial model, **do not immediately rebuild it.** First assess: structure, inputs, assumptions, formula logic, calculation errors, missing dependencies, hard-coded values, circular references (where identifiable), inconsistent formulas, broken links (where identifiable), unreasonable assumptions, and formatting/labeling issues that could cause misinterpretation.

**Keep these separate**:
- **Model errors** — genuine formula/logic/calculation mistakes.
- **Business assumptions that are simply aggressive or conservative** — not errors, just choices.

Do not label an assumption "incorrect" solely because it differs from your own expectation of what it should be.


## Revenue And Cost Modeling

# Revenue, Cost, and Profitability Modeling

## Revenue Modeling

Identify the appropriate revenue drivers for the business — depending on the model, these may include units sold, customers, average selling price, transactions, subscription users, ARPU, market share, geographic segments, or product categories.

**Prefer driver-based forecasting over arbitrary growth assumptions** when sufficient data is available. Example: `Units sold × Average selling price = Revenue`. If a driver-based approach isn't possible, clearly state the alternative assumption used instead (e.g. a flat growth rate) and label it as such.

## Cost Modeling

Separate costs where possible into:

- **Fixed costs** — don't change directly with activity in the modeled range (rent, certain salaries, software subscriptions, insurance)
- **Variable costs** — change with business activity (materials, transaction fees, shipping, sales commissions)
- **Semi-variable costs** — contain both fixed and variable components

Don't automatically classify a cost as fixed or variable without considering the business context — e.g. "salaries" can be either depending on staffing model.

## Profitability Modeling

Where relevant, model the full chain: Revenue → COGS → Gross Profit → Operating Expenses → EBITDA → D&A → EBIT → Interest → Taxes → Net Income.

Calculate and interpret relevant margins at each level, and sanity-check whether the modeled relationships make economic and business sense (e.g. does gross margin move in a way consistent with the cost assumptions used elsewhere in the model).


## Scenario Sensitivity Breakeven

# Scenario, Sensitivity, and Break-Even Analysis

## Scenario Analysis

When uncertainty is material, build multiple scenarios — typically base, upside, and downside cases. Scenarios should change **meaningful business drivers**, not just apply an arbitrary percentage adjustment to the final output.

Example downside scenario: lower unit growth, lower pricing, higher input costs, higher working-capital requirements — not just "revenue −10%."

Clearly explain which assumptions differ between scenarios and why.

## Sensitivity Analysis

Use sensitivity analysis to determine which assumptions have the greatest effect on important outputs. Candidate variables: revenue growth, pricing, volume, gross margin, opex, interest rates, capex, working capital. Prioritize variables that are both **uncertain** and **financially significant** — not every input is worth stress-testing.

**Scenario analysis vs. sensitivity analysis — keep these distinct:**
- Scenario analysis changes *multiple* assumptions together to represent a plausible business environment.
- Sensitivity analysis changes *one* (or a small number of) individual assumptions to see how strongly outputs respond.

## Break-Even Analysis

Determine the point at which revenue covers relevant costs. Consider fixed costs, variable costs, unit price, contribution margin, break-even units, and break-even revenue.

Explain what the break-even point means operationally (e.g. "the business needs to sell X units/month to cover fixed costs at current pricing and variable cost assumptions") rather than presenting it as an isolated number.
