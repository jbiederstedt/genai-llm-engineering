# Blog Post Generator

A Streamlit application that generates blog posts using OpenAI's language model. This application is built with LangChain and Streamlit to create an interactive interface for generating blog content.

## Features

- Interactive web interface using Streamlit
- OpenAI integration for high-quality blog post generation
- Secure API key handling
- Automatic word count calculation
- Professional blog post formatting

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
poetry run streamlit run main.py
```

2. Open your web browser and navigate to the provided local URL (typically http://localhost:8501)
3. Enter your OpenAI API key in the sidebar
4. Input your desired blog post topic
5. The application will generate a 400-word blog post about your topic

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
- python-dotenv
