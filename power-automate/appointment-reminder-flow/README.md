
---

## 3️⃣ Appointment Reminder Flow — `power-automate/appointment-reminder-flow/README.md`


# 📅 Appointment Reminder Flow (Power Automate)

A cloud flow that automatically sends **email reminders** for appointments scheduled for **tomorrow**, helping reduce no-shows.

---

## 📸 Flow Preview

> Screenshot files you can use:
> - `./screenshots/appointment-reminder-flow-overview.png`
> - `./screenshots/appointment-reminder-flow-logic.png`

![Appointment Reminder Flow](./screenshots)

---

## 🎯 Goal

- Detect patients with appointments scheduled for **the next day**
- Send a personalized reminder email
- Optionally log that the reminder was sent

---

## 📁 Project Files

- **Flow export** (when you export it from Power Automate):  
  `./exports/appointment-reminder-flow.zip`  *(placeholder name you can use)*

- **Sample data source** (stored outside or referenced in docs):  
  Based on `appointments.csv` from your portfolio datasets.

---

## 🔧 High-Level Logic

1. **Trigger**  
   - Recurrence trigger: every day at 08:00 AM

2. **Get appointments**  
   - From Excel / SharePoint / SQL table based on `appointments.csv`

3. **Filter rows**  
   - `appointment_datetime` = tomorrow  
   - `status = "Scheduled"`

4. **For each result**  
   - Send email to `patient_email` with date/time + visit type

5. **(Optional)**  
   - Update row / log “Reminder Sent”

---

## 🧪 Example Email Text

> Subject: Appointment Reminder for Tomorrow  
>  
> Body:  
> Hello, this is a reminder of your appointment scheduled for **{date} at {time}**.  
> Visit type: **{visit_type}**.  
> If you need to reschedule, please contact our clinic.

---

## 🚀 How to Use (later)

1. Import `appointment-reminder-flow.zip` into Power Automate  
2. Map data source to your actual appointments table  
3. Update email sender & text  
4. Turn the flow **On**  
