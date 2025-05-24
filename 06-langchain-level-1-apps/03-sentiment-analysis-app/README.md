# Sentiment Analysis App

This project demonstrates a sentiment analysis application built using LangChain and OpenAI's GPT-3.5 Turbo model. The application analyzes text to determine sentiment, political tendency, and language of the input text.

## Features

- Sentiment analysis of text input
- Political tendency classification
- Language detection
- Structured output using Pydantic models
- Support for both free-form and enum-based classifications

## Prerequisites

- Python 3.8+
- OpenAI API key
- Poetry (for dependency management)

## Installation

1. Clone the repository
2. Copy `.env.example` to `.env` and add your OpenAI API key:
   ```bash
   cp .env.example .env
   ```
3. Install dependencies using Poetry:
   ```bash
   poetry install
   ```

## Usage

The project includes both a Python script and a Jupyter notebook:

- `001-sentiment-analysis.py`: Main script demonstrating the sentiment analysis functionality
- `zzz-nb001-sentiment-analysis.ipynb`: Jupyter notebook with detailed examples and explanations

To run the Python script:

```bash
poetry run python 001-sentiment-analysis.py
```

## Project Structure

```
.
├── 001-sentiment-analysis.py      # Main script
├── zzz-nb001-sentiment-analysis.ipynb  # Jupyter notebook
├── .env.example                   # Example environment variables
├── pyproject.toml                 # Poetry dependencies
├── poetry.lock                    # Locked dependencies
└── tests/                         # Test directory
```

## Features in Detail

The application can analyze text in two ways:

1. **Free-form Classification**:

   - Sentiment: Any text describing the sentiment
   - Political tendency: Any text describing political views
   - Language: Any text describing the language

2. **Enum-based Classification**:
   - Sentiment: ["happy", "neutral", "sad"]
   - Political tendency: ["conservative", "liberal", "independent"]
   - Language: ["spanish", "english"]

## Example Output

The script includes example analyses of two different political statements, showing both free-form and enum-based classifications.
