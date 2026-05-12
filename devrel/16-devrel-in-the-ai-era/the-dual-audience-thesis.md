# The Dual Audience Thesis

The single organising idea of DevRel in 2026. **Developer Relations now serves two distinct audiences simultaneously, and the content that works for one rarely works for the other.**

## The two audiences

### Audience A — AI agents (execution)

Cursor, Claude Code, GitHub Copilot, Windsurf, Aider, Continue, Replit Agent, Bolt, and the growing class of background autonomous coding agents. They:

- Read your docs and code samples *programmatically*, often via retrieval-augmented systems.
- Are increasingly likely to consume your product's MCP server, its `llms.txt`, its OpenAPI spec, and your sample-app repositories *before* any human sees them.
- Generate code on a human developer's behalf, often without that human inspecting every page of your reference material.
- Need exhaustive, structured, machine-parseable content: complete examples (with imports), explicit version metadata, clean URL hierarchies, deterministic tool schemas, no half-finished snippets.

For this audience, your product is a set of *capabilities*. The work of DevRel is to make those capabilities cleanly *machine-readable*.

### Audience B — Human developers (inspiration)

The actual humans who decide whether to start using your product, whom to ask their AI assistant about, and which products to advocate for inside their teams. They:

- Form opinions on X (still), Bluesky (growing), YouTube (dominant), Reddit, Hacker News, Discord, podcasts, and at conferences.
- Increasingly never visit your homepage. The first time they encounter your product may be in an AI assistant's response, in a podcast guest's casual mention, or in a YouTube tutorial's sponsorship segment.
- Care about *who* says something. Trust transfers through human reputations — founders, advocates, content creators, peer recommendations.
- Are emotionally moved by aesthetics, voice, ambition, humour, vulnerability, and craft. Polished marketing reads as fake; rough authenticity reads as real.

For this audience, your product is a *story*. The work of DevRel is to make that story emotionally resonant, technically credible, and amplified by trusted voices.

## Why a single piece of content rarely serves both

Consider a quickstart guide. The optimal version for an AI agent:

- One concept per page.
- Complete, runnable code blocks with all imports.
- Explicit `dateModified`.
- Stable URL.
- No marketing copy.
- Linked from `llms.txt`.

The optimal version for a human:

- A vivid hook ("In five minutes, you'll have a working chat app").
- Personality. Maybe a joke. Maybe a screenshot.
- A reason to care, not just a procedure.
- Embedded video or animated demo.
- A clear, opinionated path with the author's voice.

Both can be true at once with effort — Stripe, Mintlify, Vercel, and Cloudflare's docs all approximate the synthesis — but the *strategic* mistake is to write one and hope it serves both. Many do, and produce content that is dry to humans and confusing to agents at the same time.

## The split practical operations look like in 2026

Mature DevRel teams have begun structuring their outputs around the split deliberately.

**For agents:**

- Authoritative reference documentation, structured cleanly.
- `llms.txt` and `llms-full.txt` files.
- Public MCP servers exposing the product's capabilities to AI agents.
- Sample-app repositories with disciplined READMEs and complete runnable code.
- OpenAPI / GraphQL schemas published canonically.
- Clear, deterministic error messages.
- Versioned URLs that survive site reorganisations.

**For humans:**

- Live-streamed coding sessions and engineering vlogs.
- Founder posts on X / Bluesky / LinkedIn with strong personal voice.
- YouTube tutorials embedded in trusted creators' channels.
- Podcast guest appearances by senior team members.
- Conference talks with vivid demos and personality.
- Vlogs, ship-week blog series, in-public build threads.
- Authentic Discord/Reddit/X conversations from named people.

A practical heuristic: **agents need completeness; humans need character**. Agents read everything; humans skim what they're already inclined to read. The two audiences require different writing.

## Why the split is structurally permanent

This isn't a short-term phenomenon. Four reasons it will persist:

