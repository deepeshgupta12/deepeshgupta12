# Hi, I’m Deepesh 👋

Senior Product Manager building AI + data products that **ship**, **measure**, and **hold up in production**.

I’ve spent 6+ years across B2B, B2C, D2C, and B2B2C — marketplaces, data platforms, and internal tools. I enjoy turning messy, ambiguous problem spaces into crisp product bets with success metrics, then prototyping the fastest path to *“does this work?”* before scaling.

**Core focus:** marketplace discovery, real-estate intelligence, evidence-grounded LLM systems (with evals), recommendation engines, and geo/data analytics.

---

## What you’ll find here

This GitHub is a mix of:

- **Production-minded prototypes** — projects I’d confidently harden and plug into a real system  
- **AI/ML systems** — LLM workflows, recommender stacks, applied ML/CV, and evaluation tooling  
- **POCs & sandboxes** — quick experiments to validate hypotheses before engineering investment  

Most repos start from a real product problem — not a tutorial.

---

## Tech I use

- **Backend (APIs + services):** FastAPI, Pydantic (v2), async patterns, dependency injection, structured error handling, request/response contracts, pagination, idempotency, and service-first design.
- **Data stores:** Postgres + **pgvector** (embeddings, similarity search, hybrid retrieval hooks), MongoDB / SQLite (local-first prototypes, snapshot-driven pipelines).
- **Retrieval & search:** Elastic-style search patterns (filters, faceting, ranking), lexical + semantic retrieval, hybrid strategies, chunking, reranking concepts, thresholding + refusal conditions.
- **LLM systems (grounded + reliable):** RAG with evidence snippets, citation-first answers, structured outputs (JSON schemas), prompt versioning, guardrails (hallucination control, refusal flows), eval harnesses (offline checks + spot QA), and “no-claim-without-evidence” pipelines.
- **Web extraction & ingestion:** Playwright, httpx, extraction pipelines, dedupe + timeline building, strict source whitelisting, and HTML artifacts for auditability.
- **Data processing:** Pandas, feature engineering, time-decay features, rule + heuristic layers, batch pipelines (CSV → process → validate → store), deterministic processing for repeatability.
- **ML toolchain (pragmatic):** scikit-learn baselines, CatBoost/LightGBM-style approaches (where relevant), train/val splits, leakage checks, model persistence, batch + realtime inference.
- **Recommender systems:** candidate generation (popularity, item-item similarity, collaborative filtering), ranking models, feedback loops, and metrics like hit-rate@k / nDCG.
- **Geo & analytics:** Mapbox GL JS, vector tiles, geospatial aggregation, choropleths, polygon/multipolygon handling, EPSG:4326 schemas, exports (PNG/CSV), shareable URLs.
- **Frontend (when needed):** Next.js/React, Streamlit for rapid UIs, and lightweight HTML/CSS for report rendering and previews.
- **Infra & ops (local-first → production-ready):** Docker + docker-compose, env management, background jobs/queues, logging, basic observability patterns, and reproducible repo hygiene.
- **Testing & quality:** pytest-style tests, contract tests for APIs, schema validation tests, golden files for deterministic generation, and regression checks for prompt changes.

---

## Best walkthrough repos (how I think + build)

### Computer Vision, Applied ML, Data Science, LLM/RAG fundamentals

