# Low-Cost Option App

A multi-agent LLM application built with CrewAI that demonstrates how to create cost-effective AI applications using alternative LLM providers.

## Overview

This project showcases how to build a multi-agent system using CrewAI while optimizing for cost by leveraging alternative LLM providers like Groq. It demonstrates best practices for creating efficient and cost-effective AI applications.

## Prerequisites

- Python 3.12 or higher
- Poetry for dependency management
- API keys for:
  - OpenAI
  - Groq
  - Tavily
  - LangChain (optional, for tracing)

## Installation

1. Clone the repository
2. Install dependencies using Poetry:
   ```bash
   poetry install
   ```
3. Copy the environment variables template:
   ```bash
   cp .env.example .env
   ```
4. Fill in your API keys in the `.env` file

## Project Structure

```
.
├── app/               # Main application code
├── tests/            # Test files
├── .env.example      # Environment variables template
├── poetry.lock       # Poetry lock file
└── pyproject.toml    # Project configuration and dependencies
```

## Dependencies

- crewai: ^0.28.8 - For building multi-agent systems
- beautifulsoup4: ^4.12.3 - For web scraping
- langchain-groq: ^0.1.3 - For using Groq as an LLM provider
