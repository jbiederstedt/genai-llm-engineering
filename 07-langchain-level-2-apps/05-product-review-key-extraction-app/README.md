# Product Review Key Extraction App

A Streamlit application that uses LangChain and OpenAI to extract key information from product reviews. The app analyzes customer reviews and extracts sentiment, delivery time, and price perception.

## Features

- Extract key information from product reviews:
  - Customer sentiment (Positive/Negative/Neutral/Unknown)
  - Delivery time
  - Price perception (Expensive/Cheap/Neutral/Unknown)
- User-friendly Streamlit interface
- Real-time analysis using OpenAI's language model
- Maximum review length of 700 words

## Prerequisites

- Python 3.11.4 or higher
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

1. Start the Streamlit app:

```bash
poetry run streamlit run main.py
```

2. Open your browser and navigate to the provided local URL (typically http://localhost:8501)

3. Enter your OpenAI API key in the designated field

4. Input a product review in the text area

5. View the extracted information:
   - Sentiment analysis
   - Delivery time
   - Price perception

## Dependencies

- streamlit: ^1.37.0
- langchain: ^0.2.11
- langchain-openai: ^0.1.19

## Project Structure

```
.
├── main.py              # Main application code
├── pyproject.toml       # Poetry dependencies
├── poetry.lock         # Locked dependencies
├── .env.example        # Example environment variables
└── tests/              # Test directory
```
