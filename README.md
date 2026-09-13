# 🚀 Bellon Nakad - Étudiant en cycle ingénieur spécialisation IA/ML

Bienvenue sur mon GitHub ! Je suis un étudiant passionné par le **Machine Learning, le MLOps et l'IA Générative**. J'aime transformer des données complexes en solutions innovantes avec un impact concret.

## 🛠️ Tech Stack

### **Data Science & ML**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)

### **MLOps & DevOps**
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

### **LLM & NLP**
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG_Architecture-00A98F?style=for-the-badge)

## 🌟 Projets Récents

### 🛡️ [AI Pentest — AI Engineering for Cybersecurity](https://github.com/NakadBellon/ai-pentest)

#### 🎯 Projet d’AI Engineering appliqué à la cybersécurité

**Plateforme d’analyse automatisée de résultats de sécurité combinant ingestion de données, corrélation de findings, embeddings locaux et agents IA pour assister le triage de vulnérabilités dans un cadre de test autorisé.**

Le projet a été conçu comme une démarche **end-to-end d’AI Engineering**, depuis la structuration et la normalisation des données de sécurité jusqu’à l’intégration d’un **agent LLM local orchestré avec LangGraph**.

#### 🚀 Highlights Techniques

##### 🔍 Pipeline de Sécurité

* **Nmap XML** : ingestion et parsing de résultats de scans
* **Pydantic** : modèles de données typés et validation
* **Normalization** : transformation des résultats bruts en objets de sécurité structurés
* **Correlation Engine** : détection de similarités entre findings
* **Evaluation Framework** : mesure de la qualité de la corrélation avec un golden dataset

##### 🧠 AI & Machine Learning

* **TF-IDF** : première approche de similarité textuelle déterministe
* **Embeddings locaux** avec `nomic-embed-text`
* **Ollama** : exécution locale de modèles open-source
* **Qwen3 4B** : LLM local utilisé pour l'analyse des findings
* **LangChain** : intégration du LLM et structured outputs
* **Pydantic** : validation des réponses structurées générées par le LLM

##### 🤖 Agentic AI

* **Tool Calling** : capacité du LLM à sélectionner des outils selon le contexte
* **LangGraph** : orchestration du workflow agentique
* **ToolNode** : exécution contrôlée des outils
* **StateGraph** : gestion de l'état et de l'historique des messages
* **Security Knowledge Base** : contexte local sur les services et technologies
* **Evidence-based analysis** : l'agent doit s'appuyer sur les informations disponibles avant de produire son analyse

#### 🏗️ Architecture

```text
Security Tools
      ↓
   Ingestion
      ↓
 Normalization
      ↓
  Correlation
      ↓
Finding + Evidence
      ↓
 LangGraph Agent
      ↓
      LLM
   ┌──┼────────────────────┐
   ↓  ↓                    ↓
Context  Evidence   Security Knowledge
   └──┼────────────────────┘
      ↓
  AI Analysis
```

#### 🧪 Qualité & Tests

* **183 tests automatisés**
* Tests unitaires et d'intégration
* Golden dataset pour l'évaluation de la corrélation
* Tests d'intégration avec **Ollama**
* Validation des modèles et des sorties structurées
* Tests du routing et du cycle d'exécution LangGraph

##### 📊 Résultats de corrélation

* **Accuracy : 95.0%**
* **Precision : 100%**
* **Recall : 91.7%**
* **F1-score : 95.7%**

#### 🧩 Architecture Logicielle

| Domaine                  | Technologies              | Réalisation                      |
| ------------------------ | ------------------------- | -------------------------------- |
| **Security Data**        | Nmap, XML, Pydantic       | Ingestion et normalisation       |
| **Machine Learning**     | Scikit-learn, TF-IDF      | Similarité et corrélation        |
| **Embeddings**           | Ollama, nomic-embed-text  | Représentation sémantique locale |
| **LLM**                  | Qwen3, Ollama             | Analyse locale des findings      |
| **AI Engineering**       | LangChain, LangGraph      | Chains, tools et agent           |
| **Software Engineering** | Python, pytest, Git       | Architecture modulaire et tests  |
| **Security**             | Pentest, triage, evidence | Analyse dans un cadre autorisé   |

#### 🔐 Approche Security-by-Design

Le projet privilégie une approche **read-only et evidence-based** :

* Les outils IA analysent les données fournies par les outils de sécurité.
* Aucune exploitation automatique de vulnérabilités n'est implémentée.
* L'agent distingue les **faits observés** des **hypothèses**.
* Les informations non présentes dans les données doivent être signalées comme insuffisamment documentées.
* Le projet est destiné à des **tests de sécurité autorisés et à un usage éducatif**.

#### 💡 Objectif du Projet

Ce projet me permet d'explorer concrètement la conception de systèmes **AI Engineering** appliqués à la cybersécurité, en travaillant progressivement sur :

* la conception d'architectures Python modulaires ;
* l'ingestion et la structuration de données de sécurité ;
* les méthodes de similarité et de corrélation ;
* les embeddings et les LLM locaux ;
* le **tool calling** et les agents IA ;
* l'orchestration avec **LangGraph** ;
* les tests unitaires et d'intégration ;
* la conception de systèmes IA fiables et contrôlables.

