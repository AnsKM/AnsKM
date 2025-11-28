# Ans Khalid
### AI Engineer | Full-Stack Developer | Systems Architect

Building production-ready AI systems that deliver measurable business impact.
Specializing in real-time audio processing, LLM integration, and desktop applications.

**Munich, Germany** 🇩🇪 | **German (C1)** | **Open to AI/Backend roles**

📧 ansmohal@gmail.com | [LinkedIn](https://linkedin.com/in/anskhalid) | 💼 [Portfolio](#)

---

## 🎯 Core Technical Expertise

### AI & LLM Integration
![Python](https://img.shields.io/badge/Python-Expert-3776AB?logo=python&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_2.5-Expert-4285F4?logo=google&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-Expert-1C3C3C?logoColor=white)

**Impact**: Built 5+ production AI systems serving 100+ users
- **Interview Assistant**: Real-time AI suggestions with <2s response time
- **Memory Agent**: Sub-100ms vector search with Qdrant + Voyage AI
- **Claude Workflows**: 6-module automation suite for content processing

**Key Technologies**: GPT-5.1, Claude Opus 4.5, Gemini 3.0, RAG pipelines, Vector DBs (Qdrant, ChromaDB, Pinecone)

---

### Voice AI & Real-Time Audio Processing
![Rust](https://img.shields.io/badge/Rust-Expert-000000?logo=rust&logoColor=white)
![Whisper](https://img.shields.io/badge/Whisper-Expert-412991?logoColor=white)
![Deepgram](https://img.shields.io/badge/Deepgram-Expert-13EF93?logoColor=white)

**Impact**: Processed 100+ hours of voice data with <300ms latency
- **Whisper-Flow**: Cross-platform voice dictation with local/cloud options
- **Meeting Assistant**: Dual-channel audio capture via Core Audio Taps
- **Real-time STT**: Multi-provider architecture (Deepgram, Whisper, Gemini Live)

**Key Technologies**: Tauri, CPAL, Deepgram Nova-3, Whisper.rs, tokio async runtime

---

### Desktop Application Development
![Tauri](https://img.shields.io/badge/Tauri-Expert-24C8D8?logo=tauri&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-Expert-007ACC?logo=typescript&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-Advanced-47848F?logo=electron&logoColor=white)

**Impact**: Shipped 3 cross-platform desktop apps with 20K+ LOC
- **Meeting Assistant**: 20,000+ lines of Rust/TypeScript production code
- **Free Cluely**: Invisible AI assistant with local/cloud LLM support
- **Whisper-Flow**: Voice dictation with GPU acceleration (macOS/Windows/Linux)

**Key Technologies**: React 19, Zustand, SQLite, native system integration (Core Audio, IPC)

---

<details>
<summary><b>📦 Full-Stack Development</b> (Click to expand)</summary>

### Frontend
- **React + TypeScript**: Production apps with Vite, Material-UI, Tailwind CSS
- **State Management**: Zustand, TanStack Query, Redux patterns
- **Build Tools**: Vite 7, Webpack, optimized for performance

### Backend
- **Python**: FastAPI, Flask (MCP servers, AI APIs)
- **Node.js**: Express, RESTful APIs, WebSocket servers
- **Rust**: Tauri backends, system-level programming

### Databases
- **Vector DBs**: Qdrant, ChromaDB, Pinecone (semantic search)
- **Relational**: PostgreSQL, SQLite (local-first architecture)
- **NoSQL**: Firebase Firestore, Redis caching

</details>

<details>
<summary><b>🤖 AI/ML Ecosystem</b></summary>

### LLM Providers
- Google Gemini 2.5/3.0, OpenAI GPT-5.1, Claude 4.5, Grok 4.1, DeepSeek, Mistral

### Frameworks & Tools
- LangChain, LangGraph (multi-agent systems), LlamaIndex
- Prompt engineering, context optimization, RAG architectures
- Model Context Protocol (MCP) server development

### Voice AI Stack
- Whisper (local inference with CPU/GPU)
- Deepgram (streaming transcription)
- Groq API (fast inference)

</details>

<details>
<summary><b>🛠️ DevOps & Infrastructure</b></summary>

- **Containerization**: Docker, multi-stage builds
- **CI/CD**: GitHub Actions, automated testing
- **Cloud**: Azure, Firebase (Auth, Functions, Firestore)
- **Automation**: n8n workflows, Apify actors, web scraping

</details>

---

## 🔧 Additional Technologies

**Systems Programming**: Core Audio Taps API, CPAL, audio processing, IPC
**Web**: Chrome Extension APIs (Manifest v3), Shadow DOM, content scripts
**Tools**: Git, npm/cargo/pip, Turborepo monorepos, Firebase CLI
**Languages**: SQL, Bash/Shell, HTML/CSS

---

## 🎙️ Interview Assistant - Real-Time AI Interview Copilot

![Status](https://img.shields.io/badge/Status-Production_MVP-success)
![Private](https://img.shields.io/badge/Repo-Private-orange)
![Lines](https://img.shields.io/badge/Lines-20K+-blue)

**Private Repository** | **20,000+ lines of Rust/TypeScript** | **Production MVP**

A sophisticated desktop application providing real-time AI assistance during technical meetings through live audio processing and intelligent response generation.

### Business Impact
- **Sub-2 second** AI response generation with context-aware prompting
- **<300ms latency** real-time transcription with Deepgram Nova-3
- **Zero driver installation** via macOS Core Audio Taps API (14.2+)
- **90% cost reduction** with explicit prompt caching

### Technical Architecture

**Audio Pipeline**:
```
[Microphone + System Audio] → Core Audio Taps API
  ↓
24kHz Resampling (Rubato) → VAD Filter → Crossbeam Channels
  ↓
Multi-STT (Deepgram/Gemini Live/Whisper) → SQLite Storage
  ↓
Context Assembly → Gemini 2.5 Flash Lite → Streaming UI (SSE)
```

### Key Technical Achievements
- **Dual-Channel Audio Capture**: Simultaneous mic + system audio via native macOS API
- **Multi-Provider STT**: Hot-swappable between Deepgram, Gemini Live, OpenAI Whisper
- **Advanced Audio Processing**: 24kHz resampling with anti-aliasing, VAD filtering
- **Async Architecture**: Tokio runtime with lock-free crossbeam channels
- **Local Persistence**: SQLite with UUID v7 time-ordered session IDs
- **Context Management**: RAG-style interview prep document loading

### Tech Stack
- **Backend**: Rust, Tauri 2.0, CPAL, tokio, rubato, whisper-rs
- **Frontend**: React 19, TypeScript, Zustand, TanStack Query, Vite
- **AI/STT**: Gemini Live, Deepgram Nova-3, OpenAI Whisper
- **Database**: SQLite with sqlx, async migrations

### Features
- 🎤 Real-time dual audio capture (no drivers needed)
- 🧠 Context-aware AI with loaded interview prep notes
- ⚡ Sub-500ms end-to-end latency
- 🔒 100% local data storage (no cloud sync)
- 🎨 Transparency mode with adjustable opacity
- ⌨️ Global keyboard shortcuts

**[📸 Screenshots Coming Soon]** | **[📄 Architecture Documentation Coming Soon]**

**Cost**: <$1.00 per 2-hour interview session

---

## 🎤 Murmur - AI Voice Dictation with Privacy

![License](https://img.shields.io/badge/License-AGPLv3-blue)
![Platform](https://img.shields.io/badge/Platform-Cross--Platform-brightgreen)

**[View on GitHub](https://github.com/AnsKM/murmur)** | **Tauri + React + Rust** | **Cross-Platform**

AI-powered voice dictation desktop app with local-first privacy and flexible backend options.

### Business Impact
- **100% privacy** option via local Whisper inference
- **Multi-language** UI support (English, Spanish, French)
- **Cross-platform** deployment (macOS, Windows, Linux)
- **Auto-learning dictionary** with AI-powered suggestions

### Technical Highlights
- **Local Whisper Inference**: CPU and GPU-accelerated (Vulkan/Metal)
- **Streaming Transcription**: Deepgram Nova-3 WebSocket integration
- **LLM Post-Processing**: Custom tone personalization (Groq Llama)
- **Smart Dictionary**: Glossary terms + replacement rules + auto-learning
- **Turborepo Monorepo**: Shared packages for voice-ai, types, utilities

### Architecture Philosophy
> **"Rust is the API, TypeScript is the Brain"**
- Rust provides native capabilities (audio, keyboard, SQLite, Whisper)
- TypeScript handles all business logic and state management
- Repository pattern abstracts local (SQLite) vs. cloud (Firebase)

### Tech Stack
- **Framework**: Tauri 2, React 19, TypeScript, Vite 7
- **State**: Zustand with Immer
- **Audio**: CPAL, whisper-rs, WebSocket (tokio-tungstenite)
- **AI**: Whisper (local), Groq API, Deepgram Streaming
- **UI**: Material-UI v7, React Router v6, react-intl

**[Download Releases](https://github.com/AnsKM/whisper-flow/releases)** | **[View Documentation](https://github.com/AnsKM/whisper-flow)**

---

## 🤖 Claude Code Workflows - AI Content Automation Suite

![Status](https://img.shields.io/badge/Status-Production-success)
![Modules](https://img.shields.io/badge/Modules-6-blue)

**[View on GitHub](https://github.com/AnsKM/claude_code_workflows)** | **Python + FastAPI + Gemini** | **6 Specialized Modules**

Comprehensive AI-powered tools for content extraction, market analysis, and automation.

### Business Impact
- **6 production modules** serving multiple business use cases
- **Automated workflows** saving hours of manual research
- **Market intelligence** for competitive analysis and strategy
- **Educational content** generation from YouTube videos

### Modules

1. **YouTube Educator**
   - Converts videos → study guides, lesson plans, references
   - AI-generated summaries and code snippet extraction

2. **Meta Ad Analyzer**
   - Facebook/Meta ad scraping via Apify
   - Competitive intelligence and performance tracking
   - Export to JSON/CSV/Excel with web dashboard

3. **YouTube Trends**
   - Multi-channel monitoring and trend detection
   - Viral prediction scoring with PostgreSQL/SQLite storage

4. **AI Offers Intelligence**
   - Google Sheets integration for market analysis
   - Interactive dashboards with price trend analysis

5. **AI Job Hunter**
   - Real job scraping from StepStone.de, Indeed.de (Apify)
   - Flask dashboard with salary trends and skills analysis

6. **LinkedIn Personal Branding**
   - Complete profile scraping and strength assessment
   - 7/30/90-day actionable growth plans

### Tech Stack
- **AI**: Google Gemini 2.5, prompt engineering
- **Scraping**: Apify actors, BeautifulSoup
- **Web**: FastAPI, Flask dashboards
- **Storage**: Google Sheets API, PostgreSQL, JSON/CSV
- **Tools**: Batch processing, automated reporting

**[View Tools Documentation](https://github.com/AnsKM/claude_code_workflows#readme)** | **[Download Channel Transcripts Tool](https://github.com/AnsKM/claude_code_workflows/tree/main/tools)**

---

## 🖥️ More Projects

<details>
<summary><b>Desktop Applications & Browser Tools</b></summary>

### Free Cluely - Invisible AI Assistant
**Electron + React + TypeScript** | **Cross-Platform**

Translucent desktop app for real-time AI assistance during meetingsinterviews
- **Dual AI Modes**: Cloud (Gemini 2.5) or Local (Ollama)
- **Screenshot Analysis**: Smart content analysis with vision models
- **Global Hotkeys**: System-wide shortcuts for instant access
- **Privacy-First**: Auto-delete screenshots, local processing option

**Tech**: Electron, React, Gemini API, Ollama, FFmpeg
**[View on GitHub](https://github.com/AnsKM/free_cluely)** | **[Download](https://github.com/AnsKM/free_cluely/releases)**

---

### Memory Agent MCP Server
**FastAPI + Qdrant + MCP Protocol** | **AI Infrastructure**

Persistent memory system for Claude Code with semantic search
- **Sub-100ms retrieval** via vector embeddings (Voyage AI)
- **Project isolation** with separate memory stores
- **Smart ranking**: Relevance + recency + importance
- **Cost-effective**: ~$12/month VPS hosting

**Tech**: Python, FastAPI, Qdrant, Voyage AI, MCP
**[View on GitHub](https://github.com/AnsKM/memory-agent)**

---

### AI Form Filler - Chrome Extension
**JavaScript + Chrome Extension API** | **Shadow DOM**

One-click job application auto-fill with intelligent field detection
- **German + English** field name recognition
- **30+ field types**: Personal, professional, education, job-specific
- **Domain filtering**: Job site detection and smart activation
- **Privacy-focused**: All data stored locally

**Tech**: Chrome Manifest v3, Shadow DOM, content scripts
**Status**: Production-ready

</details>

<details>
<summary><b>Enterprise & SaaS Projects</b></summary>

### Zeit Erfassung System
**Node.js + React + PostgreSQL** | **100+ Users**

Enterprise time-tracking system with AI-powered features
- **40% efficiency improvement** in time management
- **DORA-compliant** architecture for regulated environments
- **German labor law** compliance (Arbeitszeitgesetz)
- **Redis caching** for performance at scale

**Tech**: Node.js, Express, React 18, TypeScript, PostgreSQL 16, Redis, Docker

---

### Cold Email AI System
**LangGraph + Gemini + Apify** | **B2B SaaS**

Multi-agent automation for deeply-personalized outreach
- **LangGraph orchestration** for agent workflows
- **Apify integration** for LinkedIn/web scraping
- **5+ active clients** with recurring revenue
- **MCP tool integration** for campaign state management

**Tech**: Python, LangGraph, Gemini API, Apify, MCP

---

### Time Tracker (PentaSoft)
**React + Node.js + PostgreSQL** | **Enterprise**

Employee time tracking for 100+ employees
- **Two-layer timesheet** system (daily + weekly)
- **Dashboard & reporting** with export capabilities
- **German business hours** compliance

**Tech**: React, Node.js, PostgreSQL

</details>

<details>
<summary><b>Tools & Utilities</b></summary>

### Resume/Cover Letter Generation
**Python + WeasyPrint + BeautifulSoup**

Professional German-style document generation from markdown
- **DIN 5008 compliance** for business letters
- **Photo processing** for German CV format
- **Structure validation** with age-based bullet limits
- **n8n workflow integration** with Gemini 2.0 Flash

---

### YouTube Channel Transcript Downloader
**Python + yt-dlp + YouTube API**

Bulk transcript download for entire YouTube channels
- **Smart error handling** with yt-dlp fallback
- **Multi-language** and format support (TXT/JSON)
- **Resume capability** (skip existing transcripts)
- **Organized storage** with metadata tracking

---

### Job Description Extractor
**Chrome Extension + Content Scripts**

Automatically extract and structure job posting data
- **LinkedIn/Indeed** scraping
- **Google Sheets** integration
- **Structured export** (JSON, CSV)

</details>

---

## 📊 GitHub Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=AnsKM&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub Stats" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=AnsKM&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>

### Highlights
- 🔨 **14+ Active Repositories** (public + private)
- ⚡ **20,000+ Lines** of production Rust/TypeScript in Interview Assistant
- 🌟 **6 Production Systems** deployed and maintained
- 🤝 **Open Source**: MCP servers, desktop apps, automation tools

---

<details>
<summary><b>🗺️ Technology-to-Project Mapping</b></summary>

Quick reference for recruiters scanning for specific technologies:

| Technology | Primary Projects | Business Impact |
|------------|------------------|-----------------|
| **Rust** | Interview Assistant, Whisper-Flow | Real-time audio processing, system programming |
| **Python** | Memory Agent, Claude Workflows, AI Job Hunter | AI/ML pipelines, automation, web scraping |
| **TypeScript** | Interview Assistant, Free Cluely, Whisper-Flow | Desktop apps, React frontends, type safety |
| **Tauri** | Interview Assistant, Whisper-Flow | Cross-platform desktop with native performance |
| **LLM APIs** | All AI projects | Production AI integrations across 6+ systems |
| **Voice AI** | Interview Assistant, Whisper-Flow | 100+ hours processed, <300ms latency |
| **Vector DBs** | Memory Agent, RAG systems | Sub-100ms semantic search, context retrieval |
| **FastAPI** | Memory Agent, AI APIs | High-performance Python backends |
| **React** | All desktop apps, Zeit Erfassung | Modern UI with hooks, state management |
| **n8n** | Resume tailor, automation workflows | No-code integration, business automation |

</details>

---

## 💼 Open to Opportunities

I'm actively seeking **AI Engineer**, **Full-Stack Developer**, or **Backend Engineer** roles in **Munich, Germany** or remote within the EU.

### What I Bring
- ✅ **Production AI experience**: Built 5+ systems serving 100+ users with measurable ROI
- ✅ **Systems programming**: Real-time audio processing, desktop apps, performance optimization
- ✅ **Full-stack capabilities**: React/TypeScript frontends, Python/Rust backends, vector DBs
- ✅ **Business impact focus**: 40% efficiency gains, <$1 per session costs, scalable architectures
- ✅ **German market fit**: C1 fluency, regulatory awareness (DORA, GDPR), DACH experience

### Let's Connect
- 📧 **Email**: ansmohal@gmail.com
- 💼 **LinkedIn**: [linkedin.com/in/anskhalid](https://linkedin.com/in/anskhalid)
- 🌐 **Location**: Munich, Germany
- 🗣️ **Languages**: German (C1 CEFR), English (Fluent), Urdu/Hindi (Native)

**Interested in**: AI/ML Engineering, Technical Leadership, Full-Stack Development with AI integration

---

*"Building AI systems that deliver business value while maintaining trust—especially in environments where compliance isn't optional."*
