# LangSmith Chatbot using LangChain, Groq, FAISS & Streamlit

An AI-powered **RAG (Retrieval-Augmented Generation) chatbot** built using **LangChain**, **Groq LLM**, **HuggingFace Embeddings**, **FAISS Vector Store**, and **Streamlit**.

This chatbot retrieves information directly from the official LangSmith documentation and generates accurate contextual answers using semantic search + LLM reasoning.

---

## Features

- RAG-based Question Answering
- Retrieves live documentation data from LangSmith docs
- Semantic Search using HuggingFace Embeddings
- Vector Storage using FAISS
- Fast response generation using Groq Llama 3.3 70B
- Document similarity search viewer
- Interactive Streamlit UI
- Efficient chunking using RecursiveCharacterTextSplitter

---

## Tech Stack

### Frontend
- Streamlit

### Backend
- Python
- LangChain

### LLM
- Groq
- Llama 3.3 70B Versatile

### Embeddings
- HuggingFace Sentence Transformers

Model Used:

```python
sentence-transformers/all-MiniLM-L6-v2
```

### Vector Database
- FAISS

### Document Loader
- WebBaseLoader

Source:

https://docs.smith.langchain.com/

---

## Project Architecture

```text
User Query
    ↓
Streamlit UI
    ↓
Retrieval Chain
    ↓
FAISS Vector Search
    ↓
Relevant Document Chunks
    ↓
Groq LLM
    ↓
Context-Aware Response
```

---

## Project Structure

```text
langchain-project/
│
├── app.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/langchain-project.git
```

Move into project directory:

```bash
cd langchain-project
```

Create virtual environment:

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Mac/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Environment Variables

Create a `.env` file:

```env
GROQ_API_KEY=your_groq_api_key
```

Get API key from:

https://console.groq.com/

---

## Run the Application

```bash
streamlit run app.py
```

Application opens at:

```text
http://localhost:8501
```

---


## Learning Outcomes

This project demonstrates:

- Retrieval-Augmented Generation (RAG)
- Vector Databases
- Semantic Search
- Prompt Engineering
- LLM Orchestration
- LangChain Chains
- Streamlit Deployment

---
## Acknowledgements

- LangChain
- Groq
- HuggingFace
- Streamlit
- FAISS
- LangSmith Documentation
