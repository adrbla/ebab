# OpenClaw — Design Brief (Élie Blaise)

*Prepared in Cowork — 2026-03-29. Implementation in Claude Code.*

---

## What is OpenClaw

OpenClaw is an open-source personal AI assistant that runs locally on Élie's Mac Mini 24/7. It connects to Telegram (and potentially iMessage later) and responds to natural language requests. It can browse the web, read files, run scripts, and call external APIs.

Think of it as a personal analyst that's always on — you send a message from your phone, it does the work and sends back a synthesis.

- **Provider**: Anthropic (Claude)
- **Primary channel**: Telegram
- **Runs on**: Mac Mini (macOS 15+)
- **Install**: `npm install -g openclaw@latest` → `openclaw onboard`
- **Repo**: `framework/openclaw-elie/`

---

## The 6 Core Capabilities

### 1. Veille NBIM
Monitor everything NBIM publishes or that is written about them.

**Sources to monitor**:
- nbim.no (news, publications, annual reports, strategy documents)
- nbim.no/en/about-us/career/vacancies/ (job postings)
- Top1000funds.com (NBIM coverage)
- Financial press (FT, Bloomberg, CNBC) — NBIM-tagged articles
- NordSip, Investment Magazine AU (specialist coverage)

**Trigger**: Daily or on new publication. Alert Élie via Telegram when something significant drops.

**Output format**: 3-4 sentence synthesis + link. Flag if it's about: AI strategy, hiring, investment process changes, leadership statements.

---

### 2. Veille acteurs norvégiens
Monitor the Norwegian investment ecosystem beyond NBIM.

**Organizations to track**:
- Storebrand Asset Management
- DNB Asset Management
- Ferd (Johan H. Andresen)
- Canica (Stein Erik Hagen)
- Kistefos
- Aker / Aker Capital
- Arctic Securities / Arctic Fund Management
- Skagen Funds
- Holberg Funds
- KLP

**Focus**: AI adoption signals, hiring signals, investment mandate changes, notable transactions.

**Output format**: Weekly digest or instant alert on major news.

---

### 3. Veille AI buy-side (global)
Track the evolution of AI in investment management globally.

**Sources**:
- Top1000funds.com
- Institutional Investor
- The Hedge Fund Journal
- AlphaSense blog
- Resonanz Capital insights
- Key AI/finance newsletters and research

**Focus**: New tools, real adoption cases (not hype), named fund examples, what's becoming table stakes for analysts.

**Output format**: Weekly digest — top 5 developments, with one-liner commentary on why it matters.

---

### 4. Briefing quotidien
Every morning at 07:30 (or configurable time), Élie receives a Telegram message synthesizing the overnight signals from capabilities 1, 2, and 3.

**Format**:
```
☀️ Morning Brief — [date]

📌 NBIM: [1-2 lines if anything new, else "nothing significant"]
🇳🇴 Norway: [1-2 lines on Norwegian actors]
🤖 AI buy-side: [1-2 lines on key trend]
💼 Jobs: [new relevant postings if any]

---
Full digests available on request.
```

**Tone**: Analyst-to-analyst, no fluff. If nothing significant, say so clearly.

---

### 5. Veille job postings norvégiens
Monitor investment roles open in Norway — calibrated for Élie's profile.

