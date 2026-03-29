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
   - Installer [cc-openclaw](https://github.com/rahulsub-be/cc-openclaw) : `git clone` + `stow` — 9 Claude Code skills pour piloter OpenClaw (/openclaw-new-agent, /openclaw-add-channel, /openclaw-add-cron, /openclaw-add-secret, /openclaw-status, /openclaw-restart, etc.)
   - Vérifier que les slash commands fonctionnent dans Claude Code

### Semaine (lundi 30 – vendredi 4 avril) — ~18-22h

**Ajustement** : +1-2h par après-midi disponible cette semaine → heures supplémentaires utilisées pour avancer sur NotebookLM et amorcer OpenClaw avant le weekend du 5 avril.

**Objectif semaine** : absorber le socle IA et le contexte finance via NotebookLM, commencer à configurer OpenClaw.

| Créneau | Activité | Durée | Notes |
|---------|----------|-------|-------|
| Lun matin/après-midi | Écouter épisode NotebookLM socle IA #2 en interactif | 1-2h | "Prompts et ingénierie de prompt" — pause + questions aux hosts. |
| Lun soir | Écouter épisode NotebookLM socle IA #3 en interactif | 1h | "RAG, agents, architectures avancées" — niveau conceptuel. |
| Mar après-midi | Quiz NotebookLM socle IA (difficulté Medium puis Hard) + flashcards | 1-2h | Tester la rétention. Bouton "Explain" à chaque erreur. |
| Mar soir | Épisodes NotebookLM "AI & Finance" — Deep Dive NBIM | 1h | Focus : que fait le NBIM concrètement ? Ce qu'ils cherchent chez un candidat. |
| Mer après-midi | Épisodes NotebookLM "AI & Finance" — paysage norvégien + buy-side global | 1-2h | Quels acteurs correspondent à mon profil ? Quels outils AI sont réels vs. hype ? |
| Mer soir | Synthèse personnelle avec Claude : "ce que je comprends de l'AI en finance" | 1h | Dans ses propres mots — première brique du narratif d'entretien. |
| Jeu après-midi | Concevoir OpenClaw : définir ce qu'on veut que l'agent fasse | 1-2h | Avec Adrien ou en solo : veille NBIM, acteurs norvégiens, briefing quotidien. Livrable : `output/openclaw-design.md`. |
| Jeu soir | Quiz Hard NotebookLM "AI & Finance" | 1h | Ancrage du contexte finance. |
| Vendredi (home) | Session Claude Code : installer OpenClaw + configurer premières skills | 3h | Squelette fonctionnel avec Telegram connecté. |
| Vendredi après-midi | Explorer le ClawHub — parcourir les skills disponibles, en installer 2-3 | 1-2h | Curiosité guidée : qu'est-ce qui existe ? Qu'est-ce qui pourrait servir ? |

**Ce qu'Élie sait faire à la fin de la semaine 1** :
- Expliquer ce qu'est un LLM, un token, un prompt, le RAG, un agent — dans ses mots, en reliant à la finance
- Décrire ce que le NBIM fait avec l'AI et nommer 5+ autres acteurs norvégiens pertinents
- Utiliser NotebookLM comme outil d'apprentissage (podcasts interactifs, quiz, flashcards)
- Avoir un OpenClaw qui tourne sur son Mac Mini avec Telegram connecté et les premières skills de veille
- Avoir une première ébauche de son narratif AI personnel

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

**Après-midi (4h) — Setup avancé + Conception micro-app(s)**

4. **Advanced Vibe Coding + Sécurité : setup et compréhension** (~2h) — avec Claude Code
   - **Objectif** : avant de commencer à vibe-coder, installer et comprendre les outils qui font la différence entre un usage naïf et un usage avancé de Claude Code.
   - **Installer 5 outils** :
     - [Superpowers](https://github.com/obra/superpowers) — framework qui impose un workflow structuré : plan → exécution → test → review. Analogie directe avec la construction de thèse d'investissement.
     - [Everything Claude Code](https://github.com/affaan-m/everything-claude-code) — playbook complet : 30+ subagents, 135+ skills, slash commands. Le setup de référence pour du Claude Code en production.
     - [GET SHIT DONE](https://github.com/gsd-build/get-shit-done) — context engineering pour projets longs : phases structurées, fresh contexts, commits atomiques. Résout le "context rot".
     - [Claude-Guardrails](https://github.com/dwarvesf/claude-guardrails) — hooks de sécurité déterministes : bloque commandes dangereuses (rm -rf, force push), protège .env/SSH keys, scan anti-injection. Version "lite" ou "full".
     - Sandboxing natif Claude Code — isolation filesystem/réseau, permissions par glob patterns, "Auto mode".
   - **Comprendre ce que chaque outil fait** : pas juste installer — Élie doit pouvoir expliquer en une phrase ce que fait chaque outil et pourquoi c'est important.
   - **Commandes de base** : explorer les commandes principales de Superpowers et Everything Claude Code. Objectif : être capable de répondre à une question comme "Quelle est la commande que tu utilises le plus souvent dans Claude Code ?"
   - **Pourquoi c'est important** : en entretien, la différence entre "j'ai utilisé Claude Code" et "j'ai un setup structuré avec guardrails, workflow discipliné et context engineering" est la différence entre un touriste et quelqu'un qui comprend le sujet.

5. **Session de conception micro-app avec Adrien** (~2h) — dans Cowork
   - Sur la base des DR : quels pain points / opportunités ressortent ?
   - Brainstorm : quelle(s) micro-app(s) démontreraient une compréhension profonde de l'AI appliquée à l'investissement ?
   - Critères : ça doit "parler" à un interlocuteur type NBIM, montrer qu'Élie comprend comment l'AI transforme le métier (pas juste automatiser), être réalisable en ~20-30h de vibe-coding
   - **Pistes à explorer** (à affiner avec les DR) :
     - Un "Investment Thesis Challenger" qui structure et stress-teste une thèse via adversarial prompting
     - Un "ESG Risk Scanner" inspiré de ce que fait NBIM (screening AI de portefeuille)
     - Un "Perception Gap Detector" qui identifie les dislocations entre narratif sell-side et fondamentaux
     - Un dashboard de veille AI-powered sur un secteur/thème
   - **Livrable** : un brief de conception (`output/micro-app-design.md`) — 1 ou 3 apps, scope, stack, ce que ça démontre

6. **Premiers pas vibe-coding** (~2h) — avec Claude Code
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

**⚠️ Ajustement** : weekend de Pâques (18-19 avril) non disponible. Le weekend du 19-20 avril est retiré du planning. Le contenu prévu est redistribué sur la semaine (lundi-vendredi) et sur le travail avancé des semaines précédentes.

### Semaine (lundi 20 – mercredi 23 avril) — ~12-15h

| Créneau | Activité | Durée | Notes |
|---------|----------|-------|-------|
| Lun matin/après-midi | Micro-app : derniers ajustements, bug fixes, polish | 2-3h | La micro-app doit être montrable, pas parfaite. |
| Lun soir | OpenClaw : check final — briefing calibré, skills stables | 1h | Vérifier que tout tourne sans intervention. |
| Mar après-midi | Narratif : finaliser le "AI story" d'Élie | 2h | Parcours, ce qu'il a construit, sa vision — structuré comme un pitch naturel. Sauvegarder dans `output/ai-narrative.md`. |
| Mar soir | Dry-run avec Claude : questions techniques AI + fit + micro-app | 1h30 | Claude joue recruteur NBIM. Mode adversarial : "prouve-moi que tu comprends vraiment." |
| Mer après-midi | Dry-run intensif avec Adrien | 2h | Feedback direct. Identifier les derniers trous. |
| Mer soir | Révision flashcards + cheat sheet | 1h | Ancrage final avant le départ. |
| Jeu soir | Relire les DR (NBIM surtout) avec un œil frais | 1h30 | Repérer les détails qui feront la différence en conversation. |
| Ven matin | Check final avec Adrien — go/no-go | 1h | Derniers ajustements. Questions à poser en Norvège. |

**Ce qu'Élie a à la fin de la semaine 4 (et du Phase 1)** :
- Une compréhension solide de l'IA générative, de son application en finance, et du paysage norvégien
- Un OpenClaw configuré et opérationnel — preuve tangible de compréhension agentique
- Une micro-app fonctionnelle et documentée — showcase de sa capacité à concevoir et builder avec l'IA
- Un narratif rodé pour les entretiens
- Les outils et la confiance pour continuer à apprendre (Phase 2+)

---

## Budget temps estimé

| Bloc | Heures | Notes |
|------|--------|-------|
| Semaine 1 — WE (dimanche 29 mars) | 8 | |
| Semaine 1 — Semaine (30 mars – 4 avril) | 18-22 | +1-2h/après-midi ajoutées |
| Semaine 2 — WE (sam 5 + dim 6 avril) | 16 | |
| Semaine 2 — Semaine (7–11 avril) | 10-12 | |
| Semaine 3 — WE (sam 12 + dim 13 avril) | 16 | |
| Semaine 3 — Semaine (14–18 avril) | 10-12 | |
| Semaine 4 — WE Pâques (18-19 avril) | 0 | ⚠️ Non disponible |
| Semaine 4 — Semaine (20–25 avril) | 12-15 | Contenu redistribué |
| **Total estimé** | **~90–101h** | Dans l'enveloppe cible |

La perte du weekend de Pâques (~16h) est compensée par les heures supplémentaires de la semaine 1 (~8-10h de gain) et une semaine 4 en semaine plus chargée.

---

*Ce document est une base vivante. Il sera mis à jour après chaque session.*

*Dernière mise à jour : 2026-03-28*
