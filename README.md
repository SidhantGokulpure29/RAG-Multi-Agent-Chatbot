# 🤖 RAG Multi-Agent Chatbot

A **Retrieval-Augmented Generation (RAG)** powered chatbot built with **LangGraph**, **Groq LLMs**, and **ChromaDB**.  
This project demonstrates how multi-agent orchestration + vector databases can deliver **context-aware, reliable answers** from long-form documents.  

---

## ✨ Features
- 🔍 **Document Retrieval**: Uses ChromaDB + Sentence Transformers for semantic search.  
- 🧠 **Multi-Agent Workflow**: Classifier routes queries to either RAG Agent or Logical Agent.  
- 📚 **Context-Aware Responses**: RAG Agent grounds answers in retrieved chunks.  
- ⚡ **Error Handling**: Falls back gracefully when context is insufficient.  
- 🛠️ **Prompt Engineering**: Custom system prompts reduce hallucinations and enforce clarity.  

---

## 📦 Requirements
Install dependencies with:
```bash
pip install groq langgraph langchain_community chromadb sentence-transformers langchain-text-splitters
