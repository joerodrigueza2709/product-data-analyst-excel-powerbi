# Mobile App UA Investment Analysis

## Project Overview:
This project analyzes mobile app marketing performance to determine which apps deserve additional user acquisition (UA) investment.

The analysis evaluates acquisition efficiency, short-term revenue recovery, long-term user value, and user retention using key marketing metrics.

The goal is to simulate a real-world product analytics workflow and demonstrate how data analysts support marketing investment decisions.

## Tools used:
Excel

Power BI

## Business Problem:
Marketing teams must decide how to allocate limited user acquisition budgets across multiple mobile apps.

Investing in the wrong campaigns can significantly reduce marketing efficiency and return on investment.

**This project answers the following question:**

**Which mobile apps should receive additional user acquisition investment?**

## Dataset:
**The dataset is a simulated marketing performance dataset containing:**

25 mobile applications

3 platforms (iOS, Android, Amazon)

200+ countries

**Each row represents performance metrics for a specific:**

App × Platform × Country



**Two datasets are included:**


**Raw Dataset:**

📥 **Download the Raw Dataset:**  
[raw_app_performance_data.csv](data/raw/raw_app_performance_data.csv)

**This dataset intentionally contains inconsistencies such as:**

inconsistent column names

mixed currency formatting

spacing and labeling issues

These simulate common real-world marketing export data.


**Cleaned Dataset:**

📥 **Download the Cleaned Dataset:**  
[cleaned_app_performance_data.csv](data/processed/cleaned_app_performance_data.csv)

The cleaned dataset contains standardized fields and engineered metrics ready for analysis.

## Data Preparation
The raw dataset required preparation before analysis.

**The following steps were performed in Excel:**

Removed duplicate records

Standardized country naming conventions

Cleaned inconsistent currency formats

Converted numeric fields to proper numeric types

Ensured consistent platform labels

Verified that revenue and spend values were positive

Standardized column naming conventions

## Feature Engineering:
Several analytical metrics were created to evaluate marketing performance.

| Metric        | Formula                     | Business Meaning              |
| ------------- | --------------------------- | ----------------------------- |
| CAC           | Ad Spend / Installs         | Cost to acquire one user      |
| ROAS 30d      | Revenue 30d / Ad Spend      | Short-term return on ad spend |
| LTV 90d       | Revenue 90d / Installs      | Long-term user value          |
| Retention 30d | Active Users 30d / Installs | User engagement               |
| LTV:CAC       | LTV / CAC                   | Unit economics strength       |

## Investment Decision Framework:
**Apps were considered eligible for additional user acquisition investment if:**
ROAS > 1
AND
LTV > CAC

**Eligible apps were then ranked using a weighted Investment Score:**

ROAS 30d → 50%

LTV 90d → 30%

Retention 30d → 20%

This framework simulates how marketing teams evaluate campaign efficiency and prioritize investment opportunities.

<img width="2629" height="390" alt="Eligible_for_UA_Campaign" src="https://github.com/user-attachments/assets/19b039fc-2178-4853-bd09-a6e5696572c4" />

## Excel Analysis:

📥 **Download the Excel Analysis Workbook:**  
[mobile_app_ua_investment_analysis.xlsx](excel_analysis/mobile_app_ua_investment_analysis.xlsx)

Excel was used to:

Clean and validate the dataset

Engineer marketing metrics

Build pivot tables for aggregated performance

Calculate the investment score

Identify the top apps for UA investment

<img width="1530" height="1072" alt="excel_overview" src="https://github.com/user-attachments/assets/ca2927cb-bbe7-4a84-b8ab-bdc07f8dd16d" />

## Power BI Dashboard:

📥 **Download the Power BI Dashboard:**  
[mobile_app_ua_investment_dashboard.pbix](powerbi_dashboard/mobile_app_ua_investment_dashboards.pbix)

A Power BI dashboard was created to visualize campaign performance and highlight the most promising apps for additional investment.

**The dashboard includes:**


Portfolio KPI overview

Top apps for UA investment

LTV:CAC analysis

ROAS vs CAC scatter analysis

LTV vs CAC profitability visualization

<img width="2050" height="1148" alt="dashboard_overview" src="https://github.com/user-attachments/assets/cd0e00dd-3423-4a44-94bd-8f441b1987e5" />

## Key Insights:
**The analysis identified several apps that demonstrate strong marketing efficiency based on:**

• High ROAS indicating strong short-term revenue recovery

• Strong long-term LTV suggesting sustainable user value

• Healthy retention levels reflecting strong user engagement

• Favorable LTV:CAC ratios demonstrating profitable acquisition

**Apps such as Ninja Numbers and Hero Helper HQ showed particularly strong unit economics and represent the best candidates for additional UA investment.**

