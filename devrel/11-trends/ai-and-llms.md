# AI and LLMs: How They Reshape Developer Relations

> **For deeper treatment, see Section 16: [DevRel in the AI Era](../16-devrel-in-the-ai-era/README.md)** — a dedicated, in-depth section covering the dual-audience thesis, LLM-mediated discovery, `llms.txt`, MCP as DevRel surface, Agent Experience (AX), GEO/AEO, vibe coding, metrics, perspectives and debates, critical takes, and early signals of what works. This page remains as a higher-level trend summary.

The single most disruptive shift in DevRel since the discipline professionalised. Within a window of less than three years (late 2022 through 2026), AI changed how developers discover products, learn technologies, evaluate options, consume documentation, and write code. DevRel teams that have adapted are operating differently than they did in 2022; teams that haven't are losing influence quietly.

## The shift in three observations

1. **LLMs are now the first-touch developer discovery surface.** Many developers now research products through ChatGPT, Claude, or Perplexity before they search Google. A DevRel team whose product is poorly represented in these surfaces is invisible at the top of the funnel.
2. **Documentation is consumed by AI as much as by humans.** Copilot, Cursor, Claude Code, and other agentic coding tools ingest documentation to write code on developers' behalf. Docs that aren't well-structured for machine consumption fail their AI readers, who in turn fail the developer.
3. **Developers themselves are partly agentic.** Code is increasingly written by AI under developer supervision rather than by developers directly. The developer's job is shifting toward management of execution loops. DevRel must serve both the developer and the agent.

## Implications for DevRel work

### Documentation must serve AI agents

Practical implications:

- **Structured Markdown.** Clear heading hierarchy, consistent formatting.
- **Self-contained code examples.** All imports, all setup, runnable as-is.
- **Explicit versioning.** AI agents need to know what's current.
- **Avoid burying key info in images.** Without alt text, AI doesn't see it.
- **Canonical URLs.** AI agents store links; stable URLs survive.
- **`llms.txt` or equivalent.** A growing convention: companies publish a top-level `llms.txt` indexing AI-readable canonical pages, modelled loosely on `robots.txt`. Anthropic, Mintlify, and others have implemented and promoted this pattern.
- **Documentation site maps optimised for AI ingestion** as well as for human navigation.

### Sample apps are AI training data

A high-quality public sample app repository becomes:

- Training data for next-generation models.
- Retrieval-augmented reference for current AI assistants.
- The canonical "how to use product X" the AI tells developers.

Many AI-era DevRel teams now design their sample-app strategy *explicitly* around AI ingestion: more samples, smaller scope per sample, clearer code style, exhaustive README.

### Model Context Protocol (MCP)

Launched by Anthropic in November 2024, MCP is an open standard for connecting AI systems to external applications and data sources.

Key data points:

- **From ~100 servers in November 2024 to 17,000+ by early 2026.**
- Cross-vendor support: OpenAI, Google, and Anthropic all support MCP.
- For developer products, an MCP server is a new DevRel surface — exposing the product's capabilities directly to AI agents.

For DevRel teams, the question is no longer "should we have an MCP server?" but "what does our MCP server expose, and how do we make sure AI agents using it succeed?"

### Discovery surfaces have multiplied

A DevRel team in 2022 had to optimise for Google, Twitter, conferences, and a few content sites. A DevRel team in 2026 must additionally optimise for:

