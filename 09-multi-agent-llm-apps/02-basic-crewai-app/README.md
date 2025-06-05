# Basic CrewAI Multi-Agent Application

This project demonstrates a practical implementation of CrewAI, showcasing how multiple AI agents can work together to create content. The application uses a team of specialized agents to research, write, and manage content across different platforms.

## Project Overview

The application implements a content creation workflow using four specialized AI agents:

1. **Online Researcher**: Scours the internet for relevant information and trending stories
2. **Blog Manager**: Transforms research into well-structured, SEO-optimized blog articles
3. **Social Media Manager**: Creates engaging social media content (tweets) based on the research
4. **Content Marketing Manager**: Reviews and approves all content for publication

## Features

- Multi-agent collaboration using CrewAI
- Web research capabilities using Tavily Search
- Content processing and web scraping
- Automated content creation workflow
- Content review and approval system

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
3. Copy `.env.example` to `.env` and add your API keys:
   ```bash
   cp .env.example .env
   ```

## Environment Variables

Create a `.env` file with the following variables:

```
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key
```

## Usage

Run the main script:

```bash
python 001-basic-multiagent-crewai.py
```

The script will:

1. Research a topic using the Online Researcher
2. Generate a blog article using the Blog Manager
3. Create a tweet using the Social Media Manager
4. Review and approve the content using the Content Marketing Manager

## Project Structure

- `001-basic-multiagent-crewai.py`: Main application script
- `pyproject.toml`: Project dependencies and configuration
- `.env.example`: Example environment variables
- `tests/`: Test directory
- `zzz-nb001-basic-crewai.ipynb`: Jupyter notebook version of the application

## Dependencies

- crewai: ^0.28.8
- beautifulsoup4: ^4.12.3
- Additional dependencies managed by Poetry
