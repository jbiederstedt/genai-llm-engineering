# Simple Agent with LangChain and LangGraph

This project demonstrates the implementation of a simple agent using LangChain and LangGraph, capable of answering questions about current events using web search capabilities.

## Features

- Integration with OpenAI's GPT-3.5 Turbo model
- Web search functionality using Tavily Search
- Agent implementation using LangGraph's ReAct framework
- Streaming responses for real-time interaction
- Memory management for conversation context
- Thread-based conversation management

## Prerequisites

- Python 3.11.4 or higher
- Poetry for dependency management
- OpenAI API key
- Tavily API key

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

## Usage

The project includes both a Python script and a Jupyter notebook implementation:

- `001-simple-agent.py`: Main script implementation
- `zzz-nb001-simple-agent.ipynb`: Jupyter notebook version with detailed explanations

To run the script:

```bash
poetry run python 001-simple-agent.py
```

## Example Queries

The agent can handle various types of questions, such as:

- "Where is the soccer Eurocup 2024 played?"
- "When and where will it be the 2024 Eurocup final match?"
- "Who won the 2024 soccer Eurocup?"
- "Who were the top stars of that winner team?"

## Project Structure

```
.
├── 001-simple-agent.py          # Main script
├── zzz-nb001-simple-agent.ipynb # Jupyter notebook
├── pyproject.toml              # Project dependencies
├── poetry.lock                 # Locked dependencies
├── .env.example               # Example environment variables
└── tests/                     # Test directory
```

## Dependencies

- langchain
- langchain-openai
- langchain-community
- langgraph
- python-dotenv
- jupyterlab
