# Hi, I’m Deepesh 👋

Senior Product Manager building AI + data products that ship and measure.

I’ve spent 6+ years across B2B, B2C, D2C and B2B2C — marketplaces, data platforms, and internal tools. I like taking messy, ambiguous problems and turning them into clear product bets with success metrics, then prototyping the fastest path to “does this work?” before scaling.

**Core focus areas:** marketplace discovery, real-estate intelligence, LLM systems with evidence + evaluation, recommendation engines, and geo/data analytics.

---

## What you’ll find here

This GitHub is a mix of:

- **Production-minded prototypes** — things I’d confidently harden and plug into a real system
- **AI/ML systems** — LLM workflows, recommender systems, applied ML/CV, and evaluation tooling
- **POCs & sandboxes** — quick experiments to validate hypotheses before asking engineering to invest

Most repos start from a real product problem, not a tutorial.

---

## Tech I use

Data Science, Machine Learning, FastAPI, Pydantic, Postgres/Mongo, Python, Typescript, HTML and CSS, Elastic-style search patterns, vector search (where needed), Playwright/httpx, background jobs, Docker, and pragmatic evaluation/guardrails for LLM outputs.

---

These are the best “walkthrough” repos if you want to understand how I think and build:

### Computer Vision, Applied ML, Data Science and AI/LLM/RAG/Vector principles:

- **[movie-recommendation-mvp](https://github.com/deepeshgupta12/movie-recommendation-mvp)**  
  Local-first, production-style recommender: hybrid candidate retrieval (popularity + item-item + ALS + genre signals), time-decay-aware feature store, trained ranker, FastAPI serving, and a Streamlit UI with posters + feedback-driven personalization. End-to-end demo of discovery → ranking → iteration loops.

- **[smart-kitchen-os](https://github.com/deepeshgupta12/smart-kitchen-os)**  
  AI-powered culinary operating system combining inventory management + health intelligence + automated meal planning. Includes recipe extraction to structured data, pantry deduction logic, TDEE/macros profiling, and a FastAPI + Postgres backend with a Next.js frontend.

- **[realestate-image-classifier](https://github.com/deepeshgupta12/realestate-image-classifier)**  
  Image classification pipeline to categorize and optimize thumbnails (rooms, amenities, visuals) to improve engagement in visual catalogs. Includes dataset strategy, labeling approach, model training, and inference patterns.

- **[brain-tumor-ai](https://github.com/deepeshgupta12/brain-tumor-ai)**  
  Applied CV project on medical imaging and tumor detection — built to deepen practical understanding of CV workflows, model interpretation patterns, and responsible handling of sensitive domains.

- **[hotel-booking-cancellation-model](https://github.com/deepeshgupta12/hotel-booking-cancellation-model)**  
  End-to-end ML pipeline + FastAPI service that predicts booking cancellations, exposes risk buckets, and supports both batch and real-time scoring.

- **[youtube-learning-copilot](https://github.com/deepeshgupta12/youtube-learning-copilot)**
  A grounded, transcript-first study companion that turns any YouTube video into a structured learning pack — with searchable chunks, chapter flows, flashcards, quizzes, progress tracking, and citation-backed Q&A.

- **[used-car-price-prediction](https://github.com/deepeshgupta12/used-car-price-prediction)**
  UCPP is a local-first, Docker-friendly Used Car Price Prediction service for two markets: India (IN) and United States (US). It ships with a clean preprocessing pipeline, persisted ML artifacts, and a FastAPI server exposing simple single and batch prediction endpoints.
  
---

### Agentic Product Engineering (AI Systems & Tooling)

- **[pm-agent-os](https://github.com/deepeshgupta12/pm-agent-os)**
  Local-first PM agent OS with pipeline templates + pipeline runs (Discovery → Strategy → PRD), step-level retrieval (RAG) with evidence batch scoping, run console (retrieval preview/regenerate), and pipeline UI with step statuses, latest artifacts, and scoped RAG debug deep-links.

---

### AI for Discovery & Personalization (Marketplace systems):
- **[squareyards-rec-engine](https://github.com/deepeshgupta12/squareyards-rec-engine)**  
  Experiments for recommendation-driven discovery in marketplace journeys — ranking signals, shortlist logic, segment-driven recommendations, and practical “what should the user see next?” widgets.

- **[personal-finance-copilot](https://github.com/deepeshgupta12/personal-finance-copilot)**
  A local-first, AI-assisted personal finance dashboard for young professionals. This project ingests mock bank/UPI/credit card data, auto-categorises spending, detects “bad patterns”, and generates a plain-language money story for each month – plus concrete actions to try next month. Built with FastAPI, SQLite, Pandas, scikit-learn, Jinja2, and the OpenAI API.

---

### Data & Geo Analytics (Decision intelligence):
- **[geo-map-analytics](https://github.com/deepeshgupta12/geo-map-analytics)**
  A lightweight, developer-friendly geospatial analytics UI that renders city → micromarket → locality → roads → projects layers from Mapbox vector tiles, overlays monthly metrics as a dynamic choropleth, and supports A/B pinned comparisons + exports (PNG + CSV) + shareable URLs.

---

### LLM-Powered Content & Intelligence (Guardrailed generation):
- **[sy-pdp-content-llm](https://github.com/deepeshgupta12/sy-pdp-content-llm)**  
  High-intent page content generation workflows with guardrails for consistency, quality, and SEO hygiene. Emphasis on structured outputs, reusable templates, and controllable tone across large page inventories.

- **[sqy-locality-llm](https://github.com/deepeshgupta12/sqy-locality-llm)**  
  Context-aware locality content + FAQs to help users make sense of complex real-estate choices. Focus on grounded explanations, structured FAQ generation, and locality-level narrative consistency.

- **[squareyards-review-engine](https://github.com/deepeshgupta12/squareyards-review-engine)**  
  Trust-layer engine to collect, structure, and surface user-generated feedback. Built around turning messy reviews into decision-ready insights (themes, pros/cons, persona-fit, and credibility signals).

- **[review-summary-engine](https://github.com/deepeshgupta12/review-summary-engine)**  
  Local-first Review Intelligence pipeline that ingests large review datasets and produces:  
  (1) **project-wise AI summaries** and (2) **per-review tags** (persona + USPs). Built for resume/batching, deterministic outputs, and scale-friendly processing patterns.

- **[stalled-project-news](https://github.com/deepeshgupta12/stalled-project-news)**  
  Search-first pipeline that generates **evidence-backed** stalled/delayed project updates (JSON + HTML). Built with strict source whitelisting, snippet-level evidence mapping, dedupe/timeline generation, and citation coverage verification. Designed for zero-hallucination outputs and buyer/investor-readable narratives.

- **[area-converter-ai](https://github.com/deepeshgupta12/area-converter-ai)**  
  Content generation toolkit for area converter experiences: landing + child pages, Mongo-ready JSON, HTML previews, strict word-length validation, and batch pipelines (CSV → generation → validation/regeneration → DB payloads).

- **[sqy-dse-llm](https://github.com/deepeshgupta12/sqy-dse-llm)**  
  LLM-driven enhancements for catalog exploration — making search/filter-heavy experiences feel guided and conversational. Focused on user intent capture, contextual nudges, structured outputs, and reliability constraints.

- **[Automated-Locality-Report-Engine](https://github.com/deepeshgupta12/Automated-Locality-Report-Engine)**
  Generate a full locality report (data → charts → LLM narratives → PDF + Lovable UI) from two JSON feeds (Locality + Property Rates). Built to be repeatable for any locality (e.g., Andheri East ✅, Malad East ✅) without code changes — just swap input JSONs and the polygon/map asset.

---

## How I work

- Translate vague Product ideas and business asks into **clear product problems + success metrics**
- Partner deeply with engineering/design/data; high technical fluency
- Prefer **evidence over vibes**: evaluation, guardrails, and measurable outcomes
- Use AI and automation as leverage — not as decoration

---

## Currently exploring

- RAG and vector systems and evaluation frameworks for LLM-driven products
- Heavy Data Science and ML principle-driven products
- Engagement-based thumbnail and content optimization
- Geo & data intelligence for multi-location decision-making
- Small, composable services teams can embed into existing stacks

---

## Connect

- LinkedIn: https://www.linkedin.com/in/deepeshkumargupta
- Email: deepeshkumargupta9891@gmail.com