**Sources**:
- finn.no (Norway's primary job board)
- LinkedIn — filtered: Norway + investment + [specific keywords]
- NBIM careers page (nbim.no/en/about-us/career/vacancies/)
- Storebrand, Ferd, Canica, Arctic, Skagen, KLP career pages

**Role types to track**:
- Analyst / Senior Analyst (public equities, equity research)
- Portfolio Manager / Investment Manager
- Family office investment roles
- PE / Private Equity (Norway-based)
- Any role mentioning AI + investment in combination

**Filter logic**: Norway-based, investment-focused, senior enough for Élie's profile (5+ years implied). Exclude operations, admin, IT (unless AI+investment).

**Output**: Instant Telegram alert when a new relevant posting is detected. Include: role title, organization, brief summary, link.

---

### 6. Stock Initial Take
*The analytical centerpiece. Give the agent a ticker → it returns an initial take on the stock calibrated to Élie's investment philosophy.*

**Input**: A ticker symbol (e.g. `AKER.OL`, `EQNR.OL`, `INVE-B.ST`)

**Data pulled automatically**:
- Company fundamentals (revenue, margins, ROIC, balance sheet, valuation multiples)
- Recent news (last 30 days)
- Latest earnings transcript or most recent investor presentation
- Recent analyst consensus (if available)
- Key regulatory filings (annual report, most recent quarterly)

**Output structure** (calibrated to Élie's investment philosophy — see `context/references/elie_profile.md`):

```
📊 INITIAL TAKE — [TICKER] — [Company Name]
Generated: [date]

1. BUSINESS IN ONE PARAGRAPH
   What does this company actually do? Competitive position, moat, end markets.
   What makes it structurally interesting (or not)?

2. KEY VALUE DRIVERS
   The 3-4 variables that will determine whether this investment works.
   What KPIs matter most? What are the inflection points to watch?

3. MARKET NARRATIVE vs. POTENTIAL PERCEPTION GAP
   What does the market currently think about this name?
   Where might the narrative be wrong, incomplete, or behind?
   Is there a dislocation between price and perception?

4. BULL / BASE / BEAR
   Bull: [key assumption + implied return]
   Base: [key assumption + implied return]
   Bear: [key assumption + downside]

5. CONVICTION THRESHOLD
   What would need to be true to reach high conviction?
   What's the key risk to the thesis?

6. PRIORITY QUESTIONS (3-5)
   The questions Élie should answer before forming a view.
   Ordered by importance.

⚠️ This is a first-pass primer, not a recommendation.
```

**Philosophy calibration** (from Élie's profile):
- Focus on **holistic perception shifts**, not single KPIs
- Look for **underfollowed or misunderstood** names
- Emphasize **variant perception** — where does the market have it wrong?
- Structure for **decision closure** — the output should help move from "interesting" to "conviction or pass"
- Avoid flooding with data — identify *which variables matter*, not all variables

---

## Skills & MCP Servers Required

| Capability | Tools needed |
|-----------|--------------|
| Veille NBIM | Web search, RSS feed reader, HTTP fetch |
| Veille Norway actors | Web search, RSS feed reader, HTTP fetch |
| Veille AI buy-side | Web search, RSS feed reader |
| Briefing quotidien | Scheduler (cron), Telegram bot |
| Job postings veille | Web scraper (finn.no, LinkedIn), HTTP fetch, career page monitors |
| Stock initial take | Financial data API (Yahoo Finance / Alpha Vantage / FMP), news search, filing fetcher (SEC/Euronext), earnings transcript source |

**MCP servers to configure**:
- `@modelcontextprotocol/server-fetch` — HTTP fetch for web pages
- `@modelcontextprotocol/server-brave-search` or equivalent — web search
- Financial data MCP (to define during Claude Code session — evaluate options)
- Telegram integration (built into OpenClaw via Bot API)
- Scheduler (OpenClaw built-in or cron)

---

## Phased Rollout

| Phase | What gets built | When |
|-------|----------------|------|
| Phase 1 (Week 1) | OpenClaw installed + Telegram connected + capabilities 1-4 (veille + briefing) | Friday April 4 |
| Phase 2 (Week 2) | Job postings veille (#5) + skills refinement | Weekend April 5-6 |
| Phase 3 (Week 2-3) | Stock initial take (#6) — first version | April 7-13 |
| Phase 4 (Week 3) | Stock initial take refinement + custom skills | April 12-13 |

---

## Open Questions for Claude Code Session

- Which financial data API to use for the stock initial take? (Yahoo Finance free vs. Alpha Vantage vs. Financial Modeling Prep — evaluate cost/coverage/ease)
- How to handle earnings transcripts? (Seeking Alpha scraping vs. dedicated transcript API)
- finn.no scraping — does it have an API or is direct scraping needed?
- LinkedIn job monitoring — which approach works without API access?
- How to handle non-English sources (Norwegian press)?

---

*This document is the brief for the Claude Code installation session. Implementation starts in `framework/openclaw-elie/`.*
*Last updated: 2026-03-29*
