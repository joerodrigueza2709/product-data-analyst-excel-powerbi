# 📱 Mobile App UA Investment Analysis

## 📌 Overview
This project analyzes mobile app marketing performance to identify which applications should receive additional **User Acquisition (UA) investment**.

The analysis evaluates **acquisition efficiency, revenue recovery, long-term value, and user retention**, simulating a real-world **product analytics workflow**.

---

## 🎯 Business Objective
Marketing teams must decide how to allocate limited user acquisition budgets across multiple apps.

Investing in inefficient campaigns reduces ROI and limits growth potential.

👉 **Key Question:**  
**Which mobile apps should receive additional UA investment?**

---

## 🛠️ Tools & Technologies
- **Excel** – Data cleaning, feature engineering, and analysis  
- **Power BI** – Dashboard visualization  

---

## 🗂️ Dataset
The dataset is a **simulated marketing performance dataset** containing:

- 25 mobile applications  
- 3 platforms (iOS, Android, Amazon)  
- 200+ countries  

Each row represents:

👉 **App × Platform × Country performance**

---

### 📥 Raw Dataset
[Download Raw Dataset](data/raw/raw_app_performance_data.csv)

**Includes real-world inconsistencies such as:**
- Inconsistent column names  
- Mixed currency formats  
- Spacing and labeling issues  

---

### 📥 Cleaned Dataset
[Download Cleaned Dataset](data/processed/cleaned_app_performance_data.csv)

Contains:
- Standardized fields  
- Cleaned numeric formats  
- Engineered metrics ready for analysis  

---

## 🔄 Data Pipeline


The analytical workflow for this project follows the pipeline below:

Raw Dataset  
↓  
Excel Data Cleaning  
↓  
Feature Engineering  
↓  
Excel Analysis  
↓  
Power BI Dashboard  
↓  
Investment Decision Framework

---

## 🧹 Data Preparation (Excel)

The raw dataset required significant cleaning before analysis:

- Removed duplicate records  
- Standardized country names  
- Cleaned currency formatting  
- Converted numeric fields  
- Standardized platform labels  
- Validated revenue and spend values  
- Harmonized column naming  

---

## ⚙️ Feature Engineering

Key marketing metrics were created:

| Metric        | Formula                     | Business Meaning              |
|--------------|----------------------------|------------------------------|
| CAC          | Ad Spend / Installs        | Cost to acquire one user     |
| ROAS 30d     | Revenue 30d / Ad Spend     | Short-term return on ad spend|
| LTV 90d      | Revenue 90d / Installs     | Long-term user value         |
| Retention 30d| Active Users 30d / Installs| User engagement              |
| LTV:CAC      | LTV / CAC                  | Unit economics strength      |

---

## 🧠 Investment Decision Framework

Apps were considered eligible for additional UA investment if:

- **ROAS > 1**  
- **LTV > CAC**

---

### 🏆 Investment Score

Eligible apps were ranked using a weighted scoring model:

- ROAS 30d → **50%**  
- LTV 90d → **30%**  
- Retention 30d → **20%**

This simulates real-world marketing prioritization.

![Investment Framework](https://github.com/user-attachments/assets/19b039fc-2178-4853-bd09-a6e5696572c4)

---

## 📊 Excel Analysis

📥 [Download Excel Workbook](excel_analysis/mobile_app_ua_investment_analysis.xlsx)

Excel was used to:

- Clean and validate the dataset  
- Engineer marketing metrics  
- Build pivot tables  
- Calculate investment scores  
- Identify top-performing apps  

![Excel Overview](https://github.com/user-attachments/assets/ca2927cb-bbe7-4a84-b8ab-bdc07f8dd16d)

---

## 📊 Power BI Dashboard

📥 [Download Power BI Dashboard](powerbi_dashboard/mobile_app_ua_investment_dashboards.pbix)

The dashboard visualizes marketing performance and highlights top investment opportunities.

**Includes:**
- Portfolio KPI overview  
- Top apps for UA investment  
- LTV:CAC analysis  
- ROAS vs CAC scatter analysis  
- Profitability visualization  

![Dashboard](https://github.com/user-attachments/assets/cd0e00dd-3423-4a44-94bd-8f441b1987e5)

---

## 📈 Key Insights

- Several apps demonstrate **strong marketing efficiency** across multiple metrics  
- High-performing apps show:
  - Strong **ROAS (short-term revenue recovery)**  
  - High **LTV (long-term value)**  
  - Healthy **retention rates**  
  - Favorable **LTV:CAC ratios**  

- Apps such as **Ninja Numbers** and **Hero Helper HQ** stand out as top investment candidates  

---

## 💡 Business Recommendations

- **Increase UA investment in top-performing apps**  
  Apps like *Ninja Numbers* and *Hero Helper HQ* show strong unit economics and should be prioritized  

- **Scale profitable acquisition channels**  
  Focus on campaigns with high ROAS and LTV  

- **Monitor underperforming apps**  
  Apps with weak LTV:CAC ratios should be optimized before additional spend  

- **Leverage retention insights**  
  Prioritize apps with strong engagement to maximize long-term returns  

