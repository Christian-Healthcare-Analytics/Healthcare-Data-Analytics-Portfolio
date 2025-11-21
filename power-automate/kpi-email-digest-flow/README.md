# 📧 KPI Email Digest Flow (Power Automate)

A daily email automation that sends hospital leadership a **summary of key KPIs** (encounters, ER wait, LOS, readmission %, denial %).

---

## 📸 Flow Preview

> Suggested screenshots:
> - `./screenshots/kpi-email-digest-flow-overview.png`
> - `./screenshots/kpi-email-digest-email-sample.png`

![KPI Email Digest Flow](./screenshots/kpi-email-digest-flow-overview.png)

---

## 📁 Project Files

- **Flow export** (placeholder name):  
  `./exports/kpi-email-digest-flow.zip`

- **Data file** (outside or referenced):  
  `kpi_daily.csv` (same as Power BI KPI dashboard)

---

## 🔧 Flow Logic

1. **Trigger**: Recurrence (every morning at 07:00 AM)  
2. **Get row** from `kpi_daily` for today or most recent date  
3. **Compose email body** with:
   - Total encounters  
   - Avg ER wait  
   - Avg LOS  
   - Readmission rate  
   - Claims denial rate  
4. **Send email** to leadership / distribution list

---

## 🧪 Example Email Body

> Subject: Daily KPI Digest – {date}  
>  
> Body:  
> - Total Encounters: {total_encounters}  
> - Avg ER Wait: {avg_er_wait_minutes} minutes  
> - Avg LOS: {avg_los_hours} hours  
> - Readmission Rate: {readmission_rate_pct}%  
> - Claims Denial Rate: {claims_denial_rate_pct}%  

---

## 🚀 Usage

Later, when you’re in Power Automate:

1. Import the flow  
2. Point it to table built from `kpi_daily.csv`  
3. Set the schedule time  
4. Update recipients  
