# 🚀AI-Powered Database Query Optimizer

> AI-powered platform for analyzing SQL queries, detecting bottlenecks, and generating optimization suggestions using Large Language Models.

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Next.js](https://img.shields.io/badge/Next.js-16-black)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Overview

OptimizeQL AI is a full-stack SQL optimization platform that helps developers improve query performance through AI-assisted analysis.

The application can inspect SQL queries, evaluate execution plans, identify performance bottlenecks, and recommend:

- Index optimizations
- Query rewrites
- Statistics improvements
- Configuration tuning
- Materialized view suggestions

It supports both static SQL analysis and live database introspection using PostgreSQL and MySQL.

---

# ✨ Core Features

### 🔍 AI-Based Query Optimization
Analyze SQL queries using LLMs such as Groq, OpenAI, Gemini, Anthropic, and more.

### 📊 EXPLAIN Plan Analysis
Automatically parses and evaluates query execution plans to detect inefficient operations.

### ⚡ Optimization Suggestions
Generates actionable recommendations including:
- CREATE INDEX statements
- Query rewrites
- Join optimizations
- Statistics updates
- Config tuning

### 🧠 Multi-LLM Provider Support
Compatible with:
- Groq
- OpenAI
- Gemini
- Anthropic
- OpenRouter
- DeepSeek
- Llama models

### 🐘 PostgreSQL + MySQL Support
Connect directly to databases and run query introspection securely.

### 🧪 Hypothetical Index Simulation
Uses PostgreSQL HypoPG extension to simulate indexes without modifying production data.

### 📜 Query History Tracking
Stores previous analyses with summaries and optimization metrics.

### 🌙 Modern Dark Dashboard
Clean dashboard UI with:
- Query activity tracking
- Optimization insights
- AI-generated summaries
- Interactive result cards

### 🔐 Secure Credential Storage
Database credentials and API keys are encrypted before storage.

### 🐳 Dockerized Setup
Complete full-stack setup using Docker Compose.

---

# 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Next.js 16, React 19, TypeScript, TailwindCSS |
| Backend | FastAPI, Python 3.12, SQLAlchemy |
| Database | SQLite, PostgreSQL, MySQL |
| AI Integration | Groq, Gemini, OpenAI APIs |
| SQL Parsing | sqlglot |
| Charts/UI | Recharts, Monaco Editor |
| Containerization | Docker, Docker Compose |

---

# 📂 Project Structure

```bash
OptimizeQL-AI/
│
├── backend/
│   ├── api/
│   ├── services/
│   ├── connectors/
│   ├── core/
│   └── tests/
│
├── frontend/
│   ├── src/app/
│   ├── src/components/
│   ├── src/context/
│   └── src/lib/
│
├── docker-compose.yml
└── README.md
```

---
# 🚀 Getting Started
## 🐳 Run with Docker
git clone https://github.com/tanyasingh0909/AI-Powered-Code-Review-Assistant-for-Engineering-Teams--Team_name_doesntmatter.git](https://github.com/tanyasingh0909/AI-Powered-Database-Query-Optimizer--Team_name_doesntmatter

cd AI-Powered-Database-Query-Optimizer--Team_name_doesntmatter

docker compose up --build

Open:

http://localhost:3000
## 💻 Local Development
Backend Setup
cd backend

python -m venv .venv

# Windows
.venv\Scripts\activate

pip install -r requirements.txt

uvicorn main:app --reload

## Backend runs on:

http://localhost:8000
Frontend Setup
cd frontend

npm install

npm run dev

## Frontend runs on:

http://localhost:3000
⚙️ Environment Variables

## Create:

backend/.env

Example:

APP_ENV=development

LLM_PROVIDER=groq
LLM_MODEL=llama-3.3-70b-versatile

GROQ_API_KEY=your_api_key

RATE_LIMIT=10/minute

EXPLAIN_TIMEOUT_MS=30000
## 🔌 API Endpoints
Method	Endpoint	Description
POST	/api/v1/analyze	Analyze SQL query
POST	/api/v1/analyze/compare	Compare two queries
GET	/api/v1/analyze/history	Query history
GET	/api/v1/analyze/stats	Dashboard metrics
POST	/api/v1/connections	Add DB connection
GET	/health	Health check
# 📈 Future Improvements
AI-generated execution plan visualization
Query latency benchmarking
PDF optimization reports
Real-time collaborative SQL workspace
Advanced index recommendation engine
Cloud deployment support
Authentication system
# 🧪 Testing
cd backend

pytest tests/ -v
# 🔒 Security
Encrypted API key storage
Read-only query execution mode
EXPLAIN timeout protection
Docker-safe environment configuration
# 🤝 Contributing

# Contributions are welcome.
