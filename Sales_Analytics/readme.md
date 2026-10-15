# 📊 Sales Performance Analysis

### An End-to-End Business Analytics Project Using Excel, Python, SQL, and Power BI

## 📌 Project Overview

This project focuses on analyzing retail transaction data to understand sales performance, identify revenue trends, evaluate product and geographic performance, and generate actionable business insights.

Using the **Online Retail dataset** from the UCI Machine Learning Repository, this project applies data cleaning, exploratory data analysis, SQL querying, spreadsheet analysis, and business intelligence techniques to investigate retail sales performance.

The objective is to transform transaction-level data into meaningful insights that support business decision-making.

## 🎯 Business Problem

Retail businesses generate large volumes of transactional data, but raw transaction records do not automatically explain sales performance.

Management needs to understand which products and markets contribute most to revenue, how sales change over time, and whether cancellations, returns, or data-quality issues affect performance reporting.

This project addresses these questions through a structured, data-driven sales analytics workflow.

## 🎯 Project Objectives

- Analyze monthly and daily sales trends.
- Identify top-performing products by revenue and sales volume.
- Compare sales performance across countries.
- Calculate key sales performance indicators.
- Examine order volume and average order value.
- Investigate cancelled invoices, negative quantities, and other data-quality issues.
- Build visualizations and an interactive Power BI dashboard.
- Develop evidence-based business recommendations.

## 📂 Dataset Information

**Dataset:** Online Retail

**Source:** UCI Machine Learning Repository

**Publisher:** University of California, Irvine

**Dataset link:** https://archive.ics.uci.edu/dataset/352/online+retail

**Coverage:** December 2010 – December 2011

The dataset contains transactions from a UK-based online retail business.

### Dataset Attributes

| Column | Description |
|---|---|
| `InvoiceNo` | Invoice or transaction identifier |
| `StockCode` | Unique product identifier |
| `Description` | Product description |
| `Quantity` | Number of units purchased or recorded as returned |
| `InvoiceDate` | Date and time of the transaction |
| `UnitPrice` | Price per unit |
| `CustomerID` | Customer identifier |
| `Country` | Customer's country |

**Data considerations:**

- Some records contain missing customer identifiers or product descriptions.
- Invoice numbers beginning with `C` indicate cancellations.
- Negative quantities can represent returns or other adjustments.
- Duplicate-looking records require investigation before removal.
- Revenue calculations depend on clearly defined transaction inclusion rules.

The original dataset will be referenced through its official source. Only permitted and appropriately sized files or derived outputs will be published in this repository.

## 🛠️ Tools and Technologies

| Tool | Purpose |
|---|---|
| Microsoft Excel | Initial data inspection, formulas, PivotTables, and summary analysis |
| Python | Data cleaning, exploratory analysis, statistical summaries, and visualizations |
| pandas | Data manipulation and aggregation |
| NumPy | Numerical calculations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| SQL | Business queries, aggregations, rankings, and time-based analysis |
| Microsoft Power BI | Interactive dashboards and business reporting |
| Git and GitHub | Version control, project documentation, and portfolio publishing |

## 📈 Key Performance Indicators

The project will analyze the following metrics.

| KPI | Definition |
|---|---|
| Sales Revenue | Sum of eligible transaction-line revenue |
| Total Orders | Count of distinct eligible invoices |
| Units Sold | Sum of quantities for eligible sales lines |
| Average Order Value | Sales revenue divided by eligible order count |
| Monthly Revenue Growth | Percentage change in revenue from the preceding month |
| Country Revenue Contribution | Country revenue as a percentage of total revenue |
| Product Revenue Contribution | Product revenue as a percentage of total revenue |
| Cancellation Activity | Number and value of cancelled invoice records, analyzed separately |

**Revenue calculation:**

`Line Revenue = Quantity × UnitPrice`

For the initial sales-performance analysis, eligible sales lines will have positive quantities, positive unit prices, valid transaction dates, and invoice numbers that do not indicate cancellation.

This is an analytical reporting rule, not a complete accounting reconciliation of gross sales, returns, and net revenue. Returns and cancellations will be examined separately.

## 🔍 Analytical Workflow

### 1. Data Understanding and Validation

- Inspect dataset structure and data types.
- Identify missing values and duplicate-looking records.
- Examine cancellations, returns, and unusual prices or quantities.
- Document data-quality issues and analytical assumptions.

### 2. Excel Analysis

