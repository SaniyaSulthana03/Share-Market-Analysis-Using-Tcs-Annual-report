# Share-Market-Analysis-Using-Tcs-Annual-report

# 📊 AI-Based Share Market Analysis Using TCS Annual Report

## 🔍 Project Overview

This project presents a **GenAI-powered financial analysis tool** designed to evaluate the **investment viability** of Tata Consultancy Services (TCS) shares by analyzing its official annual report. By leveraging **advanced NLP techniques and LLMs**, the system extracts, interprets, and responds to investment-related queries using contextual information directly sourced from the document.


## 🎯 Objective

To develop a smart, AI-driven system capable of parsing TCS's annual report and answering questions about the company’s financial health, performance indicators, and investment potential using a **Retrieval-Augmented Generation (RAG)** approach.

---

## ⚙ Technologies & Tools Used

* **Python** – Core programming language used for implementation.
* **LangChain** – For building the RAG pipeline and handling document chunking and retrieval flow.
* **FAISS (Facebook AI Similarity Search)** – To store and retrieve high-dimensional vector embeddings of document chunks.
* **GPT-4o-mini (OpenAI)** – A powerful Large Language Model used to provide context-aware responses.
* **PDF Parsing** – Extracting structured text data from the TCS annual report PDF.
* **RAG Architecture** – Integrating retrieval and generation for accurate, context-based answers.
* **Share Market Fundamentals** – Applied domain knowledge to validate insights and enhance financial relevance.


## 🧠 How It Works

### 📄 PDF Parsing

The TCS annual report (PDF format) is parsed to extract all readable text content.

### 📦 Document Chunking & Embedding

The text is broken down into meaningful chunks using LangChain, and each chunk is converted into vector embeddings using OpenAI embeddings.

### 📚 Storing in Vector Database (FAISS)

These vector embeddings are stored in FAISS to enable fast and accurate similarity search.

### 🔁 Retrieval-Augmented Generation (RAG)

When a user enters a financial or investment-related query, the system retrieves the most relevant chunks from the vector store.
These retrieved chunks are combined with the user’s query and passed to GPT-4o-mini for generating a rich, context-aware answer.

### 🗣 Response Generation

The LLM interprets the information and generates human-like responses grounded in the source material, helping users understand financial performance and investment opportunities.


## 📈 Use Cases

* Investment research based on annual report data
* Financial question answering using company documents
* Automated summarization and insight extraction from financial PDFs
* Application of GenAI in finance and capital markets


## 📌 Key Features

* 📄 PDF-to-AI processing using real company data
* 🧠 Context-aware response generation with LLMs
* 🔎 Accurate and efficient information retrieval using FAISS
* 📊 Financial domain focus with practical market relevance
* 🚀 Scalable architecture for any corporate financial document

## 🧪 Example Queries

* "Is TCS a good company to invest in based on its 2023 report?"
* "What were TCS’s major revenue drivers last year?"
* "Summarize TCS’s financial performance in Q4."


## ✅ Future Enhancements

* Add support for multiple companies’ reports
* Integrate with a frontend UI for interactive querying
* Implement real-time data feeds for comparison with past reports
* Add multilingual support for financial analysis


# PROJECT STRUCTURE

├── data/
│   └── TCS_Annual_Report_2023.pdf
├── embeddings/
│   └── faiss_index.bin
├── src/
│   ├── pdf_parser.py
│   ├── embedder.py
│   ├── retriever.py
│   └── query_handler.py
├── main.py
├── requirements.txt
└── README.md


