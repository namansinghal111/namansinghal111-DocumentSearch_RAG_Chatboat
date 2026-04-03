# 📄 DocumentSearch RAG Chatbot

A Retrieval-Augmented Generation (RAG) chatbot built using LangChain, LangGraph, and FAISS for intelligent document search and question answering.

This project enables users to query documents (PDFs, URLs, etc.) and receive context-aware, accurate responses powered by LLMs.

---

## 🚀 Features

* 🔍 Semantic document search using FAISS
* 🧠 Context-aware responses with RAG pipeline
* 🔗 Graph-based orchestration using LangGraph
* 📄 Supports PDF and URL ingestion
* ⚡ Modular and scalable architecture
* 🧩 Easy to extend with new data sources

---

## 🏗️ Project Structure

```
.
├── data/
│   ├── attention.pdf
│   └── url.txt
├── src/
│   ├── config/               # Configuration files
│   ├── document_ingestion/   # Data loading & preprocessing
│   ├── graph_builder/        # LangGraph workflow setup
│   ├── node/                 # Graph nodes (LLM, retrieval, etc.)
│   ├── state/                # State management
│   ├── vectorstore/          # FAISS vector DB logic
│   └── __init__.py
├── .python-version
└── README.md
```

---

## ⚙️ Tech Stack

* **LLM Framework:** LangChain
* **Workflow Orchestration:** LangGraph
* **Vector Database:** FAISS
* **Language:** Python

---

## 🔄 How It Works

### 1. Document Ingestion

* Load PDFs or URLs
* Split into chunks
* Generate embeddings

### 2. Vector Storage

* Store embeddings in FAISS
* Enable fast similarity search

### 3. Query Processing

* User query is embedded
* Relevant chunks retrieved

### 4. RAG Pipeline

* Retrieved context + query sent to LLM
* Generates grounded response

### 5. LangGraph Workflow

* Nodes handle each step (retrieval, generation, etc.)
* State flows through graph

---

## 🛠️ Installation

```bash
# Clone the repository
git clone [https://github.com/your-username/DocumentSearch_RAG_Chatboat.git](https://github.com/namansinghal111/DocumentSearch_RAG_Chatboat.git)

# Navigate to project
cd DocumentSearch_RAG_Chatboat

# Create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

---

## ▶️ Usage

```bash
python main.py
```

* Add your documents to the `data/` folder
* Configure settings in `src/config`
* Run the chatbot and start querying

---

## 🔧 Configuration

Set your environment variables:

```bash
OPENAI_API_KEY=your_api_key
```

You can also modify:

* Chunk size
* Embedding model
* Retrieval strategy

---

## 🧠 Example Query

```
Q: What is attention mechanism?
A: The attention mechanism allows models to focus on relevant parts...
```

---

## 📌 Future Improvements

* 🌐 Web UI (Streamlit / React)
* 📊 Better evaluation metrics
* 🔐 Authentication & user sessions
* 🗂️ Multi-document collections
* 🧩 Plug-and-play LLM support

---
