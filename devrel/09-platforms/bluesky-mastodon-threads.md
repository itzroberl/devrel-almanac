# Bluesky, Mastodon, and Threads

The post-Twitter alternatives. None has fully replaced what "dev Twitter" was, but together they host substantial portions of the developer community in 2024–2026.

## Bluesky

- **Launched.** Public beta 2023; opened publicly 2024.
- **Architecture.** Built on the AT Protocol (Authenticated Transfer Protocol) — federated, with portable identity and customisable algorithmic feeds.
- **Origin.** Started as a Twitter-internal project under Jack Dorsey; spun out as an independent organisation; now operates separately.
- **Scale.** Roughly 30+ million registered users by mid-2026; daily active users peaked around 5M in January 2025 and has been more variable since.
- **Strengths for developers.**
    - **Custom feeds.** Anyone can create and share a custom algorithmic feed. Several developer-specific feeds emerged organically.
    - **Open protocol.** Developers can build on AT Protocol; a small but growing third-party-app ecosystem.
    - **No ads (currently).** Chronological-or-curated feeds without algorithmic ad insertion.
    - **Domain-as-handle.** Many developers use their own domain as their handle (e.g., `@kelseyhightower.com`).
- **Notable migrations.** Many web developers, infrastructure folks, and the journalist-and-analyst crowd moved primarily to Bluesky 2023–2025.
- **Weaknesses.**
    - Some senior developers still operate primarily on X.
    - Discovery is harder than X for large public conversation.
    - Smaller absolute audience than X, dramatically smaller than YouTube.

## Mastodon

- **Architecture.** Decentralised, federated (ActivityPub protocol). Users join an instance (server), which federates with others.
- **Notable tech instances.**
    - **fosstodon.org** — Free and open-source-focused. Among the largest tech-leaning instances.
    - **hachyderm.io** — Tech-focused; founded 2022 specifically as a developer-friendly Mastodon instance.
    - **mas.to** — Generalist, large.
    - **mastodon.social** — Generalist, very large.
    - **infosec.exchange** — Security professionals.
    - **mastodon.online** — Generalist.
- **Migration pattern.** Mastodon saw earlier and more complete migration of *communities* (rather than individuals) than Bluesky did. The open-source, federation-friendly, ad-hostile crowd moved largely to Mastodon in late 2022.
- **Strengths.**
    - Ideological alignment with open-source values.
    - No company can shut it down.
    - Many of the most committed maintainers and open-source veterans operate primarily on Mastodon.
- **Weaknesses.**
    - Discovery and onboarding are harder than centralised platforms.
    - Different instances have different cultures and rules.
    - User base is more technically homogeneous, which is both strength and limitation.

## Threads (Meta)

- **Launched.** July 2023 by Meta as a Twitter alternative tied to Instagram identity.
- **Initial trajectory.** 100M signups in first week; substantial drop-off; later recovery and growth.
- **Architecture.** Centralised; gradually integrating with the ActivityPub fediverse (Meta committed to interoperability with Mastodon).
- **Developer relevance in 2026.** Modest. The Threads community is mass-market and creator-economy oriented; developer-specific conversation is thinner than on Bluesky or Mastodon.

## How DevRel teams handle the fragmentation

Most DevRel professionals in 2026 operate a multi-platform presence:

- **Primary.** Their own newsletter / blog.
- **Secondary distribution.** LinkedIn, X, Bluesky.
- **Selective.** Mastodon (especially for open-source-focused product teams).
- **Conversational.** Threads (lighter touch, rarely primary).

A common operational pattern: write once, post natively on each platform with platform-appropriate framing. Tools like Buffer, Hypefury, and Typefully partially automate this, though native posting often outperforms cross-posted versions.

## What this means for DevRel strategy

The fragmentation has costs:

- No single platform reliably reaches "all the developers you want to reach."
- Building a single large audience on any one platform is harder than it was in 2018.
- Long-form content distribution (link-driven) is increasingly difficult algorithmically.

It also has benefits:

- More platforms means less concentration risk.
- Newsletter and own-platform investments compound.
- Specific communities (Bluesky for web dev, Mastodon for OSS, X for AI engineering, Threads for general tech-curious audience) can be served distinctly.

The most resilient DevRel content strategy in 2026 looks like:

1. Own your audience via a newsletter and a blog you control.
2. Cross-post to YouTube + the social platform(s) most relevant to your audience.
3. Treat any single social platform's algorithm as out-of-your-control infrastructure.

## See also

- [`./twitter-x.md`](twitter-x.md)
- [`./linkedin-for-developers.md`](linkedin-for-developers.md)
- [`../11-trends/future-directions.md`](../11-trends/future-directions.md)