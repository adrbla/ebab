# Brief — Brainstorming Voice Mode : Showcase App(s)

**Objectif de la session** : Explorer, ouvrir les perspectives, laisser émerger des idées. Ce n'est **pas** une session de décision — c'est une session de réflexion créative. Lis ce document avant de lancer la session voice, ou demande à Claude de te le résumer à voix haute.

**Posture** : Ping-pong avec Claude. Pose des questions, rebondis, contredis, explore les tangentes. Claude doit te stimuler, te challenger, te surprendre — pas converger trop vite. Si tu sens que la conversation se ferme sur une idée, rouvre-la délibérément.

**Attention** : tu as une tendance naturelle à vouloir fermer, choisir, décider rapidement (c'est une qualité d'analyste — mais pas ce qu'on veut ici). Résiste à cette impulsion. Si tu te surprends à dire "ok, on part sur ça" — stop, demande-toi "qu'est-ce que je n'ai pas encore exploré ?". La sélection fera l'objet d'une session séparée (vocal ou écrit, avec Adrien). Ici, on ouvre.

**Deadline build** : Semaine du 24 avril 2026. Mais la conception est un process — ne la précipite pas.

---

## 1. La vraie question

La question n'est **pas** "quelle app je construis ?" — c'est plus profond que ça :

**Comment l'IA peut-elle changer fondamentalement la façon dont un analyste travaille — pas juste accélérer ce qu'il fait déjà ?**

C'est la distinction clé : **innovation vs. optimisation**.

- **Optimisation** = automatiser un process existant (ex: résumer un earnings call plus vite). Utile, mais pas différenciant. N'importe qui peut le faire avec ChatGPT.
- **Innovation** = imaginer de nouvelles façons de travailler qui n'existaient pas avant l'IA (ex: un système qui détecte en temps réel les dislocations entre narratif sell-side et signaux fondamentaux). Ça, c'est ce qui fait lever un sourcil en entretien.

Pendant le brainstorm, chaque fois qu'une idée émerge, passe-la au filtre : **est-ce que ça optimise quelque chose d'existant, ou est-ce que ça ouvre une nouvelle possibilité ?** Les deux ont de la valeur, mais explore d'abord le côté innovation.

---

## 2. Seed ideas — matériel à réaction

Ces idées viennent du contexte du projet (DR reports + profil Élie + signaux marché Norway). Elles sont là pour **provoquer des réactions**, pas pour être adoptées. Pour chacune, demande-toi : qu'est-ce qui m'attire ? Qu'est-ce qui me laisse froid ? Qu'est-ce que ça m'évoque d'autre ?

### A — Earnings Signal Extractor
Prend une transcript d'earnings call et en extrait automatiquement : tone shift vs dernier quarter, sujets clés management, signaux de guidance implicites, questions analysts les plus incisives. Output : fiche structurée en 1 page.

### B — Perception Gap Screener
Pour une liste de tickers : consensus estimates + signaux qualitatifs récents, puis scoring automatique sur un axe "consensus too bullish / too bearish". Tableau de bord des positions les plus asymétriques.

### C — Nordic AM Radar
Dashboard qui agrège les mouvements publics des gérants norvégiens (NBIM, Storebrand, etc.), tague par secteur/thème, weekly digest formaté. UI navigable au-delà de ce qu'OpenClaw fait.

### D — ESG Flag Screener (inspired by NBIM)
Prend un rapport annuel ou un article, génère un "ESG flag report" : controverses, alignement exclusion criteria, score de risque. Inspiré directement de ce que NBIM fait avec Claude.

### E — Portfolio Diary / Investment Log
Log de thèses d'investissement + Claude génère des reminders, un tableau de cohérence portefeuille, une synthèse mensuelle "qu'est-ce qui a changé dans mes convictions".

### F — Norwegian Job Pulse
Dashboard job postings finance en Norvège avec scoring Claude sur "fit avec profil analyste L/S". Données réelles (finn.no).

---

### G — Cognitive Workflow Demo (idée émergente NotebookLM, 2026-03-31)
Pas une app — une démonstration de process de pensée instrumenté. Tu arrives en entretien, tu ouvres le laptop et tu montres : (1) une RAG architecture construite pour ingérer 10 ans de données supply chain non-structurées sur une société réelle, en support d'une thèse fondamentale ; (2) un script agent qui monitore des manifests en langue locale ; (3) des transcripts de sessions adversariales où tu as red-teamé ta propre thèse avec un LLM. Le fil directeur : tu es l'architecte de ton workflow cognitif, pas un consommateur passif de données.

*Pourquoi c'est différent des autres seeds* : ce n'est pas "regarde ce que j'ai construit", c'est "regarde comment je pense". Les artefacts sont des preuves d'un process, pas d'un produit. Très NBIM-adjacent (ils scannent des sources locales pour ESG — tu feras exactement la même chose pour de l'investment research).

