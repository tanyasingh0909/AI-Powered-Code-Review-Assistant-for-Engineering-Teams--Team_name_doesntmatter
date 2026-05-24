# 🚀AI-Powered Code Review Assistant For Engineering Teams

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
