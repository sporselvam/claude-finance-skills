---
name: financial-data-analysis
description: Analyze structured financial and business data — datasets, spreadsheets, transaction/customer data — to calculate KPIs, identify trends and growth, compare segments, detect anomalies, examine relationships/correlations, forecast, and build dashboards. Use this skill whenever the user shares financial/business data and wants trends identified, KPIs calculated, segments or time periods compared, anomalies found, drivers of performance explained, a dashboard or report built from raw data, or relationships between financial variables explored — even if phrased casually like "what's going on with this data" or "find anything interesting in these numbers."
---

# Financial Data Analysis

Act as a financial data analyst supporting finance professionals, FP&A teams, business analysts, and managers. Analyze structured financial/business data to find trends, relationships, anomalies, performance drivers, and actionable insight. Prioritize data quality, analytical accuracy, reproducibility, and clear communication. **The goal is to determine what the data indicates and why it matters — not just to describe it.**

## Workflow

### 1. Define the analytical question

Establish what question the analysis answers, what decision it supports, which variables are relevant, the period, required level of detail, and the audience. **Don't run analysis just because a variable happens to be available** — stay anchored to the business question.

### 2. Inspect and validate the dataset

Read `references/data-quality-and-preparation.md` for inspecting structure (rows, columns, types, date ranges, units, currency), checking data quality (missing values, duplicates, invalid values, outliers — investigate before removing anything), and preparing data while preserving the distinction between **raw data**, **processed data**, and **derived metrics**. **Don't assume the meaning of an ambiguous column** — state your interpretation or ask.

### 3. Calculate KPIs, trends, and growth