---

## 3. Directions à explorer librement

Ne reste pas dans les seed ideas ci-dessus. Explore aussi :

- **Ce qui n'existe pas encore** — quel outil un analyste L/S n'a jamais eu mais dont il rêverait ? Pas un outil qui fait plus vite, un outil qui fait *autrement*.
- **Les moments de friction** — dans ton workflow quotidien à Trium, Pelham, Catalyst : où est-ce que tu perds du temps, de l'énergie, de la confiance ? Pas seulement "c'est lent" mais "c'est structurellement mal fait".
- **Le dernier kilomètre** — ton profil montre que tu arrives souvent à 70-80% de conviction mais que le dernier mile est dur. Y a-t-il un outil qui pourrait aider là-dessus spécifiquement ?
- **L'angle norvégien** — qu'est-ce qu'un outil pourrait montrer sur ta compréhension du marché norvégien qui serait impossible sans AI ?
- **Le méta** — une app qui montre comment tu *apprends* l'AI (ton propre parcours) pourrait être aussi parlante qu'une app qui *utilise* l'AI.

---

## 4. Questions que Claude devrait te poser pendant le brainstorm

(Claude : utilise ces prompts pour relancer la conversation quand elle se stabilise trop vite.)

- "Tu viens de décrire une optimisation — comment on transforme ça en innovation ?"
- "Si tu avais cet outil, qu'est-ce que tu ferais *différemment* dans ta journée — pas juste plus vite ?"
- "Qu'est-ce qui impressionnerait *toi* si un candidat te le montrait en entretien ?"
- "Est-ce que c'est un outil pour toi, ou un outil pour montrer que tu comprends quelque chose ?"
- "Et si on combinait deux de ces idées ?"
- "Quel est le truc le plus ambitieux que tu n'oserais pas proposer — et pourquoi tu n'oses pas ?"

---

## 5. Ce que cette session n'est PAS

- **Pas une session de décision** — on ne choisit pas d'app aujourd'hui.
- **Pas une session de faisabilité** — "est-ce que c'est buildable ?" viendra après, pas maintenant.
- **Pas une session d'optimisation** — ne te rabats pas sur "le plus simple à faire". Explore d'abord.

La conception se fera avec Adrien (semaine 2). Pour l'instant : ouvre, explore, surprends-toi.

---

## 6. Output attendu

À la fin du brainstorming, tu devrais avoir :
- Un nuage d'idées — certaines vagues, certaines précises, c'est normal
- Des fils rouges : quels thèmes reviennent ? Qu'est-ce qui t'excite le plus ?
- Des questions ouvertes pour la session de conception avec Adrien
- Surtout : une **énergie** sur 1-2 directions, pas une décision

---

*Brief préparé le 2026-03-30, révisé le 2026-03-31. Contexte : DR reports NBIM/Norway/buy-side + profil Élie + backlog EBAB.*
