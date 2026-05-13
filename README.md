# Retail Customer Segmentation & Behaviour Dashboard

**End-to-end customer analytics project | Python · pandas · Power BI · DAX**

A customer analytics project that transforms large-scale online grocery transaction data into customer-level behavioural features, strategic customer segments, and an interactive Power BI dashboard designed to support retention, growth, upsell, cross-sell, and reactivation decisions.

The latest rebuilt segmentation model is based on:

- **32.4M+ transaction rows**
- **206,209 customer records**
- **11 strategic customer segments**
- **8 structured Power BI export tables**
- **54.3K customers in the largest reactivation segment**

[View the full portfolio case study](https://www.elialanz.com/case-study-retail-customer-segmentation/)

---

## Project Overview

Retail and eCommerce teams often have access to large volumes of customer transaction data, but the business challenge is turning that data into clear targeting decisions.

This project addresses a practical commercial question:

> **Which customers should be protected, grown, upsold, cross-sold, reactivated, or monitored?**

To answer that, I rebuilt the analysis from the ground up using Python notebooks. The workflow moves from raw order and product data through customer-level aggregation, behavioural scoring, segmentation logic, Power BI-ready exports, and a stakeholder-facing dashboard.

The final dashboard is designed for CRM, marketing, commercial, and customer performance teams that need to move beyond generic reporting and understand which customer groups require action.

---

## Business Questions

- Which customer groups represent the strongest retention and growth opportunities?
- Which low-engagement segments create the largest reactivation opportunity?
- How do customer behaviour, reorder activity, product variety, and order volume differ across priority levels?
- Which strategic segments should receive different campaign treatments?
- How can customer-level data be translated into a practical dashboard for commercial decision-making?

---

## Tools & Technologies

| Layer | Tools |
|---|---|
| Data preparation | Python, Jupyter Notebook, pandas, NumPy |
| Customer analytics | Customer-level aggregation, percentile ranking, behavioural scoring, segmentation logic |
| Dashboard | Power BI, DAX, KPI cards, slicers, multi-page report design |
| Data export | CSV outputs for Power BI |
| Documentation | Markdown, GitHub README, portfolio case study |

---

## Project Structure

```text
Retail-Customer-Segmentation/
│
├── [01] Project Brief & Planning
│     └── project_brief.pdf
│
├── [02] Data
│     ├── [1] Original Data
│     ├── [2] Data Checks & Cleaning
│     └── [3] Prepared Data
│
├── [03] Python Scripts
│     ├── 01_DataChecks.ipynb
│     ├── 02_Profiling_Data_Merging.ipynb
│     ├── 03a_Customer_Level_Aggregation.ipynb
│     ├── 03b_Customer_Level_Aggregation.ipynb
│     ├── 04_percentile_ranks_behaviour_score.ipynb
│     ├── 05_behaviour_segmentation.ipynb
│     ├── 06_demographic_bands.ipynb
│     ├── 07_strategic_target_segmentation.ipynb
│     ├── 08_transaction_level_merging.ipynb
│     └── 09_exporting_powerbi_csv.ipynb
│
├── [04] Analysis & Visualizations
│     ├── [1] Reports
│     ├── [2] Visualizations
│     └── [3] Power BI Dashboard
│
├── [05] Final Deliverables
│
└── README.md
```

---

## Analytical Workflow

### 1. Data Checks

Loaded the source tables into Python and reviewed row counts, columns, data types, missing values, duplicate records, and structural consistency before building the segmentation model.

### 2. Profiling & Data Merging

Profiled the source data and merged the relevant order, product, department, and customer-level information into structured working datasets.

### 3. Customer-Level Aggregation

Converted transaction-level data into a customer-level dataset. This created one record per customer with behavioural fields such as order activity, product variety, reorder behaviour, average product price, demographic attributes, and regional information.

### 4. Percentile Ranking & Behaviour Score

Created percentile-based behavioural indicators to compare customers consistently across multiple dimensions. These ranking features were used to build a combined behaviour score that summarises customer engagement and value signals.

### 5. Behaviour Segmentation

Grouped customers into behaviour-based segments using purchasing patterns such as order volume, reorder behaviour, product variety, and price behaviour.

### 6. Demographic Bands

Created demographic and customer profile bands, including age, income, household, and region-based groupings. These fields were used to understand whether different customer types required different commercial actions.

### 7. Strategic Target Segmentation

Translated behavioural and demographic signals into **11 strategic customer segments** that are easier for non-technical stakeholders to understand and act on.

### 8. Transaction-Level Merging

Merged the final customer segmentation fields back into transaction-level data so that product and department targeting could be analysed by segment.

### 9. Power BI Export Tables

Exported **8 structured CSV files** for Power BI, including customer-level data, strategic segment summaries, priority summaries, behaviour summaries, region summaries, demographic summaries, department targeting, and product targeting.

---

## Segmentation Framework

The final model uses three connected layers:

### Priority Levels

Customers are grouped into four priority levels:

- **High Priority**
- **Growth Priority**
- **Maintain**
- **Low Priority**

These tiers help separate customers by engagement and commercial importance.

### Behaviour Segments

Behaviour segments describe how customers shop, based on order activity, product variety, reorder patterns, and price behaviour.

### Strategic Target Segments

The final business-facing segmentation layer contains 11 strategic customer groups:

- Protect High-Value Repeat Customers
- Protect Highly Engaged Customers
- Grow Affluent Active Customers
- Grow Active Family Shoppers
- Grow Active Value-Conscious Customers
- Cross-Sell Broad Basket Explorers
- Premium Higher Price Buyers
- Upsell Frequent Low-Price Buyers
- Maintain Stable Mid-Value Customers
- Reactivate Low-Engagement Families
- Reactivate Low-Engagement Customers

These labels are designed to support practical campaign decisions rather than only describe statistical groups.

---

## Power BI Dashboard

The Power BI dashboard consumes the Python-generated export tables and turns the segmentation model into a stakeholder-facing reporting tool.

### Dashboard Pages

**1. Executive Segmentation Overview**

A high-level summary of customer volume, priority tiers, strategic segments, and the largest reactivation opportunity.

**2. Behavioural & Targeting Analysis**

A deeper view of how customer behaviour changes across segments, including order activity, reorder behaviour, and department/product targeting opportunities.

**3. Demographic Insights**

A demographic view of how age, income, household type, and region interact with strategic customer groups.

### Core Dashboard Features

- KPI cards for customer volume, income, order activity, and reorder behaviour
- Interactive slicers for strategic segment, behaviour segment, priority level, and income group
- Segment distribution visuals
- Priority-level comparisons
- Department and product targeting outputs
- Business-focused insight callouts

---

## Dashboard Screenshot

![Dashboard Page 1](./[04]%20Analysis%20%26%20Visualizations/[3]%20Power%20BI%20Dashboard/dashboard_page1_segmentation_overview.png)

![Dashboard Page 1](./[04]%20Analysis%20%26%20Visualizations/[3]%20Power%20BI%20Dashboard/dashboard_filters_view.png)
---

## Key Findings

### 1. Reactivation is the largest commercial opportunity

**Reactivate Low-Engagement Families** is the largest strategic segment, with approximately **54.3K customers**. This group sits in a low-priority behavioural position but represents a major opportunity for reactivation campaigns.

### 2. High and Growth Priority customers drive the strongest behaviour

High and Growth Priority customers represent approximately **36.3% of the customer base** and show stronger behavioural quality, with around **30.9 average orders** and a **62.4% reorder rate**. These customers should be the primary audience for retention and growth campaigns.

### 3. Similar behaviour can still require different retention strategies

Some segments behave similarly but differ demographically. For example, highly engaged customer groups may show similar order and reorder patterns but differ by income and age profile, which can justify different campaign messaging, loyalty offers, or promotion types.

### 4. Strategic segments make the dashboard more actionable

Instead of only showing raw customer metrics, the dashboard translates customers into commercial action groups: protect, grow, cross-sell, upsell, maintain, and reactivate.

---

## Business Recommendations

| Priority | Recommendation | Target Segment / Audience |
|---|---|---|
| High | Launch targeted reactivation campaigns | Reactivate Low-Engagement Families |
| High | Protect loyal and high-value customers | Protect High-Value Repeat Customers / Protect Highly Engaged Customers |
| High | Prioritise retention and growth activity | High Priority and Growth Priority customers |
| Medium | Build value-led growth campaigns | Grow Active Value-Conscious Customers |
| Medium | Use basket expansion and cross-sell messaging | Cross-Sell Broad Basket Explorers |
| Medium | Promote premium products and bundles | Premium Higher Price Buyers |
| Low | Monitor stable customers and prevent decline | Maintain Stable Mid-Value Customers |

---

## Dashboard Validation & Quality Assurance

After rebuilding the segmentation outputs, the Power BI model was validated to ensure the dashboard consumed the new files correctly.

The validation work included:

- Checking that all 8 CSV exports loaded correctly into Power BI
- Confirming column names and data types across the rebuilt files
- Fixing Power Query locale settings using **en-US** to handle decimal values correctly
- Using **UTF-8 encoding** for safer CSV imports
- Removing a Power Query replacement step that was corrupting hyphenated segment names
- Auditing DAX measures for broken references or stale hardcoded labels
- Clearing stale slicer selections that referenced old segment labels
- Confirming that the final strategic segment labels loaded consistently across the dashboard

This QA work helped ensure the final report was not only visually complete, but also technically reliable after the segmentation rebuild.

---

## Repository Notes

> **Data size note:** Source datasets exceed GitHub file limits. Key prepared files and final outputs are available via Google Drive.
>
> [Download project files from Google Drive](https://drive.google.com/drive/folders/126mlE9SaTlVNDaQPcR5IXK9j_PoN6O2q?usp=drive_link)
>
> [View live interactive dashboard on Power BI Service](https://app.powerbi.com/links/HcLLvNLjq6?ctid=64d7125b-3f16-40ce-b3fe-2f79216f7403&pbi_source=linkShare)
>
> [Download the .pbix file from Google Drive](https://drive.google.com/file/d/1XrgxcVgy7i_58-F7BytnylFyb4pXjkrb/view?usp=sharing)

---

## Portfolio Case Study

A full business-facing version of this project is available on my portfolio website:

[Read the full case study](https://www.elialanz.com/case-study-retail-customer-segmentation/)

---

## Author

**Elia Lanzuise** · Data Analyst · Melbourne, VIC, Australia

[Portfolio](https://www.elialanz.com) · [LinkedIn](https://www.linkedin.com/in/elia-lanzuise) · [GitHub](https://github.com/elialanz)

---

## About

Built by **Elia Lanzuise**, a data analyst focused on customer analytics, Power BI dashboards, Python data preparation, segmentation, business reporting, and decision-ready analytics for commercial and operational teams.

[See how I work with clients](https://www.elialanz.com/dashboard-service/) · [Other data services I offer](https://www.elialanz.com/hire-me/) · [elialanz.com](https://www.elialanz.com)
