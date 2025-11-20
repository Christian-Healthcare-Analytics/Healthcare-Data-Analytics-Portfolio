
---

# ⚙ **4. Appointment Reminder Flow — README.md**

```md
# 📅 Appointment Reminder Automation (Power Automate)

Sends automated appointment reminders based on tomorrow’s scheduled visit.

---

## 📸 Flow Preview  
![Flow Overview](./screenshots/flow-overview.png)

---

## 📁 Files  
- Flow Export Package: `./exports/appointment-reminder.zip`  
- Dataset: `appointments.csv`

---

## 🔧 Flow Logic  
1. **Trigger:** When a row is added or modified  
2. **Condition:** Appointment date = tomorrow  
3. **Action:** Send email to patient  
4. **Action:** Log reminder sent  

---

## 🧠 Use Cases  
- Reduces no-shows  
- Automates patient engagement  
- Works with clinic or telehealth visits  

---

## ▶️ To Reproduce  
1. Import `appointment-reminder.zip` into Power Automate  
2. Upload `appointments.csv` to Excel/SharePoint/SQL  
3. Test using sample data  

---
