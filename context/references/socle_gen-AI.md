# **Fondamentaux de l'Intelligence Artificielle Générative : Un Socle de Connaissances pour l'Analyse et la Recherche**

L'émergence de l'intelligence artificielle générative (IAG) au cours de la présente décennie ne constitue pas seulement une avancée technologique incrémentale, mais une mutation paradigmatique dans notre rapport à l'information et à la création de contenu. Pour les étudiants, chercheurs et professionnels issus de disciplines variées, cette technologie impose une compréhension rigoureuse qui dépasse le simple usage d'interfaces conversationnelles.1 Ce rapport analyse les fondements, les mécanismes et les architectures avancées de l'IA générative, offrant un cadre conceptuel solide pour naviguer dans ce nouvel écosystème.

## **1\. Découvrir l’IA générative**

L'intelligence artificielle générative s'inscrit dans une lignée historique de recherches visant à simuler les capacités cognitives humaines par le biais de systèmes computationnels. Pour comprendre cette technologie, il est impératif de la situer au sein de la hiérarchie des sciences de l'information.3

### **1.1 Définitions et panorama**

L'Intelligence Artificielle (IA) est la discipline mère qui regroupe l'ensemble des théories et techniques mises en œuvre en vue de réaliser des machines capables de simuler l'intelligence humaine.3 Traditionnellement, l'IA reposait sur des systèmes experts fondés sur des règles logiques explicites. Cependant, le passage au Machine Learning (Apprentissage Automatique) a marqué une transition vers des systèmes capables d'apprendre des motifs à partir de données, sans être explicitement programmés pour chaque tâche.1

Le Deep Learning (Apprentissage Profond) représente une spécialisation du machine learning utilisant des architectures de réseaux de neurones artificiels profonds, capables de traiter des données non structurées comme le texte, les images ou le son.6 Enfin, l'IA générative est une branche spécifique du deep learning dont l'objectif n'est pas seulement de classer ou de prédire, mais de produire de nouveaux contenus originaux (texte, code, images, audio, vidéo) en apprenant la distribution statistique des données d'entraînement.8

Les outils emblématiques de ce domaine incluent des modèles de langage tels que GPT-4 ou Claude pour le texte et le code, ainsi que des modèles de diffusion comme Midjourney ou Stable Diffusion pour l'image.10

### **1.2 Capacités, limites et risques**

L'IA générative excelle dans la manipulation du langage naturel. Elle est capable de générer des synthèses de documents complexes, de traduire des textes en conservant les nuances stylistiques, de reformuler des concepts pour différents publics et de servir d'outil d'idéation pour les chercheurs et créateurs.1 En analyse exploratoire, elle permet de structurer rapidement des données qualitatives massives.12

Néanmoins, ces systèmes présentent des limites intrinsèques majeures. Les "hallucinations" sont le risque le plus documenté : le modèle produit des affirmations fausses mais présentées avec une autorité convaincante, car il privilégie la probabilité linguistique sur la vérité factuelle.11 Par ailleurs, les biais et stéréotypes présents dans les données d'entraînement (souvent issues du web) sont systématiquement reproduits, ce qui pose des problèmes éthiques dans la recherche en sciences humaines et sociales.1 Enfin, les questions de confidentialité sont critiques : toute donnée partagée avec un modèle commercial peut, selon les conditions de service, être utilisée pour l'entraînement futur du système.1

### **1.3 Idées reçues et clarifications techniques**

Il est crucial de dissiper l'idée que l'IA fonctionne comme une gigantesque base de données. Contrairement à un moteur de recherche qui indexe et renvoie des documents existants, un modèle de langage est une structure probabiliste qui génère des réponses de manière dynamique.9 Il ne "cherche" pas l'information ; il "calcule" la suite de mots la plus logique.15

Une autre méprise concerne la mémoire des modèles. Dans une conversation, un système comme ChatGPT semble se souvenir du contexte, mais il est fondamentalement "stateless" (sans état).16 À chaque tour de conversation, l'intégralité de l'historique est renvoyée au modèle pour qu'il puisse générer la réponse suivante. C'est ce qu'on appelle la reconstruction du contexte dans la fenêtre de traitement.13

| Concept | Définition Simplifiée | Application Concrète |
| :---- | :---- | :---- |
| **IA Générative** | Systèmes créant du contenu original. | Rédaction d'un brouillon d'article. |
| **Hallucination** | Erreur factuelle plausible. | Invention d'une source bibliographique. |
| **Stateless** | Absence de mémoire interne permanente. | Nécessité de répéter le contexte à chaque requête. |
| **Biais** | Préjugés issus des données d'entraînement. | Représentations stéréotypées des genres. |

#### **Idées clés à retenir (Section 1\)**

* L'IA générative crée du contenu neuf plutôt que de simplement trier l'existant.8  
* Elle repose sur des couches successives : IA \> Machine Learning \> Deep Learning.6  
* Les modèles sont des prédicteurs statistiques et non des bases de données.9  
* L'absence de mémoire intrinsèque impose de fournir le contexte à chaque fois (stateless).16  
* Les hallucinations sont structurelles et non accidentelles.11  
* La protection des données sensibles doit être une priorité absolue pour les professionnels.1

#### **Mini‑FAQ (Section 1\)**

**Q : L'IA a-t-elle une conscience?** R : Non, il s'agit d'un algorithme probabiliste sophistiqué dénué d'intentionnalité ou de compréhension du monde.6

**Q : Pourquoi ChatGPT semble-t-il se souvenir de mes messages précédents?** R : Parce que l'interface renvoie tout l'historique de la discussion à chaque nouveau message pour "rafraîchir" sa mémoire de travail.16

**Q : Est-ce que l'IA peut remplacer un chercheur?** R : Elle agit comme un assistant puissant pour la synthèse et l'idéation, mais manque de rigueur critique et de capacité de découverte scientifique autonome.8

**Q : Comment éviter les biais dans les résultats?** R : En diversifiant les sources de données et en exerçant une critique systématique des réponses fournies par le modèle.1

