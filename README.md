# Hi, I'm Deepesh 👋

**Senior Product Manager** building AI + data products that ship, measure, and hold up in production.

7 years across **B2B · B2C · D2C · B2B2C** — marketplaces, data platforms, and internal tools. I turn messy, ambiguous problem spaces into crisp product bets with success metrics, then prototype the fastest path to *"does this work?"* before scaling.

**Core focus:** agentic AI systems · multi-agent orchestration · marketplace discovery · real-estate intelligence · evidence-grounded LLM systems (with evals) · hybrid vision + CV estimation with guardrails · recommendation engines · geo/data analytics · pricing engines · consumer pain intelligence · SEO/AEO content platforms

---

## 🗂️ What You'll Find Here

A mix of:
- **Live products** — fully deployed, production-running platforms with real users and real infrastructure
- **Agentic AI systems** — multi-agent pipelines, orchestrated workflows, safety governance, and autonomous task execution
- **Production-minded prototypes** — projects I'd confidently harden and plug into a real system
- **AI/ML systems** — LLM workflows, recommender stacks, applied ML/CV, and evaluation tooling
- **Real estate intelligence** — pricing engines, pain point research, geo analytics, master-plan vision, and content systems purpose-built for the Indian property market
- **POCs & sandboxes** — quick experiments to validate hypotheses before engineering investment

Most repos start from a **real product problem** — not a tutorial.

---

## 🛠️ Tech I Use

**Backend (APIs + services)**
FastAPI · Pydantic v2 · async patterns · dependency injection · structured error handling · request/response contracts · pagination · idempotency · service-first design · SQLAlchemy 2.x · Alembic migrations

**Data stores**
Postgres + pgvector (embeddings, similarity search, hybrid retrieval) · MongoDB · SQLite (local-first prototypes, snapshot-driven pipelines) · Redis (session cache, broker, Celery backend) · DuckDB (local-first analytics)

**Retrieval & search**
Elasticsearch (BM25, fuzziness, suggest, resolve/disambiguate) · lexical + semantic retrieval · hybrid strategies · chunking · reranking · thresholding + refusal conditions · pgvector cosine similarity · Fuse.js fuzzy matching

**Agentic AI systems**
LangGraph multi-agent orchestration · agent role specialisation · inter-agent handoffs · safety governance layers · crisis detection pipelines · policy centers · PII masking · audit logging · human-in-the-loop oversight · memory systems (short-term + long-term) · checkpoint approval gates · pipeline stage orchestration

**LLM systems (grounded + reliable)**
RAG with evidence snippets · citation-first answers · NLI-style citation verification · structured outputs (JSON schemas) · prompt versioning · guardrails (hallucination control, refusal flows) · eval harnesses (offline checks + spot QA) · "no-claim-without-evidence" pipelines · multi-source intelligence pipelines · claim extraction + YMYL safety layers · Claude · OpenAI · Gemini

**Vision & computer vision**
Vision-language models for document and master-plan reasoning (Gemini, OpenAI) · OpenCV segmentation (HSV masks, overlays) · OpenCLIP zero-shot classification · PyTorch/timm CNNs · Grad-CAM explainability · structured extraction from images and PDFs · confidence-capped range estimation

**SEO/AEO content systems**
Programmatic content pipelines · keyword cluster agents · SEO brief generation · FAQ/snippet optimisation · JSON-LD schema injection (Article, FAQ, Breadcrumb, NewsArticle) · canonical tags + OG metadata · XML sitemap generation · internal linking engines · cannibalization detection · content refresh engines · headless CMS architectures

**Analytics & CDP**
First-party event tracking (consent-gated) · anonymous identity + session management · UTM attribution · identity stitching · funnel builder (dynamic + preset templates) · cohort heatmaps · audience segment builder · user activity timelines · Google Search Console integration · DPDP Act 2023 compliance (data export, right-to-delete)

**Pricing & analytical engines**
Six-factor data-driven pricing models · forward projection with scenario analysis (bear/base/bull) · sensitivity analysis across key drivers · confidence scoring · factor contribution decomposition · multi-scenario comparison

**Web extraction & ingestion**
Playwright · httpx · PRAW (Reddit) · YouTube Data API v3 · google-play-scraper · yt-dlp · SerpAPI / DataForSEO · multi-tier scraper fallback architectures · SSE streaming · extraction pipelines · dedupe + timeline building · strict source whitelisting · HTML artifacts for auditability

