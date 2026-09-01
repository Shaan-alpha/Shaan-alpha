<!-- ════════════════════════ HEADER BANNER ════════════════════════ -->
<a href="https://github.com/Shaan-alpha">
  <img src="https://raw.githubusercontent.com/Shaan-alpha/Shaan-alpha/main/assets/header.svg?v=2" width="100%" alt="Shaan Satsangi, Agentic AI &amp; Systems Engineer" />
</a>

<!-- ════════════════════════ ROLE PILLARS ════════════════════════ -->
<div align="center">

**Agentic AI Systems** &nbsp;·&nbsp; **AI/ML Engineering** &nbsp;·&nbsp; **RAG &amp; LLM Applications** &nbsp;·&nbsp; **Python Backends** &nbsp;·&nbsp; **Data Engineering**

<!-- ════════════════════════ TYPING SUBTITLE ════════════════════════ -->
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=A78BFA&center=true&vCenter=true&width=900&lines=Agentic+AI+%26+Systems+Engineer;Creator+of+skillissue.tech;Multi-agent+systems+%C2%B7+RAG+%C2%B7+FastAPI+backends;Open+to+AI+%2F+ML+%2F+Backend+roles)](https://github.com/Shaan-alpha)

<!-- ════════════════════════ SOCIAL BADGES ════════════════════════ -->
<a href="https://linkedin.com/in/shaansatsangi"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://shaansatsangi.com"><img src="https://img.shields.io/badge/Portfolio-A78BFA?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Portfolio" /></a>
<a href="mailto:shaansatsangi@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://github.com/Shaan-alpha"><img src="https://img.shields.io/badge/Follow-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>

</div>

<br />

<!-- ════════════════════════ ABOUT ME ════════════════════════ -->
## <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28" /> About Me

I'm an **Agentic AI & Systems Engineer** who likes owning a problem end-to-end, from the data and the retrieval layer through the model to the product people actually use.

- 🔭 I build **autonomous Python pipelines**, **PySpark / Databricks lakehouses**, and **RAG / LLM systems**: then ship them as full-stack apps with **Next.js & FastAPI**.
- 🧩 Deepest in **agents, RAG and Python backends**, with real range across **data engineering and full-stack** when the problem needs it.
- 🎓 **B.Tech CSE, Class of 2026** (graduated). Earned an **M.Tech CSE seat at IIIT Tiruchirappalli** and turned it down to build full-time.
- ⚡ I default to **free, production-grade tooling**: most of my projects run at **~$0/month**.
- 📫 **Open to AI / ML / Backend roles, right now.** Let's talk: **shaansatsangi@gmail.com**

<br />

<!-- ════════════════════════ HOW I BUILD ════════════════════════ -->
## 🧭 How I Build

The same spine runs through almost everything below: **the model writes the prose, never the number.** Decisions live in code that can be tested; the LLM narrates, routes, and asks for clarification around it. Every layer fails open, except the gates, which fail closed.

```mermaid
flowchart LR
    IN["<b>Messy input</b><br/>APIs · webhooks<br/>PDFs · voice · sheets<br/>event streams"]

    subgraph CORE ["Deterministic core — the part that must be right"]
        direction TB
        ING["<b>Typed ingestion</b><br/>rate-limit aware<br/>conditional requests<br/>bounded fan-out"]
        LOGIC["<b>Pure decision code</b><br/>scoring · matching · salience<br/><i>every output traces to evidence</i>"]
        CACHE["<b>Fail-open cache</b><br/>Redis · Postgres · Parquet"]
        ING --> LOGIC --> CACHE
    end

    subgraph EDGE ["LLM at the edges"]
        direction TB
        NARR["<b>Narration &amp; synthesis</b><br/>receives computed JSON,<br/>never the raw data"]
        ROUTE["<b>Tool routing</b><br/>closure-bound per user<br/>failover across model chains"]
    end

    GATE{"<b>Gate</b><br/>is this worth<br/>sending at all?"}
    OUT["<b>Shipped surface</b><br/>Next.js · FastAPI<br/>Telegram · MCP · CLI"]
    SILENT(["<b>Silence</b><br/><i>audited, never accidental</i>"])

    IN --> ING
    LOGIC --> NARR
    LOGIC --> ROUTE
    NARR --> GATE
    ROUTE --> GATE
    CACHE --> OUT
    GATE -->|"clears the bar"| OUT
    GATE -->|"doesn't, or fails"| SILENT

    classDef core fill:#1e293b,stroke:#a78bfa,stroke-width:2px,color:#e2e8f0
    classDef edge fill:#312e81,stroke:#818cf8,stroke-width:2px,color:#e2e8f0
    classDef term fill:#0f172a,stroke:#475569,stroke-width:1.5px,color:#cbd5e1
    class ING,LOGIC,CACHE core
    class NARR,ROUTE edge
    class IN,OUT,SILENT,GATE term
```

**Where each piece is real, not aspirational:** the deterministic core is [Skill Issue](https://github.com/Shaan-alpha/Skill-Issue)'s two-pass scorer · the gate is [Atlas](https://github.com/Shaan-alpha/atlas-financial-assistant)'s salience check, which returns `send: false` and means it · closure-bound routing is Atlas's 20 tools, each welded to one user id · fail-open caching is Skill Issue's four Redis layers.

<br />

### What I work on, and what proves it

```mermaid
flowchart TD
    ME(("<b>Shaan</b>"))

    ME --> A["<b>Agentic AI</b>"]
    ME --> B["<b>RAG &amp; retrieval</b>"]
    ME --> C["<b>Python backends</b>"]
    ME --> D["<b>Data engineering</b>"]

    A --> A1["<b>Atlas</b> — 20 tools under Gemini<br/>function calling, live on Telegram"]
    A --> A2["<b>Syntrueno</b> — agent swarm that mutates<br/>real Cloud Run behind a human gate"]
    A --> A3["<b>telegram-mcp</b> — MCP server giving<br/>agents your own Telegram account"]

    B --> B1["<b>Think9 Brain</b> — cites its source section,<br/>refuses when the corpus can't answer"]
    B --> B2["<b>disaster-management-rag</b> — 18/20 held-out,<br/>reproducible with no API key"]
    B --> B3["<b>JARVIS-PY</b> — semantic memory +<br/>threshold-gated PDF RAG, fully local"]

    C --> C1["<b>Skill Issue</b> — FastAPI, Neon, Upstash,<br/>OAuth, warm p95 ≤ 200 ms"]
    C --> C2["<b>VouchRank</b> — multi-tenant SaaS on<br/>Postgres RLS + 12 Deno edge functions"]

    D --> D1["<b>YouTube Wrapped</b> — Databricks medallion<br/>lakehouse on Delta Lake"]
    D --> D2["<b>CRM Sales Warehouse</b> — Airflow-orchestrated<br/>star schema, dbt-tested, Power BI"]

    classDef root fill:#a78bfa,stroke:#7c3aed,stroke-width:3px,color:#0f172a
    classDef pillar fill:#312e81,stroke:#818cf8,stroke-width:2px,color:#e2e8f0
    classDef proof fill:#1e293b,stroke:#475569,stroke-width:1.5px,color:#cbd5e1
    class ME root
    class A,B,C,D pillar
    class A1,A2,A3,B1,B2,B3,C1,C2,D1,D2 proof
```

<br />

<!-- ════════════════════════ FEATURED PROJECTS ════════════════════════ -->
## 🚀 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 📈 [Atlas](https://github.com/Shaan-alpha/atlas-financial-assistant) &nbsp;·&nbsp; [**▶ Talk to it**](https://t.me/AtlasAnalyst_bot)
`AI Agent` · `Fintech` · `Backend`

An **AI financial analyst that lives in Telegram**: conversation only, no slash commands or buttons. Learns you as you talk, pulls live quotes and fundamentals through an **eight-provider failover chain** (five quote, three fundamentals), reads PDFs and spreadsheets natively (tables stay tables), transcribes voice notes, and sends a morning briefing *only* when something on your watchlist matters; silence is enforced control flow, not a prompt suggestion.

**Gemini function calling** drives the loop across **20 tools**, each closure-bound to one user so the model cannot reach another's data. Always-on under `systemd` with a polling watchdog that force-exits a bot which is up but no longer listening: back serving **six seconds after `kill -9`**. 191 tests.

![Python](https://img.shields.io/badge/-Python_3.13-3776AB?style=flat-square&logo=python&logoColor=white)
![Gemini](https://img.shields.io/badge/-Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![Telegram](https://img.shields.io/badge/-Telegram_Bot-26A5E4?style=flat-square&logo=telegram&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-Postgres_18-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/-SQLAlchemy_2.0-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)
![Azure](https://img.shields.io/badge/-Azure_VM-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)

[**▶ Talk to it**](https://t.me/AtlasAnalyst_bot) · [**Code**](https://github.com/Shaan-alpha/atlas-financial-assistant)

</td>
<td width="50%" valign="top">

### ⚡ [Skill Issue](https://github.com/Shaan-alpha/Skill-Issue)
`Full-Stack` · `AI` · `Production`

[![release](https://img.shields.io/github/v/release/Shaan-alpha/Skill-Issue?style=flat-square&label=&color=10b981)](https://github.com/Shaan-alpha/Skill-Issue/releases)

Reads any public GitHub profile and scores it **out of 100** across six weighted signals, then places you on a **7-tier ladder** from Hobbyist to Principal with a sub-rank. Every point traces to real evidence in your repos; the AI writes the *narrative*, never the numbers (**0 hallucinated scores**). Pick **Roast Mode** for what a blunt senior would say, or **Mentor Mode** for how to fix it. Free, no signup; sign in to save reports and share them.

> It scored me **81/100: Staff Engineer**, nine points off Principal, then roasted me for it.

![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Neon](https://img.shields.io/badge/-Neon-00E699?style=flat-square&logo=neon&logoColor=white)
![Vercel](https://img.shields.io/badge/-Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Groq](https://img.shields.io/badge/-Groq-F55036?style=flat-square&logo=groq&logoColor=white)

[**Live**](https://skillissue.tech) · [**Code**](https://github.com/Shaan-alpha/Skill-Issue)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 💬 [VouchRank](https://github.com/Shaan-alpha/vouchrank) &nbsp;·&nbsp; [**▶ Live Demo**](https://vouchrank.vercel.app)
`Full-Stack` · `SaaS` · `AI`

Multi-tenant, white-label **reputation + AI-search-optimization SaaS**: a compliance-first review funnel (FTC / Google 2026 review rules), **LLM-visibility audits** (ChatGPT · Gemini · Perplexity), embeddable social-proof widgets, **Stripe** subscriptions + billing portal, and **Supabase Postgres Row-Level Security** tenant isolation across 12 Deno edge functions; fully clickable live in demo mode.

![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/-Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Supabase](https://img.shields.io/badge/-Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-Postgres_RLS-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Stripe](https://img.shields.io/badge/-Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white)
![Deno](https://img.shields.io/badge/-Deno-000000?style=flat-square&logo=deno&logoColor=white)

[**▶ Live Demo**](https://vouchrank.vercel.app) · [**Code**](https://github.com/Shaan-alpha/vouchrank)

</td>
<td width="50%" valign="top">

### 🎬 [AI Reel Factory](https://github.com/Shaan-alpha/AI-Reel-Factory)
`AI/ML` · `Data Eng` · `Automation`

Fully autonomous, **~$0/month** pipeline that researches news, writes & narrates scripts in a near-human voice, generates AI B-roll, auto-edits a captioned cinematic vertical video, and publishes daily YouTube Shorts: **one Telegram tap** is the only human input.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Gemini](https://img.shields.io/badge/-Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![FFmpeg](https://img.shields.io/badge/-FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white)

[**▶ Watch**](https://youtube.com/@butitmatters) · [**Code**](https://github.com/Shaan-alpha/AI-Reel-Factory)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📊 [YouTube Wrapped](https://github.com/Shaan-alpha/Youtube-Wrapped)
`Data Eng` · `Analytics`

Personal watch-history analytics product built on a **Databricks medallion lakehouse** (Bronze → Silver → Gold) over Delta Lake, served through a deployed **FastAPI + Next.js** dashboard.

![Databricks](https://img.shields.io/badge/-Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white)
![PySpark](https://img.shields.io/badge/-PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Delta Lake](https://img.shields.io/badge/-Delta_Lake-00ADD4?style=flat-square&logo=delta&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

[**Code**](https://github.com/Shaan-alpha/Youtube-Wrapped)

</td>
<td width="50%" valign="top">

### 🏗️ [CRM Sales Warehouse](https://github.com/Shaan-alpha/CRM-Sales-Warehouse)
`Data Eng` · `Analytics`

End-to-end CRM analytics platform: Python **ETL/ELT** into a star-schema **PostgreSQL** warehouse, orchestrated with **Airflow**, validated with **dbt tests**, and surfaced as a 5-page **Power BI** executive dashboard.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![dbt](https://img.shields.io/badge/-dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Airflow](https://img.shields.io/badge/-Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![Power BI](https://img.shields.io/badge/-Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)

[**Code**](https://github.com/Shaan-alpha/CRM-Sales-Warehouse)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧠 [JARVIS-PY](https://github.com/Shaan-alpha/jarvis-py)
`AI/ML`

Local-first AI **voice assistant** with wake-word barge-in, online/offline STT, **semantic memory**, **PDF RAG**, tool-agent routing, reminders, and interruptible TTS; privacy-first, runs on your machine.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Ollama](https://img.shields.io/badge/-Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![FAISS](https://img.shields.io/badge/-FAISS-0467DF?style=flat-square&logo=meta&logoColor=white)
![Vosk](https://img.shields.io/badge/-Vosk-1E88E5?style=flat-square&logo=audiomack&logoColor=white)

[**Code**](https://github.com/Shaan-alpha/jarvis-py)

</td>
<td width="50%" valign="top">

### 🛡️ [Sahaara](https://github.com/Shaan-alpha/Sahaara_APP)
`Full-Stack`

Safety-focused full-stack app with gesture-based **emergency SOS**, **MapLibre** live location sharing, trusted contacts, and **Twilio** SMS alerts; built for fast, reliable real-world response.

![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Supabase](https://img.shields.io/badge/-Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![Twilio](https://img.shields.io/badge/-Twilio-F22F46?style=flat-square&logo=twilio&logoColor=white)
![MapLibre](https://img.shields.io/badge/-MapLibre-396CB2?style=flat-square&logo=maplibre&logoColor=white)

[**Code**](https://github.com/Shaan-alpha/Sahaara_APP)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛰️ [Syntrueno](https://github.com/Shaan-alpha/syntrueno) &nbsp;·&nbsp; [**▶ Live service**](https://syntrueno-18489510475.us-central1.run.app)
`Agentic AI` · `Zero-Trust` · `GCP`

A **zero-trust autonomous cloud-ops swarm**. Gemini agents diagnose live incidents, propose remediations, judge their own plans for safety, and: behind a **single-use SHA-256 human gate bound to that exact action**: execute real changes against real Cloud Run infrastructure, then re-read live state until it converges rather than trusting the API's acknowledgement.

Five guards fail closed, cheapest first. Every refusal is audited into a **hash-chained Firestore ledger**, never silent. **113 tests** run offline in ~0.9 s with no credentials.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Gemini](https://img.shields.io/badge/-Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![Cloud Run](https://img.shields.io/badge/-Cloud_Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Firestore](https://img.shields.io/badge/-Firestore-FFCA28?style=flat-square&logo=firebase&logoColor=black)

[**▶ Live**](https://syntrueno-18489510475.us-central1.run.app) · [**Code**](https://github.com/Shaan-alpha/syntrueno)

</td>
<td width="50%" valign="top">

### 🧾 [Think9 Brain](https://github.com/Shaan-alpha/think9-brain) &nbsp;·&nbsp; [**▶ Live**](https://think9-brain.vercel.app)
`RAG` · `LangGraph` · `Retrieval`

A grounded **institutional-memory assistant** that cites the exact source section, states a good-as-of date, and holds back superseded documents. Built to be *trusted*, which means built to say "I don't know."

**Refusal recall is 1.000 on both eval sets**: across 32 unanswerable questions (invented vendors, plausible-but-absent figures, out-of-scope functions) it never once fabricated an answer.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![LangGraph](https://img.shields.io/badge/-LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Groq](https://img.shields.io/badge/-Groq-F55036?style=flat-square&logo=groq&logoColor=white)

[**▶ Live**](https://think9-brain.vercel.app) · [**Code**](https://github.com/Shaan-alpha/think9-brain)

</td>
</tr>
</table>

<sub>**More:** [telegram-mcp](https://github.com/Shaan-alpha/telegram-mcp) (MCP server for your own Telegram account) · [Face Sort Studio](https://github.com/Shaan-alpha/Face-Sort-Studio) (local CV photo organizer) · [Cog & Cosmos](https://github.com/Shaan-alpha/Cog-and-Cosmos) (Svelte/PixiJS idle game) · and [browse all repos →](https://github.com/Shaan-alpha?tab=repositories)</sub>

<br />

<!-- ════════════════════════ OPEN SOURCE ════════════════════════ -->
## 🌐 Open Source

Shipping into other people's codebases, where the review bar isn't mine to set.

**Merged upstream**

| PR | Project | What it fixed |
| :--- | :--- | :--- |
| [narwhals#3697](https://github.com/narwhals-dev/narwhals/pull/3697) | **Narwhals** · 1.7k ⭐ | Added a `maintain_order` argument to `Expr.list.unique` / `Series.list.unique`, across the backend implementations |
| [ha-mcp#1670](https://github.com/homeassistant-ai/ha-mcp/pull/1670) | **Home Assistant MCP** · 4.5k ⭐ | A restart through a reverse proxy returned 502/503 and was read as a failure; the known-good patterns now cover it |
| [anker-solix-api#314](https://github.com/thomluther/anker-solix-api/pull/314) | **anker-solix-api** · 291 ⭐ | Extended X1 device support by updating the status enumerations |

**Open, in review**

| PR | Project | What it does |
| :--- | :--- | :--- |
| [ollama#16715](https://github.com/ollama/ollama/pull/16715) | **Ollama** · 179k ⭐ | Fixes CLI image-path parsing bugs |
| [supabase#46915](https://github.com/supabase/supabase/pull/46915) | **Supabase** · 108k ⭐ | Allows newlines in the SMS OTP template string in Studio |
| [appwrite#12597](https://github.com/appwrite/appwrite/pull/12597) | **Appwrite** · 57k ⭐ | Allows a null `name` parameter on the user-creation endpoints |
| [helm#32250](https://github.com/helm/helm/pull/32250) | **Helm** · 30k ⭐ | Surfaces the installed chart's source location |
| [android#7018](https://github.com/home-assistant/android/pull/7018) | **Home Assistant Android** · 3.8k ⭐ | Refactors the media-player widget config activity to Compose + Material 3 |
| [langchain-google#1950](https://github.com/langchain-ai/langchain-google/pull/1950) · [#1840](https://github.com/langchain-ai/langchain-google/pull/1840) | **LangChain Google** · 400 ⭐ | Stops the spurious `$defs` warning on converted schemas; migrates the integration tests to async |

```mermaid
flowchart LR
    ME(("<b>Contributions</b>"))

    ME --> DATA["<b>Data &amp; DataFrames</b>"]
    ME --> INFRA["<b>Infrastructure</b>"]
    ME --> AI["<b>AI tooling</b>"]
    ME --> IOT["<b>Home &amp; IoT</b>"]

    DATA --> N["Narwhals<br/><b>merged ✅</b>"]
    INFRA --> H["Helm<br/><i>in review</i>"]
    INFRA --> S["Supabase<br/><i>in review</i>"]
    INFRA --> AP["Appwrite<br/><i>in review</i>"]
    AI --> O["Ollama<br/><i>in review</i>"]
    AI --> LG["LangChain Google<br/><i>in review ×2</i>"]
    IOT --> HM["Home Assistant MCP<br/><b>merged ✅</b>"]
    IOT --> HA["Home Assistant Android<br/><i>in review</i>"]
    IOT --> AS["anker-solix-api<br/><b>merged ✅</b>"]

    classDef root fill:#a78bfa,stroke:#7c3aed,stroke-width:3px,color:#0f172a
    classDef area fill:#312e81,stroke:#818cf8,stroke-width:2px,color:#e2e8f0
    classDef merged fill:#064e3b,stroke:#10b981,stroke-width:2px,color:#d1fae5
    classDef review fill:#1e293b,stroke:#475569,stroke-width:1.5px,color:#cbd5e1
    class ME root
    class DATA,INFRA,AI,IOT area
    class N,HM,AS merged
    class H,S,AP,O,LG,HA review
```

<br />

<!-- ════════════════════════ TECH STACK ════════════════════════ -->
## 🛠️ Tech Stack

**🗄️ Data Engineering & Analytics**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-00ADD4?style=for-the-badge&logo=delta&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logoColor=white)

**🤖 AI / ML**

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logo=groq&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge&logo=meta&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)

**💻 Full-Stack**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Neon](https://img.shields.io/badge/Neon-00E699?style=for-the-badge&logo=neon&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white)
![Deno](https://img.shields.io/badge/Deno-000000?style=for-the-badge&logo=deno&logoColor=white)

**☁️ DevOps & Cloud**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=for-the-badge&logo=render&logoColor=white)

<details>
<summary><b>+ more tools I reach for</b></summary>
<br />

![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Whisper](https://img.shields.io/badge/faster--whisper-412991?style=for-the-badge&logo=openai&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-154F3C?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Redis](https://img.shields.io/badge/Upstash_Redis-00E9A3?style=for-the-badge&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=for-the-badge&logo=ffmpeg&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=for-the-badge&logo=twilio&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

</details>

<br />

<!-- ════════════════════════ CURRENTLY ════════════════════════ -->
## 🎯 What I'm Up To

- 🛰️ Built **[Syntrueno](https://github.com/Shaan-alpha/syntrueno)** for the Google Cloud "All Things Agentic" Hackathon: an agent swarm that makes real infrastructure changes behind a cryptographic human gate. [Live on Cloud Run](https://syntrueno-18489510475.us-central1.run.app).
- 🚀 Shipping **[Skill Issue](https://github.com/Shaan-alpha/Skill-Issue)** at [skillissue.tech](https://skillissue.tech) — currently **v1.0.11**. Scores any GitHub profile out of 100, roasts it, and hands you the receipt. Free, no signup.
- 📈 Running **[Atlas](https://github.com/Shaan-alpha/atlas-financial-assistant)** live on Telegram ([@AtlasAnalyst_bot](https://t.me/AtlasAnalyst_bot)); always-on AI financial analyst, self-healing, 191 tests. Earned a **Certificate of Distinction** at the Atlas AI Hackathon (Humanity Founders).
- 🎬 Running **AI Reel Factory**: a fully autonomous, ~$0/month pipeline that publishes daily Shorts to [**@butitmatters**](https://youtube.com/@butitmatters).
- 🌐 Contributing upstream — merged into **Narwhals**, **Home Assistant MCP**, and **anker-solix-api**; open PRs at **Ollama**, **Supabase**, **Appwrite**, and **Helm**.
- 🤝 **Open to AI/ML · Agentic AI · Backend · Data Engineering roles** and available immediately.

<br />

<!-- ════════════════════════ CERTIFICATIONS ════════════════════════ -->
## 📜 Certifications & Awards

| Certification | Issuer | Year |
| :--- | :--- | :---: |
| 🏆 Certificate of Distinction: Atlas AI Hackathon | Humanity Founders | 2026 |
| 🎓 M.Tech CSE admission offer (declined for full-time work) | IIIT Tiruchirappalli | 2026 |
| Introduction to Model Context Protocol (MCP) | Anthropic | 2026 |
| Data Science, AI/ML Engineer & Data Engineer | micro1 | 2026 |
| Fundamentals of Machine Learning | Microsoft | 2023 |
| Fundamental AI Concepts | Microsoft | 2023 |
| 🥈 2nd Place: IEEE Debate Competition | IEEE | - |

<br />

<!-- ════════════════════════ GITHUB STATS ════════════════════════ -->
## 📈 GitHub Activity

<div align="center">

<img width="49%" src="https://raw.githubusercontent.com/Shaan-alpha/Shaan-alpha/main/profile-summary-card-output/tokyonight/3-stats.svg" alt="GitHub stats" />
<img width="49%" src="https://raw.githubusercontent.com/Shaan-alpha/Shaan-alpha/main/profile-summary-card-output/tokyonight/1-repos-per-language.svg" alt="Top languages" />

<img src="https://streak-stats-delta.vercel.app/?user=Shaan-alpha&theme=tokyonight&hide_border=true&background=0d1117" alt="GitHub streak" />

</div>

### ⚡ Recent Activity

<!-- ACTIVITY_STREAM_START -->
- 🚀 Pushed 1 commit to <b><a href="https://github.com/Shaan-alpha/AI-Reel-Factory">Shaan-alpha/AI-Reel-Factory</a></b> (Sep 01, 2026)
- ⚡ Opened PR <a href="https://github.com/Shaan-alpha/AI-Reel-Factory/pull/8">"Fix the 2026-09-01 audit: invented citations, unapproved re-runs, missing voice direction"</a> in <b><a href="https://github.com/Shaan-alpha/AI-Reel-Factory">Shaan-alpha/AI-Reel-Factory</a></b> (Sep 01, 2026)
- 🚀 Pushed 1 commit to <b><a href="https://github.com/Shaan-alpha/syntrueno">Shaan-alpha/syntrueno</a></b> (Aug 30, 2026)
- 🚀 Pushed 1 commit to <b><a href="https://github.com/Shaan-alpha/Skill-Issue">Shaan-alpha/Skill-Issue</a></b> (Aug 25, 2026)
<!-- ACTIVITY_STREAM_END -->

<br />

<!-- ════════════════════════ GUESTBOOK & AMA ════════════════════════ -->
## 💬 Guestbook & AMA

<div align="center">

<a href="https://github.com/Shaan-alpha/Shaan-alpha/issues/new?template=guestbook.yml"><img src="https://img.shields.io/badge/📖_Sign_my_Guestbook-A78BFA?style=for-the-badge" alt="Sign my Guestbook" /></a>
&nbsp;
<a href="https://github.com/Shaan-alpha/Shaan-alpha/issues/new?template=ama.yml"><img src="https://img.shields.io/badge/🎙️_Ask_Me_Anything-1F6FEB?style=for-the-badge" alt="Ask Me Anything" /></a>

</div>

<table width="100%">
  <tr><th align="left">Visitor</th><th align="left">Message</th><th>Date</th></tr>
  <!-- GUESTBOOK_START -->
  <tr><td colspan="3" align="center"><i>👋 Want to appear here? Sign the guestbook above!</i></td></tr>
</table>

<!-- AMA_START -->
<!-- AMA_END -->

<br />

<!-- ════════════════════════ CONNECT ════════════════════════ -->
## 🤝 Let's Build Something

<div align="center">

I like turning messy inputs into useful outcomes; data platforms, AI systems, and products that ship.<br/>
Always happy to talk **data, AI, and building things**.

<a href="https://linkedin.com/in/shaansatsangi"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:shaansatsangi@gmail.com"><img src="https://img.shields.io/badge/Email_Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://shaansatsangi.com"><img src="https://img.shields.io/badge/View_Portfolio-A78BFA?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Portfolio" /></a>

</div>

<!-- ════════════════════════ FOOTER ════════════════════════ -->
<img src="https://raw.githubusercontent.com/Shaan-alpha/Shaan-alpha/main/assets/footer.svg" width="100%" alt="" />

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=Shaan-alpha&color=a78bfa&style=flat-square&label=Profile+views" alt="Profile views" />
</div>
