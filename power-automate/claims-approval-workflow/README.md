# ✔ Claims Approval Workflow (Power Automate)

A multi-level approval flow that routes **new claims** through one or more approvers, logs decisions, and notifies stakeholders.

---

## 📸 Flow Preview

> Suggested screenshots:
> - `./screenshots/claims-approval-flow-overview.png`
> - `./screenshots/claims-approval-flow-steps.png`

![Claims Approval Flow](./screenshots)

---

## 📁 Project Files

- **Flow export** (placeholder):  
  `./exports/claims-approval-workflow.zip`

- **Data file** (referenced, not stored here):  
  `claims.csv`

---

## 🔧 High-Level Logic

1. **Trigger**: when a new claim is added or status = "Pending"  
2. **Create approval** → send to Level 1 approver  
3. If **approved**, optionally send to Level 2  
4. **Write decision** back to data source (status, approver, timestamp)  
5. **Send notification email** to claim owner

---

## 💼 Business Value

- Standardizes claim approval  
- Clear audit trail of decisions  
- Faster resolution of pending claims  

---

## 🚀 Usage

1. Build (or import) this flow in Power Automate  
2. Connect it to your claims list or table  
3. Configure approver emails  
4. Test with a few synthetic claims  
