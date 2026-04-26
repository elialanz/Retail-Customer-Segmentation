# Retail Customer Segmentation & Behaviour Dashboard

**End to end analytics pipeline | Python · Power BI**

A full stack customer analytics project combining a structured Python data preparation pipeline with an interactive Power BI dashboard. Built to support retention, growth, upsell, and reactivation strategy across a large scale retail eCommerce customer base of 162,000+ customers.

---

## Project Overview

This project addresses a core business problem in retail eCommerce: understanding *which customers to prioritise, why, and what action to take*. Rather than treating all customers equally, the analysis builds a rule based behavioural and demographic segmentation model that classifies customers into 11 strategic segments | enabling marketing and commercial teams to make faster, more targeted decisions.

The project is structured as a two layer analytics pipeline:

- **Layer 1 | Python pipeline:** Raw data import, profiling, cleaning, merging, feature engineering, and export of structured outputs
- **Layer 2 | Power BI dashboard:** Interactive stakeholder facing dashboard consuming the Python outputs, with slicers, KPI cards, and insight callouts designed for business decision making

---

## Business Questions

- Which customer segments represent the highest retention and revenue risk?
- Where are the largest untapped reactivation opportunities in the customer base?
- How do ordering behaviour, reorder rates, and average income differ across priority tiers?
- Which regions and income groups contain the highest value customer concentrations?
- What commercial actions should marketing and CRM teams prioritise?

---

## Tools & Technologies

| Layer | Tools |
|---|---|
| Data preparation | Python, Jupyter Notebook, pandas, NumPy |
| Visualisation (EDA) | matplotlib, seaborn |
| Dashboard | Power BI (DAX, slicers, KPI cards, multi page report) |
| Data export | CSV (8 structured output files) |
| Documentation | Markdown, Excel |

---

## Project Structure

```
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
│     ├── 01_data_import_and_initial_profiling.ipynb
│     ├── 02_data_wrangling_and_structuring.ipynb
│     ├── 03_data_quality_checks_and_cleaning.ipynb
│     ├── 04_data_combining_and_merging.ipynb
│     ├── 05a_data_corrections_for_analysis.ipynb
│     ├── 05b_outlier_and_data_corrections.ipynb
│     ├── 06b_feature_engineering_and_customer_flags.ipynb
│     ├── 07a_visual_exploration_and_insight_development.ipynb
│     └── 07b_visual_exploration_and_insight_development.ipynb
│
├── [04] Analysis & Visualizations
│     ├── [1] Reports
│     ├── [2] Visualizations
│     └── [3] Power BI Dashboard
│           ├── dashboard_page1_segmentation_overview.png
│           └── dashboard_page2_coming_soon.png
│
├── [05] Final Deliverables
│
└── README.md
```

---

## Analytical Workflow

### 1. Data Import & Profiling
Loaded multiple raw retail datasets into pandas. Reviewed structure, dimensions, data types, and descriptive statistics to establish a baseline understanding of data quality and completeness.

### 2. Data Wrangling & Structuring
Removed unnecessary columns, renamed fields for analytical clarity, adjusted data types, and standardised variable formats across datasets.

### 3. Data Quality Checks & Cleaning
Identified and resolved missing values, duplicate records, mixed data types, and out of range values. Documented all decisions for reproducibility.

### 4. Data Combining & Merging
Merged transactional, product, department, and customer datasets using shared identifier fields. Validated merge quality and resolved join inconsistencies.

### 5. Feature Engineering & Customer Flags
Engineered derived variables to support segmentation including loyalty tiers, order frequency bands, price range groupings, reorder behaviour classifications, and demographic profile flags. Produced 8 structured CSV exports for Power BI consumption.

### 6. Visual Exploration & Insight Development
Built charts to identify distributions, behavioural trends, outliers, and segment differences. Used findings to inform the segmentation framework and dashboard design.

### 7. Power BI Dashboard Development
Imported the 8 structured CSV outputs into Power BI. Built a multi page interactive dashboard with DAX measures, KPI cards, and slicers across strategic segment, region, and income group dimensions.

---

## Dashboard | Page 1: Segmentation Overview

![Dashboard Page 1](./[04]%20Analysis%20%26%20Visualizations/[3]%20Power%20BI%20Dashboard/dashboard_page1_segmentation_overview.png)

**Key metrics visible:**
- Total customers: 162,631
- Average income: $95.7K
- Average orders per customer: 18.8
- Average item reorder rate: 48.8%

**Interactive filters:** Strategic segment · Region · Income group

**11 strategic segments including:**
- High Priority | Protect: Highly Engaged Customers
- Growth Priority | Grow: Active Family Shoppers
- Maintain | Stable Mid Value Customers
- Reactivate | Low Engagement Families *(largest segment: 45.2K customers)*

> Pages 2 and 3 in development | full dashboard publishing May 2026

---

## Key Findings

**1. Reactivation is the single largest opportunity**
Low Engagement Families account for 45.2K customers | the largest segment in the entire base | yet sit in low priority by order activity. A targeted reactivation campaign for this group represents the highest potential revenue recovery opportunity.

**2. High Priority customers are disproportionately valuable**
High Priority customers average 54.7 orders and a 73.1% reorder rate, compared to 7.0 orders and 32.6% reorder rate for Low Priority customers. Protecting and growing this segment should be the primary retention focus.

**3. Premium segments are concentrated in specific regions and income bands**
Filtering to Very High Income + Northeast surfaces a Premium: Higher Price Buyers segment with average income of $150.4K and 18.1 average orders per customer | a clear upsell and premium product targeting opportunity.

**4. Mid value customers dominate volume but lack targeted strategy**
Maintain: Stable Mid Value Customers (38.5K) represent a large, stable base with moderate engagement. Tailored loyalty incentives for this group could shift a meaningful portion into Growth Priority over time.

---

## Business Recommendations

| Priority | Recommendation | Target Segment |
|---|---|---|
| High | Launch reactivation campaign | Low Engagement Families (45.2K) |
| High | Protect and deepen loyalty rewards | High Priority customers (18.1K) |
| Medium | Develop upsell campaign for premium products | Premium: Higher Price Buyers (1.7K) |
| Medium | Design loyalty incentive programme | Maintain: Stable Mid Value (38.5K) |
| Low | Monitor and re-engage | Low Engagement Customers (15.2K) |

---

## Repository Notes

> **Data size note:** Source datasets exceed GitHub file limits. Key prepared files and final outputs are available via Google Drive.
>
> [Download project files from Google Drive](https://drive.google.com/file/d/1tBwlvX_N_K7dNHm02v1ammVfMMvE4VVA/view?usp=sharing)

---

## Author

**Elia Lanzuise** · Data Analyst · Melbourne, VIC, Australia

[Portfolio](https://www.elialanz.com) · [LinkedIn](https://www.linkedin.com/in/elia-lanzuise) · [GitHub](https://github.com/elialanz)
