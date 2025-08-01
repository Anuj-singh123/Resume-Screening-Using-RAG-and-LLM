# Resume Screening RAG Pipeline  

## Introduction  

Hiring a candidate today is like **finding a needle in a haystack**.  
For a single job posting, thousands of resumes are received.  

- Recruiters spend hours scrolling through resumes.  
- Old tools only check for **keywords** like "Python" or "SQL".  
- But keywords can be misleading.  

Example:  
- Candidate A: “Built a fraud detection system using TensorFlow.”  
- Candidate B: “Attended a 2‑day workshop on TensorFlow.”  

A keyword search will say both are equal ❌.  
But any human recruiter knows Candidate A is stronger ✅.  

This project was built to solve exactly this problem.  

It uses **AI (Large Language Models + Retrieval-Augmented Generation)** to **understand resumes like a human**, not just match words.  

---

## What Does This Project Do?  

Think of this project as your **AI Recruiter Assistant**.  

### Step 1: Recruiter gives a Job Description  
Example:  
“We need a Data Scientist skilled in Python, Machine Learning, SQL, and AWS.”  

### Step 2: The System Reads All Resumes  
It doesn’t just look for words. It looks for **skills, responsibilities, and real project work** in the resume.  

### Step 3: It Finds the Best Candidates  
- Scores each candidate from **most relevant → least relevant**.  
- Creates a **ranking table** (ID + Score).  

### Step 4: Explains the Match  
For each candidate, it shows:  
- ✅ Skills that match the job  
- ❌ Skills that are missing  

Example Output:  
1. **Tushar Patel (Applicant 202)**  
   - ✅ Python, TensorFlow, Cloud experience  
   - ❌ SQL not found  
   - Strong ML project experience  
   - **Score: 0.86**  

2. **Riya Sharma (Applicant 145)**  
   - ✅ Python, SQL, GCP  
   - ❌ TensorFlow missing  
   - Strong Data Analysis background  
   - **Score: 0.74**  

---

## Why Not Just Keyword Search?  

Because **humans don’t write resumes in one fixed way**.  
- One candidate might write “ML pipelines with Python.”  
- Another might write “Developed predictive models in Python.”  
Both mean the same, but a keyword tool may miss it.  

That’s why we use **RAG (Retrieval-Augmented Generation)**.  

- **Step 1:** Convert resumes into vectors (mathematical form of meaning).  
- **Step 2:** When a job description comes, the system **retrieves the most similar resumes**.  
- **Step 3:** The LLM (AI model) then explains why those resumes match.  

This way, we get **context-aware, human-like results** instead of blind keyword matches.  

---

## Tech Behind the Scenes  

- **LangChain** → Connects AI with retriever logic  
- **HuggingFace Embeddings** → Turns resumes into vector form  
- **FAISS** → Fast similarity search between job and resumes  
- **OpenAI GPT / HuggingFace LLMs** → Generates answers & explanations  
- **Streamlit** → Easy-to-use web interface for recruiters  

---

## Real-Life Example  

**Job Description:**  
“Looking for Machine Learning Engineer with strong Python, Deep Learning (TensorFlow/PyTorch), SQL, and Cloud (AWS/GCP).”  

**System Output:**  

1. **Tushar Patel (Applicant 202)**  
   - ✅ Python, TensorFlow, Cloud experience  
   - ❌ SQL missing  
   - Past projects: Fraud detection system on IoT data  
   - **Score: 0.86**  

2. **Riya Sharma (Applicant 145)**  
   - ✅ Python, SQL, Cloud (GCP)  
   - ❌ Deep Learning missing  
   - Past projects: Sales prediction, data pipelines  
   - **Score: 0.74**  



## Features  

✔ Rank all resumes by relevance  
✔ Show matched vs missing skills  
✔ Compare candidates side-by-side  
✔ Upload your own resume dataset (CSV format)  
✔ Chatbot Q&A — Ask: “Who are top 5 for Data Scientist role?”  



## Why It’s Important  

- Saves **hours of recruiter effort**  
- Ensures **fair screening** (not just buzzwords)  
- Works even when job descriptions are **long and complex**  
- Brings **Explainability** → recruiters know *why* a candidate is selected  

---

## Future Scope  

- Visual dashboard: Graphs for skill coverage per candidate  
- Deployment on Cloud (so HRs can use it online directly)  
- Integration with existing ATS (Applicant Tracking Systems)  

---

## 👨‍💻 Author  

This project is developed by **Anuj Singh (IIT Kharagpur)** as part of an advanced AI project portfolio.  
It demonstrates expertise in:  
- Machine Learning  
- Deep Learning  
- NLP  
- RAG pipelines  
- Deployment (Streamlit)  

Targeting **Data Scientist / ML Engineer** roles at top companies.

**Mobile Number**-6390277170

**Email**-anujsinghanuj97@gmail.com

**Linkdin**-[Link Text](https://www.linkedin.com/in/anuj-singh-5882971a9/details/education/)




---

