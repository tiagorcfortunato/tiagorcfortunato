# Tiago Fortunato
**Product Engineer · AI Applications · SaaS · Berlin**

Shipping AI-powered products end-to-end with LLMs, RAG, and modern web stacks. Founder of [Odys](https://odys.com.br), a live multi-tenant SaaS. Builder of production RAG and Vision AI systems on FastAPI. MSc Software Engineering, Berlin 2026. Trilingual (Portuguese, English, German B2.2).

Daily user of Claude Code and agentic AI development workflows. My edge is shipping fast and owning outcomes from idea to production.

## Featured Projects

### [Odys](https://odys.com.br): Scheduling SaaS
Multi-tenant SaaS scheduling platform for Brazilian freelance professionals, built solo from scratch. Live in production, currently in active validation with industry professionals before scaling marketing.
- **Stack:** Next.js 16, TypeScript, React, Drizzle ORM, PostgreSQL, Supabase Auth, Stripe (subscriptions + PIX), Evolution API (WhatsApp)
- **Architecture:** Multi-tenant with isolated data per professional; public booking pages at `/p/[slug]`; rate limiting with Upstash Redis; error monitoring with Sentry; transactional email via Resend
- **Infra:** Self-hosted WhatsApp messaging server (Evolution API v2) on Railway; reminder flows via Supabase pg_cron; CI/CD via GitHub Actions

### [AI Career Assistant](https://chatbot.tifortunato.com): Production RAG Chatbot
Production RAG chatbot where recruiters ask questions about my background and get answers grounded in a curated knowledge base. [Live demo](https://chatbot.tifortunato.com) · [GitHub](https://github.com/tiagorcfortunato/rag-pdf-chatbot)
- **Hybrid retrieval:** semantic search + BM25 fused with Reciprocal Rank Fusion (RRF) for higher precision
- **Custom section-aware chunking** via font-size analysis to keep semantically related content together
- **Streaming SSE responses** via Groq (Llama 3.1) with conversation history and follow-up suggestions
- **RAGAs evaluation pipeline** measuring faithfulness, answer relevance, and context precision/recall
- **Stack:** FastAPI, LangChain, ChromaDB, fastembed, Groq, Docker. Self-hosted on AWS EC2 with Nginx and Let's Encrypt HTTPS

### [Inspection Management API](https://github.com/tiagorcfortunato/inspection-management-api): Vision AI REST API
Production REST API for infrastructure inspections with autonomous Vision AI classification. Upload a photo, the system returns severity, damage type, and an explainable rationale. [API Docs](https://inspection-management-api.onrender.com/docs) · [Dashboard](https://inspection-dashboard.vercel.app)
- **Vision AI** classification via Groq SDK with structured LLM output (LangChain)
- **Explainable AI:** human-readable rationale for every classification
- **LangSmith** integration for full LLM observability and tracing
- **JWT auth, rate limiting, comprehensive Pytest suite, CI/CD** via GitHub Actions

### [Road Hazard Detection](https://github.com/tiagorcfortunato): MSc Thesis
Two-stage hybrid pipeline: YOLOv8 object detection + rule-based expert system for automated road maintenance prioritization on the RDD2022 dataset.
- Best config (YOLOv8s): mAP50 0.663, Precision 0.694, Recall 0.604
- Rule-based post-processing reduced noisy detections by 31.2% while preserving structurally relevant defects
- Designed for interpretability: every prioritization decision traceable to explicit, auditable rules

### [DSA-Mastery](https://github.com/tiagorcfortunato/DSA-Mastery)
Centralized hub for algorithm and data structure solutions, synchronized from NeetCode.io.

## Technical Skills

- **AI-Augmented Development:** Claude Code, Cursor, agentic coding workflows, prompt engineering
- **AI & LLM Applications:** LLMs, RAG pipelines, embeddings, vector databases, hybrid retrieval, BM25, LangChain, ChromaDB, Groq, Llama, Vision AI, LangSmith, RAGAs, fastembed, YOLOv8, PyTorch
- **Backend & APIs:** Python, FastAPI, REST APIs, PostgreSQL, SQL, SQLAlchemy, Drizzle ORM, Pydantic, Alembic, JWT, Pytest
- **Full-Stack & SaaS:** TypeScript, JavaScript, React, Next.js, Tailwind, Supabase, Stripe, Resend, Upstash Redis, Evolution API
- **DevOps & Cloud:** Docker, GitHub Actions, CI/CD, AWS EC2, Nginx, Linux, Let's Encrypt, Railway, Vercel, Git, Sentry
- **Languages:** Portuguese (Native), English (Fluent), German (B2.2)

## Open to

**Product Engineer**, **AI Engineer**, **Solutions Engineer**, or **Founding Engineer** roles. Berlin or remote.

## Contact

- **Portfolio:** [tifortunato.com](https://tifortunato.com)
- **Career Assistant chatbot:** [chatbot.tifortunato.com](https://chatbot.tifortunato.com)
- **LinkedIn:** [linkedin.com/in/tiagorcfortunato](https://www.linkedin.com/in/tiagorcfortunato/)
- **Email:** tifortunato.eng@gmail.com

---

**Technical note:** This repository also contains the source code for my portfolio website (`index.html`) and CV source (`cv.tex`).
