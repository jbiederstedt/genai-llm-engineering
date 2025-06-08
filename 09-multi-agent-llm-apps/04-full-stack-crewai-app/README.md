# Full-Stack CrewAI Application

This is a full-stack application that demonstrates the power of CrewAI, a framework for orchestrating role-playing AI agents. The application features a modern Next.js frontend and a Flask backend that coordinates multiple AI agents working together to accomplish complex tasks.

## 🚀 Features

- **Multi-Agent System**: Leverages CrewAI to create a team of specialized AI agents
- **Modern Frontend**: Built with Next.js, TypeScript, and Tailwind CSS
- **Robust Backend**: Flask-based API with comprehensive agent orchestration
- **Real-time Updates**: WebSocket support for live agent activity monitoring
- **Task Management**: Structured task execution and progress tracking
- **Custom Tools**: Extensible tool system for agent capabilities

## 🏗️ Project Structure

```
.
├── frontend/               # Next.js frontend application
│   ├── app/               # Next.js app directory
│   ├── components/        # React components
│   ├── hooks/            # Custom React hooks
│   └── public/           # Static assets
│
└── backend/              # Flask backend application
    ├── agents.py         # Agent definitions
    ├── api.py           # API endpoints
    ├── crews.py         # Crew configurations
    ├── tasks.py         # Task definitions
    ├── models.py        # Data models
    └── tools/           # Custom agent tools
```

## 🛠️ Prerequisites

- Python 3.9+
- Node.js 18+
- OpenAI API key
- YouTube API key (for video search functionality)
- Poetry (for Python dependency management)

## 🚀 Getting Started

### Backend Setup

1. Navigate to the backend directory:

   ```bash
   cd backend
   ```

2. Install dependencies using Poetry:

   ```bash
   poetry install
   ```

3. Create a `.env` file based on `.env.example`:

   ```bash
   cp ../.env.example .env
   ```

   Then edit the `.env` file to add your API keys and configuration:

   ```
   OPENAI_API_KEY=your_api_key_here
   YOUTUBE_API_KEY=your_youtube_api_key_here
   MODEL_NAME=gpt-4-turbo-preview
   ```

4. Start the backend server:
   ```bash
   poetry run python api.py
   ```
   The server will run on port 3001 by default.

### Frontend Setup

1. Navigate to the frontend directory:

   ```bash
   cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env.local` file:

   ```
   NEXT_PUBLIC_API_URL=http://localhost:3001
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## 🤖 Agent System

The application uses CrewAI to orchestrate multiple AI agents, each with specific roles and capabilities:

- **Research Manager**: Coordinates research efforts and manages the research process
- **Research Agent**: Conducts detailed research on technologies and business areas

## 🔧 API Endpoints

The backend provides several endpoints for interacting with the agent system:

- `POST /api/multiagent`: Create and execute a new research task

  - Request body: `{ "technologies": ["tech1", "tech2"], "businessareas": ["area1", "area2"] }`
  - Returns: `{ "input_id": "task_id" }`

- `GET /api/multiagent/{input_id}`: Get task status and results
  - Returns: Task status, results, and event history

## 📝 Environment Variables

The application requires several environment variables to function properly. Copy `.env.example` to `.env` and fill in your values:

```
# OpenAI API Configuration
OPENAI_API_KEY=your_openai_api_key_here
MODEL_NAME=gpt-4-turbo-preview

# YouTube API Configuration
YOUTUBE_API_KEY=your_youtube_api_key_here

# Server Configuration
FLASK_ENV=development
FLASK_DEBUG=1
PORT=3001

# Frontend Configuration
NEXT_PUBLIC_API_URL=http://localhost:3001
```
