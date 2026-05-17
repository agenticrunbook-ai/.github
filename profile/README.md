## Agentic Runbook

AI consulting firm specializing in production-ready agentic systems. We build multi-agent systems your team can own, operate, and extend — not a dependency on our services.

**Domain:** agenticrunbook.ai  
**Stack:** LangGraph · LangChain · LangSmith · Python 3.12 · MCP (Model Context Protocol)

---

### What We Build

We design and implement agentic AI systems for mid-market B2B companies ($50M–$500M revenue). Our engagements follow a three-phase methodology:

- **Diagnose** — Map workflows, identify automation candidates, prioritize by ROI
- **Build** — Implement production-grade agents using LangGraph for orchestration, LangSmith for observability, and MCP for tool integration
- **Transfer** — Hand off running systems with documentation, runbooks, and ADRs so your team can operate and extend without us

---

### Repositories

| Repo | Description |
|------|-------------|
| `agenticrunbook-website` | Company website — Astro + Tailwind, hosted on Cloudflare Pages |
| `agentic-runbook-ip` | Internal IP library — ADR archive, engagement playbooks, prompt engineering standards, eval framework, client repo template |

---

### Technology Decisions

All major technology decisions are documented as Architecture Decision Records (ADRs) in the `agentic-runbook-ip` repository. Current decisions include:

- LangGraph as default orchestration framework (ADR-001)
- LangSmith as observability standard (ADR-003)
- Model-agnostic LLM layer with OpenAI/Anthropic defaults (ADR-004)
- MCP as standard tool protocol (ADR-031)
- Cloudflare Pages for web hosting (ADR-008)

---

### Contact

- Website: [agenticrunbook.ai](https://agenticrunbook.ai)
- Blog: [agenticrunbook.ai/blog](https://agenticrunbook.ai/blog)
- Inquiries: hello@agenticrunbook.ai
