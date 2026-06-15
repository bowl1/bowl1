# 👋 Hi, I’m Bowen Li

🧬 Carbon-based creature shipping bugs

📍 Copenhagen, Denmark  

📫 **Contact**  
Email: bowenivy0@gmail.com


## 🧩 Projects

### Full-stack & AI:

#### 👻 My Little Ghost — Anonymous Social Platform  
🔗 https://github.com/bowl1/social-chat-app  
🌐 https://social-chat-dk.vercel.app  
Figma: https://github.com/bowl1/Figma-Portfolio  (user case interview, UI design and mini component library)

- React **anonymous social sharing platform** , developing from user interview -> product requirement-> logo design -> UI design-> usability testing -> code implementing. 
- Supports text and media posts with **per-group aliases**, preserving user privacy.
- Implemented authentication, media uploads, and scalable feed interactions.

**Tech:** React, Tanstack Query, Zustand, TypeScript, Next.js, PostgreSQL, Prisma, Firebase Auth, Vercel, Figma, HTML,CSS, Styled component

---

#### ✍️ HeyWrite — AI Smart Writing Assistant

🔗 https://github.com/bowl1/Hey_write  
🌐 https://hey-write.vercel.app

An AI-powered smart writing assistant that turns a one-sentence intent into professional content, with control over tone, language, and generation mode.

**Features**
- Built two generation modes: **template-based generation** and **wild/freeform generation**
- Implemented **hybrid template retrieval** with pgvector semantic search, BM25 keyword search, weighted reranking, and match-score gating
- Built a **LangGraph-controlled agent loop** for planning, tool use, drafting, revision, evaluation, retry, and state persistence
- Supports multi-turn conversation memory, session recovery, previous-result revisiting, and incremental draft modification
- Added revision summaries that highlight changes between the previous and newly generated content
- Supports tone/style control including Formal, Casual, Polite Push, Concise & Direct, Humorous, and Creative
- Supports English, Chinese, and Danish, with one-click copy for generated content
- Added evaluator guardrails combining deterministic checks and optional LLM-as-judge feedback before persisting final output
- Deployment with Docker, GitHub Actions, Vercel, and Render

**Tech:** React, TypeScript, Python, FastAPI, LangGraph, LangChain, DeepSeek Chat API, OpenAI Embeddings (text-embedding-3-small), RAG, PostgreSQL, pgvector, BM25, Docker, GitHub Actions, Vercel, Render

---

#### Ask My Docs — PDF-based RAG Chatbot  
🔗 https://github.com/bowl1/AskMyDocs-AI-app  
🌐 https://askmydocument.vercel.app  

- Built a **document-grounded AI assistant** that answers questions strictly from user-uploaded PDFs.
- Always provides **page-level citations** and refuses to hallucinate.
- Deployed backend and frontend separately with automated CI/CD pipelines.

**Tech:** Python, LangChain, TypeScript, FastAPI, React, RAG, ChromaDB, Tailwind CSS, Docker, GitHub Actions, LLMs, Vercel, AWS, HuggingFace，OpenAI-compatible LLM APIs (DeepSeek)

---
---

### ML & Data Engineering:

#### Behaviour-Aware Federated Wind Power Forecasting  
**Master’s Thesis Project**  
🔗 Strategy design and model training (Python, FL, LSTM): https://github.com/bowl1/Wind-and-AI

🔗 Published findings as a research paper: "A Behaviour-Aware Federated Forecasting Framework for Distributed Stand-Alone Wind Turbines" 
  https://arxiv.org/abs/2603.05263


🔗 Interface application: https://github.com/bowl1/Behaviour-Aware-Federated-Wind-Power-Forecasting-System-demo

- Built a **distributed wind power forecasting system** across **400+ independent wind turbines**.
- Data preprocessing and feature engineering 
- Designed a **behaviour-aware auto-split clustering strategy** to hierarchically group
  heterogeneous clients and privacy friendly.