**Data processing**
Pandas · feature engineering · time-decay features · rule + heuristic layers · batch pipelines (CSV → process → validate → store) · deterministic processing for repeatability

**ML toolchain (pragmatic)**
scikit-learn baselines · RandomForest tuning · CatBoost/LightGBM-style approaches · train/val splits · leakage checks · model persistence · batch + realtime inference · slice-level diagnostics

**Recommender systems**
Candidate generation (popularity · item-item similarity · collaborative filtering · KNN) · hybrid reranking · MMR diversification · learning-to-rank · feedback loops · session-aware recommendations · metrics: hit-rate@k / nDCG · pgvector-powered semantic recommendations

**Monetisation systems**
AdSense slot components · affiliate cards + comparison modules · lead capture forms · digital product catalogs · Razorpay checkout (test + live) · HMAC download token delivery · intent-aware module selection · A/B testing (intent-based vs static) · Stripe recurring billing · premium content gating

**Geo & analytics**
Mapbox GL JS · vector tiles (tippecanoe) · geospatial aggregation · choropleths with timelines · polygon/multipolygon handling · EPSG:4326 schemas · 3D models (glTF) · exports (PNG/CSV) · shareable URLs

**Frontend (when needed)**
Next.js 14 (App Router) · React · TypeScript · Vite · Tailwind CSS · shadcn/ui · Recharts · Streamlit for rapid UIs · lightweight HTML/CSS for report rendering and previews · Framer Motion

**Infra & ops (local-first → production-ready)**
Docker + docker-compose · Celery + Celery Beat · ARQ + Redis (background jobs) · APScheduler · DigitalOcean App Platform · managed Postgres + Valkey · Prometheus · Sentry · env management · background jobs/queues · logging · basic observability patterns · reproducible repo hygiene

**Testing & quality**
pytest-style tests · Playwright E2E · browser accessibility runs · contract tests for APIs (OpenAPI-first clients) · schema validation tests · golden files for deterministic generation · regression checks for prompt changes

---

## 📌 Best Walkthrough Repos

### 🚀 Live Products

> Fully deployed, production-running platforms — not prototypes. Real infrastructure, real users, real traffic.

