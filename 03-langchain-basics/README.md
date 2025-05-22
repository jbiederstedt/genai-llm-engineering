# LangChain Basics

This project provides a comprehensive introduction to LangChain, covering essential concepts and practical implementations through both Python scripts and Jupyter notebooks.

## Project Structure

The project is organized into two main formats:

- Python scripts (`*.py`) for direct execution
- Jupyter notebooks (`*.ipynb`) with detailed explanations and examples

### Core Components

1. **Data Loaders** (`001-data-loaders.py`, `zzz-nb001-data-loaders.ipynb`)

   - Loading and processing different types of data
   - Working with various document formats

2. **Text Splitters** (`002-splitters.py`, `zzz-nb003-splitters.ipynb`)

   - Document chunking strategies
   - Text splitting techniques

3. **Embeddings** (`003-embeddings.py`, `zzz-nb004-embeddings.ipynb`)

   - Text embedding generation
   - Vector representations

4. **Vector Stores** (`004-vector-stores.py`, `zzz-nb005-vector-stores.ipynb`)

   - Storing and retrieving vector embeddings
   - Vector database operations

5. **Retrievers** (`005-retrievers.py`, `zzz-nb006-retrievers.ipynb`)

   - Document retrieval strategies
   - Search and retrieval methods

6. **Top-K Retrieval** (`006-top-k.py`, `zzz-nb007-top-k.ipynb`)

   - Implementing top-k retrieval
   - Ranking and filtering results

7. **RAG with LCEL** (`007-rag-with-lcel.py`, `zzz-nb008-rag-with-lcel.ipynb`)

   - Retrieval-Augmented Generation
   - LangChain Expression Language (LCEL) implementation

8. **Indexing** (`zzz-nb009-indexing.ipynb`)
   - Document indexing strategies
   - Efficient data organization

## Setup

1. Install dependencies using Poetry:

   ```bash
   poetry install
   ```

2. Set up environment variables:
   ```bash
   cp .env.example .env
   ```
   Then edit `.env` with your API keys and configuration.

## Usage

Each component can be run either as a Python script or through its corresponding Jupyter notebook:

- For Python scripts:

  ```bash
  python 001-data-loaders.py
  ```

- For Jupyter notebooks:
  ```bash
  jupyter notebook
  ```

## Data

The project includes a `data/` directory containing sample data for testing and demonstration purposes.

## Testing

Run tests using:

```bash
poetry run pytest
```

## Dependencies

The project uses Poetry for dependency management. Key dependencies are listed in `pyproject.toml`.
