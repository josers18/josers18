<!--
  IMPORTANT: commas in capsule-render's color= param MUST be %2C-encoded
  inside srcset (and ideally in src too). HTML5 srcset parsing treats raw
  commas as candidate separators, which silently truncates the URL and
  drops &text=, &desc=, animation, etc. Don't "simplify" these to plain
  commas — you'll lose the name and subtitle from the rendered banner.
-->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0:0A2540%2C50:0062CC%2C100:29B5E8&height=220&section=header&text=Jose%20Sifontes&fontSize=56&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Data%20Science%20%7C%20Engineering%20%7C%20AI&descAlignY=58&descSize=22&descColor=cfe8ff" />
  <source media="(prefers-color-scheme: light)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0:00A1E0%2C50:29B5E8%2C100:9CD7FF&height=220&section=header&text=Jose%20Sifontes&fontSize=56&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Data%20Science%20%7C%20Engineering%20%7C%20AI&descAlignY=58&descSize=22&descColor=ffffff" />
  <img width="100%" alt="Jose Sifontes — Data Science | Engineering | AI" src="https://capsule-render.vercel.app/api?type=waving&color=0:0062CC%2C50:29B5E8%2C100:00A1E0&height=220&section=header&text=Jose%20Sifontes&fontSize=56&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Data%20Science%20%7C%20Engineering%20%7C%20AI&descAlignY=58&descSize=22&descColor=e0f4ff" />
</picture>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1000&color=29B5E8&center=true&vCenter=true&width=720&lines=Distinguished+Technical+Architect+%40+Salesforce;Data+%26+AI+Leader+%7C+ML+Practitioner;Building+with+Python+%7C+R+%7C+SQL+%7C+Snowflake;Military+Veteran+%F0%9F%87%BA%F0%9F%87%B8+%7C+Oenophile+%F0%9F%8D%B7+%7C+Tech+Geek+%F0%9F%A4%96" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/jsifontes">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://github.com/josers18">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://analyticsmadesimple.com">
    <img src="https://img.shields.io/badge/Blog-analyticsmadesimple.com-29B5E8?style=for-the-badge&logo=hashnode&logoColor=white" />
  </a>
  <a href="https://josers18.github.io">
    <img src="https://img.shields.io/badge/Portfolio-josers18.github.io-0062CC?style=for-the-badge&logo=githubpages&logoColor=white" />
  </a>
</p>

---

## 🧑‍💻 About Me

I'm a **Distinguished Technical Architect on Data and AI at Salesforce** with deep roots in data — from wrangling raw datasets to deploying ML models in production. I hold an **M.S. in Data Science from Northwestern University** and an **M.S. in Data Engineering from WGU** and bring a rare combination of technical depth and customer-facing consultative experience across the data and AI space.

Before tech, I served in the **U.S. Military**, which shaped my approach to problem solving: methodical, high-stakes, and mission-first. I'm fluent in **English and Spanish**, based in **Miami, FL**, and equally at home in a Jupyter notebook and a customer discovery call.

