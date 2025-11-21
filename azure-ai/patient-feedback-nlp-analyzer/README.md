# 💬 Patient Feedback NLP Analyzer (Azure AI)

An NLP-based project that classifies **patient feedback** by sentiment, category, and urgency.

---

## 📁 Project Files

- **Sample input** (in `./sample-input/`):  
  `patient_feedback.csv`

  Columns:
  - feedback_id  
  - patient_id  
  - submitted_date  
  - feedback_text  
  - sentiment_label (pre-labeled, for comparison)  
  - category_label  
  - urgency_label  

- **Sample output**:  
  Later you can save model predictions to `./sample-output/`.

---

## 📸 Screenshots

> Suggested files:
> - `./screenshots/patient-feedback-nlp-workflow.png`
> - `./screenshots/patient-feedback-input.png`
> - `./screenshots/patient-feedback-output.png`

![NLP Workflow](./screenshots)

---

## 🔧 Conceptual Flow

1. Take `feedback_text` from `patient_feedback.csv`  
2. Use Azure AI / Azure OpenAI classification to predict:
   - Sentiment (Positive / Neutral / Negative)  
   - Category (Staff, Billing, Wait Time, etc.)  
   - Urgency (Low / Medium / High)  
3. Compare predicted vs labeled classifications  
4. Trigger alerts for high-urgency, negative feedback (via Power Automate)

---

## 💼 Business Value

- Faster detection of serious complaints  
- Trend analysis for patient experience  
- Improved service recovery and reputation management  

---

## 🚀 Future Implementation

Once Azure AI is available to you:

- Build classification prompts  
- Score new feedback in real-time  
- Integrate with Power BI & Power Automate  
