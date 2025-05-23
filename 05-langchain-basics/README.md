# LangChain Basics

This project demonstrates fundamental concepts and implementations using LangChain, a framework for developing applications powered by language models.

## Overview

This repository contains examples and implementations of various LangChain features, focusing on:

- Conversation buffers and memory management
- Chat history handling
- Basic LangChain components and chains

## Prerequisites

- Python 3.11.4 or higher
- Poetry for dependency management

## Installation

1. Clone the repository
2. Install dependencies using Poetry:

```bash
poetry install
```

3. Copy the environment variables template and set up your API keys:

```bash
cp .env.example .env
```

## Project Structure

- `001-conversation-buffer.py` - Example of implementing conversation buffers
- `002-chat-memory.py` - Implementation of chat memory management
- `zzz-nb001-buffer-memory.ipynb` - Jupyter notebook exploring buffer memory concepts
- `zzz-nb002-chat-history.ipynb` - Jupyter notebook demonstrating chat history functionality

## Dependencies

The project uses the following main dependencies:

- langchain (^0.2.11)
- langchain-openai (^0.1.17)
- langchain-community (^0.2.10)
- python-dotenv (^1.0.1)
- tiktoken (^0.7.0)
- jupyterlab (^4.2.4)

## Usage

1. Ensure you have set up your environment variables in the `.env` file
2. Run the Python scripts directly:

```bash
python 001-conversation-buffer.py
python 002-chat-memory.py
```

Or open the Jupyter notebooks to explore the concepts interactively:

```bash
jupyter lab
```
