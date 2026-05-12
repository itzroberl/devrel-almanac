# Early Signals: What Works

The most useful question to ask, after all the framing and debate: *which DevRel approaches are demonstrably producing outcomes in 2025–2026?*

This file collects concrete patterns observed across DevRel programs that are visibly succeeding in the AI era. Each is grounded in observable practice at specific companies, not in speculation.

## 1. Cookbook repositories as a primary DevRel deliverable

**Pattern.** A public GitHub repository organised as a collection of small, complete, runnable recipes covering different use cases of your product. Each recipe is self-contained, has a `README.md`, and demonstrates one thing clearly.

**Why it works.**

- AI agents read the recipes as training data and retrieval-augmented context.
- Human developers clone individual recipes as starting points for their own integrations.
- The repository becomes a single source of canonical patterns that AI assistants reference when asked "how do I do X with [your product]?"
- The cost per recipe is low; the compound value is high.

**Notable exemplars.**

- **OpenAI Cookbook** (github.com/openai/openai-cookbook). The defining example. Hundreds of recipes. Substantial external-contributor community.
- **Anthropic Cookbook.** Direct competitor and arguably the more curated version. Recipes are tightly scoped, well-tested, and include explicit version metadata.
- **Stripe Samples** (github.com/stripe-samples). Per-language repositories with complete deployable examples.
- **Vercel Templates** (vercel.com/templates). Templates that can be deployed with a click.
- **LangChain templates** and **LlamaIndex examples**. Recipe-style code reflecting common integration patterns.

The pattern is so dominant that "ship a cookbook" is now a default early-stage DevRel deliverable at AI-adjacent companies.

## 2. Founder-led written content

**Pattern.** Founders and senior technical leaders write under their own names, on topics adjacent to but not always about their product. The content is substantive, opinionated, sometimes long, and intellectually serious.

**Why it works.**

- Authenticity. AI cannot replicate Patrick Collison's voice; Mitchell Hashimoto's architectural reasoning; Guillermo Rauch's framing of frontend ergonomics; Clem Delangue's view of open-source community.
- Sustained authority. A decade of founder-written essays compounds into a kind of authority no marketing budget can buy.
- AI citation effect. AI assistants weight authority sources heavily; founder-authored content tends to be authoritatively cited.

**Notable exemplars.**

- **Stripe Press.** Stripe's broader intellectual project — books, essays, sustained long-form publishing.
- **Mitchell Hashimoto's personal blog** (mitchellh.com). Post-HashiCorp writing on systems software and Ghostty terminal-emulator work.
- **DHH's writing across two decades.** Hey, Basecamp, REWORK, his personal site.
- **Sam Altman's blog and OpenAI announcements.** Even at scale, the voice is identifiable.
- **swyx's writing across his personal site and Latent Space.** Sustained essay-driven authority.

The pattern requires founders willing to write, which not all are. Where founders won't write, senior technical leaders can substitute — but the effect is weaker than founder-led writing.

## 3. Build-in-public Launch Weeks

**Pattern.** A coordinated multi-day or multi-week launch where the company ships visibly, in public, with daily blog posts, demos, and community engagement. Several features ship per week; the energy is sustained; the audience is engaged across the full period.

**Why it works.**

- Sustained presence beats sporadic announcement.
- Creates anticipation; builds community momentum.
- Each day's content is shareable and amplifiable.
- AI assistants citing your product encounter rich, coherent, dated content covering many capabilities at once.
- Functions as a forcing function for the engineering and product teams to ship.

**Notable exemplars.**

- **Supabase Launch Weeks** (every few months since 2020). Probably the canonical example. Multiple features per week, daily posts, livestreams, community participation.
- **Cloudflare Developer Week.** Annual, content-saturated week of new product announcements.
- **Vercel Ship.** Annual customer-event-as-launch-week.
- **Linear's smaller launch series.**

Pattern adoption across the developer-product industry is rapid through 2024–2026.

## 4. MCP server as a first-class product surface

**Pattern.** Publishing an MCP server alongside your SDK and CLI, treating it as a maintained product. Tool naming is deliberate; documentation is complete; updates ship with the product.

**Why it works.**

- Agents can invoke your product across all AI clients (Claude Code, Cursor, Windsurf, ChatGPT, Gemini).
- The MCP server is increasingly the entry point for agentic developer work; without one you're invisible to that audience.
- The discipline of writing clean tool descriptions improves the rest of your API documentation as a side effect.

**Notable exemplars.**

- **GitHub MCP, Sentry MCP, Cloudflare MCP, Linear MCP, Notion MCP, Stripe MCP, Supabase MCP, Snowflake MCP** — partial list of major developer-product MCP servers in 2026.
- **Vercel AI SDK** with MCP support.
- **Microsoft Playwright MCP** for browser automation.

