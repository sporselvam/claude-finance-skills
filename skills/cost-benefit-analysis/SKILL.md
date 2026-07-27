---
name: cost-benefit-analysis
description: Evaluate whether a proposed business decision, project, or investment is financially and economically worthwhile — identify and quantify costs and benefits, calculate NPV/IRR/ROI/payback, and compare alternatives with scenario and sensitivity analysis. Use this skill whenever the user wants to evaluate a business project, compare investment or strategy options, decide on new equipment/technology/hiring/outsourcing, assess a cost-saving initiative, or determine whether expected benefits justify expected costs — even if phrased casually like "is this worth it," "should we do X or Y," or "does this pay for itself."
---

# Cost-Benefit Analysis

Act as a cost-benefit analysis specialist supporting finance professionals, business analysts, managers, executives, and decision-makers. Identify, quantify, and compare relevant costs and benefits of a proposed decision, incorporating time value of money, opportunity costs, risk, and scenario analysis where appropriate. The goal is a structured economic assessment — **never present a conclusion as certain when it depends heavily on assumptions.**

## Workflow

### 1. Define the decision and baseline

Establish: what decision is being evaluated, what alternatives exist, the relevant time horizon, the decision-maker, the objective, and — critically — the **baseline ("do nothing") scenario**. Compare current situation vs. proposed situation vs. alternatives. **Never compare an initiative against zero costs and zero benefits if the business would incur costs or receive benefits anyway without it** — that inflates the apparent case for change.

### 2. Define the scope

Establish what's in scope: business unit, geography, time period, stakeholders, financial costs/benefits, operational and strategic effects, external effects where relevant. State the scope explicitly and avoid pulling in irrelevant costs or benefits just because they're available.

### 3. Identify costs and benefits

Read `references/costs-and-benefits-identification.md` for the full categorization of initial/recurring/indirect/opportunity costs and revenue/cost-saving/productivity/risk-reduction/strategic benefits, how to separate sunk costs (exclude them from the incremental decision) from opportunity costs (include them when material), and how to distinguish quantifiable financial benefits from genuinely qualitative ones — **don't force a dollar value onto a benefit just to make the analysis look more precise.**

### 4. Establish the baseline and calculate incremental effects

Read `references/baseline-and-incremental-analysis.md` for defining what happens without the proposal, and calculating: **Incremental Benefit = Benefit(with) − Benefit(without)**, **Incremental Cost = Cost(with) − Cost(without)**, **Net Benefit = Incremental Benefits − Incremental Costs**. Also covers choosing an appropriate, non-arbitrary time horizon.

### 5. Calculate financial return metrics

Read `references/financial-metrics.md` for time value of money, NPV, IRR, payback period, and ROI — including their formulas, what they mean, and their limitations. **Always state the methodology/formula used** — these vary by convention and aren't objectively "correct" once assumptions are baked in.

### 6. Assess risk, sensitivity, and scenarios

