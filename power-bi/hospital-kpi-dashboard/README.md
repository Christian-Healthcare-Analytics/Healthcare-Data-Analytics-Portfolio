📈 Hospital KPI Dashboard (Power BI)

A clinical performance dashboard tracking ER wait times, length of stay (LOS), readmission %, encounter volume, and denial rates using synthetic healthcare data.

📊 Dashboard Preview

Add your screenshot here:

## 📊 Dashboard Preview
![Hospital KPI Dashboard](./screenshots/hospital-kpi-dashboard-overview.png)

## 🗺️ Data Model
![Data Model](./screenshots/hospital-kpi-data-model.png)

## 📈 KPI Insights
![Insights](./screenshots/hospital-kpi-insights.png)


📂 Project Structure
/hospital-kpi-dashboard
    raw-data/
    cleaned-data/
    pbix/
    screenshots/
    README.md

📁 Key Files

Power BI file (PBIX):
./pbix/hospital-kpi-dashboard.pbix

Synthetic datasets:

kpi_daily.csv

encounters.csv (optional)

departments.csv (optional)

📌 KPIs Included

Average ER Wait Time (minutes)

Average LOS (hours)

Daily Encounter Volume

Readmission Rate (%)

Claims Denial Rate (%)

🔧 Example DAX Measures

Average ER Wait (min):

Avg ER Wait (min) =
    AVERAGE(kpi_daily[avg_er_wait_minutes])


Average LOS (hrs):

Avg LOS (hrs) =
    AVERAGE(kpi_daily[avg_los_hours])


Readmission Rate (%):

Readmission Rate (%) =
    AVERAGE(kpi_daily[readmission_rate_pct])


Denial Rate (%):

Claims Denial Rate (%) =
    AVERAGE(kpi_daily[claims_denial_rate_pct])

🔌 Data Model (Recommended)

Use kpi_daily[date] as your main date field, optionally linking:

encounters[admit_datetime]

departments[department_id]

Add your model screenshot here:

![Data Model](./screenshots/data-model.png)

🧠 Example Insights

ER wait times peak on weekends and evenings.

Readmission rates increase when LOS rises above threshold levels.

Denial rates correlate with high encounter-volume days.

▶️ How to Rebuild This Dashboard

Import kpi_daily.csv

Add line charts for ER Wait, LOS, Readmission %

Create KPI cards

Add slicers (Date, Department)

Apply conditional formatting (Green/Yellow/Red)

Style with healthcare theme (Blue/Green/White)

✅ Skills Demonstrated

Healthcare operations analytics

KPI dashboard design

Time-series analysis

Power BI modeling + DAX