See [`./mcp-as-devrel-surface.md`](mcp-as-devrel-surface.md).

## 5. Disciplined `llms.txt` plus `llms-full.txt` plus OpenAPI plus schema

**Pattern.** A clean, well-maintained set of machine-readable surfaces:

- Auto-generated `llms.txt` and `llms-full.txt` (often via Mintlify or similar).
- Publicly accessible OpenAPI spec at a stable URL.
- Schema.org markup on key product pages.
- Consistent canonical URLs across the docs site.
- Robots.txt explicitly allowing the major AI crawlers.

**Why it works.**

- Cumulatively improves AI assistants' ability to extract correct information about your product.
- The discipline of maintaining these files keeps documentation hygiene high.
- Even if `llms.txt`'s direct AI-citation effect is uncertain, the surrounding practices produce measurable improvements.

**Notable exemplars.**

- **Anthropic docs** at docs.anthropic.com — clean `llms.txt` and `llms-full.txt`, well-structured pages, consistent vocabulary.
- **Mintlify-hosted documentation generally** — Anthropic, Cursor, Resend, Perplexity, dozens of others.
- **Stripe docs** — long-standing best-in-class documentation with strong AI-readable structure.
- **Vercel docs and Next.js docs** — clean, well-versioned, machine-friendly.

## 6. Sponsored YouTube placements on trusted channels

**Pattern.** Paying for sponsored segments on YouTube channels whose audience overlaps your ICP. The segments are honest, often demonstrate the product in use, and feature the channel's own creator vouching for the product.

**Why it works.**

- Trust transfer. Fireship saying "we've integrated X" is more credible than X's own marketing.
- Compounding. Sponsored videos live on YouTube for years, accumulating views and citations into AI assistants' training data.
- Scale. The top channels reach millions per video.

**Notable exemplars.**

- **Fireship sponsorships.** *The Code Report* segments and product features regularly drive substantial signup spikes.
- **ThePrimeagen sponsorships.** Direct engineer-to-engineer credibility.
- **Theo Browne (t3.gg).** Strong frontend-developer reach.
- **Web Dev Simplified, Net Ninja, NetworkChuck, ByteByteGo** — high-conversion channels for various developer products.

Approximate rates are documented in [`../09-platforms/youtube-tech.md`](../09-platforms/youtube-tech.md). The pattern is well-established: well-targeted YouTube sponsorships produce more activation per dollar than nearly any other paid channel.

## 7. Podcast guesting by senior team members

**Pattern.** Senior engineers, founders, and DevRel leaders appearing as guests on respected developer podcasts. Often discussing topics adjacent to but not strictly about their product. The product comes up naturally in conversation.

**Why it works.**

- Long-form trust. A 60-minute conversation produces depth of impression no short-form content matches.
- Cross-pollination. The podcast's existing audience meets your team's voice.
- Durable. Episodes live on, accumulating listeners over years.
- AI assistants weight transcripts and episode descriptions; episode show notes are particularly well-indexed.

**Notable exemplars.**

- **Latent Space appearances.** For AI-adjacent products, an appearance with swyx and Alessio Fanelli is the canonical conversion event.
- **The Changelog appearances.** Broad industry reach; Adam Stacoviak and Jerod Santo run high-quality interviews.
- **Syntax.fm appearances.** Front-end audience.
- **Acquired episodes.** For broader company-strategy reach (less developer-focused but high-prestige).
- **Community Pulse appearances.** For DevRel-practitioner audience (i.e., influencing other DevRel teams).

## 8. AI Engineer Summit / specialised conference presence

**Pattern.** Companies whose products serve AI Engineers invest deliberately in specialised AI-engineering conferences and channels rather than generic developer events.

**Why it works.**

- Audience concentration. The AI Engineer Summit, MLOps World, NeurIPS, Ray Summit, GTC, Snowflake Summit AI tracks, Databricks Data + AI Summit — these concentrate the exact audience that matters for AI-infrastructure products.
- Authority transfer. Speaking at AI Engineer Summit signals you are taken seriously by the practitioner community.
- Connections compound. Senior AI Engineers meet your team in person; the relationships drive enterprise adoption.

**Notable exemplars.**

- **Pinecone, Weaviate, Chroma, Qdrant** all show up consistently at AI-engineering conferences.
- **OpenAI, Anthropic** maintain visible AI Engineer Summit presence.
- **Modal, Together AI, Replicate** focus most of their DevRel event spend on AI-Engineer-specific conferences.

## 9. Discord office hours and structured community presence

**Pattern.** Predictable, regular times when company engineers are visibly available in the community Discord (or equivalent). Office hours; AMAs; bug-triage hours; "ask me anything about X" themed sessions.

**Why it works.**

