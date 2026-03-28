# Roadmap – EBAB Phase 1

**Objectif** : donner à Élie un socle crédible d'AI literacy (connaissance + expérience) en ~100–120h sur 4 semaines.
**Deadline** : semaine du 24 avril 2026 (voyage Norvège).
**Format** : week-ends 2×8h (samedi + dimanche), semaine ~10–12h en sessions de 1–3h.
**Checkpoints** : Adrien disponible matin/midi/soir les week-ends, et sur sollicitation en semaine.

Ce document est une base vivante — il sera mis à jour au fur et à mesure avec Élie et Claude Code.

---

## Semaine 1 — Fondations (29 mars – 4 avril)

### Thème : Comprendre l'IA, comprendre le contexte, mettre les mains dedans

### Dimanche 29 mars (8h) — Kickoff

**Matin (4h) — Socle de connaissances IA + NotebookLM**

1. **Prise en main NotebookLM** (~30 min)
   - Créer un compte sur [notebooklm.google.com](https://notebooklm.google.com)
   - Créer un premier notebook "Socle IA"
   - Uploader le rapport DR `socle_gen-AI.md`

2. **Audio Overview — première imprégnation** (~45 min)
   - Générer un Audio Overview "Deep Dive" du rapport
   - L'écouter en **mode interactif** : mettre en pause quand un concept n'est pas clair, poser des questions aux hosts, qui répondent en s'appuyant sur le document
   - L'idée : ce n'est pas de l'écoute passive. C'est une conversation avec le contenu.

3. **Podcasts ciblés — 3 épisodes thématiques** (~1h30)
   - Générer 3 Audio Overviews avec des focus areas différents :
     - Épisode 1 : "Les fondamentaux — qu'est-ce qu'un LLM, comment ça fonctionne, les tokens, le transformer" (niveau : débutant curieux)
     - Épisode 2 : "Prompts et ingénierie de prompt — comment bien parler à un modèle" (niveau : praticien)
     - Épisode 3 : "RAG, agents, outils — les architectures avancées" (niveau : conceptuel, pas technique)
   - Écouter au moins l'épisode 1 en interactif. Les 2 autres peuvent être écoutés en semaine.

4. **Quiz + Flashcards** (~45 min)
   - Générer un quiz (difficulté Medium) sur le rapport
   - Le faire — utiliser le bouton "Explain" à chaque erreur ou doute
   - Générer des flashcards sur les concepts clés
   - L'objectif : ancrer le vocabulaire de base (token, LLM, prompt, RAG, agent, fine-tuning, hallucination, etc.)

5. **Debrief matin avec Adrien** (~30 min)
   - Qu'est-ce qui est clair ? Qu'est-ce qui reste flou ?
   - Quels concepts l'ont surpris ou intéressé ?

**Après-midi (4h) — NotebookLM contexte finance + conception OpenClaw**

6. **Deuxième notebook NotebookLM : "AI & Finance"** (~1h30)
   - Créer un nouveau notebook
   - Uploader les 3 DR reports (NBIM, Norway actors, buy-side global)
   - Générer un Audio Overview "Deep Dive" sur l'ensemble
   - Écoute interactive — focus : que fait le NBIM concrètement ? Quels autres acteurs en Norvège ? Comment l'AI change le buy-side ?
   - Générer 1-2 épisodes ciblés :
     - "Le NBIM et sa stratégie AI — ce qu'ils font, ce qu'ils cherchent"
     - "Le paysage norvégien — qui fait quoi au-delà du NBIM"

7. **Conception OpenClaw** (~1h30) — avec Adrien
   - Qu'est-ce qu'OpenClaw ? (assistant AI personnel, open-source, tourne sur ton Mac Mini 24/7, accessible depuis Telegram/iMessage/web)
   - Définir ensemble ce qu'on veut que l'agent fasse :
     - **Veille NBIM** : surveiller les publications, communiqués, articles sur le fonds et sa stratégie AI
     - **Veille acteurs norvégiens** : Storebrand, Ferd, Aker, Arctic, Skagen, etc.
     - **Veille AI buy-side** : tendances, outils, cas d'usage dans l'investissement
     - **Briefing quotidien** : synthèse envoyée chaque matin sur Telegram
   - Définir les canaux (Telegram pour commencer)
   - Lister les skills/MCP servers nécessaires (recherche web, RSS, etc.)
   - **Livrable** : un document de conception (`output/openclaw-design.md`) qui servira de brief pour la session Claude Code d'installation

8. **Installation OpenClaw** (~1h) — avec Claude Code
   - Ouvrir Claude Code dans un nouveau dossier `framework/openclaw-elie/`
   - Installer OpenClaw (`openclaw onboard`)
   - Configurer le provider (Anthropic API key)
   - Connecter Telegram
   - Vérifier que l'agent répond
   - Ne pas encore configurer les skills — juste le squelette qui fonctionne

### Semaine (lundi 31 – vendredi 4 avril) — ~10-12h

**Objectif semaine** : absorber le socle IA et le contexte finance via NotebookLM, commencer à configurer OpenClaw.

| Créneau | Activité | Durée | Notes |
|---------|----------|-------|-------|
| Lun-Mar soir | Écouter les épisodes NotebookLM restants (socle IA épisodes 2-3) en mode interactif | 2×1h | Pause + questions aux hosts. Prendre des notes des concepts clés. |
| Mer soir | Quiz NotebookLM socle IA (difficulté Hard) + flashcards | 1h | Tester la rétention après quelques jours. |
| Jeu soir | Épisodes NotebookLM "AI & Finance" (NBIM + paysage norvégien) en interactif | 1h30 | Focus : quels sont les vrais use cases AI chez NBIM ? Quels acteurs correspondent le plus à mon profil ? |
| Vendredi (home) | Session Claude Code : configurer les premières skills OpenClaw | 3h | Installer les skills de veille (web search, RSS). Configurer les premières sources. Tester un premier briefing. |
| Vendredi soir (optionnel) | Explorer le ClawHub — parcourir les skills disponibles, en installer 2-3 qui semblent utiles | 1-2h | Curiosité guidée : qu'est-ce qui existe ? Qu'est-ce qui pourrait servir ? |

**Ce qu'Élie sait faire à la fin de la semaine 1** :
- Expliquer ce qu'est un LLM, un token, un prompt, le RAG, un agent — dans ses mots, en reliant à la finance
- Décrire ce que le NBIM fait avec l'AI et nommer 5+ autres acteurs norvégiens pertinents
- Utiliser NotebookLM comme outil d'apprentissage (podcasts interactifs, quiz, flashcards)
- Avoir un OpenClaw qui tourne sur son Mac Mini avec Telegram connecté et les premières skills de veille

---

## Semaine 2 — Approfondissement + Conception (5–11 avril)

### Thème : Aller en profondeur, concevoir l'agent et les micro-apps

### Samedi 5 avril (8h)

**Matin (4h) — Approfondissement contexte finance**

1. **NotebookLM "AI & Finance" — session approfondie** (~2h)
   - Générer des épisodes ciblés supplémentaires :
     - "Comment l'AI change la construction de thèses d'investissement" (directement lié au profil d'Élie)
     - "Le vibe-coding chez NBIM — 50% du staff qui code avec Claude"
   - Mode Debate : générer un épisode où les hosts débattent sur "L'AI remplace-t-elle le jugement de l'investisseur ?"
   - Quiz Hard sur les 3 DR combinés

2. **Synthèse personnelle** (~1h)
   - Avec Claude Code, rédiger une note de synthèse : "Ce que je comprends de l'AI dans la finance en 2026" — dans ses propres mots
   - Cette note servira de base pour son narratif d'entretien plus tard

3. **Review OpenClaw** (~1h) — avec Adrien
   - Le briefing quotidien fonctionne-t-il ? Qu'est-ce qui manque ?
   - Ajuster les sources, les skills, le format du briefing
   - Identifier les MCP servers à ajouter (financial data feeds, etc.)

**Après-midi (4h) — Conception micro-app(s)**

4. **Session de conception avec Adrien** (~2h) — dans Cowork
   - Sur la base des DR : quels pain points / opportunités ressortent ?
   - Brainstorm : quelle(s) micro-app(s) démontreraient une compréhension profonde de l'AI appliquée à l'investissement ?
   - Critères : ça doit "parler" à un interlocuteur type NBIM, montrer qu'Élie comprend comment l'AI transforme le métier (pas juste automatiser), être réalisable en ~20-30h de vibe-coding
   - **Pistes à explorer** (à affiner avec les DR) :
     - Un "Investment Thesis Challenger" qui structure et stress-teste une thèse via adversarial prompting
     - Un "ESG Risk Scanner" inspiré de ce que fait NBIM (screening AI de portefeuille)
     - Un "Perception Gap Detector" qui identifie les dislocations entre narratif sell-side et fondamentaux
     - Un dashboard de veille AI-powered sur un secteur/thème
   - **Livrable** : un brief de conception (`output/micro-app-design.md`) — 1 ou 3 apps, scope, stack, ce que ça démontre

5. **Premiers pas vibe-coding** (~2h) — avec Claude Code
   - Sur la base du brief, commencer le scaffolding de la micro-app principale
   - Élie expérimente : décrire ce qu'il veut en langage naturel, Claude Code génère le code
   - L'objectif n'est PAS de finir — c'est de comprendre le flow du vibe-coding
   - Commit initial dans un nouveau repo `framework/micro-app-elie/` (ou un nom plus parlant)

### Dimanche 6 avril (8h)

**Matin (4h) — OpenClaw avancé**

6. **Skills et MCP servers dédiés** (~2h) — avec Claude Code
   - Installer et configurer des skills finance-spécifiques
   - Configurer des MCP servers pertinents (financial news APIs, etc.)
   - Écrire une première skill custom : par ex. un format de briefing adapté au profil d'Élie (pas un résumé générique mais une synthèse orientée "qu'est-ce qui change pour un investisseur fondamental")

7. **Concevoir un workflow agentique** (~2h)
   - Au-delà de la veille passive : définir un agent qui, quand Élie lui donne un nom d'entreprise, va chercher les dernières publications, les filings, les news, et produit un "primer" structuré
   - C'est le début d'un vrai outil de travail, pas juste un gadget
   - L'expérience est dans la conception autant que dans le résultat

**Après-midi (4h) — Micro-app**

8. **Vibe-coding session longue** (~4h)
   - Continuer la construction de la micro-app
   - Itérations : Élie décrit → Claude Code génère → Élie teste → ajuste
   - Focus : avoir un prototype fonctionnel (même minimal) à la fin de la journée
   - Ce prototype sera itéré en semaine 3

### Semaine (lundi 7 – vendredi 11 avril) — ~10-12h

| Créneau | Activité | Durée | Notes |
|---------|----------|-------|-------|
| Lun-Mar soir | Vibe-coding : itérer sur la micro-app (features, UI, polish) | 2×1h30 | Sessions courtes et focalisées. Un objectif par session. |
| Mer soir | OpenClaw : ajuster les skills, tester le workflow "company primer" | 1h30 | L'agent s'améliore au fil des jours. |
| Jeu soir | NotebookLM : épisode "Learning Guide" sur un concept avancé (agents, multi-agent systems, RAG) | 1h | Garder le fil rouge apprentissage. |
| Vendredi (home) | Vibe-coding session longue : itérer, tester, debugger | 3h | Avoir un prototype solide pour le week-end. |

**Ce qu'Élie sait faire à la fin de la semaine 2** :
- Articuler sa compréhension de l'AI en finance — dans ses mots, avec des exemples concrets
- Avoir un OpenClaw configuré avec des skills finance + veille + un workflow "company primer"
- Avoir un prototype de micro-app fonctionnel (même brut)
- Avoir conçu et configuré des MCP servers et des skills customs — comprendre ce que c'est et pourquoi c'est puissant

---

## Semaine 3 — Construction (12–18 avril)

### Thème : Construire, raffiner, tester

### Samedi 12 avril (8h)

**Matin (4h) — Micro-app : itération majeure**

1. **Review du prototype avec Adrien** (~1h)
   - Où en est-on ? Qu'est-ce qui fonctionne, qu'est-ce qui manque ?
   - Décisions : scope final, features à garder, features à couper
   - Focus : la micro-app doit raconter une histoire — pas tout faire, mais bien faire une chose qui "parle"

2. **Vibe-coding intensif** (~3h)
   - Implémenter les features clés
   - Affiner l'UX — ça doit être montrable, pas juste fonctionnel

**Après-midi (4h) — OpenClaw + consolidation**

3. **OpenClaw : skills avancées** (~2h)
   - Écrire 1-2 skills customs supplémentaires calibrées pour le contexte norvégien
   - Tester le briefing quotidien après 2 semaines de données : est-ce utile ? Qu'est-ce qui manque ?
   - Éventuellement : connecter l'agent à d'autres canaux (iMessage, web)

4. **Consolidation des connaissances** (~2h)
   - NotebookLM : quiz final (Hard) sur socle IA + contexte finance
   - Écrire un "cheat sheet" : les 20 concepts AI qu'Élie doit pouvoir expliquer en entretien, avec pour chacun une phrase simple + un exemple finance
   - Sauvegarder dans `output/ai-cheat-sheet.md`

### Dimanche 13 avril (8h)

**Journée complète — Micro-app finition**

5. **Vibe-coding marathon** (~6h)
   - Finir les features
   - Polish : design, messages, flow utilisateur
   - Tests : est-ce que ça marche end-to-end ?

6. **Documentation** (~2h)
   - Écrire un court README pour la micro-app : ce que ça fait, pourquoi, comment c'est construit
   - Ce README fait partie du "showcase" — c'est ce qu'un interlocuteur lirait pour comprendre la démarche

### Semaine (lundi 14 – vendredi 18 avril) — ~10-12h

| Créneau | Activité | Durée | Notes |
|---------|----------|-------|-------|
| Lun soir | Micro-app : tests, edge cases, derniers ajustements | 1h30 | |
| Mar soir | OpenClaw : review et optimisation du briefing quotidien | 1h | 2 semaines de données — qu'est-ce qui a été vraiment utile ? |
| Mer soir | Rédiger la note de synthèse : "Mon parcours AI en 3 semaines" | 1h30 | Réflexion sur ce qu'il a appris, construit, compris. |
| Jeu soir | Préparer le narratif d'entretien : comment parler de tout ça | 1h30 | Avec Claude (chat ou Code) : simuler des questions, préparer des réponses. |
| Vendredi (home) | Dry-run : simulation d'entretien avec Claude en mode adversarial | 3h | Claude joue le rôle d'un recruteur NBIM exigeant. Tester les réponses, identifier les trous. |

**Ce qu'Élie sait faire à la fin de la semaine 3** :
- Micro-app terminée et documentée, prête à être montrée
- OpenClaw mature avec skills customs, briefing quotidien rodé
- Capacité à expliquer 20+ concepts AI avec des exemples finance
- Premier narratif d'entretien structuré

---

## Semaine 4 — Consolidation + Norvège (19–25 avril)

### Thème : Consolider, pratiquer, être prêt

### Samedi 19 avril (8h) — Pâques, Élie a vendredi + samedi + dimanche

**NB** : Pâques offre potentiellement un jour supplémentaire (vendredi 18 avril). À ajuster.

**Matin (4h) — Polissage final**

1. **Micro-app : derniers ajustements** (~1h)
   - Bug fixes, polish, déploiement si pertinent

2. **OpenClaw : état final** (~1h)
   - Dernier check : tout tourne, le briefing est calibré, les skills sont stables

3. **Narratif : consolidation** (~2h)
   - Finaliser le "AI story" d'Élie : parcours d'apprentissage, ce qu'il a construit, ce qu'il comprend, sa vision
   - Le structurer comme un pitch naturel, pas un récit linéaire
   - Sauvegarder dans `output/ai-narrative.md`

**Après-midi (4h) — Préparation entretiens**

4. **Dry-run intensif avec Adrien** (~2h)
   - Simulation d'entretien : questions techniques IA, questions "fit", questions sur la micro-app
   - Feedback direct, ajustements

5. **Dry-run avec Claude** (~2h)
   - Claude joue différents rôles : recruteur NBIM technique, recruteur family office, investisseur curieux
   - Mode adversarial : "prouve-moi que tu comprends vraiment, pas juste le vocabulaire"
   - Identifier les derniers trous et les combler

### Dimanche 20 avril (8h)

**Journée buffer / approfondissement**

6. **Selon les besoins** :
   - Compléter ce qui manque (micro-app, narratif, connaissances)
   - Approfondir un sujet identifié pendant les dry-runs
   - Préparer des questions intelligentes à poser aux interlocuteurs en Norvège (basées sur les DR)
   - Relaxer et laisser décanter si tout est prêt

### Semaine (lundi 21 – mercredi 23 avril) — derniers jours

| Créneau | Activité | Durée | Notes |
|---------|----------|-------|-------|
| Lun soir | Dernière révision des flashcards + cheat sheet | 1h | Ancrage final. |
| Mar soir | Relire les DR (NBIM surtout) avec un œil frais | 1h30 | Repérer les détails qui feront la différence en conversation. |
| Mer soir | Check final avec Adrien | 1h | Go/no-go. Derniers ajustements. |

**Ce qu'Élie a à la fin de la semaine 4 (et du Phase 1)** :
- Une compréhension solide de l'IA générative, de son application en finance, et du paysage norvégien
- Un OpenClaw configuré et opérationnel — preuve tangible de compréhension agentique
- Une micro-app fonctionnelle et documentée — showcase de sa capacité à concevoir et builder avec l'IA
- Un narratif rodé pour les entretiens
- Les outils et la confiance pour continuer à apprendre (Phase 2+)

---

## Budget temps estimé

| Bloc | Heures |
|------|--------|
| Semaine 1 — WE (dimanche) | 8 |
| Semaine 1 — Semaine | 10-12 |
| Semaine 2 — WE (sam + dim) | 16 |
| Semaine 2 — Semaine | 10-12 |
| Semaine 3 — WE (sam + dim) | 16 |
| Semaine 3 — Semaine | 10-12 |
| Semaine 4 — WE (sam + dim) | 16 |
| Semaine 4 — Semaine | 5-6 |
| **Total estimé** | **~91–98h** |

Il reste une marge de ~10-20h pour les imprévus, les approfondissements, et le grappillage en soirée.

---

*Ce document est une base vivante. Il sera mis à jour après chaque session.*

*Dernière mise à jour : 2026-03-28*
