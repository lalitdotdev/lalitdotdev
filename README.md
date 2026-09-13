<div align="center">

# Lalit Sharma
### Full-Stack Developer & AI Engineer

[![Portfolio](https://img.shields.io/badge/Portfolio-lalitsharma.dev-black?style=flat-square&logo=vercel&logoColor=white)](https://lalitsharma.dev)
[![DevCastle](https://img.shields.io/badge/DevCastle-Live-58A6FF?style=flat-square&logo=rocket&logoColor=white)](https://devcastle.vercel.app)
[![X](https://img.shields.io/badge/X-@lalitdotdev-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/lalitdotdev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pinglalit-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/pinglalit)

</div>

<br/>

## About Me

I'm a full-stack developer with an Electronics & Communications Engineering background — self-taught in software and AI systems. I build and ship real products end-to-end: the app, the backend, and the AI features layered on top. My main project, **DevCastle**, is a live developer community platform with real users that I've built and run solo.

I care about shipping things that actually work for real users, not just demos — which means paying attention to type safety, caching, and what happens when an LLM call fails or times out.

<br/>

## 🏰 DevCastle — Developer Community Platform

A community platform for developers: discussion feeds, project launches, a job board, and an AI assistant — built and maintained solo.

**Live:** [devcastle.vercel.app](https://devcastle.vercel.app) &nbsp;|&nbsp; **Scale:** real users tested (currently in making)· ~174K lines of TypeScript · 25+ database models

- **AI Assistant** — In-app assistant using Groq for inference, local embeddings (`@xenova/transformers`), and Upstash Vector for retrieval-augmented answers about the platform. Built in stages: streaming chat → tool calling against the database → RAG → multi-agent coordination via LangGraph → rate limiting.
- **Reddit Market Intelligence** — Scrapes subreddit discussions (via Decodo + Cheerio) and uses an LLM to score and summarize SaaS opportunities from them — demand signals, existing competitors, monetization ideas.
- **Community & Social Feed** — Sub-communities, threaded comments, an editor for long-form posts, project launches with voting.
- **Job Board** — Full-text search over listings with filters for role, compensation, and stack.
- **CI/CD** — GitHub Actions pipeline running lint, typecheck, Lighthouse, CodeQL, and secret scanning (TruffleHog) on every push.
- **Analytics** — PostHog integrated for product usage tracking.

**Stack:** Next.js 14 (App Router) · TypeScript · MySQL + Prisma · Upstash Redis/Vector · Groq · LangGraph · Vercel

<br/>

## ✈️ Wayfarer — Multi-Agent Travel Planner

A travel planning tool that splits the problem across a few cooperating agents instead of one big prompt. [**GitHub Repo**](https://github.com/lalitdotev/wayfarer-multiagent)

- Built with **LangGraph**, running specialized agents (flight search, hotel search, itinerary synthesis) in parallel with shared state.
- Session state persisted in **PostgreSQL** so a planning session can be resumed.
- **Streamlit** frontend for interacting with the planner.

**Stack:** Python · LangGraph · LangChain · Streamlit · PostgreSQL

<br/>

## 🛠️ Tech Stack

**Languages:** TypeScript · JavaScript · Python · SQL

**Frontend:** Next.js · React · Tailwind CSS · Streamlit · TanStack Query · Zustand

**Backend:** Node.js · Express · FastAPI · tRPC · REST/GraphQL · Zod

**Data:** PostgreSQL · MySQL · MongoDB · Prisma · Redis · Pinecone

**AI/LLM:** LangGraph · LangChain · OpenAI API · Anthropic Claude API · Google Gemini · Groq · RAG (dense/hybrid retrieval)

**Infra:** AWS · Docker · Vercel · GitHub Actions · Sentry

<br/>

## 📬 Get in Touch

Open to full-stack and AI engineering roles, and to conversations about AI product work.

[![Email](https://img.shields.io/badge/Email-mailfor.lalitsharma%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:mailfor.lalitsharma@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pinglalit-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/pinglalit)
[![X](https://img.shields.io/badge/X-@lalitdotdev-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/lalitdotdev)

**AWS Certified:** [AWS Cloud Technical Essentials — 98%](https://www.coursera.org/account/accomplishments/verify/PST2AE5CWFFK)

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

</details>
