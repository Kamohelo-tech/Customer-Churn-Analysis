
# CUSTOMER RETENTION & CHURN ANALYSIS

**Telco Customer Churn - Analytics Report**

- **Dataset:** Telco Customer Churn Dataset (Kaggle)
- **Tools Used:** Microsoft Excel | Power BI Desktop
- **Total Customers Analysed:** 7,043
- **Prepared by:** Kamohelo Mabena
- **Programme:** Future Interns - Data Science & Analytics Task 2 (2026)

---

## 1. Executive Summary

This report presents a comprehensive customer retention and churn analysis for a telecommunications company. The analysis is based on 7,043 customer records, examining demographics, service subscriptions, contract types, and churn behaviour.

The overall churn rate stands at **26.5%** meaning more than 1 in 4 customers left the business during the analysis period. This represents a significant revenue risk. The analysis identifies **contract type, tenure, and internet service type** as the three most powerful predictors of churn.

Clear, actionable recommendations are provided to help the business reduce churn, improve retention, and protect long-term revenue.

---

## 2. Key Performance Indicators

| **Total Customers** | **Churned Customers** | **Churn Rate** | **Avg Tenure** |
|---|---|---|---|
| **7,043** | **1,869** | **26.5%** | **32 months** |

---

## 3. Overall Churn Analysis

Of the 7,043 customers analysed, 1,869 churned a rate of 26.5%. This is significantly above the industry benchmark of 15–20% for telecommunications companies, indicating the business has a serious retention problem that requires immediate attention.

The remaining 73.5% of customers (5,174) were retained. However, the high churn rate means the business must constantly acquire new customers just to maintain its current size, which is far more expensive than retaining existing ones.

**Key Insight:** Reducing churn from 26.5% to 20% would retain approximately **460 additional customers** per cycle, directly improving recurring revenue.

---

## 4. Churn by Contract Type

Contract type is the single strongest predictor of churn in this dataset. The analysis reveals a dramatic difference in churn rates across the three contract types:

| **Contract Type** | **Customers** | **Churned** | **Churn Rate** |
|---|---|---|---|
| Month-to-Month | 3,875 | 1,655 | 42.7% |
| One Year | 1,473 | 166 | 11.3% |
| Two Year | 1,695 | 48 | 2.8% |

Month-to-month customers churn at an alarming rate of **42.7%** over **15 times higher** than two-year contract customers. This is the most critical finding in the analysis. Customers on long-term contracts are far more committed and significantly less likely to leave.

**Recommendation:** Aggressively incentivise customers to upgrade from month-to-month to annual or two-year contracts. Offer 1–2 months free, discounted rates, or premium features as switching incentives.

---

## 5. Churn by Customer Tenure

Tenure analysis reveals that the risk of churn is heavily concentrated in the early months of a customer's lifecycle. Customers in their first 12 months are significantly more likely to churn than long-term customers.

| **Tenure Group** | **Avg Churn Rate** | **Risk Level** |
|---|---|---|
| 0–12 months | 47.4% |  Very High |
| 13–24 months | 31.2% |  High |
| 25–48 months | 18.6% |  Medium |
| 49+ months | 6.1% |  Low |

Almost half of all new customers (**47.4%**) churn within their first year. This points to a critical onboarding and early engagement problem. Once customers pass the 4-year mark, churn drops to just 6.1%, indicating that long-term customers are highly loyal.

**Recommendation:** Implement a **90-day onboarding programme** for all new customers. Assign dedicated support, send proactive check-in communications, and offer early loyalty rewards to customers who stay past 6 months.

---

## 6. Churn by Internet Service Type

Internet service type shows a strong correlation with churn. Fibre Optic customers churn at a significantly higher rate than DSL customers, despite Fibre Optic being the premium, higher-cost service.

| **Internet Service** | **Customers** | **Churn Rate** |
|---|---|---|
| Fibre Optic | 3,096 | 41.9% |
| DSL | 2,421 | 18.9% |
| No Internet | 1,526 | 7.4% |

Fibre Optic customers churn at **41.9%** more than double the DSL rate. This is counterintuitive given that Fibre Optic is the premium service. It suggests that Fibre Optic customers may have higher expectations that are not being met, or that competitors are offering better Fibre deals.

**Recommendation:** Conduct an urgent satisfaction survey among Fibre Optic customers. Investigate service quality, pricing competitiveness, and support response times. Consider a loyalty discount for Fibre customers at the 12-month mark.

---

## 7. Churn by Payment Method

Payment method analysis reveals that customers paying by **electronic check** churn at a much higher rate (**45.3%**) compared to customers on automatic payment methods (15-18%). This suggests that friction in the payment process or financial instability may be contributing to churn.

**Recommendation:** Incentivise customers to switch to automatic payment methods (bank transfer or credit card auto-pay). Offer a **5% monthly discount** for customers who enable auto-pay. This reduces payment friction and improves retention.

---

## 8. Retention Drivers - What Keeps Customers?

The analysis identified the following factors that are strongly associated with customer retention:

- **Long-term contracts:** Two-year contract customers have a churn rate of just 2.8%  the strongest retention factor identified.
- **Tenure beyond 12 months:** Customers who survive the first year are dramatically more likely to stay long-term.
- **Multiple services:** Customers subscribed to 3 or more services (phone + internet + streaming) churn at lower rates due to switching costs.
- **Automatic payment:** Auto-pay customers show 15-18% churn vs 45% for manual payment customers.
- **Tech support subscription:** Customers with tech support add-ons churn at lower rates, suggesting support quality drives loyalty.

---

## 9. Summary Recommendations

1. **Convert month-to-month customers:** Offer 1-2 months free or a 20% discount to customers who upgrade to annual contracts. Target the 3,875 month-to-month customers first this is the highest-impact action available.

2. **Fix the first-year experience:** Build a 90-day onboarding programme. Send proactive check-ins at 30, 60, and 90 days. Reward customers who reach 6 months with a loyalty benefit.

3. **Investigate Fibre Optic satisfaction:** Urgently survey Fibre Optic customers. At 41.9% churn, this segment is haemorrhaging revenue. Identify whether the issue is price, quality, or competition.

4. **Push auto-pay adoption:** Offer a 5% monthly discount for auto-pay. Electronic check customers churn at 45% switching them to auto-pay could halve their churn risk.

5. **Bundle services strategically:** Promote multi-service bundles. Customers with more services have higher switching costs and lower churn rates. Create attractive phone + internet + streaming packages.

6. **Prioritise tech support quality:** Customers with tech support subscriptions churn less. Improve support response times and resolution rates across all customer segments.

---

## 10. Tools & Methodology

**Data Source:** Telco Customer Churn Dataset (Kaggle- blastchar/telco-customer-churn). The dataset contains 7,043 customer records with 21 features including demographics, services, contract type, payment method, tenure, and churn status.

**Data Cleaning:** Performed in Microsoft Excel - blank cell removal (TotalCharges column had 11 blank rows which were removed), data type formatting, and creation of tenure group and churn flag columns.

**Analysis & Visualisation:** Conducted in Power BI Desktop. Six interactive visuals were built: 4 KPI cards, churn by contract type bar chart, churn by tenure line chart, churn by internet service donut chart, churn by payment method chart, and retention drivers summary.

**Calculated Columns:** Tenure Group (0-12, 13-24, 25-48, 49+ months), Churn Flag (1/0), and Customer Segment columns were created using DAX and Power Query.

---

*Kamohelo Mabena | Future Interns Data Science & Analytics Task 2 (2026) | Customer Churn Analysis*