- **[movie-recommendation-mvp](https://github.com/deepeshgupta12/movie-recommendation-mvp)**  
  Local-first, production-style recommender: hybrid candidate retrieval (popularity + item-item + ALS + genre signals), time-decay-aware feature store, trained ranker, FastAPI serving, and a Streamlit UI with posters + feedback-driven personalization. End-to-end: discovery → ranking → iteration.

- **[smart-kitchen-os](https://github.com/deepeshgupta12/smart-kitchen-os)**  
  Culinary OS combining inventory + health intelligence + automated meal planning: recipe extraction to structured data, pantry deduction logic, TDEE/macros profiling, FastAPI + Postgres backend, Next.js frontend.

- **[realestate-image-classifier](https://github.com/deepeshgupta12/realestate-image-classifier)**  
  Image classification pipeline to categorize/optimize thumbnails (rooms, amenities, visuals) for better engagement in visual catalogs. Includes dataset strategy, labeling approach, training, and inference patterns.

- **[brain-tumor-ai](https://github.com/deepeshgupta12/brain-tumor-ai)**  
  Applied CV project on medical imaging + tumor detection to deepen CV workflows, interpretation patterns, and responsible handling for sensitive domains.

- **[hotel-booking-cancellation-model](https://github.com/deepeshgupta12/hotel-booking-cancellation-model)**  
  End-to-end ML pipeline + FastAPI service predicting booking cancellations, exposing risk buckets, with batch + real-time scoring.

- **[youtube-learning-copilot](https://github.com/deepeshgupta12/youtube-learning-copilot)**  
  Transcript-first study companion: searchable chunks, chapter flows, flashcards/quizzes, progress tracking, and citation-backed Q&A.

- **[used-car-price-prediction](https://github.com/deepeshgupta12/used-car-price-prediction)**  
  Local-first, Docker-friendly Used Car Price Prediction service for India (IN) + United States (US) with clean preprocessing, persisted artifacts, and FastAPI endpoints (single + batch).

---

### Agentic Product Engineering (AI Systems & Tooling)

- **[pm-agent-os](https://github.com/deepeshgupta12/pm-agent-os)**  
  PM Agent OS is a full-stack platform where specialised AI agents write product documents grounded in your team's actual evidence — PRDs, strategy memos, problem briefs, launch plans, and more. Agents can be chained into multi-step pipelines. Every artifact goes through a review and approval workflow before publishing. A Policy Center enforces governance on what knowledge sources agents can use, with PII masking and an immutable audit log of every decision the system makes.

---

### AI for Discovery & Personalization (Marketplace systems)

- **[squareyards-rec-engine](https://github.com/deepeshgupta12/squareyards-rec-engine)**  
  Experiments for recommendation-driven discovery: ranking signals, shortlist logic, segment-driven recs, and practical “what should the user see next?” widgets.

- **[personal-finance-copilot](https://github.com/deepeshgupta12/personal-finance-copilot)**  
  Local-first AI-assisted personal finance dashboard: ingests mock bank/UPI/credit card data, auto-categorizes spending, detects bad patterns, and generates a plain-language monthly money story + next actions. Built with FastAPI, SQLite, Pandas, scikit-learn, Jinja2, and the OpenAI API.

---

### Data & Geo Analytics (Decision intelligence)

- **[geo-map-analytics](https://github.com/deepeshgupta12/geo-map-analytics)**  
  Developer-friendly geospatial analytics UI: city → micromarket → locality → roads → projects from Mapbox vector tiles, monthly metrics choropleths, pinned A/B comparisons, exports (PNG + CSV), shareable URLs.

---

### LLM-Powered Content & Intelligence (Guardrailed generation)

- **[sy-pdp-content-llm](https://github.com/deepeshgupta12/sy-pdp-content-llm)**  
  High-intent page content generation with guardrails for consistency, quality, and SEO hygiene: structured outputs, reusable templates, controllable tone at scale.

- **[sqy-locality-llm](https://github.com/deepeshgupta12/sqy-locality-llm)**  
  Context-aware locality content + FAQs for real-estate decisions: grounded explanations, structured FAQ generation, locality-level narrative consistency.

- **[squareyards-review-engine](https://github.com/deepeshgupta12/squareyards-review-engine)**  
  Trust-layer engine to collect, structure, and surface user feedback into decision-ready insights (themes, pros/cons, persona-fit, credibility signals).

- **[review-summary-engine](https://github.com/deepeshgupta12/review-summary-engine)**  
  Review Intelligence pipeline: ingests large datasets and produces (1) project-wise summaries and (2) per-review tags (persona + USPs). Built for deterministic outputs, batching/resume, and scale-friendly processing.

- **[stalled-project-news](https://github.com/deepeshgupta12/stalled-project-news)**  
  Search-first pipeline generating evidence-backed stalled/delayed project updates (JSON + HTML): strict source whitelisting, snippet-level evidence mapping, dedupe/timeline generation, citation coverage verification. Designed for zero-hallucination narratives.

- **[area-converter-ai](https://github.com/deepeshgupta12/area-converter-ai)**  
  Content generation toolkit for area converter experiences: landing + child pages, Mongo-ready JSON, HTML previews, strict length validation, batch pipelines (CSV → generation → validation/regeneration → DB payloads).

- **[seo-content-generation-system](https://github.com/deepeshgupta12/seo-content-generation-system)**  
  A programmatic SEO content engine for Square Yards resale listing pages. The system ingests raw datacenter JSON exports, performs deep keyword research via DataForSEO, and uses OpenAI to produce publication-ready SEO drafts in multiple formats — all through a REST API with a React-based review workbench UI.
  
- **[Automated-Locality-Report-Engine](https://github.com/deepeshgupta12/Automated-Locality-Report-Engine)**  
  Generates full locality reports (data → charts → LLM narratives → PDF + Lovable UI) from two JSON feeds (Locality + Property Rates). Repeatable for any locality without code changes — swap inputs + polygon/map asset.

---

## How I work

- Turn vague asks into **sharp product problems + success metrics**
- Partner deeply with engineering/design/data (high technical fluency)
- Prefer **evidence over vibes**: evaluation, guardrails, measurable outcomes
- Use AI + automation as leverage — not decoration

---

## Currently exploring

- **Evaluation-first LLM product development:** offline test sets, rubric-based scoring, citation coverage checks, refusal thresholds, and regression testing when prompts/models change.
- **Better retrieval over “more tokens”:** chunking strategies, query rewriting, hybrid retrieval (lexical + vector), reranking, and confidence gating.
- **Evidence-backed “news/intelligence” pipelines:** extraction → claim detection → dedupe → timelines → human-readable narratives + auditable artifacts.
- **Personalization loops that actually learn:** feedback-driven recommenders, session intent inference, segment-driven widgets, and “next best action” logic.
- **Local-first product engineering:** reproducible pipelines, persisted artifacts, Docker-first setup, and clean upgrade paths to production.
- **Geo + decision intelligence at scale:** multi-layer geo rendering, metric overlays, performant choropleths, and config-over-code onboarding for new cities/datasets.
- **Content systems with control:** template-driven generation, SEO hygiene, structured outputs, and strict validation so content is predictable and debuggable.
- **Agentic workflows for product work:** pipeline-based agents with scoped retrieval per step, run consoles, versions/logs, and artifacted outputs.
- **Trust layers in marketplaces:** review intelligence, credibility signals, persona-fit tagging, and deterministic-enough summarization to ship.

---

## Connect

- LinkedIn: https://www.linkedin.com/in/deepeshkumargupta  
- Email: deepeshkumargupta9891@gmail.com
