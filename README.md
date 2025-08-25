# Resume Screening & HR Conversations Dataset for LLM Training  

Recruitment and career advisory tools often require sensitive data, which is difficult to access and share. This dataset removes that barrier by providing **synthetic HR conversations and resume screening Q&A**, structured for **LLM training** in JSONL format.  

It’s designed for developers and researchers who want to build **HR assistants, candidate screening bots, and career guidance tools**—without using real resumes or personal information.  

---

## ✅ Why This Dataset?
- **Accelerate HR AI development** – No need to source or anonymize real resumes.
- **Ready for LLM Training** – Structured in OpenAI-compatible JSONL format.
- **Privacy-Safe & Scalable** – 100% synthetic, zero PII.

---

## 📂 Dataset Description  
This dataset contains **synthetic HR conversations and resume screening Q&A**, formatted for **LLM fine-tuning**. Each record represents a dialogue simulating real-world HR workflows like candidate evaluation and career guidance.

- **Format:** JSONL (OpenAI fine-tuning compatible)
- **Schema:**  
  - `messages`: An array of chat messages with roles (`system`, `user`, `assistant`) and their respective content.

### Example:
```json
{
  "messages": [
    {"role": "system", "content": "You are an informative assistant."},
    {"role": "user", "content": "What is AbdulMuiz Shaikh's current job title?"},
    {"role": "assistant", "content": "AbdulMuiz Shaikh's current job title is Associate Data Scientist."}
  ]
}
```

---

## 🔍 What's Inside
- **Resume Screening Q&A**
  - Job titles, experience, role responsibilities.
- **Career Guidance Questions**
  - Tech trends, upskilling, and career planning.

---

## 👥 Who Should Use This Dataset?
- **Recruitment Tech Startups** – Build automated candidate screeners.
- **HR Teams** – Deploy internal career chatbots.
- **AI Engineers & Researchers** – Fine-tune LLMs for HR applications.
- **EdTech Platforms** – Power career advisory assistants.

---

## 🚀 How To Use
Fine-tune with OpenAI:
```bash
openai tools fine_tunes.prepare_data -f hr_resume_qna.jsonl
openai api fine_tunes.create -t "hr_resume_qna.jsonl" -m "gpt-3.5-turbo"
```

Explore in a Jupyter Notebook:  
👉 [**View Notebook**](#) *(coming soon)*

---

## ✅ Why Synthetic?
- **No compliance headaches** (GDPR, PII safe)
- **Faster experimentation** for LLM applications
- **High-fidelity HR scenarios** for realistic model behavior

---

## 🔗 Start Generating Your Own Synthetic Data

[**→ Generate your own synthetic datasets now**](https://app.syncora.ai/login)
