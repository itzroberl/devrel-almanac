# The Four Pillars Framework

The **Four Pillars** model, articulated most prominently by Caroline Lewko and James Parton in *Developer Relations: How to Build and Grow a Successful Developer Program* (Apress, 2021), describes how a complete developer-relations program is composed of four distinct but interconnected functions sitting on a foundation of authentic advocacy. It is the most widely used *functional* model in the field — companion to AAARRRP (a *strategy* framework) and Orbit (a *community* framework).

## The structure

```
                ┌────────────────────────────────────────────┐
                │            DEVELOPER EXPERIENCE             │
                └────────────────────────────────────────────┘
                          ↑   ↑   ↑   ↑
                ┌─────────┴───┴───┴───┴──────────┐
                │   EDU.   MARKET.   SUCCESS    PROGRAMS │
                └─────────┬───┬───┬───┬──────────┘
                          ↑   ↑   ↑   ↑
                ┌────────────────────────────────────────────┐
                │      AUTHENTIC ADVOCACY (TRUST)             │
                └────────────────────────────────────────────┘
```

Below the pillars: **authentic advocacy** — credibility, trust, and the willingness to put developer interests on equal footing with company interests.

The four pillars themselves: **Developer Education, Developer Marketing, Developer Success, Developer Programs**.

Above the pillars: **Developer Experience** — the holistic outcome the four pillars produce.

## Pillar 1 — Developer Education

**What it covers.** Documentation, quickstarts, tutorials, reference, videos, courses, sample apps, certifications.

**Goal.** Help a developer move from "never heard of this" to "shipped to production" to "expert."

**Typical artefacts.**

- API reference docs (often OpenAPI-driven).
- Conceptual docs explaining the model.
- Getting-started guides and quickstarts (time-bound, success-defined).
- Long-form tutorials.
- Cookbooks and recipe collections.
- Video courses and screencasts.
- Workshop curricula (live and async).
- Sample applications, deployable in minutes.
- Certification programs.

**Common roles.** Technical writer, developer educator, curriculum developer, docs engineer, video producer.

**Key principle.** Match the format to the learning curve. A reference page answers a different question than a tutorial; a workshop solves a different problem than a video. Treating them as interchangeable wastes effort.

**Practical guidance.**

- Treat docs as a product, not an artefact. They deserve their own roadmap.
- Optimise the quickstart relentlessly. Reducing Time to First Hello World is one of the highest-leverage activities in DevRel.
- Build for both humans and AI. AI agents now read your docs to write code; structure them for machine parsing too. See [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md).
- Maintain ruthlessly. Stale tutorials are worse than no tutorials.

See [`../10-tactics/documentation-as-product.md`](../10-tactics/documentation-as-product.md).

## Pillar 2 — Developer Marketing

**What it covers.** Persona research, positioning and messaging, content marketing, events, social, community presence, distribution.

**Goal.** Reach developers where they are with content they value, in tone they respect.

**Key differences from traditional marketing.**

- Audience is technical; messaging must be substantively accurate.
- Channels favour developer-specific places (Hacker News, dev.to, Reddit, GitHub, niche newsletters, technical YouTube).
- Gated lead magnets and BANT-style qualification break trust.
- Long-form, technically deep content outperforms short, polished marketing pieces.
- Authority comes from individuals, not brands; named bylines and authentic voices outperform corporate channels.

**Common roles.** Developer marketing manager, product marketing manager (developer), developer growth manager, content strategist.

**Practical guidance.**

- Use peer-to-peer recommendation as a primary distribution channel. SparkLoop-style newsletter referrals, ambassador-amplified social, customer-story content.
- Invest in distribution as much as creation. A great post unread is the same as no post.
- Co-create content with customers. The most effective developer marketing is published *by* developers, not at them.
- Measure with developer-appropriate metrics (DQLs, qualified signups, activation), not consumer-marketing metrics (CTR, generic MQLs).

## Pillar 3 — Developer Success

**What it covers.** The function ensuring developers who try the product actually ship with it.

**Goal.** Move developers from "evaluated" to "in production at scale" without unnecessary friction.

