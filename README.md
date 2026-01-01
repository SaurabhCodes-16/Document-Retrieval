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

```
---

## Quick Start
1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
2. **Set environment variables:**
   - Copy `.env.example` to `.env` and fill in your API keys (OpenAI, Gemini, etc.)
3. **Run the server:**
   ```bash
   uvicorn app.main:app --reload
   ```
4. **API Endpoints:**
   - `POST /api/v1/hackrx/run` — Submit document URL and questions
   - `GET /api/v1/health` — Health check

## Technologies Used
- Python, FastAPI, Pydantic
- PyTorch, SentenceTransformers
- FAISS (vector search)
- OpenAI API, Google Gemini API
- LangChain, LangSmith
- pdfplumber, python-docx, BeautifulSoup, pytesseract (OCR)


## License
Apache 2.0

## Images Included

The repository includes the following images located in the `images/` folder:

<img width="998" height="327" alt="Screenshot (47)" src="https://github.com/user-attachments/assets/52b859f4-63aa-41ac-9ea6-d509bf5a80d5" />
<img width="1276" height="381" alt="Screenshot (49)" src="https://github.com/user-attachments/assets/89ca1129-10f9-46e1-bd09-0855378c4b2e" />
<img width="1285" height="503" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/5fa1750f-ad8d-4cf6-9bab-e35694c738f9" />
<img width="1237" height="353" alt="Screenshot (51)" src="https://github.com/user-attachments/assets/c98a6775-2d9d-46ca-b037-69d4f6e04b13" />



