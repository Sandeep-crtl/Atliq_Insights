# 🚀 Bank Loan Analysis — Power BI Analytics Project

[![Power BI](https://img.shields.io/badge/Tool-Power%20BI-orange)]()
[![DAX](https://img.shields.io/badge/Language-DAX-blue)]()
[![PowerQuery](https://img.shields.io/badge/ETL-Power%20Query-yellowgreen)]()

A professional, end-to-end **Bank Loan Analytics** solution built using Power BI.  
This project consolidates loan application, funding, risk, and profitability data into a single, interactive dashboard suite that enables **data-driven credit, risk, and business decisions**.

---

## Table of Contents
- About
- Business Context
- Problem Statement
- Project Objective
- Data Sources
- Data Cleaning & Modeling
- Dashboard Scope
- KPI Framework
- Tools & Technologies
- Key Insights (Summary)
- Strategic Recommendations
- Skills & Learnings
- How to Review / Run
- Limitations & Data Privacy
- Contact

---

## About
This repository documents the design, data model, DAX logic, and insights developed for a **Bank Loan Analysis Power BI Dashboard**.  
The project focuses on **loan performance, borrower behavior, credit risk, and profitability**, using structured KPIs and time intelligence (MTD, PMTD, MoM).

---

## 🏦 Business Context
The bank provides loans across multiple purposes, borrower profiles, and credit grades.  
As loan volume grows, decision-makers need:
- Clear visibility into loan demand and funding
- Early identification of credit risk
- Understanding of profitability versus risk
- Consistent reporting across time

This dashboard addresses these needs through a unified analytics layer.

---

## 🚩 Problem Statement
Loan reporting was fragmented and metric-heavy without clear narratives, resulting in:
- Difficulty tracking month-to-date performance
- Poor visibility into default and risk concentration
- Limited understanding of profitability drivers
- Manual effort to compare trends across months

A centralized Power BI solution was required to **standardize KPIs**, **enable trend analysis**, and **support faster decisions**.

---

## 🎯 Project Objective
Design and deliver a Power BI dashboard that:
- Tracks loan demand, funding, and repayments
- Monitors credit risk using defensible metrics
- Measures profitability and unit economics
- Supports MTD, PMTD, and MoM analysis
- Separates business, risk, and profit narratives clearly

---

## 🗄️ Data Sources
The dataset contains historical loan-level records including:
- Loan ID
- Application Date
- Loan Amount & Funded Amount
- Total Payment Received
- Loan Purpose
- Loan Grade
- Employment Length
- Debt-to-Income Ratio (DTI)
- Interest Rate
- Loan Status (Good / Bad)

A dedicated **Date Table** is used to enable time intelligence.

---

## 🧹 Data Cleaning & Modeling
Key steps performed:
- Standardized column names and data types
- Removed duplicates and invalid records
- Created a Date dimension for time-based analysis
- Defined relationships between fact and dimension tables
- Built reusable base measures for consistency
- Optimized model by avoiding redundant calculations

---

## 📊 Dashboard Scope

### 1️⃣ Summary Page
**Purpose:** Executive snapshot.

**KPIs:**
- Total Loan Applications
- Total Funded Amount
- Total Amount Received
- Average Interest Rate

---

### 2️⃣ Overview Page
**Purpose:** Portfolio health and momentum.

**KPIs:**
- Total Loan Applications
- Total Funded Amount
- Approval Rate (%)
- MoM Loan Application Growth (%)

---

### 3️⃣ Details Page
**Purpose:** Loan composition and borrower behavior.

**KPIs:**
- Average Loan Amount
- Applications per Borrower
- Top Loan Purpose Share (%)
- Stable Employment Share (%)

---

### 4️⃣ Risk Page
**Purpose:** Credit quality and exposure.

**KPIs:**
- Bad Loan % (Application-based)
- Bad Loan Exposure (Funded Amount)
- Average DTI
- High-Risk Grade Exposure (%)

---

### 5️⃣ Profit Page
**Purpose:** Financial return vs risk.

**KPIs:**
- Net Profit
- Profit Margin (%)
- Average Interest Rate
- Profit per Loan

---

## 📐 KPI Framework
The dashboard follows strict KPI design rules:
- Ratios are calculated from aggregated values (not averaged ratios)
- MTD and PMTD are calculated at numerator and denominator levels
- MoM % is used only for absolute metrics
- Percentage-point change is used for ratio KPIs
- Risk and profit metrics are never mixed without context

---

## ⏱️ Time Intelligence
- **MTD (Month-to-Date):** Current month performance up to selected date
- **PMTD (Previous Month-to-Date):** Same period comparison
- **MoM (Month-over-Month):** Trend analysis using correct mathematical logic

---

## 🛠️ Tools & Technologies
- Power BI Desktop
- Power Query (ETL)
- DAX (Measures & Time Intelligence)
- Excel / CSV (Data Source)
- GitHub (Version Control)

---

## 📈 Key Insights (Summary)
- Loan demand shows clear monthly seasonality
- Certain loan purposes dominate application volume
- Higher loan grades contribute disproportionately to risk
- Rising DTI often precedes increases in bad loans
- Profitability varies significantly by grade and purpose
- High volume does not always translate into high profit

---

## 📌 Strategic Recommendations
- Monitor approval rate trends to balance growth and risk
- Limit exposure to high-risk grades during growth phases
- Adjust pricing where interest does not compensate for default risk
- Focus on stable employment segments for portfolio quality
- Track profitability at a per-loan level, not just totals

---

## 🧠 Skills & Learnings
- Financial and credit risk analysis
- KPI design aligned to business questions
- Advanced DAX for time intelligence
- Data modeling best practices
- Dashboard storytelling for decision-makers

---

## ▶️ How to Review / Run
- Open the `.pbix` file using Power BI Desktop
- Ensure Date Table is properly related
- Refresh data after configuring sources
- Use slicers to test MTD and MoM behavior
- Validate KPI behavior across pages

---

## ⚠️ Limitations & Data Privacy
- Dataset is for learning and demonstration purposes
- Insights should be validated with real production data
- No personally identifiable information (PII) is included

---

## Contact
- Maintainer: **Sandeep-crtl**
- Project: **Bank Loan Analysis Dashboard**
- Platform: **Power BI**

---

## 📸 Dashboard Preview
![Dashboard Screenshot](./screenshots/bank_loan_dashboard.png)
