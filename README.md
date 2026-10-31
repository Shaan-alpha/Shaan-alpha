<p><a href="https://shaansatsangi.com">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Shaan-alpha/Shaan-alpha/main/assets/header-dark.svg?v=4">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Shaan-alpha/Shaan-alpha/main/assets/header-light.svg?v=4">
    <img src="https://raw.githubusercontent.com/Shaan-alpha/Shaan-alpha/main/assets/header-light.svg?v=4" width="100%" alt="shaansatsangi.com: Shaan Satsangi, AI systems engineer in Jaipur, India. Diagram of a five-step pipeline: input, model (in yellow), guards, human approval, ship.">
  </picture>
</a></p>

I build agents and retrieval systems with the guardrails designed in: deterministic scoring, checks that fail closed, and a human approval wherever a mistake would be expensive. Only the yellow step in the diagram runs a model; the guards, the approval gate and the shipping around it are code, covered by tests.

I finished a B.Tech in computer science in 2026 and turned down an M.Tech seat at IIIT Tiruchirappalli to work full time. I'm open to AI engineering, backend and data roles, and I can start now. Email [shaansatsangi@gmail.com](mailto:shaansatsangi@gmail.com), or find me on [LinkedIn](https://linkedin.com/in/shaansatsangi) and at [shaansatsangi.com](https://shaansatsangi.com).

## Projects

### [Skill Issue](https://github.com/Shaan-alpha/Skill-Issue)