**Q : L'IA "sait-elle" quand elle ment?** R : Non, elle ne fait que prédire le token suivant le plus probable. Elle n'a aucune notion de vérité ou de mensonge.9

## ---

**2\. Comment ça marche, grosso modo?**

La compréhension du fonctionnement des grands modèles de langage (LLM) nécessite de saisir l'équilibre entre les mathématiques statistiques et les architectures neuronales complexes.

### **2.1 Apprendre à partir de données : Entraînement vs Inférence**

Le processus se divise en deux phases distinctes. L'entraînement est une phase de calcul massive où le modèle analyse des pétaoctets de texte pour ajuster ses paramètres internes.6 Durant cette phase, le modèle tente de minimiser une fonction de perte, c'est-à-dire l'écart entre sa prédiction et le mot réel dans le texte d'entraînement. L'inférence est la phase d'utilisation : le modèle est figé, ses paramètres ne changent plus, et il répond aux requêtes des utilisateurs.6

L'idée centrale est celle de l'approximation statistique. Le modèle ne comprend pas la grammaire au sens linguistique ; il en saisit les régularités statistiques. Il n'apprend pas la logique, mais la corrélation entre les concepts.6

### **2.2 Réseaux de neurones et paramètres**

Un réseau de neurones artificiels est un ensemble de fonctions mathématiques organisées en couches. Chaque "neurone" reçoit des entrées, leur applique un poids (importance relative) et un biais, puis passe le résultat à travers une fonction d'activation.6

Les paramètres du modèle (souvent des milliards) sont les poids qui déterminent la force des connexions entre ces neurones. C'est dans ces paramètres qu'est "stocké" le savoir du modèle.6 Intuitivement, on peut imaginer un immense tableau de bord avec des milliards de curseurs que l'on ajuste jusqu'à ce que la machine produise des phrases cohérentes.5

### **2.3 L’architecture Transformer et les Tokens**

Les LLM traitent le texte par unités appelées tokens. Un token peut être un mot, une partie de mot ou un signe de ponctuation.6 En moyenne, 100 tokens correspondent à environ 75 mots en anglais.13

L'architecture Transformer (le "T" de GPT) a révolutionné le domaine grâce au mécanisme d'auto-attention (self-attention). Ce mécanisme permet au modèle de traiter tous les mots d'une phrase simultanément et de comprendre les relations de longue distance entre eux.9 Par exemple, dans la phrase "La banque a refusé le prêt car elle est trop prudente", le mécanisme d'attention permet au modèle de comprendre que "elle" se rapporte à "la banque" et non au "prêt".15

Mathématiquement, pour chaque token, le modèle calcule trois vecteurs :

* **La Requête (Query \- Q) :** "Ce que je cherche dans mon contexte."  
* **La Clé (Key \- K) :** "Ce que je propose comme information aux autres."  
* **La Valeur (Value \- V) :** "Le contenu informationnel que je partage.".15

Le score d'attention est obtenu par le produit scalaire entre la Requête d'un mot et les Clés des autres, permettant de pondérer l'importance de chaque mot pour la compréhension du token actuel.15

### **2.4 Paramètres de génération**

La génération n'est pas un processus fixe ; elle est modulée par des hyperparamètres d'échantillonnage :

* **Temperature :** Contrôle le caractère aléatoire. Une température basse (![][image1] à ![][image2]) rend les réponses prévisibles et cohérentes (idéal pour le code). Une température élevée (![][image3] à ![][image4]) favorise la diversité et la créativité, mais augmente le risque d'incohérence.13  
* **Top‑p / Top‑k :** Ces techniques limitent le choix du prochain mot aux tokens les plus probables dont la somme des probabilités atteint un seuil ![][image5], ou aux ![][image6] meilleurs tokens, évitant ainsi de choisir des mots totalement hors de propos.15  
* **Max Tokens :** Définit la longueur maximale de la réponse générée.10

| Paramètre | Effet à Valeur Basse | Effet à Valeur Haute |
| :---- | :---- | :---- |
| **Temperature** | Déterministe, factuel, répétitif. | Créatif, varié, imprévisible. |
| **Top-p** | Sélection très restreinte. | Vocabulaire plus riche et risqué. |
| **Max Tokens** | Réponses courtes et tronquées. | Synthèses longues et détaillées. |

#### **Idées clés à retenir (Section 2\)**

* L'entraînement est la phase d'apprentissage globale, l'inférence est la phase de réponse.6  
* Un token est l'unité de base de traitement, plus granulaire qu'un mot.6  
* Le Transformer utilise l'auto-attention pour saisir le contexte global d'une séquence.9  
* La prédiction du prochain token est purement probabiliste.13  
* Les paramètres (poids) sont le résultat de l'entraînement et définissent l'intelligence du modèle.6  
* La température est le levier principal pour ajuster la créativité du modèle.13

#### **Mini‑FAQ (Section 2\)**

**Q : Pourquoi mon IA change-t-elle de réponse pour la même question?** R : En raison de l'échantillonnage probabiliste et de la température qui introduisent une part d'aléa volontaire.13

**Q : Qu'est-ce qu'un Transformer?** R : C'est une architecture de réseau de neurones capable de traiter les données en parallèle et de se concentrer sur les parties les plus pertinentes d'une entrée grâce à l'attention.9

**Q : Un modèle avec plus de paramètres est-il toujours meilleur?** R : Généralement oui pour la complexité du raisonnement, mais il est aussi plus lent et coûteux en énergie.6

**Q : Comment l'IA connaît-elle l'ordre des mots?** R : Par le codage positionnel, qui ajoute des informations mathématiques sur la place de chaque token dans la phrase.15

**Q : Qu'est-ce que la phase de fine-tuning?** R : C'est un entraînement complémentaire sur un jeu de données spécialisé pour adapter un modèle généraliste à un domaine précis (ex: droit ou médecine).6

## ---

**3\. Bien parler à un modèle : les prompts**

L'ingénierie de prompt (prompt engineering) consiste à structurer les instructions envoyées au modèle pour maximiser la pertinence et la précision de la réponse.11

### **3.1 Notion de prompt et d'alignement**

