
![Hello Myself,Subhranshu](https://github.com/CantBeSubh/CantBeSubh/assets/83113185/cadf7712-af12-4f6d-a1a1-8993700cb002)

<p align='center'>
	🌐 Portfolio
	<br/>
	https://subhranshu.com
	<br/><br/>
	📎 Resume
	<br/>
	<a href="https://dub.subhranshu.com/Resume">Subhranshu's Resume 2026</a>
	<br/><br/>
	🤝 Hire me
	<br/>
	<a href="mailto:work.suhbranshu@gmail.com">work.suhbranshu@gmail.com</a>
</p>

<h1 align='center'>✨whoami</h1> 

<p>
<a  href="#">
	<img width="30%" align="right" alt="Github Image" src="https://github.com/CantBeSubh/CantBeSubh/blob/main/assets/undraw_code_thinking_re_gka2.svg" '/>
</a>
	
▸ Hello! Myself Subhranshu.

▸ **AI & Backend Engineer** specializing in production LLM systems — multi-agent orchestration, RAG, semantic search, MLOps, LLMOps — and the high-throughput, distributed **Python** backend services & data pipelines that run them at scale.

▸ As the **founding software engineer** at an AI startup, I owned architecture and delivery across the stack, building POCs and systems that scale with both users and ambition, with stakeholder communication and user thinking. My work helped us raise a **$4M seed round**, and land partnerships with **NVIDIA**, **Microsoft** and **Accenture**.

▸ Roles I'm interested in — AI Engineer, GenAI Engineer, Backend Engineer, Fullstack Engineer, Product Engineer

▸ Currently pursuing a part-time **MS in Computer Science at Georgia Tech (OMSCS)**.

▸ Technologies:
- **GenAI**: LangChain, LangGraph, LangSmith, RAG, Multi-Agent Systems, Semantic/Hybrid Search, Reranking, LLM Evaluation, OpenAI, Anthropic, Vertex AI, Azure AI Foundry
- **Backend**: Python, FastAPI, REST, SSE, WebSockets, Airflow, Celery, Microservices
- **Databases**: PostgreSQL, MongoDB, Redis, Neo4j, OpenSearch, Milvus, Pinecone, Supabase
- **Cloud & DevOps**: GCP, Azure, Docker, Kubernetes, Terraform, ArgoCD, GitHub Actions, Helm
- **Frontend**: TypeScript, React, Next.js, Redux Toolkit, React Query, TailwindCSS, Shadcn
- **Observability & Testing**: OpenTelemetry, Prometheus, Grafana, LangSmith, Sentry, Playwright, Pytest

▸ Resume: https://dub.subhranshu.com/Resume

▸ Portfolio: https://subhranshu.com/

▸ LinkedIn: [LinkedIn/subhranshu-pati](https://www.linkedin.com/in/subhranshu-pati/)

▸ Email: [work.suhbranshu@gmail.com](mailto:work.suhbranshu@gmail.com)

</p>

<h1 align='center'>🛠 What I've Built</h1>

### FOUNDING SOFTWARE ENGINEER — [Everstar](https://everstar.ai) · NY, USA (Remote) · Aug 2024 – Jun 2026

An agentic RAG platform for **nuclear regulatory compliance** — from the idea stage, through a [**$4M seed**](https://www.prnewswire.com/news-releases/everstar-secures-4m-in-pre-seed-funding-to-revolutionize-nuclear-compliance-with-ai-302379015.html), into **Prometheus**, a **$60M DOE Genesis Mission Phase II** program with Idaho National Laboratory.

- Architected and shipped a production **Multi-Agent RAG system** with a knowledge base of **10M+ PDF files**, using **LangGraph** & **LangChain**, that reduced nuclear compliance drafting **from weeks to hours**, using Claude Opus for the agent and Claude Sonnet/Haiku for sub-agents/tasks.
- Designed the Agent Layer: **hallucination guardrails**, routing, handoff, parallelism, **human-in-the-loop**, **agent memory** (both long and short-term), **reflection loop** and **error recovery**, token budgeting, **prompt caching**, resulting in generation of reliable and accurate citation-backed regulatory documents (1,000+ pages).
- Drove a **Search Engine** overhaul, implementing **Hybrid Search** (BM25 + Vector Search + RRF) using **OpenSearch**, that reduced retrieval from 3-4s to **under 200ms**, without any compromise in accuracy, by using **Cohere Rerank**, combining sparse & dense vectors and metadata pre-filtering.
- Owned the **Document Ingestion Pipeline** end-to-end using **Airflow** hosted on **GCP**, so customers could onboard **terabytes** of data without losing records or needing engineers to babysit failures.
- Delivered a secure, highly available, scalable **REST Backend** using **Python FastAPI** with SSE and **Redis** Caching and Streaming, that preserved user's progress, in case they disconnected in middle of agent's answer streaming.
- Established an **MLOps** pipeline to train & deploy a **YOLO model** for circuit diagram extraction, using **Roboflow**, **Vertex AI**, and **Weights & Biases**, auto-validating newer model against the older deployment, preventing regression.
- Introduced a **LLM-as-judge Evaluation Framework** for our Agent, using **LangSmith**, comparing any new changes to the Agent against a golden dataset, to evaluate — faithfulness, helpfulness, correctness and relevance, that ensured changes were non-regressive and followed **TDD** approach.
- Led the **CI/CD** buildout with **GitHub Actions** and **ArgoCD** on **GKE**, deploying **MongoDB**, **OpenSearch**, our backend, and **Airflow** on **Docker** & **Kubernetes** for scale, with **Terraform** for IaC, auto-deploying every code change with zero downtime and one-click rollback if a release fails.
- Engineered **Custom Extraction and Chunking Systems**, with image extraction, table structure parsing using **NumPy**, and contextual chunking, and using **OpenAI's `text-embedding-3-small`**, eliminating the information loss that drives most wrong answers downstream.
- Ensured reliability of production AI systems through end-to-end tracing in **LangSmith**, plus **OpenTelemetry**, **Prometheus**, and **Grafana** observability (LLMOps).

### PRODUCT ENGINEER INTERN — [Ethica](https://heyethica.com) · SF, USA (Remote) · Sept 2023 – May 2024

- Built a production grade Home Search Platform that processed voice described lifestyle preferences into structured search criteria, scaling relevance based ranking across **50,000+ property listings**, using **Pinecone Vector Database** and **LangChain** for the Voice Chatbot.

<h1 align='center'>🚀 Projects</h1>

### [Wizz AI](https://wizz.subhranshu.com) — Multi-Tenant RAG Chatbot SaaS

- Embeddable citation-grounded **RAG** chatbot with per-tenant **Milvus Vector DB** isolation, event-driven **Celery** ingestion, and an async **FastAPI** backend with **SSE** streaming.
- Isolation is physical, not a `WHERE tenant_id = ?` — every tenant gets their own collection, making a cross-tenant leak **structurally impossible** instead of conditionally prevented.

### [Homelab](https://github.com/CantBeSubh/homelab) — MCP Server & Self-Hosted Infrastructure

- **MCP** server exposing a self-hosted **Proxmox** homelab to Claude: Home Assistant control, domain-scoped sub-servers, **STDIO** bridged to remote **HTTP**, using **FastMCP**.
- **CasaOS** + **Portainer** running open-source replacements for iCloud, Google Suite, S3 and Bitwarden, public surface via **Cloudflare Tunnel**, private access over **Tailscale**, and **zero open inbound ports**.

### Second Brain — AI-first Personal OS *(in progress)*

- A composable skills layer on top of **Obsidian** that holds projects, goals and habits in context and **acts** on them, built with **Claude Code** — not a to-do app with an LLM stapled on.

<h1 align='center'>⚙Technical Skills </h1>

<p align='center'>
	<b>GenAI</b>
<br>
	<img src='https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54'/>
	<img src='https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white'/>
	<img src='https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logoColor=white'/>
	<img src='https://img.shields.io/badge/Anthropic-191919?style=for-the-badge&logo=anthropic&logoColor=white'/>
	<img src='https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black'/>
<br><br>
	<b>Backend & Data</b>
<br>
	<img src='https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi&logoColor=white'/>
	<img src='https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white'/>
	<img src='https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white'/>
	<img src='https://img.shields.io/badge/OpenSearch-005EB8?style=for-the-badge&logo=opensearch&logoColor=white'/>
<br>
	<img src='https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white'/>
	<img src='https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white'/>
	<img src='https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white'/>
	<img src='https://img.shields.io/badge/Neo4j-4581C3?style=for-the-badge&logo=neo4j&logoColor=white'/>
<br><br>
	<b>Cloud & DevOps</b>
<br>
	<img src='https://img.shields.io/badge/Google%20Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white'/>
	<img src='https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logoColor=white'/>
	<img src='https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white'/>
	<img src='https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white'/>
<br>
	<img src='https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white'/>
	<img src='https://img.shields.io/badge/Argo%20CD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white'/>
	<img src='https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white'/>
<br><br>
	<b>Frontend</b>
<br>
	<img src='https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white'/>
	<img src='https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB'/>
	<img src='https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white'/>
	<img src='https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white'/>
<br><br>
	<b>Observability & Testing</b>
<br>
	<img src='https://img.shields.io/badge/OpenTelemetry-000000?style=for-the-badge&logo=opentelemetry&logoColor=white'/>
	<img src='https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white'/>
	<img src='https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white'/>
	<img src='https://img.shields.io/badge/Sentry-362D59?style=for-the-badge&logo=sentry&logoColor=white'/>
	<img src='https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logoColor=white'/>
	<img src='https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white'/>
</p>

<h1 align='center'>📊Github Stats</h1> 

<img src='https://github.com/CantBeSubh/CantBeSubh/blob/main/assets/undraw_version_control_re_mg66.svg' align='right' width='40%'/>

<p align='center'><img src='https://github-readme-stats.vercel.app/api/top-langs/?username=CantBeSubh&&theme=dracula&hide=lua,assembly,Jupyter+Notebook' align='center'/></p>

<br>

<p align='center'><img src='https://github-readme-stats.vercel.app/api/?username=CantBeSubh&theme=dracula&show_icons=true' align='center'/></p>

<br>

<p align='center'><img src='https://github-profile-trophy.vercel.app/?username=CantBeSubh&theme=dracula&row=1&column=6' align='center'/></p>

<br>

<p align='center'><img align="center" src="https://github.com/CantBeSubh/CantBeSubh/blob/output/github-contribution-grid-snake-dark.svg" /></p>
		 


<p align='center'></p>
		 
<br>
																	       
<h1 align='center'>🎮 Hobbies</h1>

- Video Games(Multiplayer FPS, RPG, 3D/2D Platform)

- Music(Old School Hip-hop, Dubstep, City Pop, Jazz, Future Bass)

- Video Editing and 3D Modelling(Blender,Davichi Resolve)

- Reading(Sci-Fi, Autobiography)

<p align='center'>
<a href='https://open.spotify.com/user/57dordqsbmjjihsqd6xwt9hg4'><img src='https://novatorem-rho-ten.vercel.app/api/spotify'/></a>
</p>


<h1 align='center'>🌐Socials </h1>

<p align='center'>
	<a href='https://linktr.ee/CantBeSubh'>LinkTree</a>
	<br> 
	<a href='https://subhranshu.com/'>Portfolio</a>
	<br> 
	<a href='https://twitter.com/cantbesubh'>Twitter</a>
	<br> 
	<a href='https://www.linkedin.com/in/subhranshu-pati/'>LinkedIn</a>
</p>
