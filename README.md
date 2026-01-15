# 📄 RAG PDF Chatbot using Gemini & Streamlit

A Retrieval-Augmented Generation (RAG) based PDF chatbot that allows users to upload PDF documents and ask questions using **Google Gemini**, **LangChain**, **FAISS**, and **Streamlit**.

---

## 🚀 Features

- 📂 Upload multiple PDF files
- 🔍 Semantic search using FAISS vector database
- 🧠 Gemini-powered question answering
- 📑 Accurate answers strictly from document context
- ⚡ Fast & interactive Streamlit UI
- 🔐 Secure API key handling with `.env`

---

## 🏗️ Tech Stack

- **Frontend:** Streamlit  
- **LLM:** Google Gemini (Gemini 1.5 Pro)  
- **Embeddings:** Google Generative AI Embeddings  
- **Framework:** LangChain  
- **Vector DB:** FAISS  
- **PDF Parsing:** PyPDF2  

---

## 📁 Project Structure

```bash
.
├── app.py
├── requirements.txt
├── .env
├── faiss_index/
└── README.md
```
---

## 🔑 Environment Setup

Create a .env file in the root directory:
```bash
GOOGLE_API_KEY=your_google_gemini_api_key_here
```
⚠️ Never commit .env to GitHub. Add it to .gitignore.

---

## 📦 Installation
```bash
pip install -r requirements.txt
```
## ▶️ Run the Application
```bash
streamlit run app.py
```
---

## 🧠 How It Works (RAG Flow)
- Upload PDFs
- Extract text from documents
- Split text into chunks
- Generate embeddings
- Store embeddings in FAISS
- Perform similarity search
- Gemini generates answers from retrieved context

---

## 📸 UI Preview

- Upload PDFs from the sidebar
- Ask questions in the main chat input
- Get AI-powered answers instantly

---

## 🛡️ Security Notes

- API keys are loaded securely via .env
- Responses are restricted to document content
- Prevents hallucinations by context grounding

---

## 🌟 Future Improvements

- Chat history & memory
- Source citations
- Streaming responses
- Multi-user session handling
- Cloud deployment (Streamlit Cloud / Docker)

---

## 🙌 Author

Chintan Dabhi
AI / ML Engineer
