# RAXAR SOLUTIONS S.L.

> **Premium AI Consulting · B2B + B2C** · *Del Caos al Éxito*

Algeciras, España · [raxar.es](https://raxar.es) · [contacto@raxar.es](mailto:contacto@raxar.es)

🚀 **2026-05-05**: First enterprise client signed in Algeciras. Real-traffic soak ongoing.

---

## What we do

We design and operate **autonomous AI agent platforms** for SMBs and enterprises. We don't sell hours; we sell systems that run themselves — production-grade, multi-tenant, GDPR + AI Act compliant from day one.

- 🧠 **FENIX** — AI dashboard + 11 productos (ARIA · Atlas Pro · Hermes · SOLVA · Oracle · Sentinel · Radar · Pulse-CV · 4 partners) live serving real customers.
- 🤖 **n8n orchestration** — 39 production workflows · 99.99% success rate · errorWorkflow + executionTimeout 100% compliance · multi-tenant RLS-isolated.
- 🛡️ **Self-hosted privacy** — On-premise LLM routing via LiteLLM Proxy (11 providers) + Ollama torre (9 models · 96 GB) · EU residency policy enforced · GDPR Art. 5 compliant.
- 📊 **Observability** — VIGIA torre (20 signals) + LLM cost tracking + GlitchTip + Uptime Kuma + activity_log audit trail.

## Stack at a glance

```
Frontend         Next.js 16 · Tailwind v4 · React 19
Backend          Node.js 24 · Python 3.12 · FastAPI · LangGraph
Database         PostgreSQL 16 · 115 fenix tables · 100% RLS coverage
LLM Router       LiteLLM Proxy · Anthropic · Groq · Gemini · DeepSeek · Together · OpenRouter · Ollama torre
Vector Store     Qdrant (5 collections · raxar-help-center · oracle · ARIA RAG · Atlas Pro)
Orchestration    n8n v2.17 · LangGraph (piloto) · Temporal.io (S268+)
Infra            Coolify v4 · Docker · Hostinger VPS · Tailscale mesh
Compliance       SOC 2 (mindset · vendor S269+) · GDPR · AI Act CV Manager assessment
```

## Compliance + security

- **GDPR**: 9 RGPD docs · DSR pipeline E2E live (1m34s historical resolution)
- **AI Act EU**: CV Manager HIGH-RISK assessment v1.0 · production gate enforced
- **Headers**: 7/7 strong (CSP · HSTS preload · frame DENY · nosniff · XSS · Referrer · Permissions)
- **Webhooks**: HMAC dual-mode · 3/3 reject 401 sin firma · 7 evidence captures 7d
- **Audit log**: 19 event_types · 5 paths instrumented · activity_log fenix.activity_log

## Repository map

| Repository | Purpose | Visibility |
|---|---|---|
| `.github` | Org-face profile · CI templates · disclosure policy | Public |
| `raxar-platform` | FENIX dashboard B2B + RAXAR Platform B2C apps monorepo | Private |
| `raxar-web` | Corporate website Next.js (raxar.es HUB · 4-way split) | Private |
| `raxar-cluster` | Develop team · Python cluster + partner backends (Bardo · Vizor · Resona · Overture) | Private |
| `raxar-infra` | IaC · runbooks · scripts · docker compose · n8n compliance gates | Private |
| `raxar-projects` | Project handoff · informes Markdown→PDF · grandes proyectos Stripe milestones | Private |
| `raxar-docs` | Internal documentation + KNOWLEDGE/ + ADRs + planning | Private |

### 4-way product portfolio (S272.36 ADR-S272-025)

| Surface | URL | Audience | Container |
|---|---|---|---|
| HUB landing | [raxar.es](https://raxar.es) | Marketing + ARIA chat público | `raxar-web` |
| FENIX App | [dashboard.raxar.es](https://dashboard.raxar.es) | B2B clients · 11 productos · admin | `raxar-dashboard` |
| RAXAR Platform | [app.raxar.es](https://app.raxar.es) | B2C prosumer creators (post-firma) | `raxar-explore` |
| **RAXAR Lab** | [**lab.raxar.es**](https://lab.raxar.es) | Playground · blog · periódico · arcade · experimentos | `raxar-lab` |

### Engineering practices

- **Conventional Commits** + linear history (squash-merge enforced)
- **CODEOWNERS** routing per surface area · ≥1 approval per CI gate
- **SOC 2 mindset**: every PR labeled with Trust Service Criteria
- **Compliance hard gates** in CI: TypeScript strict · n8n compliance linter · RLS preserved · LLM Router enforcement · HMAC on public webhooks
- **Dependabot** weekly multi-ecosystem · auto-merge patch + minor + security
- **AI co-engineering** under human supervision · Claude Opus 4.7 (1M context) for senior IT agent role

## Team

- **Jose** — Founder · CEO · Production owner
- **Sebas** — Develop lead · Cluster + partner backends
- **Jaime** — Admin role · core team

## Contact

- 📧 [contacto@raxar.es](mailto:contacto@raxar.es) — General inquiries
- 📧 [jose@raxar.es](mailto:jose@raxar.es) — Founder direct
- 📧 [dpo@raxar.es](mailto:dpo@raxar.es) — Data protection officer (GDPR DSR)
- 🌐 [raxar.es](https://raxar.es) — Website
- 💼 [Pricing & Quotes](https://raxar.es/contacto?intent=presupuesto)

---

*🤖 RAXAR is an AI-first company. This README, our infrastructure, and parts of our platform are co-engineered with AI agents under human supervision. We dogfood our own stack.*
