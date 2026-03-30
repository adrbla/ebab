# Decisions – EBAB

## 2026-03-27 – Project structure and approach

**Context**: Initial framing session in Cowork (Adrien). Élie is a finance professional with no AI/tech background beyond daily chatbot use. He's preparing for a career move to Norway with a hard deadline of April 24.

**Decision**: Structure the project around three pillars: (1) research on AI in finance, (2) personal AI tool implementation (agentic workflows, monitoring), (3) one or more showcase micro-applications. The balance between these will be calibrated after the bootstrap interview with Élie.

**Rejected alternatives**: Pure research-only track (not enough hands-on credibility), pure coding bootcamp (too far from Élie's starting point and professional context), off-the-shelf course (too generic, doesn't leverage Élie's finance expertise).

**Consequences**: Need to front-load research (weeks 1–2) to inform what tools and applications to build (weeks 2–4). The bootstrap interview is critical to calibrate the split.

***

## 2026-03-27 – Bootstrap interview before roadmap

**Context**: Need to deeply understand Élie's starting point, motivations, learning style, and projections to calibrate the roadmap properly.

**Decision**: Conduct a dedicated interview session in Cowork (30–45 min) with structured instructions. Output: `elie-profile.md` which becomes the foundational context document for all subsequent Claude Code sessions.

**Rejected alternatives**: Skip interview and start from assumptions based on LinkedIn profile (insufficient depth), have Élie fill a questionnaire (too rigid, misses nuance and follow-up).

**Consequences**: The interview must happen before the first working session. Everything downstream depends on its quality.

***

## 2026-03-28 – NotebookLM as primary learning tool

**Context**: Need an active (not passive) learning method adapted to Élie's learning style (dialogue, hands-on, trial and error). Traditional reading or watching videos would not fit.

**Decision**: Use NotebookLM with 2 separate notebooks ("Socle IA" from DR socle, "AI & Finance" from 3 DR reports). Learning via interactive podcasts (Audio Overviews with pause/question mode), quiz, flashcards, and Learning Guide. Podcasts are active learning tools — Élie interrupts, asks questions, digs deeper.

**Rejected alternatives**: Pure reading of DR reports (too passive for Élie's learning style), generic online courses (too slow, not calibrated to his finance context), Claude chat only (less structured for knowledge retention).

**Consequences**: NotebookLM becomes the knowledge absorption backbone for weeks 1-2. The interactive podcast approach should fit Élie's preference for dialogue-based learning.

***

## 2026-03-28 – OpenClaw: conception in Cowork, install in Claude Code

**Context**: OpenClaw requires terminal access for installation (`openclaw onboard`) and configuration (skills, MCP servers). Cowork can guide but can't execute terminal commands.

**Decision**: Design the OpenClaw setup (what sources, what agents, what channels) with Adrien in Cowork, then install and configure in Claude Code. Each major component (OpenClaw, micro-app) gets its own repo at `framework/` level alongside ebab.

**Rejected alternatives**: Install in Cowork (not possible — no terminal execution), install without prior design (would lead to generic uncalibrated setup).

**Consequences**: Sunday 29 afternoon: conception session in Cowork → `output/openclaw-design.md`, then Claude Code session for install. Separate repos keep things clean.

***

## 2026-03-28 – Micro-app(s) oriented "meta", not personal pain point

**Context**: The micro-app must serve as a showcase for potential employers (NBIM and others). It must demonstrate genuine understanding of how AI transforms investment, not just surface-level automation.

**Decision**: Micro-app conception grounded in DR findings. Must "speak" to interlocutors — show understanding of real use cases, not generic AI application. 1 app or 3 smaller ones — to be decided with Élie based on DR insights. Conception week 2 (after knowledge foundation is solid), build weeks 2-3, polish week 4.

**Rejected alternatives**: Personal productivity tool (wouldn't demonstrate finance+AI understanding to interlocutors), generic AI demo (too superficial), premature build before research is absorbed (would lack depth).

**Consequences**: Need DR insights fully absorbed before conception session. The micro-app brief (`output/micro-app-design.md`) must articulate what it demonstrates and to whom.

***

## 2026-03-28 – Repos on Élie's GitHub, framework from CLAUDE-CW.md

**Context**: Need separate repos for OpenClaw and micro-app(s), at same level as ebab. Can't nest git repos. Need to decide who owns the repos and how to structure them.

**Decision**: Repos created on Élie's GitHub account (not adrbla). Adrien added as collaborator. Each repo gets the full "framework" structure based on CLAUDE-CW.md code project template: CLAUDE.md, DEVS.md, context/ (vision, backlog, decisions, journal, tech-stack, references/). Claude (in Cowork) guides Élie through repo creation and generates the framework files.

**Rejected alternatives**: Creating repos on adrbla's account (doesn't reflect Élie's ownership/portfolio), skipping the framework structure (would lose persistence and workflow benefits).

**Consequences**: Élie needs `gh` CLI authenticated on his Mac. Desktop Commander needed in Cowork to execute git operations. Framework generation happens at repo creation time (OpenClaw: Sunday 29, micro-app: week 2).

***

## 2026-03-30 – Déployer OpenClaw sur VPS Hetzner (pas Mac Mini)

**Context**: Le briefing quotidien du 2026-03-30 n'a pas été envoyé sur Telegram parce que le Mac Mini d'Élie était éteint. Un assistant AI qui dépend d'une machine allumée 24/7 n'est pas fiable.

**Decision**: Migrer OpenClaw sur un VPS Hetzner CX23 (2 vCPU, 4GB RAM, 40GB SSD, cost-optimized). Adrien prépare un domaine et mappe un sous-domaine. Déploiement prévu le 2026-03-30 au soir.

**Rejected alternatives**: Garder sur Mac Mini (pas fiable — dépend de l'uptime de la machine d'Élie), VPS plus gros (surdimensionné pour OpenClaw).

**Consequences**: OpenClaw tourne 24/7 indépendamment du Mac d'Élie. Le briefing quotidien devient fiable. Le repo `openclaw-elie/` devra être adapté pour refléter le déploiement distant.

***