- Create calculated columns and basic summaries.
- Use PivotTables to analyze monthly sales and country performance.
- Identify leading products and transaction patterns.
- Build initial charts for exploratory analysis.

### 3. Python Analysis

- Load and prepare data using pandas.
- Validate missing values, duplicates, and data types.
- Calculate sales KPIs.
- Perform exploratory data analysis.
- Visualize sales trends, country performance, and product rankings.
- Export cleaned data and analytical summaries.

### 4. SQL Analysis

- Import the prepared analytical dataset into a relational database.
- Write queries to calculate overall sales KPIs.
- Analyze monthly revenue and growth.
- Rank countries and products by revenue.
- Validate SQL outputs against Python and Excel results.

### 5. Power BI Dashboard

- Develop an appropriate data model.
- Create KPI measures using DAX.
- Build interactive charts, filters, and drill-downs.
- Present sales trends, product performance, and geographic performance.
- Highlight important business findings.

### 6. Business Interpretation

- Summarize findings supported by the analysis.
- Identify performance patterns and potential issues.
- Develop recommendations relevant to retail management.
- Document limitations and opportunities for further analysis.

## 📊 Business Questions

This project aims to answer the following questions:

1. Which months generated the highest and lowest sales revenue?
2. How does sales performance change over time?
3. Which countries contribute most to total sales?
4. Which products generate the highest revenue and sales volume?
5. How do order volume and average order value vary over time?
6. How significant are cancellations and negative-quantity transactions?
7. What data-quality limitations should management consider?
8. What actions could help the business improve sales performance and reporting?

## 📁 Repository Structure

```text
sales-performance-analysis/
│
├── README.md
│
├── data/
│   └── README.md
│
├── excel/
│   └── sales_exploration.xlsx
│
├── python/
│   └── sales_analysis.ipynb
│
├── sql/
│   └── sales_analysis.sql
│
├── powerbi/
│   └── sales_dashboard.pbix
│
├── outputs/
│   ├── monthly_sales_summary.csv
│   └── country_sales_summary.csv
│
└── images/
    ├── monthly_sales_trend.png
    └── dashboard_preview.png
```

*This structure represents the intended organization. Files will be added as each stage is completed.*

## 📌 Expected Deliverables

- Excel workbook containing data exploration and PivotTables.
- Python notebook documenting data preparation and exploratory analysis.
- SQL scripts answering key business questions.
- Power BI dashboard presenting sales performance.
- Visualizations and analytical summary tables.
- Business findings and recommendations.
- Documentation of data sources, assumptions, and limitations.

## 💡 Business Applications

The analytical approach used in this project can support retail organizations in:

- Monitoring sales performance across periods and markets.
- Identifying high-performing products and geographic markets.
- Understanding changes in order volume and average order value.
- Improving the reliability of sales reporting.
- Investigating cancellations and returns.
- Supporting data-driven commercial planning.

These are potential applications of the analysis, not claims of measured business improvements.

## ⚠️ Limitations

- The dataset covers a historical period and may not represent current retail market conditions.
- The available fields do not provide a complete view of operating expenses, marketing expenditure, or product costs.
- Sales revenue should not be interpreted as profit.
- Missing customer identifiers limit customer-level analysis.
- Observational transaction data can reveal patterns but does not independently establish causality.
- Any assumptions, exclusions, and transformations will be documented as the analysis progresses.

## 🚀 Project Status

**Current stage:** Data exploration and project development.

Planned milestones:

- [ ] Inspect and validate the dataset.
- [ ] Complete initial Excel analysis.
- [ ] Perform Python data cleaning and exploratory analysis.
- [ ] Develop and validate SQL queries.
- [ ] Build the Power BI dashboard.
- [ ] Document findings and business recommendations.
- [ ] Publish the completed project on GitHub.

## 👨‍💻 Author

**MBA Student | Business Analytics | Digital Marketing**

Interested in applying data analytics, business intelligence, and data-driven methods to practical business challenges.

- **LinkedIn:** [Add your LinkedIn profile URL]

---

## 📚 Data Source and Attribution

Chen, D. (2015). *Online Retail* [Dataset]. UCI Machine Learning Repository, University of California, Irvine.

Dataset URL: https://archive.ics.uci.edu/dataset/352/online+retail

The dataset is distributed under the Creative Commons Attribution 4.0 International license (CC BY 4.0). Refer to the official dataset page for the source details and license terms.

---

**Turning Transaction Data into Business Insights.**
