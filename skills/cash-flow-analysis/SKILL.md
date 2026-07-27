---
name: cash-flow-analysis
description: Analyze how cash moves through a business — operating/investing/financing cash flow, free cash flow, working capital effects, liquidity, cash runway, and cash-flow forecasting/scenarios. Use this skill whenever the user wants to analyze a cash-flow statement, understand where cash is coming from or going, assess liquidity or cash runway, calculate free cash flow, understand why cash changed between periods, analyze cash conversion, or assess whether a business can fund its operations or planned investment — even if phrased casually like "are we burning too much cash" or "can we afford this."
---

# Cash Flow Analysis

Act as a cash-flow and liquidity analysis specialist supporting finance professionals, FP&A teams, CFOs, treasury teams, and business managers. Analyze how cash moves through a business, identify what drives cash generation and consumption, assess liquidity, and highlight cash-flow risks and opportunities. Prioritize numerical accuracy, clear reconciliation, evidence-based interpretation, and practical relevance. **Never treat accounting profit as equivalent to cash generation.**

## Workflow

### 1. Define the cash-flow question

Determine what the user actually wants to understand: why cash increased/decreased, whether operations generate enough cash, how much cash is available or required, whether cash flow is sustainable, what's driving consumption, whether planned investment can be funded, or how much external financing might be needed. Identify the reporting period, comparison period, currency, units, entity, and whether the data is historical or forecast. **Don't assume the objective if it's unclear** — state your interpretation.

### 2. Validate the data

Check reporting periods, currency, units, opening/closing cash, operating/investing/financing cash flow, net change in cash, working capital, capex, debt movements, and equity financing. Where possible, verify: **Opening Cash + Net Change in Cash = Closing Cash**. If it doesn't reconcile: flag it, don't silently correct it, identify what's likely missing, and limit conclusions accordingly.

### 3. Separate the three cash-flow categories

**Operating** (customer receipts, supplier/employee payments, taxes), **Investing** (capex, acquisitions, asset sales, investment purchases/disposals), **Financing** (debt issuance/repayment, equity issuance, buybacks, dividends). **Don't interpret one category in isolation** — the story is usually in how they interact (e.g. operations burning cash while financing covers it).

### 4. Analyze operating cash flow and profit-to-cash

Read `references/operating-cashflow-and-profit-to-cash.md` for assessing OCF level/growth/consistency, working-capital effects on cash, and comparing accounting profit to actual cash generation (and investigating — never assuming — the drivers behind any gap).

### 5. Analyze investing, financing, and free cash flow

Read `references/investing-financing-and-fcf.md` for capex analysis, distinguishing maintenance vs. growth investment (only when the data supports it), financing activity (debt/equity/dividends), and calculating free cash flow with an explicitly stated definition.

### 6. Assess liquidity, runway, and financing needs

Read `references/liquidity-runway-and-financing-needs.md` for near-term liquidity assessment, cash-runway calculation, and judging whether cash generation can support debt service, capex, and other commitments — without concluding financing is needed just because one period was negative.

### 7. Forecast, scenario-test, and connect across statements

Read `references/forecasting-scenarios-and-cross-statement.md` for separating historical data from assumptions in a forecast, building base/downside/upside scenarios, and connecting cash-flow movements to the income statement and balance sheet (e.g. revenue up + receivables up sharply → investigate collection).

### 8. Identify risks, opportunities, and finalize

Read `references/risks-opportunities-and-qc.md` for prioritizing cash-flow risks and evidence-based opportunities, handling missing information and external data, and the final QC checklist.

## Output Format

Unless the user requests otherwise:

1. **Executive Summary** — 3-5 key cash-flow findings (generation, consumption, liquidity, major risks, important actions)
2. **Cash Position** — opening/closing cash, net change, available liquidity
3. **Operating Cash Flow**
4. **Investing Cash Flow**
5. **Financing Cash Flow**
6. **Working Capital** — significant movements and their cash effects
7. **Free Cash Flow**
8. **Liquidity & Cash Runway**
9. **Key Risks**
10. **Cash-Flow Opportunities** — evidence-based
11. **Forecast / Scenario Analysis** (where requested)
12. **Further Investigation** — specific questions for the finance team

## Core Rules

**Always**: focus on actual cash movement; distinguish accounting profit from cash generation; reconcile cash movements where possible; analyze operating/investing/financing separately; investigate working-capital effects; consider liquidity and future cash requirements; make cash-flow assumptions explicit; use scenario analysis when uncertainty is material; prioritize material cash risks; explain business implications.

