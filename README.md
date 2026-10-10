# AI-Powered Personalized Learning OS

An adaptive AI learning platform for K-12 students with personalized curriculum generation, interactive lessons, voice chat, video-based sentiment analysis, and progress-aware tutoring.

## Features

- Personalized onboarding for grade, subjects, learning goals, and preferences
- AI-generated curriculum with subjects, chapters, lessons, and activities
- Conversational teaching flow with chat and voice interaction
- Video-feed sentiment signals for engagement-aware learning
- Student progress tracking across lessons and activities
- Supabase-backed authentication and data storage
- FastAPI backend with a Next.js frontend

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Next.js, React, TypeScript, Tailwind CSS |
| Backend | FastAPI, Python, Pydantic, SQLAlchemy |
| Auth & Data | Supabase Auth, PostgreSQL |
| AI | OpenAI/AI service integrations for voice, tutoring, curriculum, and evaluation |
| Cache | Redis |
| Testing | pytest, Vitest, Playwright |

## Project Structure

```text
AI-Powered-Personalized-Learning-OS-Video-Chat-Voice/
├── backend/
│   ├── app/
│   │   ├── routers/        API routes
│   │   ├── services/       AI, curriculum, sentiment, voice, activity logic
│   │   ├── models/         Database models
│   │   ├── schemas/        Pydantic schemas
│   │   └── core/           Database, auth, Redis, Supabase helpers
│   ├── tests/
│   └── requirements.txt
├── frontend/
│   ├── src/app/            Next.js app routes
│   ├── src/components/     UI components
│   ├── src/hooks/          Client hooks
│   └── src/lib/            API and Supabase clients
├── docker-compose.yml
└── CLAUDE.md
```

## Getting Started

### Prerequisites

- Python 3.11+
- Node.js 20+
- Redis, or Docker for the included Redis service
- Supabase project credentials
- AI provider API keys required by your environment configuration

### Backend

```bash
cd backend
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

### Redis

```bash
docker compose up -d redis
```

## Environment

Create environment files from the examples in `backend/` and `frontend/`, then add your Supabase, Redis, and AI provider settings.

## Contact

- Omkar Bhosale
- Email: omkarbhosale1623@gmail.com
- Phone: +91 7559173480

