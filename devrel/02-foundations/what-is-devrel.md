# What Is Developer Relations?

**Developer Relations (DevRel)** is the organizational discipline of building and sustaining trusted relationships between a company and the software developers who use, evaluate, or influence the adoption of its products. It encompasses advocacy, education, community building, developer experience, and developer marketing, with the dual goals of (a) helping developers succeed and (b) producing measurable business outcomes — adoption, retention, revenue influence, product feedback, and brand trust.

DevRel is **not** marketing in a hoodie. It is not a sales role. It is not a glorified speaker bureau. It is an applied discipline that exists at the intersection of engineering, product, marketing, and community management, and is most effective when it has structural autonomy from any single one of those functions.

## The two-question test

Phil Leggetter's classic framing: every DevRel team can be evaluated by how confidently it can answer two questions:

1. **How much do our developers like us?**
2. **How many people are they telling about us?**

Strong DevRel programs collect signals continuously to answer both. Weak programs default to vanity metrics (followers, stars, event attendance) that gesture at the answer without ever providing it.

## The bridge metaphor

DevRel operates as a **bidirectional bridge** between the company and the external developer community:

```
External developers  ⇄  Developer Relations  ⇄  Internal teams
                                              (product, engineering,
                                               marketing, sales)
```

Outbound:

- Explains what the product does, why it matters, and how to use it.
- Translates technical capability into accessible understanding.
- Models the kind of developer the company wants to attract.
- Distributes expertise across content, code, talks, and 1:1 conversation.

Inbound:

- Carries developer pain, confusion, joy, and feature requests back to product and engineering.
- Identifies friction in onboarding, docs, APIs, and pricing before it shows up in churn.
- Validates messaging against real audiences before marketing ships it.
- Surfaces high-leverage community members who can later become customers, partners, advocates, or hires.

When DevRel runs primarily in one direction, it degrades into either evangelism-as-marketing (all outbound) or developer support (all inbound). Both are functional, neither is the full discipline.

## The umbrella

In common usage, "DevRel" is an umbrella term covering several adjacent disciplines that often share staff and reporting structure:

- **Developer Advocacy** — Public-facing technical practitioners who teach, demo, and represent developer interests internally.
- **Developer Evangelism** — A more outbound-oriented variant emphasizing awareness and adoption, historically associated with sales-adjacent goals. (See [`./disciplines.md`](disciplines.md) for the advocate vs. evangelist distinction.)
- **Developer Experience (DevEx / DX)** — The end-to-end experience a developer has with a product. Often partly owned by DevRel, partly by product/engineering, sometimes by a dedicated DX team.
- **Developer Education** — Documentation, tutorials, courses, videos, sample apps, certification.
- **Developer Marketing** — Marketing whose audience is developers; respects technical norms and avoids consumer-marketing tropes.
- **Developer Success / Enablement** — Helping developers move from "tried it" to "shipped it in production." Closely related to customer success but with technical depth.
- **Community Management** — Operating the spaces (Discord, forum, Slack, in-person) where developers connect.
- **Developer Programs** — Structured initiatives (ambassador, champion, MVP, student, certified-expert) that recognise and equip top community members.

Different organisations carve the umbrella differently. See [`../03-frameworks/four-pillars.md`](../03-frameworks/four-pillars.md).

## Audience characteristics that make DevRel distinct

Developers are not "consumers who write code." Several characteristics make them a distinct audience and demand a distinct discipline:

1. **They detect insincerity at distance.** Marketing claims unsupported by working code, accurate docs, or honest engineering answers get punished publicly.
2. **They trust peers far more than companies.** Recommendations from a respected engineer in their network beat any advertising spend.
3. **They make adoption decisions through use, not through brochures.** A free tier, a working tutorial, and a clean SDK do more than a landing page.
4. **They are simultaneously evaluator, end user, and procurement influencer.** They often choose tools their employer buys, so "developer-led" and "B2B" overlap.
5. **They are unusually generous as content creators when treated well**, and unusually loud as critics when not.

These traits are why DevRel works and why marketing-only approaches consistently fail against developer audiences.

## What DevRel is *not*

- **Not a synonym for technical marketing.** Technical marketing is a sibling function that produces case studies, technical content, and sales enablement aimed at decision-makers.
- **Not a free conference-speaking gig.** Speaking is a tactic, not the job.
- **Not customer support.** Though DevRel often runs first-line triage in community spaces, scaled support is a separate function with different incentives.
- **Not "the thing you do when you can't justify a sales team."** Mature DevRel coexists with sales and influences pipeline; it does not replace it.
- **Not a function that exists for every company.** Companies whose products are not developer-led probably do not need a DevRel team. The 2022–2024 layoff wave was partly a correction of premature investment in DevRel by companies whose products did not require it.

## When does a company need DevRel?

A useful heuristic: a company needs DevRel when **developers are decision-makers, integrators, or amplifiers** for its product. That includes:

- API-first products (Stripe, Twilio, Postman, Auth0, Algolia).
- Infrastructure and developer tools (HashiCorp, GitHub, Vercel, Datadog).
- Cloud platforms (AWS, GCP, Azure, Cloudflare, DigitalOcean).
- Databases and data infrastructure (MongoDB, Redis, Snowflake, Databricks, Neon, Supabase).
- AI model/tool providers (OpenAI, Anthropic, Hugging Face, Cohere, LangChain, NVIDIA).
- Open-source-led commercial products (Elastic, MongoDB, GitLab, Confluent).

Companies whose buyer is solely the CIO and whose product is a managed service that developers never touch directly typically do not benefit from a dedicated DevRel function and would be better served by technical marketing and customer engineering.

## Further reading inside this almanac

- [`./disciplines.md`](disciplines.md) — Detailed breakdown of advocacy, evangelism, education, marketing, success, and community management.
- [`./job-titles-and-roles.md`](job-titles-and-roles.md) — Title taxonomy.
- [`./org-structures.md`](org-structures.md) — Where DevRel reports and how teams are sized.
- [`../03-frameworks/aaarrrp.md`](../03-frameworks/aaarrrp.md) — Strategy framework.
- [`../11-trends/plg-and-devrel.md`](../11-trends/plg-and-devrel.md) — Why product-led growth makes DevRel structurally necessary.

## Primary sources

- Mary Thengvall, *The Business Value of Developer Relations* (Apress, 2018).
- Caroline Lewko & James Parton, *Developer Relations: How to Build and Grow a Successful Developer Program* (Apress, 2021).
- Phil Leggetter, "AAARRRP — Developer Relations Strategy Framework," 2016.
- Jono Bacon, *People Powered* (HarperCollins, 2019) and *The Art of Community* (O'Reilly, 2012).
- SlashData, *State of the Developer Nation* and *State of Developer Relations* reports.