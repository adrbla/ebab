# Brief — Brainstorming Voice Mode : Showcase App(s)

**Objectif de la session** : Générer et filtrer des idées de micro-applications à construire avec Claude Code pour démontrer une fluency AI crédible en interview. Ce document est ton point de départ — lis-le avant de lancer la session voice, ou demande à Claude de te le résumer à voix haute.

**Deadline** : Semaine du 24 avril 2026. Réaliste = 2-3 weekends de build (weeks 3-4 du programme).

---

## 1. Ce que tu dois démontrer

Une bonne showcase app prouve **trois choses simultanément** :

1. **Tu comprends le problème** — tu as l'instinct métier pour identifier un vrai pain point dans le workflow d'un analyste ou d'un gérant
2. **Tu sais utiliser l'IA pour le résoudre** — pas juste "j'ai utilisé ChatGPT", mais tu as conçu un système avec des outils (API, prompts, agents)
3. **Tu peux l'expliquer simplement** — tu racontes ce que ça fait, pourquoi c'est non-trivial, et ce que tu as appris en le construisant

**Ce que ce n'est PAS** : une app parfaite, scalable, production-ready. C'est un prototype fonctionnel que tu peux démo en 3 minutes et expliquer en 5.

---

## 2. Contraintes à garder en tête

- **Pas de dev background** — tout est vibe-coded avec Claude Code. La complexité doit rester dans ce que Claude peut construire avec toi en quelques sessions.
- **Données réelles de préférence** — une app qui tourne sur de vraies données (même publiques) est infiniment plus crédible qu'un mock.
- **Finance-first** — l'app doit parler à un intervieweur dans la gestion d'actifs. Évite les use cases génériques (résumer des PDFs, traduire du texte...).
- **1 ou 2 apps max** — mieux vaut une chose solide qu'un portfolio de stubs.

---

## 3. Seed ideas — réagis, ne valide pas encore

Ces idées viennent du contexte du projet (DR reports + profil Élie + signaux marché Norway). Elles sont là pour stimuler, pas pour contraindre.

### A — Earnings Signal Extractor
Prend une transcript d'earnings call (Seeking Alpha, API) et en extrait automatiquement : le tone shift vs dernier quarter, les 3 sujets clés management, les signaux de guidance (upgrade/downgrade implicite), les questions analysts les plus incisives. Output : une fiche structurée en 1 page.

*Pourquoi ça parle* : c'est exactement le workflow manuel d'un analyste L/S. Tu l'as fait des centaines de fois — tu sais où est la valeur.

### B — Perception Gap Screener
Pour une liste de tickers, requête automatique de l'estimation consensus (Yahoo Finance API gratuit) + quelques signaux qualitatifs récents (news Google RSS), puis prompt Claude pour scorer chaque position sur un axe "consensus too bullish / too bearish". Output : un tableau de bord simple avec les positions les plus asymétriques.

*Pourquoi ça parle* : c'est ta philosophie d'investissement ("perception gap") codée en outil. Très narrativement fort en interview.

### C — Nordic AM Radar
Un mini-dashboard qui agrège les mouvements publics des grands gérants norvégiens (NBIM déclarations, Storebrand rapports, etc.), tague chaque news par secteur/thème, et sort un weekly digest formaté. Version enrichie d'un subset de ce qu'OpenClaw fait déjà — mais avec une UI navigable.

*Pourquoi ça parle* : montre que tu connais le paysage norvégien ET que tu peux construire des outils de veille. Double signal pour NBIM/Storebrand/DNB AM.

### D — ESG Flag Screener (inspired by NBIM)
NBIM utilise Claude pour le screening ESG. Tu construis un prototype qui prend un rapport annuel (PDF) ou un article, et génère un "ESG flag report" structuré : controverses identifiées, alignement avec les exclusion criteria typiques (armes, charbon, droits humains), score de risque. Output : fiche en markdown.

*Pourquoi ça parle* : citation directe de NBIM → "j'ai essayé de répliquer ce qu'ils font, voilà ce que ça donne". Très fort pour les entretiens NBIM-adjacent.

### E — Portfolio Diary / Investment Log
Une app minimaliste où tu loggues tes thèses d'investissement (ticker, thèse courte, date entry, horizon), et Claude génère automatiquement : un reminder des hypothèses clés à un check-in schedulé, un tableau de bord de cohérence de portefeuille, et une synthèse mensuelle "qu'est-ce qui a changé dans mes convictions". Outil de discipline personnelle pour analyste.

*Pourquoi ça parle* : très "augmented analyst" — tu utilises l'IA pour améliorer ta rigueur de process, pas pour substituer ton jugement.

### F — Norwegian Job Pulse
Version UI de la capability #5 d'OpenClaw : un dashboard qui affiche les job postings finance en Norvège avec tags (type de fonds, séniorité, deadline), filtre par keywords, et ajoute un layer Claude qui score chaque posting sur "fit avec profil analyste L/S". Données réelles (finn.no + career pages).

*Pourquoi ça parle* : outil que tu utilises activement toi-même. Crédible, démontrable, données réelles.

---

## 4. Grille de sélection — pour chaque idée, pose-toi ces questions

| Critère | Ce que tu veux |
|---|---|
| **Pain réel** | Est-ce que tu as personnellement souffert de ce problème dans ta carrière ? |
| **Démo en 3 min** | Est-ce qu'on peut voir l'output en live sans avoir besoin d'expliquer 10 minutes de contexte ? |
| **Données accessibles** | Les données sont-elles disponibles gratuitement ou facilement ? |
| **Buildable en 2 weekends** | Claude Code peut-il produire un v1 fonctionnel avec toi en 6-8h de sessions ? |
| **Narrativement fort** | Est-ce que ça raconte une histoire sur *toi* spécifiquement — pas n'importe quel analyste ? |

---

## 5. Ce que tu peux laisser émerger librement

La session voice est faite pour ça — laisse-toi surprendre. Quelques pistes ouvertes à explorer :

- Y a-t-il un moment précis dans ta carrière (Pelham, Trium, Catalyst) où tu t'es dit "si j'avais eu un outil qui faisait X, ça m'aurait sauvé des heures" ?
- Qu'est-ce qui t'a le plus frustré dans le process de recherche analyste que tu as le plus répété ?
- Y a-t-il une chose que tu fais manuellement chaque semaine qui est stupidement automatisable ?
- Qu'est-ce qui impressionnerait *toi* si un candidat te le montrait en entretien ?

---

## 6. Output attendu de la session voice

À la fin du brainstorming, tu devrais avoir :
- 1 ou 2 idées retenues avec une phrase de pitch ("ça fait X, pour Y, en utilisant Z")
- Un sentiment clair sur l'idée principale vs backup
- Quelques contraintes/risques identifiés à anticiper

Ce draft sera ensuite travaillé avec Adrien (semaine 2, Saturday) pour finaliser le scope avant le build.

---

*Brief préparé le 2026-03-30. Contexte : DR reports NBIM/Norway/buy-side + profil Élie + backlog EBAB.*
