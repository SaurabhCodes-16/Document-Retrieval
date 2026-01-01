# 📚 RAG-Based LLM Powered Query–Retrieval System

A **Retrieval-Augmented Generation (RAG)** system capable of extracting, embedding, retrieving, and answering questions from multi-format documents with **context-grounded, concise, and reliable responses**.

This system integrates **FastAPI, PyTorch, FAISS, LangChain, and OpenAI/Gemini LLMs**, with performance optimization through **async concurrency, batching, structured logging, authentication, and multi-API key failover handling**.

---

## Features

- Intelligent retrieval using FAISS vector similarity search  
- LLM reasoning with grounded contextual responses  
- Supports PDF, DOC, TXT, and mixed structured/unstructured data  
- Optimized with async execution & batching  
- Secure APIs with logging and API key rotation  
- Postman validated & reliability focused  

---

## Architecture

```mermaid
flowchart LR
A[User Query] --> B[FastAPI Backend]
B --> C[Embedder - PyTorch]
C --> D[FAISS Vector DB]
D --> E[Retriever]
E --> F[LLM - OpenAI/Gemini]
F --> G[Context Grounded Answer]
