# DevRel in the AI Era

A dedicated section. The 2023–2026 wave of LLMs, AI coding agents, and agent-mediated discovery has changed what Developer Relations does, who its audience is, and how it is measured — more fundamentally than any shift since the 2008 emergence of GitHub and Stack Overflow.

This section synthesises the perspectives, evidence, and early signals.

## The central claim

Modern DevRel now serves **two distinct audiences simultaneously**:

1. **AI agents** — Cursor, Claude Code, Copilot, ChatGPT, Perplexity, Gemini, and the growing class of background coding agents — that read your docs, sample code, and `llms.txt` *to produce code on behalf of developers*. They are the **execution audience**. They want exhaustive, structured, machine-parseable material.

2. **Human developers** — who increasingly never read your docs first. They form opinions about your product on X, Bluesky, YouTube, Twitch, Reddit, Hacker News, Discord, podcasts, and conferences. They are the **inspiration audience**. They need authentic engineering brand, vivid demos, opinionated takes, and people they trust.

The same content rarely serves both well. The most successful 2025–2026 DevRel teams have begun to design for the split: agent-readable surfaces optimised for LLM consumption, and human-shaped surfaces optimised for emotional and aesthetic engagement. See [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md).

## What changed between 2022 and 2026

| Dimension | 2022 | 2026 |
|---|---|---|
| First-touch discovery | Google search → docs | "Ask ChatGPT" / "Ask Claude" / Perplexity → maybe-docs |
| Code authorship | Developer types code | AI agent writes code under developer supervision |
| Doc reader | Human | Human + AI agent (often AI first) |
| Documentation surface | Web page | Web page + `llms.txt` + MCP server |
| Integration interface | REST/GraphQL API + SDK | Same + MCP server + agent-friendly tool schemas |
| Onboarding metric | TTFHW for human | TTFHW for human + agent task success rate |
| Discovery channel | Google + Twitter + HN | Google + ChatGPT + YouTube + LinkedIn + Bluesky + Reddit + podcasts |
| Trust signal | Stars, follower counts, "recommended by" | Cited by AI assistants, vouched for by trusted humans |
| Content type that travels | Polished blog posts | Live streams, founder voices, opinionated takes, failures |

Each of these shifts is treated in detail in subsequent files.

## What this section covers

**Foundations**

- [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md) — Why DevRel now has two audiences and how to serve both.
- [`./llm-mediated-discovery.md`](llm-mediated-discovery.md) — How developer research moved from Google to LLMs.
- [`./inspiration-stays-human.md`](inspiration-stays-human.md) — Why YouTube, X, podcasts, and conferences matter *more* in the AI era, not less.

**Agent-facing surfaces**

- [`./llms-txt-standard.md`](llms-txt-standard.md) — The `llms.txt` convention: origin, adoption, evidence, scepticism.
- [`./mcp-as-devrel-surface.md`](mcp-as-devrel-surface.md) — Model Context Protocol as a primary DevRel offering.
- [`./agent-experience-ax.md`](agent-experience-ax.md) — Agent Experience as an emerging discipline alongside DX.
- [`./documentation-for-agents.md`](documentation-for-agents.md) — Writing docs both humans and machines can use.

**Optimisation and measurement**

- [`./geo-aeo-for-devrel.md`](geo-aeo-for-devrel.md) — Generative / Answer Engine Optimisation tactics.
- [`./metrics-in-ai-era.md`](metrics-in-ai-era.md) — Share of Model, prompt feedback, citation tracking, AI-mediated activation funnels.

**Identity and culture**

- [`./vibe-coding-and-the-ai-engineer.md`](vibe-coding-and-the-ai-engineer.md) — New developer identities; Karpathy's "vibe coding"; swyx's "AI Engineer."

**The debates**

- [`./perspectives-and-debates.md`](perspectives-and-debates.md) — Named voices and what they argue.
- [`./critical-takes.md`](critical-takes.md) — "DevRel is dead because AI" arguments and the rebuttals.
- [`./early-signals-what-works.md`](early-signals-what-works.md) — Concrete, observable patterns of what works in 2026.

## The trains of thought, summarised

The discourse on AI-era DevRel splits into roughly five trains of thought. Each is developed in detail elsewhere in this section; the short versions:

1. **The Dual Audience.** Most operationally pragmatic. Practitioners design separately for human inspiration and AI execution. Both audiences are now real; the strategies differ. Best articulated by people running working DevRel programs at AI-first companies (Anthropic, Mintlify, Vercel) and by the AngelHack and DocE-AI essays of 2025–2026.

2. **The Strategic-Reframe Camp.** Argues DevRel is more important than ever, not less. "Plot twist: we're not dead. We're standing on the biggest stage of our careers" — Angie Jones, *How DevRel is Leading AI Adoption* (2025). DevRel becomes the modeller of authentic AI-augmented practice, the translator between developer perception and telemetry, and the curator of trust signals AI assistants cannot synthesise.

3. **The Post-Mortem Camp.** Argues that the kind of DevRel that died in 2022–2024 was dying anyway and AI just accelerated the reckoning. "RIP DevRel 2010–2024" (MB Consulting, 2024). DevRel-as-content-marketing is the casualty; DevRel-as-strategic-function lives on, restructured.

4. **The Agent-Experience Camp.** Sees the most important new DevRel discipline as designing for AI agents — your APIs, docs, `llms.txt`, MCP servers, prompt templates, error messages, and so on are now consumed primarily by software, not by people. Best operationalised inside AI-product companies (OpenAI, Anthropic) and at infrastructure companies that already ship MCP servers.

5. **The Sceptical / Empirical Camp.** Cautions that much of what's claimed about AI-era DevRel is unverified marketing. `llms.txt` may have negligible measurable impact; AI-citation studies show inconsistent results; some of the breathless 2024–2025 advice has not survived 2026 data. Best represented by analyses like Signals.sh's "Does llms.txt actually work?" (2026) and the broader observability community's caution that *sentiment about AI productivity diverges from telemetry*.

In practice, most mature DevRel teams in 2026 hold a position that draws from camps 1, 2, and 4 — adopting the dual-audience design, retaining the strategic-reframe argument, building agent-facing surfaces — while taking camp 5's empirical caution seriously enough to instrument outcomes rather than trust the rhetoric.

## What to read first

If you have time for only three of the files below:

1. [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md)
2. [`./agent-experience-ax.md`](agent-experience-ax.md)
3. [`./early-signals-what-works.md`](early-signals-what-works.md)

If you have time for one: the dual-audience thesis. It is the lens for everything else.

## See also

- [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md) — The earlier, briefer treatment of AI's impact on DevRel.
- [`../05-companies/ai-companies.md`](../05-companies/ai-companies.md) — AI companies' DevRel programs.
- [`../10-tactics/documentation-as-product.md`](../10-tactics/documentation-as-product.md) — Documentation strategy generally.
- [`../11-trends/future-directions.md`](../11-trends/future-directions.md) — Broader future patterns.