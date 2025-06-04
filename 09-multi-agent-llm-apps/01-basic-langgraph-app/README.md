# Basic LangGraph Multi-Agent Application

This project demonstrates a basic implementation of a multi-agent system using LangGraph, where multiple AI agents collaborate to perform content marketing tasks. The system consists of a content marketing manager coordinating three specialized agents: an online researcher, a blog manager, and a social media manager.

## Features

- **Content Marketing Manager**: Orchestrates the workflow between different agents
- **Online Researcher**: Searches and gathers relevant information from the web
- **Blog Manager**: Transforms research into well-structured, SEO-optimized blog content
- **Social Media Manager**: Creates engaging social media content from the blog posts

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

- `001-basic-multiagent.py`: Main implementation of the multi-agent system
- `zzz-nb001-basic-multi-agent.ipynb`: Jupyter notebook with examples and explanations
- `tests/`: Directory containing test files
- `pyproject.toml`: Project dependencies and configuration
- `.env.example`: Template for environment variables

## Usage

The system can be used to create content marketing workflows. For example, to generate a report on a specific topic:

```python
from multiagent import multiagent

result = multiagent.invoke({
    "messages": [
        HumanMessage(
            content="Write me a report on [topic]. After the research, pass the findings to the blog manager to generate the final blog article. Once done, pass it to the social media manager to write a tweet on the subject."
        )
    ]
})
```

## Dependencies

- langchain: ^0.1.16
- langgraph: ^0.0.38
- langchain-openai: ^0.1.3
- jupyterlab: ^4.2.4
- python-dotenv: ^1.0.1
- beautifulsoup4: ^4.12.3
