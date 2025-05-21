# Poetry Setup Project

This project demonstrates the use of Poetry for Python dependency management and project setup, with a focus on AI/ML development using LangChain.

## Project Overview

This project serves as a practical example of using Poetry for managing Python dependencies in an AI/ML project. It includes:

- A structured Python project setup using Poetry
- Integration with LangChain and OpenAI
- Jupyter notebook examples and tutorials
- Test environment setup

## Prerequisites

- Python 3.11.4
- Poetry (Python package manager)
- JupyterLab

## Installation

1. Install Poetry (if not already installed):

   ```bash
   # Using Homebrew (recommended for macOS)
   brew install poetry

   # Or using the official installer
   curl -sSL https://install.python-poetry.org | python3 -
   ```

2. Clone this repository and navigate to the project directory:

   ```bash
   cd A003-POETRY-SETUP-master
   ```

3. Install project dependencies:

   ```bash
   poetry install
   ```

4. Activate the virtual environment:
   ```bash
   poetry shell
   ```

## Project Structure

- `a003_poetry_setup/` - Main project package
- `tests/` - Test files
- `*.ipynb` - Jupyter notebooks with tutorials and examples
- `pyproject.toml` - Poetry project configuration
- `poetry.lock` - Locked dependencies

## Dependencies

The project uses the following main dependencies:

- langchain (^0.2.10)
- langchain-openai (^0.1.17)
- jupyterlab (^4.2.4)
- python-dotenv (^1.0.1)

## Usage

1. After installation, you can start JupyterLab:

   ```bash
   poetry run jupyter lab
   ```

2. Open the notebooks in the following order:
   - `zzz-nb001-poetry-vs-pyenv.ipynb` - Introduction to Poetry vs Pyenv
   - `zzz-nb002-student-setup-after-downloading-code.ipynb` - Setup guide

## Learning Resources

The included notebooks provide comprehensive guides on:

- Understanding Poetry vs Pyenv
- Setting up development environments
- Managing Python dependencies
- Working with LangChain and AI development
