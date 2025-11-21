# 📈 Hospital KPI Dashboard (Power BI)

This dashboard tracks key hospital performance metrics such as **ER wait time**, **average length of stay (LOS)**, **daily encounter volume**, **readmission rate**, and **claims denial rate** using synthetic healthcare data.

---

## 📊 Dashboard Preview

> Save your main dashboard screenshot as:
> `power-bi/hospital-kpi-dashboard/screenshots/hospital-kpi-dashboard-overview.png`

![Hospital KPI Dashboard](./screenshots/hospital-kpi-dashboard-overview.png)

---

## 🧠 Purpose

This dashboard helps hospital leaders:

- Monitor operational performance day-to-day
- Spot trends in ER congestion and LOS
- Track readmission and denial rates
- Support decisions around staffing & capacity

Used by:

- Operations leadership  
- Quality & performance teams  
- Clinical managers  

---

## 📁 Project Files

- **PBIX file**:  
  `./pbix/hospital-kpi-dashboard.pbix`

- **Raw data** (place in `./raw-data/`):
  - `kpi_daily.csv`
  - `encounters.csv` (optional for drill-through)
  - `departments.csv` (optional for department breakdown)

---

## 🧩 Data Model

> Optional: screenshot at  
> `./screenshots/hospital-kpi-data-model.png`

![Data Model](./screenshots/hospital-kpi-data-model.png)

Core table:

- `kpi_daily` (one row per day)

Optional links:

- `kpi_daily[date]` → `encounters[admit_datetime]` (date)
- `departments` for breaking down encounters by department

---

## 📐 Key DAX Measures (to add later in Power BI)

```DAX
Avg ER Wait (min) =
AVERAGE(kpi_daily[avg_er_wait_minutes])

Avg LOS (hrs) =
AVERAGE(kpi_daily[avg_los_hours])

Readmission Rate (%) =
AVERAGE(kpi_daily[readmission_rate_pct])

Claims Denial Rate (%) =
AVERAGE(kpi_daily[claims_denial_rate_pct])

Total Encounters =
SUM(kpi_daily[total_encounters])