Un prompt est le texte d'entrée qui sert de base au calcul probabiliste du modèle. L'alignement est l'effort constant pour s'assurer que le modèle répond conformément aux intentions humaines et aux valeurs de sécurité.14 Un mauvais prompt est ambigu ("Parle-moi d'histoire"), tandis qu'un bon prompt est spécifique ("Résume les causes de la Révolution française en 5 points pour un lycéen").

### **3.2 Types de prompts et hiérarchie**

L'interaction avec un modèle moderne repose sur une structure hiérarchique des instructions :

* **Prompt système (System prompt) :** Il définit le rôle permanent du modèle, ses contraintes et son ton. C'est le socle de la personnalité de l'IA.14  
  * *Exemple de rôle :* "Tu es un tuteur pédagogique expert en sciences physiques. Utilise des analogies simples et vérifie toujours la compréhension de l'élève avant d'avancer."  
* **Prompt utilisateur (User prompt) :** C'est la requête spécifique liée à une tâche immédiate.14  
* **Few‑shot prompting :** Cette technique consiste à fournir quelques exemples de paires "Entrée/Sortie" dans le prompt pour aider le modèle à comprendre un format ou un style complexe.17

### **3.3 Bonnes pratiques de rédaction**

Un prompt efficace doit clarifier trois dimensions essentielles :

1. **Le Contexte :** Qui parle à qui? Quel est le but ultime?.14  
2. **La Tâche :** Quel est le verbe d'action (comparer, synthétiser, corriger)?.14  
3. **Le Format de sortie :** Liste, tableau Markdown, code JSON, ou plan détaillé.14

Il est également recommandé d'inviter le modèle à poser des questions de clarification avant de générer le résultat final : "Si ma demande est incomplète, pose-moi des questions pour préciser mon besoin avant de rédiger".14

| Stratégie | Description | Exemple |
| :---- | :---- | :---- |
| **Zero-shot** | Demande directe sans exemple. | "Traduis ce texte en latin." |
| **Few-shot** | Demande avec 2-3 exemples. | "Texte: Chat \-\> Latin: Felis. Texte: Chien \-\> Latin: Canis. Texte: Oiseau \-\> Latin:" |
| **Chain of Thought** | Demande de raisonnement étape par étape. | "Résous ce problème de maths en détaillant chaque étape de ton calcul." |

#### **Idées clés à retenir (Section 3\)**

* La qualité de l'entrée détermine la qualité de la sortie (principe GIGO : Garbage In, Garbage Out).11  
* Le prompt système définit le cadre comportemental et éthique.17  
* Le few-shot prompting est l'un des moyens les plus puissants pour guider le modèle.17  
* La structure "Rôle \+ Contexte \+ Tâche \+ Format" est le standard de l'efficacité.14  
* Le "Chain of Thought" aide le modèle à éviter les erreurs de logique complexes.17  
* Demander des clarifications au modèle réduit les approximations.14

#### **Mini‑FAQ (Section 3\)**

**Q : C'est quoi un "Persona" dans un prompt?** R : C'est une technique consistant à demander au modèle d'agir comme un expert spécifique (ex: "Agis en tant qu'analyste financier") pour orienter son style et son vocabulaire.14

**Q : Pourquoi donner des exemples (few-shot) fonctionne si bien?** R : Parce que cela réduit l'incertitude statistique du modèle en lui montrant le motif (pattern) exact attendu.17

**Q : Faut-il être poli avec l'IA?** R : Ce n'est pas techniquement nécessaire pour l'algorithme, mais cela peut influencer le ton de la réponse du modèle qui imite les interactions humaines polies présentes dans ses données.11

**Q : Quelle est la longueur idéale d'un prompt?** R : Il doit être suffisamment détaillé pour donner tout le contexte nécessaire, mais assez direct pour ne pas diluer l'instruction principale dans des détails inutiles.17

**Q : Qu'est-ce qu'une "instruction négative"?** R : C'est une contrainte indiquant au modèle ce qu'il ne doit pas faire (ex: "N'utilise pas de jargon technique").14

## ---

**4\. D’où viennent les informations? Contexte & RAG**

L'un des enjeux majeurs de l'IAG est l'accès à l'information fraîche et vérifiée, car les modèles sont limités par leur date de fin d'entraînement (knowledge cutoff).1

### **4.1 Connaissances apprises vs Contexte fourni**

On distingue deux sources d'information pour le modèle :

* **Connaissances paramétriques :** Ce que le modèle a appris lors de son entraînement initial sur le web et les livres. Ces connaissances sont figées et peuvent être obsolètes.6  
* **Connaissances contextuelles :** Les informations fournies dynamiquement dans la fenêtre de contexte (le prompt actuel). Le modèle peut raisonner sur ces données même s'il ne les connaissait pas auparavant.13

La fenêtre de contexte est la limite physique (en tokens) de ce que le modèle peut "voir" à un instant donné. Une fenêtre trop petite entraîne une perte d'information lors de longs dialogues.13

### **4.2 Retrieval‑Augmented Generation (RAG)**

Le RAG est une architecture qui combine la puissance de raisonnement du LLM avec un moteur de recherche externe. Au lieu de compter sur sa mémoire interne faillible, le système :

1. **Récupère (Retrieval) :** Cherche des extraits pertinents dans une base de documents fiable (PDF, rapports, web) en fonction de la question de l'utilisateur.15  
2. **Augmente (Augmentation) :** Insère ces extraits dans le prompt comme contexte.15  
3. **Génère (Generation) :** Demande au modèle de répondre en s'appuyant exclusivement sur les documents fournis.15

Le RAG est la solution standard pour réduire les hallucinations et garantir que l'IA parle de données internes confidentielles ou récentes.20

### **4.3 Formes de stockage et de recherche sémantique**

Pour trouver les bons documents dans un RAG, plusieurs techniques coexistent :

