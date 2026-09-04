# Taimoor Khan — AI engineer, Karachi

I take AI-built prototypes to production: **AI agents, RAG systems, and the backend underneath them.**

> [!NOTE]
> **Available for contract and freelance work.**
> Email [khant8k83@gmail.com](mailto:khant8k83@gmail.com) or message me on [LinkedIn](https://linkedin.com/in/taimoorkhan55).

Founders ship an MVP with a coding agent, it demos well, then it meets real users and real data. That gap — auth that leaks across tenants, retrieval that hallucinates, a queue with no idempotency, zero tests, no way to tell what broke — is the work I do. TypeScript and NestJS on the backend, Next.js and React on the front, PostgreSQL and Supabase underneath.

## From prototype to production

```mermaid
flowchart LR
    A["AI-built MVP<br/>the demo works"] --> B{"Production audit"}
    B --> C["Tenant isolation<br/>auth and sessions"]
    B --> D["Data integrity<br/>migrations, transactions"]
    B --> E["Agent behaviour<br/>tool boundaries, evals"]
    B --> F["Operability<br/>tests, logs, traces"]
    C --> G["Safe to charge for"]
    D --> G
    E --> G
    F --> G
```

**Take an AI-built MVP to production.** Tenant isolation, authentication and session handling, payment integration, migrations, error handling, tests, and the observability needed to debug it at 2am. The unglamorous layer between "the demo works" and "we can charge for this".

**Build AI agents and RAG systems that hold up.** Tool design and permission boundaries enforced outside the model, multi-tenant retrieval where tenant identity comes from the session and never from the model, streaming responses with provenance, and evals so behaviour is measured rather than vibed.

**Clean up vibe-coded repositories.** Codebases generated fast by AI, now unmaintainable: no boundaries, duplicated logic, silent breakage. I give them a structure a human team and a coding agent can both work inside.

**Review before launch.** Adversarial, whole-repository audits of security, data integrity, deployment and test coverage — with a go/no-go answer, not a list of nits.

## How I work: agent-first engineering

Humans make the engineering decisions. Agents do the work inside them.

```mermaid
flowchart TD
    H["Humans decide, once"] --> H1["Architecture"]
    H --> H2["API contracts"]
    H --> H3["Data model and boundaries"]
    H --> H4["Allowed dependencies"]
    H1 --> R["Written into the repository"]
    H2 --> R
    H3 --> R
    H4 --> R
    R --> W["Agent implements freely inside them"]
    W --> Q{"Hits a decision<br/>it does not own?"}
    Q -->|"no"| S["Ships"]
    Q -->|"yes"| E["Raises the blocker<br/>instead of inventing an answer"]
```

Architecture, API contracts, the data model and allowed dependencies are decided by people and written into the repository, so neither a new engineer nor a coding agent has to re-derive them. Within those constraints an agent picks the implementation freely. Outside them — a new dependency, a new service, a schema change with a migration path — it raises the blocker.

That principle is why the tools below exist: they encode the decision, so it only has to be made once.

## Open source

**[prod-readiness](https://github.com/Taimoorkhan1122/prod-readiness)** — Production-readiness audit plugin for Claude Code. Seven parallel specialist agents review security, backend, database, DevOps, QA, frontend and AI-security concerns over one shared evidence pass, and return a SHIP / FIX THEN SHIP / HOLD verdict with an evidence ledger. Built for teams shipping AI-generated code.

**[boring-react](https://github.com/Taimoorkhan1122/boring-react)** — Agent Skills that make coding agents write boring, production-grade React: no needless `useEffect`, no surprise dependencies, no cargo-cult memoization. Portable `SKILL.md` format, 12 adversarial evals.

**[langraph_agent](https://github.com/Taimoorkhan1122/langraph_agent)** — Hierarchical LangGraph agent on NestJS. An LLM classifies each query, a StateGraph routes it to RAG, chart, direct or hybrid branches, retrieval runs per-tenant against Weaviate, and the answer streams over SSE with file and page references.

**[ecommerce-backend](https://github.com/Taimoorkhan1122/ecommerce-backend)** — E-commerce API in TypeScript with Node, Express, GraphQL and PostgreSQL.

## Stack

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=ts,js,python,rust,nodejs,nestjs,express,graphql,react,nextjs,tailwind,vite,postgres,supabase,mongodb,redis,docker,kubernetes,githubactions,cloudflare,vercel&theme=dark&perline=11">
  <img alt="TypeScript, JavaScript, Python, Rust, Node.js, NestJS, Express, GraphQL, React, Next.js, Tailwind CSS, Vite, PostgreSQL, Supabase, MongoDB, Redis, Docker, Kubernetes, GitHub Actions, Cloudflare, Vercel" src="https://skillicons.dev/icons?i=ts,js,python,rust,nodejs,nestjs,express,graphql,react,nextjs,tailwind,vite,postgres,supabase,mongodb,redis,docker,kubernetes,githubactions,cloudflare,vercel&theme=light&perline=11">
</picture>

- **Languages** — TypeScript, JavaScript, Python, SQL, some Rust
- **Backend** — Node.js, NestJS, Express, GraphQL, REST, WebSockets, Server-Sent Events
- **Frontend** — React, Next.js, TanStack Query, Tailwind CSS, Vite
- **Data** — PostgreSQL, Supabase, MongoDB, Redis, Weaviate, pgvector
- **AI** — LangGraph, LangChain, RAG pipelines, agent tooling and evals, Claude Code, Codex, MCP
- **Infrastructure** — Docker, Kubernetes, GitHub Actions, Cloudflare Workers, Vercel

## Background

Six years building for the web, starting in 2020 with React frontends and moving to backend and platform work from 2021. Currently at Geeks of Kolachi in Karachi, Pakistan, working across full-stack product delivery and AI systems. I work remotely.

## GitHub activity

![On GitHub since 2019](https://img.shields.io/badge/on_GitHub_since-2019-1f6feb?style=flat-square)
![443 merged pull requests](https://img.shields.io/badge/merged_pull_requests-443-1f6feb?style=flat-square)
![2142 commits in the last year](https://img.shields.io/badge/commits_last_year-2%2C142-1f6feb?style=flat-square)
![Based in Karachi, Pakistan](https://img.shields.io/badge/based_in-Karachi,_PK-1f6feb?style=flat-square)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-streak-stats.herokuapp.com/?user=Taimoorkhan1122&hide_border=true&theme=github-dark-blue">
  <img alt="Contribution streak for Taimoorkhan1122: current streak, longest streak and total contributions" src="https://github-readme-streak-stats.herokuapp.com/?user=Taimoorkhan1122&hide_border=true&theme=default">
</picture>

## Contact

| | |
|---|---|
| **Email** | [khant8k83@gmail.com](mailto:khant8k83@gmail.com) |
| **LinkedIn** | [linkedin.com/in/taimoorkhan55](https://linkedin.com/in/taimoorkhan55) |
| **X** | [@Taimi360](https://x.com/Taimi360) |
| **Stack Overflow** | [taimoor](https://stackoverflow.com/users/12393165/taimoor) |
| **Website** | [tamork.tech](http://tamork.tech/) |

> [!TIP]
> Best first message: what you have built, what is breaking, and when you need it working.
