<p align="center">
  <img src="https://img.shields.io/badge/version-2.0-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/langue-FR%20%7C%20EN-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/modèle-Claude%20Anthropic-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/licence-MIT-lightgrey?style=for-the-badge" />
  <img src="https://img.shields.io/badge/auteur-BrainJey-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/statut-actif-brightgreen?style=for-the-badge" />
</p>

<h1 align="center">🧠 Cerveau Universel / Universal Brain</h1>
<h3 align="center">Prompt de création d'un orchestrateur IA personnalisé<br/>Universal prompt to build your own personalized AI orchestration system</h3>

<p align="center">
  <a href="#-version-française">🇫🇷 Lire en Français</a> · 
  <a href="#-english-version">🇬🇧 Read in English</a> · 
  <a href="#-faq--foire-aux-questions">FAQ</a> · 
  <a href="#-changelog">Changelog</a>
</p>

---

## 🗂 Structure du dépôt / Repository Structure

```
cerveau-universel/
│
├── README.md                          ← Ce fichier / This file
├── LICENSE
├── CHANGELOG.md
├── CONTRIBUTING.md
│
├── prompts/
│   ├── FR/
│   │   └── cerveau-universel-FR.md    ← Prompt complet en français
│   └── EN/
│       └── universal-brain-EN.md      ← Full prompt in English
│
├── examples/
│   ├── cerveau-etudiant-master.md     ← Exemple : étudiant Master
│   ├── cerveau-freelance-marketing.md ← Exemple : freelance marketing
│   ├── cerveau-entrepreneur.md        ← Exemple : entrepreneur
│   └── brain-lawyer-EN.md             ← Example: lawyer (EN)
│
└── docs/
    ├── architecture.md                ← Détail des 7 composants
    ├── faq.md                         ← FAQ complète
    └── contributing.md                ← Guide de contribution
```

---

---

# 🇫🇷 VERSION FRANÇAISE

---

## 📌 Table des matières

