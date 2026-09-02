# Multi-Document RAG System

A **Multi-Document Retrieval-Augmented Generation (RAG)** system built using Python, LangChain, and an LLM. The project loads information from multiple text documents, splits them into smaller chunks, retrieves the most relevant chunks based on a user query, and generates a context-aware final answer.

## 📌 Project Overview

This project demonstrates how RAG can be used to work with information stored across multiple documents.

The system currently works with medical-related documents such as:

* `cancer_medicine.txt`
* `diagnosing_cancer.txt`
* `diagnosis.txt`
* `paracetamol.txt`

The documents are loaded and divided into smaller chunks. When a query is provided, the system retrieves the most relevant chunks from the available documents and uses them as context to generate the final response.

## 🔄 Workflow

```text
Multiple Documents
        ↓
Document Loading
        ↓
Text Chunking
        ↓
Vector/Embedding Representation
        ↓
Similarity Search
        ↓
Relevant Chunks Retrieved
        ↓
LLM
        ↓
Final Answer
```

## 📊 Current Output

The system successfully:

* Loads **4 documents**
* Creates **57 text chunks**
* Retrieves relevant chunks from different documents
* Displays the source document for each retrieved chunk
* Generates a final answer using the retrieved context

Example retrieved sources:

```text
SOURCE: cancer_medicine.txt
SOURCE: diagnosis.txt
SOURCE: cancer_medicine.txt
SOURCE: diagnosis.txt
```

This demonstrates that the system can retrieve information from **multiple documents** rather than relying on a single source.

## 🧠 Key Concepts Demonstrated

* Multi-document loading
* Document chunking
* Embeddings
* Vector similarity search
* Retrieval-Augmented Generation (RAG)
* Context-aware question answering
* Source-aware retrieval
* Large Language Models (LLMs)
* LangChain

## 🛠️ Technologies Used

* Python
* LangChain
* UV
* Large Language Model (LLM)
* Embeddings
* Vector Store
* Text Documents

## ▶️ How to Run

Clone the repository and navigate to the project folder.

```bash
uv run multidoc.py
```

The program loads the available documents, retrieves relevant chunks, and generates the final answer.

## ⚠️ Disclaimer

The included documents contain medical-related information for **educational and demonstration purposes only**. The generated responses should not be considered medical advice, diagnosis, or treatment recommendations.

## 🎯 Purpose

The main purpose of this project is to understand and demonstrate how **Retrieval-Augmented Generation can combine information from multiple documents to produce relevant and context-aware responses.**

## 🚀 Future Improvements

* Add PDF document support
* Add DOCX document support
* Add a web-based user interface
* Improve retrieval accuracy
* Add source citations to final answers
* Support larger document collections
* Add conversation memory