- ChatGPT, Claude, Perplexity (LLM-mediated search).
- AI-powered IDE assistants (Cursor, Copilot, Claude Code).
- Coding agents (Devin, OpenAI's agents, Claude Code agents).
- AI-driven research workflows.

Different surfaces favour different content. Long-form authoritative writing increases the likelihood of being cited by AI assistants; short social posts that worked on X have minimal AI-citation value.

### Sentiment in AI assistants matters

If you ask ChatGPT or Claude about your product, what does it say? The answer is a meaningful DevRel surface in 2026. Teams check it regularly across the major assistants.

Mechanisms by which AI assistants form views:

- **Training data.** Long-form authoritative content (your docs, your blog, third-party reviews).
- **Real-time retrieval.** What AI search surfaces for your product.
- **User feedback loops.** Some assistants reflect what users have asked recently.

If the AI is wrong about your product, the fix usually involves clearer authoritative content the AI can ingest, plus engagement with the platform if available.

## Implications for content strategy

| Content type | Pre-2023 emphasis | 2024–2026 emphasis |
|---|---|---|
| Reference docs | Human readability | Human readability + AI ingestion |
| Quickstarts | TTFHW for human | TTFHW for human + AI completing tasks |
| Code samples | Educational | Educational + AI training data |
| Blog posts | SEO | SEO + AI citation likelihood |
| Conference talks | In-room impact + replay | In-room impact + replay + AI-searchable transcripts |
| Newsletter | Subscriber relationship | Same |
| Sample apps | Demonstrative | Demonstrative + AI agent reference |

## Implications for developer education

The role of developer educators is shifting:

- **Less "how to use the SDK basics"** (AI assistants now handle these explanations).
- **More "how to architect a working system"** (AI is weaker at strategic decisions).
- **More "how to evaluate trade-offs"** (AI hallucinates with confidence; the educator's job is to teach the developer to detect this).
- **More content about working *with* AI tools to build with your product** — meta-content about the new development workflow.

## Implications for community

- **Real-time community help is partly replaced by AI assistants.** Many questions that used to flood Discord channels now go to ChatGPT first.
- **Communities are becoming places for harder questions** that AI couldn't answer.
- **The role of expert community members has elevated.** They are the place a developer goes when AI failed them.

This is not all loss. Healthy communities are more focused; expert contribution is more valued.

## Implications for advocacy

- **Advocates' content has new audiences.** Every video, blog, and tweet is now potential training data and citation source.
- **Authority signals matter more.** AI assistants weight authoritative sources; named experts with reputation get cited more than anonymous posts.
- **Real-time presence matters less.** A great podcast appearance is more durable than a tweet thread.
- **Open-source visibility has compounding value.** AI agents reference GitHub heavily.

## Tools and agents in the DevRel workflow itself

DevRel teams use AI tools internally:

- **Content generation assistance.** Draft posts, edit, summarise.
- **Community sentiment analysis at scale.** Tools like Common Room layer AI on top of conversation data.
- **Personalised outreach.** Identifying and engaging individual community members.
- **Doc gap detection.** Asking AI to identify questions docs don't answer.
- **Translation.** Producing localised content efficiently.

The principle that works: AI augments DevRel; it does not replace the trust, authenticity, and technical credibility that the function fundamentally produces.

## AI-engineering as a DevRel category

Beyond AI's effect on DevRel practice, AI has produced a substantial new category of developer products requiring DevRel:

- Foundation-model providers (OpenAI, Anthropic, Google, Cohere, Mistral, etc.).
- Open-source model hubs (Hugging Face).
- AI orchestration tools (LangChain, LlamaIndex, Haystack).
- Vector databases (Pinecone, Weaviate, Chroma, Qdrant).
- AI infrastructure (Modal, Together AI, Replicate, RunPod).
- Coding agents and tools (Cursor, Aider, Continue, GitHub Copilot, Claude Code).

These companies built DevRel functions over 2023–2026 from scratch. The category employs a substantial fraction of the laid-off DevRel professionals from the 2022–2024 contraction and has effectively become a new sub-field with its own conferences (AI Engineer Summit), publications (Latent Space), and senior practitioners (Logan Kilpatrick, Romain Huet, swyx, Harrison Chase, Jerry Liu).

See [`../05-companies/ai-companies.md`](../05-companies/ai-companies.md).

## What gets harder

- **Attribution.** AI-mediated discovery makes attribution to specific DevRel activities harder.
- **Voice.** AI-assisted content tends to converge on average prose; distinctive voice is harder to maintain at speed.
- **Original research.** Long-form posts compete with AI-generated competitive content; the bar is higher.
- **Real-time community help.** When AI is the first stop, only the hardest questions reach humans, which can overwhelm the community team.

## What gets easier

- **Content production volume.** A team can produce more drafts faster.
- **Personalisation.** Tailoring content to specific developer segments.
- **Multi-language reach.** Translation and localisation are cheaper.
- **Analytics.** Sentiment, gap analysis, and pattern detection are more tractable.

## The agentic-experience (AX) question

A specific 2024–2026 development: companies are beginning to think about **agent experience** — the experience that AI agents have when interacting with their APIs, docs, and tools — as a deliberate design surface, parallel to developer experience.

This shows up in:

- API design that is easy for agents to use (predictable, well-typed, well-documented).
- Error messages designed for both human and AI consumption.
- Authentication flows that work well for agentic access.
- Rate limits and quotas designed with agent patterns in mind.

For DevRel teams at AI-adjacent infrastructure companies, AX is becoming as deliberate a function as DX.

## See also

- [`./plg-and-devrel.md`](plg-and-devrel.md)
- [`./devex-movement.md`](devex-movement.md)
- [`./future-directions.md`](future-directions.md)
- [`../05-companies/ai-companies.md`](../05-companies/ai-companies.md)
- [`../10-tactics/documentation-as-product.md`](../10-tactics/documentation-as-product.md)
- [`../09-platforms/stack-overflow.md`](../09-platforms/stack-overflow.md)