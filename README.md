# 💬 SU-Chat: Sitare University Chatbot (RAG-based AI System)

A smart, interactive chatbot built for **Sitare University** using a **Retrieval-Augmented Generation (RAG)** pipeline. This chatbot helps prospective students by answering their queries about joining SU, all through a simple and user-friendly web portal 💡

---

## 🧠 Objective

To build an intelligent system that integrates:
- ✅ An **Information Retrieval (IR)** module using pgVector and transformer-based embeddings.
- ✅ A **Generative AI** layer using **LLaMA 3.1 (70B Versatile)** to generate natural, detailed answers.
- ✅ A **Flask-based web portal** for real-time user interaction and feedback collection.

---

## 👨‍💻 Team Members

- **Deepak Kumar**
- **Sahil Kumar**
- **Manu Kumar**
- **Sanjay V P**

---

## 🔍 Project Workflow

### 📥 Data Collection
- Initial dataset from a senior (Shravan, 3rd year)
- Google Form responses from juniors/seniors
- Manually curated 200+ Q&A pairs

### 🧹 Data Cleaning
- Removed irrelevant/duplicate entries
- Opted *not* to use NLTK or regex due to accuracy issues

---

## 🔧 IR Pipeline

- Used embedding models:
  - `all-minilm-l6-v2` (fast & lightweight)
  - `all-mpnet-base-v2` (balanced)
  - ✅ `multi-qa-mpnet-base-dot-v1` (**final choice** for multi-domain Q&A accuracy)
- Stored embeddings in PostgreSQL using **pgVector**
- Retrieved relevant responses using **cosine similarity**

---

## 🤖 Generative Model

- Integrated **LLaMA 3.1 (70B Versatile)** for:
  - Generating summaries
  - Enhancing user-facing answers
- Hybrid RAG pipeline: combines factual retrieval with fluid, contextual replies

---

## 🌐 Web Portal (Frontend)

- Built using **Flask**, **HTML**, **CSS**, and **JavaScript**
- Features:
  - Chat UI for query input
  - Real-time answers
  - Thumbs up/down buttons for **user feedback**
  - Feedback stored in PostgreSQL for analysis

---

## ✅ Accuracy & Evaluation

- **250+ test queries** over 12 topics
  - 200+ accurate responses ✅
  - 30+ queries lacked dataset coverage
  - 10+ returned irrelevant output
- **Achieved ~80% accuracy**

---

## 📊 User Feedback

- Feedback collected from actual SU students
- Stored in DB for further analysis
- Users can rate chatbot responses directly via UI

---

## ⚙️ Challenges Faced

- Time-consuming data collection
- Manual accuracy checks
- Integration hurdles with pgVector + embeddings

---

## 🔗 Useful Links

- 📂 [Complete Code, Dataset & Feedback Folder](https://drive.google.com/drive/folders/1Oj9BRDgo94y7i-4--Xg7UocihXomAtmS?usp=sharing)
- 📑 [Dataset & Forms Folder](https://drive.google.com/drive/folders/1atbHEi_LPWlsW7bUeFvkjMwactDc-tN-?usp=drive_link)
- 📋 [Feedback Sheet (Google Doc)](https://docs.google.com/document/d/1rFtVtE8ZeLldtv6QAaewRs0B-3bCqd13xBIUlmbTt4Q/edit?usp=sharing)

---

## 🥂 Conclusion

SU-Chat was built to provide seamless, intelligent interaction for students and aspirants of **Sitare University**. From real-time answering to feedback-driven improvement, this RAG-based chatbot showcases the power of combining retrieval with generation.

> Built with 💙 by SU Students: Deepak, Sahil, Manu, and Sanjay

---

