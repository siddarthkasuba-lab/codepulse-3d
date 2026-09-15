# CodePulse — 3D Codebase Intelligence

> **Don't search your codebase. Understand it.**

CodePulse is a developer-focused codebase intelligence concept that turns a repository into a visual, explorable architecture map. Instead of jumping between files and search results, developers can explore relationships, ask natural-language questions, inspect code evidence, and understand the likely impact of a change before editing the code.

## 🚀 Live Demo

**Web demo:** https://codepulse-3d.hatchable.site

## 🎯 The Problem

Large codebases become difficult to understand because important behavior is distributed across many files and functions. Traditional search tells you where text appears, but it does not give you a clear mental model of how the system is connected.

This creates three common problems:

- Slow onboarding for new developers
- Hidden dependencies between functions and modules
- Risky changes caused by an unclear impact radius

## 💡 Our Solution

CodePulse combines a visual codebase map with intelligent code retrieval and impact analysis.

The experience is centered around a **3D architecture graph** where developers can move from repository → module → function → dependency → evidence.

### ⭐ Standout Feature: Change Impact Simulator

Select a function or symbol and simulate a change before making it.

CodePulse can visualize:

- Direct dependents
- Affected files/modules
- Dependency paths
- Potential risk areas
- Evidence explaining why an area may be impacted

The goal is to answer a practical developer question:

> **“What could break if I change this?”**

## ✨ Key Features

- **3D Codebase Map** — Explore repository structure as an interactive graph.
- **Function-Level Exploration** — Drill down from files and modules to important symbols.
- **Natural-Language Code Q&A** — Ask questions about how the codebase works.
- **Evidence-First Answers** — Connect responses back to relevant source locations.
- **Change Impact Simulation** — Visualize the potential blast radius of a change.
- **Developer Onboarding** — Use the architecture map to build a mental model faster.
- **Git-Aware Roadmap** — Planned support for reasoning over code evolution and history.

## 🧠 What Makes CodePulse Different?

Codebase RAG and code search tools already exist. CodePulse focuses on the **developer interaction layer**: connecting intelligent retrieval directly to a visual architecture model and a pre-change impact experience.

The key idea is simple:

**Search gives you results. CodePulse aims to give you understanding.**

## 🏗️ Architecture

```text
                    ┌─────────────────────┐
                    │      Developer      │
                    └──────────┬──────────┘
                               │
                    ┌──────────▼──────────┐
                    │   CodePulse UI      │
                    │  3D Architecture    │
                    │      Explorer       │
                    └──────────┬──────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
       ┌──────▼──────┐  ┌──────▼──────┐  ┌──────▼──────┐
       │ Code Parser │  │ Vector/RAG  │  │ Dependency  │
       │   & Chunks  │  │  Retrieval  │  │    Graph    │
       └──────┬──────┘  └──────┬──────┘  └──────┬──────┘
              │                │                │
              └────────────────┼────────────────┘
                               │
                    ┌──────────▼──────────┐
                    │ Impact Analysis +   │
                    │ Evidence Generation │
                    └─────────────────────┘
```

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **3D Visualization:** Three.js
- **AI / Code Intelligence:** LLM + embeddings / RAG architecture
- **Code Intelligence:** Function/class parsing and relationship analysis
- **Model Option:** Qwen Coder via Ollama for local development
- **Repository Integration:** GitHub
- **Deployment / Prototype Hosting:** Hatchable

## 🖥️ Prototype Status

The current public demo focuses on the **visual interaction and product experience** for CodePulse. The full production architecture can be extended with real repository ingestion, embeddings, vector retrieval, dependency extraction, and AI-generated evidence-backed answers.

This keeps the hackathon prototype fast while preserving a clear path toward a production developer tool.

## 🔥 Demo Flow

1. Open the CodePulse dashboard.
2. Explore the 3D repository architecture.
3. Select a function/module.
4. Inspect connected dependencies.
5. Trigger **Change Impact**.
6. Review the affected areas and reasoning.

## 📈 Roadmap

### Phase 1 — Hackathon MVP

- [x] 3D architecture experience
- [x] Developer-focused dashboard
- [x] Impact simulation concept
- [x] GitHub project repository

### Phase 2 — Intelligent Backend

- [ ] Repository ingestion
- [ ] AST/function-level chunking
- [ ] Embeddings + vector retrieval
- [ ] Dependency graph extraction
- [ ] Evidence-backed code Q&A

### Phase 3 — Advanced Intelligence

- [ ] Git history reasoning
- [ ] Pull-request impact analysis
- [ ] Automated architecture summaries
- [ ] Onboarding missions for unfamiliar repositories
- [ ] Risk scoring for proposed changes

## 📁 Project Structure

```text
codepulse-3d/
├── public/
│   └── index.html
├── README.md
└── ...
```

## 🏆 Hackathon Pitch

> **CodePulse is a 3D codebase intelligence layer that helps developers understand a repository before they change it — combining visual architecture, intelligent retrieval, and change-impact analysis in one experience.**

## 📄 License

This project is currently intended as a hackathon/prototype project. Add a license before using it as a public production library.

---

Built with ❤️ for the next generation of developer tools.
