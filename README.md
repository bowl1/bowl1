# 👋 Hi, I’m Bowen Li

📍 Copenhagen, Denmark  

---

## 🧩 Projects

### ✍️ HeyWrite — Intent-Driven AI Writing Assistant

🔗 https://github.com/bowl1/Hey_write  
🌐 https://hey-write.vercel.app

A full-stack AI application that turns a one-sentence user intent into structured professional documents (emails, reports, meeting summaries).

### Features
- Designed a **semantic template routing system** using embeddings + vector search to select the correct document structure before generation
- Implemented **context-aware editing** — updates only relevant sections instead of regenerating the whole document
- Built fallback **wild mode generation** when no template matches
- Similarity-based retrieval filtering (semantic gating)
- Handles chat history and incremental document refinement
- Deployment with Docker, GitHub Actions, Vercel, Render

**Tech:** React, TypeScript, Python, FastAPI, LangChain, OpenAI API Embeddings, OpenAI-compatible LLM APIs (DeepSeek), RAG, ChromaDB, Docker, GitHub Actions, Vercel, Render

---

### 👻 My Little Ghost — Anonymous Social Platform  
🔗 https://github.com/bowl1/social-chat-app  
🌐 https://social-chat-dk.vercel.app  
Figma: https://github.com/bowl1/Figma-Portfolio  (user case interview, UI design and mini component library)

- React **anonymous social sharing platform** , developing from user interview -> product requirement-> logo design -> UI design-> usability testing -> code implementing. 
- Supports text and media posts with **per-group aliases**, preserving user privacy.
- Implemented authentication, media uploads, and scalable feed interactions.

**Tech:** React, Tanstack Query, Zustand, TypeScript, Next.js, PostgreSQL, Prisma, Firebase Auth, Vercel, Figma, HTML,CSS, Styled component

---

### 🤖 Ask My Docs — PDF-based RAG Chatbot  
🔗 https://github.com/bowl1/AskMyDocs-AI-app  
🌐 https://askmydocument.vercel.app  

- Built a **document-grounded AI assistant** that answers questions strictly from
  user-uploaded PDFs.
- Always provides **page-level citations** and refuses to hallucinate.
- Deployed backend and frontend separately with automated CI/CD pipelines.

**Tech:** Python, LangChain, TypeScript, FastAPI, React, RAG, ChromaDB, Tailwind CSS, Docker, GitHub Actions, LLMs, Vercel, AWS, HuggingFace，OpenAI-compatible LLM APIs (DeepSeek)

---

### 🌀 Behaviour-Aware Federated Wind Power Forecasting  
**Master’s Thesis Project**  
🔗 Strategy design and model training (Python, FL, LSTM): https://github.com/bowl1/Wind-and-AI

🔗 Interface application: https://github.com/bowl1/Behaviour-Aware-Federated-Wind-Power-Forecasting-System-demo

- Built a **distributed wind power forecasting system** across **400+ independent wind turbines**.
- Data preprocessing and feature engineering 
- Designed a **behaviour-aware auto-split clustering strategy** to hierarchically group
  heterogeneous clients and privacy friendly.
- Trained **cluster-specific federated LSTM models** and evaluated metrics.
- Build a React interface to for users interacting with models

**Tech:** Python, PyTorch, Machine Learning, Federated Learning, LSTM, Time-Series Forecasting, FastApi, React, deep learning, ETL pipelines, TypeScript

---

### 🥗 FridgeToFood — Recipe Discovery Mobile App  
🔗 https://github.com/bowl1/Food-Mobile-App


A cross-platform recipe app that turns fridge ingredients into practical meal ideas to reduce food waste.  Built with **React Native (Expo + TypeScript)** and a **Node.js/Express** backend with **Firebase Auth + Firestore**.

- Firebase Auth login/register
- Recipe search via backend proxy to third-party API + dietary tag filtering (with strict vegetarian post-filter)
- Favorites with offline-first **SQLite** cache + background sync
- Profile with avatar upload (camera / photo library)
- Recipe detail long-image sharing + local notifications on favorite save

**Tech:** Expo (React Native), TypeScript, React Navigation, Zustand, TanStack Query, expo-sqlite, expo-notifications, Express, Firebase Admin, Firestore

---

### 🌬️ Wind Power Forecasting System (API & Deployment)  
🔗 https://github.com/bowl1/short-time-wind-energy-forecasting-system  
📡 API Docs: http://13.60.68.102/docs  

- Developed a **machine learning–powered forecasting service** using real-world weather and energy data.
- Built a RESTful API, tracked experiments with MLflow, and deployed the system on a cloud VM using Docker and CI/CD.

**Tech:** Python, FastAPI, scikit-learn, MLflow, Docker, AWS, MLflow

---

### 🔎 Search Engine with Different Index Structures  
🔗 https://github.com/bowl1/Search-Engine-with-different-index  

- Implemented a **mini search engine** using forward and inverted indexing.
- Indexed **25,000+ Wikipedia articles** and benchmarked query performance.

**Tech:** Java, SQLite, Indexing, JUnit testing, JMH benchmark, forward index, inverted index

---


📫 **Contact**  
Email: bowenivy0@gmail.com