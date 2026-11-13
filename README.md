# DSA 2.0 Data Analysis Learning Journey

This is where i buit my first portfolio while learning at the Incubator Hub

## Overview
This repository documents my hands-on learning journey as an aspiring Data Analyst at **DSA 2.0 (Incubation Hub)**. It contains my practice exercises, cleaned datasets, and beginner projects built using Excel, SQL, and Power BI as I develop practical skills in turning raw data into clear insights. [Incubator Hub](https://app.theincubatorhub.org/)

## Central Business Question
Revenue has increased significantly from 2024 to 2025. Why hasn't profit increased at the same rate?

## Business Objectives
Management has commissioned you to build an automated, reliable Power BI Financial Reporting Solution that will:
  1. Produce a monthly interactive Profit & Loss (Income) Statement.
  2. Compare period-over-period financial performance (2024 vs 2025).
  3. Pinpoint the major operational and macroeconomic expense drivers behind profit margin compression.
  4. Evaluate branch-level and department-level cost efficiencies.
  5. Provide data-backed actionable strategic recommendations for executive leadership.

## Data Model Architecture (Star Schema)
The Power BI semantic model strictly follows a **Star Schema** design built around 5 core analytical tables:
- **`FactFinancialTransactions` (Central Fact Table):** Contains ~4,500 financial transaction records (revenues, COGS, and operating expenses).
- **`DimAccount` (Dimension):** Chart of Accounts defining account codes, names, and P&L categories.
- **`DimDepartment` (Dimension):** Corporate departments for departmental cost and performance tracking.
- **`DimBranch` (Dimension):** Geographical branches for regional profitability comparisons.
- **`DimCostCentre` (Dimension):** Functional cost pools for granular expense driver analysis.

*(Note: All Dimension tables connect to `FactFinancialTransactions` using One-to-Many (`1:*`) single-direction relationships.)*
