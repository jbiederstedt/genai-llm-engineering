# LangChain Chatbot Applications

This project contains two implementations of chatbots using LangChain and OpenAI:

1. A simple chatbot implementation
2. An advanced chatbot implementation with additional features

## Project Structure

```
.
├── 001-simple-chatbot.py          # Basic chatbot implementation
├── 002-advanced-chatbot.py        # Enhanced chatbot with additional features
├── messages.json                  # Sample conversation data
├── zzz-nb001-simple-chatbot.ipynb # Jupyter notebook for simple chatbot
├── zzz-nb002-advanced-chatbot.ipynb # Jupyter notebook for advanced chatbot
└── tests/                        # Test directory
```

## Prerequisites

- Python 3.11.4 or higher
- Poetry for dependency management
- OpenAI API key

## Installation

1. Clone the repository
2. Install dependencies using Poetry:
   ```bash
   poetry install
   ```
3. Copy `.env.example` to `.env` and add your OpenAI API key:
   ```bash
   cp .env.example .env
   ```

## Dependencies

- langchain (^0.2.11)
- langchain-openai (^0.1.20)
- python-dotenv (^1.0.1)
- jupyterlab (^4.2.4)
- langchain-community (^0.2.10)

## Usage

### Simple Chatbot

Run the simple chatbot implementation:

```bash
python 001-simple-chatbot.py
```

### Advanced Chatbot

Run the advanced chatbot implementation:

```bash
python 002-advanced-chatbot.py
```

### Jupyter Notebooks

You can also explore the implementations through the provided Jupyter notebooks:

- `zzz-nb001-simple-chatbot.ipynb`
- `zzz-nb002-advanced-chatbot.ipynb`

## Features

### Simple Chatbot

- Basic conversation capabilities
- Integration with OpenAI's language models
- Simple message handling

### Advanced Chatbot

- Enhanced conversation capabilities
- More sophisticated message processing
- Additional features and improvements over the simple version
