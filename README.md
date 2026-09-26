# Veloce: Olist Marketplace Operations & Logistics Intelligence

[![Power BI](https://img.shields.io/badge/Power_BI-Desktop-F2C811?logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Status](https://img.shields.io/badge/Project_Status-In_Development-blue)](#)
[![Data Source](https://img.shields.io/badge/Dataset-Kaggle_Olist-20BEFF?logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

An enterprise Business Intelligence and Operations Analytics portfolio project delivering end-to-end operational visibility into Brazilian e-commerce logistics, delivery Service Level Agreement (SLA) breaches, and marketplace growth dynamics.

---

## 📌 Business Problem & Executive Context
Olist operates a nationwide marketplace connecting independent small businesses across Brazil to national retail channels. Operating across Brazil's complex interstate logistics network creates three primary operational vulnerabilities:

1. **Regional SLA Variance:** Unpredictable carrier lead times lead to unmonitored customer delivery delays and platform dissatisfaction.
2. **Fulfillment Lead Time Lag:** Bottlenecks between merchant order approval and carrier dispatch compound shipping risks.
3. **Freight Economics Disparity:** High freight-to-price ratios in distant states suppress conversion and reduce net order profitability.

**Objective:** Design an interactive, executive-grade Power BI dashboard backed by structured Business Analysis deliverables (BRD, KPI Dictionary, Agile Stories) to monitor fulfillment health, enforce carrier SLAs, and optimize regional revenue distribution.

---

## 🏗️ Repository Architecture

```text
├── docs/                     # Formal BA Documentation
│   ├── BRD.md                # Business Requirements Document
│   ├── KPI_DICTIONARY.md     # Business metric definitions & calculation logic
│   └── TRELLO_BACKLOG.md     # Agile user stories & Gherkin acceptance criteria
├── data/
│   ├── raw/                  # Kaggle CSV extracts (.gitignore tracked)
│   └── data_dictionary.md    # Raw data grain, data types, and integrity notes
├── pbix/                     # Power BI report files (.pbix)
├── assets/                   # Architecture diagrams, wireframes, and UI screenshots
├── .gitignore                # Excludes large CSVs and Power BI temp files
└── README.md                 # Project executive summary
