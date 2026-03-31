# Deep Research Prompt — OpenClaw & Agentic AI Assistants

*À lancer dans ChatGPT Deep Research ou Perplexity. Output à sauvegarder dans `context/references/` et à uploader dans un notebook NotebookLM dédié.*

---

## PROMPT

I am building a personal AI literacy program and want to deeply understand a category of tool called "personal AI agents" — specifically through the lens of OpenClaw, a personal AI assistant framework I am actively using. I need a well-structured research document that will serve as the primary source for a NotebookLM notebook, so it should be comprehensive, educational, and clearly structured.

Please cover the following:

---

### 1. What is a personal AI agent — and how is it different from a chatbot?

- Define the core distinction: a chatbot responds to queries; an agent acts autonomously, monitors, decides, and delivers outputs without being prompted each time
- Explain the key architectural concepts: tools, skills, memory, channels, cron jobs, triggers
- What makes something "agentic" vs. just "automated"? Where is the intelligence?
- Explain the concept of a "gateway" — a persistent process that runs 24/7 and orchestrates agents
- Use concrete analogies: an agent is like a junior analyst you've briefed once and who sends you updates every morning without being asked again

---

### 2. OpenClaw specifically — architecture and capabilities

*Note: OpenClaw is a personal AI assistant framework. Research what is publicly known about it, its design philosophy, and how it compares to similar tools.*

- What is OpenClaw? Who built it, what is its design philosophy?
- Core architecture: gateway, agents, skills, channels (Telegram, etc.), cron jobs, blogwatcher
- What is a "skill" in OpenClaw? How does it differ from a prompt or a tool?
- What is "blogwatcher"? How does feed monitoring and RSS ingestion work?
- How does OpenClaw handle authentication, security, and multi-device pairing?
- What is the difference between running OpenClaw locally (Mac) vs. on a VPS? What does "24/7 uptime" actually mean in practice?
- How does OpenClaw relate to Claude Code and MCP (Model Context Protocol)?

---

### 3. The broader landscape — similar tools and approaches

- What other personal AI agent frameworks exist? (e.g., Open Interpreter, Auto-GPT, similar tools)
- How do personal agents differ from enterprise agent platforms?
- What is the "agentic stack" in 2025-2026 — what layers make up a complete agentic system? (LLM, tools, memory, orchestration, channels)
- What is MCP (Model Context Protocol) and why does it matter for connecting agents to external data sources?
- What are "skills" in the broader agentic ecosystem — how do Claude Code skills, OpenClaw skills, and LLM tool use relate to each other?

---

### 4. Use cases — what can a personal agent actually do that a chatbot cannot?

Focus on **investment and finance professional use cases** specifically:
- Autonomous daily briefings (news monitoring, synthesis, delivery)
- Job market monitoring (automated scanning of postings against a profile)
- Company/sector monitoring (RSS, filings, local-language sources)
- Research assistance (RAG over a document corpus, structured extraction)
- Portfolio diary / investment log with scheduled reminders
- Red-teaming / adversarial sessions (scheduled thesis challenges)
- What are the limits? What can agents not do reliably yet?

---

### 5. The "create vs automate" distinction

This is conceptually the most important section.

- What is the difference between using AI to automate an existing process vs. using AI to create a new process that didn't exist before?
- Give concrete examples of each in an investment context
- Why does this distinction matter for how professionals should think about AI adoption?
- What does "augmented analyst" mean in practice — what new analytical moves become possible with agents that were impossible before?
- How do leading asset managers (NBIM, Two Sigma, Bridgewater, etc.) think about this distinction publicly?

---

### Output format

Please structure the output as a well-organised document with clear headers, concrete examples, and analogies where helpful. Aim for depth over breadth — this will be used as a study source, not a summary. Target length: 2,000–3,000 words. Avoid lists of bullet points where prose would be clearer.

---

*Prompt créé le 2026-03-31. Usage : Deep Research → sauvegarder output dans `context/references/dr-openclaw-agents.md` → uploader dans NotebookLM notebook "OpenClaw & Agentic AI".*
