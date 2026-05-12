# Agent Experience (AX)

A discipline that did not exist as a vocabulary in 2022, was emerging in 2024, and by 2026 has its own job titles, design practices, and measurement frameworks. **Agent Experience (AX) is the experience that AI agents have when interacting with your APIs, docs, tools, and developer surfaces.**

It is to AI agents what Developer Experience is to humans.

## Why AX needs its own term

The argument, articulated across multiple essays in 2024–2026:

- DX optimises for what humans experience. Many of those optimisations (clear UI, vivid prose, branding) are wasted on agents.
- Agents need things humans don't. Determinism. Idempotency. Machine-readable schemas. Tool descriptions written for retrieval, not for marketing. Error messages structured for programmatic interpretation.
- The same product can have great DX and terrible AX. A beautifully designed dashboard with confusing tool naming, inconsistent error shapes, and undocumented rate limits delights humans and frustrates agents.
- The reverse is also true. A product with a brilliant MCP server and machine-perfect documentation can read as soulless to humans who arrive looking for personality.

The dual-audience thesis (see [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md)) requires both DX and AX. They are siblings, not the same thing.

## What AX covers in practice

A working scope for AX work as of mid-2026:

### 1. Agent-facing schemas and capability descriptions

- OpenAPI / GraphQL spec quality.
- MCP server design (tool naming, descriptions, schema, parameter constraints).
- Schema.org / JSON-LD markup on web surfaces.
- Type-correct, version-stable representations.

### 2. Documentation written for agent consumption

- One concept per page.
- Complete runnable code examples (no "// rest omitted for brevity").
- Explicit version metadata.
- Canonical URLs.
- `llms.txt` and `llms-full.txt`.

See [`./documentation-for-agents.md`](documentation-for-agents.md).

### 3. Error message design

- Programmatically parseable error codes.
- Clear human-readable hints embedded in error responses.
- Suggested fixes ("did you mean...").
- Stable error-code stability (versioned errors).

### 4. Idempotency and retry semantics

- Idempotency keys exposed on side-effecting operations.
- Predictable retry behaviour.
- Clear semantics for partial success / failure.

### 5. Rate limit and quota communication

- Limits documented and surfaced in response headers (`X-RateLimit-Remaining` patterns).
- Backoff hints.
- Quota-exceeded errors that agents can act on rather than fail with.

### 6. Authentication ergonomics for agentic access

- OAuth scopes that map to the operations an agent is likely to perform.
- Token introspection so agents can check their own permissions.
- Refresh flows that agents can complete without human intervention (where appropriate).

### 7. Performance and latency

- Agents have time budgets per tool call. Slow tools time out and hurt agent task completion.
- Long-running operations exposed as Tasks (see [`./mcp-as-devrel-surface.md`](mcp-as-devrel-surface.md)).

### 8. Observability of agent behaviour

- Logs that distinguish agent traffic from human traffic.
- Metrics on tool-call success rate, latency distribution, error patterns.
- Feedback loops from agent-mediated usage into product and DevRel decisions.

## Agent Experience as a job

Several distinct job patterns have emerged:

- **Agent Experience Engineer** (or AX Engineer). Owns the MCP server, the OpenAPI quality, and the schemas. Often sits inside engineering or DX but with explicit "agent-facing" responsibilities. Common at AI infrastructure companies and at developer-tool companies whose products are increasingly invoked by agents.
- **DevRel Engineer with AX scope.** A developer advocate whose remit explicitly includes both human-facing content and machine-facing surfaces. Less specialised but pragmatic for mid-stage companies.
- **Documentation Engineer for AI.** A technical writer or doc engineer who treats AI-readability as the primary craft concern.
- **Solutions Engineer for AI integrations.** A pre-sales / customer-facing engineer who helps enterprise customers wire their agents to your MCP server cleanly.

