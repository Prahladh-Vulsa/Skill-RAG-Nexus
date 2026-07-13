# 🚀 Skill RAG Nexus

<p align="center">
  <strong>
    An AI-powered Career & Research Assistant that combines Multi-Tool Retrieval-Augmented Generation (RAG), Resume Analysis, Web Search, and Job Discovery using LangChain and Google Gemini.
  </strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-Agent-1C3C3C?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Google-Gemini-4285F4?style=for-the-badge&logo=google"/>
  <img src="https://img.shields.io/badge/ChromaDB-Vector%20Store-7E57C2?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/HuggingFace-Embeddings-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/>
  <img src="https://img.shields.io/badge/Tavily-Web%20Search-0A84FF?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/MCP-Protocol-6C63FF?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/RapidAPI-JSearch-00C7B7?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Google-Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white"/>
</p>

<p align="center">
  <img src="assets/architecture.png" alt="Skill RAG Nexus Architecture" width="100%">
</p>

---

# 📖 Overview

Skill RAG Nexus is an intelligent **Multi-Tool AI Agent** that combines **Retrieval-Augmented Generation (RAG)**, **resume analysis**, **real-time web search**, and **job discovery** into a single unified workflow.

Unlike traditional RAG applications that retrieve information from only one document, Skill RAG Nexus intelligently selects the most appropriate tool based on the user's query. It can search research papers, analyze resumes, retrieve the latest information from the web, and discover relevant job opportunities before generating a comprehensive response using **Google Gemini**.

By integrating **LangChain Agents**, **ChromaDB**, **Model Context Protocol (MCP)**, and **external APIs**, the project demonstrates how multiple AI components can collaborate to build a practical assistant for **research, learning, and career development**.

---

# ✨ Features

- 📄 Load research papers from PDF
- 📄 Load resumes from PDF
- ✂️ Split documents into semantic chunks
- 🧠 Generate embeddings using Hugging Face Sentence Transformers
- 🗄️ Store embeddings in ChromaDB
- 🔍 Semantic similarity search over research papers
- 👤 Retrieve and analyze resume information
- 🌐 Live web search using Tavily Search (MCP)
- 💼 Search real-time job opportunities using RapidAPI JSearch
- 🤖 Generate responses with Google Gemini 2.5 Flash
- 🧩 LangChain Agent that automatically selects the appropriate tool
- 🔄 Combine information from multiple sources into a single response
- 💬 Answer research, career, and technical questions intelligently

---

# 🏗️ Architecture

```text
                             User Question
                                   │
                                   ▼
                     LangChain Multi-Tool Agent
                                   │
     ┌───────────────┬──────────────┼───────────────┐
     │               │              │               │
     ▼               ▼              ▼               ▼
Research Tool   Resume Tool   Tavily Search   Job Search API
     │               │              │               │
     ▼               ▼              ▼               ▼
Research DB     Resume DB      Web Results     Job Listings
     │               │              │               │
     └───────────────┴───────┬──────┴───────────────┘
                             ▼
                    Google Gemini 2.5 Flash
                             │
                             ▼
                       Final AI Response
```

---

# ⚙️ Workflow

1. Load a research paper using **PyPDFLoader**.
2. Load a resume using **PyPDFLoader**.
3. Split both documents using **RecursiveCharacterTextSplitter**.
4. Generate embeddings with **Hugging Face all-mpnet-base-v2**.
5. Store embeddings inside separate **ChromaDB** vector collections.
6. Create semantic retrieval tools for the research paper and resume.
7. Connect **Tavily Search** through **Model Context Protocol (MCP)**.
8. Create a **Job Search Tool** using **RapidAPI JSearch**.
9. Build a **LangChain Multi-Tool Agent**.
10. The agent automatically selects the most suitable tool(s) for each query.
11. **Google Gemini** combines the retrieved information into a comprehensive response.

---

# 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| Language | Python |
| Development Environment | Google Colab |
| Framework | LangChain |
| Agent Framework | LangGraph |
| LLM | Google Gemini 2.5 Flash |
| Embeddings | Hugging Face (`all-mpnet-base-v2`) |
| Vector Database | ChromaDB |
| Web Search | Tavily Search (MCP) |
| Job Search | RapidAPI JSearch |
| PDF Loader | PyPDFLoader |

---

# 📂 Project Structure

```text
Skill-RAG-Nexus/
│
├── assets/
│   └── architecture.png
│
├── Skill_RAG_Nexus.ipynb
├── README.md
├── requirements.txt
└── LICENSE
```

---

# 🚀 Getting Started

## Prerequisites

- Python 3.10+
- Google Colab (Recommended)
- Google Gemini API Key
- Tavily API Key
- RapidAPI Key

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Configure API Keys

Store the following secrets in **Google Colab**:

```text
GEMINI_API_KEY
TAVILY_API_KEY
RAPIDAPI_KEY
```

No API keys are hardcoded inside the notebook.

---

## Run the Project

1. Open `Skill_RAG_Nexus.ipynb` in Google Colab.
2. Upload a research paper.
3. Upload a resume.
4. Configure the required API keys.
5. Run all notebook cells.
6. Start interacting with the AI agent.

---

# 💬 Example Queries

### 📚 Research

> Summarize the methodology proposed in the research paper.

---

### 👤 Resume

> What machine learning skills are present in my resume?

---

### 🌐 Web Search

> What are the latest developments related to this research topic?

---

### 💼 Job Search

> Find Machine Learning Engineer jobs matching my resume.

---

### 🤖 Multi-Tool Query

> Compare my resume with the research paper, identify missing skills, recommend suitable Machine Learning jobs, and include the latest industry trends.

The agent will automatically:

- 📄 Retrieve information from the research paper
- 👤 Analyze the uploaded resume
- 🌐 Search the web for recent information
- 💼 Find matching job opportunities
- 🤖 Combine all retrieved information using Google Gemini
- ✅ Generate a comprehensive response

---

# 🔮 Future Improvements

- 📚 Multi-document RAG
- 🧠 Long-term conversation memory
- 🌐 Streamlit / Gradio web interface
- 🔀 Hybrid Retrieval (BM25 + Vector Search)
- 📖 Source citations
- 🤖 Support for multiple LLM providers
- 📊 Resume skill-gap analysis
- 🎯 Personalized career recommendations
- ☁️ Docker deployment
- 🔐 User authentication

---

# 👨‍💻 Author

**Prahladh Vulsa**

GitHub: **https://github.com/Prahladh-Vulsa**

---

<p align="center">
⭐ If you found this project useful, consider giving it a star!
</p>
