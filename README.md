# product-data-analyst-excel-powerbi
#Mobile App UA Investment Analysis

#Project Overview:
This project analyzes mobile app marketing performance to determine which apps deserve additional user acquisition (UA) investment.
The analysis evaluates acquisition efficiency, short-term revenue recovery, long-term user value, and user retention using key marketing metrics.
The goal is to simulate a real-world product analytics workflow and demonstrate how data analysts support marketing investment decisions.

Tools used:
Excel
Power BI

Business Problem:
Marketing teams must decide how to allocate limited user acquisition budgets across multiple mobile apps.
Investing in the wrong campaigns can significantly reduce marketing efficiency and return on investment.
This project answers the following question:
Which mobile apps should receive additional user acquisition investment?

Dataset:
The dataset is a simulated marketing performance dataset containing:
25 mobile applications
3 platforms (iOS, Android, Amazon)
200+ countries
Each row represents performance metrics for a specific:
App × Platform × Country

Two datasets are included:

Raw Dataset:
Located in: data/raw/raw_app_performance_data.csv
This dataset intentionally contains inconsistencies such as:
inconsistent column names
mixed currency formatting
spacing and labeling issues
These simulate common real-world marketing export data.

Cleaned Dataset:
Located in:data/cleaned/cleaned_app_performance_data.csv
The cleaned dataset contains standardized fields and engineered metrics ready for analysis.

Data Preparation
The raw dataset required preparation before analysis.
The following steps were performed in Excel:
Removed duplicate records
Standardized country naming conventions
Cleaned inconsistent currency formats
Converted numeric fields to proper numeric types
Ensured consistent platform labels
Verified that revenue and spend values were positive
Standardized column naming conventions

Feature Engineering:
Several analytical metrics were created to evaluate marketing performance.
| Metric        | Formula                     | Business Meaning              |
| ------------- | --------------------------- | ----------------------------- |
| CAC           | Ad Spend / Installs         | Cost to acquire one user      |
| ROAS 30d      | Revenue 30d / Ad Spend      | Short-term return on ad spend |
| LTV 90d       | Revenue 90d / Installs      | Long-term user value          |
| Retention 30d | Active Users 30d / Installs | User engagement               |
| LTV:CAC       | LTV / CAC                   | Unit economics strength       |

Investment Decision Framework:
Apps were considered eligible for additional user acquisition investment if:
ROAS > 1
AND
LTV > CAC
Eligible apps were then ranked using a weighted Investment Score:
ROAS 30d → 50%
LTV 90d → 30%
Retention 30d → 20%
This framework simulates how marketing teams evaluate campaign efficiency and prioritize investment opportunities.

Excel Analysis:
Excel was used to:
Clean and validate the dataset
Engineer marketing metrics
Build pivot tables for aggregated performance
Calculate the investment score
Identify the top apps for UA investment
The Excel workbook is located in: excel_analysis/mobile_app_ua_investment_analysis.xlsx

Power BI Dashboard:
A Power BI dashboard was created to visualize campaign performance and highlight the most promising apps for additional investment.
The dashboard includes:
Portfolio KPI overview
Top apps for UA investment
LTV:CAC analysis
ROAS vs CAC scatter analysis
LTV vs CAC profitability visualization
Dashboard file: powerbi_dashboard/mobile_app_ua_investment_dashboards.pbix

<img width="3436" height="1398" alt="Final Screen" src="https://github.com/user-attachments/assets/aeadf531-699e-4e96-ab22-7e44c0c6933e" />

Key Insights:
The analysis identified several apps that demonstrate strong marketing efficiency based on:
high ROAS
strong long-term LTV
healthy retention
favorable LTV:CAC ratios
These apps represent the best candidates for additional user acquisition investment.

Tools Used:
Excel
Power BI
