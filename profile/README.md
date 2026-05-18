## Agentic Runbook

AI consulting firm specializing in production-ready agentic systems. We build multi-agent systems your team can own, operate, and extend — not a dependency on our services.

**Domain:** [agenticrunbook.ai](https://agenticrunbook.ai)  
**Stack:** LangGraph · LangChain · LangSmith · Python 3.12 · MCP (Model Context Protocol) · Cloudflare Pages · Astro

---

### What We Build

We design and implement agentic AI systems for mid-market B2B companies ($50M–$500M revenue). Our engagements follow a three-phase methodology:

- **Diagnose** — Map workflows, identify automation candidates, prioritize by ROI. Output: scored workflow map + build recommendation.
- **Build** — Implement production-grade agents using LangGraph for orchestration, LangSmith for observability, and MCP for tool integration.
- **Transfer** — Hand off running systems with documentation, runbooks, and ADRs so your team can own and extend without us.

---

### Repositories

| Repo | Description |
|------|-------------|
| [`agenticrunbook-website`](https://github.com/agenticrunbook-ai/agenticrunbook-website) | Company website — Astro + Tailwind, hosted on Cloudflare Pages. 12-post blog archive. |
| [`agentic-runbook-ip`](https://github.com/agenticrunbook-ai/agentic-runbook-ip) | Internal IP library — 56 ADRs, engagement playbooks (Diagnose/Build/Transfer), prompt engineering standards, eval framework, client repo templates, SOW/NDA/MSA Jinja2 templates. |
| [`agentic-runbook-agents`](https://github.com/agenticrunbook-ai/agentic-runbook-agents) | Internal agent fleet — LangGraph implementations for `@finance-bot`, `@legal-bot`, `@cto-bot`, `@ceo-bot`, `@cmo-bot`, `@inbound-triage-agent`, `knowledge-retrieval-mcp`. |
| [`company-knowledge-base`](https://github.com/agenticrunbook-ai/company-knowledge-base) | Company-wide knowledge base — strategy documents, published decisions, org principles. |
| [`agentic-runbook-brand`](https://github.com/agenticrunbook-ai/agentic-runbook-brand) | Brand assets — logo, color system, typography, design guidelines. |

---

### Architecture Decision Records (ADRs)

All major technology and delivery decisions are documented as immutable Architecture Decision Records in [`agentic-runbook-ip/adr/`](https://github.com/agenticrunbook-ai/agentic-runbook-ip/tree/main/adr). **56 ADRs accepted as of May 2026.**

**Selected decisions:**

| ADR | Decision |
|-----|----------|
| ADR-001 | LangGraph as default agent orchestration framework |
| ADR-003 | LangSmith as sole observability platform |
| ADR-004 | Model-agnostic LLM layer — OpenAI (gpt-4o) + Anthropic (claude-3-5-sonnet) defaults |
| ADR-008 | Cloudflare Pages for web hosting |
| ADR-024 | Agent Eval Framework — golden dataset, P0/P1/P2 metric hierarchy, CI eval gate |
| ADR-025 | Fleet Agent Deployment Standards — naming, env vars, AGENTS.md frontmatter |
| ADR-026 | Security & Secrets Management Standard — 3-tier model, HMAC-256, rotation policy |
| ADR-028 | LangGraph Agentic Patterns Standard — 5 canonical patterns, state design rules |
| ADR-029 | Data Privacy & Client Data Handling Standard — 3-tier taxonomy, per-client isolation |
| ADR-031 | MCP (Model Context Protocol) as standard tool integration protocol |
| ADR-035 | Agent Versioning & Rollback Standard — SemVer, git tags, rollback SLA ≤30 min P1 |
| ADR-041 | Agent Observability & Cost Attribution — LangSmith metadata tags, weekly cost rollup |
| ADR-050 | Client Engagement SOW Template Standard — Jinja2 templates, 3-phase SOW library |
| ADR-051 | Day-1 Go-Live Operations Runbook — T-24h checklist, T-0 launch sequence, rollback plan |
| ADR-055 | MSA & NDA Template Standard — Jinja2 NDA/MSA, sub-4h NDA turnaround target |
| ADR-056 | @legal-bot Full Implementation — contract review, NDA/MSA/SOW generation, 5-tier risk model |

---

### Internal Agent Fleet

| Agent | Role | Model | Status |
|-------|------|-------|--------|
| `@cto-bot` | Chief Technology Officer | Claude 3.5 Sonnet (Opus for strategy) | Active |
| `@ceo-bot` | Chief Executive Officer | Claude 3.5 Sonnet | Active |
| `@cmo-bot` | Chief Marketing Officer | Claude 3.5 Sonnet | Active |
| `@finance-bot` | Finance & invoicing operations | GPT-4o | Deploy-ready |
| `@legal-bot` | Contract review, NDA/MSA/SOW generation | Claude 3.5 Sonnet | Deploy-ready |
| `@inbound-triage-agent` | Lead qualification & routing | GPT-4o | Deploy-ready |
| `knowledge-retrieval-mcp` | Qdrant-backed RAG MCP server | — | Deploy-ready |

---

### Engagement Methodology

Our IP library contains the full delivery methodology:

- **Diagnose Playbook v1.0** — 3-week diagnostic sprint: workflow mapping, agent readiness scoring, ROI prioritization
- **Build Playbook v1.0** — Sprint 0–4 structure, RACI, technical standards reference, exit criteria
- **Transfer Playbook v1.0** — 35-item exit checklist, capability transfer protocol, 3-tier retainer model
- **Agentic Academy Curriculum v1.0** — 6-module, 40-hour curriculum for client team upskilling

---

### Contact

- Website: [agenticrunbook.ai](https://agenticrunbook.ai)
- Diagnostic Sprint: [agenticrunbook.ai/diagnostic-sprint](https://agenticrunbook.ai/diagnostic-sprint)
- Inquiries: [hello@agenticrunbook.ai](mailto:hello@agenticrunbook.ai)
