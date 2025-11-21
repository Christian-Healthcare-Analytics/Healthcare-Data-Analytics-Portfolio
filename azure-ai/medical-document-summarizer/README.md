# 📝 Medical Document Summarizer (Azure AI)

An AI-powered workflow that takes **raw clinical notes** and produces a **structured summary** with key clinical information.

---

## 📁 Project Files

- **Sample input** (in `./sample-input/`):  
  `medical_notes.csv`

  Columns include:
  - note_id  
  - patient_id  
  - encounter_id  
  - note_date  
  - note_text  

- **Sample output** (in `./sample-output/`):  
  You can later export example JSON/CSV summaries here.

---

## 📸 Screenshots

> Suggested files:
> - `./screenshots/medical-summarizer-workflow.png`
> - `./screenshots/medical-summarizer-input.png`
> - `./screenshots/medical-summarizer-output.png`

![Workflow](./screenshots)

---

## 🔧 Conceptual Flow

1. Take `note_text` from `medical_notes.csv`  
2. Send to Azure AI / Azure OpenAI with a summarization prompt  
3. Extract key fields, e.g.:
   - Condition / diagnosis  
   - Medications  
   - Follow-up plan  
   - Risks / red flags  
4. Store results in structured form (JSON, CSV, or database)

---

## 💼 Use Cases

- Faster handoffs between clinicians  
- Quick review of long notes  
- Support for care coordination teams  

---

## 🚀 Future Implementation

Later, when you have Azure AI access, you can:

- Build a prompt flow in Azure AI Studio  
- Connect a data source (Blob Storage, SQL, etc.)  
- Map `note_text` → summarizer → output table  
