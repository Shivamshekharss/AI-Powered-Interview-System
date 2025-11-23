# 🤖 AI-Powered Interview System  
### Built by **Shivamshekharss**

A fully automated AI-powered mock interview platform using **Groq Llama 3.3**, **RAG**, **FAISS**, **LangChain**, and **Streamlit**.  
It generates personalized interview questions, evaluates answers, and provides structured feedback with scoring.

---

## 🌟 Features

### 🧠 **AI Question Generation**
- Uses **Groq Llama 3.3–70B** for high-quality structured question generation  
- Generates technical, behavioral, and system design questions  
- Resume-aware question personalization  
- Difficulty-balanced question sets  

### 📚 **RAG-based Knowledge Retrieval**
- FAISS vector database  
- HuggingFace embedding model  
- Retrieves similar past questions to enrich the interview  

### 🎤 **Interview Flow**
- Step-by-step question presentation  
- Automatic evaluation of user answers  
- Real-time scoring  

### 📊 **AI Evaluation**
- Criteria-based scoring  
- Strengths, weaknesses  
- Suggested improvements  
- Final report  

### 🖥️ **Modern Streamlit UI**
- Clean centered layout  
- Blue “Start Interview” button  
- Smooth progression from input → interview → results  

---

## 🖼️ Screenshots

### 🏠 Homepage
![Homepage](assets/screenshots/homepage.png)

### 📋 After Filling Interview Details
![Homepage Filled](assets/screenshots/homepage_filled.png)

### ❓ Question 1
![Question 1](assets/screenshots/question1.png)

### ❓ Last Question
![Question 5](assets/screenshots/question5.png)

### 🧾 Results – Part 1
![Result 1](assets/screenshots/result1.png)

### 🧾 Results – Part 2
![Result 2](assets/screenshots/result2.png)

---

## ⚙️ Tech Stack

### **Backend**
- Groq Llama 3.3–70B  
- LangChain  
- FAISS Vector Store  
- HuggingFace Embeddings  
- Python 3.10  

### **Frontend**
- Streamlit

---

## 🚀 Installation & Setup

### 1️⃣ Clone the Repo
```bash
git clone https://github.com/Shivamshekharss/AI-Powered-Interview-System.git
cd AI-Powered-Interview-System
2️⃣ Create Virtual Environment
python -m venv venv
venv\Scripts\activate

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Add Environment Variables

Create a .env file:

GROQ_API_KEY=your_key_here

5️⃣ Run the App
streamlit run app.py

🧩 Project Structure
backend/
 ├── agents/
 │    ├── question_generator.py
 │    ├── interviewer_agent.py
 ├── rag/
 │    ├── embeddings.py
 │    ├── rag_retriever.py
 │    ├── vector_store.py
 ├── orchestrator/
 │    └── interview_orchestrator.py
app.py
assets/
 └── screenshots/
