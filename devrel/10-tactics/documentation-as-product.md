# Documentation as a Product

For developer products, the documentation *is* the product to most users on their first day. The trial doesn't fail because the API is broken — it fails because the docs are confusing. The conversion happens not when sales calls but when the quickstart works.

Documentation strategy is therefore not "what the technical writers do" — it is a core DevRel and product responsibility.

## The audience problem

Every doc page is read by multiple audiences with different needs:

- **The complete beginner** who has never used your product.
- **The advanced user** debugging a corner case.
- **The evaluator** trying to decide if your product fits their needs.
- **The architect** assessing your product against alternatives.
- **The AI assistant** indexing your docs to answer questions about your product.

A single page cannot serve all of these. A documentation system can.

## Diátaxis

Daniele Procida's Diátaxis framework defines the canonical decomposition. Use it.

| Type | Goal | Tone | Example |
|---|---|---|---|
| **Tutorials** | Learning | Hand-holding, sequential | "Build your first chat app" |
| **How-to guides** | Solve specific problem | Concise, recipe-style | "How to authenticate with OAuth" |
| **Reference** | Lookup | Exhaustive, factual | API reference, CLI flags |
| **Explanation** | Understanding | Discursive, conceptual | "How our consensus algorithm works" |

Each docs page should clearly be one of these. Mixing types is the single most common docs failure.

## The minimum viable docs structure

For a launching developer product, the minimum docs are:

1. **Quickstart** (a tutorial) — 5 minutes to first hello world.
2. **Getting started** (slightly more depth) — first real feature usage.
3. **Concepts** (an explanation) — what the model is.
4. **API reference** (reference) — all endpoints / classes / methods.
5. **How-to guides** (how-to) — top 10 things users want to do.
6. **SDK docs** (reference + tutorial mix per SDK).

Anything beyond this is good-to-have. Without all of this, the product is incomplete.

## Time to first hello world

The single most important metric for documentation is **time to first hello world** (TTFHW). It measures the elapsed time from a developer arriving at your docs to having a working example produce visible output.

For most API products, the target is **under 5 minutes**. For complex platforms, **under 15 minutes**. Anything longer than 30 minutes is a structural failure.

Drivers of TTFHW:

- Signup friction (account creation, credit card requirements).
- API key generation friction.
- SDK installation friction.
- Working sample code.
- Sandbox / playground availability.

A useful exercise: have a new hire (with relevant background) attempt your quickstart cold and time it. Most teams discover the time is several times what they thought.

See [`../04-metrics/activation-metrics.md`](../04-metrics/activation-metrics.md).

## OpenAPI / spec-first docs

For API products, generating reference docs from an OpenAPI / Swagger / GraphQL schema is now the default approach. Benefits:

- Reference docs are always in sync with the API.
- Multiple output formats from one source (docs, SDK generators, mock servers, validators).
- Machine-readable spec serves downstream tooling.

Tools:

- **Stoplight, Redocly, Mintlify, ReadMe, Bump.sh** — covered in [`../08-tools/documentation-tools.md`](../08-tools/documentation-tools.md).
- **Postman** — also a primary surface for many developers.

## Interactive elements

Docs that are interactive convert better than docs that are static:

- **Embedded sandboxes.** CodeSandbox, StackBlitz, Sandpack.
- **Live API consoles.** Try-it-now widgets with your API key.
- **Curl-to-code generators.** Show curl example then auto-generate equivalent SDK code.
- **Switchable code samples.** "View in Python | JavaScript | Go | Rust."

## SDK docs as a separate problem

Each SDK has its own docs sub-problem. Common pattern: a shared "concepts" layer with per-language tutorials and per-language reference.

Don't make users with different stacks read the same Python-centric docs.

## Versioning

For mature products, docs versioning is non-trivial:

- **API versioning** with deprecation paths.
- **Docs for current version visible by default**, with prior versions accessible.
- **Clear migration guides** between versions.
- **Changelog** that is actually useful.

Stripe's API versioning model and docs are the canonical example.

## Search

Docs search is one of the highest-impact investments:

- **Algolia DocSearch** — Free for open source; commercial otherwise. Best-in-class.
- **Mintlify built-in search, GitBook search** — Adequate.
- **Custom search** with proper relevance tuning — Expensive but often necessary at scale.

Tracking search-query logs is one of the most underrated DevRel insights — it tells you what your users want to know that you haven't covered.

## AI-readiness

From 2024 onward, much of your docs traffic is AI agents on behalf of developers (ChatGPT, Claude, Cursor, Copilot). Practical implications:

- **Clear semantic structure** — headings, lists, code blocks.
- **One concept per page.** AI agents work better with focused content.
- **Explicit versions and dates.** AI agents need to know what's current.
- **Complete runnable examples** with all imports.
- **Clean URLs.** Persistent URLs that survive site reorganisations.
- **Expose an `llms.txt`** or equivalent index of canonical AI-readable pages.

See [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md).

## Doc culture

The hardest part of great docs is not tooling but culture:

- **Docs as a product surface, not a back-office artefact.** PMs care about docs; engineers care about docs.
- **Doc reviews part of code review.** Shipping a feature without docs is shipping a feature half-done.
- **A dedicated docs owner per area.** Not everyone owning it equals no one owning it.
- **A docs roadmap.** Quarterly investments in documentation quality.

Companies whose docs are best-in-class (Stripe, Twilio, Auth0, DigitalOcean tutorials, Cloudflare Workers, Postman, Algolia, MongoDB) all share this cultural orientation.

## See also

- [`../08-tools/documentation-tools.md`](../08-tools/documentation-tools.md)
- [`../04-metrics/activation-metrics.md`](../04-metrics/activation-metrics.md)
- [`../08-tools/code-sandboxes.md`](../08-tools/code-sandboxes.md)
- [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md)