# Community Platforms

The infrastructure where developer communities actually live. Choosing between these platforms is one of the highest-stakes DevRel decisions: the wrong choice limits community potential for years.

---

## Discord

- **Founded.** 2015 by Jason Citron.
- **Origin.** Gamer chat platform; pivoted aggressively toward broader community use 2020 onward.
- **Scale.** 200M+ monthly active users; primary community platform for many modern developer products.
- **Strengths.** Real-time chat; voice/video stage channels; threads; rich presence; free for community use; strong mobile experience; native bots and webhooks.
- **Weaknesses.** Poor search (real-time only, hard to find old conversations); poor SEO (content not indexed); single-tenant per server; can feel chaotic for newcomers.
- **Used by.** Vercel/Next.js, Supabase, Cloudflare, Neon, the Rust community, most AI startups (LangChain, OpenAI's developer community, Hugging Face, Anthropic), most modern frontend frameworks (Astro, Svelte), most modern indie developer products.
- **Strategic placement.** Best for real-time conversation, AMAs, office hours, peer-to-peer help where speed and presence matter more than archive value.

---

## Slack

- **Founded.** 2009 (as Tiny Speck / Glitch); pivoted to Slack 2013. Acquired by Salesforce 2020.
- **Scale.** 32M+ daily active users; enterprise dominant.
- **Strengths.** Enterprise-grade; 2,600+ integrations; strong threading; mature workflow tools; reliable for distributed work.
- **Weaknesses.** Free-tier message limit (90 days of history) was introduced in 2022 — disqualified Slack for many community uses overnight. Cost scales linearly with users.
- **Used by.** Many older / enterprise-leaning developer communities (Kubernetes Slack, many CNCF projects, many enterprise infrastructure communities, the DevRel Collective itself). Some communities maintained Slack throughout but most newer developer-product communities chose Discord post-2020.
- **Strategic placement.** Best for enterprise customer communities, internal DevRel ops, smaller invite-only programs.

---

## Discourse

- **Founded.** 2013 by Jeff Atwood (co-founder of Stack Overflow), Sam Saffron, and Robin Ward.
- **Open source.** Yes; self-hostable. Also offered as managed SaaS.
- **Strengths.** Threaded forum structure with excellent search; SEO-friendly (community content gets indexed and drives organic discovery); badges and gamification; trust levels; substantial moderation tooling.
- **Weaknesses.** Async-first format; lacks real-time presence; perception bias toward "old internet" for younger developers.
- **Used by.** Rust users forum, Hashnode, Postman community, many language and project communities (Elixir, Julia, Pharo, etc.), Discourse's own meta forum.
- **Strategic placement.** Best when long-tail searchable Q&A is critical; complements Discord/Slack rather than replacing it.

---

## Circle (circle.so)

- **Founded.** 2020 by Sid Yadav (formerly Teachable).
- **Positioning.** Modern, design-led community platform; branded site, discussions, courses, events, payments, AI agents, native email.
- **Used by.** Many course-creator communities; growing presence in technical communities.
- **Pricing.** Mid-range SaaS.

---

## Mighty Networks

- **Founded.** 2017 by Gina Bianchini (formerly co-founder of Ning).
- **Positioning.** Community + courses + events + native commerce; emphasis on member-led activity.
- **Reported scale.** $500M+ earned through the platform in 2025; ~$48/mo average membership pricing.
- **Used by.** Less common for developer products specifically; more common for creator economy.

---

## Tribe (now Bettermode)

- **Founded.** 2019.
- **Renamed.** Bettermode.
- **Positioning.** Customisable branded community platform; over 10,000 communities reported.
- **Strengths.** Strong customisation; embeddable widgets; API integration.

---

## Khoros, Higher Logic, Vanilla Forums

- **Khoros.** Enterprise community-software vendor; large traditional B2B install base.
- **Higher Logic.** Enterprise community software; common for associations and large enterprise communities.
- **Vanilla Forums.** Mature forum platform.

These platforms are mature but rarely chosen by modern developer-product companies for grassroots developer community; they appear most often in customer-success / enterprise contexts.

---

## Reddit-style platforms

- **Reddit itself.** Some companies maintain subreddits (r/cloudflare, r/MongoDB, r/postgresql). Generally hosted, not company-controlled.
- **Lemmy.** Federated open-source Reddit alternative; small but growing developer-adjacent communities.

---

## Stack Overflow (and Stack Exchange)

- **Founded.** 2008.
- **Status in 2026.** Substantial decline. Question volume dropped roughly 95% from 2014 peak by late 2025. Many developers no longer post questions there; most still consult its archives. See [`../09-platforms/stack-overflow.md`](../09-platforms/stack-overflow.md).
- **Strategic placement.** Less effective as primary community space; still valuable as a knowledge archive.

---

## GitHub Discussions

- **Launched.** 2020 by GitHub.
- **Strengths.** Lives where the code lives; no separate signup; integrates with issues and code.
- **Weaknesses.** Less polished community UX; limited moderation tooling; limited to GitHub users.
- **Used by.** Most large open-source projects (Next.js, Astro, Supabase, many AI projects).

---

## Less common but interesting

- **Element / Matrix.** Federated; used by some open-source projects (especially those with privacy / federation values).
- **IRC and IRCv3.** Survived among hardcore communities (FreeBSD, NetBSD, certain Linux projects).
- **Zulip.** Slack alternative with threading at the channel level; used by Rust language community development, Recurse Center.
- **Mattermost.** Open-source Slack alternative; used by some self-hosting communities.
- **Rocket.Chat.** Similar.

---

## Multi-platform reality

Most large DevRel programs operate on multiple platforms simultaneously:

- **Discord or Slack** for real-time community.
- **Discourse or GitHub Discussions** for long-form Q&A.
- **GitHub** for code / contributions.
- **Stack Overflow** as a knowledge archive (less actively, in 2026).
- **Reddit** if there is an active subreddit.

The challenge is **identity resolution and engagement measurement across platforms**, which is exactly what community-CRM tools (Common Room, LFX Community Data Platform) try to solve. See [`./community-crm-platforms.md`](community-crm-platforms.md).

## Choosing

A practical decision tree:

| If your community is… | Choose primary platform |
|---|---|
| Modern, real-time, indie / startup product | Discord |
| Enterprise / sensitive to corporate policies | Slack |
| Q&A-heavy with valuable archived knowledge | Discourse |
| Open-source project, GitHub-native | GitHub Discussions |
| Creator-economy / course-led | Circle or Mighty Networks |
| Federation-and-privacy-aligned | Matrix / Zulip |

For most modern developer-product companies in 2024–2026, the default is **Discord for real-time + GitHub Discussions or Discourse for searchable Q&A**.

## See also

- [`./community-crm-platforms.md`](community-crm-platforms.md)
- [`../09-platforms/discord-slack.md`](../09-platforms/discord-slack.md)
- [`../10-tactics/community-building.md`](../10-tactics/community-building.md)