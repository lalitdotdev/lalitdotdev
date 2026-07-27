
<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=26&duration=2800&pause=1200&color=58A6FF&center=true&vCenter=true&width=620&lines=Full-Stack+%2B+AI+Systems+Engineer;Distributed+Systems+%2B+Agentic+Architectures;Founder+%40+DevCastle;I+ship+resilient+production+systems." alt="Typing SVG" />

<br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-litsharmadev.tech-black?style=for-the-badge&logo=vercel&logoColor=white)](https://litsharmadev.tech)
[![DevCastle](https://img.shields.io/badge/DevCastle-Live-58A6FF?style=for-the-badge&logo=rocket&logoColor=white)](https://devcastle.vercel.app)
[![X](https://img.shields.io/badge/X-@lalitdotdev-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/lalitdotdev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pinglalit-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/pinglalit)

</div>

<br/>

## ⚡ Engineering Philosophy

Building production software requires predictable systems, not magical assumptions. AI models and external APIs are inherently non-deterministic, high-latency network dependencies. I architect full-stack applications around one core rule: **the software stack must remain deterministic, type-safe, and resilient—regardless of service volatility.**

```

Client Input ──> [Type Boundary] ──> [State & Caching] ──> [Resilience Gateway] ──> [LLM / Data Service] ──> [Streaming UI]

```

* **Type Safety & Data Contracts:** Full end-to-end type safety from database models to UI components. All incoming inputs, API responses, and LLM outputs are validated at runtime with strict Zod/Pydantic schemas before reaching core application logic.
* **Backend Resilience & Scale:** High-throughput Node.js/TypeScript and Python services engineered with multi-tier caching (In-Memory ➔ Redis), sliding-window rate limiters, retries with exponential backoff + jitter, circuit breakers, and connection pooling.
* **Applied AI & LLM Systems:** Productionizing LLM features using stateful multi-agent orchestrations (LangGraph), hybrid search RAG (dense + sparse vector indexing), structured JSON output enforcement, and semantic caching to reduce latency and token cost.
* **Real-Time Streaming UI:** Building non-blocking user interfaces powered by Server-Sent Events (SSE) and WebSockets to render token streams in real-time while bypassing serverless gateway execution limits.
* **System Observability:** End-to-end telemetry with structured JSON logs tied to request correlation IDs, ensuring edge-case failures, API throttles, or LLM drops are isolated and debugged instantly.



```
request → input validation (Zod) → state machine → resilience gateway → distributed DB / LLM stream → UI render
```

**Core Focus:** High-throughput Node.js/TypeScript & Python backends, MERN/Next.js architectures, serverless platform engineering, production RAG & multi-agent systems, and real-time streaming interfaces.

<br/>

## 🚀 Featured Builds & Systems

### 🏰 DevCastle — Sovereign Social & Intelligence Platform
> A production-grade platform for modern developers combining community infrastructure, market intelligence, launch arenas, and career engines. **Live. Deployed. Hardened against real failure.**

<details open>
<summary><b>🔍 View Complete Feature Suite & System Breakdown</b></summary>

<br/>

#### 🤖 AI-Powered Reddit Market Intelligence Pipeline
* **Decodo Proxy-Backed Scraper** — Cheerio + Decodo proxy pipeline extracts top weekly threads and nested comments from targeted subreddits.
* **LLM Opportunity Scorer** — OpenAI/Insforge LLM processes scraped data to generate scored (0–10) SaaS opportunities with demand breakdown, existing competitors, monetization models, and go-to-market strategies.
* **Non-Blocking SSE Streaming** — Server-Sent Events stream incremental progress to dodge serverless connection limits (Vercel 504 gateway timeouts).
* **Dual-Layer Caching** — In-memory LRU Map → Prisma MySQL (12h TTL) delivering near-zero latency for repeated queries.
* **Upstash Distributed Rate Limiting** — Sliding-window IP limiter enforcing API endpoint protection with standard `X-RateLimit-*` headers.

#### 📊 Crunchbase Market Intelligence
* **Startup Discovery Engine** — Live graph integration searching Crunchbase organizations for funding rounds, investor networks, and valuation metrics inline.
* **Server Actions SSR** — Instant, server-rendered data fetching using Next.js 14 Server Actions with built-in caching.
* **Rate-Limited Client & Mocking** — In-memory request throttling with a full offline mock layer for local testing and CI/CD pipelines.

#### 📡 Social Engine & LaunchPad Arena
* **Sub-Dev Communities** — Granular member controls, moderation queues, topic spaces, and unique community identities.
* **Threaded Feed & EditorJS 2.0** — Fast feed with nested comments, syntax-highlighted code blocks, link previews, and image embeds.
* **LaunchPad Marketplace** — Dedicated arena for project launches featuring image carousels, status tracking, and upvote-weighted ranking algorithms.
* **Engagement Engine** — Follow graph, notification fan-out, bookmarks, and real-time activity metrics.

#### 💼 Career Engine & Creator Studio
* **Pro-Grade Job Board** — MySQL full-text search indexing with multi-dimensional filtering (roles, compensation, location, tech stack).
* **GitHub Curation Showcase** — Direct repository curation and showcasing on developer profiles.
* **AI Creator Studio** — Long-form EditorJS workspace powered by Google Gemini for drafting, summarizing, and technical documentation.
* **Stripe Monetization** — Subscription gating, recurring billing, and creator payout management via Stripe Webhooks.

#### 🗄️ System Architecture & Schema (Prisma MySQL — 25+ Relational Models)

```

MySQL (Prisma)
├── User, Account, Session         → Auth & Security Layer
├── Community, Subscription        → Social & Follow Graph
├── Post, Comment, Vote            → Threaded Feed Engine
├── LaunchProject, LaunchVote      → LaunchPad Marketplace
├── Job, Company, Application      → Career & Talent Engine
├── Essay, Category                → AI Creator Studio
├── RedditAnalysis                 → Market Intelligence Cache
└── StripeSubscription, Customer   → Payments & Subscriptions

```

**Tech Stack:** `Next.js 14 (App Router)` `TypeScript 5` `React 18` `Tailwind CSS` `Prisma ORM` `Aiven MySQL` `Upstash Redis` `Decodo Proxy + Cheerio` `Google Gemini` `InsForge AI` `G2 API V2` `UploadThing` `NextAuth.js` `Stripe API` `PostHog` `Vitest / Bun Test`

</details>

<br/>

### ✈️ Wayfarer — Multi-Agent Travel Planner
> An intelligent travel planning system coordinating specialized agents via LangGraph. [**GitHub Repo**](https://github.com/lalitdotdev/wayfarer-multiagent)

- **LangGraph Multi-Agent Orchestration** — Graph-based agent state management where specialized agents plan, execute, and pass state deterministically.
- **Domain-Specialized Sub-Agents** — Dedicated agent nodes for flight search, hotel discovery, custom itinerary synthesis, and final travel plan aggregation.
- **Tool Calling & External Search** — Dynamically fetches travel intelligence, pricing, and availability through structured tool interfaces.
- **Streamlit Interactive UI** — Clean, responsive web frontend for real-time plan generation, interactive edits, and structured recommendations.

**Stack:** `Python` `LangGraph` `LangChain` `Streamlit` `OpenAI / Claude API` `Tavily / Search APIs`

<br/>

## 🔭 High-Impact Systems Built

<table>
<tr>
<td width="50%" valign="top">

**🌐 Production Full-Stack Platforms**
Scalable web applications built on Next.js, React, Node.js/Express, and Python. Engineered with strict type boundaries, optimized database indexing (SQL/NoSQL), automated CI/CD pipelines, and zero-trust authentication.

</td>
<td width="50%" valign="top">

**🤖 Multi-Agent Orchestration & RAG**
Production LangGraph & Python multi-agent orchestration engines. High-accuracy Retrieval-Augmented Generation (RAG) pipelines utilizing dense vector indexing, hybrid search, and semantic caching over raw vector similarity.

</td>
</tr>
</table>

<br/>

## 🛠️ Production Tech Stack

<div align="left">

**Core Languages & Runtimes**
<br/>
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![HTML5/CSS3](https://img.shields.io/badge/HTML5_%2F_CSS3-E34F26?style=flat-square&logo=html5&logoColor=white)

**Frontend & Client State**
<br/>
![Next.js](https://img.shields.io/badge/Next.js_14-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React 18](https://img.shields.io/badge/React_18-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![React Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=flat-square&logo=reactquery&logoColor=white)
![Redux Toolkit](https://img.shields.io/badge/Redux_Toolkit-764ABC?style=flat-square&logo=redux&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-433E38?style=flat-square&logo=react&logoColor=white)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white)

**Backend Architecture & Middleware**
<br/>
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![tRPC](https://img.shields.io/badge/tRPC-2596BE?style=flat-square&logo=trpc&logoColor=white)
![REST & GraphQL](https://img.shields.io/badge/REST_%26_GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![Zod](https://img.shields.io/badge/Zod_Validation-3E67B1?style=flat-square&logo=zod&logoColor=white)
![Server-Sent Events](https://img.shields.io/badge/SSE_%2F_WebSockets-FF6B6B?style=flat-square&logo=webhook&logoColor=white)

**Data Infrastructure & ORMs**
<br/>
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Prisma ORM](https://img.shields.io/badge/Prisma_ORM-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=flat-square&logo=mongoose&logoColor=white)
![Redis Cache](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone_Vector_DB-000000?style=flat-square&logo=pinecone&logoColor=white)

**Agentic AI & LLM Systems**
<br/>
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=graphql&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![OpenAI API](https://img.shields.io/badge/OpenAI_API-412991?style=flat-square&logo=openai&logoColor=white)
![Anthropic Claude](https://img.shields.io/badge/Claude_API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)

`Stateful Agent Memory` `Multi-Agent Planning` `Tool/Function Execution` `Dense Semantic Search` `Hybrid RAG` `Structured Output Control`

**DevOps, Reliability & Cloud**
<br/>
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions_CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Axiom](https://img.shields.io/badge/Axiom_Logging-000000?style=flat-square&logo=axiom&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry_Observability-362D59?style=flat-square&logo=sentry&logoColor=white)

</div>

<br/>

## 📐 Systems & Reliability Standards

| Pillar | Engineering Execution |
|---|---|
| **Defensive I/O Execution** | Assume all external I/O will eventually fail, time out, or rate limit. Enforce strict timeouts, retries with jitter, and circuit breakers. |
| **Strict Type Boundaries** | Compile-time validation with TypeScript paired with runtime schema enforcement via Zod at every API boundary. |
| **Full Traceability** | Structured JSON logging tied to request correlation IDs. If an incident cannot be traced to root-cause in seconds, the telemetry is incomplete. |
| **Verification over SDK Assumptions** | Inspect raw HTTP payloads (`curl`, packet dumps) directly against the wire before trusting third-party abstractions or client SDKs. |

<br/>

## 📬 Connect & Collaborate

Open to technical leadership discussions, distributed systems design, high-performance web architecture, and production AI engineering.

[![Email](https://img.shields.io/badge/Email-mailfor.lalitsharma%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mailfor.lalitsharma@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pinglalit-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/pinglalit)
[![X](https://img.shields.io/badge/X-@lalitdotdev-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/lalitdotdev)

<br/>

<details>
<summary><b>📊 GitHub Engineering Metrics</b></summary>
<br/>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=lalitdotdev&theme=tokyonight&hide_border=true" />
</p>
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=lalitdotdev&show_icons=true&theme=tokyonight&hide_border=true" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=lalitdotdev&layout=compact&theme=tokyonight&hide_border=true" />
</p>

</details>

```
