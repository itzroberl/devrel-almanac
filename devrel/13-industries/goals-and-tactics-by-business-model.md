# Goals and Tactics by Business Model

DevRel looks different depending on how the company makes money. This file maps how the function adapts across the major business-model archetypes.

---

## Pure product-led growth (PLG)

**Examples.** Stripe, Twilio, Postman, MongoDB Atlas, Supabase, Neon, Vercel.

**Revenue model.** Self-serve trial → free tier → paid usage → expansion. No (or minimal) sales required.

**Primary DevRel goals.** Activation, retention, referral.

**Top tactics.**

- Aggressive investment in quickstart, docs, and SDK quality.
- Sample apps and templates for top use cases.
- Active community with fast first-response times.
- Education programs (certifications, courses, workshops).
- Coordinated launches with content + community + social distribution.

**What to deprioritise.** Enterprise-style direct sales support; one-off conference sponsorships without follow-up.

**Risk.** Treating DevRel as "brand marketing." It isn't — it's the activation funnel.

---

## PLG with enterprise expansion (PLG + sales hybrid)

**Examples.** GitHub, HashiCorp, Snowflake, Databricks, Datadog, Sentry.

**Revenue model.** Self-serve trial drives team-level adoption; enterprise sales close large contracts based on that adoption.

**Primary DevRel goals.** Activation, retention, referral, *plus* product feedback and influence on enterprise architects.

**Top tactics.**

- Everything from pure PLG, plus:
- Architecture content for senior engineering leaders.
- Speaker placement at enterprise-relevant conferences.
- Customer-success-style depth with the largest customers' developer teams.
- Reference customer co-marketing.
- Champion programs that bring senior engineers into ambassador-style roles.

**Risk.** Sales team and DevRel pulling in different directions about what content to produce.

---

## Sales-led enterprise

**Examples.** Some Microsoft / IBM / Oracle / Salesforce / SAP product lines, large enterprise infrastructure.

**Revenue model.** Multi-month sales cycles with multiple stakeholders; developers are influencers but not buyers.

**Primary DevRel goals.** Awareness with senior architects; pipeline support; certification (which adds to enterprise customer ROI on the product); customer expansion.

**Top tactics.**

- Conference sponsorship at flagship industry events.
- Customer advisory boards.
- Architecture white papers.
- Certification programs as revenue and credibility.
- Roadshow / regional executive briefings.
- Reference customer programs.

**What to deprioritise.** Hardcore quickstart obsession (the activation funnel doesn't run there).

**Risk.** DevRel becoming pre-sales technical marketing in disguise.

---

## Open-source-led (commercial open source)

**Examples.** Confluent (Kafka), Elastic, MongoDB, GitLab, HashiCorp pre-acquisition, Grafana Labs, Vercel/Next.js, Supabase, Neon.

**Revenue model.** Open-source project drives adoption; commercial product adds enterprise features (hosting, support, security, compliance).

**Primary DevRel goals.** Open-source community health, contribution velocity, brand mindshare, conversion from open-source user to commercial customer.

**Top tactics.**

- Visible commitment to open-source governance.
- Maintainer recognition (sometimes employment).
- Community contributor programs.
- Conference speaker placement.
- Documentation as primary commercial-product-and-OSS-product surface.
- Transparency in product roadmap.

**Risk.** Friction between OSS community and commercial product. "Open source rugpull" perception is corrosive.

---

## Marketplace / platform

**Examples.** Shopify, Salesforce, Atlassian Marketplace, Slack apps, WordPress ecosystem, Apple App Store, Google Play, Stripe Apps.

**Revenue model.** Take rate on third-party developer products. Developers building on the platform are the customer.

**Primary DevRel goals.** Onboarding third-party developers; growing the partner ecosystem; partner success.

**Top tactics.**

- Partner programs with tiers and benefits.
- Partner conferences and certification.
- SDK and platform-API quality.
- Marketing for top partners (co-branded customer stories, featured-app placement).
- Developer financial incentives (Apple's 15% small-business tier, Shopify's Plus programs, etc.).

**Risk.** Squeezing partners through take-rate or competitive-product moves.

---

## Hardware-led (with software ecosystem)

**Examples.** NVIDIA, Apple silicon, Arduino, Raspberry Pi, ARM ecosystem.

**Revenue model.** Hardware sales, sometimes with software-services revenue layered on top.

**Primary DevRel goals.** Build the software ecosystem that drives hardware purchases.

**Top tactics.**

- Long-running developer programs (NVIDIA's, Apple's).
- Educational programs (university curricula, certifications).
- Hardware kit programs for developers.
- Conference investment (GTC, WWDC).
- Open-source toolchain support.

**Risk.** Hardware-software disconnects produce frustrating developer experience.

---

## Two-sided / network-effect

**Examples.** Plaid (banks + fintech apps), Twilio (carriers + senders), Marketplace platforms.

**Revenue model.** Network effects between two sides require both to grow.

**Primary DevRel goals.** Vary by side; usually focused on whichever side is currently the bottleneck.

**Top tactics.**

- Side-specific developer programs.
- Cross-side success stories.
- Joint developer events.

**Risk.** Focusing too much on one side and losing the other.

---

## Embedded / SDK-licensed

**Examples.** Stripe Issuing, Twilio SDKs in third-party products, mapping providers (Mapbox, HERE), payment SDKs.

**Revenue model.** Licensing fees or per-transaction pricing for embedding in customer products.

**Primary DevRel goals.** Architect mindshare; integration enablement.

**Top tactics.**

- Architecture content for build-vs-buy decisions.
- Reference integration guides.
- Customer integration teams (DevRel-adjacent).
- Co-marketing with customer products.

**Risk.** Embedded relationships are hard to make visible; harder to evangelise.

---

## Freemium / consumer-developer hybrid

**Examples.** GitHub (free tier for individuals + paid tiers), Replit, CodePen, JetBrains (individual licenses), Notion, Figma.

**Revenue model.** Free tier drives consumer/individual usage; paid tiers drive revenue.

**Primary DevRel goals.** Awareness, individual-developer adoption, conversion to paid (sometimes via team usage).

**Top tactics.**

- Free-tier generosity.
- Education content.
- Student programs.
- Conference / event presence.
- Influencer-developer relationships.

**Risk.** Free-tier abuse without conversion mechanisms.

---

## Internal platform engineering

A different model: not selling to external developers, but building for internal ones.

**Examples.** Most large companies' internal platform-engineering organisations (Spotify Backstage, Netflix's Spinnaker, etc.).

**Revenue model.** Productivity savings, not direct revenue.

**Primary DevRel goals.** Internal adoption, satisfaction, productivity.

**Top tactics.**

- Internal documentation.
- Internal "shipping team" advocacy.
- Internal metrics (SPACE, DORA, DXI).
- Internal community building (internal Slack, internal newsletters).

**Risk.** Treated as not-real-DevRel by external community.

---

## How to read this file

Match your company's primary business model to one of the archetypes above. The goals and tactics shift meaningfully across them.

The most common DevRel strategic mistake is **applying tactics from one model to a company operating a different one**. Open-source-style community-led growth tactics applied to a sales-led enterprise will underperform. Conversely, enterprise-style ABM tactics applied to a PLG product will be ignored by developers.

The right tactics are determined by the business model first, the audience second, and personal preference last.

## See also

- [`./industries-served.md`](industries-served.md)
- [`../11-trends/plg-and-devrel.md`](../11-trends/plg-and-devrel.md)
- [`../03-frameworks/aaarrrp.md`](../03-frameworks/aaarrrp.md)
- [`../02-foundations/org-structures.md`](../02-foundations/org-structures.md)