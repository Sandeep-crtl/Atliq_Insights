# 🚀 Business Insights 360 — Power BI Analytics Project

[![Power BI](https://img.shields.io/badge/Tool-Power%20BI-orange)]() [![DAX](https://img.shields.io/badge/Language-DAX-blue)]() [![PowerQuery](https://img.shields.io/badge/ETL-Power%20Query-yellowgreen)]()

A professional, end-to-end Power BI analytics solution built for AtliQ Hardware (fictional). The project transforms fragmented reports into a single, scalable dashboard suite that enables faster, data-driven decisions across Finance, Sales, Marketing, and Supply Chain.

---

## Table of Contents
- About
- Business Context
- Problem Statement
- Project Objective
- Data Sources
- Data Cleaning & Modeling
- Dashboard Scope
- Tools & Technologies
- Key Insights (summary)
- Strategic Recommendations
- Skills & Learnings
- How to review / run (notes)
- Limitations & Data Privacy
- Contact

---

## About
AtliQ Hardware is a fast-scaling electronics manufacturer. This repository documents the Power BI design, data model, and insights developed as part of the Business Insights 360 project.

---

## 🏢 Business Context
AtliQ sells PC accessories, printers, notebooks, desktops, and networking devices through multiple channels:
- Offline retail partners
- E-commerce platforms (global & regional)
- Sales segments: **Retailers**, **Direct Stores**, **Distributors**

Note: Customers are primarily retailers and distributors; end consumers purchase via those channels.

---

## 🚩 Problem Statement
As AtliQ scaled, analytics remained fragmented (Excel-driven), causing:
- Poor visibility into performance
- Slow, manual reporting cycles
- Suboptimal strategic decisions

Competitors adopted modern analytics and gained faster insights. The project addresses this gap with a scalable Power BI solution.

---

## 🎯 Project Objective
Design and deliver a unified Power BI dashboard suite that provides:
- Actionable KPIs for Finance, Sales, Marketing, and Supply Chain
- Executive-ready summary and trend analysis
- Customer, product, and region-level performance views
- A scalable, high-performance data model aligned to AtliQ’s fiscal calendar

---

## 🗄️ Data Sources
Data originates from a mix of SQL databases and Excel files.

Excel
- Operating Expenses.xlsx
- Targets (FY 2022).xlsx
- Market Share (PC division).xlsx

SQL Databases and tables
- gdb041
  - Fact tables: `fact_sales_monthly`, `fact_forecast_monthly`
  - Dimension tables: `dim_customer`, `dim_market`, `dim_product`
- gdb056
  - Tables: `freight_cost`, `gross_price`, `manufacturing_cost`, `pre_invoice_deductions`, `post_invoice_deductions`

Additional context
- Fiscal year: **September → August**
- Actual sales: **Sep 2017 – Dec 2021**
- Forecasts & targets include **FY 2022**
- Raw datasets are not included in the repo due to bootcamp constraints

---

## 🧹 Data Cleaning & Modeling (highlights)
- Standardized naming conventions and removed leading/trailing spaces
- Ensured consistent join keys across tables
- Created custom Date dimension aligned with AtliQ’s fiscal calendar
- Consolidated sales & forecasts into `fact_actual_estimates`
- Derived metrics:
  - Pre-invoice deductions
  - Post-invoice deductions
  - Net sales, Gross Margin, Net Profit %
- Disabled Load for intermediary tables to reduce model size and improve performance

---

## 📊 Dashboard Scope
Delivered Power BI report contains:
- Functional dashboards: Finance, Sales, Marketing, Supply Chain
- Executive Summary: high-level KPIs & trend lines
- Key Performers: top customers, products, and regions
- Additional panels:
  - Information panel (FAQs, future Excel export capability)
  - Support panel (feedback, issues, feature requests) — (integration subject to org approval)

---

## 🛠️ Tools & Technologies
- Data transformation: Power Query (M)
- Data modeling & measures: DAX
- Visualization & reporting: Power BI Desktop
- Source systems: SQL Server / Excel

---

## 📈 Key Insights (summary)
Financial
- Net sales grew multi-year (FY 2019 → FY 2022)
- Net Profit % declined after 2020 due to growth-stage operational & marketing investments

Market & Revenue
- APAC (led by India) is the largest revenue contributor
- Latin America is the smallest market
- Amazon is the top global customer; Nova declined after FY 2020

Product & Segment
- Notebook segment: highest revenue growth, lower profitability in FY 2022
- Desktop & Networking: underperformed in certain fiscal years
- USB flash drives: consistent decline in FY 2021–2022

Sales & Pricing
- Uniform discounting across products/customers reduced gross margins
- Several products had zero sales in FY 2022 → portfolio rationalization opportunities

Forecasting & Supply Chain
- Forecast accuracy dipped during COVID-19, recovered by FY 2022
- Inventory issues shifted from overstocking (FY 2019–2020) to shortages (FY 2021–2022)
- WFH demand increased strain on processors, keyboards, WiFi extenders

Regional & Competitive
- PC market share grew significantly FY 2021 → FY 2022
- India fastest-growing market
- North America: high revenue but lower market penetration
- UK & Germany: high marketing cost with uneven returns

---

## 📌 Strategic Recommendations
- Gradually optimize operational & marketing expenses as market share stabilizes
- Replace flat discounting with performance-based discount strategies
- Prioritize high-growth APAC markets (especially India)
- Reassess pricing and cost structure for the Notebook segment
- Reposition or upgrade declining product categories
- Improve customer-level forecasting to balance inventory
- Strengthen North America market penetration strategies
- Optimize marketing spend in high-cost, low-return regions
- Align inventory planning to peak months (Sep–Dec)

---

## 🧠 Skills & Learnings
- End-to-end BI project execution
- Cross-functional KPI design
- Advanced Power BI data modeling and DAX
- Scalable, executive-ready dashboard design
- Translating business problems into analytical solutions

---

## ▶️ How to review / run (notes)
- Open the Power BI Desktop report (.pbix) in Power BI Desktop (recommended latest stable)
- Connect to authorized SQL sources or swap in sample data files (not included)
- Refresh model after configuring data source credentials
- Test filter interactions and measure performance; optimize visuals if needed

---

## ⚠️ Limitations & Data Privacy
- Raw data excluded due to bootcamp constraints
- Some conclusions are sample-driven and should be validated with full production data before operational decisions

---

## Contributing
- Suggestions, issue reports, and feature requests are welcome. Please file issues in the repository or send feedback via the Support panel in the report.

---

## Contact
- Maintainer: Sandeep-crtl
- Project: AtliQ Insights (fictional dataset)

---
