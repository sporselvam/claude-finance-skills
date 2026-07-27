# Claude Finance Skills

A modular collection of **Claude Skills designed for financial analysis, business intelligence, and finance-related decision-making**.

The project provides reusable AI workflows that help finance professionals and business teams analyze financial information, evaluate decisions, identify trends, and generate actionable insights from structured data.

---

## Overview

Modern finance teams work across large volumes of financial and business data, often requiring repetitive analysis, reporting, forecasting, and decision-making.

This project provides **Claude Skills** that can be structured into specialized, reusable analytical tools for common finance and business workflows.

Each skill is designed around a specific financial task and provides Claude with structured instructions, analytical frameworks, quality-control procedures, and output guidelines.

The skills can be used individually or combined into broader financial workflows.

---

## Skills

### 1. Economic Data Analysis

Analyzes economic and business datasets to identify trends, relationships, indicators, and economic insights relevant to business decision-making.

**Applications:**

* Economic indicators
* Market analysis
* Business environment analysis
* Trend identification
* Economic comparisons

---

### 2. Financial Statement Analysis

Analyzes financial statements to evaluate business performance, financial position, profitability, liquidity, efficiency, and financial risks.

**Applications:**

* Income statement analysis
* Balance sheet analysis
* Financial ratios
* Profitability analysis
* Financial health assessment

---

### 3. Financial Forecasting

Develops structured financial forecasts using historical information, assumptions, trends, and scenario analysis.

**Applications:**

* Revenue forecasting
* Expense forecasting
* Profit forecasting
* Financial planning
* Scenario analysis
* Forecast sensitivity

---

### 4. Budget & Variance Analysis

Compares actual performance against budgets, forecasts, or previous periods to identify material deviations and understand their financial implications.

**Applications:**

* Budget vs. actual analysis
* Expense variance analysis
* Revenue variance analysis
* Profit variance analysis
* Management reporting
* Corrective-action identification

---

### 5. Cash Flow Analysis

Analyzes cash generation, cash consumption, liquidity, working capital, free cash flow, and financing requirements.

**Applications:**

* Operating cash flow
* Free cash flow
* Liquidity analysis
* Cash runway
* Working-capital analysis
* Cash-flow forecasting

---

### 6. Cost-Benefit Analysis

Evaluates business decisions by comparing expected costs, benefits, risks, and financial returns.

**Applications:**

* Investment decisions
* Project evaluation
* Capital allocation
* Operational changes
* Technology investments
* ROI, NPV, IRR, and payback analysis

---

### 7. Financial Data Analysis

Analyzes structured financial and business datasets to identify trends, patterns, anomalies, KPIs, relationships, and actionable insights.

**Applications:**

* KPI analysis
* Financial performance analysis
* Segment analysis
* Trend analysis
* Anomaly detection
* Data-driven business insights

---

## Repository Structure

```text
claude-finance-skills/
│
├── README.md
│
├── skills/
│   │
│   ├── economic-data-analysis/
│   │   └── SKILL.md
│   │
│   ├── financial-statement-analysis/
│   │   └── SKILL.md
│   │
│   ├── financial-forecasting/
│   │   └── SKILL.md
│   │
│   ├── budget-variance-analysis/
│   │   └── SKILL.md
│   │
│   ├── cash-flow-analysis/
│   │   └── SKILL.md
│   │
│   ├── cost-benefit-analysis/
│   │   └── SKILL.md
│   │
│   └── financial-data-analysis/
│       └── SKILL.md
│
└── LICENSE
```

Each skill is contained within its own directory and includes a dedicated `SKILL.md` file containing its instructions and analytical framework.

---

## Design Principles

The skills were designed around several principles:

### Data Integrity

Skills are instructed to validate data before performing analysis and identify missing, inconsistent, or potentially incorrect information.

### Evidence-Based Analysis

The system should distinguish between observed information, calculated results, assumptions, and interpretations.

### Transparency

Important assumptions, methodologies, calculations, and limitations should be clearly communicated.

### Business Relevance

Analysis should move beyond presenting numbers and explain their implications for business decisions.

### Risk Awareness

Where uncertainty is significant, the skills encourage scenario analysis, sensitivity analysis, and explicit discussion of risks.

### Reusability

Each skill is designed as an independent module that can be used across different financial and business workflows.

---

## Potential Business Applications

The skills can support a range of finance and business functions, including:

* Financial Planning & Analysis (FP&A)
* Corporate finance
* Business analysis
* Management reporting
* Budgeting
* Financial forecasting
* Investment analysis
* Strategic planning
* Financial performance monitoring
* Business intelligence
* E-commerce analytics

---

## External Data Integration

The framework can potentially be extended with external business data sources.

One example is **Helium 10**, which can provide e-commerce data that may be useful for financial and business analysis.

Potential applications include:

* Product performance analysis
* Sales analysis
* Revenue trends
* Market analysis
* Product profitability
* E-commerce forecasting
* Competitive analysis

The external data integration is intended as an extension to the core skills rather than a requirement for using them.

---

## Example Workflow

A finance team could combine several skills into a single workflow:

```text
Raw Financial Data
        ↓
Financial Data Analysis
        ↓
Financial Statement Analysis
        ↓
Budget & Variance Analysis
        ↓
Cash Flow Analysis
        ↓
Financial Forecasting
        ↓
Cost-Benefit Analysis
        ↓
Business Decision
```

For example, a company considering a new investment could:

1. Analyze historical financial performance.
2. Identify relevant trends and KPIs.
3. Compare actual performance with budget.
4. Assess the effect on cash flow.
5. Forecast future financial outcomes.
6. Evaluate the investment using cost-benefit analysis.
7. Present the results to decision-makers.

---

## Intended Users

This project is intended for:

* Finance professionals
* FP&A teams
* Business analysts
* Financial analysts
* Managers
* Entrepreneurs
* Students learning financial analysis
* Teams experimenting with AI-assisted finance workflows

The skills are designed to **support human decision-making rather than replace professional judgment**.

---

## Limitations

AI-generated financial analysis should be reviewed before being used for material business decisions.

Users should independently verify:

* Source data
* Financial calculations
* Assumptions
* External information
* Forecasts
* Regulatory or accounting requirements
* Investment conclusions

The quality of the analysis depends heavily on the quality, completeness, and relevance of the information provided.

---

## Project Goals

This project aims to explore how specialized AI skills can be structured to support practical financial workflows.

The broader objectives are to:

* Create reusable finance-focused AI tools
* Improve the consistency of financial analysis
* Reduce repetitive analytical work
* Encourage structured financial reasoning
* Connect financial data with business decisions
* Demonstrate practical applications of Claude Skills

---

## Technology

This project is built around **Claude Skills**, using structured `SKILL.md` files to provide specialized instructions and workflows for finance-related tasks.

The repository is designed to be modular so that individual skills can be developed, tested, improved, and extended independently.

---

## Disclaimer

This project is intended for **educational, analytical, and workflow-support purposes**.

It does not constitute financial, investment, accounting, legal, or professional advice.

Users are responsible for independently verifying outputs before relying on them for real-world decisions.

---

## Author

Shreepranav Porselvam

---

## License

This project is licensed under the terms specified in the repository's `LICENSE` file.
