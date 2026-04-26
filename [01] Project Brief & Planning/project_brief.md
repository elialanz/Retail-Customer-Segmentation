# Retail Customer Segmentation & Behaviour Dashboard
## Project Brief

**Project Type:** End-to-end retail analytics — customer segmentation, behavioural profiling, and interactive dashboard development

**Primary Tools:** Python, Jupyter Notebook, pandas, NumPy, matplotlib, seaborn, Power BI

**Data Scope:** Large-scale retail eCommerce transactional dataset (162,000+ customers) combined with supplemental customer demographic and profile data

**Intended Audience:** Marketing, CRM, customer strategy, and commercial decision-makers

---

## 1. Executive Summary

This project addresses a core commercial challenge in retail eCommerce: understanding which customers to prioritise, why, and what action to take. The business has strong order volume but lacks a structured view of how different customer groups behave and where marketing and sales actions can be more precisely targeted.

The engagement is scoped as a full-stack analytics pipeline — from raw data through to a stakeholder-ready interactive dashboard. The work covers data preparation, feature engineering, behavioural segmentation, and Power BI dashboard development, producing outputs that directly support retention, growth, upsell, and reactivation strategy.

---

## 2. Business Objective

To perform an end-to-end customer and transactional analysis that produces a structured segmentation model and interactive dashboard, enabling commercial teams to:

- Identify and prioritise high-value customer segments
- Quantify the reactivation opportunity within low-engagement groups
- Understand behavioural differences across regions, income groups, and demographic profiles
- Make faster, more targeted marketing and CRM decisions

---

## 3. Stakeholders & Decision Users

| Role | Primary Need | How This Project Supports Them |
|---|---|---|
| VP Marketing | Improve campaign targeting and offer relevance | Segments customers by loyalty, profile, income, and ordering behaviour |
| SVP Sales | Understand product demand and weaker-performing areas | Surfaces order timing, price bands, and department-level demand patterns |
| Customer Strategy / CRM | Improve communication relevance and retention | Identifies behavioural differences that support personalised outreach |

---

## 4. Key Business Questions

1. Which customer segments represent the highest retention and revenue risk?
2. Where are the largest untapped reactivation opportunities in the customer base?
3. How do ordering behaviour, reorder rates, and average income differ across priority tiers?
4. Which regions and income groups contain the highest-value customer concentrations?
5. What are the busiest ordering periods and how can those windows inform promotion strategy?
6. How is customer loyalty distributed across the base, and how do habits differ across segments?
7. What practical commercial actions should marketing and CRM teams prioritise?

---

## 5. Data Sources

| Source | Content | Use in Analysis |
|---|---|---|
| Retail eCommerce transactional dataset | Order, product, department, and transactional history | Core behavioural and product analysis |
| Supplemental customer dataset | Demographic and profile variables | Customer segmentation, regional and income comparisons |
| Project-created derived datasets | Wrangled, merged, and analysis-ready files | Feature engineering, grouped metrics, visualisation, and Power BI dashboard |

---

## 6. Analytical Scope

The project covers the full analytics pipeline from raw data to stakeholder dashboard:

- Data import, profiling, and initial quality assessment
- Data wrangling, restructuring, and standardisation
- Data quality validation — missing values, duplicates, type inconsistencies
- Multi-dataset merging and integration
- Feature engineering and customer flag creation
- Grouped aggregation and summary metric development
- Visual exploration and pattern identification
- Power BI dashboard development with interactive slicers and KPI cards
- Business findings and commercial recommendations

---

## 7. Analytical Workflow

| Stage | Description |
|---|---|
| Project setup | Established folder structure, notebook standards, and working environment |
| Data import & profiling | Loaded raw datasets, reviewed structure, dimensions, types, and summary statistics |
| Data wrangling | Renamed, recoded, subsetted, and standardised variables across datasets |
| Data quality validation | Identified and resolved missing values, duplicates, mixed types, and abnormal values |
| Data integration | Merged datasets using shared identifiers and validated join quality |
| Feature engineering | Created derived variables and flags for segmentation and behavioural profiling |
| Grouping & aggregation | Produced customer-level and department-level summary metrics |
| Visual exploration | Built charts to assess distributions, trends, outliers, and segment differences |
| Power BI dashboard | Built multi-page interactive dashboard from structured Python exports |
| Reporting & recommendations | Summarised findings and recommended commercial actions for stakeholders |

---

## 8. Segmentation Framework

Customers are classified into 11 strategic segments across four priority tiers:

| Priority Tier | Segments |
|---|---|
| High Priority | Protect: Highly Engaged Customers · Protect: High-Value Repeat Customers |
| Growth Priority | Grow: Active Family Shoppers · Grow: Affluent Active Customers · Grow: Active Value-Conscious Customers · Upsell: Frequent Low-Price Buyers · Cross-Sell: Broad Basket Explorers |
| Maintain | Maintain: Stable Mid-Value Customers · Premium: Higher Price Buyers |
| Reactivate | Reactivate: Low-Engagement Families · Reactivate: Low-Engagement Customers |

Segmentation is rule-based, combining order frequency, reorder rate, average spend, income band, and demographic profile variables.

---

## 9. Deliverables

- Structured project workspace with consistent folder and file naming
- Python notebooks documenting the end-to-end analytical workflow (9 notebooks)
- Cleaned and prepared data files for downstream analysis
- 8 structured CSV exports for Power BI consumption
- Derived segmentation variables and grouped summary outputs
- Exported visualisations supporting key findings
- Multi-page interactive Power BI dashboard (3 pages — pages 2 and 3 in development)
- Project brief and README documentation

---

## 10. Success Criteria

- Data is imported, validated, and organised in a reproducible project structure
- All datasets are cleaned, merged appropriately, and reduced to analysis-relevant variables
- Derived variables and segment flags are clearly connected to stated business questions
- Visualisations are well-labelled, interpretable, and support insight communication
- Power BI dashboard enables stakeholder-level drill-down across segment, region, and income dimensions
- Final outputs provide direct answers to business questions with practical recommendations

---

## 11. Data Governance & Ethics

Customer-level analysis is conducted with appropriate care where demographic and profile variables are used to define segments. The project avoids over-interpreting sensitive characteristics, documents assumptions clearly, and keeps stakeholder communication focused on responsible, proportionate use of data.

Any personally identifiable information present in source files is treated according to standard data handling practice and removed or protected where not essential to the analysis.

---

*Retail Customer Segmentation & Behaviour Dashboard — Project Brief v1.0*
*Elia Lanzuise · Data Analyst · Melbourne, VIC, Australia*
*elialanz.com · linkedin.com/in/elia-lanzuise*
