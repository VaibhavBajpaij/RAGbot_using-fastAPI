# 👽 RAG PDFBot - V3 (FastAPI + Streamlit)

This is the **production-ready refactor** of the RAG PDFBot, introducing a real separation between frontend (UI) and backend (logic) using **Streamlit** and **FastAPI** respectively. This modular architecture helps in scaling, extending, and deploying the bot in real-world environments.

---

## 🧑‍💻 Author & Repository

- 👤 **Author:** Vaibhav Bajpai  
- 🔗 **Repository:** https://github.com/VaibhavBajpaij/RAGbot_using-fastAPI  

---

## 🔄 What Changed from `rag-bot-chroma`

| Feature | Version 2 | Version 3 |
|--------|-------------|--------------|
| Codebase | One Streamlit app | Split into `client/` + `server/` |
| PDF Upload | In Streamlit | Async FastAPI API |
| Chat | In Streamlit | Calls `/chat` API |
| Vectorstore | In UI | Controlled by backend |
| Model Options | Static | Dynamically fetched |
| Inspector | In sidebar | Main panel toggle |
| Splitting | `RecursiveTextSplitter` | `TokenTextSplitter` |
| UX | Crude | Responsive, clear, downloadable |
| Extendability | Hard | Easy to plug new LLMs, tools |

---

## 🧪 Demo

![demo-gif](/assets/rag-bot-fastapi.gif)

---

## 🏗️ Architecture

![architecture](/assets/rag-bot-fastapi-architecture.png)

---

## 🚀 Features

- 📁 Upload multiple PDFs and chat with them  
- 🔌 Choose from Groq or Gemini as LLM providers  
- 🔎 Query inspector for vectorstore transparency  
- 🧠 RAG with LangChain + ChromaDB  
- 📦 Streamlit frontend, FastAPI backend  
- 🧪 Token-based chunking for LLM precision  
- 💬 Downloadable chat history  
- 🧰 Tools for reset, undo, clear  
- 🌐 Fully API-driven interaction  

---

## 🛠️ Tech Stack

- **Frontend**: Streamlit  
- **Backend**: FastAPI  
- **LLMs**: Groq & Gemini via LangChain  
- **Vector DB**: ChromaDB  
- **Embeddings**: HuggingFace & Google GenAI  
- **Chunking**: TokenTextSplitter  
- **Parsing**: PyPDF  
- **Orchestration**: LangChain Retrieval Chain  

---

## 📦 Installation

```bash
git clone https://github.com/VaibhavBajpaij/RAGbot_using-fastAPI.git
cd RAGbot_using-fastAPI