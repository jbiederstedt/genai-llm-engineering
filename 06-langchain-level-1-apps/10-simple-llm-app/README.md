# Simple LLM App

This project demonstrates a simple implementation of a Language Model (LLM) application using LangChain. It includes various examples of LLM interactions, including translation capabilities and basic LLM operations.

## Features

- Simple LLM interactions using LangChain
- Translation examples (including built-in Spanish translation)
- Jupyter notebook examples
- FastAPI integration with LangServe
- Environment configuration for LangChain tracing

## Prerequisites

- Python 3.11.4 or higher
- Poetry for dependency management
- OpenAI API key
- (Optional) Tavily API key
- (Optional) LangChain API key for tracing

## Installation

1. Clone the repository
2. Install dependencies using Poetry:
   ```bash
   poetry install
   ```
3. Copy the environment file and configure your API keys:
   ```bash
   cp .env.example .env
   ```
4. Edit the `.env` file and add your API keys:
   - `OPENAI_API_KEY`
   - `TAVILY_API_KEY` (optional)
   - `LANGCHAIN_API_KEY` (optional)

## Project Structure

- `001-simpleTranslator.py` - Basic translation example
- `002-simpleTranslatorBuiltInSpanish.py` - Translation example with built-in Spanish support
- `zzz-nb001-simple-llm-app.ipynb` - Jupyter notebook with examples
- `01_simple_llm_app/` - Main application directory
- `tests/` - Test files

## Usage

1. Activate the Poetry environment:

   ```bash
   poetry shell
   ```

2. Run the translation examples:

   ```bash
   python 001-simpleTranslator.py
   # or
   python 002-simpleTranslatorBuiltInSpanish.py
   ```

3. For interactive examples, open the Jupyter notebook:
   ```bash
   jupyter lab zzz-nb001-simple-llm-app.ipynb
   ```

## Dependencies

- langchain
- langchain-openai
- langserve
- fastapi
- python-dotenv
- jupyterlab
- sse-starlette
