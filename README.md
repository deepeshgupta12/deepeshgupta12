# Hi, I'm Deepesh 👋

**Senior Product Manager** building AI + data products that ship, measure, and hold up in production.

6+ years across **B2B · B2C · D2C · B2B2C** — marketplaces, data platforms, and internal tools. I turn messy, ambiguous problem spaces into crisp product bets with success metrics, then prototype the fastest path to *"does this work?"* before scaling.

**Core focus:** agentic AI systems · multi-agent orchestration · marketplace discovery · real-estate intelligence · evidence-grounded LLM systems (with evals) · recommendation engines · geo/data analytics · pricing engines · consumer pain intelligence

---

## 🗂️ What You'll Find Here

A mix of:
- **Agentic AI systems** — multi-agent pipelines, orchestrated workflows, safety governance, and autonomous task execution
- **Production-minded prototypes** — projects I'd confidently harden and plug into a real system
- **AI/ML systems** — LLM workflows, recommender stacks, applied ML/CV, and evaluation tooling
- **Real estate intelligence** — pricing engines, pain point research, geo analytics, and content systems purpose-built for the Indian property market
- **POCs & sandboxes** — quick experiments to validate hypotheses before engineering investment

Most repos start from a **real product problem** — not a tutorial.

---

## 🛠️ Tech I Use

**Backend (APIs + services)**
FastAPI · Pydantic v2 · async patterns · dependency injection · structured error handling · request/response contracts · pagination · idempotency · service-first design

**Data stores**
Postgres + pgvector (embeddings, similarity search, hybrid retrieval) · MongoDB · SQLite (local-first prototypes, snapshot-driven pipelines) · Alembic migrations

**Retrieval & search**
Elastic-style search patterns (filters, faceting, ranking) · lexical + semantic retrieval · hybrid strategies · chunking · reranking · thresholding + refusal conditions · pgvector cosine similarity

**Agentic AI systems**
LangGraph multi-agent orchestration · agent role specialisation · inter-agent handoffs · safety governance layers · crisis detection pipelines · policy centers · PII masking · audit logging · human-in-the-loop oversight · memory systems (short-term + long-term)

**LLM systems (grounded + reliable)**
RAG with evidence snippets · citation-first answers · structured outputs (JSON schemas) · prompt versioning · guardrails (hallucination control, refusal flows) · eval harnesses (offline checks + spot QA) · "no-claim-without-evidence" pipelines · multi-source intelligence pipelines

**Pricing & analytical engines**
Six-factor data-driven pricing models · forward projection with scenario analysis (bear/base/bull) · sensitivity analysis across key drivers · confidence scoring · factor contribution decomposition · multi-scenario comparison

**Web extraction & ingestion**
Playwright · httpx · PRAW (Reddit) · YouTube Data API v3 · google-play-scraper · yt-dlp · multi-tier scraper fallback architectures · SSE streaming · extraction pipelines · dedupe + timeline building · strict source whitelisting · HTML artifacts for auditability

**Data processing**
Pandas · feature engineering · time-decay features · rule + heuristic layers · batch pipelines (CSV → process → validate → store) · deterministic processing for repeatability

**ML toolchain (pragmatic)**
scikit-learn baselines · CatBoost/LightGBM-style approaches · train/val splits · leakage checks · model persistence · batch + realtime inference

**Recommender systems**
Candidate generation (popularity · item-item similarity · collaborative filtering) · ranking models · feedback loops · metrics: hit-rate@k / nDCG

**Geo & analytics**
Mapbox GL JS · vector tiles · geospatial aggregation · choropleths · polygon/multipolygon handling · EPSG:4326 schemas · exports (PNG/CSV) · shareable URLs

**Frontend (when needed)**
Next.js/React · TypeScript · Tailwind CSS · Recharts · Streamlit for rapid UIs · lightweight HTML/CSS for report rendering and previews

**Infra & ops (local-first → production-ready)**
Docker + docker-compose · ARQ + Redis (background jobs) · Prometheus · Sentry · Alembic · env management · background jobs/queues · logging · basic observability patterns · reproducible repo hygiene

**Testing & quality**
pytest-style tests · contract tests for APIs · schema validation tests · golden files for deterministic generation · regression checks for prompt changes

---

## 📌 Best Walkthrough Repos

### 🧠 Computer Vision · Applied ML · Data Science · LLM/RAG Fundamentals

