# Journal – EBAB

*Narrative log of sessions, decisions, and open questions. Append new entries at the bottom.*

***

## 2026-03-28 — Project bootstrap (Adrien B.)

**Goal**: Initialize the EBAB project from scratch — profile Élie, structure the program, prepare Deep Research inputs.

**What we did**:
- Ran bootstrap interview with Élie (45-min structured conversation in Cowork)
- Produced `context/references/elie-profile.md` — full professional profile, motivations, constraints
- Identified 3 Deep Research angles: (1) NBIM's AI strategy, (2) Norwegian AM landscape, (3) AI in buy-side globally
- Drafted 3 calibrated DR prompts and ran them → received all 3 reports
- Saved reports in `context/references/dr-reports/`: dr1-nbim-ai-strategy.md, dr2-norway-am-landscape.md, dr3-ai-buyside-global.md
- Defined the 4-week roadmap: exploration → NotebookLM → OpenClaw → micro-app → interview prep
- Saved roadmap in `context/roadmap.md`

**Key decisions**:
- Program deadline: week of April 24, 2026 (Norway trip / interview window)
- Structure: 3 pillars (research, personal implementation, showcase micro-app)
- Phase 1 anchor: NBIM — but scope is all roles where AI fluency is a differentiator
- Learning approach: "learn by doing" — every tool introduced is actually configured and used

**Open questions resolved**:
- Élie confirmed: no coding background, comfortable with terminal in principle, wants hands-on
- Adrien confirmed: will set up OpenClaw concept before Sunday session with Élie

***

## 2026-03-29 — Premier jour complet Élie — NotebookLM + OpenClaw + finn.no (Élie B.)

**Goal**: Première session active d'Élie — installer et configurer les outils, explorer le marché emploi norvégien.