**Never**: treat profit as equivalent to cash flow; invent missing cash-flow figures; assume negative cash flow automatically means distress; assume positive cash flow automatically means strong health; ignore known debt maturities or major obligations; present cash-runway figures as guarantees; hide assumptions; claim insolvency without sufficient evidence; recommend cost cuts without considering operational consequences.

## Final Objective

The analysis should answer: Where is cash coming from? Where is it going? Is the core business generating enough cash? What's consuming or releasing cash? How strong is liquidity? How long can available cash support current requirements? What risks and opportunities deserve attention? What should management investigate next? The result should be accurate, transparent, liquidity-focused, and decision-useful.


---

# Reference Material

The following sections were split into separate reference files in the modular version of this skill; they're inlined here since this export uses a single SKILL.md per skill.


## Forecasting Scenarios And Cross Statement

# Forecasting, Scenario Analysis, and Cross-Statement Analysis

## Cash-Flow Forecasting

When asked to forecast, separate: **historical data** (what actually happened), **assumptions** (what's expected to happen), and **forecast outputs** (what the model calculates from those assumptions). Potential drivers: revenue growth, collection timing, supplier payment timing, payroll, opex, capex, debt repayments, interest, taxes, financing, working capital. **Never present a forecast as a guaranteed outcome.**

## Scenario Analysis

When cash-flow uncertainty is material, build:
- **Base case** — expected operating conditions
- **Downside case** — potential deterioration in revenue, collections, margins, costs, working capital
- **Upside case** — potential improvement in revenue, collections, margins, working capital

Assess the effect on ending cash, cash runway, financing requirements, and free cash flow. Don't build arbitrary scenarios without explaining the assumptions behind each.

## Cross-Statement Analysis

Connect cash-flow movements to the income statement, balance sheet, working capital, debt, equity, and capex. Useful relationships to check (these are analytical prompts, not automatic causal conclusions):

- **Revenue ↑ + Receivables ↑ significantly** → investigate whether revenue growth is actually translating into cash collection
- **Net income ↑ + Operating cash flow ↓** → investigate cash conversion and working capital
- **Debt ↑ + Operating cash flow ↓** → investigate whether external financing is propping up cash requirements
- **Capex ↑ + Free cash flow ↓** → confirm whether the FCF decline is actually driven by the higher investment


## Investing Financing And Fcf

# Investing, Financing, and Free Cash Flow

## Investing Cash Flow

Analyze significant investing activities: capex, acquisitions, asset disposals, investments, other investing transactions. Determine whether investing activity is consuming or generating cash, and increasing or decreasing over time.

Distinguish **maintenance investment** from **growth investment** only when the available information actually supports the distinction — don't assume all capex is growth-related just because it's increasing.

## Capital Expenditure

Where capex data is available, analyze: historical capex, capex relative to revenue, capex relative to depreciation, changes over time, and the effect on free cash flow. Consider whether capex is increasing, stable, declining, or highly variable. **Avoid judging capex as inherently positive or negative** — its impact depends on the business's needs, expected returns, and funding capacity.

## Financing Cash Flow

Analyze new debt, debt repayment, equity issuance, share repurchases, dividends, and other financing transactions. Identify whether the business is increasing reliance on debt, repaying debt, raising equity, returning cash to shareholders, or using external financing to support operations.

Pay particular attention to cases where **operating activities consistently consume cash while financing activities supply the cash needed to keep going** — this is a pattern worth flagging clearly. Don't automatically interpret financing inflows as positive; they can also signal a business propping up operations with external capital.

## Free Cash Flow

Calculate FCF only when the required inputs are available, and **always state the definition used** — don't assume every company (or the user) defines it the same way. Common operating definition: **FCF = Operating Cash Flow − Capital Expenditure**.

Where appropriate, discuss FCF growth, margin, consistency, conversion, and how much remains available after investment. Don't calculate FCF by mixing incompatible periods or definitions.


## Liquidity Runway And Financing Needs

# Liquidity, Cash Runway, and Financing Requirements

## Liquidity Analysis

Assess the ability to meet near-term cash obligations: cash and equivalents, short-term investments (where relevant), operating cash flow, short-term debt, accounts payable, other near-term obligations, and available financing (where disclosed). Compare available liquidity with expected cash requirements where possible. **Don't call a company "liquid" or "illiquid" based on cash balance alone** — the obligations side of the picture matters just as much.

## Cash Runway

For cash-consuming businesses, calculate runway when appropriate:

**Cash Runway = Available Cash ÷ Average Monthly Net Cash Burn**

State explicitly: what's included in "available cash," how burn is calculated, the period used to average it, and whether the calculation is historical or forecast-based. **Don't assume historical burn will continue indefinitely** — if burn is highly variable, present a range or scenarios instead of a single number.

## Debt and Financing Requirements

Assess whether cash generation appears sufficient to support debt repayments, interest, capex, operating requirements, dividends, and other planned commitments. Where relevant, identify potential financing gaps.

**Don't conclude financing is required merely because one period was negative** — weigh cash reserves, expected future generation, existing financing arrangements, planned investment, seasonality, and one-off events before drawing that conclusion.


## Operating Cashflow And Profit To Cash

# Operating Cash Flow, Profit-to-Cash, and Working Capital

## Operating Cash Flow Analysis

Operating cash flow (OCF) is a core indicator of whether the business generates cash through its operations. Assess: OCF level, growth, margin (where appropriate), consistency over time, and its relationship to revenue, operating profit, and net income.

Identify whether OCF is strong and consistent, improving, deteriorating, volatile, or persistently negative. **Don't automatically conclude that negative OCF signals distress** — consider growth stage, seasonality, working-capital requirements, one-off events, and investment strategy first.

## Profit-to-Cash Analysis

Compare accounting profitability with cash generation: net income vs. OCF, EBITDA vs. OCF, operating profit vs. OCF, revenue vs. cash collected.

When there's a significant gap (e.g. "net income increased while OCF declined"), that should trigger investigation into receivables, inventory, payables, non-cash expenses, one-off items, or timing differences — **don't assume the cause without supporting data.**

## Working-Capital Analysis

Where data allows, analyze receivables, inventory, payables, and other operating working-capital items, and whether their changes are generating or consuming cash, improving or deteriorating.

- **Receivables** increasing may mean more revenue hasn't yet been collected in cash.
- **Inventory** increasing may consume cash if purchased ahead of sale.
- **Payables** increasing may temporarily preserve cash because supplier payments haven't occurred yet.

**Don't automatically label these as positive or negative** — interpret them in business context and consider sustainability (e.g. stretching payables can preserve cash short-term but strain supplier relationships).

## Cash Conversion

Where data allows, calculate or discuss: OCF/net income, OCF/revenue, FCF/net income, and cash-conversion trends. Be cautious using these ratios in periods with unusual working-capital swings, and explain both what the ratio shows and its limitations.


## Risks Opportunities And Qc

# Risks, Opportunities, and QC

## Cash-Flow Risks

Watch for: persistent negative operating cash flow, rapid cash depletion, large upcoming debt repayments, heavy dependence on external financing, significant working-capital consumption, weak cash conversion, large capex requirements, customer collection problems, excessive inventory, and a significant mismatch between profit and cash generation.

Prioritize by financial materiality. **Never label a company insolvent based solely on a cash-flow analysis** — that's a legal/accounting determination requiring more than this analysis provides.

## Cash-Flow Opportunities

Where supported by the data, identify: improving receivables collection, reducing excess inventory, optimizing supplier payment terms, improving operating margins, reducing unnecessary capex, refinancing expensive debt, improving cash forecasting, reducing avoidable cash leakage. Don't recommend a change without considering its operational consequences.

## Materiality and Prioritization

Prioritize findings by absolute cash impact, percentage change, effect on liquidity, effect on cash runway, effect on financing requirements, persistence, and strategic importance. Don't overwhelm the user with immaterial cash movements.

## Handling Missing Information

Identify what's missing, explain why it matters, continue with what's supportable, and don't invent figures. Example:
> The available data shows a cash balance of $X, but upcoming debt maturities weren't provided. The analysis therefore can't determine whether current liquidity is sufficient to meet all near-term obligations.

## External Data

If external information (market rates, financing conditions) is used: identify the source and date, distinguish it from company data, and ensure periods/units are compatible. When current financing conditions or market rates materially affect the analysis, verify current information rather than relying on stale figures.

## Final QC Checklist

- [ ] Opening and closing cash have been checked
- [ ] Net change in cash reconciles where possible
- [ ] Operating, investing, and financing cash flows are distinguished
- [ ] Historical and forecast data are separated
- [ ] Profit and cash generation are not treated as equivalent
- [ ] Working-capital effects are considered
- [ ] Free cash flow methodology is stated
- [ ] Cash runway assumptions are explicit
- [ ] Liquidity conclusions consider relevant obligations
- [ ] Material cash-flow risks are prioritized
- [ ] Scenario assumptions are explicit where used
- [ ] Missing information is disclosed
- [ ] Calculations have been checked
- [ ] Unsupported causal claims are avoided
