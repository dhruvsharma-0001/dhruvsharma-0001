
<div align="center">

# Dhruv Sharma

### Python · Generative AI · LLM Systems

*I build grounded, measurable AI systems: retrieval pipelines, agent workflows, and an LLM inference engine written from scratch.*

<a href="https://www.linkedin.com/in/dhruv-sharma9015150070/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge" alt="LinkedIn"/></a>
<a href="mailto:dhruvsharmahp0001@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://YOUR-RESUME-LINK"><img src="https://img.shields.io/badge/Resume-View-1F2937?style=for-the-badge" alt="Resume"/></a>

</div>

---

## 👨‍💻 About

I'm a **BTECH/IITM BS DEGREE** student at **UIIT SHIMLA/IIT MADRAS**, focused on building LLM applications that are **grounded, tested and measurable**. I care about what makes AI systems trustworthy in practice (citations, safety guardrails, evaluation, latency, observability), not just the demo.

- 🔎 **Retrieval & grounded QA**: hybrid BM25 + dense search, rank fusion, citation validation
- 🤖 **Agentic workflows**: LangGraph state machines with self-critique and retry loops
- ⚙️ **LLM systems**: KV-cache inference, OpenAI-compatible serving, tracing with LangSmith
- 🎯 **Open to internships and entry-level roles** in Generative AI, LLM applications and Python backend development

---

## 🚀 Featured Projects

### 🌿 [AyurCite](https://github.com/dhruvsharma-0001/AyurCite): citation-grounded QA over classical Ayurvedic texts
A fully local question-answering engine over the *Charaka* and *Sushruta Samhitas* that answers only from retrieved verses, or refuses.
- Hybrid retrieval (BM25 + dense embeddings in LanceDB, fused with Reciprocal Rank Fusion) over **5,905 verse records**
- Pre-retrieval **safety router** (0.006 ms) blocking emergencies, pregnancy and medication queries, with **100% catch rate** on a 40-query adversarial set
- Deterministic **citation validator**: 0% hallucinated citations, versus 72.4% for the same LLM without retrieval
- Runs fully offline with a local Gemma model via Ollama, at zero inference cost

`Python` `LanceDB` `BM25` `Ollama` `RAG` `Evaluation`

### ⚡ [nano-llm-engine](https://github.com/dhruvsharma-0001/nano-llm-engine): LLM inference engine from scratch
A lightweight inference engine in pure PyTorch for Llama-family models, implementing the architecture without Hugging Face's modeling code.
- Implements **RoPE, RMSNorm, Grouped-Query Attention, SwiGLU** and a dynamic **KV cache** (up to **3.65× faster** decoding than naive recomputation)
- **Numerically verified** against Hugging Face outputs (logit difference < 10⁻⁴)
- Advanced sampling: temperature, top-k, top-p, min-p, repetition penalty
- **OpenAI-compatible** `/v1/chat/completions` server with streaming (SSE)

`Python` `PyTorch` `Transformers` `Safetensors` `SSE`

### ♻️ [EPR Compliance Copilot](https://github.com/dhruvsharma-0001/epr-copilot): AI research assistant for India's plastic-waste EPR rules
A citation-grounded compliance copilot plus a deterministic liability calculator for CPCB Schedule II (Plastic Waste Management Rules).
- **LangGraph RAG pipeline** with citation badges and confidence ratings over statutory knowledge chunks
- Deterministic **EPR liability and penalty calculator** (Category I–IV targets, certificates, environmental compensation)
- **Multi-provider LLM routing** (Groq, OpenRouter, Gemini, Claude, OpenAI) with an offline mock-mode fallback
- **18 automated tests**, Docker Compose deployment, printable audit-ready reports

`Python` `Flask` `LangChain` `LangGraph` `Docker` `pytest`

### 🩺 [medbook-ai](https://github.com/dhruvsharma-0001/medbook-ai): sub-millisecond medical textbook search
An in-memory hybrid retrieval engine that lets students search their own textbooks with exact book, chapter and page citations.
- Dense **HNSW** + sparse **BM25**, combined with weighted RRF (**~0.85 ms p50** total retrieval)
- Medical **acronym expansion** (~90 terms) at index and query time
- 100% offline and private, served through a **FastAPI** API and web UI, Docker-ready

