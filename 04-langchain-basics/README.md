# LangChain Basics

This project contains a series of examples and tutorials demonstrating the fundamental concepts of LangChain, with a focus on the LangChain Expression Language (LCEL) and its practical applications.

## Project Structure

The project is organized into several key components:

- Python scripts demonstrating various LangChain concepts (numbered 001-008)
- Jupyter notebooks with detailed explanations and examples (zzz-nb001 through zzz-nb008)
- Supporting data and test directories
- Visual documentation (LCEL chain graphs)

## Key Topics Covered

1. Simple Chain Implementation
2. Legacy vs LCEL Chain Comparison
3. Runnable Execution Order
4. Invoke, Stream, and Batch Operations
5. Built-in Runnables
6. Built-in Functions for Runnables
7. Combining Chains
8. LCEL Chains in RAG Applications

## Prerequisites

- Python 3.11.4
- Poetry for dependency management

## Installation

1. Clone the repository
2. Install dependencies using Poetry:
   ```bash
   poetry install
   ```
3. Copy `.env.example` to `.env` and add your API keys:
   ```bash
   cp .env.example .env
   ```

## Dependencies

The project uses the following main dependencies:

- langchain (^0.2.11)
- langchain-openai (^0.1.17)
- langchain-community (^0.2.10)
- jupyterlab (^4.2.4)
- Additional utilities like faiss-cpu, docarray, and tiktoken

## Getting Started

1. Start with the Jupyter notebooks in order (zzz-nb001 through zzz-nb008) for a guided learning experience
2. Review the corresponding Python scripts for implementation details
3. Check the visual documentation (LCEL-chain-graph.png, lcel-2.png) for chain structure visualization

## Project Organization

- `*.py` files: Implementation examples
- `zzz-nb*.ipynb` files: Detailed tutorials and explanations
- `data/`: Supporting data files
- `tests/`: Test cases
- `b403/`: Additional project-specific code
