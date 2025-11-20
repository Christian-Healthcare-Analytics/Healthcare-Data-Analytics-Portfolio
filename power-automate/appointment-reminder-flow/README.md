📅 Appointment Reminder Automation (Power Automate)

A Power Automate cloud flow that sends email reminders for appointments scheduled for tomorrow, reducing no-shows and improving patient engagement.

📸 Flow Preview

## 📸 Flow Overview
![Appointment Reminder Flow](./screenshots/appointment-reminder-flow-overview.png)

## ⚙️ Logic Example
![Flow Logic](./screenshots/appointment-reminder-flow-logic.png)



📂 Project Structure
/appointment-reminder-flow
    screenshots/
    exports/
    README.md

📁 Key Files

Exported Flow Package (ZIP):
./exports/appointment-reminder.zip

Dataset used (external):
appointments.csv
(Contains patient_id, appointment_datetime, patient_email, visit_type, status)

🎯 Flow Objective

Automatically send a reminder email to a patient the day before their appointment.

This workflow helps:

Reduce appointment no-shows

Automate administrative work

Improve communication in clinics/telehealth settings

🔧 High-Level Flow Steps

Trigger

Recurrence (Daily at 8:00 AM)

or: “When an item is created/modified”

Get Appointments

Read from Excel / SharePoint / SQL table

Filter for Tomorrow’s Appointments
Condition examples:

appointment date = tomorrow

status = "Scheduled"

Send Reminder Email
Use patient_email from dataset.

Log Reminder Sent (optional)

Update row

Or append to a log sheet

🧪 Example Email Content

Subject:
Appointment Reminder for Tomorrow

Body:
Hello, this is a reminder for your appointment scheduled for {date} at {time}.
Visit type: {visit_type}.
If you need to reschedule, please contact us.

▶️ How to Import the Flow

Go to Power Automate
https://make.powerautomate.com

Select Import

Choose ./exports/appointment-reminder.zip

Fix all required connections:

Outlook

Excel/SharePoint/SQL

Map the data source to your appointments table

Test with sample data

Turn the flow On

✅ Skills Demonstrated

Power Automate cloud flows

Date filtering and dynamic content

Email automation

Healthcare operations workflow
