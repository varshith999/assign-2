# PlacementSprint (Pydantic AI + FastAPI + OpenRouter)

## Local run
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
source .venv/bin/activate

pip install -r requirements.txt
uvicorn src.index:app --reload --port 8000

Smart Study Planner – Generative AI Agent
Overview

Smart Study Planner is a full-stack generative AI application that creates realistic, personalized study plans based on time availability and exam constraints. The system is built as a structured AI agent, not a chatbot, ensuring reliable and deterministic outputs.

Problem

Students struggle to convert limited time into effective study schedules. Most tools provide generic plans without validating feasibility, leading to poor planning and last-minute stress.

Solution

This application uses a Pydantic AI–based agent to validate inputs, check feasibility, and generate a structured, day-wise study plan tailored to the user’s constraints. The agent enforces strict schemas, retries on invalid outputs, and provides fallback responses when needed.

Key Features

Personalized, constraint-aware study planning

Feasibility validation before plan generation

Structured, deterministic AI outputs

Robust agent orchestration with retries and fallbacks

Clean API design and smooth user experience

Fully deployed, end-to-end usable application

Tech Stack

Frontend: Next.js, Tailwind CSS

Backend: FastAPI

AI Agent: Pydantic AI

Model Provider: OpenRouter

Deployment: Vercel (frontend), Render/Fly.io (backend)
