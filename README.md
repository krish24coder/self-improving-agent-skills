# 🚀 Self-Improving Agent Skills

> Automatically optimize AI agent skills using a collaborative **multi-agent system** powered by **Google ADK** and **Gemini**.

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688.svg)
![Next.js](https://img.shields.io/badge/Next.js-15-black.svg)
![React](https://img.shields.io/badge/React-19-61DAFB.svg)
![Google ADK](https://img.shields.io/badge/Google-ADK-blue.svg)
![Gemini](https://img.shields.io/badge/Gemini-AI-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

---

## 📖 Overview

**Self-Improving Agent Skills** is an AI-powered platform that automatically improves prompt-based agent skills through iterative optimization.

Built with **Google Agent Development Kit (ADK)** and **Gemini**, the application enables users to upload an agent skill, automatically generate evaluation scenarios, test performance, identify weaknesses, and continuously improve the prompt using a team of specialized AI agents.

Instead of manually tweaking prompts, the system intelligently evaluates and refines them until the desired performance is achieved.

---

# ✨ Features

- 📂 Upload Agent Skills (.zip or folder)
- 🤖 Automatic Test Scenario Generation
- ✅ Binary Evaluation Criteria Generation
- 🧠 Multi-Agent Optimization Pipeline
- 📊 Performance Scoring
- 🔄 Iterative Prompt Improvement
- ⚡ Live Optimization Progress (SSE)
- 📜 Detailed Changelog
- 📥 Download Improved Skill
- 🌙 Modern Responsive UI
- 🔐 Gemini API Integration

---

# 🧠 Multi-Agent Architecture

The optimization workflow consists of **three specialized AI agents**.

| Agent | Responsibility |
|--------|---------------|
| 🟢 Executor | Runs the skill, generates test cases, evaluates outputs, and calculates scores |
| 🔵 Analyst | Diagnoses failures, identifies prompt weaknesses, and recommends improvement strategies |
| 🟣 Mutator | Applies one targeted modification to the prompt based on Analyst recommendations |

---

# 🔄 Optimization Workflow

```text
Upload Skill
      │
      ▼
Generate Test Scenarios
      │
      ▼
Run Skill
      │
      ▼
Evaluate Results
      │
      ▼
Analyze Failures
      │
      ▼
Improve Prompt
      │
      ▼
Re-test
      │
      ▼
Better Score?
   ┌──────┴──────┐
   │             │
  Yes            No
   │             │
Keep Change   Revert Change
      │
      ▼
Repeat Until Target Score
```

---

# 🏗️ Project Structure

```
self-improving-agent-skills/

│
├── backend/
│   ├── app.py
│   ├── adk_optimizer.py
│   ├── executor_agent.py
│   ├── analyst_agent.py
│   ├── mutator_agent.py
│   ├── requirements.txt
│   └── .env.example
│
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   ├── components/
│   │   └── lib/
│   ├── package.json
│   └── tailwind.config.ts
│
├── examples/
├── README.md
└── LICENSE
```

---

# ⚙️ Tech Stack

### Backend

- Python 3.10+
- FastAPI
- Google ADK
- Pydantic
- Uvicorn

### Frontend

- Next.js 15
- React 19
- Tailwind CSS v4
- TypeScript
- Recharts

### AI

- Google Gemini
- Google Agent Development Kit (ADK)

### Real-Time Communication

- Server-Sent Events (SSE)

---

# 🚀 Quick Start

## Clone Repository

```bash
git clone https://github.com/yourusername/self-improving-agent-skills.git

cd self-improving-agent-skills
```

---

## Backend Setup

```bash
cd backend

python -m venv venv

# Windows
venv\Scripts\activate

# Linux / macOS
source venv/bin/activate

pip install -r requirements.txt

cp .env.example .env
```

Add your Gemini API key:

```
GOOGLE_API_KEY=YOUR_API_KEY
```

Start the backend:

```bash
python app.py
```

Runs on:

```
http://localhost:8891
```

---

## Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

Runs on:

```
http://localhost:3000
```

---

# 📂 Skill Format

Skills follow the **agentskills.io** specification.

```
my-skill/

├── SKILL.md
├── scripts/
├── references/
└── assets/
```

Example:

```yaml
---
name: Example Skill
description: Example description
license: MIT

metadata:
  author: John Doe
  version: "1.0"
---

# Example Skill

Your prompt goes here...
```

---

# 📡 API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/api/upload` | Upload Skill |
| POST | `/api/analyze` | Generate Tests |
| POST | `/api/start/{id}` | Start Optimization |
| GET | `/api/stream/{id}` | Live Progress |
| POST | `/api/stop/{id}` | Stop Optimization |
| GET | `/api/download/{id}` | Download Skill |
| GET | `/api/examples` | Example Skills |
| GET | `/health` | Health Check |

---

# 📈 Optimization Loop

The optimization process follows an iterative cycle:

1. Upload Skill
2. Analyze Prompt
3. Generate Test Cases
4. Execute Skill
5. Evaluate Output
6. Detect Weaknesses
7. Improve Prompt
8. Re-run Evaluation
9. Keep Better Version
10. Repeat Until Target Score

---

# 📊 Performance Metrics

The platform tracks:

- Overall Pass Rate
- Failed Tests
- Successful Mutations
- Optimization Rounds
- Prompt Quality Score
- Execution Time
- Improvement Percentage

---

# 🔒 Configuration

### Upload Limits

- Maximum Upload Size: **10 MB**
- Maximum File Size: **1 MB**
- Maximum Files: **50**
- Supported Text Files:
  - .md
  - .txt
  - .json
  - .yaml
  - .py
  - .js
  - .ts

---

# 💡 Use Cases

- AI Prompt Optimization
- Agent Skill Evaluation
- Prompt Engineering
- Autonomous Prompt Improvement
- AI Agent Benchmarking
- Research Experiments
- LLM Workflow Testing

---

# 🛣️ Roadmap

- [ ] OpenAI Models
- [ ] Claude Support
- [ ] Local LLM Support
- [ ] Docker Deployment
- [ ] Kubernetes Support
- [ ] Team Collaboration
- [ ] Prompt Versioning
- [ ] Dashboard Analytics

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository

2. Create a feature branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Add feature"
```

4. Push to GitHub

```bash
git push origin feature-name
```

5. Open a Pull Request

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 🙌 Acknowledgements

- Google Agent Development Kit (ADK)
- Google Gemini
- FastAPI
- Next.js
- React
- Tailwind CSS
- Pydantic

---

## ⭐ Support

If you found this project useful, please consider giving it a **⭐ Star** on GitHub.

It helps the project reach more developers and encourages future improvements.

---

<div align="center">

### 🚀 Build Better AI Agents with Automated Prompt Optimization

**Made with ❤️ using Google ADK, Gemini, FastAPI & Next.js**

</div>
