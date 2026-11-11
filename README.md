# Warplogic AI — Open-Source AI Coding Rules & Blueprints

> A curated, battle-tested collection of **89+ production-grade system rules** for **Cursor (.mdc)**, **Anthropic Claude Code (CLAUDE.md)**, **AGENTS.md**, **GitHub Copilot**, and **Windsurf**.

[![License: MIT](https://img.shields.io/badge/License-MIT-emerald.svg)](LICENSE)
[![Rules Count: 89+](https://img.shields.io/badge/Rules-89%2B%20Verified-blue.svg)](https://www.warplogicai.com/prompts)
[![Web Directory](https://img.shields.io/badge/Web-warplogicai.com-cyan.svg)](https://www.warplogicai.com)

---

## ⚡ Instant 1-Click Pull (Zero Setup)

Download and install any rule directly into your project using `curl`:

```bash
# 1. Cursor IDE (.cursor/rules/*.mdc)
mkdir -p .cursor/rules && curl -sL "https://www.warplogicai.com/api/v1/prompts/nextjs-14-15-app-router-cursorrules/raw?tool=cursor" -o .cursor/rules/nextjs-rules.mdc

# 2. Anthropic Claude Code (CLAUDE.md)
curl -sL "https://www.warplogicai.com/api/v1/prompts/python-fastapi-pydantic-cursorrules/raw?tool=claude" >> CLAUDE.md

# 3. AGENTS.md Standard (Codex, Devin, Jules, Amp)
curl -sL "https://www.warplogicai.com/api/v1/prompts/supabase-pgvector-vector-search-cursorrules/raw?tool=agents" >> AGENTS.md

# 4. GitHub Copilot (.github/copilot-instructions.md)
mkdir -p .github && curl -sL "https://www.warplogicai.com/api/v1/prompts/docker-compose-production-hardening-cursorrules/raw?tool=copilot" >> .github/copilot-instructions.md
```

---

## 🎛️ Interactive Stack Rule Builder & Linter

Instead of managing static files by hand, use the free in-browser tools on Warplogic AI:

- 🛠️ **[Interactive AI Stack Rule Builder](https://www.warplogicai.com/builder)**: Select your framework (Next.js 15, FastAPI, SvelteKit, Go, Rust), database (Supabase, Neon, Prisma, Drizzle), and security guardrails to generate a unified, production-ready rule in 1 click.
- 🔍 **[AI Rule Linter & Security Auditor](https://www.warplogicai.com/linter)**: Paste your existing prompt to scan for token bloat, leaked API secrets, and conflicting negative constraints with 1-click auto-fix.

---

## 📚 Complete Rules Catalog (89 Blueprints)

### 📦 Backend Development (3)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Production Cursor Rules for Python FastAPI & Pydantic v2**](rules/python-fastapi-pydantic-cursorrules.md) | `FastAPI` | `npx warplogic add python-fastapi-pydantic-cursorrules` |
| [**Cursor Rules for Django Ninja & OpenAPI Schema Design**](rules/django-ninja-cursorrules.md) | `Django Ninja` | `npx warplogic add django-ninja-cursorrules` |
| [**Cursor Rules for Flask Application Factory & Flask-SQLAlchemy**](rules/flask-factory-sqlalchemy-cursorrules.md) | `Flask` | `npx warplogic add flask-factory-sqlalchemy-cursorrules` |

### 📦 Testing & QA (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Pytest, Asyncio & FastAPI Test Coverage**](rules/pytest-asyncio-fastapi-cursorrules.md) | `Pytest / FastAPI` | `npx warplogic add pytest-asyncio-fastapi-cursorrules` |

### 📦 Data Engineering (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Advanced Pydantic v2 Custom Validators & Serialization**](rules/pydantic-v2-data-validation-cursorrules.md) | `Pydantic v2` | `npx warplogic add pydantic-v2-data-validation-cursorrules` |

### 📦 Database & ORM (2)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for SQLAlchemy 2.0 Async Session & Repository Pattern**](rules/sqlalchemy-2-async-orm-cursorrules.md) | `SQLAlchemy 2.0` | `npx warplogic add sqlalchemy-2-async-orm-cursorrules` |
| [**Cursor Rules for High-Performance Asyncpg & PostgreSQL Query Pooling**](rules/asyncpg-postgres-raw-sql-cursorrules.md) | `Asyncpg` | `npx warplogic add asyncpg-postgres-raw-sql-cursorrules` |

### 📦 Distributed Systems (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Celery & Redis Asynchronous Task Queues**](rules/celery-redis-background-tasks-cursorrules.md) | `Celery / Redis` | `npx warplogic add celery-redis-background-tasks-cursorrules` |

### 📦 DevOps & Tools (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Poetry Dependency Management & Packaging**](rules/poetry-python-packaging-cursorrules.md) | `Poetry` | `npx warplogic add poetry-python-packaging-cursorrules` |

### 📦 DevOps & Infra (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Multi-Stage Docker & Compose Python Deployments**](rules/docker-python-fastapi-cursorrules.md) | `Docker / Compose` | `npx warplogic add docker-python-fastapi-cursorrules` |

### 📦 Frontend Architecture (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Next.js App Router, React 19 & Tailwind CSS v4 Cursor Rules**](rules/nextjs-14-15-app-router-cursorrules.md) | `Next.js (App Router)` | `npx warplogic add nextjs-14-15-app-router-cursorrules` |

### 📦 Form Handling & Validation (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**React Hook Form, Zod v3 & Type-Safe Validation Cursor Rules**](rules/react-hook-form-zod-cursorrules.md) | `React 19 / Next.js` | `npx warplogic add react-hook-form-zod-cursorrules` |

### 📦 UI Design System (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Shadcn UI, Radix Primitives & Tailwind CSS v4 Cursor Rules**](rules/shadcn-ui-tailwind-cursorrules.md) | `Tailwind / Shadcn UI` | `npx warplogic add shadcn-ui-tailwind-cursorrules` |

### 📦 Global State Management (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Zustand State Management & Slice Pattern Cursor Rules**](rules/zustand-react-state-cursorrules.md) | `Zustand / React` | `npx warplogic add zustand-react-state-cursorrules` |

### 📦 Server State Management (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**TanStack React Query v5 & Async Data Fetching Cursor Rules**](rules/tanstack-react-query-cursorrules.md) | `TanStack Query` | `npx warplogic add tanstack-react-query-cursorrules` |

### 📦 Cloud & DevOps (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Docker Multi-Stage Builds & Python Security**](rules/docker-multi-stage-python-cursorrules.md) | `Docker / Docker Compose v2` | `npx warplogic add docker-multi-stage-python-cursorrules` |

### 📦 Infrastructure as Code (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Terraform AWS Infrastructure as Code**](rules/terraform-aws-infrastructure-cursorrules.md) | `Terraform 1.8+ / AWS` | `npx warplogic add terraform-aws-infrastructure-cursorrules` |

### 📦 Database Architecture (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for PostgreSQL Indexing & Prisma Migrations**](rules/postgresql-prisma-cursorrules.md) | `PostgreSQL 16 / Prisma ORM` | `npx warplogic add postgresql-prisma-cursorrules` |

### 📦 Distributed Systems & Cache (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Redis Caching & Sliding Window Rate Limiting**](rules/redis-cache-ratelimit-cursorrules.md) | `Redis 7` | `npx warplogic add redis-cache-ratelimit-cursorrules` |

### 📦 DevOps & Security (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for GitHub Actions CI/CD Pipeline Hardening**](rules/github-actions-cicd-cursorrules.md) | `GitHub Actions` | `npx warplogic add github-actions-cicd-cursorrules` |

### 📦 Backend API (2)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Node.js Express & TypeScript**](rules/node-express-typescript-cursorrules.md) | `Express.js` | `npx warplogic add node-express-typescript-cursorrules` |
| [**Cursor Rules for NestJS Enterprise Architecture & DI**](rules/nestjs-architecture-di-cursorrules.md) | `NestJS` | `npx warplogic add nestjs-architecture-di-cursorrules` |

### 📦 Database Access (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Prisma ORM & Type-Safe Database Queries**](rules/prisma-orm-typescript-cursorrules.md) | `Prisma ORM` | `npx warplogic add prisma-orm-typescript-cursorrules` |

### 📦 Data Validation (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for Zod Schema Validation & Inference**](rules/zod-validation-typescript-cursorrules.md) | `Zod` | `npx warplogic add zod-validation-typescript-cursorrules` |

### 📦 API Protocol (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Cursor Rules for tRPC End-to-End Type-Safe APIs**](rules/trpc-type-safe-api-cursorrules.md) | `tRPC` | `npx warplogic add trpc-type-safe-api-cursorrules` |

### 📦 AI & Machine Learning (11)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Production Cursor Rules for LangChain & LangGraph Agents**](rules/langchain-python-agent-cursorrules.md) | `LangChain` | `npx warplogic add langchain-python-agent-cursorrules` |
| [**Cursor Rules for LlamaIndex RAG & VectorStore Pipelines**](rules/llamaindex-rag-vectorstore-cursorrules.md) | `LlamaIndex` | `npx warplogic add llamaindex-rag-vectorstore-cursorrules` |
| [**Cursor Rules for OpenAI SDK v4 & Structured Outputs**](rules/openai-sdk-v4-typescript-cursorrules.md) | `OpenAI SDK` | `npx warplogic add openai-sdk-v4-typescript-cursorrules` |
| [**Cursor Rules for Anthropic Claude SDK & Prompt Caching**](rules/anthropic-claude-sdk-cursorrules.md) | `Anthropic SDK` | `npx warplogic add anthropic-claude-sdk-cursorrules` |
| [**Cursor Rules for Pinecone Vector DB & Hybrid Search**](rules/pinecone-vector-database-cursorrules.md) | `Pinecone` | `npx warplogic add pinecone-vector-database-cursorrules` |
| [**Gemini 2.0 Multimodal Live API & WebRTC Streaming Rules**](rules/gemini-2-0-multimodal-live-api-cursorrules.md) | `Google GenAI SDK` | `npx warplogic add gemini-2-0-multimodal-live-api-cursorrules` |
| [**LangChain v0.3 & LangGraph Stateful Workflow Rules**](rules/langchain-v03-tool-calling-pydantic-cursorrules.md) | `LangChain v0.3` | `npx warplogic add langchain-v03-tool-calling-pydantic-cursorrules` |
| [**Supabase pgvector & Semantic Search .cursorrules**](rules/supabase-pgvector-embeddings-cursorrules.md) | `Supabase` | `npx warplogic add supabase-pgvector-embeddings-cursorrules` |
| [**Anthropic Claude 3.5 Sonnet Prompt Architecture .cursorrules**](rules/anthropic-claude-3-5-sonnet-prompt-engineering-cursorrules.md) | `Anthropic SDK` | `npx warplogic add anthropic-claude-3-5-sonnet-prompt-engineering-cursorrules` |
| [**OpenAI o3-mini & Reasoning Models .cursorrules**](rules/openai-o3-mini-reasoning-sdk-cursorrules.md) | `OpenAI SDK` | `npx warplogic add openai-o3-mini-reasoning-sdk-cursorrules` |
| [**LangGraph Multi-Agent Architecture .cursorrules**](rules/langchain-langgraph-multi-agent-cursorrules.md) | `LangGraph` | `npx warplogic add langchain-langgraph-multi-agent-cursorrules` |

### 📦 LLM System Prompts (6)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Claude 3.5 Sonnet Chain-of-Thought (CoT) & Prompt Caching Rules**](rules/claude-3-5-sonnet-chain-of-thought-prompting.md) | `Anthropic Claude 3.5` | `npx warplogic add claude-3-5-sonnet-chain-of-thought-prompting` |
| [**OpenAI GPT-4o Strict Structured Outputs & JSON Schema Rules**](rules/openai-gpt4o-structured-outputs-json-schema.md) | `OpenAI API` | `npx warplogic add openai-gpt4o-structured-outputs-json-schema` |
| [**LangGraph Multi-Agent Orchestrator & State Management Rules**](rules/langgraph-multi-agent-orchestrator-cursorrules.md) | `LangGraph` | `npx warplogic add langgraph-multi-agent-orchestrator-cursorrules` |
| [**Llama 3.3 Local Tool Calling & Function Execution Rules**](rules/llama-3-local-tool-calling-cursorrules.md) | `Llama 3 / Ollama` | `npx warplogic add llama-3-local-tool-calling-cursorrules` |
| [**Mistral Large 2 Automated Code Review & Security Audit Rules**](rules/mistral-large-code-review-audit-cursorrules.md) | `Mistral AI` | `npx warplogic add mistral-large-code-review-audit-cursorrules` |
| [**DeepSeek-R1 & V3 CoT Reasoning & Code Synthesis System Prompt**](rules/deepseek-v3-r1-reasoning-system-prompt.md) | `DeepSeek API` | `npx warplogic add deepseek-v3-r1-reasoning-system-prompt` |

### 📦 Database Engineering (5)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**PostgreSQL 16 JSONB & GIN Index Optimization Rules**](rules/postgresql-16-gin-jsonb-indexing-cursorrules.md) | `PostgreSQL 16` | `npx warplogic add postgresql-16-gin-jsonb-indexing-cursorrules` |
| [**Supabase & Postgres Row-Level Security (RLS) Multi-Tenant Rules**](rules/supabase-row-level-security-multi-tenant-cursorrules.md) | `Supabase / PostgreSQL` | `npx warplogic add supabase-row-level-security-multi-tenant-cursorrules` |
| [**Redis Lua Script Token-Bucket Rate Limiter & Sliding Window Rules**](rules/redis-token-bucket-rate-limiting-cursorrules.md) | `Redis / Upstash` | `npx warplogic add redis-token-bucket-rate-limiting-cursorrules` |
| [**Prisma ORM N+1 Query Prevention & Connection Tuning Rules**](rules/prisma-orm-performance-query-tuning-cursorrules.md) | `Prisma ORM` | `npx warplogic add prisma-orm-performance-query-tuning-cursorrules` |
| [**Drizzle ORM Lightweight Schema & Prepared Query Rules**](rules/drizzle-orm-relations-prepared-queries-cursorrules.md) | `Drizzle ORM` | `npx warplogic add drizzle-orm-relations-prepared-queries-cursorrules` |

### 📦 API Security & Auth (6)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**OAuth 2.1 PKCE Authorization Code Flow & Anti-CSRF Rules**](rules/oauth2-pkce-authorization-code-cursorrules.md) | `OAuth 2.1 / Web Security` | `npx warplogic add oauth2-pkce-authorization-code-cursorrules` |
| [**Asymmetric RS256/ES256 JWT Verification & Rotation Rules**](rules/jwt-asymmetric-rs256-rotation-cursorrules.md) | `Node.js / Express` | `npx warplogic add jwt-asymmetric-rs256-rotation-cursorrules` |
| [**HMAC SHA-256 Cryptographic Webhook Verifier Middleware Rules**](rules/express-hmac-sha256-webhook-verifier-cursorrules.md) | `Express.js / Node.js` | `npx warplogic add express-hmac-sha256-webhook-verifier-cursorrules` |
| [**Hashed API Key Authentication & Per-Tenant Rate Limiting Rules**](rules/api-key-rate-limited-middleware-cursorrules.md) | `Node.js / Express` | `npx warplogic add api-key-rate-limited-middleware-cursorrules` |
| [**Apollo GraphQL Federation v2 & Subgraph N+1 Rules**](rules/graphql-federation-apollo-subgraph-rules.md) | `Apollo Federation v2` | `npx warplogic add graphql-federation-apollo-subgraph-rules` |
| [**Express JWT Rotation & Middleware Rules**](rules/express-jwt-rotation-middleware-cursorrules.md) | `Express.js` | `npx warplogic add express-jwt-rotation-middleware-cursorrules` |

### 📦 Zero Trust Security (2)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**SPIFFE SVID mTLS 1.3 & Certificate SAN Validation Rules**](rules/spiffe-svid-mtls-san-validation-cursorrules.md) | `Envoy / SPIFFE` | `npx warplogic add spiffe-svid-mtls-san-validation-cursorrules` |
| [**Zero-Trust API Gateway mTLS & Envoy Sidecar Enforcement Rules**](rules/zerotrust-gateway-mTLS-cursorrules.md) | `Envoy Proxy v1.29+ / SPIFFE SPIRE` | `npx warplogic add zerotrust-gateway-mTLS-cursorrules` |

### 📦 Cloud Infrastructure (12)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Terraform AWS ECS Fargate Envoy Sidecar Module Rules**](rules/terraform-aws-ecs-fargate-envoy-cursorrules.md) | `Terraform / AWS ECS` | `npx warplogic add terraform-aws-ecs-fargate-envoy-cursorrules` |
| [**Docker Compose Production Security Hardening & Isolation Rules**](rules/docker-compose-production-hardening-cursorrules.md) | `Docker Compose` | `npx warplogic add docker-compose-production-hardening-cursorrules` |
| [**Cloudflare Workers & D1 Serverless SQL Edge Router Rules**](rules/cloudflare-workers-d1-edge-router-cursorrules.md) | `Cloudflare Workers` | `npx warplogic add cloudflare-workers-d1-edge-router-cursorrules` |
| [**Kubernetes Helm 3 Values Schema Validation & ArgoCD Rules**](rules/kubernetes-helm3-schema-validation-cursorrules.md) | `Kubernetes / Helm 3` | `npx warplogic add kubernetes-helm3-schema-validation-cursorrules` |
| [**GitHub Actions OIDC Passwordless AWS Deployment Pipeline Rules**](rules/github-actions-oidc-aws-deployment-cursorrules.md) | `GitHub Actions` | `npx warplogic add github-actions-oidc-aws-deployment-cursorrules` |
| [**Cloudflare D1 & Drizzle ORM Edge Database Rules**](rules/cloudflare-d1-drizzle-edge-orm-rules.md) | `Cloudflare Workers / Drizzle` | `npx warplogic add cloudflare-d1-drizzle-edge-orm-rules` |
| [**AWS Lambda Powertools TypeScript & Idempotency Rules**](rules/aws-lambda-powertools-typescript-cursorrules.md) | `AWS Lambda / Powertools` | `npx warplogic add aws-lambda-powertools-typescript-cursorrules` |
| [**Kubernetes KEDA v2 Event-Driven Autoscaling Rules**](rules/kubernetes-keda-event-driven-autoscaling.md) | `Kubernetes / KEDA` | `npx warplogic add kubernetes-keda-event-driven-autoscaling` |
| [**OpenTofu Multi-Region AWS VPC Peering & KMS Rules**](rules/opentofu-aws-multi-region-iac-rules.md) | `OpenTofu / Terraform` | `npx warplogic add opentofu-aws-multi-region-iac-rules` |
| [**AWS CDK v2 Serverless & Lambda Powertools .cursorrules**](rules/aws-cdk-v2-serverless-typescript-cursorrules.md) | `AWS CDK` | `npx warplogic add aws-cdk-v2-serverless-typescript-cursorrules` |
| [**Multi-Cloud Terraform AWS EKS & GCP GKE Federated Module Rules**](rules/multicloud-terraform-eks-gke-cursorrules.md) | `HashiCorp Terraform 1.8+` | `npx warplogic add multicloud-terraform-eks-gke-cursorrules` |
| [**Terraform AWS ECS Fargate Module Rules**](rules/terraform-aws-ecs-fargate-module-cursorrules.md) | `Terraform 1.8+ / AWS` | `npx warplogic add terraform-aws-ecs-fargate-module-cursorrules` |

### 📦 AI Automation (5)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**n8n AI Agent Node & LangChain Multi-Tool Routing Rules**](rules/n8n-langchain-ai-agent-workflow-rules.md) | `n8n / LangChain` | `npx warplogic add n8n-langchain-ai-agent-workflow-rules` |
| [**n8n Stripe Webhook & HubSpot Multi-Step Lead Routing Rules**](rules/n8n-webhook-hmac-stripe-hubspot-sync.md) | `n8n` | `npx warplogic add n8n-webhook-hmac-stripe-hubspot-sync` |
| [**Zapier & Make Webhook Payload Transformation & Error Handling Rules**](rules/zapier-make-webhook-transformation-cursorrules.md) | `Zapier / Make` | `npx warplogic add zapier-make-webhook-transformation-cursorrules` |
| [**n8n PostgreSQL pgvector RAG Embedding & Document Upsert Pipeline Rules**](rules/n8n-postgres-vector-rag-pipeline-rules.md) | `n8n / PostgreSQL` | `npx warplogic add n8n-postgres-vector-rag-pipeline-rules` |
| [**n8n Real-Time DevOps Incident Alert & Slack PagerDuty Triage Rules**](rules/n8n-slack-incident-pagerduty-alert-rules.md) | `n8n` | `npx warplogic add n8n-slack-incident-pagerduty-alert-rules` |

### 📦 Database Optimization (3)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**ClickHouse OLAP Columnar Time-Series Analytics Rules**](rules/clickhouse-olap-timeseries-analytics-rules.md) | `ClickHouse` | `npx warplogic add clickhouse-olap-timeseries-analytics-rules` |
| [**DuckDB-Wasm In-Browser Fast Analytical Parquet Rules**](rules/duckdb-wasm-in-browser-analytics-rules.md) | `DuckDB-Wasm` | `npx warplogic add duckdb-wasm-in-browser-analytics-rules` |
| [**MongoDB 7.0 Aggregation Pipeline & Compound Index Rules**](rules/mongo-aggregation-pipeline-index-tuning-rules.md) | `MongoDB 7.0` | `npx warplogic add mongo-aggregation-pipeline-index-tuning-rules` |

### 📦 DevOps & CI/CD (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**GitHub Actions Multi-Arch Docker Buildx & Cache Rules**](rules/github-actions-docker-buildx-cache-ci-rules.md) | `GitHub Actions / Docker` | `npx warplogic add github-actions-docker-buildx-cache-ci-rules` |

### 📦 Frontend Frameworks (3)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**React 19 & Next.js 15 Server Actions Production .cursorrules**](rules/react-19-compiler-server-actions-cursorrules.md) | `React 19` | `npx warplogic add react-19-compiler-server-actions-cursorrules` |
| [**Tailwind CSS v4 & Shadcn UI Modern .cursorrules**](rules/tailwind-v4-vite-shadcn-cursorrules.md) | `Tailwind v4` | `npx warplogic add tailwind-v4-vite-shadcn-cursorrules` |
| [**SvelteKit 5 Runes & Tailwind v4 Production Cursor Rules**](rules/sveltekit-5-runes-tailwind-v4-cursorrules.md) | `SvelteKit` | `npx warplogic add sveltekit-5-runes-tailwind-v4-cursorrules` |

### 📦 DevOps & Infrastructure (2)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Kubernetes Helm Chart Security & Hardening .cursorrules**](rules/kubernetes-helm-production-hardening-cursorrules.md) | `Kubernetes` | `npx warplogic add kubernetes-helm-production-hardening-cursorrules` |
| [**Docker Compose Production Security & Multi-Stage .cursorrules**](rules/docker-compose-production-security-cursorrules.md) | `Docker` | `npx warplogic add docker-compose-production-security-cursorrules` |

### 📦 API Security (2)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Stripe Billing & Webhooks Idempotency .cursorrules**](rules/stripe-webhooks-idempotency-cursorrules.md) | `Stripe SDK` | `npx warplogic add stripe-webhooks-idempotency-cursorrules` |
| [**Upstash Redis Sliding-Window Rate Limiting .cursorrules**](rules/redis-upstash-rate-limiting-cursorrules.md) | `Upstash` | `npx warplogic add redis-upstash-rate-limiting-cursorrules` |

### 📦 Databases & Storage (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Drizzle ORM & Neon Serverless Postgres .cursorrules**](rules/drizzle-orm-neon-serverless-cursorrules.md) | `Drizzle ORM` | `npx warplogic add drizzle-orm-neon-serverless-cursorrules` |

### 📦 Kubernetes & DevOps (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Kubernetes Helm 3 Chart Templating & GitOps ArgoCD Release Rules**](rules/kubernetes-helm-chart-release-cursorrules.md) | `Helm 3 / ArgoCD` | `npx warplogic add kubernetes-helm-chart-release-cursorrules` |

### 📦 Mobile Development (2)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**React Native Expo Router v4 Production Cursor Rules**](rules/react-native-expo-router-cursorrules.md) | `React Native` | `npx warplogic add react-native-expo-router-cursorrules` |
| [**Flutter 3.24 & BLoC Clean Architecture Cursor Rules**](rules/flutter-bloc-clean-architecture-cursorrules.md) | `Flutter` | `npx warplogic add flutter-bloc-clean-architecture-cursorrules` |

### 📦 Backend & Systems (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Rust Axum 0.7 & Tokio Async Microservice Cursor Rules**](rules/rust-axum-tokio-sqlx-cursorrules.md) | `Axum` | `npx warplogic add rust-axum-tokio-sqlx-cursorrules` |

### 📦 Fullstack & Real-Time (1)

| Rule & Blueprint | Framework | Install Command |
| :--- | :---: | :--- |
| [**Elixir Phoenix LiveView 1.0 Production Cursor Rules**](rules/elixir-phoenix-liveview-cursorrules.md) | `Phoenix LiveView` | `npx warplogic add elixir-phoenix-liveview-cursorrules` |


---

## 🛠️ Interactive Stack Builder & Zero-Trust Studio
Generate custom multi-framework rules and simulate L7 mTLS policies at:
[https://www.warplogicai.com](https://www.warplogicai.com)

## 🤝 Contributing
1. Fork this repository.
2. Add your rule file in `rules/<slug>.md`.
3. Open a Pull Request!

## 📄 License
MIT License. Free for commercial and personal use.
