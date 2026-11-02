# 👋 Hi, I’m Bowen Li

🧬 Carbon-based creature shipping bugs

📍 Copenhagen, Denmark  

📫 **Contact**  
Email: bowenivy0@gmail.com


## 🧩 Projects

---
### Full-stack & AI:

#### ✍️ HeyWrite — AI-Powered Template Selection & Content Generation

🔗 [GitHub](https://github.com/bowl1/Hey_write)  
🌐 [Live Demo](https://hey-write.vercel.app)

An AI-powered content generation system that understands user intent, retrieves and selects the most relevant writing templates, and generates context-aware content based on their structure and style. Combines **hybrid retrieval (semantic search + BM25)** with **LangGraph agent workflows** to automate template selection, drafting, evaluation, and iterative refinement.

**Features**
- **Intelligent template selection:** Matches user intent to suitable writing templates through pgvector semantic search, BM25 keyword retrieval, weighted reranking, and relevance-score gating
- **RAG-based content generation:** Uses retrieved templates as structural and stylistic guidance to produce context-aware drafts instead of relying solely on generic LLM prompts
- **Agentic workflow orchestration:** Built a LangGraph-controlled loop for planning, tool execution, template retrieval, drafting, evaluation, revision, and bounded retries
- **Dual generation strategies:** Supports template-guided generation and freeform generation when users prefer creative flexibility
- **Iterative refinement:** Enables multi-turn editing, session recovery, conversation memory, previous-result retrieval, and revision summaries
- **Quality evaluation:** Combines deterministic validation with optional LLM-as-a-Judge evaluation before saving final outputs
- **LLM observability:** Integrated Langfuse to trace agent execution, tool calls, evaluation results, retries, and available token usage and latency metrics
- **Secure user workspaces:** Supabase Auth, PostgreSQL, and backend token validation for private templates, conversations, and saved drafts
- **Multilingual support:** English, Chinese, and Danish, with configurable tone and writing style
- **Deployment & CI/CD:** Docker, GitHub Actions, Vercel, and Render

**Tech:** React, TypeScript, Python, FastAPI, LangGraph, LangChain, Langfuse, RAG, pgvector, BM25, Supabase (Auth, PostgreSQL), DeepSeek API, OpenAI Embeddings, Docker, GitHub Actions, Vercel, Render

---

#### 🥗 FridgeOut — AI-Powered Recipe Mobile App

🔗 [GitHub](https://github.com/bowl1/Food-Mobile-App) | [iOS TestFlight](https://testflight.apple.com/join/QqwUY2qK)

An AI-powered iOS app that transforms fridge photos into personalized recipes to reduce food waste. Built with **React Native (Expo + TypeScript)** and a **Python/FastAPI** backend, integrating **OpenAI multimodal models, LangGraph, MCP, and Supabase**.

- **AI ingredient recognition** from fridge photos, with user review and editable inventory
- **Agentic recipe generation** using LangGraph, structured outputs, deterministic guardrails, LLM-as-a-Judge evaluation, and bounded retries
- **MCP-based tool integration** for authenticated access to user inventory and dietary preferences
- **Supabase Auth + PostgreSQL** with Row Level Security (RLS) for secure, user-specific data
- **Offline-aware favorites and inventory**, with local caching and synchronization
- **AI-generated recipe images** and subscription management via RevenueCat and Apple in-app purchases
- **Testing & AI evaluation:** pytest, Node.js and SQL tests, TypeScript checks, custom offline evaluation pipelines for ingredient recognition and recipe quality, and regression testing
- **LLM observability:** Langfuse tracing for generation rounds, guardrail rejections, evaluation scores, and recipe selection outcomes during development
- **CI/CD & deployment:** Automated checks with GitHub Actions, FastAPI deployment on Render, and iOS distribution via Expo EAS and TestFlight

**Tech:** React Native, Expo, TypeScript, Python, FastAPI, OpenAI API, LangGraph, MCP, Supabase, PostgreSQL, RevenueCat, Langfuse, pytest, GitHub Actions, Render, Expo EAS

---

#### Ask My Docs — PDF-based RAG Chatbot  
🔗 https://github.com/bowl1/AskMyDocs-AI-app  
🌐 https://askmydocument.vercel.app  

- Built a **document-grounded AI assistant** that answers questions strictly from user-uploaded PDFs.
- Always provides **page-level citations** and refuses to hallucinate.
- Deployed backend and frontend separately with automated CI/CD pipelines.

**Tech:** Python, LangChain, TypeScript, FastAPI, React, RAG, ChromaDB, Tailwind CSS, Docker, GitHub Actions, LLMs, Vercel, AWS, HuggingFace，OpenAI-compatible LLM APIs (DeepSeek)

---

#### 👻 My Little Ghost — Anonymous Social Platform  
🔗 https://github.com/bowl1/social-chat-app  
🌐 https://social-chat-dk.vercel.app  
Figma: https://github.com/bowl1/Figma-Portfolio  (user case interview, UI design and mini component library)

- React **anonymous social sharing platform** , developing from user interview -> product requirement-> logo design -> UI design-> usability testing -> code implementing. 
- Supports text and media posts with **per-group aliases**, preserving user privacy.
- Implemented authentication, media uploads, and scalable feed interactions.

**Tech:** React, Tanstack Query, Zustand, TypeScript, Next.js, PostgreSQL, Prisma, Firebase Auth, Vercel, Figma, HTML,CSS, Styled component

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

### Java:

#### Search Engine with Different Index Structures  
🔗 https://github.com/bowl1/Search-Engine-with-different-index  

- Implemented a **mini search engine** using forward and inverted indexing.
- Indexed **25,000+ Wikipedia articles** and benchmarked query performance.

**Tech:** Java, SQLite, Indexing, JUnit testing, JMH benchmark, forward index, inverted index

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

