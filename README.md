# project_01 — Adventure Story Generator

An interactive text-adventure game where a story is generated on the fly by an LLM. The player picks a theme, the backend generates a branching story, and the frontend walks the player through it screen by screen.

## Stack

- **Backend** (`backend/`): FastAPI, LangChain + Google Gemini, SQLAlchemy/PostgreSQL. Managed with [uv](https://docs.astral.sh/uv/).
- **Frontend** (`frontend/`): React 19 + TypeScript, Vite, React Router.

## Getting started

### Backend

```bash
cd backend
uv sync
uv run main.py
```

API docs available at `http://localhost:8000/docs`.

### Frontend

```bash
cd frontend
npm install
npm run dev
```

## Project structure

```
project_01/
├── backend/    # FastAPI service: story/job routers, DB models, Gemini integration
└── frontend/   # React app: theme input, story loader/generator, game UI
```