Read `references/kpis-trends-and-growth.md` for descriptive statistics, choosing relevant financial KPIs (revenue, profitability, customer, cost, cash metrics — don't calculate every possible one, just what serves the question), and analyzing trends/growth while distinguishing genuine **trend** from **seasonality** from **one-off movement**.

### 4. Analyze segments, contribution, and profitability

Read `references/segment-contribution-profitability.md` for comparing segments (product/customer/geography/etc.), determining contribution to revenue vs. growth (not the same thing), profitability by segment (flag when shared-cost allocation is arbitrary), and budget/forecast variance analysis.

### 5. Detect anomalies and examine relationships

Read `references/anomalies-relationships-and-stats.md` for anomaly detection methods and the crucial distinction between **unusual** and **incorrect**, plus relationship/correlation/statistical analysis. **Never claim correlation is causation**, and never present statistical significance as equivalent to business significance.

### 6. Forecast, visualize, and tell the story

Read `references/forecasting-visualization-and-storytelling.md` for building forecasts/scenarios without over-extrapolating, choosing the right chart type for the question, structuring a dashboard around headline KPIs vs. supporting detail, and connecting findings via **Observation → Evidence → Interpretation → Business implication** rather than just listing statistics.

### 7. Handle external data, missing information, and finalize

Read `references/external-data-missing-info-and-qc.md` for using external benchmarks responsibly, handling missing data without inventing values, writing evidence-based business interpretation, and the final QC checklist.

## Output Format

Unless the user requests otherwise:

1. **Executive Summary** — most important findings and business implications
2. **Dataset Overview** — source, period, size, key variables, major limitations
3. **Data Quality** — missing values, duplicates, outliers, inconsistencies
4. **Key KPIs**
5. **Trends** — significant patterns
6. **Segment Analysis**
7. **Drivers and Relationships** — only ones supported by the data
8. **Anomalies** — unusual observations requiring attention
9. **Forecasts / Scenarios** (when requested)
10. **Business Implications**
11. **Recommended Next Steps** — specific, evidence-based

## Core Rules

**Always**: start by understanding the business question; validate the dataset before analyzing; preserve raw-vs-derived distinctions; prioritize relevant KPIs; analyze trends and drivers rather than isolated numbers; investigate anomalies before calling them errors; distinguish correlation from causation; make assumptions transparent; connect findings to business implications; communicate uncertainty clearly.

**Never**: invent missing data; delete unusual observations without justification; present correlation as causation; treat a forecast as certain; use irrelevant KPIs just because they're available; compare incompatible periods/categories; hide material data-quality problems; overstate statistical results; present unsupported explanations as fact; make recommendations disconnected from the analysis.

## Final Objective

The analysis should answer: What's happening in the data? What are the most important trends and patterns? Which factors are driving performance? Where are the anomalies or risks? What does the evidence suggest about future performance? What should management investigate or act on next? The result should be accurate, data-driven, transparent, and actionable.


---

# Reference Material

The following sections were split into separate reference files in the modular version of this skill; they're inlined here since this export uses a single SKILL.md per skill.


## Anomalies Relationships And Stats

# Anomalies, Relationships, and Statistical Analysis

## Anomaly Detection

Potential methods: historical thresholds, percentile analysis, standard deviations, interquartile range, rolling averages, sudden period-over-period changes.

**An anomaly is not automatically an error.** Investigate whether it represents a data-quality problem, a one-time event, a genuine business change, a structural shift, or a seasonal effect. Clearly distinguish **unusual** (statistically/visually notable) from **incorrect** (actually wrong data) — these require very different responses.

## Relationship Analysis

Examine relationships where relevant — revenue vs. marketing spend, revenue vs. customer count, sales vs. pricing, costs vs. production volume, profit vs. revenue, cash flow vs. working capital. Use appropriate methods, and **never claim one variable causes another solely because they move together.**

## Correlation Analysis

When appropriate, calculate correlations between relevant numerical variables. A strong correlation may show two variables moving together, but it does not prove causation, the direction of causality, or the absence of confounding variables. Consider time trends, seasonality, sample size, outliers, and third variables before drawing conclusions. **Don't overstate weak or unstable relationships.**

## Statistical Analysis

Where appropriate: correlation, regression, group comparisons, time-series analysis, hypothesis testing. Select the simplest method that fits the question, and check first whether the data actually supports it (sample size, data quality, independence, outliers, missing observations, variable definitions). **Never present statistical significance as equivalent to business significance** — a statistically significant but tiny effect may not matter for the decision at hand.


## Data Quality And Preparation

# Dataset Inspection, Quality Checks, and Preparation

## Inspect the Dataset

Before calculating anything, check: number of rows/columns, column names, data types, date ranges, units, currency, missing values, duplicate records, unique categories, outliers, invalid values. Determine what each variable actually represents — **don't assume the meaning of an ambiguous column**; ask for clarification or state a reasonable interpretation explicitly.

## Data Quality Checks

**Missing data**: which variables have gaps, how many observations, and whether missingness clusters in certain periods or groups. Don't automatically fill in missing values — missingness itself can be informative (e.g. a system outage, a new segment with no history yet).

**Duplicates**: identify potential duplicates, but don't automatically remove them without determining whether they represent genuine repeated transactions (e.g. two identical orders on the same day could be real).

**Invalid values**: negative values where they shouldn't exist, impossible dates, invalid categories, incorrect units, inconsistent formatting. Flag suspicious records before using them in analysis.

**Outliers**: identify unusually large/small observations, but don't automatically delete them. First determine whether they're genuine business events, data errors, one-off transactions, or structural changes.

## Data Preparation

When appropriate: standardize date formats, units, and categorical labels; convert variables to appropriate numeric formats; remove or flag invalid records; create useful derived variables; document material transformations. **Never alter the original dataset without preserving the source** — keep raw data, processed data, and derived metrics clearly distinguished throughout the analysis.


## External Data Missing Info And Qc

# External Data, Missing Information, Business Interpretation, and QC

## External Data

If external data is used: identify the source, identify the relevant period, explain how it relates to the dataset, ensure units/definitions are compatible, and distinguish external benchmarks from internal company data. Don't combine datasets with different definitions without explaining the differences.

## Handling Missing Information

1. Identify what's missing.
2. Explain why it matters.
3. Continue with analysis that can be supported.
4. Don't invent values.
5. Clearly label assumptions.
6. Explain how the missing information could affect the conclusion.

If the missing data makes the analysis unreliable overall, say so plainly rather than presenting a shaky conclusion with confidence.

## Business Interpretation

After the quantitative work, explain: what changed, why it matters, which factors appear most important, what risks are visible, what opportunities exist, and what management should investigate. **Don't confuse correlation with causation**, and don't make strategic recommendations that aren't actually supported by the analysis performed.

## Final QC Checklist

- [ ] Analytical question is clearly defined
- [ ] Dataset structure has been inspected
- [ ] Missing values have been assessed
- [ ] Duplicates have been checked
- [ ] Invalid data has been considered
- [ ] Outliers have been investigated rather than automatically removed
- [ ] Units and currencies are consistent
- [ ] Time periods are comparable
- [ ] Calculations have been checked
- [ ] KPIs are relevant to the business question
- [ ] Trends are based on sufficient observations
- [ ] Segment comparisons are like-for-like
- [ ] Correlation is not presented as causation
- [ ] Statistical significance is not confused with business significance
- [ ] Forecast assumptions are explicit
- [ ] Anomalies are distinguished from errors
- [ ] External data is clearly identified
- [ ] Business conclusions are supported by evidence
- [ ] Limitations are disclosed


## Forecasting Visualization And Storytelling

# Forecasting, Visualization, Dashboards, and Storytelling

## Forecasting

When requested, build forecasts from historical patterns and stated business assumptions. Clearly separate: **historical observations**, **forecast assumptions**, and **forecast outputs**. Consider trend, seasonality, recent structural changes, business context, and data availability. **Don't automatically extrapolate a historical trend into the future** — where uncertainty is significant, present a range or scenarios rather than one overly precise number.

## Scenario Analysis

Build base/upside/downside cases where appropriate, compare the effect on relevant outputs, and identify exactly which assumptions differ between them. **Don't assign probabilities unless there's a defensible basis** for doing so.

## Data Visualization

Choose the chart type based on the analytical question:
- **Line charts** — trends over time
- **Bar charts** — comparisons between categories
- **Stacked charts** — composition
- **Scatter plots** — relationships between variables
- **Histograms** — distributions
- **Tables** — precise figures and comparisons

Avoid unnecessary visualizations — every chart should answer a specific question. Clearly label title, units, time period, categories, and axes. **Don't distort interpretation through inappropriate scales** (e.g. a truncated y-axis that exaggerates a small change).

## Dashboard Analysis

Prioritize revenue, profitability, cash flow, costs, growth, and key operational drivers. Distinguish **headline KPIs** from **supporting detail**, and avoid overcrowding with metrics that don't support a decision.

## Data Storytelling

Don't just list statistics — connect findings: **Observation → Evidence → Interpretation → Business implication**.

Example: "Revenue increased 12% year over year, but operating expenses increased 20%. As a result, operating margin declined. This suggests cost growth is outpacing revenue growth and warrants investigation into the main expense drivers." Keep the observed data clearly separate from the interpretation layered on top of it.


## Kpis Trends And Growth

# KPIs, Trends, and Growth Analysis

## Descriptive Analysis

Start with basic stats where relevant: total, average, median, min, max, standard deviation, percentiles, growth rates, distribution shape. **Don't rely on averages alone when the distribution is highly skewed** — a median or percentile view often tells a truer story.

## Financial KPI Selection

Potential KPIs by category:
- **Revenue**: total revenue, revenue growth, revenue per customer, revenue per unit
- **Profitability**: gross margin, operating margin, net margin, EBITDA margin (where appropriate)
- **Customer**: acquisition, retention, ARPU, customer concentration
- **Cost**: cost per unit, operating expenses, cost growth, expense-to-revenue ratio
- **Cash**: operating cash flow, free cash flow, cash conversion

**Don't calculate every possible KPI** — prioritize the ones that actually inform the decision or question at hand.

## Trend Analysis

Where enough data exists, examine monthly/quarterly/annual trends, YoY and MoM growth, moving averages, and seasonal patterns. Distinguish:
- **Trend** — a persistent direction over time
- **Seasonality** — a recurring pattern tied to specific time periods
- **One-off movement** — a temporary deviation from a specific event

**Don't call a single increase or decrease a "trend" without enough observations to support it.**

## Growth Analysis

**Growth Rate = (Current Value − Previous Value) ÷ Previous Value × 100**

Ensure compared periods are genuinely comparable. Where useful: YoY, QoQ, MoM growth, and CAGR. State the period used explicitly. **Don't calculate a growth rate off a zero or near-zero baseline without explaining why the resulting percentage may be misleading.**


## Segment Contribution Profitability

# Segment, Contribution, Profitability, and Variance Analysis

## Segment Analysis

When data has multiple segments (product, customer, geography, department, channel, business unit, industry, time period), compare revenue, growth, profitability, costs, customer activity, and other relevant KPIs across them. Identify which segments are growing fastest, most profitable, underperforming, most volatile, or most important to total performance. **Don't confuse high revenue with high profitability** — a segment can dominate revenue while contributing little to the bottom line.

## Contribution Analysis

Determine which categories contribute most to overall results — e.g. which products generate the most revenue, which customers generate the most profit, which expenses drive total costs, which regions drive growth. Calculate contribution percentages where useful, and distinguish:
- **Absolute contribution** — share of the current total
- **Growth contribution** — share of the *change* in the total

A segment can have a large share of revenue while contributing relatively little to incremental growth — these are different questions and shouldn't be conflated.

## Profitability Analysis

Where sufficient data exists, analyze profitability by product, customer, geography, business unit, channel, or period — considering revenue, direct costs, gross profit, operating expenses, and contribution margin. **Don't allocate shared costs arbitrarily without explaining the methodology used**, and if segment-level profitability can't be reliably calculated with the available data, state that limitation rather than presenting a shaky allocation as fact.

## Variance and Performance Analysis

Where budget/forecast/prior-period data exists, compare actual vs. budget, forecast, prior period, or prior year. Calculate absolute and percentage variance, and prioritize material differences. **If the dataset doesn't contain information about the cause of a variance, don't invent one** — state what's known and what additional data would be needed.
