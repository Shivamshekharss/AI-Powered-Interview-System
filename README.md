🚀 AI Interview Simulator

Fully Offline • Multi-Agent Architecture • Llama 3.1 (Ollama) • Streamlit UI

A production-ready offline AI interview platform powered by local LLMs, featuring adaptive questioning, role-based question generation, semantic evaluation, and multi-agent orchestration — without requiring any API keys or internet access.

This project demonstrates strong skills in LLM application engineering, agent design, system orchestration, full-stack integration, and offline RAG pipelines — ideal for real-world enterprise deployments.

<div align="center">
🔥 100% Local. 100% Private. 100% Real AI.

https://img.shields.io/badge/LLM-Llama3.1-green

https://img.shields.io/badge/Framework-Ollama-blue

https://img.shields.io/badge/UI-Streamlit-red

https://img.shields.io/badge/Database-ChromaDB-purple

https://img.shields.io/badge/Architecture-Multi--Agent-yellow

</div>
📌 Overview

This system simulates a complete technical interview experience:

💬 Conversational Interviewer (adaptive, natural, context-aware)

🧠 Dynamic Question Generator (role, difficulty, and experience-based)

📊 Evaluator Agent (semantic scoring + feedback)

📝 Explanation Agent (shows correct answers / reasoning)

🔎 Offline Embedding + RAG Support (ChromaDB + Nomic embeddings)

🖥 Streamlit UI (clean, responsive, real-time interaction)

Everything runs offline, making the project suitable for enterprise compliance, security-first applications, and deployment inside restricted environments.

🧠 Multi-Agent Architecture
                         ┌──────────────────────────┐
                         │      Streamlit UI        │
                         └────────────┬─────────────┘
                                      │
                           Interview Orchestrator
                                      │
     ┌────────────────────┬───────────┬──────────────────┬──────────────────┐
     │                    │           │                  │                  │
┌────────────┐     ┌────────────┐  ┌───────────┐  ┌────────────┐   ┌─────────┐
│ Interviewer│     │ Question   │  │ Evaluator │  │ Explanation │   │ Vector  │
│   Agent    │     │ Generator  │  │   Agent   │  │    Agent    │   │  Store  │
└────────────┘     └────────────┘  └───────────┘  └────────────┘   └─────────┘
     │                     │            │              │               │
     └───────────────────── Llama 3.1 (via Ollama) ────────────────────┘
                                      │
                               Local Embeddings
                                      │
                                   ChromaDB

✨ Features
🧩 1. Offline LLM Engine

Runs on Llama 3.1 via Ollama

No OpenAI API required

Fast, private, and secure

🤖 2. Multi-Agent System

Interviewer Agent: human-like dialog

Question Generator: custom questions

Evaluator: scores correctness, depth, clarity

Explanation: provides ideal answers

📚 3. RAG + Embeddings

Uses nomic-embed-text model

Stores embeddings in ChromaDB

Enhances question quality & evaluation

🖥 4. Modern UI

Built using Streamlit

Live conversation

Session tracking

Evaluation summary

🔌 5. Plug-and-Play Architecture

Agents are modular and easily replaceable.

📂 Folder Structure
project-root/
│── app.py                           # Streamlit UI
│── README.md
│── .env
│── requirements.txt
│
│── backend/
│   ├── agents/
│   │    ├── interviewer_agent.py
│   │    ├── question_generator.py
│   │    ├── evaluator_agent.py
│   │    ├── simple_explanation.py
│   │
│   ├── orchestrator/
│   │    └── interview_orchestrator.py
│   │
│   ├── core/
│   │    ├── config.py
│   │    ├── embeddings.py
│   │    └── vector_store.py
│
│── data/
│── logs/
│── screenshots/
│── venv/
