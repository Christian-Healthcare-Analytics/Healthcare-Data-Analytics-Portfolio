# 👋 Christian Kassa – Healthcare Data & Automation Portfolio

Welcome to my healthcare analytics portfolio.

I combine **hands-on healthcare operations experience** with **Power BI**, **Power Automate**, and **Azure AI** to build dashboards, automations, and AI-powered tools that support patient care, operations, and revenue cycle improvement.

---

## 🧑‍💻 Profile at a Glance

- 🏥 Focus: **Healthcare operations, patient flow, and revenue cycle analytics**
- 📊 Tools: **Power BI**, **Power Query**, **DAX**
- ⚙ Automation: **Power Automate (cloud flows, approvals, notifications)**
- 🤖 AI: **Azure AI / Azure OpenAI (NLP & summarization)**
- 📂 Portfolio code & datasets:  
  [GitHub – Healthcare Data Analytics Portfolio](https://github.com/Christian-Healthcare-Analytics/Healthcare-Data-Analytics-Portfolio)

---

## 📊 Power BI Dashboards

### 1. Patient Flow Dashboard

**Goal:** Understand patient movement through the hospital: ER wait time, length of stay (LOS), readmissions, and department utilization.

- Tracks **ER wait times**, **LOS (hours)**, and **30-day readmission rate**
- Highlights **bottlenecks** across ER, Inpatient, ICU, and other departments
- Uses synthetic data for **patients**, **encounters**, **providers**, and **departments**

[🔗 View project on GitHub](https://github.com/Christian-Healthcare-Analytics/Healthcare-Data-Analytics-Portfolio/tree/main/power-bi/patient-flow-dashboard)

---

### 2. Hospital KPI Dashboard

**Goal:** Provide leadership with a daily KPI view for hospital operations.

- Monitors **daily encounters**, **avg ER wait**, **avg LOS**
- Includes **readmission rate %** and **claims denial rate %**
- Built to support **daily/weekly KPI huddles** and email summaries

[🔗 View project on GitHub](https://github.com/Christian-Healthcare-Analytics/Healthcare-Data-Analytics-Portfolio/tree/main/power-bi/hospital-kpi-dashboard)

---

### 3. Claims & Billing Dashboard

**Goal:** Analyze financial performance by payer, denial reason, and claim status.

- Compares **billed vs paid** amounts
- Calculates **denial rates** and **Paid/Billed ratio**
- Breaks down **denial reasons** (e.g., prior auth missing, coding error)
- Helps identify **revenue leakage** and payer trends

[🔗 View project on GitHub](https://github.com/Christian-Healthcare-Analytics/Healthcare-Data-Analytics-Portfolio/tree/main/power-bi/claims-billing-dashboard)

---

## ⚙ Power Automate Workflows

### 4. Appointment Reminder Flow

**Goal:** Reduce no-shows by automatically reminding patients about next-day appointments.

- Daily trigger checks **appointments scheduled for tomorrow**
- Sends personalized emails using **patient email**, **date/time**, and **visit type**
- Built to connect with data modeled from `appointments.csv`

[🔗 View project on GitHub](https://github.com/Christian-Healthcare-Analytics/Healthcare-Data-Analytics-Portfolio/tree/main/power-automate/appointment-reminder-flow)

---

### 5. KPI Email Digest Flow

**Goal:** Email hospital leadership a one-page KPI summary each morning.

- Uses **kpi_daily** data (encounters, ER wait, LOS, readmission %, denial %)
- Converts daily metrics into a clean email format
- Demonstrates how **Power Automate + Power BI data** can support leadership

[🔗 View project on GitHub](https://github.com/Christian-Healthcare-Analytics/Healthcare-Data-Analytics-Portfolio/tree/main/power-automate/kpi-email-digest-flow)

---

### 6. Claims Approval Workflow

**Goal:** Standardize claims approvals with a structured, multi-level workflow.

- Triggered when a new claim enters a **Pending** status
- Routes to one or more approvers
- Logs decisions and can notify relevant stakeholders

[🔗 View project on GitHub](https://github.com/Christian-Healthcare-Analytics/Healthcare-Data-Analytics-Portfolio/tree/main/power-automate/claims-approval-workflow)

---

## 🤖 Azure AI Projects

### 7. Medical Document Summarizer

**Goal:** Turn long clinical notes into concise summaries that are easier to review.

- Uses synthetic **medical notes** as input
- Designed to extract:
  - Key condition or diagnosis  
  - Medications  
  - Follow-up plan  
  - Risks / red flags
- Conceptual design using **Azure AI / Azure OpenAI**

[🔗 View project on GitHub](https://github.com/Christian-Healthcare-Analytics/Healthcare-Data-Analytics-Portfolio/tree/main/azure-ai/medical-document-summarizer)

---

### 8. Patient Feedback NLP Analyzer

**Goal:** Classify patient feedback by **sentiment**, **category**, and **urgency**.

- Uses synthetic **patient feedback** text
- Intended to:
  - Detect **negative, high-urgency feedback**
  - Categorize issues (staff, billing, wait time, facility)
  - Support service recovery workflows (via Power Automate)

[🔗 View project on GitHub](https://github.com/Christian-Healthcare-Analytics/Healthcare-Data-Analytics-Portfolio/tree/main/azure-ai/patient-feedback-nlp-analyzer)

---

## 🧠 Skills Demonstrated

- **Power BI**
  - Data modeling & relationships (star schema)
  - DAX measures for KPIs (LOS, ER wait, readmission, denial rate)
  - Time-series & KPI visualization
- **Power Automate**
  - Recurrence triggers
  - Condition logic and approvals
  - Email automation
- **Azure AI**
  - NLP classification concepts
  - Document summarization flows
  - Integrating AI with healthcare text data
- **Healthcare Domain**
  - Patient flow & throughput
  - Hospital KPIs and performance monitoring
  - Claims, billing, and denial analysis

---

## 🗺 Learning Journey

Right now I am focusing on:

- Deepening skills in **Power BI** for healthcare analytics  
- Building more **end-to-end workflows** (Power BI + Power Automate + Azure AI)  
- Expanding this portfolio with additional real-world-style healthcare use cases  

Future additions will include:

- Predictive LOS and readmission models  
- More detailed revenue cycle analytics  
- Combined dashboards and automation for operations leaders  

---

## 📬 Contact

I’m open to roles in:

- Healthcare Data Analyst  
- Clinical / Operations Analyst  
- BI Analyst (Healthcare)  
- EMR / EHR & Data roles  

**Email:** `chriszethio@gmail.com`  
**GitHub:** [Christian-Healthcare-Analytics](https://github.com/Christian-Healthcare-Analytics)  
**LinkedIn:** *(add your profile link here once ready)*

