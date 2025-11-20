# 💰 Claims & Billing Dashboard (Power BI)

A financial performance dashboard analyzing billing, payments, denials, and payer behavior in a healthcare setting.

---

## 📊 Dashboard Preview

![Claims Billing Dashboard](./screenshots/claims-billing-dashboard-overview.png)

![Denial Reasons](./screenshots/claims-denial-reasons-chart.png)

![Paid vs Billed](./screenshots/paid-vs-billed-chart.png)

![Payer Breakdown](./screenshots/payer-performance-breakdown.png)

![Data Model](./screenshots/claims-billing-data-model.png)


)

---

## 📂 Project Structure


---

## 📁 Key Files

- **PBIX file:**  
  `./pbix/claims-billing-dashboard.pbix`

- **Raw data (synthetic):**  
  - `claims.csv`  
  - `encounters.csv`  

- **Screenshots (example names):**  
  - `./screenshots/dashboard.png`  
  - `./screenshots/data-model.png`  
  - `./screenshots/insights.png`

---

## 📌 Business Questions

This dashboard helps answer:

- How much are we **billing vs paid** by payer?
- What is our **claims denial rate (%)**?
- What are the **top denial reasons**?
- How does financial performance vary by **payer** and **encounter type**?

---

## 📊 Main Metrics

- Total Billed Amount  
- Total Paid Amount  
- Denial Rate (%)  
- Payments by Payer  
- Top Denial Reasons  
- Paid / Billed Ratio  

---

## 🔧 Sample DAX Measures

**Denial Rate (%):**

```DAX
Denial Rate (%) =
DIVIDE(
    CALCULATE(COUNT(claims[claim_id]), claims[status] = "Denied"),
    COUNT(claims[claim_id])
)
Total Billed =
SUM(claims[billed_amount])
Total Paid =
SUM(claims[paid_amount])
Paid to Billed Ratio =
DIVIDE([Total Paid], [Total Billed])