| Repo | What It Is |
|------|------------|
| [**movie-recommendation-mvp**](https://github.com/deepeshgupta12/movie-recommendation-mvp) | Local-first, production-style recommender: hybrid candidate retrieval (popularity + item-item + ALS + genre signals), time-decay-aware feature store, trained ranker, FastAPI serving, Streamlit UI with posters + feedback-driven personalization. End-to-end: discovery → ranking → iteration. |
| [**smart-kitchen-os**](https://github.com/deepeshgupta12/smart-kitchen-os) | Culinary OS combining inventory + health intelligence + automated meal planning: recipe extraction to structured data, pantry deduction logic, TDEE/macros profiling, FastAPI + Postgres backend, Next.js frontend. |
| [**realestate-image-classifier**](https://github.com/deepeshgupta12/realestate-image-classifier) | Image classification pipeline to categorize/optimize thumbnails (rooms, amenities, visuals) for better engagement in visual catalogs. Includes dataset strategy, labeling approach, training, and inference patterns. |
| [**brain-tumor-ai**](https://github.com/deepeshgupta12/brain-tumor-ai) | Applied CV project on medical imaging + tumor detection to deepen CV workflows, interpretation patterns, and responsible handling for sensitive domains. |
| [**hotel-booking-cancellation-model**](https://github.com/deepeshgupta12/hotel-booking-cancellation-model) | End-to-end ML pipeline + FastAPI service predicting booking cancellations, exposing risk buckets, with batch + real-time scoring. |
| [**youtube-learning-copilot**](https://github.com/deepeshgupta12/youtube-learning-copilot) | Transcript-first study companion: searchable chunks, chapter flows, flashcards/quizzes, progress tracking, and citation-backed Q&A. |
| [**used-car-price-prediction**](https://github.com/deepeshgupta12/used-car-price-prediction) | Local-first, Docker-friendly Used Car Price Prediction service for India (IN) + United States (US) with clean preprocessing, persisted artifacts, and FastAPI endpoints (single + batch). |

---

### 🤖 Agentic AI — Multi-Agent Systems & Orchestration

> These are my flagship **Agentic AI** products: production-grade platforms where autonomous agents collaborate across pipelines, enforce governance policies, and produce real artifacts — not just chat responses. Built with **LangGraph**, **FastAPI**, and enterprise-grade safety + audit layers.

| Repo | What It Is |
|------|------------|
| [**pm-agent-os**](https://github.com/deepeshgupta12/pm-agent-os) | Full-stack agentic platform where specialised AI agents write product documents grounded in your team's actual evidence — PRDs, strategy memos, problem briefs, launch plans, and more. Agents are chained into multi-step pipelines with a review + approval workflow before publishing. A Policy Center enforces governance on what knowledge sources agents can use, with PII masking and an immutable audit log of every decision the system makes. |
| [**AI-Mental-Wellbeing-Copilot-with-Safety-Governed-Multi-Agent-Architecture**](https://github.com/deepeshgupta12/AI-Mental-Wellbeing-Copilot-with-Safety-Governed-Multi-Agent-Architecture) | Production-grade AI mental health support platform built on a **27-agent orchestration pipeline** with safety-first design, enterprise governance, and personalized memory systems. Combines LangGraph-driven agent workflows, a FastAPI async backend, and a modern Next.js React frontend to deliver empathetic, context-aware mental wellbeing assistance with robust crisis detection and human oversight. |
| [**wayfarer-ai**](https://github.com/deepeshgupta12/wayfarer-ai) | AI-powered travel planning and destination intelligence platform — Wayfarer is a full-stack application that uses agentic AI orchestration to help travellers research destinations, build personalised itineraries, compare cities, and monitor their active trips in real time. Every planning decision, enrichment step, and notification is driven by LangGraph agents running on a FastAPI backend, with a React frontend that consumes those results. |

---

### 🏠 Real Estate Intelligence (Pricing · Pain · Analytics)

> A cluster of full-stack products built around real problems in the Indian property market — from pricing fair value to surfacing what buyers and renters actually complain about.

| Repo | What It Is |
|------|------------|
| [**Pan-India-Price-Projection**](https://github.com/deepeshgupta12/Pan-India-Price-Projection) | Full-stack analytical workspace for estimating current fair asking prices and 1Y/3Y/5Y forward price projections for primary-market residential projects across India. Built on a six-factor data-driven pricing engine (specification quality, supply-demand, connectivity, developer premium, macro conditions, regulatory risk), multi-scenario analysis (bear/base/bull/custom), sensitivity sweeps across six key drivers, save/compare/export flows, and a 49-test unit suite. FastAPI backend + Next.js 16 frontend, Postgres-ready SQLite, fully config-driven with no hardcoded lookup tables. |
| [**real-estate-pain-intelligence**](https://github.com/deepeshgupta12/real-estate-pain-intelligence) | AI-powered platform that scrapes public sources (Reddit, YouTube, App Stores, X/Twitter, review sites) for any Indian real estate brand, then runs a multi-agent LLM pipeline — extraction → taxonomy/clustering → root-cause hypothesis → competitor benchmarking → prioritization → action recommendations. Surfaces everything in a streaming console UI with semantic search (pgvector), human review queue, Notion sync, and CSV/JSON/PDF export. FastAPI + PostgreSQL + pgvector + Next.js 16 + ARQ background workers. |
| [**geo-map-analytics**](https://github.com/deepeshgupta12/geo-map-analytics) | Developer-friendly geospatial analytics UI: city → micromarket → locality → roads → projects from Mapbox vector tiles, monthly metrics choropleths, pinned A/B comparisons, exports (PNG + CSV), shareable URLs. |
| [**squareyards-rec-engine**](https://github.com/deepeshgupta12/squareyards-rec-engine) | Experiments for recommendation-driven discovery: ranking signals, shortlist logic, segment-driven recs, and practical "what should the user see next?" widgets. |

---

### 🔍 AI for Discovery & Personalization (Marketplace Systems)

| Repo | What It Is |
|------|------------|
| [**personal-finance-copilot**](https://github.com/deepeshgupta12/personal-finance-copilot) | Local-first AI-assisted personal finance dashboard: ingests mock bank/UPI/credit card data, auto-categorizes spending, detects bad patterns, and generates a plain-language monthly money story + next actions. Built with FastAPI, SQLite, Pandas, scikit-learn, Jinja2, and the OpenAI API. |

---

### ✍️ LLM-Powered Content & Intelligence (Guardrailed Generation)

| Repo | What It Is |
|------|------------|
| [**sy-pdp-content-llm**](https://github.com/deepeshgupta12/sy-pdp-content-llm) | High-intent page content generation with guardrails for consistency, quality, and SEO hygiene: structured outputs, reusable templates, controllable tone at scale. |
| [**sqy-locality-llm**](https://github.com/deepeshgupta12/sqy-locality-llm) | Context-aware locality content + FAQs for real-estate decisions: grounded explanations, structured FAQ generation, locality-level narrative consistency. |
| [**squareyards-review-engine**](https://github.com/deepeshgupta12/squareyards-review-engine) | Trust-layer engine to collect, structure, and surface user feedback into decision-ready insights (themes, pros/cons, persona-fit, credibility signals). |
| [**review-summary-engine**](https://github.com/deepeshgupta12/review-summary-engine) | Review Intelligence pipeline: ingests large datasets and produces (1) project-wise summaries and (2) per-review tags (persona + USPs). Built for deterministic outputs, batching/resume, and scale-friendly processing. |
| [**stalled-project-news**](https://github.com/deepeshgupta12/stalled-project-news) | Search-first pipeline generating evidence-backed stalled/delayed project updates (JSON + HTML): strict source whitelisting, snippet-level evidence mapping, dedupe/timeline generation, citation coverage verification. Designed for zero-hallucination narratives. |
| [**area-converter-ai**](https://github.com/deepeshgupta12/area-converter-ai) | Content generation toolkit for area converter experiences: landing + child pages, Mongo-ready JSON, HTML previews, strict length validation, batch pipelines (CSV → generation → validation/regeneration → DB payloads). |
| [**seo-content-generation-system**](https://github.com/deepeshgupta12/seo-content-generation-system) | Programmatic SEO content engine for Square Yards resale listing pages. Ingests raw datacenter JSON exports, performs deep keyword research via DataForSEO, and uses OpenAI to produce publication-ready SEO drafts in multiple formats — all through a REST API with a React-based review workbench UI. |
| [**Automated-Locality-Report-Engine**](https://github.com/deepeshgupta12/Automated-Locality-Report-Engine) | Generates full locality reports (data → charts → LLM narratives → PDF + Lovable UI) from two JSON feeds (Locality + Property Rates). Repeatable for any locality without code changes — swap inputs + polygon/map asset. |

---

## ⚙️ How I Work

- Turn vague asks into sharp product problems + success metrics
- Partner deeply with engineering/design/data (high technical fluency)
- Prefer **evidence over vibes**: evaluation, guardrails, measurable outcomes
- Use AI + automation as leverage — not decoration

---

## 🔭 Currently Exploring

**Evaluation-first LLM product development** — offline test sets, rubric-based scoring, citation coverage checks, refusal thresholds, and regression testing when prompts/models change.

**Better retrieval over "more tokens"** — chunking strategies, query rewriting, hybrid retrieval (lexical + vector), reranking, and confidence gating.

**Evidence-backed "news/intelligence" pipelines** — extraction → claim detection → dedupe → timelines → human-readable narratives + auditable artifacts.

**Pricing engines with real analytical depth** — six-factor data-driven models, scenario-based forward projections, sensitivity analysis, confidence scoring, and no-hardcode design where all parameters are DB-injected at runtime.

**Consumer pain intelligence at scale** — multi-source scraping, multi-agent LLM pipelines, taxonomy clustering, root-cause hypothesis generation, and human-in-the-loop review queues.

**Personalization loops that actually learn** — feedback-driven recommenders, session intent inference, segment-driven widgets, and "next best action" logic.

**Local-first product engineering** — reproducible pipelines, persisted artifacts, Docker-first setup, and clean upgrade paths to production.

**Geo + decision intelligence at scale** — multi-layer geo rendering, metric overlays, performant choropleths, and config-over-code onboarding for new cities/datasets.

**Content systems with control** — template-driven generation, SEO hygiene, structured outputs, and strict validation so content is predictable and debuggable.

**Agentic AI architectures** — LangGraph-driven multi-agent pipelines, role-specialised agents, inter-agent communication protocols, safety governance, crisis detection, human oversight loops, and policy-enforced artifact generation at scale.

**Trust layers in marketplaces** — review intelligence, credibility signals, persona-fit tagging, and deterministic-enough summarization to ship.

---

## 🤝 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/deepeshkumargupta)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:deepeshkumargupta9891@gmail.com)
