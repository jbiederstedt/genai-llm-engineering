# Conversational RAG Application

This project demonstrates a conversational Retrieval-Augmented Generation (RAG) system built using LangChain. The application allows users to have natural conversations with an AI assistant that can reference and retrieve information from a knowledge base.

## Features

- Document loading and text splitting
- Vector storage using Chroma
- Conversational memory with chat history
- Context-aware question answering
- Session-based conversation management

## Prerequisites

- Python 3.11.4 or higher
- Poetry for dependency management
- OpenAI API key

## Installation

1. Clone the repository
2. Install dependencies using Poetry:

```bash
poetry install
```

3. Create a `.env` file in the project root and add your OpenAI API key:

```
OPENAI_API_KEY=your_api_key_here
```

## Project Structure

```
.
├── 001-conversational-rag.py    # Main application script
├── data/                        # Directory containing source documents
├── tests/                       # Test files
├── pyproject.toml              # Project dependencies
└── README.md                   # This file
```

## Usage

The application can be run in two ways:

1. Using the Python script:

```bash
poetry run python 001-conversational-rag.py
```

2. Using the Jupyter notebook:

```bash
poetry run jupyter notebook zzz-nb001-conversational-rag.ipynb
```

## How It Works

1. The application loads documents from the `data` directory
2. Documents are split into chunks and embedded using OpenAI's embeddings
3. A vector store (Chroma) is created to store and retrieve document chunks
4. The RAG chain combines:
   - A retriever to fetch relevant context
   - A question-answering chain to generate responses
   - Chat history management for contextual conversations

## Dependencies

- langchain
- langchain-openai
- langchain-community
- langchain-chroma
- python-dotenv
- bs4
- jupyterlab
