**Business Insights 360 – Power BI Analytics Project**
🏢 Business Context

AtliQ Hardware (fictional company) is a fast-scaling electronics manufacturer offering products such as PC accessories, printers, notebooks, desktops, and networking devices. Over the last few years, the company has expanded its footprint across major global regions including APAC, North America, Latin America, and the European Union.

AtliQ sells its products through multiple routes:

Offline retail partners (electronics stores and large retailers)

E-commerce platforms (global and regional online marketplaces)

Sales operations are further segmented into:

Retailers – third-party sellers (online & offline)

Direct Stores – AtliQ-owned branded outlets

Distributors – used in regulated markets such as China and South Korea

Note: AtliQ’s customers are retailers and distributors, while end consumers purchase products through these channels.

🚩 Business Problem

As AtliQ expanded rapidly, its analytics ecosystem failed to scale at the same pace. Critical business decisions were driven by fragmented Excel reports, resulting in poor visibility, delayed insights, and costly missteps—most notably during the company’s expansion into Latin America.

Meanwhile, competitors adopted advanced analytics platforms, gaining faster insights and sharper decision-making capabilities. To address this gap and establish a scalable, data-driven culture, AtliQ initiated a centralized analytics transformation project.

🎯 Project Objective

The objective of this project is to design a comprehensive Power BI dashboard suite that delivers actionable insights across key business functions:

Finance

Sales

Marketing

Supply Chain

Executive & Key Performers View

The solution improves transparency, accelerates decision-making, and supports strategic planning across the organization.

🗄️ Data Sources

The analysis is based on a combination of SQL databases and Excel files.

Excel Files

Operating Expenses

Targets (FY 2022 only)

Market Share (Personal Computer division only)

SQL Databases

gdb041

Fact Tables

fact_sales_monthly

fact_forecast_monthly

Dimension Tables

dim_customer

dim_market

dim_product

gdb056

freight_cost

gross_price

manufacturing_cost

pre_invoice_deductions

post_invoice_deductions

Additional Context

Fiscal Year: September to August

Actual sales data: Sep 2017 – Dec 2021

Forecasts and targets include FY 2022

Raw datasets cannot be shared due to bootcamp constraints

🧹 Data Cleaning & Modeling
Data Standardization

Removed leading and trailing spaces

Standardized naming conventions

Ensured consistent join keys across tables

Data Modeling & Optimization

Created a custom Date dimension aligned with AtliQ’s fiscal calendar

Consolidated sales and forecast data into a unified table: fact_actual_estimates

Derived calculated metrics including:

Pre-invoice deductions

Post-invoice deductions

Net sales and profitability

Disabled load for intermediary tables to reduce model size and improve performance

📊 Dashboard Scope

The Power BI report includes:

Functional dashboards for Finance, Sales, Marketing, and Supply Chain

Executive summary with high-level KPIs

Key performers analysis by product, customer, and region

Additional Panels

Information Panel – FAQs and future provision for Excel exports

Support Panel – feedback, issue reporting, feature requests, and contingency planning
(integration subject to organizational approval)

🛠️ Tools & Technologies

Data Transformation: Power Query

Data Modeling & Analysis: DAX

Visualization & Reporting: Power BI

📈 Key Insights
Financial Performance

Net sales showed strong multi-year growth from FY 2019 to FY 2022

Net Profit % declined post-2020 due to heavy operational and marketing investments typical of growth-stage companies

Market & Revenue Trends

APAC remained the largest revenue contributor, led by India

Latin America remained the smallest market

Amazon was the top global customer, while Nova showed declining contribution after FY 2020

Product & Segment Analysis

Notebook segment achieved the highest revenue growth but suffered declining profitability in FY 2022

Desktop and Networking segments underperformed in different fiscal years

USB flash drives consistently declined in FY 2021 and FY 2022

Sales & Customer Behavior

Uniform discounting across customers and products significantly reduced Gross Margin %

Several products recorded zero sales in FY 2022, indicating portfolio rationalization opportunities

Forecasting & Supply Chain

Forecast accuracy dropped during COVID-19 but recovered steadily by FY 2022

Inventory challenges shifted from overstocking (FY 2019–2020) to shortages (FY 2021–2022)

Work-from-home demand strained supply for processors, keyboards, and WiFi extenders

Competitive & Regional Insights

PC market share increased significantly from FY 2021 to FY 2022

India emerged as the fastest-growing market

North America generated high revenue but showed relatively low market penetration

UK and Germany incurred high marketing costs with uneven revenue returns

📌 Strategic Recommendations

Gradually optimize operational and marketing expenses as market share stabilizes

Replace flat discounting with performance-based discount strategies

Increase focus on high-growth APAC markets, particularly India

Reassess pricing and cost structure of the Notebook segment

Address declining product categories through repositioning or upgrades

Improve customer-level forecasting to reduce inventory imbalance

Strengthen market penetration strategies in North America

Optimize marketing spend in high-cost, low-return regions

Align inventory planning with peak sales months (September–December)

🧠 Skills & Learnings

End-to-end BI project execution

Strong understanding of cross-functional business KPIs

Advanced Power BI data modeling and DAX

Designing scalable, executive-ready dashboards

Translating business problems into analytical solutions
