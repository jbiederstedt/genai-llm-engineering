# PDF Question Answering Application

This application demonstrates how to build a Question Answering (QA) system using LangChain that can answer questions about the content of PDF documents. It uses a combination of document loading, text splitting, vector storage, and retrieval-augmented generation (RAG) to provide accurate answers based on the PDF content.

## Features

- PDF document loading and processing
- Text splitting with configurable chunk sizes
- Vector storage using Chroma
- OpenAI embeddings for semantic search
- RAG-based question answering
- Concise and accurate responses

## Prerequisites

- Python 3.8+
- OpenAI API key
- Poetry (for dependency management)

## Installation

1. Clone the repository
2. Copy `.env.example` to `.env` and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```
3. Install dependencies using Poetry:
   ```bash
   poetry install
   ```

## Project Structure

```
.
├── data/               # Directory for PDF documents
├── tests/             # Test files
├── 001-qa-from-pdf.py # Main application script
├── poetry.lock        # Poetry lock file
├── pyproject.toml     # Project dependencies
└── .env.example       # Example environment variables
```

## Usage

1. Place your PDF document in the `data/` directory
2. Update the `file_path` variable in `001-qa-from-pdf.py` to point to your PDF
3. Run the script:
   ```bash
   poetry run python 001-qa-from-pdf.py
   ```

## How It Works

1. The application loads a PDF document using PyPDFLoader
2. The text is split into manageable chunks using RecursiveCharacterTextSplitter
3. Chunks are converted to embeddings and stored in a Chroma vector store
4. When a question is asked, the system:
   - Retrieves relevant chunks from the vector store
   - Uses these chunks as context for the LLM
   - Generates a concise answer based on the retrieved context

## Configuration

The application uses several configurable parameters:

- Chunk size: 1000 characters
- Chunk overlap: 200 characters
- LLM model: GPT-3.5-turbo-0125

You can modify these parameters in the code to suit your needs.