| Product | What It Is |
|---------|------------|
| [**trekyatra**](https://github.com/deepeshgupta12/trekyatra) · [🌐 trekyatra.co.in](https://www.trekyatra.co.in) | **AI-powered trekking content platform.** Discovers high-opportunity trek topics via trend + keyword agents, generates SEO/AEO-optimised long-form guides through a 12-agent LangGraph pipeline, publishes through a custom headless CMS with human approval gates, and monetises via AdSense, affiliate cards, lead forms, Razorpay digital products, and Stripe subscriptions. Full CDP analytics layer (funnel builder, cohort heatmaps, segment builder, DPDP compliance), operator marketplace, trip planning wizard, multilingual content (Hindi), and 581 backend tests. Deployed on DigitalOcean BLR1. Next.js 14 · FastAPI · PostgreSQL + pgvector · Redis · Celery · LangGraph · Claude. |

---

### 🤖 Agentic AI — Multi-Agent Systems & Orchestration

> These are my flagship **Agentic AI** products: production-grade platforms where autonomous agents collaborate across pipelines, enforce governance policies, and produce real artifacts — not just chat responses. Built with **LangGraph**, **FastAPI**, and enterprise-grade safety + audit layers.

| Repo | What It Is |
|------|------------|
| [**pm-agent-os**](https://github.com/deepeshgupta12/pm-agent-os) | Full-stack agentic platform where 16 specialised AI agents write product documents grounded in your team's actual evidence — PRDs, strategy memos, problem briefs, launch plans, and more. Agents are chained into multi-step pipelines with a review + approval workflow before publishing. A Policy Center enforces governance on what knowledge sources agents can use, with PII masking and an immutable audit log of every decision the system makes. FastAPI · PostgreSQL + pgvector · React 19 · OpenAI. |
| [**AI-Mental-Wellbeing-Copilot-with-Safety-Governed-Multi-Agent-Architecture**](https://github.com/deepeshgupta12/AI-Mental-Wellbeing-Copilot-with-Safety-Governed-Multi-Agent-Architecture) | Production-grade AI mental health support platform built on a **27-agent orchestration pipeline** with safety-first design, enterprise governance, and personalized memory systems. Combines LangGraph-driven agent workflows, a FastAPI async backend, and a modern Next.js React frontend to deliver empathetic, context-aware mental wellbeing assistance with robust crisis detection and human oversight. |
| [**wayfarer-ai**](https://github.com/deepeshgupta12/wayfarer-ai) | AI-powered travel planning and destination intelligence platform. Agentic orchestration helps travellers research destinations, build personalised itineraries, compare cities, and monitor active trips in real time. Every planning decision, enrichment step, and notification is driven by LangGraph agents on a FastAPI backend, streamed to a React + Vite frontend. |
| [**journeylab**](https://github.com/deepeshgupta12/journeylab) | **A trip digital twin for comparing feasible futures before and during travel.** Turns a traveller's intent and constraints into several evidence-backed, feasible trip scenarios, makes the trade-offs visible on a synchronised map and timeline, and maintains the chosen scenario as a live companion. Deterministic solvers own feasibility; the model explains and parses language. OpenAPI-first contracts, pnpm + uv monorepo, 26-step verify gate with real-browser accessibility runs. |
| [**agentic-rag-verified-citations**](https://github.com/deepeshgupta12/agentic-rag-verified-citations) | Agentic RAG that verifies every citation against source text before answering, and abstains when the evidence does not hold. Self-correcting retrieval loop, deterministic citation grounding, NLI entailment checks, prompt-injection defence, 471 tests. |
| [**agentic_ai_review_model**](https://github.com/deepeshgupta12/agentic_ai_review_model) | Agentic project intelligence: collects real people's reviews of residential projects from portals, Reddit, Quora, YouTube and Instagram, tags them by category, puts every one before a moderator, and publishes approved, evidence-linked review lists. FastAPI, LangGraph, MongoDB, Next.js, Claude. |

---

### 🏠 Real Estate Intelligence (Pricing · Pain · Vision · Geo)

> A cluster of full-stack products built around real problems in the Indian property market — from pricing fair value, to reading master plans, to surfacing what buyers and renters actually complain about.

| Repo | What It Is |
|------|------------|
| [**master-plan-intelligence**](https://github.com/deepeshgupta12/master-plan-intelligence) | **Reads a real-estate master plan image and turns it into structured, auditable intelligence.** A spatial entity map (towers and wings, amenities, legend markers, roads, water, open space) reconciled against the printed legend; executive dashboards for land use, amenity mix, spatial access and architectural block plans; key-value site metrics with density benchmarks when project records are supplied; and range-based Green Area % / Open Area % estimates with confidence reasons and hard guardrails (green ≤ open, no "official" language without a source). Every analysis is checked by backend QA agents (reviewer, fixer, teacher with a self-tuning playbook), and an offline engineer agent turns their backlog into pull requests gated by unit tests and a five-plan regression. Typed output contract, identical across plans. FastAPI · Gemini 3.5 Flash · OpenCV · React + Vite. |
| [**Pan-India-Price-Projection**](https://github.com/deepeshgupta12/Pan-India-Price-Projection) | Full-stack analytical workspace for estimating current fair asking prices and 1Y/3Y/5Y forward price projections for primary-market residential projects across India. Built on a six-factor data-driven pricing engine (specification quality, supply-demand, connectivity, developer premium, macro conditions, regulatory risk), multi-scenario analysis (bear/base/bull/custom), sensitivity sweeps across six key drivers, save/compare/export flows, and a 49-test unit suite. FastAPI backend + Next.js frontend, fully config-driven with no hardcoded lookup tables. |
| [**real-estate-pain-intelligence**](https://github.com/deepeshgupta12/real-estate-pain-intelligence) | AI-powered platform that scrapes public sources (Reddit, YouTube, App Stores, X/Twitter, review sites) for any Indian real estate brand, then runs a multi-agent LLM pipeline — extraction → taxonomy/clustering → root-cause hypothesis → competitor benchmarking → prioritization → action recommendations. Surfaces everything in a streaming console UI with semantic search (pgvector), human review queue, Notion sync, and CSV/JSON/PDF export. Handles Hinglish and Hindi app reviews. FastAPI + PostgreSQL + pgvector + Next.js 15 + ARQ background workers. |
| [**geo-map-analytics**](https://github.com/deepeshgupta12/geo-map-analytics) | Map-first real-estate analytics for Mumbai: zoom-driven drill-down from micromarkets to localities to projects, monthly choropleths with a smooth timeline, project heatmap, 3D project models (glTF on Mapbox Standard), pinned A/B comparisons, exports (PNG + CSV), and shareable views. Mapbox GL JS + Next.js + TypeScript. |
| [**sqy-mumbai-poc**](https://github.com/deepeshgupta12/sqy-mumbai-poc) | The backend-free POC that preceded geo-map-analytics: GeoJSON validation, metric CSV → JSON preprocessing, tippecanoe vector tiles, and a locality choropleth with metric / month / asset / BHK filters and click-through summary stats. |
| [**Automated-Locality-Report-Engine**](https://github.com/deepeshgupta12/Automated-Locality-Report-Engine) | Generates full locality reports (data → charts → LLM narratives → PDF + React UI) from two JSON feeds (Locality + Property Rates). Grounded narratives via OpenAI Structured Outputs, ReportLab PDF, repeatable for any locality without code changes — swap inputs + polygon/map asset. |
| [**ocr-payment-plan-pipeline**](https://github.com/deepeshgupta12/ocr-payment-plan-pipeline) | Turns developer payment plans and price sheets — images or PDFs in any layout — into validated structured JSON and publish-ready SEO/AEO content for project detail pages. Vision-model extraction with strict Structured Outputs (not OCR), verbatim extraction + deterministic arithmetic validation, and auto-publish vs human-review gating. Payment-plan errors are a trust issue, so numbers never come from the model alone. |

---

### 🔍 Search, Discovery & Recommendation

> Discovery surfaces for marketplaces: understanding what the user meant, routing them to the right destination, and deciding what they should see next.

| Repo | What It Is |
|------|------------|
| [**realestate-search**](https://github.com/deepeshgupta12/realestate-search) | Elasticsearch-powered navigation search for a real-estate site: autocomplete grouped by entity type, typo correction, intent resolve (redirect vs SERP vs disambiguate for same-name localities), grouped SERP with did-you-mean, zero-state trending, and search/click event logging for future ranking. FastAPI + Next.js. |
| [**movie-recommendation-mvp**](https://github.com/deepeshgupta12/movie-recommendation-mvp) | Local-first, production-shaped recommender that evolves from classic baselines to a Netflix-style hybrid stack: multiple candidate generators, blended retrieval priors, learning-to-rank, "why this" explanations, an online feedback loop, and a session-aware, diversity-aware V4 with posters and live interactions. FastAPI serving + Streamlit UI. |
| [**music-recsys**](https://github.com/deepeshgupta12/music-recsys) | Local-first music recommender over a Spotify-style feature catalog: KNN similar tracks, hybrid reranking (similarity, momentum, popularity, freshness), MMR-style playlist generation, and session-driven "For You" recommendations behind a FastAPI API with a test-first workflow. |
| [**sy-project-comparability-engine**](https://github.com/deepeshgupta12/sy-project-comparability-engine) | Client-side engine that surfaces the 3 most comparable residential projects to any subject project using TF-IDF keyword vectors plus z-score numerical similarity, with Pure Match, Business Priority and Recommended views. Drag-and-drop XLSX input, plain-English tooltips on every label, zero backend. |
| [**squareyards-rec-engine**](https://github.com/deepeshgupta12/squareyards-rec-engine) | Interactive content-based recommender for real-estate projects: weighted similarity over price, area, BHK, developer grade, status and distance, status-priority and focus boosts, adaptive candidate filtering, and a soft distance penalty. Single-file Python CLI over a CSV — the sandbox that informed later discovery work. |

---

### 🧠 Computer Vision · Applied ML · Learning Tools

| Repo | What It Is |
|------|------------|
| [**realestate-image-classifier**](https://github.com/deepeshgupta12/realestate-image-classifier) | FastAPI service that classifies real-estate photos (kitchen, bedroom, clubhouse, master plan, …) with zero-shot OpenCLIP plus an optional trained linear head, and auto-selects the best listing thumbnail using sharpness, exposure, saliency, duplicate penalties and configurable bans (never a bathroom). YAML-driven taxonomy and rules, runs locally on Apple Silicon. |
| [**brain-tumor-ai**](https://github.com/deepeshgupta12/brain-tumor-ai) | FastAPI service + PyTorch/timm CNN that classifies brain MRI scans into no_tumor, glioma, meningioma and pituitary, with Grad-CAM heatmaps, a `/metrics` batch evaluation endpoint, dataset builder, test-time augmentation and an Apple Silicon training recipe. Research and triage only — not a medical device. |
| [**hotel-cancellation-model**](https://github.com/deepeshgupta12/hotel-cancellation-model) | Production-minded ML system predicting hotel booking cancellation probability with Low / Medium / High risk buckets: multi-source dataset unification, feature engineering, tuned RandomForest, batch scoring, a FastAPI raw-booking → features → prediction API, prediction logging and slice-level diagnostics. |
| [**used-car-price-prediction**](https://github.com/deepeshgupta12/used-car-price-prediction) | Local-first, Dockerised used-car price prediction service for India (IN) + United States (US) with a cleaning pipeline for messy listings, persisted artifacts, FastAPI single + batch endpoints, readiness/liveness probes, CI gates and tests. |
| [**smart-kitchen-os**](https://github.com/deepeshgupta12/smart-kitchen-os) | AI kitchen operating system: GPT-4o-mini recipe extraction with DALL-E imagery, an autonomous pantry that deducts stock when meals are completed, BMR-based nutrition goals with consumption tracking, and unified shopping lists. Python backend, web frontend, Docker Compose. |
| [**youtube-learning-copilot**](https://github.com/deepeshgupta12/youtube-learning-copilot) | Transcript-first study companion: turns any YouTube video into a learning pack with searchable timestamped chunks, chapter flows, summary, flashcards, quizzes, progress tracking, and citation-backed Q&A. |

---

### 💰 Fintech & Decision Support

| Repo | What It Is |
|------|------------|
| [**Saakshya**](https://github.com/deepeshgupta12/Saakshya) | *Saakshya* (Sanskrit for **evidence**): spec-first, AI-assisted equity research, market scanner and portfolio-intelligence platform for NSE/BSE. Deterministic signals that the AI layer explains but never invents — no made-up prices, targets or returns. Positioned as research and decision support, not advice; launches in a pure-analytics mode with recommendation features gated behind SEBI RA registration. Currently a complete 30-document product + engineering specification with a local-first build plan (DuckDB, Claude Haiku). |
| [**personal-finance-copilot**](https://github.com/deepeshgupta12/personal-finance-copilot) | Local-first AI-assisted personal finance dashboard for young professionals: ingests mock bank/UPI/credit card data, auto-categorises India-friendly spending, detects bad patterns, and writes a plain-language monthly money story + next actions. FastAPI, SQLite, Pandas, scikit-learn, Jinja2, OpenAI API. |

---

### ✍️ LLM-Powered Content & Intelligence (Guardrailed Generation)

| Repo | What It Is |
|------|------------|
| [**seo-content-generation-system**](https://github.com/deepeshgupta12/seo-content-generation-system) | Programmatic SEO content engine for real-estate resale listing pages. Ingests raw datacenter JSON exports, performs deep keyword research via DataForSEO, and uses OpenAI to produce AEO-optimised drafts with deterministic tables, FAQ blocks and JSON-LD — validated factually against source data and exported to JSON / Markdown / DOCX / HTML through a React review workbench with section regeneration and version restore. |
| [**stalled-project-news**](https://github.com/deepeshgupta12/stalled-project-news) | Search-first pipeline generating evidence-backed stalled/delayed project updates (JSON + HTML): SerpAPI retrieval, strict source whitelisting, snippet-level evidence mapping, dedupe/timeline generation, citation coverage verification. Every claim maps to stored evidence or the output says "insufficient evidence". |
| [**sy-pdp-content-llm**](https://github.com/deepeshgupta12/sy-pdp-content-llm) | SEO + AEO long-form content for real-estate project detail pages: ingests per-project datacenter JSON, grounds facts with SERP evidence, learns tone from human-written examples, and outputs structured JSON plus styled HTML with controllable tone at scale. |
| [**sqy-locality-llm**](https://github.com/deepeshgupta12/sqy-locality-llm) | Facts-only locality overview generator: plain-language, non-repetitive SEO/AEO HTML written strictly from a FACTS JSON (no invented numbers, abbreviations expanded on first use), indices explained once, merged market section, optional SERP enrichment for qualitative lines, normalised snapshots for audit. |
| [**review-summary-engine**](https://github.com/deepeshgupta12/review-summary-engine) | Review intelligence pipeline: ingests a CSV of thousands of project reviews and produces (1) one grounded summary per project and (2) exactly three UI tags per review (persona + USPs). Built for deterministic outputs, batching/resume safety, and scale-friendly processing. |
| [**squareyards-review-engine**](https://github.com/deepeshgupta12/squareyards-review-engine) | Trust-layer pipeline for project reviews: normalises Google reviews, scores sentiment with GPT, clusters key phrases into UI tags with embeddings, and writes a quote-backed project summary. YAML-configured. |
| [**area-converter-ai**](https://github.com/deepeshgupta12/area-converter-ai) | Content generation toolkit for area-unit converter experiences: unique, India-focused landing + unit-pair pages (sq ft → sq m, bigha → acre, …) with multi-persona FAQs, Mongo-ready JSON, HTML previews, strict length validation, and batch pipelines (CSV → generation → validation/regeneration → DB payloads). |

---

### 🧰 Data Extraction & Sandboxes

| Repo | What It Is |
|------|------------|
| [**one-mg-scraper**](https://github.com/deepeshgupta12/one-mg-scraper) | Playwright scraper for 1mg drug detail pages producing a clean, normalised medicines dataset (name, salt composition, uses, side effects, fact box, substitutes, patient FAQs) as JSONL + CSV, with manual mode for challenges and respectful rate limits. |

---

## ⚙️ How I Work

- Turn vague asks into sharp product problems + success metrics
- Partner deeply with engineering/design/data (high technical fluency)
- Prefer **evidence over vibes**: evaluation, guardrails, measurable outcomes
- Use AI + automation as leverage — not decoration
- Ship to production, not just to demos: real infra, real monitoring, real edge cases handled
- Write to think — documenting architecture, agent contracts, and product bets as I build

---

## 🔭 Currently Exploring

**Evaluation-first LLM product development** — offline test sets, rubric-based scoring, citation coverage checks, refusal thresholds, and regression testing when prompts/models change.

**Hybrid vision estimation with honest uncertainty** — vision-language reasoning plus classical CV measurement, range-based outputs, confidence caps tied to evidence quality, and copy guardrails so the UI never over-claims.

**Better retrieval over "more tokens"** — chunking strategies, query rewriting, hybrid retrieval (lexical + vector), reranking, and confidence gating.

**Evidence-backed "news/intelligence" pipelines** — extraction → claim detection → dedupe → timelines → human-readable narratives + auditable artifacts.

**Pricing engines with real analytical depth** — six-factor data-driven models, scenario-based forward projections, sensitivity analysis, confidence scoring, and no-hardcode design where all parameters are DB-injected at runtime.

**Consumer pain intelligence at scale** — multi-source scraping, multi-agent LLM pipelines, taxonomy clustering, root-cause hypothesis generation, and human-in-the-loop review queues.

**Simulation over single answers** — trip digital twins, deterministic feasibility solvers with LLM explanation layers, and comparing feasible futures instead of returning one itinerary.

**Personalization loops that actually learn** — feedback-driven recommenders, session intent inference, segment-driven widgets, and "next best action" logic.

**Local-first product engineering** — reproducible pipelines, persisted artifacts, Docker-first setup, and clean upgrade paths to production.

**Geo + decision intelligence at scale** — multi-layer geo rendering, metric overlays, performant choropleths, and config-over-code onboarding for new cities/datasets.

**Content systems with control** — template-driven generation, SEO/AEO hygiene, structured outputs, strict validation so content is predictable and debuggable, and headless CMS architectures that scale programmatically.

**Agentic AI architectures** — LangGraph-driven multi-agent pipelines, role-specialised agents, inter-agent communication protocols, safety governance, crisis detection, human oversight loops, and policy-enforced artifact generation at scale.

**Trust layers in marketplaces** — review intelligence, credibility signals, persona-fit tagging, and deterministic-enough summarization to ship.

**First-party analytics and CDP systems** — event taxonomy governance, funnel/cohort/segment infrastructure, identity stitching, and DPDP-compliant data platforms built from scratch.

---

## 🤝 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/deepeshkumargupta)
[![Medium](https://img.shields.io/badge/Medium-000000?style=flat&logo=medium&logoColor=white)](https://medium.com/@guyshazam12)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:deepeshkumargupta9891@gmail.com)