`Python` `FastAPI` `HNSW` `BM25` `Docker`

### 🧠 [PaperMind AI](https://github.com/dhruvsharma-0001/PaperMind-Ai): self-correcting research-paper tutor
An agent that ingests an arXiv paper or PDF and explains it from first principles, and won't finish until it passes its own comprehension check.
- **Cyclic LangGraph** pipeline: ingest → understand (Feynman-style breakdown) → recall quiz → apply
- **Feedback loop**: if the quiz score drops below 0.7, it re-reads the paper with targeted feedback (up to 3 attempts)
- Generates PyTorch reference code and a teach-back summary, with a live web dashboard
- Multi-provider LLM support (Groq default)

`Python` `LangGraph` `Groq` `arXiv API`

### 🔬 [Fact-Checked Research Agent](https://github.com/dhruvsharma-0001/Fact-Checked-Research-Agent): research agent that audits itself
A LangGraph agent that plans, searches, critiques its own findings and re-investigates weak claims before writing a report.
- **Plan → Research → Critique → Write** graph, re-researching only the flagged sub-questions (capped revision budget)
- Parallel web search (DuckDuckGo / Tavily) with per-claim source and confidence tracking
- Streamlit UI with live graph tracker and a CLI with mock mode for offline testing

`Python` `LangGraph` `Streamlit` `Tavily`

---

## 🧩 More Projects

| Project | What it is | Stack |
|---|---|---|
| [**ScholarLens AI**](https://github.com/dhruvsharma-0001/ScholarLens-Ai) | Research-paper comprehension engine with an 8-layer analysis stack, Anki flashcard export, semantic search and RAG chat over a paper library | `Python` `FastAPI` |
| [**Daily Vocab**](https://github.com/dhruvsharma-0001/daily-vocab-webapp-newsletter) | Spoken-English coach with a daily newsletter, Hindi meanings, voice practice and SM-2 spaced-repetition flashcards | `Python` `Flask` `Groq` |
| [**RAG Observability with LangSmith**](https://github.com/dhruvsharma-0001/RAG_Observability_Using_LangSmith) | PDF RAG pipeline iterated over four versions, improving latency and tracing with LangSmith | `LangChain` `FAISS` `LangSmith` |
| [**LangGraph Blog Project**](https://github.com/dhruvsharma-0001/LangGraph_Blog_Project) | Blog-writing agent workflow built up in stages, with a frontend | `LangGraph` `Jupyter` |
| [**LangGraph Chatbot**](https://github.com/dhruvsharma-0001/Chat-Bot-Using-LangGraph) | Chatbot with database-backed memory and tool calling | `LangGraph` `Python` |
| [**Placement Portal**](https://github.com/dhruvsharma-0001/Placement_Portal_College-main) | Multi-role (admin / company / student) placement management system with drive approvals, applications and resume uploads | `Flask` `SQLite` |
| [**Spendly**](https://github.com/dhruvsharma-0001/Spendly) | Expense tracker with auth, expense CRUD and a pytest suite, built with a Gemini CLI agent workflow | `Flask` `SQLite` `pytest` |

---

## 🛠️ Tech Stack

**Languages & Backend**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)

**GenAI & LLM**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![LangSmith](https://img.shields.io/badge/LangSmith-1C3C3C?style=flat-square)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square)

**Retrieval & Search**

![RAG](https://img.shields.io/badge/RAG-4B5563?style=flat-square)
![Hybrid Search](https://img.shields.io/badge/BM25%20%2B%20Dense-4B5563?style=flat-square)
![FAISS](https://img.shields.io/badge/FAISS-4B5563?style=flat-square)
![LanceDB](https://img.shields.io/badge/LanceDB-4B5563?style=flat-square)
![HNSW](https://img.shields.io/badge/HNSW-4B5563?style=flat-square)

**Tools & Practices**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)

---

## 🌱 Currently

- Extending **AyurCite** to more texts and Devanagari-script retrieval
- Going deeper on **LLM inference** (KV cache, sampling, serving) and **RAG evaluation**
- Looking for an **internship or entry-level role** where I can build production LLM applications

---

<div align="center">



*Building one measurable project at a time.*

</div>
