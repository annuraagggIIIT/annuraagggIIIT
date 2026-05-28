<h1 align="center">Anurag Khanna</h1>
<h3 align="center">Founding Software Engineer · Distributed Systems · Backend Infrastructure</h3>

<p align="center">
  <a href="https://twitter.com/annuraaggg"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=flat&logo=twitter&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/anuragkhannaiiitm"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" /></a>
  <a href="https://anuragiiit.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-000000?style=flat&logo=vercel&logoColor=white" /></a>
  <a href="https://www.leetcode.com/anuragkhanna"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=flat&logo=leetcode&logoColor=black" /></a>
  <img src="https://komarev.com/ghpvc/?username=annuraagggiiit&style=flat&color=0e75b6" />
</p>

---

### About

Backend engineer focused on distributed systems and high-throughput infrastructure. Currently **Founding Software Engineer at Openleaf** (Mumbai), where I design and ship production systems across logistics, e-commerce, and AI/LLM integrations.

- Building on a **322-table PostgreSQL schema** serving 13+ carriers, 9+ e-commerce channels, and 5 WMS integrations
- Shipped systems processing millions of events: **BullMQ concurrency=128**, AWS SQS FIFO, Redis multi-tier caching
- Integrated LLMs (Google Gemini, Claude 3.5 Sonnet) into production document intelligence and B2B automation pipelines
- **ICPC Asia Taiwan 2024** — India Rank 3, Asia Rank 99

---

### Experience

| Role | Company | Period |
|---|---|---|
| Founding Software Engineer | Openleaf | Apr 2026 – Present |
| Software Engineer I | Facilgo (Anukta) | Dec 2024 – Apr 2026 |
| Software Engineer Intern | Maroon | Jul 2024 – Jan 2025 |
| Software Engineer Intern | Airtel (Wynk Music) | Jun 2024 – Aug 2024 |
| Blockchain Engineer Intern | SkyTrade | Jan 2024 – Dec 2024 |

---

### What I've Built

**Carrier Pricing Engine** — Go · PostgreSQL  
Hierarchical lookup across warehouse → pincode → city → zone → state → region with 40+ charge types, bidirectional route matching, and carrier-specific volumetric divisors.

**LLM Document Intelligence Pipeline** — Google Gemini · Claude 3.5 Sonnet · IMAP · Focus8 ERP  
Ingests POs, GRNs, and invoices from email; classifies document type, extracts SKU tables from multi-page XLSX with zero-tolerance PO number accuracy, and syncs to ERP. Separate Claude integration with prompt caching resolves ambiguous B2B customer mappings via streaming API + exponential backoff.

**32-Carrier Shipment Tracking System** — BullMQ · Redis · Node.js  
Two-tier Redis cache (1h config TTL / 7-day immutable field TTL) eliminating 2 serial DB round-trips per job tick. Parallelised 4 terminal-state writes with `Promise.all` saving ~7ms/job. 13-carrier NDR workflows integrated with Bitespeed, Contlo, ElasticRun, SagePilot.

**Shopify Order Ingestion Service** — Go · AWS SQS FIFO · PostgreSQL  
Exactly-once delivery via FIFO queues between webhook producer and order consumer. Replaced N+1 image cache lookups with batch queries, converted O(n²) tag-matching to O(n+m) map lookup, singleton S3 client via `sync.Once`, PG connection pool (25 open / 10 idle / 5-min lifetime).

**Playwright RPA Service** — Go · PostgreSQL  
Automates Blinkit PartnersBiz hyperlocal scheduling — OTP-authenticated sessions, cookie/localStorage persistence, environment-driven CSS selector overrides. Migrated Socket.IO cluster adapter from redis-adapter (PSUBSCRIBE) to redis-streams-adapter for AWS ElastiCache Serverless.

**AI Voice Agent** — Python · Twilio · Google Cloud STT · Gemini · ElevenLabs  
Async NDR re-attempt call pipeline with FFmpeg audio encoding, Prometheus metrics, and a no-action-taken guard preventing premature RTO classification.

**Orchestr** — React 19 · Express 5 · TypeScript · Prisma · MySQL · BullMQ  
Full-stack e-commerce platform following the Saga pattern. Real-time Tally ERP sync via XML-over-HTTP. Razorpay payment gateway, Pino structured logging, admin dashboard.

---

### Tech Stack

**Languages**

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)

**Backend & Infrastructure**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)
![Gin](https://img.shields.io/badge/Gin-00ADD8?style=flat&logo=go&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-FF4444?style=flat&logo=redis&logoColor=white)
![AWS SQS](https://img.shields.io/badge/AWS_SQS-FF9900?style=flat&logo=amazonaws&logoColor=white)
![AWS S3](https://img.shields.io/badge/AWS_S3-569A31?style=flat&logo=amazons3&logoColor=white)

**Databases & Caching**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat&logo=elasticsearch&logoColor=white)

**Observability & DevOps**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![DataDog](https://img.shields.io/badge/DataDog-632CA6?style=flat&logo=datadog&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=flat&logo=sentry&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat&logo=tailwindcss&logoColor=white)

---

### Achievements

- **ICPC Asia Taiwan 2024** — India Rank 3, Asia Rank 99
- **IIIT'M Tech Fest Hackathon** — 1st Place (Apr 2024)
- **ETHGlobal Frameworks Hackathon** — Privy.io Honourable Mention (Mar 2024)
- **SuperTeam.fun** — $750 grant for blockchain project (Mar 2024)

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=annuraagggiiit&show_icons=true&theme=dark&hide_border=true&count_private=true" height="150"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=annuraagggiiit&layout=compact&theme=dark&hide_border=true" height="150"/>
</p>
<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=annuraagggiiit&theme=dark&hide_border=true" />
</p>