**What we did**:
- **NotebookLM** — configuré 2 notebooks : "Socle IA" (DR socle générative AI uploadé) et "AI & Finance" (3 DR reports NBIM/Norway/buy-side). Élie a généré son premier podcast Audio Overview en mode interactif. Premier quiz complété — a confirmé que les concepts probabilistes étaient déjà connus, calibration utile.
- **OpenClaw installé sur Mac Mini** — full stack opérationnel :
  - `openclaw onboard` exécuté dans terminal (TUI interactif → nécessite terminal natif, pas Desktop Commander)
  - Gemini API configuré comme moteur de web search (Brave Search n'est plus gratuit depuis févr. 2026)
  - Telegram bot créé via BotFather, token configuré
  - Gateway lancé comme LaunchAgent (persistant après reboot)
  - Allowlist sécurité : ID Telegram numérique d'Élie (`8742203868`) ajouté dans `~/.openclaw/openclaw.json`
  - Pairing approuvé via `openclaw pairing approve telegram V27EXQSR`
  - Statut final : gateway actif, Telegram connecté, modèle claude-sonnet-4-6, 0 critical warnings
- **Framework repo openclaw-elie créé** :
  - `CLAUDE.md` complet (6 capabilities, calibration philosophie investissement, protocole de session)
  - `context/backlog.md` et `context/journal.md` initialisés
  - Repo sur GitHub Élie, Adrien ajouté comme collaborateur
- **Exploration finn.no** — calibration du skill #5 (job postings) :
  - Query large (`forvalter OR aksjeanalytiker OR ...`) → 726 résultats, 90%+ de bruit (gestionnaires de propriété, admins IT, etc.)
  - Query ciblée (`investeringsanalytiker OR kapitalforvaltning OR aksjeanalytiker`) → 22 résultats, beaucoup plus propre
  - Seul posting vraiment aligné trouvé : **Investeringsanalytiker – Kapitalforvaltning** chez Pensjonskassen (NOK 57Mrd, équipe 4 personnes, report au CIO, deadline 10 avril)
  - LinkedIn : seulement 2 résultats — finn.no est le canal dominant pour le marché norvégien
  - Permian (fund admin/accountant PE) : 2 rôles postés — davantage back-office

**Important decisions**:
- Keywords OpenClaw skill #5 calibrés : `investeringsanalytiker OR kapitalforvaltning OR aksjeanalytiker OR porteføljeforvalter` (pas "forvalter" seul — trop de bruit)
- Monitoring direct des career pages (NBIM, Storebrand, DNB AM, Ferd, KLP) plus fiable pour les rôles seniors
- finn.no : vérification quotidienne suffisante (postings restent actifs 9-26 jours)
- Brave Search supprimé du plan — Gemini (Google Search) retenu comme moteur gratuit pour OpenClaw

**Repo structure clarification** (réponse à question d'Élie) :
- Les deux repos sont correctement séparés — ils ne sont PAS imbriqués
- `ebab/` → `/Users/elie/Documents/Project/ebab/` (git root = ebab/)
- `openclaw-elie/` → `/Users/elie/Documents/Project/framework/openclaw-elie/` (git root = openclaw-elie/)
- Ces deux dossiers sont des **siblings** dans `/Users/elie/Documents/Project/` — aucun problème de git nested

**Open questions**:
- **Pour Élie** : cc-openclaw (9 slash commands Claude Code) à installer dans une prochaine session Claude Code
- **Pour Adrien** : Valider la calibration skill #5 et les keywords finn.no avant config capabilities 1-4

**Next steps**:
- Session Claude Code `framework/openclaw-elie/` : configurer capabilities 1-4 (veille NBIM, Norway, AI buy-side, briefing 07h30)
- Installer cc-openclaw via `git clone` + `claude skill install` dans le terminal
- NotebookLM : 3 épisodes thématiques "Socle IA" + épisode "AI & Finance"
- Radar : Investeringsanalytiker Pensjonskassen — deadline 10 avril

***

## 2026-03-29 — NotebookLM "AI & Finance" + clôture de session (Élie B.)

**What we did**:
- **NotebookLM "The Augmented Analyst"** (3 sources : DR1-NBIM, DR2-Norway, DR3-buy-side) — Studio complet généré :
  - **Podcast** : Analyse approfondie, Long, en anglais, focus calibré (NBIM Strategy 2028 + Investment Simulator + paysage Norway + profil analyst attendu pour 2026)
  - **Quiz** : Difficile, Plus de questions, focus NBIM + Norway actors + buy-side analyst workflow
  - **Fiches DR1** (NBIM) : Plus de cartes, Difficile — Investment Simulator, Strategy 2028, vibe-coding, ESG screening Claude, critères d'embauche
  - **Fiches DR2** (Norway landscape) : Plus de cartes, Difficile — Storebrand, Ferd, DNB AM, KLP, maturity tiers, signaux hiring
  - **Fiches DR3** (buy-side global) : Plus de cartes, Difficile — workflow analyst AI-augmenté, outils top funds 2025-2026, alpha generation, normes professionnelles
- **cc-openclaw + capabilities 1-4** : confirmés comme déjà accomplis en session Claude Code parallèle (lu dans `framework/openclaw-elie/context/journal.md`)
- **Backlog + journal mis à jour** et pushés sur GitHub

**Session close — état au 29 mars soir** :
- OpenClaw : gateway actif, 18 feeds configurés, briefing 07h30 Oslo actif → **premier briefing demain lundi 30 mars**
- NotebookLM : 2 notebooks armés, 6 Studio outputs disponibles (podcast + quiz + 3 decks fiches)
- finn.no : keywords calibrés, prêts pour capability #5
- cc-openclaw : 9 slash commands installés dans Claude Code
- GitHub : tout pushé, à jour

**Next steps pour la semaine** :
- Lundi matin : valider réception briefing Telegram 07h30
- Semaine : écouter podcast "AI & Finance" en mode interactif (pauses + questions)
- Semaine : faire quiz DR1/DR2/DR3 (difficile) + réviser avec les fiches
- Semaine : 3 épisodes thématiques "Socle IA" à générer (tokens/transformer, prompt engineering, RAG/agents)
- Claude Code : capability #5 (finn.no) + capability #6 (stock initial take, choix API financière)

***

## 2026-03-30 — Briefing raté + décision migration VPS (Adrien B.)

**Goal**: Constater le problème d'uptime et décider de la solution.

**What happened**:
- Le briefing quotidien OpenClaw de 07h30 n'a pas été envoyé sur Telegram — le Mac Mini d'Élie était éteint.
- Décision : migrer OpenClaw sur un VPS Hetzner CX23 (2 vCPU, 4GB RAM, 40GB SSD). Domaine enregistré : `elibla.com` — page racine + sous-domaines pour les apps/installs.
- Déploiement prévu le 2026-03-30 au soir.

**Important decisions**:
- VPS Hetzner CX23 pour héberger OpenClaw 24/7 (voir `context/decisions.md`)
- Le Mac Mini reste l'environnement de dev/config ; le VPS est l'environnement de production

**Next steps**:
- 2026-03-30 soir : provisionner VPS, configurer domaine/sous-domaine, déployer OpenClaw
- Valider que le briefing du 2026-03-31 arrive bien sur Telegram

***

## 2026-03-30 — Provisionnement VPS Hetzner (Élie B.)

**Goal**: Créer le VPS, tester la connexion SSH, préparer l'environnement Node.js pour OpenClaw.

**What we did**:
- **Compte Hetzner créé** par Élie
- **VPS provisionné** via Hetzner Cloud Console :
  - Nom : **elibla** (serveur générique — pas dédié à OpenClaw uniquement)
  - Type : CX23 (2 vCPU, 4 GB RAM, 40 GB SSD, 20 TB traffic)
  - Location : **Nuremberg** (eu-central) — Helsinki indisponible en CX23 au moment de la création
  - Image : Ubuntu 24.04 LTS
  - IP publique : **178.104.112.7**
  - Prix : €4.19/mo (CX23 €3.59 + IPv4 €0.60)
  - SSH key : `elie@elibla.com` (ed25519, générée sur Mac Mini `~/.ssh/id_ed25519`)
- **Connexion SSH testée** depuis le Mac Mini : ✅ `SSH_OK` — Linux elibla 6.8.0-90-generic
- **Node.js installé** via NodeSource : `node v22.22.0`, `npm 10.9.4`
- **Décision** : déploiement OpenClaw et configuration (API keys, cron, Telegram pairing) délégué à une session Claude Code — l'interface interactive est mieux adaptée que Cowork pour `openclaw onboard`

**Technical notes**:
- La SSH key dans Hetzner Console est nommée `elie@elibla.com` (le commentaire de la clé ed25519)
- Le domaine `elibla.com` est enregistré mais pas encore actif (DNS non configuré) — à faire quand le VPS sera stabilisé
- `~/.ssh/id_ed25519.pub` sur Mac Mini : `ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIA0vEjoWMLAOuUoku6abtNow6F81eEo6Pur9scoiWm4R elie@elibla.com`

**Next steps** :
- **Claude Code** (`framework/openclaw-elie/`) : `npm install -g openclaw@latest` sur le VPS, `openclaw onboard` interactif, migration config depuis Mac Mini (API keys, Telegram token, feeds), cron 07h30 Oslo, validation premier briefing
- Objectif : briefing du **2026-03-31 à 07h30** livré depuis le VPS

***