Scores any public GitHub profile out of 100 at [skillissue.tech](https://skillissue.tech), tracing every point to evidence; here is [what it makes of my profile](https://skillissue.tech/u/Shaan-alpha).

The score is computed in code and the model only narrates it. 1,000+ tests run in CI.

### [Atlas](https://github.com/Shaan-alpha/atlas-financial-assistant)

An AI financial analyst on Telegram ([@AtlasAnalyst_bot](https://t.me/AtlasAnalyst_bot)) that you talk to in plain language.

Its 20 tools run under Gemini function calling, and the 10 that touch user data are bound to one user id. It is serving again 6 seconds after `kill -9`.

### [Syntrueno](https://github.com/Shaan-alpha/syntrueno)

Gemini agents [running on Cloud Run](https://syntrueno-18489510475.us-central1.run.app) diagnose live incidents and propose fixes, and every consequential change waits for a person to approve that exact action.

It uses single-use SHA-256 approvals and five guards that fail closed, writing every refusal to a hash-chained audit log.

### [AI Reel Factory](https://github.com/Shaan-alpha/AI-Reel-Factory)

Send `/makeshort` in Telegram and it pitches story ideas from the news; the ones I approve are scripted, fact-checked, voiced and published as [YouTube Shorts](https://www.youtube.com/channel/UC5rDIoOPYLrHaf2IQ5hRlRw).

Each idea must cite two or more sources it actually retrieved, and the pipeline runs for under $10 a month.

### [Think9 Brain](https://github.com/Shaan-alpha/think9-brain)

A LangGraph app at [think9-brain.vercel.app](https://think9-brain.vercel.app) that answers questions over a synthetic multi-brand corpus, citing the exact source section and its good-as-of date, and holding back superseded documents unless you ask about history.

It refused all 32 unanswerable questions in evaluation, and held-out accuracy is 0.881.

### Smaller work

- [disaster-management-rag](https://github.com/Shaan-alpha/disaster-management-rag): grounded answers over disaster-management guidelines, behind three gates: a confidence threshold, a constrained prompt, and a check for unsupported details. 18 of 20 right on the held-out set, and the evaluation reproduces on a clean clone with no API key. 97 tests.
- [prospect-assist-ai](https://github.com/Shaan-alpha/prospect-assist-ai): ranks 25,000 synthetic bank customers by loan propensity, built for IDBI Innovate 2026. AUC 0.81 on held-out data, and the top 200 convert at 49.5% against a 4.2% base rate. [Try the demo](https://shaan-alpha.github.io/prospect-assist-ai/).
- [YouTube Wrapped](https://github.com/Shaan-alpha/Youtube-Wrapped): a Databricks medallion lakehouse on Delta Lake over 9,418 of my own watches, served by FastAPI and a Next.js dashboard. [See the live dashboard](https://youtube-wrapped-by-shaan.vercel.app).
- [CRM Sales Warehouse](https://github.com/Shaan-alpha/CRM-Sales-Warehouse): Python ETL on Airflow into a PostgreSQL star schema, with 10 SQL data-quality checks and a 5-page Power BI dashboard.
- [JARVIS](https://github.com/Shaan-alpha/jarvis-py): a local-first voice assistant on Ollama, with wake-word detection, semantic memory and threshold-gated PDF retrieval over FAISS. 615 tests pass in CI.
- [telegram-mcp](https://github.com/Shaan-alpha/telegram-mcp): a local MCP server that gives AI agents your own Telegram account, through Telethon.
- [Face Sort Studio](https://github.com/Shaan-alpha/Face-Sort-Studio): sorts photos by face on your own machine, with OpenCV and ONNX.
- [Sahaara](https://github.com/Shaan-alpha/Sahaara_APP): a safety app whose one-tap SOS reaches online users within a radius, over Supabase Realtime.
- [Cog & Cosmos](https://github.com/Shaan-alpha/Cog-and-Cosmos): an idle game in Svelte and PixiJS. [Play it in the browser](https://shaan-alpha.github.io/Cog-and-Cosmos/).

Everything else is in [my repositories](https://github.com/Shaan-alpha?tab=repositories).

## Open source

Merged upstream:

- [Home Assistant Android #7018](https://github.com/home-assistant/android/pull/7018): rebuilt the media-player widget settings screen in Jetpack Compose and Material 3.
- [Narwhals #3697](https://github.com/narwhals-dev/narwhals/pull/3697): added a `maintain_order` option to `list.unique`, wired through the DuckDB, Ibis and Spark-like backends, with tests. Narwhals is the dataframe layer behind Altair, Bokeh and LightGBM.
- [ha-mcp #1670](https://github.com/homeassistant-ai/ha-mcp/pull/1670), the community Home Assistant MCP server: fixed restarts through a reverse proxy being reported as failures.

Open, not yet merged (checked 31 Oct 2026): [Ollama #16715](https://github.com/ollama/ollama/pull/16715), [Supabase #46915](https://github.com/supabase/supabase/pull/46915), [Helm #32250](https://github.com/helm/helm/pull/32250), [dbt #12952](https://github.com/dbt-labs/dbt/pull/12952), [LangChain Google #1950](https://github.com/langchain-ai/langchain-google/pull/1950) and [LangChain Google #1840](https://github.com/langchain-ai/langchain-google/pull/1840).

## Tools

- **AI and retrieval:** LangGraph, Gemini function calling, Groq, MCP, ONNX embeddings, FAISS, Ollama, Whisper, OpenCV, scikit-learn
- **Backend:** Python, FastAPI, Flask, PostgreSQL (Neon, Supabase), Redis (Upstash), SQLAlchemy, SQLite
- **Data:** Airflow, Databricks, PySpark, Delta Lake, dbt, pandas, Power BI
- **Web and deployment:** TypeScript, Next.js, React, Tailwind, Docker, GitHub Actions, Google Cloud Run, Vercel, Render, an Azure VM under systemd

Also familiar with: PyTorch, TensorFlow, Playwright, C and C++.

## Certifications and awards

- Certificate of Distinction, Atlas AI Hackathon, Humanity Founders (2026)
- Introduction to Model Context Protocol, Anthropic (2026)
- Data Science, AI/ML & Data Engineer, micro1 (2026)
- Fundamentals of Machine Learning and Fundamental AI Concepts, Microsoft (2023)
- Introduction to Cybersecurity and Cybersecurity Essentials, Cisco Networking Academy
- Second place, IEEE Student Chapter inter-college debate

## Recent activity

<!-- ACTIVITY_STREAM_START -->
- Pushed to <b><a href="https://github.com/Shaan-alpha/Skill-Issue">Skill-Issue</a></b> (Oct 25, 2026)
- Pushed to <b><a href="https://github.com/Shaan-alpha/Portfolio">Portfolio</a></b> (Oct 25, 2026)
- Pushed to <b><a href="https://github.com/Shaan-alpha/Cog-and-Cosmos">Cog-and-Cosmos</a></b> (Oct 25, 2026)
- Pushed to <b><a href="https://github.com/Shaan-alpha/syntrueno">syntrueno</a></b> (Oct 25, 2026)
- Opened PR <a href="https://github.com/Shaan-alpha/Skill-Issue/pull/147">"docs: close out v1.0.16 and v1.0.17 (tagged + released)"</a> in <b><a href="https://github.com/Shaan-alpha/Skill-Issue">Skill-Issue</a></b> (merged, Oct 25, 2026)
<!-- ACTIVITY_STREAM_END -->

## Guestbook and AMA

Leave a note in the [guestbook](https://github.com/Shaan-alpha/Shaan-alpha/issues/new?template=guestbook.yml) or [ask me anything](https://github.com/Shaan-alpha/Shaan-alpha/issues/new?template=ama.yml). Notes appear here once I have read them, and questions once I have answered them.

<details>
<summary>Notes from visitors</summary>

<table width="100%">
  <tr><th align="left">Visitor</th><th align="left">Message</th><th>Date</th></tr>
  <!-- GUESTBOOK_START -->
  <tr><td colspan="3" align="center"><i>Leave yours with the guestbook link above.</i></td></tr>
</table>

</details>

<!-- AMA_START -->
<!-- AMA_END -->

Email is the fastest way to reach me: [shaansatsangi@gmail.com](mailto:shaansatsangi@gmail.com).
