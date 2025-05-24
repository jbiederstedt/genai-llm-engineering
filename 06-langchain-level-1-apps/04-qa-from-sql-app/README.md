# QA from SQL Application

This application demonstrates how to use LangChain to perform natural language queries on a SQL database. It allows users to ask questions in plain English and get answers based on the data stored in a SQLite database.

## Features

- Natural language to SQL query conversion
- SQL query execution
- Natural language response generation
- Integration with OpenAI's GPT models
- Support for SQLite databases

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

## Project Structure

```
.
├── data/                   # Contains the SQLite database
├── tests/                  # Test files
├── 001-qa-from-sql.py     # Main application file
├── zzz-nb001-qa-from-sql.ipynb  # Jupyter notebook version
├── pyproject.toml         # Poetry dependencies
└── .env.example           # Environment variables template
```

## Usage

The application provides three main functionalities:

1. Converting natural language questions to SQL queries
2. Executing SQL queries and returning results
3. Generating natural language answers based on query results

Example usage:

```python
from langchain_openai import ChatOpenAI
from langchain_community.utilities import SQLDatabase

# Initialize the database connection
db = SQLDatabase.from_uri("sqlite:///data/street_tree_db.sqlite")

# Create and execute a chain
chain = create_sql_query_chain(llm, db)
response = chain.invoke({"question": "List the species of trees that are present in San Francisco"})
```

## Dependencies

- langchain
- langchain-openai
- langchain-community
- python-dotenv
- jupyterlab