* **Recherche par mots‑clés (BM25 / Sparse) :** Recherche classique type "moteur de recherche" qui cherche la correspondance exacte des termes. Très efficace pour les noms propres ou les termes techniques précis.22  
* **Recherche vectorielle (Dense / Embeddings) :** Utilise des modèles de plongement pour transformer chaque paragraphe en un vecteur (une liste de nombres) représentant son sens. On calcule la similarité cosinus entre la question et les documents pour trouver des réponses même si les mots exacts sont différents (recherche sémantique).15  
* **Recherche hybride :** Combine les deux méthodes pour capturer à la fois la précision des mots-clés et la richesse du sens sémantique.22  
* **NL2SQL :** Technique consistant à traduire une question en langage naturel en requête SQL pour interroger des bases de données structurées (tables, colonnes).21  
* **Graphes de connaissance :** Représentent les données sous forme de nœuds (entités) et de liens (relations). Ils permettent de répondre à des questions complexes de type "X est-il lié à Y par un intermédiaire?".28

| Technologie | Usage Idéal | Analogie |
| :---- | :---- | :---- |
| **Vecteurs** | Trouver des concepts ou des idées proches. | Demander à un bibliothécaire un livre "triste". |
| **Mots-clés** | Trouver une référence précise ou un ID. | Chercher un nom dans l'annuaire. |
| **NL2SQL** | Analyser des chiffres dans un tableau. | Demander à un comptable d'extraire un bilan. |
| **Graphes** | Comprendre des relations complexes. | Explorer un arbre généalogique. |

#### **Idées clés à retenir (Section 4\)**

* Le RAG connecte l'IA à des données fraîches et privées sans ré-entraînement.20  
* Les embeddings permettent une recherche par le sens plutôt que par les mots exacts.15  
* La fenêtre de contexte est la "mémoire de travail" immédiate du modèle.16  
* La recherche hybride est le standard pour une fiabilité maximale.22  
* Le NL2SQL permet d'interroger des bases de données chiffrées sans connaître le code.21  
* Les graphes de connaissance capturent des relations métier complexes que les vecteurs ignorent.28

#### **Mini‑FAQ (Section 4\)**

**Q : Pourquoi ne pas simplement mettre tout mon dossier dans le prompt?** R : Parce que le coût et la performance se dégradent avec la longueur, et que le modèle finit par "se perdre" dans trop d'informations (phénomène du "lost in the middle").13

**Q : Qu'est-ce qu'un "Embedding"?** R : C'est une traduction mathématique d'un texte en un vecteur numérique où les distances entre vecteurs reflètent la proximité de sens.6

**Q : Le RAG protège-t-il mes données?** R : Oui, s'il est déployé localement ou sur un cloud privé, car les données ne servent pas à entraîner le modèle de base ; elles sont juste lues temporairement.1

**Q : Quelle est la différence entre une base de données SQL et un Graphe?** R : SQL stocke des tables rigides ; le Graphe stocke des connexions souples et multidirectionnelles entre les entités.28

**Q : Qu'est-ce qu'un "Knowledge Cutoff"?** R : C'est la date de la dernière information vue par le modèle lors de son entraînement final.1

## ---

**5\. Les agents : LLM \+ tools \+ skills**

L'étape ultime de l'évolution de l'IA est le passage de l'assistance textuelle à l'action autonome via les agents intelligents.31

### **5.1 Définition d’un agent**

Un agent est un système basé sur un LLM qui ne se contente pas de répondre, mais qui utilise des outils pour accomplir un objectif complexe. Un agent peut planifier des étapes, utiliser des logiciels tiers et corriger ses erreurs au fil de l'exécution.19 Il est défini par :

* **Un Objectif :** Une mission claire (ex: "Fais une veille hebdomadaire sur les brevets éoliens").  
* **Des Outils (Tools) :** Des capacités d'action concrètes (APIs, scripts).  
* **Des Compétences (Skills) :** Des savoir-faire méthodologiques packagés.18

### **5.2 Tools (Les Mains)**

Un tool est une fonction exécutable par l'agent. Contrairement à la génération de texte, l'appel d'un tool produit un effet dans le monde réel ou sur un système d'information 19 :

* Exécuter une requête SQL.  
* Envoyer un e-mail ou un message Slack.  
* Lire un fichier PDF ou écrire un rapport Word.  
* Appeler une API financière ou un CRM.19

### **5.3 Skills (Le Savoir‑faire)**

Un skill est une expertise encapsulée (souvent un prompt complexe ou un workflow) qui enseigne à l'agent *comment* utiliser les tools pour une tâche spécifique.18

* **Skill d'analyse scientifique :** Extraire les limites méthodologiques d'une étude.  
* **Skill financier :** Identifier les anomalies dans un compte de résultat.  
* **Skill utilisateur :** Classer des retours clients par sentiment et urgence.18

### **5.4 Exemples d’agents dans des processus métiers**

L'intégration d'agents transforme les pipelines de travail classiques :

