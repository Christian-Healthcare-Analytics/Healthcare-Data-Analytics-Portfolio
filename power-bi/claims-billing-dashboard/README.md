
---

## 2️⃣ Claims & Billing Dashboard — `power-bi/claims-billing-dashboard/README.md`


# 💰 Claims & Billing Dashboard (Power BI)

This dashboard analyzes **billed vs paid amounts**, **denial rates**, **denial reasons**, and **payer performance** to support revenue cycle optimization.

---

## 📊 Dashboard Preview

> Main screenshot file:
> `./screenshots/claims-billing-dashboard-overview.png`

![Claims Billing Dashboard](./screenshots/claims-billing-dashboard-overview.png)

Additional visuals (optional):

![Denial Reasons](./screenshots/claims-denial-reasons-chart.png)  
![Paid vs Billed](./screenshots/paid-vs-billed-chart.png)  
![Payer Breakdown](./screenshots/payer-performance-breakdown.png)

---

## 📁 Project Files

- **PBIX file**:  
  `./pbix/claims-billing-dashboard.pbix`

- [Raw data](./raw-data):
  - `claims.csv`
  - `encounters.csv` (for clinical context, LOS vs denials)

---

## 🧩 Data Model

> Optional: screenshot at  
> `./screenshots/claims-billing-data-model.png`

![Data Model](./screenshots/claims-billing-data-model.png)

Key relationship:

- `claims.encounter_id` → `encounters.encounter_id`

---

## 📐 Key DAX Measures (later in Power BI)

```DAX
Total Billed =
SUM(claims[billed_amount])

Total Paid =
SUM(claims[paid_amount])

Denial Rate (%) =
DIVIDE(
    CALCULATE(COUNT(claims[claim_id]), claims[status] = "Denied"),
    COUNT(claims[claim_id])
)

Paid to Billed Ratio =
DIVIDE([Total Paid], [Total Billed])