Companies experimenting with AX-specific titles in 2025–2026 include several AI infrastructure providers (Anthropic, OpenAI, smaller agent-platform companies), some API companies (Stripe, Twilio, Postman), and a growing number of mid-market developer-tool companies.

## How AX is measured

The metric stack is still developing. Some early candidates:

- **Tool call success rate.** Across agent-mediated invocations of your MCP server / API, what share succeed without error?
- **Agent task completion rate.** When an agent starts a workflow that involves your product, what fraction complete successfully? (Hard to measure without telemetry from the agent itself; sometimes inferred from server-side logs.)
- **Recovery rate from errors.** When your API returns an error to an agent, how often does the agent self-correct and retry successfully?
- **Time-to-first-successful-tool-call.** The agent analogue of TTFHW: from MCP server install to first successful invocation, what's the median time?
- **Citation accuracy in AI assistants.** When ChatGPT / Claude is asked about your product, what percentage of the technical claims it makes are accurate?
- **Schema completeness.** What percentage of your public API surface is exposed via OpenAPI, GraphQL schemas, or MCP tool definitions?

These are nascent. Most teams in 2026 are still figuring out which metrics correlate with business outcomes; the canonical AX scorecard does not yet exist.

## How AX intersects with DX

A useful framing:

| Layer | DX | AX |
|---|---|---|
| **Onboarding** | Quickstart written for humans; vivid first impression; hand-holding | Quickstart written for agents; complete code; explicit imports; no preamble |
| **Docs** | Conceptual, opinionated, varied formats; voice | Reference-complete, structured, stable URLs, dated |
| **APIs** | Easy to call; good error messages | Predictable; idempotent; machine-parseable errors |
| **Errors** | "Something went wrong. Try X." | `{"code": "INVALID_INPUT", "message": "...", "hint": "...", "docs_url": "..."}` |
| **Authentication** | Easy human OAuth flow; smooth UI | Scoped tokens; refresh flows; introspectable |
| **Versioning** | Clear migration guides; deprecation banners | Predictable versioning; capability negotiation; tool versioning |
| **Discovery** | Marketing site; blog posts; conference talks | `llms.txt`; MCP server; OpenAPI; schema.org |
| **Support** | Community forum; Discord; office hours | Telemetry-driven; doc gap analysis; agent log review |

A team that builds for both produces a product that performs well across the dual audience.

## Common AX failure modes

- **Treating MCP server as marketing.** Tool descriptions full of brand language; agents struggle to invoke effectively.
- **Beautiful docs, terrible schemas.** Mintlify-pretty pages, but underlying OpenAPI spec is incomplete or inconsistent.
- **Error messages designed only for humans.** Agents can't parse them; they fail and retry inappropriately.
- **No telemetry distinguishing agent traffic from human traffic.** You can't optimise what you can't measure.
- **AX as an afterthought.** Engineering ships features; AX gets "added later." By the time it's added, the technical debt is substantial.

## Where AX is going

Two trends visible at the end of 2025–2026:

1. **AX is becoming a hiring spec.** Job postings increasingly mention "designs APIs for agentic consumption" or "owns the MCP server" or "writes AI-readable docs." The role may not be titled "AX Engineer" — but the responsibility is being scoped explicitly.
2. **AX is becoming a measurement spec.** As more companies invest in agentic integrations, the demand for clear AX metrics rises. Tools that measure agent-mediated success (analogous to Mixpanel for human-mediated success) are an emerging category.

The discipline is real. It is not the same as DX. And in 2026 it is no longer optional for developer-product companies whose customers' developers use AI agents — which is essentially all of them.

## See also

- [`./mcp-as-devrel-surface.md`](mcp-as-devrel-surface.md)
- [`./documentation-for-agents.md`](documentation-for-agents.md)
- [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md)
- [`./metrics-in-ai-era.md`](metrics-in-ai-era.md)
- [`../11-trends/devex-movement.md`](../11-trends/devex-movement.md)