| | |
|---|---|
| 🔭 **Building** | AI/ML integrations with Salesforce Data Cloud & Snowflake |
| 🌱 **Exploring** | LLMs, Agent-to-Agent (A2A) protocols, MCP, AI/ML DevOps |
| 💬 **Ask me about** | Data Science, ML, Data Governance, Analytics Engineering |
| 🌎 **Languages** | English, Spanish |
| ✍️ **Blog** | [analyticsmadesimple.com](https://analyticsmadesimple.com) |
| 🎖️ **Fun fact** | Military veteran, oenophile, and permanent resident of the rabbit hole |

---

## 🧭 What I Build

> The recurring shape across most of my work — agentic, conversation-first UIs talking to enterprise data through MCP. Click any node to jump to a representative repo.

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'ui-sans-serif, system-ui, -apple-system','background':'#0D1117','primaryColor':'#0D1117','primaryTextColor':'#E6EDF3','primaryBorderColor':'#21262D','lineColor':'#7D8590','clusterBkg':'#161B22','clusterBorder':'#21262D','titleColor':'#29B5E8','edgeLabelBackground':'#161B22','tertiaryColor':'#0D1117','tertiaryTextColor':'#E6EDF3','tertiaryBorderColor':'#21262D'}}}%%
flowchart LR
    %% ── Personas ──────────────────────────────────────────────
    Banker([🧑‍💼 Relationship Banker]):::persona
    Customer([👤 End Customer]):::persona

    %% ── Apps / Surfaces ───────────────────────────────────────
    subgraph SURFACE["🖥️ Conversational Surfaces"]
        direction TB
        Horizon["<b>Horizon</b><br/><i>Headless-JDO</i><br/>Next.js · TypeScript"]:::app
        Sim["<b>Transaction Simulator</b><br/><i>Data360 Fin Sim</i><br/>Python"]:::app
        Token["<b>Token Comparison Tool</b><br/>FastAPI · OAuth 2.1 + PKCE"]:::app
    end

    %% ── Agent / Orchestration ────────────────────────────────
    subgraph BRAIN["🧠 Agent Layer"]
        direction TB
        Claude{{"<b>Claude Sonnet</b><br/>tool-calling LLM"}}:::agent
        Agentforce(["<b>Agentforce</b><br/>topics · actions · guardrails"]):::agent
    end

    %% ── MCP fabric ────────────────────────────────────────────
    subgraph MCP_LAYER["🔌 Model Context Protocol"]
        direction TB
        HostedMCP["<b>Data360-Hosted-MCP</b><br/>Heroku · SSE + stdio<br/>43 tools / 16 families"]:::mcp
        RefMCP["<b>Salesforce-Data360-MCP</b><br/>reference impl"]:::mcp
    end

    %% ── Platform / Data ───────────────────────────────────────
    subgraph PLATFORM["🗄️ Salesforce Platform & Data"]
        direction TB
        CRM[("Salesforce CRM<br/>accounts · cases · ops")]:::data
        DC[("Data 360 / Data Cloud<br/>unified profile · CIs")]:::data
        TN[("Tableau Next<br/>analytics surface")]:::data
        Snow[("Snowflake<br/>warehoused signal")]:::data
    end

    %% ── Edges ─────────────────────────────────────────────────
    Banker --> Horizon
    Customer --> Sim
    Banker -. "benchmarking" .-> Token

    Horizon --> Claude
    Sim --> Claude
    Token --> Claude

    Claude <==> Agentforce
    Claude --> HostedMCP
    Claude --> RefMCP
    Agentforce --> HostedMCP

    HostedMCP --> CRM
    HostedMCP --> DC
    HostedMCP --> TN
    HostedMCP --> Snow
    RefMCP --> DC

    %% ── Styling (dark fills + white text — readable on both GitHub themes) ──
    classDef persona fill:#0A2540,stroke:#cfe8ff,stroke-width:1.5px,color:#ffffff
    classDef app     fill:#0062CC,stroke:#9CD7FF,stroke-width:1.5px,color:#ffffff
    classDef agent   fill:#1C3C3C,stroke:#D97757,stroke-width:2px,color:#ffffff
    classDef mcp     fill:#00A1E0,stroke:#0A2540,stroke-width:1.5px,color:#ffffff
    classDef data    fill:#29B5E8,stroke:#0A2540,stroke-width:1.5px,color:#0A2540

    %% ── Click-throughs to representative repos ──
    click Horizon "https://github.com/josers18/Headless-JDO" "Horizon — headless banker UI"
    click Sim "https://github.com/josers18/Salesforce-Data360-Financial-Transaction-Simulator" "Financial transaction simulator"
    click Token "https://github.com/josers18/Token-Comparison-Tool" "Token Comparison Tool"
    click HostedMCP "https://github.com/josers18/Data360-Hosted-MCP" "Hosted Data 360 MCP server"
    click RefMCP "https://github.com/josers18/Salesforce-Data360-MCP" "Reference Data 360 MCP impl"
