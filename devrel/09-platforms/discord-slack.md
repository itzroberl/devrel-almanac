# Discord and Slack

The two dominant real-time chat platforms for developer communities. Choosing between them is one of the most consequential decisions a DevRel team makes about its community infrastructure. See also [`../08-tools/community-platforms.md`](../08-tools/community-platforms.md) for the broader platform landscape.

---

## Discord

### History

- **Founded.** 2015 by Jason Citron and Stanislav Vishnevskiy.
- **Origin.** Built for gamers; gradually pivoted toward broader community use from 2019 onward.
- **Scale.** 200M+ monthly active users; one of the largest real-time communication platforms globally.

### Why it became the modern developer default

- **Free for community use.** No per-user pricing.
- **Servers + channels + threads** maps cleanly to a multi-topic developer community.
- **Voice and stage channels** support office hours and meetups without external tooling.
- **Bots and webhooks** ecosystem is mature (welcome bots, GitHub integration, moderation bots, etc.).
- **Persistent membership.** Members stay in the server across sessions, unlike Slack's per-workspace flow.
- **Cultural fit.** Younger developers default to Discord for community spaces.

### Used by

Most modern developer-product communities operate on Discord:

- Vercel / Next.js, Supabase, Neon, PlanetScale.
- The Rust language community.
- Most AI startups (LangChain, Hugging Face, OpenAI dev community, Anthropic, Pinecone, Modal).
- Most modern frontend frameworks (Astro, Svelte, Solid, Qwik).
- Cloudflare, DigitalOcean.
- Most indie developer products.

### Weaknesses

- **Search is poor.** Real-time only; old conversations are hard to find.
- **Content is not indexed by Google.** No SEO value.
- **Chaotic for newcomers.** Multiple channels, fast-moving conversation, lots of context.
- **Moderation at scale is hard.** Discord's tools are improving but lag what mature forum software provides.

### How to run a Discord well

- **Welcome flow.** Pin a clear welcome with rules, useful channels, and how to ask for help.
- **Channel structure.** Fewer channels than you think; consolidate categories. Use threads for topic-specific conversations.
- **Office hours and stage channels.** Schedule predictable events.
- **Staffing.** Have visible team-member presence at predictable hours.
- **Recognition.** Reward useful community members (roles, swag, recognition in stage events).
- **Moderation.** Clear and consistently applied rules. Document reasons for actions publicly.

---

## Slack

### History

- **Founded.** 2009 (as Tiny Speck / Glitch). Pivoted to Slack in 2013. Launched publicly 2014. Acquired by Salesforce 2020.
- **Scale.** 32M+ daily active users; enterprise dominant.

### Why it remains for some communities

- **Enterprise legitimacy.** Slack is what large enterprises already use internally; reduces friction for enterprise customer communities.
- **2,600+ integrations.** Mature ecosystem.
- **Threading.** Better than Discord's threads.
- **Workflows.** Slack's built-in workflow builder and automation are stronger than Discord's.

### The 2022 message-limit change

In 2022, Slack changed its free-tier policy to limit message history to 90 days. Previously, free-tier communities could access their full history. Many community Slacks had to either move to paid tier (linear cost with member count) or migrate to other platforms.

This single policy change moved a substantial number of communities to Discord.

### Used by

- **Enterprise-facing developer communities** (Snowflake's community, Confluent's community, many enterprise infrastructure products).
- **The DevRel Collective** itself (the professional Slack community of DevRel practitioners).
- **Kubernetes community Slack** (still one of the largest technical Slacks in operation).
- **Many CNCF projects.**
- **Some long-established communities** that predate Discord's rise.

### Weaknesses for community use

- **Cost scales with members.** A 10,000-person community on a paid tier is expensive.
- **Per-workspace silo.** Users need to switch workspaces to access different communities.
- **Less culturally aligned with grassroots developer communities** post-2020.

### When to choose Slack over Discord

- Your customers are mostly enterprise organisations whose employees already use Slack.
- You can absorb the linear per-user cost.
- Your community values threading discipline over real-time chaos.
- You have an existing Slack community with valuable history.

---

## Discord vs Slack: quick decision

| Question | Discord | Slack |
|---|---|---|
| Free unlimited users? | Yes | Limited (history capped) |
| Mature threading? | Improving | Yes |
| Voice/video built in? | Yes | Yes (huddles) |
| Mobile experience? | Excellent | Good |
| Searchable archive? | No | Limited on free |
| Bots/integrations? | Many | Many more |
| Enterprise customer fit? | Less so | Yes |
| Indie / grassroots fit? | Yes | Less so |

For most modern developer-product companies in 2024–2026, **the default is Discord**.

## Bridging and multi-platform community work

Some communities operate on both Discord and Slack with bidirectional bridges (using bots that mirror messages). This is fragile and often produces a confusing user experience; most teams settle on one as primary.

A more common multi-platform approach: Discord for real-time, GitHub Discussions or Discourse for searchable long-form Q&A. See [`../08-tools/community-platforms.md`](../08-tools/community-platforms.md).

## See also

- [`../08-tools/community-platforms.md`](../08-tools/community-platforms.md)
- [`../10-tactics/community-building.md`](../10-tactics/community-building.md)
- [`./github-as-platform.md`](github-as-platform.md)