# Monster vs. Celsius: What Drives Profitability in the Energy Drink Industry?

> **Course:** BR 6210 — Quantitative Methods for Business Research  
> **Presented at:** 12th Annual Research Symposium, Madonna University — April 2026  
> **Author:** Nikola Sasaroga | MBA Candidate, Madonna University  
> 📧 nikola.sasaroga@gmail.com | [LinkedIn](https://linkedin.com/in/nikola-sasaroga)

---

## Project Overview

This study examines what drives profitability in the energy drink industry by analyzing 10 years of financial data (2016–2025) from two publicly traded companies: **Monster Beverage Corporation** and **Celsius Holdings, Inc.**

The core question: **Does revenue growth actually lead to higher profit — or does cost control matter more?**

Using multiple linear regression (OLS) in Microsoft Excel, the project quantifies the relationship between production costs (COGS), marketing and administrative expenses (SG&A), revenue growth, and EBITDA margin.

---

## Dataset

| Detail | Value |
|--------|-------|
| **Sources** | SEC EDGAR 10-K Annual Filings, Yahoo Finance |
| **Companies** | Monster Beverage Corporation, Celsius Holdings |
| **Period** | 2016 – 2025 |
| **Observations** | 20 (10 per company, panel dataset) |

**Variables:**

| Variable | Role | Description |
|----------|------|-------------|
| `EBITDA_Margin` | Dependent (Y) | Profitability measure: EBITDA / Revenue |
| `COGS / Revenue` | Independent (X1) | Production cost efficiency |
| `SG&A / Revenue` | Independent (X2) | Marketing & admin spend intensity |
| `Revenue Growth` | Independent (X3) | YoY revenue growth rate |

**Why EBITDA margin?** It eliminates the effects of capital structure, tax strategy, and non-cash items — enabling a direct comparison between companies with very different financial structures.

---

## Methodology

- **Tool:** Microsoft Excel (Data Analysis Toolpak — OLS Regression)
- **Model:** `EBITDA Margin = β₀ + β₁(COGS/Rev) + β₂(SG&A/Rev) + β₃(Revenue Growth) + ε`
- **Visualizations:** Scatter plots (Growth vs. Profitability, COGS vs. EBITDA)

---

## Descriptive Statistics (2016–2025)

| Metric | Monster | Celsius |
|--------|---------|---------|
| Avg. EBITDA Margin | **32.6%** | **-3.6%** |
| Avg. COGS / Revenue | 42.4% | 55.5% |
| Avg. SG&A / Revenue | 26.3% | 47.1% |
| Avg. Revenue Growth | ~11.8% / year | ~69.2% / year |

Monster = stable, high-margin operator. Celsius = aggressive growth, volatile margins.

---

## Regression Results — Combined Model (n = 20)

| | Value |
|--|-------|
| **Adjusted R²** | **0.979** |
| **F-test p-value** | < 0.001 (model significant overall) |

| Variable | Coefficient (β) | p-value | Significant? |
|----------|----------------|---------|:---:|
| COGS / Revenue | **−0.988** | < 0.001 | ✅ Yes |
| SG&A / Revenue | **−0.968** | < 0.001 | ✅ Yes |
| Revenue Growth | −0.035 | 0.157 | ❌ No |

**Interpretation:**
- Every 1 percentage point increase in COGS/Revenue → EBITDA margin drops ~0.99 pp
- Every 1 percentage point increase in SG&A/Revenue → EBITDA margin drops ~0.97 pp
- Revenue growth has **no statistically significant effect** on profitability once cost factors are controlled

> **SG&A finding contradicts initial hypothesis:** Marketing spend was expected to *boost* margins through revenue gains. The data shows the opposite — costs are not fully offset by resulting revenue, compressing margins.

---

## Company-Level Regression Comparison

| Factor | Monster (R² = 0.999) | Celsius (R² = 0.952) |
|--------|---------------------|---------------------|
| COGS / Revenue | β = −1.032 (p < 0.001) ✅ | β = −0.199 (p = 0.736) ❌ |
| SG&A / Revenue | β = −1.004 (p < 0.001) ✅ | β = −1.070 (p < 0.001) ✅ |
| Revenue Growth | β = −0.020 (p = 0.275) ❌ | β = −0.035 (p = 0.394) ❌ |

**Key insight:** For Monster, **both** cost factors drive profitability equally. For Celsius, profitability is almost exclusively determined by SG&A — reflecting a company still in an aggressive growth/spending phase.

---

## Core Conclusion

> **Cost efficiency drives profitability — not revenue growth.**

Monster's disciplined cost management produces consistent ~30%+ EBITDA margins, even with slower growth (~12%/year). Celsius's explosive growth (~69%/year average) has not translated into consistent profitability — and in several years produced negative EBITDA margins due to SG&A intensity exceeding 60% of revenue.

Long-term success in the energy drink industry depends on **balancing expansion with cost control** — not growth alone.

---

## Limitations

- Small sample (n=20, 2 companies) — limits generalizability
- SG&A used as marketing proxy (includes admin/overhead costs)
- Model does not capture pricing strategy, distribution efficiency, or marketing ROI

---

## Files in This Repository

| File | Description |
|------|-------------|
| `data/energy_drink_data.xlsx` | Full dataset — raw financials, calculated ratios, regression output |
| `report/written_report.pdf` | Full academic write-up (APA format) |
| `visuals/symposium_poster.jpg` | Research poster presented at Madonna University 12th Annual Symposium |

---

## Skills Demonstrated

`Excel` · `OLS Multiple Regression` · `Panel Data Analysis` · `Data Cleaning` · `Financial Ratio Analysis` · `SEC EDGAR` · `KPI Interpretation` · `Data Visualization` · `Statistical Inference` · `Business Storytelling`

---

## Certifications (Related Research Integrity)

Completed CITI Program certifications through Madonna University (Nov 2025):
- Human Subjects Research — Research Integrity Training
- Training for IRB Committee Members  
- Responsible Conduct of Research — Plagiarism

---

*This project was prepared for educational purposes as part of BR 6210 — Quantitative Methods for Business Research, Madonna University, April 2026.*
