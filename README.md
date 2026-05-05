# 🤖 GenAI Financial Assistant: Smart Banking Agent

![Status](https://img.shields.io/badge/Status-In%20Progress-yellow?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Framework](https://img.shields.io/badge/Framework-LangChain-00A67E?style=for-the-badge)
![LLM](https://img.shields.io/badge/LLM-Ollama%20%7C%20GPT--4-blue?style=for-the-badge)

### 📖 Overview
This project features a **Generative AI Financial Agent** designed to evolve from reactive support to proactive financial consultancy. Leveraging **Large Language Models (LLMs)** and **Prompt Engineering**, the agent provides personalized investment insights, expense alerts, and consultative financial planning.

### 🎯 Key Objectives
*   **Proactive Assistance:** Antincipating user needs through transaction analysis.
*   **Hyper-Personalization:** Tailoring suggestions based on unique investor profiles and history.
*   **Reliability & Anti-Hallucination:** Implementing strict system prompts and knowledge base grounding to ensure financial safety.

---

### 📂 Repository Structure & Project Milestones

The project is divided into specialized modules to ensure scalability and clarity:

| Phase | Module | Documentation | Key Deliverables |
| :--- | :--- | :--- | :--- |
| **01** | **Core Strategy** | [`/docs/01-agent-specs.md`](./docs/01-documentacao-agente.md) | Use case definition, persona, and system architecture. |
| **02** | **Knowledge Base** | [`/docs/02-knowledge-base.md`](./docs/02-base-conhecimento.md) | RAG strategy using mocked financial data (CSV/JSON). |
| **03** | **Prompt Engineering** | [`/docs/03-prompts.md`](./docs/03-prompts.md) | System prompts, few-shot examples, and edge-case handling. |
| **04** | **Functional Prototype** | [`/src/`](./src/) | Interactive UI (Streamlit/Gradio) integrated with LLMs. |
| **05** | **Quality Metrics** | [`/docs/04-metrics.md`](./docs/04-metricas.md) | Accuracy, safety rates, and profile coherence evaluation. |

---

### 🛠️ Tech Stack
*   **Orchestration:** LangChain / LangFlow.
*   **Models:** Ollama (Local) or OpenAI GPT-4 (API).
*   **Data Handling:** Pandas for CSV transaction processing.
*   **Frontend:** Streamlit for the interactive financial dashboard.

### 📊 Mock Data Integration
The agent is grounded in a simulated financial environment using:
*   **Transactions:** `transacoes.csv` for behavioral analysis.
*   **Investor Profile:** `perfil_investidor.json` for personalized risk assessment.
*   **Product Catalog:** `produtos_financeiros.json` for consultative matching.

---

### 🚀 How to Run (Development)
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/DanielNathalia/AI-Financial-Assistant.git
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Launch the prototype:**
    ```bash
    streamlit run src/app.py
    ```

---

### 🛡️ Safety & Anti-Hallucination
In the financial sector, precision is non-negotiable. This agent employs:
*   **System Constraints:** Explicit "don't know" protocols for out-of-scope queries.
*   **Grounding:** Every recommendation must be mapped back to the provided knowledge base.

---