**Stack :** Python • Pydantic • Scikit-learn • Ollama • Qwen3 • LangChain • LangGraph • pytest • Nmap • Git

*Building AI Engineering systems for cybersecurity — one layer at a time. 🛡️🤖*


### ⚽ [Premier League Predictor - MLOps Pipeline](https://github.com/NakadBellon/machine-learning-premier-league-predictor)

#### 🎯 Projet Démonstrateur MLOps

**Système de prédiction footballistique allant du scraping de données au déploiement cloud, démontrant une maîtrise complète des pratiques MLOps modernes.**


#### 🚀 Highlights Techniques

##### 📊 Machine Learning Performant
- **Accuracy : 60.58%** (+17% vs baseline) sur la prédiction de matchs
- **Régression logistique optimisée** avec validation temporelle
- **Simulation Monte Carlo** de 10,000 saisons pour les probabilités de classement

##### 🔧 Stack MLOps Complète
- **MLflow** : Tracking d'expériences et versioning de modèles
- **DVC** : Versioning des données avec Google Drive
- **Docker** : Containerisation de l'application
- **Streamlit** : Interface utilisateur interactive
- **FastAPI** : API RESTful pour usage programmatique

##### 📈 Données et Features
- **15,960 matchs** historiques (2019-2026) scrapés depuis FBref
- **Features avancées** : xG, forme des équipes, statistiques temporelles
- **Pipeline de données** automatisé et reproductible


#### 🏗️ Architecture & Déploiement

```
Data Scraping → Feature Engineering → Model Training → MLflow Tracking → Docker Container → Hugging Face Deployment
```

##### 🌐 Déploiement Cloud
- **Hugging Face Spaces** : Application Streamlit containerisée
- **API FastAPI** : Endpoints REST pour intégrations
- **CI/CD** : GitHub Actions pour déploiement automatique


#### 🎖️ Compétences Démontrées

| Domaine | Technologies | Réalisation |
|---------|--------------|-------------|
| **Machine Learning** | Scikit-learn, XGBoost, LightGBM | Modèle à 60.58% accuracy |
| **MLOps** | MLflow, DVC, Docker | Pipeline reproductible |
| **Data Engineering** | Pandas, SoccerData, FBref | Pipeline données scalable |
| **Déploiement** | Streamlit, FastAPI, Hugging Face | Application full-stack |
| **DevOps** | Docker, GitHub Actions, CI/CD | Infrastructure as Code |


#### 📈 Résultats Concrets

##### 🏆 Prédictions Saison 2025-2026
- **Manchester City** : 76.4% chances de titre
- **Top 4** identifié avec >97% de précision
- **Risques relégation** quantifiés par simulation

##### ⚡ Performance Réelle
- **15K+ matchs** analysés en temps réel
- **Prédictions match** en <2 secondes
- **Simulations saison** en <10 minutes


#### 💡 Valeur Ajoutée

Ce projet démontre ma capacité à **concevoir, développer et déployer** des solutions ML de bout en bout, avec une attention particulière sur :
- La **reproductibilité** des expériences
- La **scalabilité** de l'infrastructure  
- La **maintenabilité** du code
- L'**impact business** des prédictions

**Stack :** Python • MLflow • Docker • Streamlit • FastAPI • Hugging Face • Scikit-learn

*Prêt à relever de nouveaux défis techniques et business !* 🚀

## 🎓 Formation

### 🏫 École d’Ingénieur EFREI Paris
**Cycle Ingénieur – Big Data & Machine Learning**  
📅 2026 – 2028  

- Machine Learning avancé
- Deep Learning & IA générative
- Data Engineering & Big Data
- MLOps et systèmes ML en production
- Architecture logicielle et APIs

### 🎓 Master 2 Statistiques & Data Science – Université Paris-Est Créteil
📅 2023 – 2025  

- Modélisation statistique et économétrie
- Machine Learning supervisé et non supervisé
- Analyse de données à grande échelle
- Optimisation et inférence statistique

### 🎓 Licence Économie – Parcours Monnaie & Finance - Université Paris 2 Panthéon-Assas
📅 2020 – 2023  

- Mathématiques et Statistiques
- Finance de marché et d’entreprises
- Macro et Microéconomie 
- Économétrie


## 📊 Certifications

| Badge | Certification | Organisme |
|-------|---------------|-----------|
| 🔧 | MLOps Practitioner | Dataiku |
| 🎨 | ML Practitioner | Dataiku |
| ⚡ | Advanced Designer | Dataiku |

## 💼 Expérience

**Chargé d'études statistiques** @Covéa GMF - Alternance

- Développement modèle prédictif (3.5M+ sociétaires)
- Segmentation réseau d'agences via clustering
- Automatisation processus de reporting

## 📫 Contact

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:nakadbellon@gmail.com)

## 📈 GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=NakadBellon&show_icons=true&theme=radical)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=NakadBellon&layout=compact&theme=radical)

---

> *"Data Scientist passionné par la création de solutions IA qui ont un impact réel"*

⭐ **N'hésitez pas à explorer mes repos et à me contacter pour collaborer !**
