# Documentation for Agents

When your docs are consumed by AI agents as much as by humans, the craft of documentation changes. This file is a practical guide.

## The two readers, side by side

A human reading docs:

- Skims for the part that's relevant.
- Forms an opinion about the product from voice and aesthetic.
- Gives up after about 30 seconds if confused.
- Wants a clear path forward.
- Remembers what they read.

An AI agent reading docs:

- Reads with no skimming; retrieves chunks and reasons over them.
- Forms no opinion; cites text into a response to its user.
- Doesn't give up; will keep trying combinations until something works (or until the context fills up).
- Wants every fact explicit, complete, and self-consistent.
- Has no memory between sessions, so each page must stand alone.

Designing documentation that serves both takes deliberate craft.

## Practical guidelines

### One concept per page

Agents struggle with pages that conflate multiple concepts. Each page should answer one question. "What is X? How do I use X? What are X's limits?" can be one page if X is small. "What is X?" and "X versus Y" and "X authentication" are three pages.

### Lead with the answer

The first 200 words of each page should contain the canonical answer to the page's question. Agents extract opening passages preferentially when synthesising responses.

A useful pattern: a single paragraph at the top that summarises everything. The rest of the page elaborates. Humans benefit from the same structure — they read the lead and decide whether to keep going.

### Complete, runnable code samples

Bad:
```python
# Configure the client
client = Foo(...)
# Make the call
result = client.do_something()
```

Good:
```python
import os
from foo_sdk import FooClient

client = FooClient(
    api_key=os.environ["FOO_API_KEY"],
    region="us-east-1",
)

result = client.do_something(input="hello")
print(result.output)
```

An agent that copies the bad example produces broken code. An agent that copies the good example produces working code on its first attempt. The compounding effect across thousands of agent-mediated trials is large.

### Explicit imports, environment variables, prerequisites

Every code sample should list:

- All imports.
- Required environment variables.
- Any prerequisite installation steps.
- Expected output (where deterministic).

The agent will copy what you write; missing context becomes broken downstream code.

### Multiple language variants per sample

If your product has SDKs in Python, TypeScript, Go, Rust, and Ruby, the canonical examples should exist in all of those languages, with parity. Agents extract the right one based on the asker's preferred language. Skipping a language means agents asking in that language get less helpful answers.

### Explicit versions and dates

- `dateModified` in JSON-LD on every page.
- Version in URLs (`/docs/v3/...`) or visibly in page metadata.
- "Last verified against version X.Y" notes on tutorials.

Agents need to know what's current. Stale information silently degrades agent output.

### Canonical, persistent URLs

A URL that resolves the same way for years is more valuable than a clever URL that gets reorganised. Once an agent has cited your URL — or once a YouTube tutorial links to it — that URL should live forever (with redirects if needed).

### Schema.org / JSON-LD markup

Particularly:

- `Article` with `dateModified`, `dateCreated`, `author`.
- `HowTo` for tutorials.
- `FAQPage` for FAQ-style content.
- `APIReference` (less mature but emerging).
- `SoftwareApplication` for product pages.

Schema markup feeds structured data directly to AI crawlers. They use it.

### Clear, consistent terminology

Pick a canonical name for each concept and use it everywhere. "Workspace" and "project" and "tenant" should mean different things if they're three different things, or be merged to one term if they're synonyms. Agents learn vocabulary from your docs and use it in their responses.

### Q&A and how-to formatting

Headings phrased as questions ("How do I X?") match the way humans phrase queries to AI assistants. Agents can extract these passages cleanly into Q&A responses.

A useful exercise: imagine the actual question a developer would ask ChatGPT, and use that as the page heading.

### Avoid burying key information in images

Diagrams are great, but every critical fact in the diagram should also exist as text. Alt text is a minimum; better is a paragraph below the diagram that restates its key claims.

Agents are improving at OCR-from-image but text is still substantially more reliable.

### Don't gate docs

Login-walled docs are invisible to most AI crawlers. If your strategy is "developers will sign up to read the docs," you're optimising against AI-mediated discovery. Public docs are now table stakes.

### Keep `llms.txt` and `llms-full.txt` current

