# TXT File Summarizer

A Streamlit application that uses LangChain and OpenAI's GPT models to summarize long text files. This application solves the limitation of ChatGPT's context window by implementing a map-reduce summarization strategy.

## Features

- Upload and process text files (.txt)
- Automatic text splitting for handling long documents
- Map-reduce summarization strategy for comprehensive summaries
- Secure API key handling
- User-friendly Streamlit interface

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

3. Copy the `.env.example` file to `.env` and add your OpenAI API key:

```bash
cp .env.example .env
```

## Usage

1. Start the Streamlit application:

```bash
poetry run streamlit run main.py
```

2. Open your web browser and navigate to the provided local URL (typically http://localhost:8501)

3. Enter your OpenAI API key in the application

4. Upload a text file (.txt) that you want to summarize

5. The application will process the file and display the summary

## Technical Details

- Uses LangChain's `RecursiveCharacterTextSplitter` for intelligent text chunking
- Implements a map-reduce summarization strategy for handling long documents
- Maximum input size: 20,000 words
- Chunk size: 5,000 characters with 350 character overlap

## Project Structure

```
.
├── main.py              # Main application file
├── pyproject.toml       # Poetry dependencies
├── poetry.lock         # Locked dependencies
├── .env.example        # Example environment variables
└── tests/              # Test directory
```

## Limitations

- Maximum input file size: 20,000 words
- Only supports .txt files
- Requires an active internet connection for API calls
