📉 Customer Retention & Churn Analysis
Future Interns — Data Science & Analytics Task 2 (2026)
Prepared by: Kamohelo Mabena
---
📌 Project Overview
This project presents a customer retention and churn analysis for a telecommunications company. Using 7,043 customer records, the analysis identifies why customers leave, which segments are most at risk, and what actions the business can take to improve retention and protect revenue.
---
🎯 Business Questions Answered
What is the overall churn rate and how does it compare to industry benchmarks?
Which contract types have the highest churn risk?
When in the customer lifecycle is churn most likely to occur?
Which internet service type has the highest churn rate and why?
What are the strongest drivers of customer retention?
What actions will have the highest impact on reducing churn?
---
📊 Dashboard Preview
![Dashboard Screenshot](./churn_dashboard_screenshot.png)
---
📁 Files in This Repository
File	Description
`WA_Fn-UseC_-Telco-Customer-Churn.csv`	Raw dataset from Kaggle
`Telco_Churn_Cleaned.xlsx`	Cleaned dataset with calculated columns
`Churn_Dashboard.pbix`	Power BI dashboard file
`Task2_Churn_Analysis_Report.docx`	Full written insights and recommendations
`churn_dashboard_screenshot.png`	Screenshot of the final Power BI dashboard
---
🛠️ Tools Used
Microsoft Excel — Data cleaning and preparation
Power BI Desktop — Dashboard and visualisation
DAX — Calculated columns and measures
Power Query — Data transformation
---
📊 Dashboard Visuals
4 KPI Cards — Total Customers (7,043), Churned (1,869), Churn Rate (26.5%), Avg Tenure (32 months)
Churn by Contract Type (Bar Chart) — Month-to-month vs One Year vs Two Year
Churn by Tenure (Line Chart) — How churn risk changes over customer lifetime
Churn by Internet Service (Donut Chart) — Fibre Optic vs DSL vs No Internet
Churn by Payment Method (Bar Chart) — Electronic check vs Auto-pay methods
Retention Drivers Summary — Key factors that keep customers loyal
Interactive Slicers — Filter by Contract Type, Internet Service, Gender
---
🔍 Key Insights
Overall churn rate is 26.5% — significantly above the 15–20% industry benchmark
Month-to-month customers churn at 42.7% — 15x higher than two-year contract customers (2.8%)
47.4% of customers churn within their first 12 months — the first year is the highest-risk period
Fibre Optic customers churn at 41.9% — double the DSL rate despite being the premium service
Electronic check payment customers churn at 45.3% — vs 15–18% for auto-pay customers
Customers with 3+ services churn significantly less — bundling creates switching costs
---
✅ Recommendations
Priority	Recommendation	Expected Impact
🔴 High	Convert month-to-month customers to annual contracts with incentives	Reduce churn by up to 30%
🔴 High	Implement 90-day onboarding programme for new customers	Reduce first-year churn
🔴 High	Investigate Fibre Optic customer satisfaction urgently	Recover high-value segment
🟡 Medium	Offer 5% discount for auto-pay adoption	Reduce payment-related churn
🟡 Medium	Promote multi-service bundles	Increase switching costs
🟢 Low	Improve tech support quality and response times	Improve loyalty scores
---
📂 Dataset
Source: Telco Customer Churn — Kaggle
Size: 7,043 rows × 21 columns
Features: Demographics, services, contract type, payment method, tenure, monthly charges, churn status
---
🧹 Data Cleaning Steps
Removed 11 blank rows in TotalCharges column
Converted TotalCharges from text to decimal number
Formatted tenure as numeric
Created Tenure Group column: 0-12, 13-24, 25-48, 49+ months
Created Churn Flag column: 1 = Churned, 0 = Retained
Verified all categorical columns (Contract, PaymentMethod, InternetService)
Saved as .xlsx for Power BI import
---
📐 DAX Measures Created
```
Churn Rate = DIVIDE(COUNTROWS(FILTER('Telco','Telco'[Churn]="Yes")), COUNTROWS('Telco'))

Total Churned = COUNTROWS(FILTER('Telco','Telco'[Churn]="Yes"))

Avg Tenure = AVERAGE('Telco'[tenure])

Retention Rate = 1 - [Churn Rate]
```
---
👤 About
Kamohelo Mabena
Future Interns Data Science & Analytics Internship Programme (2026)
📎 LinkedIn: [Add your LinkedIn URL here]
📁 Task 1 Project: [Add Task 1 GitHub link here]
---
Built with Microsoft Excel and Power BI Desktop.
