# 🤖 GenAI RAG Project — Google Gemini + LangChain + ChromaDB

This project showcases a **Retrieval-Augmented Generation (RAG)** pipeline leveraging state-of-the-art tools like **Google Gemini**, **LangChain** and **ChromaDB**. It is designed to retrieve contextually relevant data from document embeddings and enhance responses using a language model.

## Overview

The **GenAI RAG system** mimics the behavior of a smart assistant by attempting to answer queries directly using a large language model. If the model is uncertain or lacks context, it retrieves relevant content from a preprocessed document database and uses it to generate a reliable answer.

## Technology Stack

- **Google Gemini (Generative AI)** - Used for generating both text completions and embedding representations.

- **LangChain** - A framework for connecting LLMs with external data and tools to create robust applications.

- **ChromaDB** - A lightweight, fast vector database used to store and retrieve document chunks as embeddings.

- **PyMuPDF** - Library used for parsing PDF files and extracting structured document text.

- **python-dotenv** - Manages secret configuration variables like API keys securely using a `.env` file.

## 📁 Project Structure

```
GenAI_RAG_Project/
├── ai_agent.ipynb
├── .env
├── .gitignore
├── README.md
├── documents/
│ └── .gitkeep
└── db/
```

## Security & Best Practices

- Store credentials like API keys in a `.env` file and keep them out of version control.
- Use `.env` to let others know which variables are required.
- Avoid pushing files from `documents/` or `db/` to GitHub; use `.gitkeep` and `.gitignore` respectively.

## Folder Guidelines

- **`documents/`** — Input folder for PDF files. Tracked using a `.gitkeep` placeholder file.
- **`db/`** — Storage directory for the ChromaDB vector database. Should be excluded from Git tracking.
