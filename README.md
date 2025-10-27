# 🧠 RAG-Based Conversational Assistant for Ready Tensor Publications  
**AAIDC Project 1 | Built by [@yogapriya2899](https://github.com/yogapriya2899)**  
**License:** Creative Commons Attribution–NonCommercial (CC BY–NC)

---

## 📝 Abstract  
This project presents a **Retrieval-Augmented Generation (RAG)**–based conversational assistant designed to answer questions grounded in **Ready Tensor publications**.  
It integrates document ingestion, semantic embedding, and retrieval with **Large Language Models (LLMs)** to produce contextually accurate, grounded answers.

The system demonstrates an **end-to-end Agentic AI pipeline** capable of retrieving relevant publication excerpts and generating coherent, factually consistent responses — showcasing how retrieval-based grounding enhances generative reasoning.

---

## 📖 Introduction  
As part of the **AAIDC Module 1 – Foundations of Agentic AI**, this project explores how retrieval mechanisms improve factual accuracy in conversational AI.

The RAG architecture combines **semantic search** and **generative reasoning**, making it ideal for building domain-specific assistants such as academic, research, or corporate knowledge chatbots.

This implementation specifically focuses on **35 Ready Tensor publications** to enable a contextual question–answering system.

---

## 🎯 Objectives  
- Ingest 35 Ready Tensor publications (`project_1_publications.json`)  
- Generate semantic embeddings using **text-embedding-3-small**  
- Implement **FAISS-based retriever** for efficient similarity search  
- Integrate **ChatOpenAI (GPT-3.5-Turbo)** for grounded LLM responses  
- Provide two user interfaces:  
  💻 **Notebook Chat Widget (ipywidgets)**  
  🌐 **Streamlit Web App**

---

## 🧩 System Architecture  

```plaintext
📄 project_1_publications.json
        │
        ▼
🧠 RecursiveCharacterTextSplitter
        │
        ▼
💾 OpenAI text-embedding-3-small
        │
        ▼
🗂️ FAISS Vector Store
        │
        ▼
🔎 LangChain Retriever + PromptTemplate
        │
        ▼
🤖 ChatOpenAI (GPT-3.5-Turbo)
        │
        ▼
💬 Streamlit + Chat Widget UI

-------------------------------------------------------


| Component           | Description                 |
| ------------------- | --------------------------- |
| **Framework**       | LangChain                   |
| **Vector DB**       | FAISS                       |
| **Embedding Model** | text-embedding-3-small      |
| **LLM**             | GPT-3.5-Turbo               |
| **UI Frameworks**   | Streamlit, ipywidgets       |
| **Environment**     | Google Colab / VS Code      |
| **License**         | Creative Commons (CC BY–NC) |

---------------------------------------------------------
