# Welcome to my GitHub!

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/juanmcalderon/)
[![Personal Website](https://img.shields.io/badge/GitHub-%23121011.svg?logo=github&logoColor=white)](https://juancal28.github.io)

## About Me

- **EECS & Mathematics student at UC Berkeley** (Class of 2028)
- **Former Software Engineer Intern at Microsoft** (Summer 2026) — built centralized OpenTelemetry + Azure Application Insights telemetry across 6 internal AI services, cross-service correctness gates for Model Context Protocol (MCP) workflows, and LLM evaluation infrastructure with QoS dashboards used by senior leadership
- **Former SDE Intern at AWS on the SageMaker team** (Summer 2025) — built CI/CD pipelines for ECS Fargate services, developed RAG agents over 100,000+ entry S3 buckets on SageMaker Unified Studio, and coordinated a team of 6 interns on a multi-agent application
- **Published researcher** — automated a molecular docking pipeline at Emory University that scaled to 2,000,000+ molecules on HPC clusters, leading to a peer-reviewed paper and a US patent on RNA polymerase inhibitory compounds
- Interested in **quantitative trading, distributed systems, and AI infrastructure**, and the mathematics behind them

## Projects

### [NBA Live-Game Trading Bot on Polymarket](https://github.com/juancal28/nba-total-score-bot)
A live NBA over/under trading bot written in Rust that trades on Polymarket's CLOB. It fits a Poisson process to first-quarter scoring via MLE, validates rate stability with a two-sample likelihood-ratio test, and bootstraps a 95% CI on the projected total to size edge against market-implied probability. Execution runs on a multi-threaded tokio runtime with lock-free order-book snapshots from CLOB WebSockets, VWAP slippage and staleness checks, EIP-712-signed FOK orders, and redb-persisted idempotent order IDs for crash-safe restarts. Risk controls include position caps, daily-loss limits, a blowout filter, and a feed-gap kill switch.

**Tech:** Rust, tokio, WebSockets, Polymarket CLOB, SportRadar, redb

### [News-Based, RAG-Assisted Trading System](https://github.com/juancal28/quantAlgoV1)
An autonomous pipeline that ingests financial news, scores sentiment with FinBERT, embeds articles into Qdrant, and generates RAG-based strategy proposals gated behind dual-window backtesting (252-day in-sample + 90-day out-of-sample), lookahead-bias guards, and human-in-the-loop approval. A $100K paper trading layer uses cross-sectional sentiment signals, VIX volatility gating, and 10% per-position caps. The hot-path execution code (backtest engine, cost model, broker, risk checks) is compiled to C++ via pybind11/CMake and validated by 24 parity tests against the Python reference implementations.

**Tech:** Python, C++, pybind11, FastAPI, Celery, Redis, PostgreSQL, Qdrant, FinBERT, Anthropic Claude, Alpaca API

### Homely — Home Services Marketplace
A dual-sided marketplace connecting homeowners with trade professionals, built on React 19 + Express with JWT auth, role-based access control, and real-time messaging, and shipped as a cross-platform PWA with CI/CD via GitHub Actions and Railway. Features a RAG-powered AI advisor (LangChain, Claude) and an MCP server that drives agentic workflows for contractor matching, job discovery, and scheduling.

**Tech:** TypeScript, React, Node.js, Express, PostgreSQL, Tailwind CSS, LangChain, Anthropic Claude, MCP, Railway

## Awards & Honors

- Jane Street FOCUS program participant (1 of ~40)
- Gates Scholarship recipient (1 of 750)
- Microsoft HOLA Scholarship recipient (1 of 13)
- Amazon Future Engineer Scholarship recipient (1 of 400)
- Top 5% on the 2024 AMC 12B

## Publications

- Xu, E., Park, S., **Calderon, J.**, et al. (2023). [In Silico Identification and In Vitro Validation of Repurposed Compounds Targeting the RSV Polymerase](https://doi.org/10.3390/microorganisms11061608). *Microorganisms*, 11(6), 1608.
- US Patent [20240415923 A1](https://patents.google.com/patent/US20240415923A1) — "RNA-Dependent RNA Polymerase Inhibitory Compounds" (Emory University, 2024)

## Tech Stack

### Languages
![Java](https://img.shields.io/badge/-Java-007396?style=flat&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/-Rust-000000?style=flat&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/-C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![C](https://img.shields.io/badge/-C-A8B9CC?style=flat&logo=c&logoColor=black)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![SQL](https://img.shields.io/badge/-SQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/-Bash-4EAA25?style=flat&logo=gnubash&logoColor=white)
![RISC--V](https://img.shields.io/badge/-RISC--V-283272?style=flat&logo=riscv&logoColor=white)

### Frameworks & Libraries
![React](https://img.shields.io/badge/-React-61DAFB?style=flat&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Express](https://img.shields.io/badge/-Express-000000?style=flat&logo=express&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/-Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)
![Vite](https://img.shields.io/badge/-Vite-646CFF?style=flat&logo=vite&logoColor=white)
![Celery](https://img.shields.io/badge/-Celery-37814A?style=flat&logo=celery&logoColor=white)
![LangChain](https://img.shields.io/badge/-LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/-LangGraph-1C3C3C?style=flat&logo=langchain&logoColor=white)
![Tokio](https://img.shields.io/badge/-Tokio-000000?style=flat&logo=rust&logoColor=white)
![pybind11](https://img.shields.io/badge/-pybind11-00599C?style=flat&logo=cplusplus&logoColor=white)

### Tools & Platforms
![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/-Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/-OpenTelemetry-000000?style=flat&logo=opentelemetry&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Grafana](https://img.shields.io/badge/-Grafana-F46800?style=flat&logo=grafana&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Qdrant](https://img.shields.io/badge/-Qdrant-24386C?style=flat&logo=qdrant&logoColor=white)
![Railway](https://img.shields.io/badge/-Railway-0B0D0E?style=flat&logo=railway&logoColor=white)
![Cloudinary](https://img.shields.io/badge/-Cloudinary-3448C5?style=flat&logo=cloudinary&logoColor=white)

## GitHub Stats

<p align="center">
  <img src="profile-summary-card-output/tokyonight/0-profile-details.svg" alt="Profile Details" />
  <br/>
  <img src="profile-summary-card-output/tokyonight/1-repos-per-language.svg" alt="Repos Per Language" />
  <img src="profile-summary-card-output/tokyonight/2-most-commit-language.svg" alt="Most Commit Language" />
  <br/>
  <img src="profile-summary-card-output/tokyonight/3-stats.svg" alt="GitHub Stats" />
  <br/>
  <img src="https://streak-stats.demolab.com/?user=juancal28&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>
