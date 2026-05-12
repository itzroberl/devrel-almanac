# Metrics in the AI Era

DevRel metrics changed in 2024–2026. The old funnel — page view, signup, activation — is still there, but new measurement surfaces have appeared, and several pre-AI metrics now mean different things. This file is a working framework.

## The three measurement surfaces

A useful mental model:

1. **Human-funnel metrics.** The classical DevRel measurement stack: traffic, signups, activation, retention, community engagement, revenue influence.
2. **Agent-surface metrics.** New: how AI assistants represent your product, MCP server adoption, tool-call success rate, agent-mediated activation.
3. **Cross-surface metrics.** How the two interact: what fraction of new signups arrived via AI mediation, how AI presence drives or fails to drive downstream activation.

Most DevRel teams in 2026 are still learning to instrument the agent-surface layer. The human-funnel layer is mature; the cross-surface layer is the analytical frontier.

## Human-funnel metrics that still matter (but now mean different things)

### Web traffic

Direct, organic, and referral traffic still matter. But "organic search" now includes traffic from AI assistants where they cite a link. Some segments:

- **Classical organic** — Google-search-mediated traffic to your docs and blog.
- **AI-assistant-mediated** — Visitors who arrived from a ChatGPT or Perplexity citation. Increasingly tracked separately. Many sources tag their click-throughs (`?utm_source=chatgpt.com` and similar appear in 2025–2026 referrer data).
- **Hidden AI influence** — Visitors who learned about you from AI but typed your URL directly. Unattributable but real.

Traffic data with AI-source tagging is starting to be widely available; most analytics platforms (GA4, Plausible, Fathom, PostHog) now break this out.

### Signups

Still useful. But the *source* attribution has shifted. A common 2025–2026 pattern: an onboarding question — "How did you hear about us?" — with explicit AI-assistant options.

The signal is noisy because developers often don't remember exactly which surface they encountered first, but the trend is real. Many AI-first DevRel teams report 10–30%+ of new signups citing AI mediation as part of their discovery, depending on category.

### Activation rate

Still the primary funnel metric. But two things changed:

1. **Agent-mediated activation.** Some developers activate having barely touched your docs because Cursor or Claude Code wrote the integration. Their *journey* to activation is different from the classical "read docs, write code" journey. Track them separately.
2. **TTFHW per source.** Activation rate from AI-mediated signups often differs from activation rate from search or referral. The AI-mediated developers sometimes activate faster (the agent did the work) or slower (the agent got confused and abandoned).

### Retention

Mostly unchanged, but worth noting that AI-mediated activation sometimes produces shallow integrations that fail under real production load, hurting retention. Track retention by activation source.

## Agent-surface metrics

### Share of Model / Share of Voice

For a defined set of category-relevant prompts (e.g., "What are the best vector databases?"), what percentage of AI-assistant responses mention your product?

How to measure:

- Choose 20–50 high-value prompts.
- Run them across ChatGPT, Claude, Perplexity, Gemini monthly.
- Track: mention rate, position (first / mid / late), sentiment, accuracy.
- Stratify by assistant — your visibility on Perplexity may differ wildly from your visibility on Gemini.

Tools that automate this:

- Profound (tryprofound.com), AthenaHQ, Otterly.AI, Peec AI, Sight AI, Pure Visibility.
- Methodology and accuracy vary; use them for relative tracking rather than absolute claims.

### Citation accuracy

When an AI assistant describes your product, how often is the description correct?

How to measure:

- For each cited mention, classify: fully accurate, partially accurate, inaccurate, hallucinated.
- Track over time and across assistants.
- Use mistakes as a feedback loop into your documentation and `llms.txt`.

### MCP server adoption

If you publish an MCP server (see [`./mcp-as-devrel-surface.md`](mcp-as-devrel-surface.md)):

- Active connected clients per day / week.
- Tool-call volume by tool.
- Tool-call success rate (was the agent able to use the tool without error?).
- Tool-call error rate by type.
- Average latency per tool.
- Top-failing tools (these are the candidates for redesign).

### Agent task completion rate

Inferred from server-side telemetry. When an agent invokes a sequence of your tools to complete a workflow, what fraction of sequences end in a successful business outcome (the message gets sent, the resource gets created, the query returns useful data)?

Hard to measure perfectly without telemetry from the agent client, but inferable from sequences of related tool calls.

### Documentation completeness for agents

A health metric for the agent-readable surface:

- Percentage of API endpoints documented in OpenAPI spec.
- Percentage of API endpoints exposed via MCP tools.
- `llms.txt` freshness (does it match current docs structure?).
- Code-sample coverage (every important API has at least one runnable Python and one runnable TypeScript example).
- Doc-update lag (how stale are pages compared to the API they describe?).

### AI-mediated NPS

When AI assistants describe your product, what is the *sentiment* of the description? "Stripe is the developer-friendly payments platform" is positive; "Twilio has historically had developer-friendly APIs but recent pricing changes have frustrated some developers" is mixed.