Read `references/risk-scenario-sensitivity.md` for systematically identifying risk categories, running sensitivity analysis to find which assumptions matter most, building base/upside/downside scenarios, calculating break-even points, and incorporating risk without double-counting it (e.g. don't stack a risk-adjusted discount rate on top of an already-conservative scenario).

### 7. Compare alternatives and non-financial factors

Read `references/alternatives-and-nonfinancial.md` for comparing multiple options consistently (same horizon, discount rate, currency, assumptions) and layering in qualitative factors (strategic alignment, employee/customer impact, brand, regulatory) without conflating them with quantified results. **Don't select an option solely because it has the lowest cost, highest ROI, or highest IRR** — weigh scale, risk, and strategic relevance too.

### 8. Finalize

Read `references/qc-and-missing-data.md` for handling missing information (never invent costs, benefits, or probabilities), using external benchmarks responsibly, and the final QC checklist to run before presenting.

## Output Format

Unless the user requests otherwise:

1. **Executive Summary** — the decision, key financial findings, major risks, headline conclusion
2. **Decision Being Evaluated** — the proposal and baseline
3. **Alternatives** — options being compared
4. **Costs** — initial, recurring, indirect, opportunity
5. **Benefits** — financial and non-financial
6. **Incremental Analysis** — vs. baseline
7. **Financial Returns** — NPV/IRR/ROI/payback, only where appropriate and supported
8. **Scenario Analysis**
9. **Sensitivity Analysis** — assumptions that matter most
10. **Risks and Non-Financial Factors**
11. **Recommendation Framework** — which option performs best under stated assumptions, and why — never presented as certain if the analysis is highly assumption-dependent
12. **Further Information Required**

## Core Rules

**Always**: compare against a realistic baseline; focus on incremental costs/benefits; exclude irrelevant sunk costs; consider opportunity costs where material; account for time value of money when relevant; make assumptions transparent; test material uncertainty; consider financial and non-financial effects; compare alternatives consistently; explain business meaning.

**Never**: invent costs or benefits; treat assumptions as facts; ignore material opportunity costs; include irrelevant sunk costs; use ROI/IRR/NPV/payback without defining the methodology; pick an option solely for the highest ROI/IRR; hide unfavorable scenarios; treat qualitative benefits as quantified without justification; present an uncertain conclusion as guaranteed.

## Final Objective

The analysis should answer: What are the alternatives? What will each cost? What benefits could each generate? What's the incremental economic value? What happens under different assumptions? Which risks could change the conclusion? Which option offers the strongest value relative to its cost and risk? The result should be economically rigorous, transparent, risk-aware, and decision-useful.


---

# Reference Material

The following sections were split into separate reference files in the modular version of this skill; they're inlined here since this export uses a single SKILL.md per skill.


## Alternatives And Nonfinancial

# Comparing Alternatives and Non-Financial Considerations

## Alternatives Analysis

When multiple options exist, compare them consistently — same time horizon, discount rate, currency, financial definitions, and assumptions where appropriate. Compare: initial investment, operating costs, benefits, NPV, IRR, payback, risk, strategic benefits, and implementation complexity.

**Don't select an option solely because it has the lowest cost** — the objective is the option with the strongest overall value relative to its risks and constraints, not the cheapest one on paper.

## Non-Financial Considerations

After the financial analysis, weigh relevant qualitative factors: strategic alignment, employee impact, customer experience, brand impact, regulatory considerations, operational complexity, scalability, competitive positioning.

**Clearly distinguish qualitative judgment from quantified financial results** — don't let a qualitative preference masquerade as a financial conclusion, and don't let a strong financial case silently override a serious qualitative concern (e.g. regulatory risk) without naming it explicitly in the recommendation.


## Baseline And Incremental Analysis

# Baseline, Incremental Analysis, and Time Horizon

## Establishing the Baseline

Define what happens if the business does *not* implement the proposal: existing operating costs, existing revenue, existing growth, existing risks, existing maintenance requirements, and expected future changes that would happen regardless.

The analysis should generally be based on **incremental effects** — what actually changes because of the decision. Avoid counting costs or benefits that would occur either way.

## Incremental Calculation

For each option:

- **Incremental Benefit = Benefit(with proposal) − Benefit(without proposal)**
- **Incremental Cost = Cost(with proposal) − Cost(without proposal)**
- **Net Benefit = Incremental Benefits − Incremental Costs**

Always clearly distinguish these incremental values from total company financial figures — don't let a small project's incremental numbers get confused with (or diluted by) company-wide totals.

## Time Horizon

Determine an appropriate analysis period based on: expected useful life, contract duration, investment horizon, technology lifecycle, expected project lifespan, or the relevant strategic horizon.

**Don't arbitrarily pick a time horizon that makes the proposal look more attractive** (e.g. stretching the horizon to capture more cumulative benefit than is realistic). State the selected period and explain why it fits the specific decision.


## Costs And Benefits Identification

# Identifying Costs and Benefits

## Costs

**Initial costs**: equipment, software, implementation, training, consulting, setup, installation, initial working capital.

**Recurring costs**: salaries, maintenance, software subscriptions, utilities, insurance, operating expenses, support costs.

**Indirect costs**: management time, employee disruption, transition costs, productivity losses, implementation risk.

**Opportunity costs**: what else the resources could have been used for. E.g. "if $1M is invested in Project A, that capital can't simultaneously go to Project B." Don't ignore opportunity costs when material — see the dedicated section below.

## Benefits

**Revenue benefits**: increased sales, new customers, higher prices, improved retention, new markets.

**Cost savings**: lower labor costs, lower procurement costs, reduced maintenance, lower energy costs, reduced waste.

**Productivity benefits**: time savings, increased output, reduced processing time, automation, improved employee productivity.

**Risk reduction**: reduced probability of costly failures, lower compliance risk, lower operational risk, reduced downtime.

**Strategic benefits**: increased market access, improved competitive position, greater scalability, improved customer experience, new capabilities.

**Don't automatically assign a dollar value to strategic benefits if there's no defensible method for doing so** — see the qualitative-benefits note below.

## Quantifiable vs. Non-Financial Benefits

Separate **quantifiable financial benefits** from **non-financial or hard-to-quantify benefits** (employee satisfaction, customer satisfaction, brand reputation, strategic flexibility, organizational capability). Don't force a monetary value onto a benefit just to make the analysis look more precise — state clearly when a benefit is qualitative and treat it as a qualitative input to the final recommendation rather than folding it into the numbers.

## Sunk Costs

Identify costs that have already occurred and can't be recovered. **Don't include sunk costs in the incremental decision analysis** unless they have a relevant future cash consequence. Focus only on costs and benefits that change depending on the decision being made now.

## Opportunity Cost

Where resources are limited, consider the value of the best realistic alternative use — capital, employee time, production capacity, management attention, warehouse space, equipment, technology resources. **Don't count an opportunity cost unless there's a plausible alternative use** — a purely hypothetical alternative isn't a real cost.


## Financial Metrics

# Financial Return Metrics

## Time Value of Money

When costs and benefits span multiple periods, account for the time value of money — a dollar today is generally worth more than a dollar in the future, since capital can potentially earn a return and future outcomes are uncertain. Use discounted cash flow analysis when appropriate.

## Net Present Value (NPV)

**NPV = Present Value of Future Cash Inflows − Present Value of Future Cash Outflows**

Clearly identify: initial investment, future cash flows, timing, discount rate, and terminal/residual value where relevant.

- **Positive NPV** → the project is expected to create value relative to the chosen discount rate and assumptions
- **Negative NPV** → the project is expected to destroy value relative to those same assumptions

**NPV is not an objective fact** — it's entirely dependent on the assumptions and discount rate used. State them explicitly alongside any NPV figure.

## Internal Rate of Return (IRR)

IRR is the discount rate at which the project's NPV equals zero. Use carefully — watch for multiple IRRs, unusual cash-flow patterns, differences in project size/timing, and reinvestment assumptions. **When comparing projects, don't automatically pick the one with the highest IRR** — a small project can have a high IRR but create less total value than a large project with a lower one. Consider NPV, scale, risk, and strategic relevance together.

## Payback Period

Measures how long it takes for cumulative cash flows to recover the initial investment. Also consider discounted payback where appropriate. State its limitations clearly: it can ignore cash flows after the payback point, traditional payback ignores time value of money, and it doesn't directly measure total value creation. **Don't use payback as the sole decision criterion** when a more complete analysis (NPV/IRR) is available.

## Return on Investment (ROI)

**ROI = Net Benefit ÷ Investment Cost** (state this or whatever formula is actually used — organizations define ROI differently). Always state the exact methodology. **Don't compare ROI figures across projects if their definitions or time periods differ materially** — an ROI computed over 1 year isn't comparable to one computed over 5 years without adjustment.


## Qc And Missing Data

# Missing Information, External Data, and QC

## Handling Missing Information

1. Identify what's missing.
2. Explain why it matters.
3. Continue with analysis that can be supported.
4. Use an assumption only when appropriate.
5. Clearly label illustrative assumptions.
6. Show sensitivity where the missing information could materially change the conclusion.

**Never invent expected savings, revenue, costs, or probabilities.**

## External Data

If external information is used: identify the source, identify the relevant period, distinguish external benchmarks from company-specific data, ensure units/currencies are compatible, and explain any adjustments made. **Don't use an industry benchmark as though it were a company-specific forecast.**

## Final QC Checklist

- [ ] Decision and baseline are clearly defined
- [ ] Relevant alternatives are identified
- [ ] Incremental costs are separated from sunk costs
- [ ] Opportunity costs have been considered where relevant
- [ ] Benefits are supported by evidence or clearly labeled as assumptions
- [ ] Financial and non-financial benefits are separated
- [ ] Time horizon is appropriate and explained
- [ ] Discount rate is clearly stated where used
- [ ] NPV calculations have been checked
- [ ] IRR calculations have been checked where used
- [ ] Payback methodology is clear
- [ ] ROI methodology is clear
- [ ] Scenario assumptions are explicit
- [ ] Sensitivity analysis identifies the key drivers
- [ ] Risks are considered across all categories
- [ ] Missing information is disclosed
- [ ] Qualitative judgments are separated from quantitative findings
- [ ] The recommendation reflects the underlying uncertainty rather than overstating confidence


## Risk Scenario Sensitivity

# Risk, Sensitivity, Scenario, and Break-Even Analysis

## Risk Analysis

Identify risks that could affect costs or benefits, across:

- **Financial risk**: cost overruns, lower-than-expected revenue, higher operating costs, financing costs
- **Operational risk**: implementation delays, productivity disruption, staffing problems, technology failure
- **Market risk**: lower demand, competitive responses, pricing changes
- **Strategic risk**: changes in business strategy, technology becoming obsolete, regulatory changes
- **Execution risk**: difficulty implementing the proposal, resource constraints, dependence on suppliers/third parties

Prioritize by potential financial impact.

## Sensitivity Analysis

Identify which assumptions have the greatest effect on the conclusion — candidates: initial investment, revenue growth, cost savings, operating costs, implementation time, project lifespan, discount rate, customer adoption, pricing. Test meaningful variations (lower-benefit scenario, higher-cost scenario, delayed implementation, shorter lifespan) and explain which assumptions matter most to the decision.

## Scenario Analysis

Where uncertainty is significant, build base/upside/downside cases and compare total costs, total benefits, net benefits, NPV, IRR (where appropriate), payback period, and key risks across them. **Don't assign probabilities to scenarios unless there's a defensible basis** for doing so.

## Break-Even Analysis

Calculate the point at which the initiative becomes financially worthwhile — break-even units, revenue, customers, cost savings, adoption rate, or time. Explain what it means operationally, e.g. "the project requires at least 12,000 additional units of annual sales to recover its incremental costs under the stated assumptions." **Don't treat break-even as a forecast** — it's a threshold, not a prediction that it will be reached.

## Risk-Adjusted Analysis

Incorporate risk through scenario analysis, sensitivity analysis, probability-weighted outcomes, risk-adjusted discount rates, or conservative assumptions. **Don't automatically raise the discount rate just because an initiative is risky** — explain the chosen methodology, and avoid double-counting risk by stacking multiple conservative adjustments (e.g. a risk-adjusted discount rate *and* an already-pessimistic downside scenario) onto the same uncertainty.
