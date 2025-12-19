# 🚀 Beginner Research Automation (n8n + Local LLM)

A **demo-phase AI research automation** built with **n8n**, designed to convert a single topic into structured research using **live web data + local LLMs**.

This project focuses on **learning, experimentation, and practical automation** — not hype.

---

### 🖼️ Automation Workflow
![Workflow Screenshot](screenshots/n8n-beginner-research-automation.png)
![mailed Screenshot](screenshots/mailed_research.png)

## 🔧 What This Automation Does

This workflow automates the full research lifecycle:

- Accepts a topic from **Airtable**
- Fetches live web data using **Tavily API**
- Uses an **n8n AI Agent** with **Ollama (local LLM)**
- Generates structured research content:
  - Abstract
  - Introduction
  - Key Findings
  - Conclusion
  - References
- Formats output (Markdown → HTML)
- Saves results back to Airtable
- Sends the final research via **Gmail**
- Updates topic status automatically (pending → completed)

---

## 🧠 Why Local LLM?

- No API limits
- Lower cost
- Full data privacy
- Ideal for experimentation & learning
- No vendor lock-in

---

## 🛠 Tech Stack

- **n8n** (Self-hosted)
- **Airtable** (Topic & status tracking)
- **Tavily Search API** (Live web research)
- **Ollama** (Local LLM)
- **Gmail Node**
- **Markdown → HTML**

---
## 📁 Folder Structure

```
n8n-beginner-research-automation/
│
├── workflows/
│   └── beginner-research-workflow.json
│
├── screenshots/
│   ├── workflow-overview.png
│   ├── airtable-input.png
│   ├── ai-agent-node.png
│   └── email-output.png
│
├── prompt/
│   |─ agent_prompt.md
├── .env.example
├── .gitignore
├── LICENSE
└── README.md
```

### 📌 Folder Purpose

* **workflows/** → n8n exported workflow JSON files
* **screenshots/** → Visual previews of the workflow & outputs
* **docs/** → Architecture explanation and setup instructions
* **.env.example** → Environment variable template (no secrets)
* **README.md** → Project overview and usage guide


---

## ⚙️ Setup Overview

1. Self-host **n8n**
2. Configure **Airtable** table with:
   - Topic
   - Status (pending / completed)
3. Add **Tavily API key**
4. Run **Ollama** locally
5. Import the workflow JSON into n8n
6. Update credentials & environment variables

> ⚠️ Never commit secrets. Use `.env` files only.

---

## 🚧 Project Status

**Demo / Experimental Phase**

This workflow is built for:
- Learning automation
- Exploring AI agents
- Testing local LLM pipelines

Expect changes and improvements.

---

## 🎯 Use Cases

- Beginner research assistant
- Content research automation
- Teaching & learning workflows
- Knowledge drafting tool

---

## 🤝 Connect

If you’re working with **n8n, AI workflows, automation, or local LLMs**, feel free to connect.

🔗 This project is also featured on my **LinkedIn Projects section**.

