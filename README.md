# Agentic-RAG
# 📄 PDF RAG Chatbot with Gemini & LangChain

A Retrieval-Augmented Generation (RAG) application that allows users to upload a PDF document and ask questions about its content using Google's Gemini LLM.

## 🚀 Features

* Upload any PDF document
* Automatically extract text from PDF
* Split content into semantic chunks
* Generate embeddings for document chunks
* Store embeddings in ChromaDB
* Retrieve relevant information using similarity search
* Answer questions using Gemini 2.5 Flash
* Interactive chatbot interface

---

## 🛠️ Tech Stack

* Python
* LangChain
* Google Gemini 2.5 Flash
* ChromaDB
* PyPDF
* Sentence Transformers
* Google Generative AI Embeddings

---

## 📂 Project Workflow

```text
PDF Upload
     ↓
Text Extraction
     ↓
Chunking
     ↓
Embedding Generation
     ↓
Vector Database (ChromaDB)
     ↓
Similarity Search
     ↓
Gemini LLM
     ↓
Final Answer
```

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/pdf-rag-chatbot.git

cd pdf-rag-chatbot
```

Install dependencies:

```bash
pip install langchain
pip install langchain-community
pip install langchain-google-genai
pip install chromadb
pip install pypdf
pip install sentence-transformers
```

---

## 🔑 Configure API Key

Set your Gemini API key:

```python
import os

os.environ["GOOGLE_API_KEY"] = "YOUR_API_KEY"
```

Or use environment variables:

```bash
export GOOGLE_API_KEY=YOUR_API_KEY
```

---

## ▶️ Running the Project

1. Upload a PDF file.
2. Extract text from the PDF.
3. Generate embeddings.
4. Create a vector database.
5. Ask questions about the document.

Example:

```python
answer = ask_pdf(
    "Summarize this document"
)

print(answer)
```

Interactive mode:

```python
while True:
    question = input("Ask a question: ")

    if question.lower() == "exit":
        break

    print(ask_pdf(question))
```

---

## 📖 Example Questions

```text
What is this document about?

Summarize the document.

What are the key findings?

Who is the author?

Explain the main concepts.
```

---

## 🧠 How RAG Works

This project follows the Retrieval-Augmented Generation approach:

1. PDF content is loaded.
2. Text is divided into chunks.
3. Each chunk is converted into embeddings.
4. Embeddings are stored in ChromaDB.
5. User queries are matched against stored vectors.
6. Relevant chunks are retrieved.
7. Gemini generates answers using only the retrieved context.

This reduces hallucinations and improves answer accuracy.

---

## 📁 Project Structure

```text
pdf-rag-chatbot/
│
├── notebook.ipynb
├── README.md
├── requirements.txt
└── sample.pdf
```

---

## Future Improvements

* Streamlit Web UI
* Multi-PDF Support
* Chat History Memory
* Source Citation
* Hybrid Search
* Persistent ChromaDB Storage
* Deployment on Hugging Face Spaces

---

## 🤝 Contributing

Contributions are welcome.

Fork the repository and submit a pull request.

---

## 📜 License

MIT License

---
