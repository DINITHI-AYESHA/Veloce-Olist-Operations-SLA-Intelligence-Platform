# RetailPulse – Multi-Branch Sales & Inventory Analytics Dashboard

An interactive Business Intelligence solution built in Power BI to monitor multi-branch retail performance, evaluate product margins, and detect stockout risks.

---

## 📌 Project Overview
RetailPulse centralizes fragmented transactional and stock records across multiple retail branches into a unified dashboard. It helps store managers and supply chain teams make data-backed decisions around pricing, category performance, and inventory replenishment.

### Key Objectives
* **Sales Performance:** Track overall revenue, sales volume, and regional growth across retail outlets.
* **Margin Analysis:** Evaluate product- and branch-level profitability using Gross Profit Margin metrics.
* **Inventory Optimization:** Monitor inventory turnover and flag high-risk stockout thresholds early to prevent supply disruptions.

---

## 🛠️ Tools & Technologies
* **Business Intelligence:** Power BI Desktop
* **Data Transformation:** Power Query (ETL, schema normalization, data cleaning)
* **Calculations & Analytics:** DAX (Data Analysis Expressions)
* **Data Source & Querying:** SQL, Microsoft Excel
* **Project Management:** Trello

---

## 🏗️ Data Architecture & Modeling
* **Data Modeling:** Implemented a star schema with separated fact tables (Sales Transactions, Inventory Snapshots) and dimension tables (Store Locations, Products, Calendar/Dates).
* **ETL Workflow:** Cleansed raw data, normalized inconsistent branch labels, handled null values, and established strict relationship cardinalities (1-to-many) in Power Query.

---

## 📊 Dashboard Features & Views
* **Executive Summary:** High-level KPI cards covering Total Revenue, Gross Profit, and Average Inventory Turnover.
* **Store & Regional Drill-Down:** Dynamic views enabling branch-by-branch performance and margin comparisons.
* **Category & Seasonal Trends:** Visual breakdowns of best-performing product lines over monthly and seasonal periods.
* **Interactive Slicers:** Dynamic cross-filtering by date range, branch location, and product category.

---

## 📂 Repository Structure
```text
├── data/
│   ├── raw/                 # Raw transactional and inventory source files
│   └── processed/           # Cleaned datasets and lookup dimensions
├── sql/
│   └── schema_and_queries/  # SQL extraction and staging scripts
├── dashboard/
│   └── RetailPulse.pbix     # Power BI report and data model
├── docs/
│   └── screenshots/         # Dashboard previews and schema diagrams
└── README.md
