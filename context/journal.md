# Journal – EBAB

## 2026-03-27 — Initial framing (Adrien B.)

**Goal**: Set up the project framework and prepare the bootstrap interview.

**What we did**:
- Reviewed the kickoff conversation between Adrien and Élie (2026-03-26 transcription).
- Retrieved Élie's LinkedIn profile for initial context.
- Clarified the project scope: AI literacy program, 100–120h over 4 weeks, hard deadline April 24.
- Defined the three-pillar approach: research, personal AI implementation, showcase micro-apps.
- Designed the bootstrap interview: objectives, output format (elie-profile.md), 7 axes of exploration.
- Created the full project structure (CLAUDE.md, context files, meetings/, output/, interview/).

**Important decisions**:
- Three-pillar structure (research + implementation + showcase) — balance TBD after interview.
- Bootstrap interview as prerequisite to roadmap definition.
- CLAUDE.md calibrated for pedagogical tone adapted to a finance professional with no AI background.

**Open questions**:
- **For Adrien**: Skills to define and repos to explore (Anthropic, community) — to discuss.
- **For Élie**: Bootstrap interview output will shape everything downstream.

**Next steps**:
- Finalize and review INTERVIEW-INSTRUCTIONS.md.
- Conduct bootstrap interview with Élie (Cowork session).
- Launch Deep Research on NBIM AI strategy and broader AI-in-finance landscape.
- Build detailed 4-week roadmap from interview + research outputs.

***

## 2026-03-28 — Bootstrap interview + DR socle + NotebookLM (Adrien B.)

**Goal**: Conduct Élie's bootstrap interview and generate first Deep Research report.

**What we did**:
- Conducted bootstrap interview with Élie in Cowork vocal mode (~30-45 min). Output: `context/references/elie_profile.md` — comprehensive profile covering trajectory, projections, relationship to tech/AI, learning style, interests, and calibration signals.
- Generated Deep Research report on generative AI fundamentals: `context/references/socle_gen-AI.md` — a pedagogical knowledge base covering core concepts (LLMs, transformers, prompting, RAG, agents, etc.).
- Set up NotebookLM as a learning tool for Élie: uploaded the DR report, configured for interactive learning (Audio Overview, Quiz, Flashcards, Learning Guide).
- Clarified phasing in vision.md: the 100–120h block is Phase 1 (exploration/experience), a launchpad for subsequent phases.
- Updated and expanded backlog with detailed, pedagogically-described items.

**Important decisions**:
- NotebookLM for knowledge acquisition (not for fund-specific research) — Élie uses it to absorb and test his understanding of AI fundamentals.
- Phase 1 framing: explicitly a beginning, not an end. Subsequent phases will emerge from what Élie discovers here.

***

## 2026-03-28 — Deep Research prompts (Élie B.)

**Goal**: Produce three calibrated Deep Research prompts to feed the research pillar of the program.

**What we did**:
- Conducted exploratory web research on NBIM AI strategy, Norwegian investment actors, and buy-side AI adoption globally.
- Key findings from exploration: NBIM is one of the most advanced institutional AI adopters globally (Investment Simulator, Claude for ESG screening, AI ambassador program, hiring freeze to focus on AI, $400M trading cost savings target, Strategy 2028 "all-in on AI"). The Norwegian broader landscape is less documented but includes Storebrand, DNB AM, Ferd, Canica, and a range of family offices managing $720B+ in the Nordics. The global buy-side AI landscape is rapidly maturing — by 2025 top funds are operationally reliant on AI, not just experimenting.
- Wrote three fully calibrated Deep Research prompts: (1) NBIM deep dive, (2) Norwegian investment actors landscape, (3) AI adoption in buy-side investment management globally.
- Prompts are saved in `output/`. Each includes: full context framing, detailed question sets organized by theme, output format specification, and a quality bar.

**Decisions**:
- Three-prompt structure validated: NBIM (depth) + Norway actors (landscape) + buy-side global (substance for AI fluency).
- Prompts calibrated for ChatGPT Deep Research or Perplexity Deep Research — either tool should work.

**Open questions**:
- **For Élie**: Which platform will you use to run the Deep Research? (ChatGPT Deep Research recommended for depth on NBIM and buy-side global; Perplexity useful for faster iteration on Norway actors)
- **For Adrien**: Review the three prompts — any adjustment to scope or framing before launch?

**Next steps**:
- Launch the 3 DR prompts and save outputs in `context/references/`
- Build the 4-week roadmap (can start a draft in parallel with DR, refine once results are in)

***

## 2026-03-28 — DR reports received + roadmap drafted (Adrien B.)

**Goal**: Integrate DR reports, research tooling options, draft the 4-week roadmap.

**What we did**:
- Received and indexed 3 Deep Research reports in `context/references/dr-reports/`:
  - DR1: NBIM AI Strategy Deep Dive — extremely detailed, covers Strategy 2028, Investment Simulator, vibe-coding culture, ESG screening, hiring freeze, talent expectations
  - DR2: Norwegian Investment AI Landscape — maps 15+ organizations (Storebrand, Ferd, Aker, Skagen, Sissener, Arctic, etc.) with AI maturity and analyst fit ratings
  - DR3: AI in Buy-Side Investment Management — global view of how AI is transforming the fundamental analyst workflow (screening, thesis construction, monitoring, portfolio construction)
- Researched NotebookLM podcast/tutorial features: Audio Overviews support multiple formats (Deep Dive, Brief, Critique, Debate), customizable focus areas, interactive mode (pause + ask questions), plus quiz/flashcards/Learning Guide
- Researched OpenClaw: open-source personal AI assistant, runs on Mac Mini 24/7, accessible via Telegram/iMessage/web. Install via terminal (`openclaw onboard`), supports MCP servers and custom skills. 13,000+ skills on ClawHub. Install best done with Claude Code (needs terminal access).
- Drafted comprehensive 4-week roadmap (`context/roadmap.md`):
  - Week 1: Foundations (NotebookLM socle IA + contexte finance, OpenClaw conception + install)
  - Week 2: Deepening + Design (advanced NotebookLM, OpenClaw skills/MCP, micro-app conception + first vibe-coding)
  - Week 3: Building (micro-app intensive, OpenClaw refinement, narrative prep)
  - Week 4: Consolidation (polish, dry-runs, Norway prep)

**Important decisions**:
- NotebookLM as primary learning tool for both IA fundamentals and finance context (2 separate notebooks)
- NotebookLM podcast episodes to be active learning (interactive mode, not passive listening)
- OpenClaw conception in Cowork, installation in Claude Code (needs terminal)
- OpenClaw and micro-app(s) in separate repos at same level as ebab (`framework/openclaw-elie/`, `framework/micro-app-elie/`)
- Micro-app(s) oriented "meta" — must demonstrate deep understanding to interlocutors (NBIM etc.), not just solve a personal pain point
- Micro-app conception week 2, build weeks 2-3, polish week 4

**Next steps**:
- Sunday 29: Élie's first full day — NotebookLM setup + OpenClaw conception + install
- Review roadmap with Élie and adjust as needed
- Guide Élie through NotebookLM podcast generation and interactive learning

***