**Typical work.**

- 1:1 onboarding for high-value accounts.
- Scaled enablement (office hours, async support, integration help).
- Identifying churn signals (sudden drop in activity, integration regressions).
- Coordinating with engineering on patterns that cause repeated friction.
- Building a knowledge base of successful integration patterns.

**Common roles.** Developer success engineer, developer solutions engineer, customer engineer (Google Cloud's term), technical account manager (for largest accounts).

**Key principle.** The product handoff from "first hello world" to "production at scale" is where many developer products lose customers silently. Developer success is the discipline that prevents this.

## Pillar 4 — Developer Programs

**What it covers.** Structured initiatives that recognise, equip, and amplify the company's most engaged community members.

**Goal.** Compound the company's reach and credibility by investing in the developers who already love the product.

**Typical programs.**

- **Recognition programs.** Microsoft MVP, AWS Heroes, GDE, MongoDB Champions, HashiCorp Ambassadors, Oracle ACE, IBM Champions, Snyk Ambassadors, Cloudflare Developer Experts.
- **Contributor programs.** Beta-tester groups, advisory boards, contributor onboarding for open-source projects.
- **Student programs.** GitHub Campus Experts, JetBrains Academy Ambassadors, Postman Student Program.
- **User groups.** Locally led communities supported with content, swag, and (occasionally) staff visits.
- **Certification programs.** Stripe Certified, AWS Certified, Postman API Specialist, etc.

**Common roles.** Community program manager, community manager, ambassador program lead.

**Key principle.** Programs are downstream of community foundations. Building an ambassador program before you have a healthy community produces a thin shell of "ambassadors" with no one to be an ambassador *to*. See [`../10-tactics/ambassador-programs.md`](../10-tactics/ambassador-programs.md).

## The foundation — Authentic Advocacy

The four pillars sit on a foundation of authentic advocacy: the credibility and trust that make developers willing to engage at all. This includes:

- Technical truth-telling, even when it costs the company a sale.
- Listening structures that visibly change product behaviour over time.
- Recognising community contributions without conditions.
- Honest discussion of limitations, deprecations, and breaking changes.
- Treating community moderators and ambassadors as people, not channels.

Without this foundation, everything above it leans toward marketing and away from advocacy, and the developer audience disengages.

## The ceiling — Developer Experience

The four pillars produce — together — the developer experience. DevEx is the *outcome* of the function; the four pillars are the *components* that produce it. A great quickstart (Education), a respected presence on technical platforms (Marketing), responsive integration help (Success), and a generous ambassador program (Programs) collectively make a great DevEx.

DevEx, in turn, is a primary input to product adoption, retention, and revenue.

## How to use the framework

Two practical applications:

1. **Audit your function.** Score your team's investment in each pillar from 1–5. Where are you weak? An over-investment in marketing with weak education and zero success is a common DevRel failure mode and one of the patterns that the 2022–2024 layoffs corrected.
2. **Hire to balance.** A new DevRel team rarely staffs all four pillars at once. Typically: education + community first (covering pillars 1, 4, and part of 3), then marketing (pillar 2), then a dedicated success function (pillar 3) as scale demands.

## Common misuses

- **Treating "pillars" as silos.** They overlap. A great workshop is education *and* marketing *and* success in one event.
- **Skipping the foundation.** A team that builds pillars without authentic advocacy is doing marketing in a hoodie.
- **Confusing pillars with reporting lines.** The four pillars are functions; how they are organised reports-wise depends on company context.

## Primary sources

- Caroline Lewko & James Parton, *Developer Relations: How to Build and Grow a Successful Developer Program* (Apress, 2021).
- Phil Leggetter / SlashData, *Developer Marketing & Relations: The Essential Guide* (multiple editions).
- Chris Reddington, "DevRel's Four Pillars and the Authentic Foundation" (chrisreddington.com).

## See also

- [`./aaarrrp.md`](aaarrrp.md)
- [`./orbit-model.md`](orbit-model.md)
- [`./maturity-model.md`](maturity-model.md)
- [`../02-foundations/disciplines.md`](../02-foundations/disciplines.md)