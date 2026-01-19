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
```
---

## 🧑‍⚖️ Evaluator Agent (LLM-as-Judge)

To ensure reliability and auditability, this project integrates an **Evaluator Agent** acting as an **LLM-as-Judge**.  
- ✅ **Evaluation Layer**: After the RAG Agent or Logical Agent responds, the Evaluator Agent reviews outputs.  
- 🔎 **Quality Checks**: Scores responses for relevance, grounding, and logical consistency.  
- 📊 **Feedback Loop**: Flags low-confidence answers and enforces fallback/error-handling strategies.  
- 🔒 **Auditability**: Provides transparent evaluation logs, making the multi-agent workflow reproducible and manager-friendly.  

This evaluation layer strengthens the pipeline by combining **automation** with **human-like judgment**, ensuring that responses are both **accurate** and **trustworthy**.

<img width="1452" height="676" alt="image" src="https://github.com/user-attachments/assets/c1407a06-23c9-4092-909f-1ada56863aab" />