- [Qu'est-ce qu'un Cerveau ?](#-quest-ce-quun-cerveau-)
- [Architecture du système](#-architecture-du-système)
- [Comment utiliser ce prompt](#-comment-utiliser-ce-prompt)
- [Le Prompt Universel FR](#-le-prompt-universel-fr)
- [Exemples par domaine](#-exemples-par-domaine-fr)
- [Exemple de sortie attendue](#-exemple-de-sortie-attendue-fr)
- [Règles fondamentales](#-règles-fondamentales)
- [FAQ](#-faq--foire-aux-questions)
- [Changelog](#-changelog)
- [Contribuer](#-contribuer)
- [Auteur & Inspiration](#-auteur--inspiration)
- [Licence](#-licence)

---

## 🤔 Qu'est-ce qu'un Cerveau ?

Un **Cerveau** est un système d'orchestration IA personnalisé qui tourne sur Claude (Anthropic).

Ce n'est **pas** un modèle IA distinct.  
C'est une **couche d'orchestration intelligente** qui :

- Active le bon assemblage de **skills** selon la nature de la tâche
- Mobilise les **agents** appropriés dans le bon ordre
- Applique les **règles absolues** de l'utilisateur à chaque réponse
- Respecte le **style de communication** propre à l'utilisateur
- Valide toujours le plan **avant** d'exécuter

```
Utilisateur → Cerveau → [Skills + Agents] → Livrable final
```

**Différence avec un simple prompt :**

| Prompt classique | Cerveau |
|---|---|
| Une seule instruction | Système complet avec mémoire de profil |
| Résultat générique | Résultat calibré sur TON domaine |
| Aucune validation | Plan validé avant chaque exécution |
| Style IA standard | Ton style de communication personnel |
| Capacité unique | 8 à 15 skills + 10 agents coordonnés |

---

## 🏗 Architecture du système

Tout Cerveau généré avec ce prompt contient **7 composants** :

| # | Composant | Description |
|---|---|---|
| 1 | **Identité** | Nom du Cerveau, profil utilisateur, périmètre d'activation |
| 2 | **Skills (8–15)** | Capacités par catégorie : production, intelligence, communication, automatisation |
| 3 | **Agents (10)** | Rôles spécialisés avec règles d'activation et position dans la séquence |
| 4 | **Matrice de décision** | Table SI/ALORS — quelle tâche → quels agents |
| 5 | **Workflow en 3 étapes** | Analyse → Exécution → Livraison |
| 6 | **Règles absolues** | Non-négociables pour toutes les réponses |
| 7 | **Style de communication** | Calibré sur tes écrits réels ou ta description |

---

## 🚀 Comment utiliser ce prompt

### Prérequis

- Un compte [Claude.ai](https://claude.ai) (gratuit ou Pro)
- 10 minutes pour répondre aux questions de profilage

### Étapes

```
1. Copie le prompt complet ci-dessous
2. Colle-le dans une nouvelle conversation Claude
3. Réponds aux 10 questions UNE PAR UNE
4. Valide le plan architectural proposé
5. Reçois ton Cerveau en format .md prêt à l'emploi
6. Sauvegarde le fichier .md → utilise-le comme contexte système dans tes conversations
```

### ✅ Conseils pour un meilleur résultat

> **Avant de lancer le prompt, prépare :**
> - Un exemple de texte que tu as écrit (email, rapport, message) → pour calibrer ton style
> - La liste de tes 3 tâches les plus répétitives → pour personnaliser les skills
> - Le nom que tu veux donner à ton Cerveau → ex : Cerveau Atlas, Cerveau Nova, Cerveau Léa...
> - Tes outils du quotidien → pour que les agents sachent quoi générer

> **À éviter :**
> - Répondre à plusieurs questions en une seule fois → réponds UNE par UNE
> - Être vague sur ton domaine → plus tu es précis, plus le Cerveau sera utile
> - Sauter la validation du plan → c'est l'étape la plus importante

---

## 📋 Le Prompt Universel FR

> **Copie tout le bloc ci-dessous et colle-le dans Claude.**

---

```
Tu es un architecte de systèmes d'orchestration IA personnalisés.

Ton rôle est de créer pour moi un Cerveau — un système d'orchestration 
intelligent qui va coordonner des skills et des agents pour traiter toutes 
mes tâches complexes.

Ce Cerveau doit être 100% adapté à MON profil. Pour le construire, 
commence par me poser les questions suivantes UNE PAR UNE. 
Ne passe pas à la suivante avant d'avoir ma réponse.

─────────────────────────────────────────
PHASE 1 — COLLECTE DE PROFIL (10 questions)
─────────────────────────────────────────

1. Quel est ton prénom, ton nom ou ton pseudonyme/marque personnelle ?

2. Quel est ton domaine professionnel ou académique principal ?
   (ex : marketing, droit, finance, logistique, ingénierie, médecine, 
   design, éducation, entrepreneuriat, RH, informatique...)

3. Quel est ton niveau actuel ?
   (ex : étudiant Licence/Master/Doctorat, professionnel junior, 
   freelance, entrepreneur, expert senior, en reconversion...)

4. Quels sont tes 3 types de tâches les plus fréquentes ?
   (ex : rédiger des rapports, analyser des données, gérer des clients, 
   créer des présentations, automatiser des process, faire de la veille...)

5. Quels outils utilises-tu régulièrement ?
   (ex : Excel, PowerPoint, Notion, n8n, Make, Google Suite, 
   Figma, Slack, CRM, ERP, Trello, Obsidian, Canva...)

6. Dans quelle langue travailles-tu principalement ?
   As-tu besoin de travailler en plusieurs langues ?

7. As-tu un style d'écriture particulier ou une charte de communication 
   à respecter ? 
   → Si oui, colle ici un exemple de texte que tu as rédigé toi-même.
   → Si non, décris en 3 adjectifs le ton que tu préfères.

8. Quels sont tes objectifs prioritaires pour les 6 prochains mois ?
   (ex : finir un mémoire, lancer un produit, trouver un emploi, 
   développer une clientèle, automatiser mon workflow, passer une certification...)

9. Y a-t-il des règles absolues que je dois toujours respecter ?
   (ex : ne jamais inventer de données, toujours citer les sources, 
   toujours valider avant d'agir, ne jamais dépasser X pages...)

10. Y a-t-il des sujets, formats ou approches que tu veux que j'évite 
    systématiquement dans mes réponses ?

─────────────────────────────────────────
PHASE 2 — CONSTRUCTION DU CERVEAU
─────────────────────────────────────────

Une fois que tu as répondu à toutes ces questions, construis mon Cerveau 
avec les 7 composants suivants :

COMPOSANT 1 — IDENTITÉ
→ Nom du Cerveau (dérivé de ma marque ou prénom)
→ Description de mon profil en 3 lignes
→ Périmètre d'activation : quand l'activer / quand ne pas l'activer
→ Phrase d'activation recommandée (ex : "Active le Cerveau [Nom]")

COMPOSANT 2 — MES SKILLS (entre 8 et 15)
→ Organisés en 4 catégories adaptées à mon domaine :
   - Skills de PRODUCTION (livrables fichiers : docx, pptx, xlsx, pdf...)
   - Skills de COMMUNICATION (rédaction, style, humanisation de textes)
   - Skills d'INTELLIGENCE (recherche, analyse, veille sectorielle)
   - Skills d'AUTOMATISATION (si applicable à mon profil)
→ Pour chaque skill : nom | description courte | phrase de déclenchement

COMPOSANT 3 — MES 10 AGENTS
→ Chaque agent a :
   - Un nom et un rôle précis adapté à mon domaine
   - Une règle d'activation (quand est-il mobilisé ?)
   - Une position dans la séquence (avant ou après quel agent ?)
→ Structure recommandée :
   Agent 1  : Chef de projet / Analyste Général → toujours actif
   Agents 2–8 : Spécialistes selon mon domaine
   Agent 9  : Vérificateur → toujours sur documents finaux
   Agent 10 : Formateur / Livreur → toujours en dernier si fichier attendu

COMPOSANT 4 — MATRICE DE DÉCISION
→ Tableau : SI la tâche contient X → ALORS activer les agents Y
→ Minimum 6 lignes couvrant mes cas d'usage fréquents

COMPOSANT 5 — WORKFLOW EN 3 ÉTAPES
→ Étape 1 — Analyse : afficher le plan d'exécution
  Format :
  ┌──────────────────────────────────────────┐
  │ [NOM DU CERVEAU] — ANALYSE DU PROJET     │
  │ Projet      : [titre court]              │
  │ Intention   : [objectif en 1 ligne]      │
  │ Complexité  : Simple / Medium / Complexe │
  │ Format      : [type de livrable]         │
  │ Durée est.  : [estimation temps]         │
  │ Skills act. : [liste]                    │
  │ Agents mob. : [liste ordonnée]           │
  │ Séquence    : Agent1 → Agent2 → ...      │
  │ Valide ce plan ?                         │
  └──────────────────────────────────────────┘
  → NE PAS CONTINUER sans confirmation de l'utilisateur.

→ Étape 2 — Exécution : passage des outputs entre agents, résultat final poli
→ Étape 3 — Livraison :
  ┌──────────────────────────────────────────┐
  │ [NOM DU CERVEAU] — LIVRABLE PRÊT         │
  │ Format  : [format du livrable]           │
  │ Sources : [N vérifiées / ⚠ ATTENTION]   │
  │ Style   : [style appliqué]               │
  └──────────────────────────────────────────┘

COMPOSANT 6 — RÈGLES ABSOLUES
→ Liste numérotée des règles non-négociables
→ Inclure obligatoirement :
   1. Règle anti-invention : jamais de données, chiffres ou sources inventés
   2. Règle de validation : toujours valider le plan avant d'exécuter
   3. Règle de style : toujours appliquer MON style sur les contenus rédigés
   4. Règle de transparence : si incertain, écrire ⚠ ATTENTION + explication

COMPOSANT 7 — MON STYLE DE COMMUNICATION
→ Calibré sur mon exemple de texte ou ma description
→ Inclure :
   - Structure de phrases (courtes/longues, types de constructions)
   - Connecteurs naturels que j'utilise
   - Registre (soutenu, professionnel, accessible...)
   - Ce que je n'écris jamais (mots à bannir, formules à éviter)

─────────────────────────────────────────
PHASE 3 — LIVRAISON EN 2 FORMATS
─────────────────────────────────────────

Livre mon Cerveau sous DEUX formats :

FORMAT A — Fichier SKILL.md complet
→ Prêt à être sauvegardé et utilisé directement comme contexte dans Claude
→ Inclure le frontmatter YAML (name, version, description)
→ Sections claires avec titres Markdown H2/H3

FORMAT B — Fiche de référence rapide (1 page)
→ Tableau récapitulatif skills + agents en 2 colonnes
→ Phrase d'activation
→ Top 5 cas d'usage immédiats avec exemple de formulation

─────────────────────────────────────────
RÈGLE FONDAMENTALE DU CERVEAU
─────────────────────────────────────────

Ne construis rien avant d'avoir toutes mes réponses.
Ne devine pas, n'invente pas, ne suppose pas.
Chaque choix architectural doit être justifié en une ligne.
Si une réponse est ambiguë, pose une question de clarification AVANT de continuer.
Si l'utilisateur saute une question, demande-la quand même avant de passer à la suite.

Prêt ? Commence par la question 1.
```

---

## 🎯 Exemples par domaine FR

Voici comment le Cerveau s'adapte selon ton profil :

### 🎓 Étudiant Master (ex : Achats & Logistique)
```
Skills générés : Plan mémoire | Style académique | Détection IA | 
                 Humaniseur | Sources validator | PPTX soutenance | 
                 Excel KPI | Veille sectorielle | GTD étudiant

Agents clés    : Chercheur académique | Structureur mémoire | 
                 Rédacteur académique | Critique argumentation | 
                 Vérificateur sources
```

### 💼 Freelance Marketing / Communication
```
Skills générés : Brief créatif | Copywriting | Veille tendances | 
                 Calendrier éditorial | Reporting client | 
                 Email séquences | Social media | Brand voice

Agents clés    : Stratège contenu | Copywriter | Designer brief | 
                 Analyste performance | Vérificateur brief client
```

### 🏢 Manager / Chef de projet
```
Skills générés : Compte-rendu réunion | Reporting direction | 
                 Plan projet | Note de cadrage | Email escalation | 
                 Dashboard KPI | Préparation comité

Agents clés    : Analyste projet | Rédacteur exécutif | 
                 Gestionnaire risques | Formateur livrables
```

### ⚖️ Juriste / Avocat
```
Skills générés : Analyse contrats | Veille juridique | Note de droit | 
                 Courrier juridique | Synthèse jurisprudence | 
                 Checklist conformité

Agents clés    : Chercheur jurisprudence | Analyste contrat | 
                 Rédacteur juridique | Vérificateur références légales
```

---

## 📦 Exemple de sortie attendue FR

Après avoir répondu aux 10 questions, Claude génère :

```
📄 SKILL.md — Fichier complet de ton Cerveau
   ├── Frontmatter YAML (name, version, description)
   ├── Identité + périmètre d'activation
   ├── 8–15 Skills catégorisés avec triggers
   ├── 10 Agents avec rôles + règles d'activation
   ├── Matrice de décision (tableau SI/ALORS)
   ├── Workflow 3 étapes avec formats d'affichage
   ├── Règles absolues numérotées
   └── Style de communication calibré

📋 FICHE RAPIDE — Résumé 1 page
   ├── Phrase d'activation
   ├── Tableau Skills / Agents en 2 colonnes
   └── Top 5 cas d'usage avec exemples de formulation
```

---

---

# 🇬🇧 ENGLISH VERSION

---

## 📌 Table of Contents

- [What is a Brain?](#-what-is-a-brain)
- [System Architecture](#-system-architecture)
- [How to Use This Prompt](#-how-to-use-this-prompt)
- [The Universal Prompt EN](#-the-universal-prompt-en)
- [Examples by Domain](#-examples-by-domain-en)
- [Expected Output Example](#-expected-output-example-en)
- [Core Principles](#-core-principles)

---

## 🤔 What is a Brain?

A **Brain** is a personalized AI orchestration system running on Claude (Anthropic).

It is **not** a separate AI model.  
It is an **intelligent orchestration layer** that:

- Activates the right **skills** depending on the task type
- Mobilizes the appropriate **agents** in the correct order
- Applies the user's **absolute rules** to every response
- Respects the user's **personal communication style**
- Always validates the plan **before** executing

```
User → Brain → [Skills + Agents] → Final Deliverable
```

**Difference from a regular prompt:**

| Classic Prompt | Brain |
|---|---|
| Single instruction | Complete system with profile memory |
| Generic output | Output calibrated to YOUR domain |
| No validation | Plan validated before every execution |
| Standard AI style | Your personal communication style |
| Single capability | 8 to 15 skills + 10 coordinated agents |

---

## 🏗 System Architecture

Every Brain generated with this prompt contains **7 components**:

| # | Component | Description |
|---|---|---|
| 1 | **Identity** | Brain name, user profile, activation scope |
| 2 | **Skills (8–15)** | Capabilities by category: production, intelligence, communication, automation |
| 3 | **Agents (10)** | Specialized roles with activation rules and sequence position |
| 4 | **Decision Matrix** | IF/THEN table — which task → which agents |
| 5 | **3-Step Workflow** | Analysis → Execution → Delivery |
| 6 | **Absolute Rules** | Non-negotiable for all responses |
| 7 | **Communication Style** | Calibrated from your real writing or your description |

---

## 🚀 How to Use This Prompt

### Requirements

- A [Claude.ai](https://claude.ai) account (free or Pro)
- 10 minutes to answer the profiling questions

### Steps

```
1. Copy the full prompt below
2. Paste it into a new Claude conversation
3. Answer the 10 profiling questions ONE BY ONE
4. Validate the proposed architectural plan
5. Receive your Brain as a ready-to-use .md file
6. Save the .md file → use it as system context in your conversations
```

### ✅ Tips for Better Results

> **Before launching the prompt, prepare:**
> - A sample text you have written yourself (email, report, message) → to calibrate your style
> - Your top 3 most repetitive tasks → to personalize the skills
> - The name you want to give your Brain → e.g. Brain Atlas, Brain Nova, Brain Leo...
> - Your everyday tools → so agents know what to generate

> **What to avoid:**
> - Answering multiple questions at once → answer ONE at a time
> - Being vague about your domain → the more precise you are, the more useful your Brain
> - Skipping the plan validation → it is the most important step

---

## 📋 The Universal Prompt EN

> **Copy the entire block below and paste it into Claude.**

---

```
You are an architect of personalized AI orchestration systems.

Your role is to create my Brain — an intelligent orchestration system 
that will coordinate skills and agents to handle all my complex tasks.

This Brain must be 100% tailored to MY profile. To build it, 
ask me the following questions ONE BY ONE. 
Do not move to the next question until you have my answer.

─────────────────────────────────────────
PHASE 1 — PROFILE COLLECTION (10 questions)
─────────────────────────────────────────

1. What is your first name, last name, or personal brand/pseudonym?

2. What is your main professional or academic domain?
   (e.g. marketing, law, finance, logistics, engineering, medicine, 
   design, education, entrepreneurship, HR, IT...)

3. What is your current level?
   (e.g. Bachelor/Master/PhD student, junior professional, 
   freelancer, entrepreneur, senior expert, career changer...)

4. What are your 3 most frequent task types?
   (e.g. writing reports, analyzing data, managing clients, 
   creating presentations, automating processes, industry monitoring...)

5. Which tools do you use regularly?
   (e.g. Excel, PowerPoint, Notion, n8n, Make, Google Suite, 
   Figma, Slack, CRM, ERP, Trello, Obsidian, Canva...)

6. What is your main working language?
   Do you need to work in multiple languages?

7. Do you have a particular writing style or communication guidelines 
   to follow?
   → If yes, paste here an example of a text you have written yourself.
   → If no, describe your preferred tone in 3 adjectives.

8. What are your top priorities for the next 6 months?
   (e.g. complete a thesis, launch a product, find a job, 
   grow a client base, automate your workflow, pass a certification...)

9. Are there any absolute rules I must always follow?
   (e.g. never invent data, always cite sources, 
   always validate before acting, never exceed X pages...)

10. Are there any topics, formats, or approaches you want me to 
    systematically avoid in my responses?

─────────────────────────────────────────
PHASE 2 — BRAIN CONSTRUCTION
─────────────────────────────────────────

Once you have answered all these questions, build my Brain 
using the following 7 components:

COMPONENT 1 — IDENTITY
→ Brain name (derived from my brand or first name)
→ My profile description in 3 lines
→ Activation scope: when to activate / when not to activate
→ Recommended activation phrase (e.g. "Activate Brain [Name]")

COMPONENT 2 — MY SKILLS (between 8 and 15)
→ Organized into 4 categories adapted to my domain:
   - PRODUCTION skills (file deliverables: docx, pptx, xlsx, pdf...)
   - COMMUNICATION skills (writing, style, text humanization)
   - INTELLIGENCE skills (research, analysis, sector monitoring)
   - AUTOMATION skills (if applicable to my profile)
→ For each skill: name | short description | trigger phrase

COMPONENT 3 — MY 10 AGENTS
→ Each agent has:
   - A precise name and role adapted to my domain
   - An activation rule (when is it mobilized?)
   - A position in the sequence (before or after which agent?)
→ Recommended structure:
   Agent 1   : Project Manager / General Analyst → always active
   Agents 2–8: Specialists according to my domain
   Agent 9   : Verifier → always on final documents
   Agent 10  : Formatter / Deliverer → always last if file expected

COMPONENT 4 — DECISION MATRIX
→ Table: IF task contains X → THEN activate agents Y
→ Minimum 6 rows covering my frequent use cases

COMPONENT 5 — 3-STEP WORKFLOW
→ Step 1 — Analysis: display the execution plan
  Format:
  ┌──────────────────────────────────────────┐
  │ [BRAIN NAME] — PROJECT ANALYSIS          │
  │ Project     : [short title]              │
  │ Intent      : [goal in 1 line]           │
  │ Complexity  : Simple / Medium / Complex  │
  │ Format      : [deliverable type]         │
  │ Est. time   : [time estimate]            │
  │ Skills      : [list]                     │
  │ Agents      : [ordered list]             │
  │ Sequence    : Agent1 → Agent2 → ...      │
  │ Validate this plan?                      │
  └──────────────────────────────────────────┘
  → DO NOT CONTINUE without user confirmation.

→ Step 2 — Execution: agents pass outputs in sequence, final result polished
→ Step 3 — Delivery:
  ┌──────────────────────────────────────────┐
  │ [BRAIN NAME] — DELIVERABLE READY         │
  │ Format  : [deliverable format]           │
  │ Sources : [N verified / ⚠ ATTENTION]    │
  │ Style   : [style applied]                │
  └──────────────────────────────────────────┘

COMPONENT 6 — ABSOLUTE RULES
→ Numbered list of non-negotiable rules
→ Must include:
   1. No-invention rule: never invent data, figures, or sources
   2. Validation rule: always validate the plan before executing
   3. Style rule: always apply MY style to all written content
   4. Transparency rule: if uncertain, write ⚠ ATTENTION + explanation

COMPONENT 7 — MY COMMUNICATION STYLE
→ Calibrated from my text sample or my description
→ Include:
   - Sentence structure (short/long, construction types)
   - Natural connectors I use
   - Register (formal, professional, accessible...)
   - What I never write (words to ban, formulas to avoid)

─────────────────────────────────────────
PHASE 3 — DELIVERY IN 2 FORMATS
─────────────────────────────────────────

Deliver my Brain in TWO formats:

FORMAT A — Complete SKILL.md file
→ Ready to save and use directly as context in Claude
→ Include YAML frontmatter (name, version, description)
→ Clear sections with Markdown H2/H3 headings

FORMAT B — Quick reference sheet (1 page)
→ 2-column summary table of skills + agents
→ Activation phrase
→ Top 5 immediate use cases with example phrasings

─────────────────────────────────────────
FUNDAMENTAL RULE OF THE BRAIN
─────────────────────────────────────────

Build nothing before you have all my answers.
Do not guess, do not invent, do not assume.
Every architectural choice must be justified in one line.
If an answer is ambiguous, ask a clarification question BEFORE continuing.
If the user skips a question, ask it again before moving on.

Ready? Start with question 1.
```

---

## 🎯 Examples by Domain EN

Here is how the Brain adapts to different profiles:

### 🎓 Master's Student (e.g. Procurement & Logistics)
```
Generated skills : Thesis plan | Academic style | AI detection | 
                   Humanizer | Sources validator | Defense PPTX | 
                   Excel KPI | Sector monitoring | Student GTD

Key agents       : Academic researcher | Thesis structurer | 
                   Academic writer | Argument critic | 
                   Sources verifier
```

### 💼 Freelance Marketing / Copywriter
```
Generated skills : Creative brief | Copywriting | Trend monitoring | 
                   Editorial calendar | Client reporting | 
                   Email sequences | Social media | Brand voice

Key agents       : Content strategist | Copywriter | Design brief | 
                   Performance analyst | Client brief verifier
```

### 🏢 Manager / Project Lead
```
Generated skills : Meeting notes | Executive reporting | 
                   Project plan | Scoping note | Escalation email | 
                   KPI dashboard | Committee preparation

Key agents       : Project analyst | Executive writer | 
                   Risk manager | Deliverable formatter
```

### ⚖️ Lawyer / Legal Professional
```
Generated skills : Contract analysis | Legal monitoring | Legal memo | 
                   Legal correspondence | Case law synthesis | 
                   Compliance checklist

Key agents       : Case law researcher | Contract analyst | 
                   Legal writer | Legal reference verifier
```

---

## 📦 Expected Output Example EN

After answering the 10 questions, Claude generates:

```
📄 SKILL.md — Your complete Brain file
   ├── YAML frontmatter (name, version, description)
   ├── Identity + activation scope
   ├── 8–15 Skills categorized with triggers
   ├── 10 Agents with roles + activation rules
   ├── Decision matrix (IF/THEN table)
   ├── 3-step workflow with display formats
   ├── Numbered absolute rules
   └── Calibrated communication style

📋 QUICK REFERENCE — 1-page summary
   ├── Activation phrase
   ├── Skills / Agents 2-column table
   └── Top 5 use cases with example phrasings
```

---

---

## ⚙️ Règles fondamentales / Core Principles

Tout Cerveau / Every Brain generated with this prompt follows these principles:

| Règle / Rule | FR Description | EN Description |
|---|---|---|
| 🚫 Zéro invention | Jamais de données inventées | Never invent data, figures, or sources |
| ✅ Validation | Plan validé avant exécution | Plan validated before any execution |
| 🎨 Style perso | Ton style sur tous les contenus | Your style applied to all written content |
| 🔍 Chercheur en 1er | Sources vérifiées avant rédaction | Sources verified before writing |
| 📁 Formateur en dernier | Fichier généré en dernière étape | File generated as the last step |
| 💬 Proactivité | Orientation vers le bon skill | Direct routing to the right skill |
| ⚠ Transparence | ATTENTION si incertain | ATTENTION flag if uncertain |

---

## ❓ FAQ — Foire aux questions

### 🇫🇷 Français

**Q : Est-ce que ce prompt fonctionne sur la version gratuite de Claude ?**  
R : Oui. Le prompt fonctionne sur Claude.ai gratuit. La version Pro donne accès à des conversations plus longues, ce qui est utile pour les Cerveaux complexes.

**Q : Combien de temps faut-il pour créer son Cerveau ?**  
R : Entre 10 et 20 minutes selon la précision de tes réponses. Plus tu es détaillé, meilleur sera le résultat.

**Q : Est-ce que le Cerveau mémorise mes informations entre les conversations ?**  
R : Non. Claude ne mémorise pas entre les sessions. Tu dois copier-coller le fichier SKILL.md en début de conversation pour que le Cerveau soit actif.

**Q : Puis-je modifier mon Cerveau après l'avoir créé ?**  
R : Oui. Le fichier SKILL.md est entièrement modifiable. Tu peux ajouter des skills, ajuster les règles, ou raffiner ton style à tout moment.

**Q : Ce système fonctionne-t-il avec d'autres IA que Claude ?**  
R : Le prompt est conçu pour Claude (Anthropic). Il peut partiellement fonctionner avec GPT-4 ou Gemini, mais les résultats seront moins précis car l'architecture est optimisée pour Claude.

**Q : Est-ce que je peux partager mon Cerveau avec d'autres personnes ?**  
R : Oui, si tu retires les informations personnelles (nom, entreprise, données privées). Le fichier SKILL.md est facilement anonymisable.

**Q : Puis-je créer plusieurs Cerveaux pour différents contextes ?**  
R : Absolument. Tu peux créer un Cerveau Pro (travail), un Cerveau Académique (études), un Cerveau Perso (projets créatifs). Chacun a son fichier SKILL.md dédié.

---

### 🇬🇧 English

**Q: Does this prompt work on the free version of Claude?**  
A: Yes. The prompt works on free Claude.ai. The Pro version gives access to longer conversations, which is useful for complex Brains.

**Q: How long does it take to create my Brain?**  
A: Between 10 and 20 minutes depending on how detailed your answers are. The more precise you are, the better the result.

**Q: Does the Brain remember my information between conversations?**  
A: No. Claude does not remember between sessions. You need to paste the SKILL.md file at the start of a conversation to activate the Brain.

**Q: Can I modify my Brain after creating it?**  
A: Yes. The SKILL.md file is fully editable. You can add skills, adjust rules, or refine your style at any time.

**Q: Does this system work with other AIs besides Claude?**  
A: The prompt is designed for Claude (Anthropic). It may partially work with GPT-4 or Gemini, but results will be less precise as the architecture is optimized for Claude.

**Q: Can I share my Brain with others?**  
A: Yes, as long as you remove personal information (name, company, private data). The SKILL.md file is easy to anonymize.

**Q: Can I create multiple Brains for different contexts?**  
A: Absolutely. You can create a Work Brain, an Academic Brain, a Personal Brain (creative projects). Each has its own dedicated SKILL.md file.

---

## 📋 Changelog

### v2.0 — 2026-06-05
- ✅ Version bilingue FR/EN complète
- ✅ Structure de repo recommandée ajoutée
- ✅ Exemples par domaine (4 profils FR + 4 profils EN)
- ✅ FAQ complète FR/EN (7 questions chacune)
- ✅ Tableau comparatif Prompt classique vs Cerveau
- ✅ Section Contributing ajoutée
- ✅ Badges visuels enrichis
- ✅ Règles fondamentales bilingues en tableau
- ✅ Conseils pratiques et erreurs à éviter

### v1.0 — 2026-05-01
- 🚀 Version initiale — Prompt universel FR
- Architecture 7 composants
- Workflow 3 étapes
- Matrice de décision
- Inspiré du Cerveau BrainJey v1.0

---

## 🤝 Contribuer / Contributing

### 🇫🇷 Comment contribuer

Ce projet est ouvert aux contributions. Tu peux :

1. **Ajouter un exemple de Cerveau** pour un domaine non couvert
   → Crée un fichier dans `examples/` en suivant le format existant

2. **Améliorer le prompt** en proposant une modification via Pull Request
   → Décris clairement le problème que tu résous et le résultat attendu

3. **Signaler un bug ou une incohérence** via les Issues GitHub
   → Inclure le domaine testé, la version de Claude, et le comportement observé

4. **Traduire** le prompt dans une autre langue
   → Crée un dossier `prompts/[CODE_LANGUE]/` et soumets une PR

**Règle de contribution :**
> Tout ajout doit respecter le principe fondamental : **ne jamais inventer, toujours vérifier**.  
> Les exemples de Cerveaux doivent être testés sur Claude avant soumission.

### 🇬🇧 How to Contribute

This project is open to contributions. You can:

1. **Add a Brain example** for an uncovered domain
   → Create a file in `examples/` following the existing format

2. **Improve the prompt** by proposing a change via Pull Request
   → Clearly describe the problem you solve and the expected result

3. **Report a bug or inconsistency** via GitHub Issues
   → Include the tested domain, Claude version, and observed behavior

4. **Translate** the prompt into another language
   → Create a `prompts/[LANGUAGE_CODE]/` folder and submit a PR

**Contribution Rule:**
> Every addition must respect the core principle: **never invent, always verify**.  
> Brain examples must be tested on Claude before submission.

---

## 👤 Auteur & Inspiration / Author & Inspiration

Ce prompt universel est inspiré du **Cerveau BrainJey** — système d'orchestration IA personnel développé par :

This universal prompt is inspired by **Cerveau BrainJey** — a personal AI orchestration system developed by:

**Jérémie WABA** — alias **BrainJey**  
Master Achats & Approvisionnement — Ascencia Business School, Île-de-France  
Junior Buyer | n8n Automation | P2P Digitalisation

> 🇫🇷 *"Un Cerveau, c'est pas un outil générique. C'est une extension de ta façon de travailler."*

> 🇬🇧 *"A Brain is not a generic tool. It is an extension of the way you work."*

> — BrainJey

---

## 📄 Licence / License

Ce projet est sous licence **MIT**.  
This project is licensed under **MIT**.

Tu peux librement utiliser, modifier et redistribuer ce prompt, à condition de mentionner l'auteur original.  
You may freely use, modify, and redistribute this prompt, provided you credit the original author.

```
MIT License — Copyright (c) 2026 Jérémie WABA (BrainJey)
```

---

<p align="center">
  <i>Généré avec Claude (Anthropic) — Architecture BrainJey v2.0</i><br/>
  <i>Generated with Claude (Anthropic) — BrainJey Architecture v2.0</i>
</p>