```

---

## 🛠️ Tech Stack

**Languages**

<p>
  <img src="https://skillicons.dev/icons?i=python,r,js,ts,bash,scala&theme=dark" />
</p>

**Data, ML & Analytics**

<p>
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/XGBoost-FF6600?style=flat-square&logoColor=white&label=XGBoost" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" />
  <img src="https://img.shields.io/badge/Dask-FC6E6B?style=flat-square&logoColor=white&label=Dask" />
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white" />
</p>

**AI & LLM Frameworks**

<p>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/Anthropic_Claude-D97757?style=flat-square&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logoColor=white&label=LangGraph" />
  <img src="https://img.shields.io/badge/MCP-000000?style=flat-square&logoColor=white&label=MCP" />
  <img src="https://img.shields.io/badge/Agentforce-00A1E0?style=flat-square&logo=salesforce&logoColor=white" />
  <img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/ChromaDB-FF6B6B?style=flat-square&logoColor=white&label=ChromaDB" />
  <img src="https://img.shields.io/badge/Pinecone-000000?style=flat-square&logoColor=white&label=Pinecone" />
</p>

**Cloud, Platforms & Databases**

<p>
  <img src="https://skillicons.dev/icons?i=aws,heroku,mongodb&theme=dark" />
  <img src="https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white" />
  <img src="https://img.shields.io/badge/Salesforce-00A1E0?style=flat-square&logo=salesforce&logoColor=white" />
  <img src="https://img.shields.io/badge/Data%20Cloud-00A1E0?style=flat-square&logo=salesforce&logoColor=white" />
  <img src="https://img.shields.io/badge/Tableau%20Next-E97627?style=flat-square&logo=tableau&logoColor=white" />
  <img src="https://img.shields.io/badge/Heroku%20Inference-430098?style=flat-square&logo=heroku&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache%20Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white" />
</p>

**Frontend & Web**

<p>
  <img src="https://skillicons.dev/icons?i=nextjs,react,tailwind,vercel&theme=dark" />
</p>

**Tools**

<p>
  <img src="https://skillicons.dev/icons?i=git,github,docker,linux,vscode,fastapi&theme=dark" />
  <img src="https://img.shields.io/badge/OAuth_2.1-EB5424?style=flat-square&logo=auth0&logoColor=white" />
  <img src="https://img.shields.io/badge/PKCE-4B32C3?style=flat-square&logoColor=white&label=PKCE" />
</p>

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://streak-stats.demolab.com?user=josers18&theme=tokyonight&hide_border=true&background=0D1117&stroke=29B5E8&ring=29B5E8&fire=FF6600&currStreakLabel=29B5E8&sideLabels=29B5E8" />
</p>

<p align="center">
  <img width="95%" src="https://github-readme-activity-graph.vercel.app/graph?username=josers18&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=29B5E8&line=29B5E8&point=FFFFFF" />
</p>

<!--
  Snake animation below is generated daily by .github/workflows/snake.yml
  and pushed to the `output` branch as an SVG. The README references it
  directly from this repo — no third-party render-time dependency.
-->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/josers18/josers18/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/josers18/josers18/output/github-snake.svg" />
    <img alt="GitHub contribution snake animation" src="https://raw.githubusercontent.com/josers18/josers18/output/github-snake.svg" />
  </picture>
</p>

---

## ✍️ Writing & Articles

> Published on [LinkedIn](https://www.linkedin.com/in/jsifontes/recent-activity/articles/) · More at [analyticsmadesimple.com](https://analyticsmadesimple.com)

### 📌 Featured Articles

<!-- TODO: replace these LinkedIn-articles-tab URLs with the real article permalinks -->

| Article | Date |
|---|---|
| [Data Clean Rooms: Navigating the Future of Privacy and Collaboration](https://www.linkedin.com/in/jsifontes/recent-activity/articles/) | Jan 2024 |
| [Data Governance 101](https://www.linkedin.com/in/jsifontes/recent-activity/articles/) | Nov 2023 |
| [ETL vs ELT & Beyond: Choosing Your Data Integration Approach](https://www.linkedin.com/in/jsifontes/recent-activity/articles/) | Sep 2023 |
| [Getting Up to Speed on Vector Databases](https://www.linkedin.com/in/jsifontes/recent-activity/articles/) | Sep 2023 |

### 📰 Latest from analyticsmadesimple.com

<!-- BLOG-POST-LIST:START -->- [Hosted open models vs download to your machine](https://analyticsmadesimple.com/tutorials/hosted-open-models-vs-download-to-your-machine/) <sub>(Aug 27, 2026)</sub>- [Grok models chooser: 4.5, 4.6, and when to switch](https://analyticsmadesimple.com/tutorials/grok-models-chooser-4-5-4-6/) <sub>(Aug 27, 2026)</sub>- [Definitions and metric specs](https://analyticsmadesimple.com/analytics/definitions-and-metric-specs/) <sub>(Aug 27, 2026)</sub>- [What is an embedding?](https://analyticsmadesimple.com/key-terms/what-is-an-embedding/) <sub>(Aug 27, 2026)</sub>- [What is a feature store?](https://analyticsmadesimple.com/key-terms/what-is-a-feature-store/) <sub>(Aug 27, 2026)</sub><!-- BLOG-POST-LIST:END -->

> _Auto-updated daily via [`blog-post-workflow`](https://github.com/gautamkrishnar/blog-post-workflow)._

---

## 🚀 Featured Projects

> A curated set of work focused on **Salesforce Data 360, Agentforce, and MCP**. Full repo list on [my GitHub](https://github.com/josers18?tab=repositories).

| Project | What it does |
|---|---|
| **[Horizon — Headless-JDO](https://github.com/josers18/Headless-JDO)** <br/> `TypeScript · Next.js · MCP · Claude` | Headless home page for the relationship banker. Claude Sonnet orchestrates Salesforce CRM, Data Cloud, and Tableau Next MCP servers behind a no-navigation, conversation-first UI. |
| **[Data360-Hosted-MCP](https://github.com/josers18/Data360-Hosted-MCP)** <br/> `JavaScript · Heroku · MCP` | Salesforce Data 360 / Data Cloud MCP server with **43 tools across 16 families** — Heroku-hosted, dual-transport (SSE + stdio), with read-only and destructive-action guardrails. |
| **[Salesforce-Data360-MCP](https://github.com/josers18/Salesforce-Data360-MCP)** <br/> `Python · MCP · ⭐ 1` | Quick-start setup and demo for implementing MCP against Salesforce Data 360 (Data Cloud) — the reference implementation for the hosted variant above. |
| **[Token-Comparison-Tool](https://github.com/josers18/Token-Comparison-Tool)** <br/> `Python · FastAPI · OAuth 2.1` | Benchmark token cost: Salesforce native (`sf` CLI) vs Salesforce-hosted MCP servers. OAuth 2.1 + PKCE, free-format prompts, PDF export. |
| **[Data360 Financial Transaction Simulator](https://github.com/josers18/Salesforce-Data360-Financial-Transaction-Simulator)** <br/> `Python · Snowflake · Data Cloud` | Financial transaction simulator with overdraft prevention, balance tracking, and Salesforce Data Cloud / Snowflake integration. |
| **[Salesforce](https://github.com/josers18/Salesforce)** <br/> `Python · ⭐ 5` | Long-running grab-bag of Salesforce-related code, snippets, and experiments — most-starred repo on this profile. |
| **[JDO — Jose's Demo Org](https://github.com/josers18/JDO)** <br/> `Salesforce DX · Apex · LWC` | Assets and Salesforce DX projects for demo orgs: LWCs, Apex, flows, docs, and related demos. |

<details>
<summary>📚 <b>Reference & Learning Repos</b> (click to expand)</summary>

| Project | What it does |
|---|---|
| **[LangChain-Concepts](https://github.com/josers18/LangChain-Concepts)** | Reference guide for building LLM apps with LangChain — prompt templates, LCEL chains, agents, tools, RAG pipelines. |
| **[OpenAI-API-Tutorial](https://github.com/josers18/OpenAI-API-Tutorial)** | Reference guide for the OpenAI API, Hugging Face Transformers, embeddings, semantic search, ChromaDB, and Pinecone. |
| **[Python-Data-Structures](https://github.com/josers18/Python-Data-Structures)** | Personal reference for Python DS&A — Big O, linked lists, stacks, queues, trees, graphs, sorting, DP. |
| **[Python-Programming-Concepts](https://github.com/josers18/Python-Programming-Concepts)** | Reference guide for Python — OOP, error handling, testing with pytest and unittest. |
| **[Git-Tutorial](https://github.com/josers18/Git-Tutorial)** | Personal Git reference — init, branching, merging, remotes, stashing, tags. |

</details>

---

## 🎓 Education & Certifications

> A selection of credentials. Full list on [LinkedIn](https://www.linkedin.com/in/jsifontes).

**🎓 Education**

| Credential | Issuer |
|---|---|
| M.S. Data Science | Northwestern University |
| M.S. Data Engineering | Western Governors University |

**📊 Data, Analytics & AI**

| Credential | Issuer |
|---|---|
| Google Analytics Individual Qualification | Google |
| Data Scientist with R | DataCamp |
| Data Analyst with R | DataCamp |
| R Programming in Data Science: High Volume Data | LinkedIn Learning |

<details>
<summary>🛠️ <b>IT & Infrastructure Foundations</b> (click to expand)</summary>

| Credential | Issuer |
|---|---|
| MCP — Microsoft Certified Professional | Microsoft |
| MCTS — Windows 7 | Microsoft |
| Exam 413: Designing & Implementing Server Infrastructure | Microsoft |
| IT Operations Specialist | CompTIA |
| A+ | CompTIA |
| Network+ | CompTIA |

</details>

---

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:00A1E0,50:29B5E8,100:0062CC&height=120&section=footer" />
