
---

# 📁 **2. Hospital KPI Dashboard — README.md**

```md
# 📈 Hospital KPI Dashboard (Power BI)

Tracks clinical performance KPIs including ER wait time, readmission %, LOS, throughput, and patient volume.

---

## 📊 Dashboard Preview
![Hospital KPI Dashboard](./screenshots/dashboard.png)

---

## 📁 Files  
- PBIX:  
  `[Download PBIX](./pbix/hospital-kpi-dashboard.pbix)`
- Raw datasets:  
  - encounters.csv  
  - kpi_daily.csv  
  - departments.csv

---

## 📌 KPIs  
- Average ER Wait (minutes)  
- Average LOS (hours)  
- Readmission Rate (%)  
- Daily Encounter Volume  
- Claims Denial Rate (%)  

---

## 🔧 DAX Example  
```DAX
Avg LOS = AVERAGE(kpi_daily[avg_los_hours])
