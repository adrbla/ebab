# Backlog – EBAB

## Completed
- [x] Bootstrap interview avec Élie (Cowork session → elie-profile.md) — 2026-03-28
- [x] Prepare calibrated Deep Research prompts (3) — 2026-03-28
- [x] Launch DR prompts and receive reports — 2026-03-28, saved in `context/references/dr-reports/`
- [x] Define the 4-week roadmap — 2026-03-28, see `context/roadmap.md`
- [x] Install Desktop Commander MCP server — 2026-03-29
- [x] Set up NotebookLM (2 notebooks: "Socle IA" + "AI & Finance / The Augmented Analyst") — 2026-03-29
- [x] Conceive OpenClaw setup → `output/openclaw-design.md` — 2026-03-29
- [x] Install OpenClaw on Mac Mini + Telegram + repo `framework/openclaw-elie/` — 2026-03-29
- [x] Install cc-openclaw (9 slash commands Claude Code) — 2026-03-29
- [x] Configure OpenClaw capabilities 1-4 (18 feeds RSS, cron 07h30 Oslo) — 2026-03-29
- [x] Explore finn.no — calibrate keywords for OpenClaw skill #5 — 2026-03-29
- [x] Provisionner VPS Hetzner elibla (178.104.112.7) + Node.js — 2026-03-30
- [x] Déployer OpenClaw sur VPS + DNS oc.elibla.com + HTTPS Caddy — 2026-03-30
- [x] Préparer NBIM call prep — voice prompt + DR prompt + call brief final — 2026-03-31

## Now (cette semaine — 31 mars au 4 avril)

**Après pull** : réintégrer le journal de la session brouillons de mails Oslo (fichier généré dans une autre session Cowork, non pushé). L'ajouter au repo et le commiter.

**Revoir et ajuster la roadmap avec Claude** en équilibrant les 3 axes ci-dessous.

### Axe 1 — Connaissances générales (NotebookLM)
- [ ] Écouter podcast "AI & Finance" en mode interactif (pauses + questions)
- [ ] Faire quiz DR1/DR2/DR3 (difficile) + réviser avec les fiches
- [ ] Enrichir le Notebook "Socle IA" : ajouter des sources, générer de nouveaux épisodes thématiques
- [x] Lancer DR OpenClaw — sauvegardé dans `context/references/dr-openclaw-agents.md` — 2026-03-31
- [x] Créer notebook NotebookLM "OpenClaw & Agentic AI" avec output DR — 2026-03-31
- [ ] À la fin de chaque session interactive NotebookLM : générer une synthèse, la sauvegarder en markdown dans `context/references/` pour suivre la progression

### Axe 2 — Pratique
**OpenClaw** :
- [x] Régler le problème d'erreur API limit/rate sur le VPS — haiku model + --silent flag — 2026-03-31
- [x] Valider briefing Telegram VPS (premier briefing de production) — 12s, 357-621 tokens ✅ — 2026-03-31
- [ ] Creuser OpenClaw en général : comprendre l'architecture, les tools, les skills — le notebook NotebookLM dédié aide ici
- [ ] OpenClaw capability #5 (job postings finn.no)
- [ ] OpenClaw capability #6 (stock initial take) — choisir API financière

**Skills Claude Code** :
- [ ] Concevoir et implémenter 1 ou plusieurs skills custom avec Claude (dans Cowork) — exercice meta : comprendre ce qu'est un skill en en créant un. Le skill doit être spécifique (pas générique), placé au bon endroit pour être mobilisable par Claude.

**Showcase app(s)** :
- [ ] Session voice brainstorm — brief dans `output/voice-brainstorm-brief-showcase-app.md`. Explorer, ouvrir, NE PAS fermer.
- [ ] Après le brainstorm : session d'atterrissage/sélection (avec Adrien). NB : pas forcément une seule app — ça peut être 3 micro-apps (dont une plus importante), ce qui fait 3 repos / sessions de vibe-coding distinctes. À voir.

### Axe 3 — Contacts Oslo
- [x] Envoyer email à ami NBIM (adresse email Élie → transmission à HR) — 2026-03-31
- [x] CV polished — AI bullet rewritten (architectural), Technical tools updated, source of truth Google Docs "CV ELIE BLAISE - APR-26" — 2026-04-01
- [x] Email HR NBIM (Kristin Birkeland) envoyé — intro via Christian, court et direct, CV en PJ — 2026-04-01
- [ ] (Optionnel) Deep Research active equity team NBIM — prompt dans `output/nbim-call-prep-voice-prompt.md`
- [ ] Call HR NBIM — call brief final prêt dans `output/nbim-call-brief-final.md`, mentionner Oslo semaine du 23-27 avril pendant le call
- [ ] Suivre l'avancement des contacts Oslo avec Élie (point régulier)

### CV annexes (PPT pages)
Brief complet dans `context/references/track-record-ai-page-brief.md`
- [ ] Track record page (PPT) — "Selected Investment Track Record" : chart Elie Ideas vs MSCI World (equal-weighted), key stats, 2–3 case studies. **Bloqué** : entry dates + returns à fournir par Élie (WDC, DSV, SigmaRoc, Arcosa, Fielmann)
- [ ] AI workflows page (PPT) — "Applied AI – Real Workflows in Investment Process" : 3 workflows avec screenshots réels (Idea Screening, Earnings Call Decomp, Variant View Builder). Build avec WDC / SKF ou autre idée réelle.

### Interview prep infrastructure (quick setup)
- [x] Renommer/reconfigurer le projet GPT "NBIM Interview Prep" → **"Interview Prep"** (générique) — 2026-03-31
  - Instructions génériques : "At the start of each session, I'll specify which institution and role. Read the relevant context file and adopt the appropriate coaching setup."
  - Sources à uploader au fur et à mesure : un context file par institution (NBIM, DNB AM, Storebrand, Ascender…)
  - Le call brief NBIM existant devient le premier context file institution-specific

## Next (week 2 — week-end 5-6 avril)
- [ ] Explore ClawHub : browse existing skills, install 2-3 relevant ones
- [ ] NotebookLM "Socle IA" : 3 épisodes thématiques (tokens/transformer, prompt engineering, RAG/agents)
- [ ] **Advanced Vibe Coding + Sécurité setup** : 5 outils (Superpowers, Everything Claude Code, GET SHIT DONE, Claude-Guardrails, sandboxing) — samedi week 2 avant vibe-coding
- [ ] Start vibe-coding showcase app(s) avec Claude Code — potentiellement plusieurs repos si plusieurs micro-apps

## Later (weeks 3-4)
- [ ] Micro-app intensive build
- [ ] OpenClaw: custom skills, advanced workflows, channel expansion
- [ ] Write AI cheat sheet: 20 concepts Élie can explain in interview with finance analogies
- [ ] Write AI narrative: Élie's learning journey and what he built
- [ ] Dry-runs: simulated interviews with Claude (adversarial mode) + with Adrien
- [ ] Prepare smart questions for Norway interlocutors (based on DR insights)
- [ ] Write personal synthesis: "Ce que je comprends de l'AI dans la finance en 2026"
- [ ] Basic Python literacy track (if time and interest allow)
- [ ] Post Phase 1: continued learning roadmap

*This backlog is not closed — new items will emerge from working sessions.*

***
*Last updated: 2026-04-01 (evening)*
