
---

# 📁 **3. Claims & Billing Dashboard — README.md**

```md
# 💰 Claims & Billing Dashboard (Power BI)

Analyzes payer patterns, denials, billing performance, payments, and financial risk.

---

## 📊 Dashboard Preview  
![Claims Dashboard](./screenshots/dashboard.png)

---

## 📁 Files  
- PBIX: `[Download PBIX](./pbix/claims-billing-dashboard.pbix)`
- Raw data:  
  - claims.csv  
  - encounters.csv  

---

## 📌 Key Metrics  
- Total Billed Amount  
- Total Paid Amount  
- Denial Rate (%)  
- Claims by Payer  
- Denial Reasons  

---

## 🔧 DAX  
```DAX
Denial Rate (%) =
DIVIDE(
    CALCULATE(COUNT(claims[claim_id]), claims[status] = "Denied"),
    COUNT(claims[claim_id])
)