- Reliability. Members know that on Thursdays at 3pm a real engineer will be available.
- Trust. Repeated personal presence over months builds relationships.
- Knowledge accumulates. Common questions get answered repeatedly; community members start answering for each other.
- Differentiates from AI. The "I'm here in person" presence is the thing AI can't fake.

**Notable exemplars.**

- **Vercel's Next.js Discord** with regular Lee Robinson and team presence.
- **Supabase Discord** with founder participation.
- **Cloudflare Discord** for Workers / Pages community.
- **Anthropic Discord** for developer community.
- **The Rust language community's Zulip** (technically not Discord, same pattern).

## 10. Open-source maintainer sponsorship and ecosystem investment

**Pattern.** Companies investing financially or via paid roles into open-source projects their product depends on or competes with. GitHub Sponsors, Tidelift, direct grants, hiring maintainers.

**Why it works.**

- Authority signal. Companies that fund open source visibly earn community trust.
- Supply chain. Maintained dependencies are more reliable; sponsored maintainers can fix things you depend on.
- Recruitment pipeline. Senior open-source maintainers are often the best hires.

**Notable exemplars.**

- **Cloudflare's open-source funding** across multiple projects.
- **Sentry's open-source dependency fund.**
- **Vercel's funding of Next.js and many adjacent JS ecosystem projects.**
- **The various MOSS (Mozilla Open Source Support) grants** historically, plus successor programs.

## 11. Treating documentation as a versioned product with a roadmap

**Pattern.** Documentation has an owner, a quarterly roadmap, version controls, named writers, and measurable goals (TTFHW, completion rate, search-query coverage).

**Why it works.**

- Compound improvement. Quarterly investments stack.
- AI-readability is essentially documentation hygiene. Teams that treat docs as a product naturally produce machine-readable surfaces.
- Differentiates from one-off content production.

**Notable exemplars.**

- **Stripe's documentation** — long-standing best-in-class.
- **Mintlify-hosted documentation** at most AI-era developer products.
- **Twilio's documentation** — substantial team and roadmap.
- **AWS, Google Cloud, Azure** all maintain documentation teams that operate like product teams.

## 12. Founder or CEO running the launch personally

**Pattern.** Major launches are anchored by the CEO or founder doing the keynote, blog post, demo, and post-launch Q&A personally. Marketing supports but does not own.

**Why it works.**

- Authenticity at scale. The biggest launches need the most authority; founders bring that authority.
- The launch becomes a story about the company's vision, not just a product announcement.
- Press, podcasts, and community amplify founder-led launches more than marketing-led ones.

**Notable exemplars.**

- **OpenAI DevDay (Sam Altman, Greg Brockman, etc.).** Founder-led format is the default.
- **Anthropic launches.** Dario Amodei, Mike Krieger, Alex Albert all visible at major launches.
- **Vercel launches.** Guillermo Rauch leads.
- **Linear releases.** Founders consistently in the foreground.

## 13. Combining a fast-iterating cookbook with quarterly long-form essays

**Pattern.** Day-to-day content production focuses on cookbook recipes (small, complete, runnable). Long-form quarterly essays focus on strategic positioning, architectural arguments, opinionated takes on the field.

**Why it works.**

- Cookbook recipes serve agents and time-pressed developers.
- Essays serve senior decision-makers and provide AI-citable authority content.
- The two together produce a comprehensive surface: tactical answers when needed, strategic context when wanted.

**Notable exemplars.**

- **Anthropic's blog combined with cookbook.** Strategic essays plus tactical recipes.
- **OpenAI's blog plus Cookbook.**
- **Vercel's product launches plus Lee Robinson's longer-form pieces.**
- **LangChain blog plus templates repository.**

## Patterns that don't show up here (and arguably should)

Several patterns that are common in 2024–2026 marketing advice but for which the evidence of effectiveness is genuinely weaker:

- Aggressive `llms.txt` optimisation (covered with appropriate scepticism in [`./llms-txt-standard.md`](llms-txt-standard.md)).
- "AI-generated content at scale" approaches (mostly failure mode).
- Generic "AI thought leadership" content from companies without genuine AI products.
- Heavy reliance on a single AI-search visibility tool.

The pattern: things that show up here have working empirical exemplars at multiple companies. Things that don't are either too new, too unproven, or too dependent on specific company context to recommend confidently.

## See also

- [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md)
- [`./perspectives-and-debates.md`](perspectives-and-debates.md)
- [`./critical-takes.md`](critical-takes.md)
- [`./inspiration-stays-human.md`](inspiration-stays-human.md)
- [`./metrics-in-ai-era.md`](metrics-in-ai-era.md)
- [`./mcp-as-devrel-surface.md`](mcp-as-devrel-surface.md)
- [`./documentation-for-agents.md`](documentation-for-agents.md)