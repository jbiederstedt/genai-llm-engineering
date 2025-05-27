# Text Rewriting Application

A Streamlit-based application that uses LangChain and OpenAI to rewrite text in different tones and dialects. This application allows users to transform their text into formal or informal tones while also converting between American and British English dialects.

## Features

- Text rewriting with customizable tone (Formal/Informal)
- Dialect conversion (American/British English)
- User-friendly Streamlit interface
- OpenAI GPT integration for high-quality text generation
- Maximum input length of 700 words for optimal performance

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

2. Open your web browser and navigate to the provided local URL (typically http://localhost:8501)

3. Enter your OpenAI API key in the designated field

4. Input the text you want to rewrite (maximum 700 words)

5. Select your desired tone (Formal/Informal) and dialect (American/British)

6. View your rewritten text in the output section

## Dependencies

- streamlit: ^1.37.0
- langchain: ^0.2.11
- langchain-openai: ^0.1.19

## Project Structure

```
.
├── main.py              # Main application code
├── pyproject.toml       # Poetry dependencies
├── poetry.lock         # Locked dependencies
├── .env.example        # Example environment variables
└── tests/              # Test directory
```