- Trained **cluster-specific federated LSTM models** and evaluated metrics.
- Build a React interface to for users interacting with models

**Tech:** Python, PyTorch, Machine Learning, Federated Learning, LSTM, Time-Series Forecasting, FastApi, React, deep learning, ETL pipelines, TypeScript

---

#### Wind Power Forecasting System
🔗 https://github.com/bowl1/short-time-wind-energy-forecasting-system  
📡 API Docs: http://13.60.68.102/docs  

- Developed a **machine learning–powered forecasting service** using real-world weather and energy data.
- Built a RESTful API, tracked experiments with MLflow, and deployed the system on a cloud VM using Docker and CI/CD.

**Tech:** Python, FastAPI, scikit-learn, MLflow, Docker, AWS, MLflow，XGboost, Ramdom Forest

---

#### Crypto Data Pipeline — Production-Style Lakehouse
🔗 https://github.com/bowl1/crypto-data-pipeline

A data engineering pipeline that ingests real-time cryptocurrency market data and transforms it into analysis-ready datasets using a modern lakehouse architecture.

- Designed a three-layer lakehouse architecture (Raw → Silver → Gold) on Databricks with Delta Tables and AWS S3
- Built Apache Airflow DAGs for orchestrated, scheduled ingestion from Binance and Coinbase APIs
- Implemented dbt transformation models for cross-source price reconciliation and business-ready aggregations
- Applied incremental MERGE operations to avoid full reloads and reduce compute cost
- Built automated data quality checks covering freshness, completeness, null rates, and duplicate detection
- Containerised the full pipeline with Docker for reproducible local development

**Tech**: Python, Apache Airflow, dbt, Databricks, Delta Lake, AWS S3, Parquet, SQL, Docker

---
---

### Java:

#### Search Engine with Different Index Structures  
🔗 https://github.com/bowl1/Search-Engine-with-different-index  

- Implemented a **mini search engine** using forward and inverted indexing.
- Indexed **25,000+ Wikipedia articles** and benchmarked query performance.

**Tech:** Java, SQLite, Indexing, JUnit testing, JMH benchmark, forward index, inverted index

---
---

### Mobile App:

#### 📞 Escape — Fake Incoming Call App &nbsp;![Android](https://img.shields.io/badge/Published_on-Google_Play-3DDC84?logo=google-play&logoColor=white)
🔗 https://github.com/bowl1/Escape_mobile_app  
📲 **Google Play:** https://play.google.com/store/apps/details?id=com.libowen.fakecall

A **published Android app** that generates convincing fake incoming calls to help users gracefully exit awkward situations. Tap once and your phone rings with a realistic ringtone, vibration, caller name — the works.

- One-tap call generation with random callers using relationship labels (Mom, Boss, etc.)
- Custom caller support — personalize name, number, and photo
- Scheduling — delay calls from seconds up to 8 hours, works even when the phone is asleep
- Lock-screen integration — calls appear as genuine incoming calls on the lock screen
- Contact management — save favorite fake callers with default selection

**Tech:** Kotlin, Jetpack Compose, Material Design 3, Hilt, Room, DataStore, AlarmManager, Foreground Service, Clean Architecture

---

#### 🥗 FridgeToFood — Recipe Discovery Mobile App  
🔗 https://github.com/bowl1/Food-Mobile-App


A cross-platform recipe app that turns fridge ingredients into practical meal ideas to reduce food waste.  Built with **React Native (Expo + TypeScript)** and a **Node.js/Express** backend with **Firebase Auth + Firestore**.

- Firebase Auth login/register
- Recipe search via backend proxy to third-party API + dietary tag filtering (with strict vegetarian post-filter)
- Favorites with offline-first **SQLite** cache + background sync
- Profile with avatar upload (camera / photo library)
- Recipe detail long-image sharing + local notifications on favorite save

**Tech:** Expo (React Native), TypeScript, React Navigation, Zustand, TanStack Query, expo-sqlite, expo-notifications, Express, Firebase Admin, Firestore

---