The standard is minimal but works. Auto-generate via Mintlify or similar, but audit periodically. See [`./llms-txt-standard.md`](llms-txt-standard.md).

### Provide the OpenAPI spec publicly

`/openapi.yaml` or `/openapi.json` at a stable URL. Agents read these heavily for SDK-equivalent code generation. The same goes for GraphQL schemas, Protobuf definitions, and JSON Schema files.

### Robots.txt: allow AI crawlers explicitly

Many teams accidentally block AI crawlers. Allow:

- `GPTBot` (OpenAI training)
- `OAI-SearchBot` (ChatGPT live retrieval)
- `ChatGPT-User` (ChatGPT's user-initiated browsing)
- `ClaudeBot` (Anthropic training)
- `Claude-Web` (Claude's live retrieval)
- `Claude-User`
- `PerplexityBot`
- `Perplexity-User`
- `Google-Extended` (Gemini training)
- `Googlebot` (Google + Gemini retrieval)

Each AI vendor publishes its bot names. Audit your `robots.txt` quarterly.

### Server-side rendering

Agents that don't execute JavaScript only see what's in the initial HTML. If your docs are client-rendered, ensure they have a server-side rendered version or pre-rendered HTML available to bots.

Most modern docs platforms (Mintlify, Docusaurus, Astro, Hugo, Nextra) handle this by default. Custom docs sites often don't.

### Embed code that agents can extract

Long code blocks formatted as plain Markdown code fences are easier for agents to extract than code embedded in special components or hidden inside collapsed accordions. Where you have a beautiful interactive component for humans, also provide a plain version for agents.

### Provide canonical "what is X?" answers

A short, factual "What is [your product]? What does it do? Who uses it? Why?" page that's stable for years. Agents extract from this page often when asked about your product.

### Provide canonical "X versus Y" comparisons

If your category has competitors, ChatGPT will be asked "What's the difference between X and Y?" If you have a fair, well-written comparison page, that's what gets cited. If you don't, AI assistants synthesise from whatever they find — often from competitors or third-party blogs, with mixed accuracy.

This is a delicate exercise: too sales-y and the agent will discount it; too cautious and it won't help. The standard is engineering-honest. Stripe's "comparing payment processors" content is the canonical example.

### Maintain ruthlessly

Stale docs are worse than missing docs for agents. A page that documents a deprecated endpoint produces agents that call the deprecated endpoint and confused human users when it fails. Audit quarterly. Remove or clearly mark deprecations.

## What humans still need on top of all of this

The agent-readable docs aren't sufficient for humans. Humans also need:

- Voice. Personality. A reason to care.
- Embedded video and animation.
- Vivid examples drawn from real use cases.
- An emotional reason to keep reading.

Mature docs sites in 2026 layer these on top of the machine-readable foundation. Stripe, Twilio, Vercel, Cloudflare, Mintlify-hosted Anthropic — all do this. The bones are agent-readable; the surface is human-engaging.

A useful mental model: write the agent-readable version first, audit it for completeness, then add the human-engaging layer on top. Don't try to do both at once — they pull in different directions.

## A practical checklist

For each high-traffic doc page:

- [ ] One concept per page.
- [ ] Lead paragraph contains the canonical answer.
- [ ] Code samples are complete and runnable.
- [ ] All languages your product supports have parity samples.
- [ ] Date and version visible.
- [ ] Schema markup present.
- [ ] Canonical URL.
- [ ] Linked from `llms.txt`.
- [ ] No login required.
- [ ] Robots allows AI crawlers.
- [ ] Renders without JavaScript.
- [ ] Reviewed and updated in the last 6 months.
- [ ] Has a voice / personality layer for humans (where appropriate).

The checklist is mundane; the compounding effect across hundreds of pages is substantial.

## See also

- [`./agent-experience-ax.md`](agent-experience-ax.md)
- [`./llms-txt-standard.md`](llms-txt-standard.md)
- [`./mcp-as-devrel-surface.md`](mcp-as-devrel-surface.md)
- [`./geo-aeo-for-devrel.md`](geo-aeo-for-devrel.md)
- [`../10-tactics/documentation-as-product.md`](../10-tactics/documentation-as-product.md)
- [`../08-tools/documentation-tools.md`](../08-tools/documentation-tools.md)