# Text Summarizer App

A Streamlit-based web application that uses LangChain and OpenAI's GPT models to generate concise summaries of long text inputs.

## Features

- Interactive web interface built with Streamlit
- Text summarization using OpenAI's GPT models
- Secure API key handling
- Support for long-form text input
- Map-reduce summarization chain for efficient processing

## Prerequisites

- Python 3.8 or higher
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
streamlit run main.py
```

2. Open your web browser and navigate to the provided local URL (typically http://localhost:8501)

3. Enter your text in the text area
4. Enter your OpenAI API key
5. Click "Submit" to generate the summary

## Project Structure

```
.
├── main.py              # Main application file
├── pyproject.toml       # Poetry dependencies
├── poetry.lock         # Locked dependencies
├── .env.example        # Example environment variables
└── tests/              # Test directory
```

## Dependencies

- streamlit
- langchain
- langchain-openai
- openai

## Security Note

The application handles the OpenAI API key securely and does not store it permanently. The key is only used during the active session and is cleared after use.
