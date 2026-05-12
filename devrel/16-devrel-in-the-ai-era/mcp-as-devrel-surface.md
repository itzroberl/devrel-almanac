# Model Context Protocol (MCP) as a DevRel Surface

If `llms.txt` is the documentation surface for AI agents, **MCP** is the capabilities surface. Where `llms.txt` lets agents *understand* your product, MCP lets them *operate* it. For developer-product companies in 2026, publishing an MCP server has become as central as publishing an SDK.

## What MCP is

**Model Context Protocol** is an open standard, launched by Anthropic on **November 25, 2024**, for connecting AI applications to external tools, data sources, and services. The protocol defines how an AI client (Claude Desktop, Cursor, ChatGPT, Gemini, Windsurf, custom agent) discovers and invokes capabilities exposed by an MCP server.

The protocol is JSON-RPC over multiple transports (stdio, HTTP, streamable HTTP, Server-Sent Events). It defines three core primitives:

- **Tools** — Actions the agent can invoke (call this API, run this query, send this email).
- **Resources** — Read-only data the agent can fetch (a file, a database record, a configuration).
- **Prompts** — Pre-built prompt templates the user or agent can invoke.

The result: a single MCP server can expose your product's capabilities to *any* MCP-compatible AI client. One server, all the agents.

## The growth curve

MCP's adoption is the fastest-spreading developer-facing standard in recent memory.

| Date | Milestone |
|---|---|
| Nov 25, 2024 | Anthropic open-sources MCP with Python and TypeScript SDKs |
| Mar 2025 | OpenAI adopts MCP across its Agents SDK and Apps platform |
| Apr 2025 | ChatGPT Desktop adds MCP support |
| Sep 2025 | MCP Registry (later PulseMCP) launches as a directory |
| Nov 2025 | OAuth 2.1 authorization framework added; streamable HTTP becomes default |
| Dec 2025 | Anthropic donates MCP to the Linux Foundation's Agentic AI Foundation |
| Early 2026 | Google announces Gemini API and Vertex AI MCP support |
| Mar 2026 | 13,230+ public servers registered in PulseMCP directory |
| Apr 2026 | ~78% of enterprise AI teams report at least one MCP-backed agent in production |

The shift is structural. MCP is no longer "Anthropic's protocol" — it is the de facto cross-vendor agent-integration standard, and DevRel teams build for it accordingly.

## Why MCP matters for DevRel

Three structural reasons MCP is a primary DevRel surface, not a curiosity:

1. **Single server, all agents.** A tool exposed via MCP works inside Claude Code, Cursor, Windsurf, ChatGPT, Gemini, and any custom agent. Without MCP, you'd be writing separate integrations for each AI vendor's function-calling format.
2. **Time-to-integrate is dramatically shorter.** Industry analyses report median MCP integration in roughly 4 hours versus 18 hours for per-vendor function-calling implementations — a ~4x productivity gain for integration teams.
3. **Agents are now customers of your product's actions, not just its docs.** When Cursor or Claude Code wants to send a Slack message, query your database, look at your error tracker, or invoke your deployment platform, MCP is how. If you don't expose an MCP server, you are invisible to the agents that increasingly initiate developer work.

## Notable company-published MCP servers (mid-2026)

The pattern is now widespread. Categories where MCP servers are common:

- **DevTools / observability.** GitHub MCP, Sentry MCP, Datadog MCP, PagerDuty MCP, GitLab MCP, Linear MCP, Jira-adjacent MCP servers.
- **Cloud and infra.** Cloudflare MCP (Workers, R2, KV), AWS MCP servers across services, Microsoft Azure MCP, Google Cloud MCP, Vercel MCP.
- **Communications and SaaS.** Slack MCP, Notion MCP, Linear MCP, Figma MCP, Zapier-like aggregators exposing dozens of integrations through a single MCP server.
- **Payments and commerce.** Stripe MCP (read-only for payment investigations; write for sandboxed actions), Shopify MCP, PayPal MCP.
- **Databases.** PostgreSQL MCP, MongoDB MCP, Redis MCP, BigQuery MCP, Snowflake MCP, Supabase MCP, Neon MCP, PlanetScale MCP.
- **Browser and automation.** Microsoft's Playwright MCP, browser automation servers.
- **AI/ML services.** Hugging Face MCP, Replicate MCP, Pinecone MCP, Together AI MCP.

The pattern that's emerged: companies who already operate well-designed APIs ship MCP servers within months of MCP standardisation. Companies whose APIs are messy struggle to expose them through MCP cleanly — which is itself a useful diagnostic.

## What makes a good MCP server

Hard-won 2025–2026 lessons:

### Tool descriptions are documentation

The text you write in a tool's `description` field is the substrate from which AI agents decide whether and how to invoke the tool. This is documentation for an audience of one (the agent, per session) but it is *more* consequential than your human-facing docs for that interaction.

Good tool descriptions:

- State the action precisely in the present tense ("Sends a Slack message to a channel" not "Slack integration").
- List parameters and their types explicitly.
- Note constraints (rate limits, side effects, idempotency).
- Distinguish read from write operations.
- Mention which other tools in the server are relevant adjacent capabilities.

### Names matter

Agents pick tools by name plus description. Two tools called `send_message` and `delete_message` get treated as adjacent. Naming that respects categories — `slack_send_message`, `slack_delete_message`, `slack_list_channels` — produces measurably better agent behaviour.

