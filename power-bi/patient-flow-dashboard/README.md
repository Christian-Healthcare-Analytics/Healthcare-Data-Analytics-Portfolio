# 🏥 Patient Flow Dashboard (Power BI)

A healthcare operations dashboard analyzing patient throughput, ER wait times, bed utilization, and 30-day readmissions.

---

## 📂 Project Structure
---
/patient-flow-dashboard
├── raw-data/
├── cleaned-data/
├── pbix/
├── screenshots/
└── README.md


## 📊 Dashboard Preview  

![Patient Flow Dashboard](./screenshots)

---

## 📁 Files in This Project  
[Files](./raw-data)
- Raw data:  
  - `patients.csv`  
  - `encounters.csv`  
  - `providers.csv`  
  - `departments.csv`
- Cleaned data (generated in Power Query)

---

## 🧠 Key Metrics  
- **Length of Stay (LOS)**  
- **ER Wait Time (minutes)**  
- **Patient Throughput Time**  
- **Readmission Rate (30 days)**  
- **Bed Utilization (%)**

---

## 🔧 DAX Measures Used  
```DAX
Length of Stay (Hours) = AVERAGE(encounters[length_of_stay_hours])

Readmission Rate (%) =
DIVIDE(
    CALCULATE(COUNT(encounters[encounter_id]), encounters[readmitted_30d] = 1),
    COUNT(encounters[encounter_id])
)
