# Generative Engine Optimisation (GEO) and Answer Engine Optimisation (AEO) for DevRel

If SEO was the discipline of being found by search engines, **GEO** and **AEO** are the disciplines of being cited by AI assistants. The two terms overlap in practice but differ in nuance:

- **Generative Engine Optimisation (GEO).** Optimising for citation and inclusion when generative AI systems (ChatGPT, Claude, Perplexity, Gemini) produce answers. The headline metric is *Share of Model* or *Share of Voice* — how often your brand is mentioned in responses to category-relevant prompts.
- **Answer Engine Optimisation (AEO).** Structuring content so AI answer engines can extract clean, direct answers. Overlaps heavily with classical SEO best practices (Q&A formatting, schema markup) but tunes them for conversational extraction rather than ten-blue-links ranking.

For developer products, both matter. The discipline is still young, the data is noisy, but the practices that emerged through 2025–2026 are concrete enough to be worth doing.

## Where AI assistants get their answers from

A practical breakdown:

| Assistant | Primary index / retrieval source | Notes |
|---|---|---|
| **ChatGPT** | Bing (via OAI-SearchBot for live retrieval); training data | Bing Webmaster Tools verification matters; allow `OAI-SearchBot` separately from `GPTBot` (training-data crawler) |
| **Perplexity** | Live web retrieval (PerplexityBot); curated high-trust domains | Citations shown inline; surfaces only sites it considers high-authority |
| **Gemini** | Google Search index + Google's broader retrieval | Strong SEO is prerequisite; YouTube videos with `VideoObject` schema often cited for "how-to" queries |
| **Claude** | Live web retrieval (ClaudeBot, Claude-User); training data | Anthropic has not published detailed retrieval mechanics |
| **Copilot (Microsoft)** | Bing; specific developer-tool data | DevTools-specific context |

DevRel teams optimising for AI visibility need to satisfy multiple systems, each with slightly different mechanics. There is no single GEO playbook that works equally well across all of them.

## Foundational GEO practices

These work across most assistants:

### 1. Authoritative, substantive content

AI assistants weight authority strongly. Authority signals include:

- Substantive, original content (engineering posts that actually say something).
- Citations from other authoritative sources.
- Long-running domain history.
- Wikipedia presence (if applicable).
- Mentions in trusted publications.

What doesn't work: shallow content optimised purely for keyword stuffing. AI assistants discount this aggressively.

### 2. Clear semantic structure

- Headings as questions ("How do I X?") or canonical topic titles.
- One concept per page.
- Lead with the answer in the opening paragraph.
- Bullet-list and table formats where appropriate.

### 3. Schema.org / JSON-LD markup

For developer-product content particularly useful:

- `Article` with `dateModified`, `author`, `publisher`.
- `HowTo` for tutorials.
- `FAQPage` for FAQ-style content.
- `SoftwareApplication` for product pages.
- `Organization` and `Product` schema for brand consistency.
- `VideoObject` for embedded videos.

Schema feeds AI crawlers structured data directly, bypassing HTML-parsing ambiguity.

### 4. Crawler permissions

Audit your `robots.txt` to ensure AI crawlers can read what you want them to read. See [`./documentation-for-agents.md`](documentation-for-agents.md) for specifics. Many teams accidentally block AI crawlers while trying to block aggressive SEO scrapers.

### 5. Cross-platform consistency

Your product's description on your homepage, your docs site, your README, your Wikipedia entry, and on third-party listings should be consistent. When AI assistants encounter contradictions, they tend to flag uncertainty or pick less authoritative sources.

### 6. Freshness signals

`dateModified` updated when content is updated. Versions referenced explicitly. Deprecated content marked as such or removed. AI assistants trained more recently or that retrieve live weight fresh content more heavily.

## Developer-product-specific tactics

Beyond general GEO, several practices that matter especially for DevRel:

### Maintain a canonical "What is [product]?" page

A short, factual, well-structured page that answers the basic question. AI assistants extract from this page heavily when asked about your product. Don't bury this content inside a marketing-driven homepage; have a clean answer page.

### Maintain "X vs Y" comparison content

Engineering-honest, fact-led comparison content for the top three or four competitors in your category. AI assistants are asked "what's the difference between X and Y?" constantly, and they cite whoever has the best comparison content.

The trick is honesty. AI assistants discount obviously biased comparison content. Stripe-style fair comparisons get cited; product-pitch comparisons get ignored.

### Cultivate third-party authority

Get mentioned positively on:

