# LLM Engineering with LangChain

This project demonstrates various aspects of working with Large Language Models (LLMs) using the LangChain framework. It includes examples of connecting to different LLM providers, working with prompt templates, chains, and output parsers.

## Project Structure

The project is organized into several Python scripts and Jupyter notebooks that cover different aspects of LLM engineering:

- `001-connect-llm.py`: Basic connection to LLM providers
- `002-trying-different-llm-models.py`: Examples of working with different LLM models
- `003-prompt-templates.py`: Working with LangChain prompt templates
- `004-chains.py`: Creating and using LangChain chains
- `005-output-parsers.py`: Parsing and structuring LLM outputs

Each script has a corresponding Jupyter notebook (prefixed with `zzz-nb`) that provides a more interactive learning experience.

## Prerequisites

- Python 3.11.4
- Poetry (for dependency management)

## Installation

1. Clone the repository
2. Install dependencies using Poetry:

   ```bash
   poetry install
   ```

3. Copy the `.env.example` file to `.env` and add your API keys:
   ```bash
   cp .env.example .env
   ```

## Environment Variables

Create a `.env` file with the following variables:

- `OPENAI_API_KEY`: Your OpenAI API key
- `GROQ_API_KEY`: Your Groq API key (if using Groq models)

## Usage

You can run the Python scripts directly:

```bash
python 001-connect-llm.py
```

Or open the Jupyter notebooks for an interactive experience:

```bash
jupyter lab
```

## Dependencies

- langchain: ^0.2.10
- langchain-openai: ^0.1.17
- langchain-groq: ^0.1.6
- python-dotenv: ^1.0.1
- jupyterlab: ^4.2.4
