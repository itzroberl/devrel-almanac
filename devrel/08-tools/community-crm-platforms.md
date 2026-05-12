# Community CRM Platforms

Community-CRM platforms exist to solve one specific problem: developers and community members interact with companies across dozens of fragmented channels — GitHub, Discord, Slack, Stack Overflow, blog comments, conference attendance, X / Bluesky, dev.to, Reddit, Discourse, Postman, internal feedback forms — and no traditional CRM (Salesforce, HubSpot) is built to reason about those signals as a coherent picture.

The category took shape from roughly 2019 onward, matured through 2022–2024, and consolidated meaningfully in 2024–2026.

---

## Orbit (orbit.love)

The category-defining product.

- **Founded.** 2019 by Josh Dzielak (CTO; previously DevRel at Algolia, Keen.io) and Patrick Woods (CEO; previously Y Combinator).
- **Premise.** Operationalise community measurement using the **Orbit Model** — Love × Reach gravity model.
- **Integrations.** GitHub, Discord, Slack, Discourse, Twitter, Salesforce, HubSpot, dev.to, Notion, Product Hunt, Stack Overflow, and dozens more.
- **2023 transition.** Orbit announced the wind-down of the original SaaS product in 2023. The open-source Orbit Model itself remains active and influential, available at github.com/orbit-love/orbit-model. The model has been implemented in alternate tools and adapted by Common Room and others.
- **Significance.** Even though the original SaaS product wound down, the framework Orbit popularised is now industry-standard. See [`../03-frameworks/orbit-model.md`](../03-frameworks/orbit-model.md).

---

## Common Room

The current category-leading commercial product.

- **Founded.** 2020 by Tom Lehman, Linc Gasking, and Francis Larkin.
- **Premise.** Unify customer / prospect / community signals into a single platform with sales-aligned workflows.
- **Audience evolution.** Originally positioned for community teams; pivoted/expanded in 2023–2024 toward "customer-led growth" platform addressing community-influenced sales, not just community management.
- **Integrations.** GitHub, Discord, Slack, Discourse, Stack Overflow, dev.to, Reddit, podcasts, YouTube, plus enterprise CRMs and warehouses.
- **Strengths.** Identity resolution across platforms; strong workflow tooling; pipeline attribution.
- **Recent positioning.** Heavily emphasises AI-assisted prospect-research and "signal-based selling" — using community engagement signals to surface sales opportunities to revenue teams.

---

## crowd.dev → LFX Community Data Platform

- **Founded.** crowd.dev launched 2021 as an open-source community-data platform.
- **Acquired.** By the Linux Foundation in 2024.
- **Renamed.** Community Data Platform; integrated into LFX (Linux Foundation Experiences).
- **Significance.** Provides foundation-grade community data infrastructure to Linux Foundation projects (CNCF, OpenJS, Hyperledger, etc.). Free for open-source projects. Identity-resolution and contribution-tracking capabilities.

---

## Savio

- **Focus.** Customer feedback aggregation rather than community engagement.
- **Premise.** Centralise feedback from customer success, sales, and support to inform product roadmap.
- **Integration with DevRel.** Not strictly a DevRel tool, but useful for DevRel teams whose pillar 1 work includes pushing developer-feedback signals back into product.

---

## DevStats (CNCF and broader)

- **Original.** CNCF DevStats tracks contribution activity across all CNCF projects via GitHub.
- **Available.** Open-source dashboards at devstats.cncf.io and devstats.k8s.io.
- **Significance.** Defines how the largest open-source ecosystem of cloud-native projects reasons about contributor health.
- **Successor / parallel.** CHAOSS (Community Health Analytics for Open Source Software) is a Linux Foundation project producing similar metrics.

---

## Specialised community tools

- **Sourcegraph Cody Discover (and adjacent code-search tools)** — Used by some DevRel teams to discover where their product is referenced in public code.
- **Apollo, Clay, Clearbit** — Sales-data enrichment tools sometimes adopted by DevRel for prospect/contributor research.
- **Lavender, Lemlist** — Outbound email tools; relevant when DevRel is asked to do outbound (a controversial use of the function).

---

## Enterprise CRMs with growing community awareness

- **Salesforce.** Community Cloud (now Experience Cloud) for hosted community forums; salesforce Slack ecosystem.
- **HubSpot.** Connected community features rolling out 2024+.
- **Notion, Linear, Productboard.** Used by many DevRel teams to manage internal workflows around community-derived feedback.

---

## How to choose

A short decision tree:

| If you want to… | Consider |
|---|---|
| Measure community using the Orbit Model from scratch | Open-source Orbit Model + custom dashboard, or Common Room |
| Connect community signals to sales pipeline | Common Room |
| Run a Linux Foundation / open-source project | LFX Community Data Platform |
| Aggregate product feedback from internal teams | Savio |
| Build your own thing on raw data | Pull GitHub/Discord/Slack APIs into your warehouse + dbt + a BI tool |

The most sophisticated DevRel teams (Twilio, Stripe, GitHub, MongoDB, HashiCorp) generally build their own data pipelines into warehouses (Snowflake, BigQuery) and layer BI tools on top, rather than relying solely on a commercial platform.

## What community-CRM tools cannot do

- They cannot turn an absent community strategy into a present one.
- They cannot create love and reach where none exists.
- They cannot replace the relationships that DevRel professionals build by being personally present in community channels.

A tool is leverage on top of strategy. Without strategy, the tool produces dashboards that no one looks at.

## See also

- [`../03-frameworks/orbit-model.md`](../03-frameworks/orbit-model.md)
- [`../04-metrics/community-metrics.md`](../04-metrics/community-metrics.md)
- [`./community-platforms.md`](community-platforms.md)