* **Agent de veille scientifique :** Il utilise des tools (API de recherche d'articles) et des skills (résumé technique) pour produire un rapport synthétique quotidien sans intervention humaine.12  
* **Agent de reporting financier :** Il interroge l'entrepôt de données (tool SQL), analyse les écarts (skill financier) et génère un document de synthèse (tool écriture).35  
* **Agent d'ETL sémantique :** Il transforme des fichiers bruts et désordonnés en bases de données propres en utilisant le raisonnement du LLM pour structurer les données non structurées.37

### **5.5 Bonnes pratiques et boucle humaine**

L'autonomie des agents nécessite des garde‑fous. Le principe de la "Boucle Humaine" (Human‑in‑the‑loop) est essentiel pour valider les étapes critiques, particulièrement lorsqu'un agent a le pouvoir d'écrire ou de modifier des données sensibles.13

| Entité | Fonction | Exemple |
| :---- | :---- | :---- |
| **Agent** | Orchestrateur de tâches. | Gestionnaire de projet IA. |
| **Tool** | Action technique. | "Envoyer un e-mail". |
| **Skill** | Méthodologie. | "Savoir rédiger un e-mail professionnel". |
| **Pipeline** | Enchaînement. | Récupération \-\> Analyse \-\> Envoi. |

#### **Idées clés à retenir (Section 5\)**

* Un agent est une IA proactive centrée sur des objectifs.31  
* Les tools sont les capacités d'exécution concrètes (APIs, scripts).19  
* Les skills sont l'expertise métier intégrée sous forme d'instructions.18  
* Un agent décompose un objectif complexe en sous-tâches réalisables.31  
* La boucle humaine est vitale pour la sécurité et la conformité.13  
* L'agenticité permet d'automatiser des workflows complets et non juste des réponses isolées.33

#### **Mini‑FAQ (Section 5\)**

**Q : Quelle est la différence entre un "Bot" et un "Agent"?** R : Un bot suit des règles fixes ; un agent raisonne, planifie et s'adapte à des situations imprévues en utilisant des outils.31

**Q : Est-ce qu'un agent peut "voler" des données?** R : Un agent ne peut accéder qu'aux outils (APIs) auxquels l'humain lui a donné l'autorisation explicite via des clés d'accès sécurisées.14

**Q : Comment un agent sait-il quel outil utiliser?** R : Le LLM lit la description de chaque outil fourni dans son contexte et choisit celui dont la définition correspond le mieux à l'étape actuelle de son plan.19

**Q : Qu'est-ce qu'un "Multi-agent"?** R : C'est une architecture où plusieurs agents spécialisés collaborent (ex: un agent chercheur et un agent rédacteur) pour résoudre un problème.33

**Q : Est-ce que les agents apprennent de leurs erreurs?** R : Oui, grâce à des boucles de réflexion (reflection) où ils analysent le résultat de leur action précédente pour corriger le tir lors de la suivante.31

### ---

**Ressources en français recommandées (par section)**

**Section 1 : Découvrir l'IA générative**

* **Article :** "IA générative : fondamentaux pour les créateurs d'entreprise", Bpifrance Université, 2025\. 42  
* **Guide :** "IA pour les enseignants : un manuel ouvert", Ministère de l'Éducation (AI4T), 2023\. 2  
* **Page web :** "Tout savoir sur l'intelligence artificielle générative", France Num, 2024\. 14

**Section 2 : Fonctionnement technique**

* **Article :** "LLM, tokens et fine-tuning : comprendre le fonctionnement réel", Edana, 2025\. 6  
* **Vidéo/Cours :** "Cours intensif sur l'apprentissage automatique : LLM", Google Developers (version FR), 2024\. 9  
* **Synthèse :** "Architecture Transformer et probabilités", DRANE Versailles, 2024\. 13

**Section 3 : Prompt Engineering**

* **Guide :** "Comment créer des prompts efficaces : guide du débutant", France Num, 2024\. 14  
* **Manuel :** "GenAI Handbook : Maîtriser le dialogue avec l'IA", Cognizant, 2024\. 1

**Section 4 : Contexte et RAG**

* **Article :** "Qu'est-ce que la recherche sémantique?", Elastic.co (FR), 2024\. 24  
* **Documentation :** "Comprendre les bases de données vectorielles", MongoDB (FR), 2025\. 43  
* **Blog :** "Graphe de connaissances vs base de données relationnelle", AWS (FR), 2024\. 28

**Section 5 : Agents et action**

* **Article :** "Le futur de l'IA : des agents autonomes aux workflows", ChapsVision, 2024\. 12  
* **Blog :** "Différence entre agents IA, assistants et bots", Google Cloud Discover (FR), 2024\. 39

### ---

**Ressources en anglais recommandées (par section)**

**Section 1 : Découvrir l'IA générative**

* **Article :** "Learn About AI : Key terms and practical examples", Yale University, 2024\. 11  
* **Glossary :** "AI Beginner's Cybersecurity Guide", Splunk, 2024\. 3

**Section 2 : Fonctionnement technique**

* **Interactive Tool :** "Transformer Explainer : Learn How LLMs Work", Georgia Tech, 2024\. 13  
* **Article :** "What is a Transformer Model?", IBM Think, 2025\. 15

**Section 3 : Prompt Engineering**

* **Documentation :** "System Prompt Engineering in Gen AI Applications", Belitsoft, 2024\. 17  
* **Course :** "ChatGPT Prompt Engineering for Developers", DeepLearning.AI, 2024\. 44

**Section 4 : Contexte et RAG**

* **Course :** "Retrieval-Augmented Generation (RAG) Bootcamp", ZeroToMastery, 2024\. 20  
* **Blog :** "Dense vs Sparse vs Hybrid Search : Which RAG technique actually works?", Medium, 2025\. 25

**Section 5 : Agents et action**

* **Article :** "Tasks, Skills, and Tools: The Essential AI Agent Framework", Agentic Academy, 2026\. 18  
* **Technical Guide :** "What are Agent Skills and Tools?", Arcade.dev, 2025\. 19

#### **Sources des citations**

1. Guide pratique de l'IA générative \- Cognizant, consulté le mars 28, 2026, [https://www.cognizant.com/fr/fr/documents/gen-ai-handbook-fr.pdf](https://www.cognizant.com/fr/fr/documents/gen-ai-handbook-fr.pdf)  
2. IA pour les enseignants : un manuel ouvert \- STI, consulté le mars 28, 2026, [https://sti.ac-versailles.fr/IMG/pdf/ia-pour-les-enseignants-un-manuel-ouvert.pdf](https://sti.ac-versailles.fr/IMG/pdf/ia-pour-les-enseignants-un-manuel-ouvert.pdf)  
3. AI for Humans: A Beginner's Field Guide \- Splunk, consulté le mars 28, 2026, [https://www.splunk.com/en\_us/blog/security/ai-beginners-cybersecurity-guide.html](https://www.splunk.com/en_us/blog/security/ai-beginners-cybersecurity-guide.html)  
4. Science des données et intelligence artificielle : différences entre les domaines \- AWS, consulté le mars 28, 2026, [https://aws.amazon.com/fr/compare/the-difference-between-data-science-and-ai/](https://aws.amazon.com/fr/compare/the-difference-between-data-science-and-ai/)  
5. \[LUM\#22\] Pas d'IA sans humain \- Université de Montpellier, consulté le mars 28, 2026, [https://www.umontpellier.fr/articles/pas-dia-sans-humain](https://www.umontpellier.fr/articles/pas-dia-sans-humain)  
6. Comprendre les LLM : tokens, fine-tuning et IA générative \- Edana, consulté le mars 28, 2026, [https://edana.ch/2025/07/24/llm-tokens-fine-tuning-comprendre-comment-fonctionnent-reellement-les-modeles-dia-generative/](https://edana.ch/2025/07/24/llm-tokens-fine-tuning-comprendre-comment-fonctionnent-reellement-les-modeles-dia-generative/)  
7. Comment l'IA s'intègre à la science des données | Dauphine Executive Education Paris, consulté le mars 28, 2026, [https://executive-education.dauphine.psl.eu/evenements-actualites/article/comment-ia-integre-science-donnees](https://executive-education.dauphine.psl.eu/evenements-actualites/article/comment-ia-integre-science-donnees)  
8. Intégrer l'IA générative dans les stratégies ... \- OER-UCLouvain, consulté le mars 28, 2026, [https://oer.uclouvain.be/jspui/bitstream/20.500.12279/1089.3/6/CahierLLL\_IAG\_OKOER.pdf](https://oer.uclouvain.be/jspui/bitstream/20.500.12279/1089.3/6/CahierLLL_IAG_OKOER.pdf)  
9. LLM: qu'est-ce qu'un grand modèle de langage ? | Machine Learning, consulté le mars 28, 2026, [https://developers.google.com/machine-learning/crash-course/llm/transformers?hl=fr](https://developers.google.com/machine-learning/crash-course/llm/transformers?hl=fr)  
10. Le guide pratique de l'IA Générative \- 365Talents, consulté le mars 28, 2026, [https://365talents.com/wp-content/uploads/2025/04/FR\_GenerativeAI\_Workbook.pdf](https://365talents.com/wp-content/uploads/2025/04/FR_GenerativeAI_Workbook.pdf)  
11. Learn About AI \- AI at Yale, consulté le mars 28, 2026, [https://ai.yale.edu/guidance/learn-about-ai](https://ai.yale.edu/guidance/learn-about-ai)  
12. Veille scientifique : suivre efficacement les avancées R\&D avec l'IA \- ChapsVision, consulté le mars 28, 2026, [https://www.chapsvision.com/fr/blog/veille-scientifique-innovation/](https://www.chapsvision.com/fr/blog/veille-scientifique-innovation/)  
13. Comment une IA générative crée-t-elle du texte \- Délégation ..., consulté le mars 28, 2026, [https://drane-versailles.region-academique-idf.fr/spip.php?article845](https://drane-versailles.region-academique-idf.fr/spip.php?article845)  
14. IA générative : 5 compétences clés à acquérir pour bien l'utiliser \- francenum.gouv.fr, consulté le mars 28, 2026, [https://www.francenum.gouv.fr/guides-et-conseils/intelligence-artificielle/generation-de-contenus-texte-image-son-video/ia](https://www.francenum.gouv.fr/guides-et-conseils/intelligence-artificielle/generation-de-contenus-texte-image-son-video/ia)  
15. Qu'est-ce qu'un modèle de transformeur ? | IBM, consulté le mars 28, 2026, [https://www.ibm.com/fr-fr/think/topics/transformer-model](https://www.ibm.com/fr-fr/think/topics/transformer-model)  
16. Applications stateful et stateless \- Red Hat, consulté le mars 28, 2026, [https://www.redhat.com/fr/topics/cloud-native-apps/stateful-vs-stateless](https://www.redhat.com/fr/topics/cloud-native-apps/stateful-vs-stateless)  
17. System Prompt Engineering in Gen AI Applications | Belitsoft, consulté le mars 28, 2026, [https://belitsoft.com/system-prompt-engineering-in-gen-ai-applications](https://belitsoft.com/system-prompt-engineering-in-gen-ai-applications)  
18. Tasks, Skills, and Tools: The Essential AI Agent Framework, consulté le mars 28, 2026, [https://agentic-academy.ai/posts/tasks-skills-and-tools-the-holy-trinity-of-ai-agents/](https://agentic-academy.ai/posts/tasks-skills-and-tools-the-holy-trinity-of-ai-agents/)  
19. Skills vs Tools for AI Agents: Production Guide \- Arcade.dev, consulté le mars 28, 2026, [https://www.arcade.dev/blog/what-are-agent-skills-and-tools/](https://www.arcade.dev/blog/what-are-agent-skills-and-tools/)  
20. The RAG Bootcamp. Build Smarter LLMs. Become an AI Engineer | Zero To Mastery, consulté le mars 28, 2026, [https://zerotomastery.io/courses/ai-engineer-bootcamp-retrieval-augmented-generation/](https://zerotomastery.io/courses/ai-engineer-bootcamp-retrieval-augmented-generation/)  
21. Build a RAG agent with LangChain, consulté le mars 28, 2026, [https://docs.langchain.com/oss/python/langchain/rag](https://docs.langchain.com/oss/python/langchain/rag)  
22. RAG Retrieval Strategies: Sparse, Dense, and Hybrid — How to Choose and Implement, consulté le mars 28, 2026, [https://rajnandan.medium.com/rag-retrieval-strategies-sparse-dense-and-hybrid-how-to-choose-and-implement-7eaec4e65da9](https://rajnandan.medium.com/rag-retrieval-strategies-sparse-dense-and-hybrid-how-to-choose-and-implement-7eaec4e65da9)  
23. Dense vs Sparse Retrieval: Mastering FAISS, BM25, and Hybrid Search \- DEV Community, consulté le mars 28, 2026, [https://dev.to/qvfagundes/dense-vs-sparse-retrieval-mastering-faiss-bm25-and-hybrid-search-4kb1](https://dev.to/qvfagundes/dense-vs-sparse-retrieval-mastering-faiss-bm25-and-hybrid-search-4kb1)  
24. Qu'est-ce que la recherche sémantique \- Elastic, consulté le mars 28, 2026, [https://www.elastic.co/fr/what-is/semantic-search](https://www.elastic.co/fr/what-is/semantic-search)  
25. Dense vs Sparse vs Hybrid RRF: Which RAG Technique Actually Works? | by Robert Dennyson | Medium, consulté le mars 28, 2026, [https://medium.com/@robertdennyson/dense-vs-sparse-vs-hybrid-rrf-which-rag-technique-actually-works-1228c0ae3f69](https://medium.com/@robertdennyson/dense-vs-sparse-vs-hybrid-rrf-which-rag-technique-actually-works-1228c0ae3f69)  
26. Candidate Retrieval: Dense and Hybrid Search \- Emergent Mind, consulté le mars 28, 2026, [https://www.emergentmind.com/topics/candidate-retrieval-dense-hybrid-search](https://www.emergentmind.com/topics/candidate-retrieval-dense-hybrid-search)  
27. Trouvez facilement des solutions avec les fonctionnalités de modélisation | Oracle Canada, consulté le mars 28, 2026, [https://www.oracle.com/ca-fr/analytics/capabilities/model/](https://www.oracle.com/ca-fr/analytics/capabilities/model/)  
28. Base de données orientée graphe vs base de données relationnelle \- différence entre les bases de données \- AWS, consulté le mars 28, 2026, [https://aws.amazon.com/fr/compare/the-difference-between-graph-and-relational-database/](https://aws.amazon.com/fr/compare/the-difference-between-graph-and-relational-database/)  
29. Qu'est-ce qu'un graphe de connaissances ? \- SAP, consulté le mars 28, 2026, [https://www.sap.com/france/resources/knowledge-graph](https://www.sap.com/france/resources/knowledge-graph)  
30. Mais qu'est-ce qu'un graphe de connaissances? (et autres questions toutes aussi pertinentes), consulté le mars 28, 2026, [https://linkeddigitalfuture.ca/fr/2019/09/12/graphe-de-connaissances/](https://linkeddigitalfuture.ca/fr/2019/09/12/graphe-de-connaissances/)  
31. Que sont les agents d'IA? \- ServiceNow, consulté le mars 28, 2026, [https://www.servicenow.com/fr-ca/products/ai-agents/what-are-ai-agents.html](https://www.servicenow.com/fr-ca/products/ai-agents/what-are-ai-agents.html)  
32. Semantic Kernel Agent Framework | Microsoft Learn, consulté le mars 28, 2026, [https://learn.microsoft.com/en-us/semantic-kernel/frameworks/agent/](https://learn.microsoft.com/en-us/semantic-kernel/frameworks/agent/)  
33. Microsoft Agent Framework Overview, consulté le mars 28, 2026, [https://learn.microsoft.com/en-us/agent-framework/overview/](https://learn.microsoft.com/en-us/agent-framework/overview/)  
34. Introduction to Contextual AI: MCP Tools vs Skills \- Uno Platform, consulté le mars 28, 2026, [https://platform.uno/blog/contextual-ai-mcptools-vs-skills/](https://platform.uno/blog/contextual-ai-mcptools-vs-skills/)  
35. AI Agent for Finance \- IBM watsonx Orchestrate, consulté le mars 28, 2026, [https://www.ibm.com/products/watsonx-orchestrate/ai-agent-for-finance](https://www.ibm.com/products/watsonx-orchestrate/ai-agent-for-finance)  
36. 5 Use Cases for AI Agents in Finance: Drive ROI With a Strategic AI Pilot, consulté le mars 28, 2026, [https://centricconsulting.com/blog/5-use-cases-for-ai-agents-in-finance-drive-roi-with-a-strategic-ai-pilot\_ai/](https://centricconsulting.com/blog/5-use-cases-for-ai-agents-in-finance-drive-roi-with-a-strategic-ai-pilot_ai/)  
37. AI ETL: How Artificial Intelligence Automates Data Pipelines ..., consulté le mars 28, 2026, [https://www.databricks.com/blog/ai-etl-how-artificial-intelligence-automates-data-pipelines](https://www.databricks.com/blog/ai-etl-how-artificial-intelligence-automates-data-pipelines)  
38. Compétences essentielles pour gérer les agents d'IA dans une entreprise \- Agentix Labs, consulté le mars 28, 2026, [https://www.agentixlabs.com/fr/blog/g%C3%A9n%C3%A9ral/comp%C3%A9tences-essentielles-pour-g%C3%A9rer-les-agents-d%27IA-dans-une-entreprise-moderne/](https://www.agentixlabs.com/fr/blog/g%C3%A9n%C3%A9ral/comp%C3%A9tences-essentielles-pour-g%C3%A9rer-les-agents-d%27IA-dans-une-entreprise-moderne/)  
39. Qu'est-ce qu'un agent d'IA ? Définition, exemples et types | Google Cloud, consulté le mars 28, 2026, [https://cloud.google.com/discover/what-are-ai-agents?hl=fr](https://cloud.google.com/discover/what-are-ai-agents?hl=fr)  
40. AI Agent Frameworks: Choosing the Right Foundation for Your Business | IBM, consulté le mars 28, 2026, [https://www.ibm.com/think/insights/top-ai-agent-frameworks](https://www.ibm.com/think/insights/top-ai-agent-frameworks)  
41. AI Agents vs. AI Tools: Understanding the Distinction and Future Implications \- Agile Lab, consulté le mars 28, 2026, [https://www.agilelab.it/blog/ai-agents-vs-ai-tools-distinction-and-future-implications](https://www.agilelab.it/blog/ai-agents-vs-ai-tools-distinction-and-future-implications)  
42. Formation en ligne IA génératives : fondamentaux pour les créateurs d'entreprise, consulté le mars 28, 2026, [https://www.bpifrance-universite.fr/formation/ia-generatives-fondamentaux-pour-les-createurs-dentreprise/](https://www.bpifrance-universite.fr/formation/ia-generatives-fondamentaux-pour-les-createurs-dentreprise/)  
43. Exploitez la puissance de la recherche sémantique avec MongoDB Atlas Vector Search, consulté le mars 28, 2026, [https://www.mongodb.com/fr-fr/resources/basics/semantic-search](https://www.mongodb.com/fr-fr/resources/basics/semantic-search)  
44. Best Online Generative AI Courses for 2025 (Plus Free Resources), consulté le mars 28, 2026, [https://aifwd.com/education/best-generative-ai-courses-online/](https://aifwd.com/education/best-generative-ai-courses-online/)

[image1]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABwAAAAXCAYAAAAYyi9XAAABLElEQVR4Xu2VsUoDURBFRxuRdGqX2koQSRMEsUllqWgaETvBBEXByjJ1qvyEBCsbCz9B8xFC0oTUgggS5zKzcXPZJy9LYhFy4LK8M28Ysrt5K7JgnihoXjRDzZtmabw8MXeaS5YJRbFBq75e9/XyaEccD5ovsV6kNl7+5UPTJtfRfJKbhD8Holgld+8+L8GB+2LFPfLn7tfIxxIceCNWLJE/cV8mH0twYEOsuE3+0P0p+VjQW2cJLsSKO+SP3VfIx4LeK5YgeYa75M/c4y+TB/ReswQrYsVZvKV4PzJBsUXu2X2aA80WuRDovWWZkPVrsD5KrXHUwfG+LDbE9jW5kAbH0rdfQ7fjSfPOMsWjZqDpabp+7Ysdd7l5ZTFrYm7p1MDnC8/n39hksYD5AaOhR00XcUjWAAAAAElFTkSuQmCC>

[image2]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABwAAAAXCAYAAAAYyi9XAAABTUlEQVR4Xu2VPUsDQRCGRy1EbILaWVsJGtKIIDZWWvmZRsROLFNbWtsoWNkKop0gFv4CUX+EhaUpBRs/5s3Oyty7h7kzSSN54CXsM7tzd5u9RKTPf2JUc6f50jxqBrLlwsxqmhL63Gsq2XJgUsKEERuP23jwZ0Yx9jUnbnwuoU/NuRZvmktyT5p3cu1Ac6Sda4k6uQPzZXiRdE1ywUUTC14qu+bHyJch3vSKlw2TvM9b5ufIF2VVwvpjLhxaYYb8mvlt8kU40lxpPjRLVJM9CY2r5DfNJwtKEE//jZfxO5z3Utkxj0WdkByaYRPdOKXYwjNy8YKZQwnhX1hwa96zrJkmF9mQnKdxbsjLvKfBeN2N8VOX19CDGnYsgoMIh5tPuJCwJfjEJLwuzLXmmaUD7+yn5VVCn9PMjD/wwKLX/LalXQd/XxMse8kUiz7MN5z2VP3GGOHBAAAAAElFTkSuQmCC>

[image3]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABwAAAAXCAYAAAAYyi9XAAABN0lEQVR4Xu2VvS5EQRiGPxoRndVpRKiIiEYIGpWS+M1GNKLRqJUuwR2oRFQahRsgfgqtyh2oJArC+2a+3cx5nc3Mkd1G9kmebOY5M7PZsztnzbr8JwbgDfyGD7CneDmLZ3gHD+Eu3IHbcMttMmzhjfp9XPNxb3NGHlzTyrdonr3DiziAR/ghLQU3XoQTcAyOuuwFGDalHXuvwpMGcAsn47BkYeOFOII974PSqzAPLzUeWdh4RvqG91npVSi9QycWLkxJX/Vel57LmfuLAwsbT0tf974sPReuHdFIGt/hnHSeI3YemarsW4vbSfqsfb/SBi+WWMuLp9KuvcesWDhjKbhO1xYo+zQcr0VjPuqSGzlZ887hl79yMo+LcgVfNZbA9Z8a/8q9hk6TvFXthH9fQxo7ybiGLsoPyjBLjOX8XhYAAAAASUVORK5CYII=>

[image4]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABwAAAAXCAYAAAAYyi9XAAABKklEQVR4Xu2VsWoCQRCGxzQidtEutZUQJI0Ego1VSkVtQrATTDAYsLK0tvIlRKxsLHwE40MI2oh1IAREZ5jJ4v2ccJ5oEfzg59hvdlju9m6P6Mp/pMWpozyCOGfC2XK+OBFvWelzfkknSd685cDckfbHbJyw8Y2b4cMpC35zBuBmnB9wHk5ZUHor4NrmDxJ2wRxp7xP4qvlb8I6wCzZJex/Al81nwTuk+I4yAB3S3nvwBfMv4B1SbKAMQI20NwO+ZD4P3iHFD5QB+NvDR/Cv5uWT8UWKsh/HEiXtDfWWfqI0njlplHtIbw/c2LwvSdJiFwukR5TUDjaT/93IuAiOhpw1Z8lZ2HVFetztM+LMwSFyTG7sGnZ7PExRnBt8ZGdFfjuyzxcjheIKsgPKdUdN4HTynAAAAABJRU5ErkJggg==>

[image5]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAoAAAAXCAYAAAAyet74AAAAp0lEQVR4XmNgGAXUBOpAPB2IBaB8YyDeAMSmcBVAwAjEl4DYCYj/A/FDIA6Cyv0G4gVQNsNqIGYCYl8GiEIlmAQQdEDFwKAGSp9AFoSCNVjEwAIgd6KLoSjkhgpIIomxQ8XykcQY2qGCyOAREH9DEwP7DqTwAwPE9I1A/ApFBRSAFM0CYmYgDgNiflRpCAAJghTKokugg0kMmO7DCmBBAMLmaHKDAQAA1WwkZEfq36MAAAAASUVORK5CYII=>

[image6]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAsAAAAXCAYAAADduLXGAAAAoElEQVR4XmNgGJSAEYhV0QWxgadA/B+KiQJXGEhQDFJ4DV0QFwApjkAXxAaiGDCd0ATE/mhiYHCTAaGYC4jvAzEfEH+Dq0ACIIW3gVgQiDdCxX5CxTEASHAnEM9El0AHMxgQJsyGslUQ0qgAPTJA7INQdj6SOBiAJKeh8VuQ2HDACRUQRRL7CMQbgLgHiA2RxMHAE10ACDyAmANdcBTAAACQdCSKrBERiwAAAABJRU5ErkJggg==>