- Reddit (relevant subreddits — weighted heavily by some AI assistants).
- Hacker News (substantive Show HN launches and threads).
- dev.to and Hashnode posts by independent developers.
- YouTube tutorials by trusted educators.
- Podcasts with transcripts.
- High-authority newsletter mentions (Console.dev, TLDR, etc.).
- Stack Overflow answers (the archive is still cited despite the platform's decline).

These are the second-order authority signals AI assistants weight. DevRel teams that cultivate organic mentions across these channels see better AI-citation performance than teams that rely only on owned content.

### Sponsor or contribute to YouTube content with transcripts

YouTube transcripts are heavily used by Gemini (and indirectly by other assistants via training data). A well-produced YouTube tutorial with a thorough transcript can produce more AI-mediated visibility than a blog post on the same topic.

The trade-off: video is expensive to produce. The DevRel teams winning at GEO in 2026 invest in video as a deliberate AI-visibility strategy, not just as a brand exercise.

### Publish on platforms AI assistants trust

Your own domain is good but not enough. Cross-publish (with canonical URLs) to:

- dev.to and Hashnode.
- LinkedIn long-form posts and newsletters.
- Substack or Beehiiv.
- Medium (less weighted than 2018–2020 but still cited).
- Industry publications (TheNewStack, InfoQ, occasional Smashing Magazine, etc.) where the editors will accept submissions.

## Tools for monitoring brand presence in AI

A new tools category emerged in 2024–2026. Among the better-known products:

- **Profound (tryprofound.com).** Measures brand visibility across major AI assistants; tracks Share of Model and competitive positioning.
- **AthenaHQ.** AI-search analytics.
- **Otterly.AI.** Similar tracking of AI-mention frequency.
- **Peec AI.** Tracks brand mentions across AI engines.
- **LLMrefs.** Citation and authority tracking.
- **Goodie tools.** GEO-focused stack.
- **Sight AI (trysight.ai).** AI search visibility tracking.
- **Pure Visibility.** GEO platform.

The category is young, the methodologies vary, and the tools sometimes report wildly different numbers. Best use is for relative tracking (am I getting more or less visible over time?) rather than absolute measurement.

## Reasonable metrics for DevRel teams

Among the metrics worth tracking:

- **Share of Voice / Share of Model.** Across a defined set of category-relevant prompts, what percentage of responses mention your brand?
- **Citation accuracy.** When AI assistants describe your product, what fraction of technical claims they make are correct?
- **AI-mediated signup attribution.** When you ask new signups how they heard about you, what share say "ChatGPT," "Claude," "Perplexity," or "an AI assistant"?
- **Authority-domain presence.** Are you mentioned on Reddit, HN, GitHub READMEs, prominent YouTube channels?
- **Citation variance.** AI citations fluctuate; high variance month-to-month suggests fragile positioning, while stable citations suggest durable authority.

## Caveats

Two important honest acknowledgements:

1. **AI citations are noisy.** Multiple analyses through 2026 report 40–60% monthly variance in AI citations across the same prompts. AI assistant models update frequently; context windows shift; retrieval algorithms change. Treat your GEO position as a trend, not a fixed measurement.
2. **AI assistants do not always cite their sources.** ChatGPT often answers without showing links. Your AI-mediated influence on developers may be substantial and invisible. Measure what you can; don't pretend the unmeasurable is zero.

## What to deprioritise

A few practices that wasted DevRel teams' time in 2024–2025 and don't appear worth the effort in 2026:

- **Stuffing keywords into AI-readable surfaces.** AI assistants discount this.
- **Generating large volumes of AI-written content optimised for "AI search."** This often hurts authority because AI assistants weight original human-authored content.
- **Treating `llms.txt` as a complete GEO strategy.** It's one signal, not the strategy.
- **Optimising only for ChatGPT.** Each assistant has different retrieval mechanics; over-specialisation on one creates fragility.

## A 90-day GEO program for a DevRel team

Months 1: Baseline. Run prompts across all major assistants. Audit `robots.txt`. Run a schema.org audit. Verify Bing Webmaster Tools setup. Identify three to five high-value pages on your domain that need rewriting.

Month 2: Optimise. Rewrite the high-value pages with the practices above. Publish canonical "what is X?" and "X vs Y" pages. Coordinate one major YouTube collaboration with a trusted educator. Ensure all SDK READMEs have date / version / canonical URLs.

Month 3: Measure and iterate. Re-run prompts. Look for delta. Treat as ongoing — month 3 baseline becomes month 6 review.

## See also

- [`./llm-mediated-discovery.md`](llm-mediated-discovery.md)
- [`./documentation-for-agents.md`](documentation-for-agents.md)
- [`./metrics-in-ai-era.md`](metrics-in-ai-era.md)
- [`../09-platforms/youtube-tech.md`](../09-platforms/youtube-tech.md)
- [`../10-tactics/content-strategy.md`](../10-tactics/content-strategy.md)