1. **Agents and humans have different information needs.** Agents must reconstruct context they don't have. Humans bring their context but need emotional reasons to engage. These are different jobs.
2. **Agents' first-touch discovery is growing, not shrinking.** Throughout 2025–2026, the share of developer research initiated via AI assistants rather than Google grew substantially across nearly every survey that tried to measure it. This trend is structural — AI search is simply faster and better at first-pass evaluation than ten browser tabs.
3. **Humans choosing what to advocate for is not going away.** The most influential humans in any developer community will keep choosing what to recommend, what to integrate, what to defend in architecture meetings. AI assistants get their *signals* partly from those humans.
4. **Companies that excel at one will not necessarily excel at the other.** Building a great MCP server requires different muscles than building a beloved YouTube channel. Most DevRel teams will need both, and most will need to specialise to do them well.

## How the dual audience changes hiring

A DevRel team that designs for the split needs:

- **Agent-focused roles.** Often called Developer Experience Engineers, Documentation Engineers, MCP Engineers, or Agent Experience Engineers. Their work is structural: schemas, completeness, error-message design, machine-parseability.
- **Human-focused roles.** Developer Advocates, Educators, Content Creators, Community Managers. Their work is emotional and reputational: voice, presence, community trust, craft.

The unified "Developer Advocate who does everything" still exists, but is increasingly best for early-stage companies. Mature teams specialise.

See [`../02-foundations/hiring-and-career.md`](../02-foundations/hiring-and-career.md) and [`../02-foundations/job-openings.md`](../02-foundations/job-openings.md) for hiring patterns.

## How the dual audience changes measurement

Two largely-separate metric stacks:

**Agent-side:**

- **Share of Model / Share of Voice in AI assistants** — How often do ChatGPT, Claude, Perplexity, Gemini mention your product favourably when asked about your category? (See [`./geo-aeo-for-devrel.md`](geo-aeo-for-devrel.md).)
- **MCP server adoption** — Connections, tool-call volume, error rate.
- **Doc completeness / `llms.txt` health** — Coverage, freshness, machine-parseability.
- **Agent-mediated activation** — Developers who arrive having "tried it via Claude Code" or similar; success rate of agent-initiated integrations.

**Human-side:**

- Traditional content metrics, but with new emphasis on *authority signals*: named-author content, Discord active members, podcast-guest reach, conference speaker placements.
- Sentiment in named-developer-influenced channels (high-reputation X/Bluesky accounts, prominent YouTubers, top podcasts).
- Community-led growth signals (organic mentions, fork-and-build patterns, OSS contributor growth).

The integrated dashboard is the goal. Most teams in 2026 have one or the other working, not both.

## What goes wrong when teams collapse the dual audience back into one

Common failure modes from observed 2025–2026 programs:

- **"AI-readable" treated as the only goal.** Docs become flat, voiceless, optimised for parsing. Human developers find them sterile and never form an opinion about the product as a brand.
- **"Authenticity" treated as the only goal.** Quirky human-voice content fills the website. AI agents get inconsistent answers and stop citing the product. Developers who arrive via AI assistants encounter contradictions.
- **One person doing both audiences.** Burnout and quality collapse. The energy required to operate a YouTube channel is incompatible with the discipline required to maintain an exhaustive `llms-full.txt`.
- **Pretending agents aren't an audience.** Some old-school DevRel teams have stayed in pure-content mode. They are losing share of AI-mediated discovery to competitors who treat agents as first-class users.

## The synthesis claim

The companies winning the AI-era developer-mindshare battle treat their product as a thing that needs to be *both* legible to machines and *loved* by humans. They invest in both stacks. They staff for both. They measure both. They accept that the work split is permanent and design around it.

That is the dual audience thesis. The rest of this section unpacks what each side of the split actually requires in practice.

## See also

- [`./llm-mediated-discovery.md`](llm-mediated-discovery.md)
- [`./inspiration-stays-human.md`](inspiration-stays-human.md)
- [`./agent-experience-ax.md`](agent-experience-ax.md)
- [`./documentation-for-agents.md`](documentation-for-agents.md)
- [`./early-signals-what-works.md`](early-signals-what-works.md)