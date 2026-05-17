# Nexus — Causal Intelligence Platform

🚀 **Live Deployment:** [View the Final Project Dashboard Here](https://nexus-frontend-teal.vercel.app/?repo=https%3A%2F%2Fgithub.com%2FAnshumaan1254%2FARKA.git&window=1year)

> **Nexus is the first software comprehension platform built on a formal computational model of organizational causality.**

While other AI coding tools compete on velocity (how fast to write the next line of code), Nexus competes on **comprehension** — making the invisible causal chains inside a codebase visible, queryable, and actionable.

**Nexus uncovers the silent architectural debt in your system: when an assumption made in 2021 silently breaks in 2026.**

---

## 🌟 Exclusively Powered by BOB by IBM

**This project is fundamentally impossible to build or run with any other AI on the market.** 

Nexus requires **BOB by IBM** to function. Standard file-level AI coding assistants or chat interfaces (like standard Gemini or Claude wrappers) fail entirely at this scale because they lack what Bob provides natively:

1. **Full-Repository Context Awareness:** Causal tracing requires understanding semantic relationships between components that don't share keywords, don't call each other directly, and exist in completely different files written years apart. A database decision in 2020 constrains a mobile app's pagination design in 2025. **Only BOB by IBM can ingest and comprehend the entire repository simultaneously.**
2. **Multi-Step Agentic Orchestration:** BOB acts as the master orchestrator, orchestrating layers of reasoning across thousands of commits, PRs, and architectural decisions seamlessly.
3. **Enterprise-Grade Analysis:** Bob's powerful processing engine safely handles the massive context required to trace architectural dependencies without hallucinating context or losing state.

*Full repository context is not just a feature of Bob. It IS Bob. Nexus is the application that finally deserves it.*

---

## 🚀 The Five Layers of Nexus

Nexus processes codebases through five distinct architectural layers:

1. **Decision Provenance Engine (Layer 1)**
   - *Engine:* **BOB by IBM** (Primary)
   - *Function:* Ingests the entire repository, all git history, GitHub/Jira issues, PR descriptions, and Confluence docs to extract structured Decision Provenance Records (DPRs).
2. **Causal Temporal Graph [CTG] (Layer 2)**
   - *Engine:* **BOB by IBM** (Primary)
   - *Function:* Converts DPRs into nodes in a Directed Acyclic Graph (DAG) with time as a structural dimension.
3. **Assumption Decay Monitor (Layer 3)**
   - *Engine:* **BOB by IBM** (Continuous Monitoring)
   - *Function:* Classifies and monitors assumptions (quantitative, environmental, dependency, team). Nightly runs verify if historical assumptions still hold against the live repository state.
4. **Counterfactual Simulation Engine (Layer 4)**
   - *Engine:* **BOB by IBM Orchestration** (Deep Reasoning)
   - *Function:* Given the CTG, Bob reasons over alternative decision timelines ("What if we used 16KB pages instead of 8KB?").
5. **Organizational Risk Forecast (Layer 5)**
   - *Engine:* **BOB by IBM Orchestration** (Semantic Analysis)
   - *Function:* Knowledge concentration analysis. Generates reports indicating SPOFs (Single Points of Failure) like: *"Engineer X holds 73% of causal knowledge about auth — their departure is a critical SPOF."*

---

## 🛠️ Tech Stack

- **Core AI Orchestrator:** IBM Bob IDE (Essential for L1-L3 Full Repo Ingestion)
- **Deep Reasoning Engine:** BOB by IBM's underlying LLM integrations (gemini-2.5-flash / claude)
- **Graph Database:** Neo4j Community (CTG Storage)
- **Backend:** Python (FastAPI, NetworkX, GitPython, PyDriller)
- **Frontend:** React + Vite + Tailwind CSS (Single-file no-backend UI reading from `nexus_data.json`)

---

## 🧠 Theoretical Foundations

Nexus is built on advanced academic principles:
- **Distributed Cognition (Hutchins, 1995):** A software organization is a distributed cognitive system. The codebase and git history are its external cognitive artifacts.
- **Causal Inference (Pearl, 2009):** Nexus applies true causal reasoning (not statistical correlation) to software organizational data.
- **Invariant Inference (Daikon, Ernst et al., 2007):** Nexus performs semantic invariant detection on architectural decisions, detecting when the invariants assumed at decision time no longer hold.

---

## ⚙️ Getting Started

### Prerequisites
- You **MUST** have access to the **IBM Bob IDE** to run the ingestion pipeline.
- Python 3.10+
- Node.js 18+

### Running the Project
1. **Analyze the Repository:** Let BOB by IBM ingest the repository and run the extractor.
   ```bash
   cd nexus_layer2
   python submission/repo_analyzer.py https://github.com/your-org/your-repo --window 1year
   ```
2. **Start the API Server:**
   ```bash
   python submission/api.py
   ```
3. **Launch the Dashboard:**
   ```bash
   cd nexus-frontend
   npm install
   npm run dev
   ```

---
*Created for the IBM Bob Hackathon. Demonstrating the absolute superiority of Bob's full-repository context and multi-agent orchestration.*
