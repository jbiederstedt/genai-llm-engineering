# Key Data Extraction App

This application demonstrates how to use LangChain and OpenAI's GPT models to extract structured information from unstructured text. It's particularly useful for extracting person-related information from text data, such as names, last names, and countries.

## Features

- Extracts structured data from unstructured text using GPT-3.5-turbo
- Supports single and multiple entity extraction
- Uses Pydantic models for type-safe data validation
- Configurable extraction schemas
- Example implementations for different use cases

## Prerequisites

- Python 3.8+
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

The application provides several examples of data extraction:

1. Single entity extraction from a review
2. Multiple entity extraction from a list
3. Multiple entity extraction from a text with several users

To run the main script:

```bash
python 001-key-data-extraction.py
```

## Project Structure

- `001-key-data-extraction.py` - Main script with examples
- `zzz-nb001-key-data-extraction.ipynb` - Jupyter notebook version
- `pyproject.toml` - Project dependencies
- `poetry.lock` - Locked dependencies
- `.env.example` - Example environment variables
- `tests/` - Test directory

## Data Models

The application uses Pydantic models for data validation:

```python
class Person(BaseModel):
    name: Optional[str]
    lastname: Optional[str]
    country: Optional[str]

class Data(BaseModel):
    people: List[Person]
```
