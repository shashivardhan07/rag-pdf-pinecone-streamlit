# 📄 RAG PDF Chatbot using Pinecone & Streamlit

A **Retrieval-Augmented Generation (RAG)** application that allows users to **upload PDF documents and ask questions** using a conversational interface.  
The system uses **vector search (Pinecone)** and **LLMs** to generate accurate, context-aware answers, all wrapped in an interactive **Streamlit UI**.

---

## 🚀 Features

- PDF-based question answering (RAG)
- Semantic search using Pinecone vector database
- LLM-powered answer generation
- Streamlit web interface
- Clean, modular, and production-ready structure
- Environment-based configuration (no hard-coded keys)

---

## 🧠 How It Works (RAG Pipeline)

1. Upload PDF document  
2. Extract and chunk text  
3. Generate embeddings for chunks  
4. Store embeddings in Pinecone  
5. Retrieve relevant chunks based on user query  
6. Generate answer using LLM + retrieved context  

This approach reduces hallucinations and improves answer accuracy.

---

## 📂 Project Structure

<pre>
rag-pdf-pinecone-streamlit/
├── app/
│   ├── streamlit_app.py              # Main Streamlit app
│   ├── streamlit_app_voice.py        # Voice-based interaction (optional)
│   └── streamlit_app_translator.py   # Multilingual support (optional)
│
├── notebooks/
│   └── RAG_GEMINI_PINECONE_PDF.ipynb
│
├── requirements.txt
├── README.md
├── .env.example
└── .gitignore
</pre>

---

## 🛠️ Tech Stack

- Python
- Streamlit
- LangChain
- Pinecone (Vector Database)
- Google Gemini / LLM APIs
- PDF Processing (PyPDF)
- dotenv

---

## ⚙️ Environment Variables

Create a `.env` file using the template below:

GEMINI_API_KEY=your_api_key_here

PINECONE_API_KEY=your_api_key_here

PINECONE_INDEX_NAME=your_index_name
