# RAG App Evaluation Tool

A Streamlit-based application for evaluating the quality and accuracy of Retrieval-Augmented Generation (RAG) applications. This tool helps you assess whether your RAG system is providing accurate answers or hallucinating by comparing its responses against known correct answers.

## Features

- Upload and process text documents
- Evaluate RAG system responses against ground truth
- Interactive Streamlit interface
- Automatic evaluation using OpenAI's language models
- FAISS vector store for efficient document retrieval

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

3. Copy the `.env.example` file to `.env` and add your OpenAI API key:

```bash
cp .env.example .env
```

## Usage

1. Start the Streamlit application:

```bash
poetry run streamlit run main.py
```

2. In the web interface:
   - Upload a text document containing the information you want to evaluate
   - Enter a question that you have already fact-checked
   - Provide the known correct answer
   - Enter your OpenAI API key
   - Submit to evaluate the RAG system's response

The application will:

- Process your document
- Generate a response using the RAG system
- Compare the response with the known correct answer
- Provide an evaluation of the response quality

## Dependencies

- streamlit: ^1.37.0
- langchain: ^0.2.11
- langchain-openai: ^0.1.19
- chromadb: ^0.5.5
- tiktoken: ^0.7.0
- faiss-cpu: ^1.8.0.post1
- langchain-community: ^0.2.10

## Project Structure

```
.
├── main.py              # Main application code
├── pyproject.toml       # Poetry dependencies
├── poetry.lock         # Locked dependencies
├── .env.example        # Example environment variables
└── tests/              # Test directory
```

## How It Works

1. The application uses LangChain to process and split the uploaded document into chunks
2. FAISS vector store is used to create embeddings and enable efficient document retrieval
3. A RetrievalQA chain is used to generate responses to questions
4. The QAEvalChain evaluates the generated responses against the known correct answers
5. Results are displayed in the Streamlit interface
