# Simple Retriever App

This project demonstrates a basic implementation of a document retrieval system using LangChain and Chroma vector database. It showcases how to create, store, and query document embeddings using OpenAI's embedding model.

## Features

- Document storage and retrieval using Chroma vector database
- OpenAI embeddings for semantic search
- Multiple retrieval methods:
  - Simple similarity search
  - Similarity search with scores
  - Batch retrieval
  - Top-k retrieval
- Question answering using retrieved context

## Prerequisites

- Python 3.8+
- OpenAI API key
- Poetry (for dependency management)

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

## Usage

The main script `001-retriever-app.py` demonstrates various ways to use the retriever:

1. Basic similarity search
2. Similarity search with relevance scores
3. Batch retrieval of multiple queries
4. Top-k retrieval
5. Question answering using retrieved context

Run the script using Poetry:

```bash
poetry run python 001-retriever-app.py
```

## Project Structure

- `001-retriever-app.py` - Main application script
- `zzz-nb001-retriever-app.ipynb` - Jupyter notebook version of the application
- `pyproject.toml` - Project dependencies and configuration
- `.env.example` - Example environment variables
- `tests/` - Test directory

## Dependencies

- langchain-openai
- langchain-chroma
- langchain-core
- python-dotenv
- openai
