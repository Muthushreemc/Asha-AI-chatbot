Asha — AI Career Companion for Women

Project: Asha AI Chatbot

Team: Alpha
Team Lead: Muthu Shree MC

Team member: Ranga Kavya

# One‑line summary

Asha is an AI-powered, context-aware chatbot that helps women discover jobs, mentorship, and community events through real‑time retrieval-augmented generation (RAG) and bias‑mitigating, personalized conversations.

# Problem statement

Build an AI-powered, context-aware chatbot that delivers personalized, meaningful interactions and integrates seamlessly with the JobsForHer Foundation platform to empower women’s professional journeys.

# Key idea

Asha combines live API data (jobs, mentorships, events) with a vector store and a high‑quality LLM to answer questions with up‑to‑date, contextual, and bias‑aware responses. It supports multi‑turn dialogues and prioritizes inclusivity and ethical behaviour.

# Unique Selling Points (USPs)

Real‑time job & mentorship discovery via public APIs

Retrieval-Augmented Generation (RAG) for accurate, context-aware responses

Gender‑bias detection and mitigation to ensure respectful, inclusive output

Context retention for natural multi‑turn conversations

Privacy‑first, scalable architecture

# Features

Real‑Time Job & Mentorship Search: Fetches latest openings and mentor profiles.

RAG + LLM Integration: Uses vector store retrieval (Pinecone) + LLM (Groq API) for grounded answers.

Bias Detection & Correction: On‑the‑fly checks to detect and reduce gendered or biased language.

Multi‑turn Context: Maintains conversation state to provide tailored guidance.

Secure & Scalable Back-end: Flask API, Pinecone vector DB, and cloud‑ready design.

Architecture (high level)

Frontend (React) — chat UI, resume/job upload

Backend (Flask) — API endpoints, user session & context management

RAG Layer — Pinecone vector DB for embeddings + retrieval logic

LLM Calls — Groq API for generation (prompt templates + retrieved context)

External APIs — job boards, events, mentorship directories

Diagrams: See docs/architecture.png and docs/flow.png in the repository.

# Tech Stack

Frontend: React

Backend: Flask (Python)

Vector DB: Pinecone

LLM: Groq API (or configurable LLM provider)

Authentication & Hosting: (configurable — e.g., Vercel / Heroku / AWS)

Quickstart — development (example)

# Clone
git clone <repo-url>
cd asha-ai

# Backend
cd backend
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt
export PINECONE_API_KEY=...
export GROQ_API_KEY=...
flask run

# Frontend
cd ../frontend
npm install
npm run dev

Environment variables (essential)

PINECONE_API_KEY

PINECONE_ENV

GROQ_API_KEY (or other LLM provider key)

JOB_API_KEY (optional: for job listings)

#Demo & Resources

Demo video (3–5 minutes) available in assets/demo.mp4.

Prototype slides: docs/Asha_Hackathon_Prototype.pdf.


Contribution Guidelines

Fork the repo

Create a feature branch feature/<name>

Open a PR with description & screenshots

Follow code style and add tests for backend logic

Team & Contact

Team Alpha — Lead: Muthu Shree MC
For questions, reach out: 
Muthu Shree MC - muthushreemc@gmail.com
Ranga Kavya - rangakavya2004@gmail.com
(https://github.com/kavya-ux-2)
