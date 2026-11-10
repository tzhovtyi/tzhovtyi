### Timofei

Senior full-stack engineer. TypeScript, Go, PostgreSQL, Node.js/NestJS, React/Next.js.

---

### What I do

For six years I've been building production systems in TypeScript, mostly on the backend side of full-stack. Right now I'm the technical owner of a cross-border logistics ERP that runs daily operations for 124 carrier and broker offices across China and Russia. Nearly all of my work lives in private repos, so here's the short version of what's in them.

**Logistics ERP & integration platform** · senior full-stack engineer

- ~20,000 compliance-critical documents a day exchanged with customs, carriers and brokers through BullMQ workers with idempotent jobs and human escalation on retry exhaustion. No lost submissions since launch.
- Payment and ledger core handling ~200K transactions a month across 100+ corporate balances: append-only PostgreSQL ledger, idempotent payment and refund flows, multi-provider routing with failover.
- p99 API latency cut from ~1.3s to under 400ms using tiered PostgreSQL materialized views refreshed on per-dataset freshness schedules, plus EXPLAIN-driven composite and partial indexes.
- Led the R&D on a RAG pipeline for an internal company-knowledge assistant: benchmarked hybrid dense + lexical retrieval, re-ranking and synthetic chunk enrichment across several LLM APIs and embedders, landing at 84% fewer tokens than full-context prompting. One piece of the tooling I wrote to survive the API bills is public: [unkeyed](https://github.com/tzhovtyi/unkeyed), a drop-in Anthropic SDK client that routes calls through your subscription instead of an API key.
- Built the observability stack (Grafana, Loki, Prometheus) and a Docker-based CI/CD pipeline on self-hosted GitHub Actions runners.
- Testing pyramid from unit tests on finance logic up through Testcontainers integration tests to Playwright E2E, 85% coverage on critical modules.

**E-commerce rescue** · lead fullstack

- Took over an abandoned, non-functional Next.js prototype, re-architected it and shipped to production in 16 weeks: 25K monthly users, a 12K-SKU catalog, mobile LCP under 0.8s via ISR, server components and image optimization. Mentored the two mid-level engineers on the team through pairing and a code review checklist.
- Moved the Go microservices behind it from synchronous service calls to event-driven RabbitMQ messaging.

**Government workstation provisioning** · full-stack

- A browser UI that drives a local agent over WebSockets, with in-browser detection of GOST cryptography support (CryptoPro, ViPNet) and graceful fallback across 30+ browser/OS combinations.
- Telemetry ingestion into PostgreSQL so support could see which environments were actually failing instead of guessing.

### Stack

**Language** TypeScript · JavaScript · Go · SQL · Bash  
**Backend** Node.js · NestJS · Express · BullMQ · RabbitMQ · WebSockets · REST/OpenAPI  
**Frontend** React · Next.js · Vue 3 · Nuxt · Tailwind · Vite · Zustand · SSR/SSG  
**Databases** PostgreSQL · Redis · MongoDB · pgvector · Prisma · TypeORM · Drizzle  
**Infra** Docker · Kubernetes · GitHub Actions · Terraform · Nginx · WireGuard · AWS · Linux  
**Observability** Prometheus · Grafana · Loki · Promtail · Sentry  
**Testing** Vitest · Playwright · Jest · Testcontainers  
**Design** DDD · Hexagonal architecture · Event-driven · Feature-Sliced Design · ABAC/RBAC  
**AI** LLM APIs · RAG · MCP · Claude Code

### Contact

[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tim@zhovtyi.dev) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/timofei-zhovtyi/) [![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/tzhovtyy)
