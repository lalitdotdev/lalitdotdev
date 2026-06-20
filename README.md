<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=26&duration=2800&pause=1200&color=58A6FF&center=true&vCenter=true&width=620&lines=AI+Agentic+Engineer;Full-Stack+Systems+Builder;Founder+%40+DevCastle;I+ship+production%2C+not+demos." alt="Typing SVG" />

<br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-litsharmadev.tech-black?style=for-the-badge&logo=vercel&logoColor=white)](https://litsharmadev.tech)
[![DevCastle](https://img.shields.io/badge/DevCastle-Live-58A6FF?style=for-the-badge&logo=rocket&logoColor=white)](https://devcastle.vercel.app)
[![X](https://img.shields.io/badge/X-@lalitdotdev-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/lalitdotdev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pinglalit-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/pinglalit)

</div>

<br/>

## ⚡ What I do

Software is going through its biggest shift since the internet itself — the next generation of products won't be built by large teams writing boilerplate, they'll be built by engineers who can fuse AI, systems design, and product instinct into one skillset. That's the bet I'm making.

I build full-stack products where the **backend is an AI system**, not a feature bolted onto one. That means treating LLM calls like any other unreliable network dependency — timeouts, retries, circuit breaking, structured logging, graceful degradation — while still shipping a UI people actually want to use.

```
scrape → LLM analysis → resilience layer → score → stream → ship
```

**Right now:** agentic data pipelines on serverless infra, production reliability for LLM-backed APIs, and the unglamorous plumbing that keeps AI features from falling over under real traffic.

<br/>

**Focus areas:**
`Multi-Agent Architectures` `Agentic Workflows` `RAG Systems` `Knowledge Graphs` `LLM Applications` `AI Infrastructure` `System Design` `Distributed Systems` `Backend Architecture` `Developer Platforms` `Platform Strategy` `Product Engineering`

<br/>

## 🏰 DevCastle — Featured Build

> A developer platform combining AI-native workflows, market intelligence, and builder infrastructure. **Live. Deployed. Hardened against real failure**, not a demo.

<table>
<tr>
<td width="50%" valign="top">

### 📊 Reddit Market Intelligence

Agentic pipeline: scrapes target subreddits → LLM-driven analysis → ranked SaaS opportunity scoring. Built to survive serverless constraints and flaky upstream APIs.

- **SSE streaming** — long AI jobs stream incrementally to dodge Vercel's 504 ceiling
- **InsForge AI resilience layer** — timeouts, backoff retries, error classification, auto credit-refunds on failed-but-charged requests
- **Aiven MySQL retry logic** — handles transient connection drops from cold-start reconnects
- **Structured JSON logging** → Vercel Log Drain / Axiom, full request traceability
- **Test coverage** — Vitest + curl smoke tests against the *live* API

</td>
<td width="50%" valign="top">

### 🔌 G2 API V2 Integration

Full market-intelligence integration: buyer intent, competitor analysis, opportunity scoring, category browsing, credit management.

- **~22 files · ~2,400 LOC** of TypeScript
- Diagnosed a production `401` traced to a missing env token
- Fixed silent auth failure: `Token token=` → `Bearer` — the kind of detail that only surfaces by inspecting raw traffic, not docs
- Built an in-app **API explorer** so credit-metered calls can be tested without burning quota blind

</td>
</tr>
</table>

**Stack:** `Next.js 14 (App Router)` `TypeScript` `Tailwind CSS` `Prisma` `Aiven MySQL` `InsForge AI` `G2 API V2` `EmailJS`

**Platform pillars:** AI-native workflows · intelligence layer (startup discovery, competitive analysis, trend detection) · builder infrastructure (developer communities, project discovery) · platform engineering (scalable, cloud-native architecture)

<br/>

## 🔭 Other builds

<table>
<tr>
<td width="50%" valign="top">

**🤖 Multi-Agent AI Assistant**
Production-grade AI orchestration powered by LangGraph — agents that plan, delegate, and execute as a coordinated system rather than a single prompt-response loop.

</td>
<td width="50%" valign="top">

**🔍 AI Knowledge Systems**
Retrieval-first architectures for intelligent information discovery — RAG pipelines built for accuracy over vector-search vibes.

</td>
</tr>
</table>

<br/>

## 🧠 How I debug

I validate API behavior directly against the live service — `curl`, raw request/response inspection — before trusting an SDK's abstraction or assuming the docs are right. The hard bugs in AI-integrated systems live in the gap between what a provider *claims* and what it *does* under load, rate limits, or cold starts.


<br/>
## 🛠️ Tech Stack
 
<sub>Core stack used in production (Next.js · TypeScript · Prisma · Aiven MySQL · InsForge AI) marked in the DevCastle section above — the full list below spans what I build with day-to-day across full-stack and AI-native engineering.</sub>
 
<div align="left">

**Frontend**
<br/>
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Tailwind](https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-433E38?style=flat-square&logo=react&logoColor=white)
![React Query](https://img.shields.io/badge/React_Query-FF4154?style=flat-square&logo=reactquery&logoColor=white)
![Radix UI](https://img.shields.io/badge/Radix_UI-161618?style=flat-square&logo=radixui&logoColor=white)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white)
 
**Backend & APIs**
<br/>
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![tRPC](https://img.shields.io/badge/tRPC-2596BE?style=flat-square&logo=trpc&logoColor=white)
![REST](https://img.shields.io/badge/REST_APIs-02569B?style=flat-square&logo=fastapi&logoColor=white)
![Webhooks](https://img.shields.io/badge/Webhooks-FF6B6B?style=flat-square&logo=webhook&logoColor=white)
![Zod](https://img.shields.io/badge/Zod-3E67B1?style=flat-square&logo=zod&logoColor=white)
 
**Data & Storage**
<br/>
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square&logo=pinecone&logoColor=white)
![Aiven](https://img.shields.io/badge/Aiven-FF4F00?style=flat-square&logo=aiven&logoColor=white)
 
**AI / Agentic Engineering**
<br/>
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=graphql&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Vector DBs](https://img.shields.io/badge/Vector_DBs-6E56CF?style=flat-square&logo=databricks&logoColor=white)
 
`RAG pipelines` `Multi-agent orchestration` `Agent memory & state` `Tool/function calling` `Prompt engineering` `Embeddings & semantic search` `LLM evaluation & guardrails` `Streaming inference (SSE)`
 
**Infra, DevOps & Observability**
<br/>
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Axiom](https://img.shields.io/badge/Axiom-000000?style=flat-square&logo=axiom&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white)
 
`Serverless architecture` `Structured logging` `Retry & circuit-breaker patterns` `Rate limiting` `Cold-start optimization` `Log aggregation (Log Drain)`
 
**Tooling & Workflow**
<br/>
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![cURL](https://img.shields.io/badge/cURL-073551?style=flat-square&logo=curl&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
 
**Integrations shipped in production**
<br/>
`InsForge AI` `G2 API V2` `EmailJS` `Vercel Log Drain` `OAuth providers`
 
</div>
<br/>

## 📐 Engineering principles

| Principle | What it means in practice |
|---|---|
| **LLM calls are unreliable I/O** | Timeouts, retries, fallbacks aren't polish — they're what separates a demo from a product |
| **Observability before scale** | If a prod failure can't be traced request → root cause, it isn't done |
| **Verify, don't assume** | Test against the real API/DB/service before believing a fix works |

<br/>

## 📬 Let's talk

Open to conversations on agentic system design, production AI reliability, and full-stack architecture.

[![Email](https://img.shields.io/badge/Email-mailfor.lalitsharma%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mailfor.lalitsharma@gmail.com)

<br/>

<details>
<summary><b>📊 GitHub Stats</b></summary>
<br/>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=lalitdotdev&theme=tokyonight&hide_border=true" />
</p>
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=lalitdotdev&show_icons=true&theme=tokyonight&hide_border=true" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=lalitdotdev&layout=compact&theme=tokyonight&hide_border=true" />
</p>
<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=lalitdotdev&theme=algolia&no-frame=true&margin-w=10" />
</p>

</details>

<br/>

<div align="center">

<img src="https://komarev.com/ghpvc/?username=lalitdotdev&style=flat-square&color=58A6FF" alt="Profile views" />

</div>