### Idempotency is critical

Agents retry. If your tool causes side effects on retry, the agent will produce duplicates, unintended charges, or corrupted state. Design for idempotency, expose idempotency keys, and document this in the tool description.

### Distinguish read-only from write tools clearly

Read tools (`list_records`, `get_user`) are safe to invoke speculatively. Write tools (`create_user`, `delete_record`) need user consent. The MCP client typically handles consent, but your server should mark side-effecting tools explicitly and consider gating destructive operations.

### Pagination, search, and large-result handling

Agents have context windows. Returning 10,000 records to an agent's tool call is wasteful at best, harmful at worst. Implement pagination, return summaries with optional `expand` parameters, and design tools that an agent can compose into a workflow rather than tools that try to do everything in one call.

### Long-running operations and the Tasks pattern

The MCP `Tasks` feature (added in 2025–2026 refinements) supports "call-now, fetch-later" patterns for operations that take more than a few seconds. State transitions — `working`, `input_required`, `completed`, `failed`, `cancelled` — let agents reason about ongoing work without timing out.

### Authentication and authorization

Use the OAuth 2.1 authorization framework that became the default in late 2025. Avoid hard-coded API keys in server configs. Support scoped tokens so agents can be granted limited capabilities rather than full account access.

### Error messages that an agent can act on

Bad: `Error: invalid input`. Good: `Error: parameter 'channel' must start with '#' or be a channel ID starting with 'C'. Received: 'general'. Suggestion: try '#general'.`

The error message is the agent's chance to self-correct. Write them for agents *and* humans.

### Versioning

MCP itself versions; your server's tools should also version. Breaking changes should be reflected in tool names or in capability negotiation. Agents that depended on the old shape will fail predictably rather than mysteriously.

## How DevRel teams build their MCP server

A practical sequence observed at multiple companies in 2025–2026:

1. **Identify the top 10–20 actions** developers want an AI agent to perform on the product. Almost always: list, get, create, update, delete patterns plus a handful of product-specific verbs.
2. **Audit the existing public API.** Most MCP servers are thin wrappers over existing REST/GraphQL APIs. The thinness is fine; the wrapper layer is where naming, descriptions, idempotency, and error-shape live.
3. **Write the server.** Python and TypeScript SDKs are mature; Go, Rust, Java, C# SDKs exist.
4. **Test against multiple clients.** Claude Desktop, Cursor, Windsurf, ChatGPT Desktop, and a custom test harness. Agents from different vendors handle edge cases differently.
5. **Publish.** Add to PulseMCP / MCP Registry. List on your own developer portal. Document setup steps.
6. **Treat as a first-class product.** Versioned, supported, monitored. Telemetry on tool-call success rate, average latency, error patterns.

The PulseMCP directory functions as the primary discovery surface — analogous to how the npm registry, PyPI, or the GitHub Marketplace function for traditional developer tools.

## Hosted vs. self-hosted MCP servers

A debate that settled quickly in 2025–2026. Hosted (remote) MCP servers won for most products because:

- Auth is hard. OAuth 2.1 is easier to operate centrally than to deploy to every user.
- Scaling is hard. Your central infrastructure handles load better than thousands of individual user laptops.
- Updates are continuous. Push a fix to the hosted server; every client gets it instantly. With self-hosted, every user has to update.
- Telemetry. Hosted servers let the publisher learn how agents are actually using the tool.

Self-hosted MCP servers still make sense for local-machine-bound tools (browser automation, IDE integration, filesystem access), and many products ship both a hosted server for cloud capabilities and a local server for desktop integration.

## The DevRel implication

If your product can sensibly be invoked by an AI agent, publishing an MCP server is now part of the basic DevRel offering. The criteria are:

- Your product has well-defined actions agents would want to invoke.
- Those actions can be authenticated cleanly.
- The product's value increases when agents can perform actions on a human's behalf.

This is true for almost every API product, infra product, dev tool, productivity SaaS, observability platform, and database. It is less obviously true for things like media products, raw infrastructure, or end-user-only apps — but even then, integration-with-agents has become a competitive table-stakes feature.

## Agent-experience (AX) is downstream

The discipline of designing for the agent audience extends beyond MCP. Tool naming, error message design, idempotency, schema clarity, OpenAPI quality — these are the components of what an emerging vocabulary calls *Agent Experience* (AX). See [`./agent-experience-ax.md`](agent-experience-ax.md).

## See also

- [`./agent-experience-ax.md`](agent-experience-ax.md)
- [`./llms-txt-standard.md`](llms-txt-standard.md)
- [`./documentation-for-agents.md`](documentation-for-agents.md)
- [`../05-companies/ai-companies.md`](../05-companies/ai-companies.md)

## Primary sources

- Anthropic, "Introducing the Model Context Protocol," November 25, 2024.
- Anthropic, "Donating the Model Context Protocol and establishing the Agentic AI Foundation," December 2025.
- TechCrunch, "OpenAI adopts rival Anthropic's standard," March 26, 2025.
- *Latent Space*, "Why MCP Won," 2025–2026.
- PulseMCP directory and MCP Registry.
- modelcontextprotocol.io specification and roadmap.
- WorkOS, "Everything your team needs to know about MCP in 2026."