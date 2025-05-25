# Simple RAG Application

This is a simple Retrieval-Augmented Generation (RAG) application built using LangChain. The application demonstrates how to create a basic question-answering system that uses document retrieval to provide context-aware responses.

## Features

- Document loading and text splitting
- Vector storage using Chroma
- OpenAI embeddings integration
- RAG-based question answering
- Simple and clean implementation

## Prerequisites

- Python 3.11.4 or higher
- OpenAI API key
- Poetry for dependency management

## Installation

1. Clone the repository
2. Install dependencies using Poetry:
   ```bash
   poetry install
   ```
3. Copy `.env.example` to `.env` and add your OpenAI API key:
   ```bash
   cp .env.example .env
   ```

## Project Structure

```
.
├── data/               # Contains the source documents
├── tests/             # Test files
├── 001-simple-rag.py  # Main application file
├── poetry.lock        # Poetry lock file
├── pyproject.toml     # Project dependencies
└── .env.example       # Example environment variables
```

## Usage

1. Place your text documents in the `data/` directory
2. Run the application:
   ```bash
   python 001-simple-rag.py
   ```

The application will:

1. Load and split the documents
2. Create embeddings and store them in Chroma
3. Set up a RAG chain for question answering
4. Process questions using the retrieved context

## How It Works

1. **Document Processing**: The application loads text documents and splits them into manageable chunks
2. **Vector Storage**: Documents are converted into embeddings and stored in Chroma
3. **Retrieval**: When a question is asked, relevant document chunks are retrieved
4. **Generation**: The LLM generates an answer based on the retrieved context

## Dependencies

- langchain
- langchain-openai
- langchain-community
- langchain-chroma
- openai
- python-dotenv
