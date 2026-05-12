# The Orbit Model

The **Orbit Model** is a framework for understanding and measuring community engagement, originally developed by Josh Dzielak, Patrick Woods, and the team at orbit.love. It is the most influential community-management framework in DevRel and is open-source at github.com/orbit-love/orbit-model.

## Core idea

Communities are not funnels. People don't all want to be converted to the same end state. A reading-only Twitter follower is doing something valuable; a heroic open-source contributor is doing something valuable; both deserve a model.

The Orbit Model represents communities as **gravitational systems**. Members orbit at different distances from the centre. The centre is the company or project; the distance is determined by two dimensions:

- **Love** — how engaged and committed a member is. Frequency, depth, and recency of contribution.
- **Reach** — how far that member's actions propagate beyond the community itself. Their network and audience.

The key equation:

```
Gravity = Love × Reach
```

Members with high love but low reach contribute deeply but quietly. Members with high reach but low love can amplify a message but may not stick around. Members with both — high-love, high-reach Advocates — are the rarest and most leveraged participants in a community.

## The four orbits

Most implementations of the Orbit Model use four orbit levels, from closest to farthest from the centre:

| Orbit | Description | Typical share | Example behaviours |
|---|---|---|---|
| **Advocates** | High love and meaningful reach. They actively help grow and shape the community. | 1–2% | Speak at conferences, write blog posts/videos, organise events. |
| **Contributors** | High love. They actively contribute work — code, docs, answers, translations. | ~5–10% | Submit PRs, review PRs, write tutorials, answer questions, file high-quality issues. |
| **Participants** | Engaged. They use the product, attend events, hang out in the community. | ~20–30% | Regular community posters, event attendees, active product users. |
| **Explorers** | Newcomers and lurkers. They consume content and may join channels. | Bulk of the audience | Newsletter subscribers, social followers, occasional event attendees. |

These percentages are illustrative; the actual distribution varies by community and stage. What matters is the **shape of the distribution** and how members move between orbits over time.

## Operationalising Love and Reach

The Orbit Model is intentionally framework-not-formula: each community defines its own scoring, but with shared structure.

**Love scoring example.** Assign points for activities, decay them over time:

| Activity | Points | Decay window |
|---|---|---|
| Conference talk about our product | 100 | 12 months |
| Substantial blog post or video | 50 | 9 months |
| Merged code PR | 40 | 12 months |
| Workshop attendance | 10 | 6 months |
| Helpful forum answer | 5 | 3 months |
| Discord message | 1 | 30 days |

Recent activity counts more than old activity. A long-time community member who has not engaged in a year drifts outward.

**Reach scoring example.** Reach is a property of the person, not the activity:

- Twitter/X / Bluesky follower count.
- GitHub follower count.
- YouTube subscribers, podcast audience.
- Conference speaker history.
- Position at a notable company (proxy for institutional reach).

Reach changes more slowly than love and is the harder of the two to measure cleanly.

## Movement between orbits

A healthy community has people moving inward over time:

```
Explorer → Participant → Contributor → Advocate
```

The orbit model gives you the language to ask: "What is our Explorer → Participant conversion rate this quarter? What is our Participant → Contributor rate? Where do members stall? Where do they leak?"

Different programs serve different transitions:

- **Newsletter / social content / docs** → moves Explorers to Participants.
- **Discord / Slack / Discourse and active moderation** → moves Participants to Contributors.
- **Ambassador / Champion / MVP programs** → moves Contributors to Advocates.
- **Re-engagement campaigns and recognition** → prevents Advocates and Contributors from drifting outward.

## Why this beats traditional funnels for community work

The traditional marketing funnel assumes a single end state (purchase) and treats anyone who hasn't converted as "in progress." That mental model breaks badly for developer communities because:

- An open-source maintainer is not a "prospect."
- A high-reach Advocate may never personally convert to a paying customer, yet drive enormous downstream value.
- A Participant who never moves inward is still creating value through their presence in the community.

The Orbit Model represents the value of every orbit explicitly. It does not assume that closer is always better; it assumes that **knowing where each member is** is what matters.

## Reciprocity is non-negotiable

The model's strongest single principle: **every interaction with a community member should create value for that member**. Otherwise their love drops, they move outward, and over time their reach moves with them. Communities that extract value without giving it back hollow themselves out — the most common DevRel anti-pattern visible from outside.

Practical implications:

- Ambassador-program "rewards" should not just be company swag; they should include access, status, education, network.
- Conference speaker placements should serve the speaker's career, not just the company's lead-gen.
- Community moderators should be paid, equipped, recognised, and protected.

## The Orbit Model and other frameworks

- **AAARRRP.** Orbit measures the *who*; AAARRRP measures the *why*. An ambassador program (Orbit transition: Contributor → Advocate) serves Referral and Product goals (AAARRRP). They compose.
- **Four Pillars.** Orbit is one of the structures inside the Programs pillar; the model also shapes how Community Management does its work.
- **NPS.** Orbit's "love" overlaps with sentiment captured by NPS but is more granular and behaviourally grounded.

## Tooling

Community-CRM tools implementing the Orbit Model or its principles:

- **Orbit.love** (the original product; acquired and re-architected over time).
- **Common Room** — competitor focused on enterprise integration.
- **crowd.dev / LFX Community Data Platform** — open-source, acquired by Linux Foundation in 2024 and integrated into LFX Experiences.
- **Savio**, **Apollo (GTM)**, and others address adjacent slices.

See [`../08-tools/community-crm-platforms.md`](../08-tools/community-crm-platforms.md).

## Common misuses

- **Treating Orbit levels as a leaderboard.** Don't. Members aren't competing for proximity; they're choosing their own depth of involvement.
- **Gaming the metric.** If your point system rewards Discord messages, you will get more Discord messages — and worse signal. Choose scoring that rewards behaviours you genuinely want more of.
- **Confusing reach with influence.** A high follower count on a moribund platform is not reach.
- **Failing to decay.** Without recency decay, your "advocates" list calcifies into people who matter in 2019 rather than 2026.

## Primary sources

- Orbit Model open-source repository: github.com/orbit-love/orbit-model.
- Patrick Woods and Josh Dzielak, "Introducing the Orbit Model," orbit.love, 2019.
- "How to Measure Developer Love and Reach," DevRelCon talks (various years).

## See also

- [`./aaarrrp.md`](aaarrrp.md)
- [`./four-pillars.md`](four-pillars.md)
- [`../04-metrics/community-metrics.md`](../04-metrics/community-metrics.md)
- [`../10-tactics/community-building.md`](../10-tactics/community-building.md)
- [`../08-tools/community-crm-platforms.md`](../08-tools/community-crm-platforms.md)