Tools that score this exist but are early. Manual coding of a sample is often the most reliable approach.

## Cross-surface metrics

### Attribution complexity

A developer in 2026 might:

1. Hear about your product from a podcast (channel: human).
2. Ask Claude about it (channel: AI-mediated).
3. Visit your docs (channel: classical).
4. Have Cursor write the integration (channel: agent-execution).
5. Sign up.
6. Activate.

Classical attribution models (first-touch, last-touch) don't capture this well. Some emerging approaches:

- **Multi-source attribution with explicit AI-mediated touchpoint.** Onboarding questions that ask developers about all the surfaces they encountered.
- **Cohort analysis by stated AI use.** "Among developers who said they consult ChatGPT regularly, our activation rate is X. Among those who don't, it's Y."
- **Influence-attribution panels.** Survey-based research into the path-to-purchase across surfaces.

### Authority-domain presence

A leading indicator of AI visibility:

- Number of mentions on Reddit / Hacker News / dev.to / Hashnode / authoritative newsletters / podcasts per quarter.
- Top-quartile YouTube tutorials mentioning your product.
- Sample-app repositories from third parties on GitHub.
- Stack Overflow archive presence (still cited even as the platform declines).

These are leading indicators because AI assistants increasingly weight them. Growth in authority-domain presence often predicts growth in AI citation rates with a quarter or two of lag.

### Funnel-to-funnel correlation

Are improvements in agent-surface metrics translating to improvements in human-funnel outcomes?

Specifically: does improving Share of Voice in AI assistants correlate with growth in signups? Does improving MCP server quality correlate with retention? These are open questions that DevRel teams in 2026 are still working out empirically.

## Metrics that mean less than they used to

A few things to deprioritise:

- **Raw blog page views.** Always limited; now further degraded because AI assistants may absorb the content and provide answers without referring the visitor.
- **Documentation page views.** Same. The page is now read by agents and summarised; the human may never visit.
- **Social media follower counts.** Continued vanity-metric concerns; less correlated with AI-mediated discovery.
- **Stack Overflow tag-watching activity.** As the platform declines, this is a noisy signal.

## The sentiment-telemetry gap

A genuine empirical caveat carried forward from broader research: developer *sentiment* about AI tools and AI-mediated experiences often diverges from *telemetry*. People say "the AI saved me time" while metrics show their code churn is higher, their PRs need more revision, their integrations are less robust.

For DevRel teams, the implication: surveys are insufficient. If your team's measurement strategy relies primarily on "we asked 100 developers and 80% said good things," you're probably overestimating. Supplement with behavioural data wherever possible — actual usage, actual retention, actual support volume, actual error rates.

This pattern has been documented across multiple 2024–2026 sources (Faros AI, DX research, JetBrains HAX study, Anthropic skill-formation research). The honest version of AI-era DevRel measurement leans more on telemetry and less on sentiment than its predecessors did.

## A practical scorecard

A representative 2026 DevRel monthly review might include:

| Metric | Type | What you want |
|---|---|---|
| New signups | Human funnel | Growth |
| TTFHW (median) | Human funnel | Decline |
| Activation rate, by source | Human funnel + cross-surface | Growth; convergence across sources |
| 90-day retention, by source | Human funnel + cross-surface | Growth; convergence |
| AI-mediated signup share | Cross-surface | Growth |
| Share of Model (top-20 prompts) | Agent surface | Growth |
| Citation accuracy (sampled) | Agent surface | High |
| MCP server tool-call success rate | Agent surface | High |
| MCP server adoption (active clients) | Agent surface | Growth |
| Documentation completeness score | Agent surface | High |
| Authority-domain mentions | Cross-surface | Growth |
| Community NPS | Human funnel | Steady or growth |
| DevRel-influenced ARR | Human funnel | Growth |

No team in 2026 perfectly tracks all of these. The honest aspiration is to instrument what you can and be candid about what you can't.

## What's still missing from the field

Two genuine measurement gaps as of mid-2026:

1. **No standard for cross-assistant AI visibility.** Profound, AthenaHQ, Otterly.AI, and others all report different numbers using different methodologies. The field needs a stable benchmark.
2. **No good model for agent-mediated business impact.** When Cursor writes 80% of a developer's integration code using your product, who gets credit? Your DevRel team's docs work? Cursor's AI? The developer? Attribution is fundamentally underdetermined.

These gaps will close over the next few years. For now, instrumented humility is the right posture.

## See also

- [`./geo-aeo-for-devrel.md`](geo-aeo-for-devrel.md)
- [`./agent-experience-ax.md`](agent-experience-ax.md)
- [`./mcp-as-devrel-surface.md`](mcp-as-devrel-surface.md)
- [`../04-metrics/metrics-overview.md`](../04-metrics/metrics-overview.md)
- [`../04-metrics/business-impact.md`](../04-metrics/business-impact.md)