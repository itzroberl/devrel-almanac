# DevRel Metrics: Overview

The hardest single question in DevRel: how do you measure what you're doing in a way that connects to business outcomes? The 2022–2024 layoff wave exposed how many DevRel teams could not answer this question for their executives. This file gives the overview; subsequent files in this directory dive into specific metric families.

## Three layers of metrics

A useful mental model: every DevRel metric falls into one of three layers, and a healthy program tracks all three with explicit causal narratives between them.

### Layer 1: Program metrics (business outcomes)

What the company actually cares about. Examples:

- **New active developers acquired.**
- **Time to first hello world (system-wide median).**
- **Activation rate** (% of new signups who reach an activation milestone).
- **30-day / 90-day retention.**
- **Revenue influenced.**
- **Developer-qualified leads (DQLs).**
- **Product feedback items shipped.**

These are what you report to executives. They should map cleanly to AAARRRP goals.

### Layer 2: Community metrics (ecosystem health)

What's happening in the developer community around the product. Examples:

- **Active community members (DAU / WAU / MAU).**
- **Contributor return rate at 90 days.**
- **NPS / sentiment.**
- **First-response time in community.**
- **Member orbit-level distribution** (Explorers, Participants, Contributors, Advocates).
- **Geographic and demographic distribution** of the community.

These are leading indicators for Layer 1 outcomes. A weakening community in Q1 predicts weakening retention in Q2.

### Layer 3: Activity metrics (what the team does)

What the DevRel team itself produces. Examples:

- **Blog posts published.**
- **Conference talks delivered.**
- **Videos shipped.**
- **Newsletter subscribers and open rate.**
- **GitHub stars, social followers.**
- **Workshop attendance.**

These are easy to measure and easy to game. They matter only insofar as they drive Layer 2 and Layer 1 outcomes. **A team that reports only Layer 3 metrics is reporting motion, not progress.**

## The narrative connection

Mature DevRel reporting connects all three layers explicitly. A reportable insight looks like:

> *Tutorial content (Layer 3: 12 new tutorials published, 78% completion rate)* drove *measurable docs engagement (Layer 2: 23% increase in tutorial-page DAU)*, which contributed to *improved activation (Layer 1: 18% reduction in median TTFHW, 7-point activation-rate lift)*.

A team that can speak in those terms regularly is structurally protected from "cut DevRel" conversations.

## The "we don't measure" problem

State of Developer Relations surveys consistently show a non-trivial share of DevRel teams report they "don't measure" rigorously. The share has dropped over time — from ~14% in 2022 to ~9% in 2023 (per SlashData) — but remains higher than executives find acceptable.

If you are not measuring:

1. **Pick three metrics this quarter.** One Layer 1, one Layer 2, one Layer 3.
2. **Instrument them.** Even if crudely.
3. **Report weekly.** To yourself; monthly to your manager; quarterly to executives.
4. **Iterate.** As you learn what matters, refine.

Starting with three is far better than aspiring to a comprehensive dashboard.

## What not to measure (or, at least, what not to report up)

Some commonly-tracked metrics are noisy enough that reporting them up creates more confusion than insight:

- **GitHub stars in isolation.** See [`./vanity-metrics.md`](vanity-metrics.md).
- **Social follower counts.** Same.
- **Conference attendance numbers** (raw, without engagement context).
- **Newsletter subscriber counts** without engagement data.
- **Total blog page views** without per-post analysis.
- **"Reach"** without conversion data.

These are useful internally as health signals; they are not useful for executive reporting because they invite the question "and so what?" — a question that, asked honestly, often doesn't have a good answer.

## Connecting to AAARRRP

A useful exercise: take your current set of metrics and map each one to AAARRRP goals.

| Metric | Awareness | Acquisition | Activation | Retention | Referral | Revenue | Product |
|---|---|---|---|---|---|---|---|
| New signups | – | ● | – | – | – | – | – |
| TTFHW (median) | – | – | ● | – | – | – | – |
| 90-day retention | – | – | – | ● | – | – | – |
| Member-generated content | ● | – | – | – | ● | – | – |
| DQLs | – | ● | – | – | – | ● | – |
| Product feedback shipped | – | – | – | – | – | – | ● |
| Conference attendance | ● | – | – | – | – | – | – |

If your metrics only score on Awareness and Acquisition, you are running a marketing function with a DevRel label. If they only score on Activation and Retention, you are running a developer-success function. A balanced DevRel program produces metrics across all seven.

## Frequency and audience

Different metrics serve different audiences and cadences:

| Audience | Frequency | Focus |
|---|---|---|
| Daily team standup | Daily | Layer 3 activity check |
| Weekly team review | Weekly | Layer 2 community signals |
| Monthly leadership | Monthly | Layer 1 outcomes + commentary |
| Quarterly board / exec | Quarterly | Layer 1 outcomes vs. goals, big strategic stories |

## Specific metric families

The remaining files in this directory drill into each family:

- [`./activation-metrics.md`](activation-metrics.md) — TTFHW, activation rate, DQLs, the signup-to-shipped funnel.
- [`./community-metrics.md`](community-metrics.md) — Active members, contributor return, NPS, sentiment, orbit metrics.
- [`./business-impact.md`](business-impact.md) — Revenue attribution, influenced pipeline, ROI.
- [`./vanity-metrics.md`](vanity-metrics.md) — Stars, followers, and other deceiving numbers.

## Primary sources

- SlashData, *State of Developer Relations* reports (2022, 2023, 2024).
- Mary Thengvall, *The Business Value of Developer Relations* (Apress, 2018).
- Phil Leggetter, AAARRRP framework writings.
- DX (getdx.com), *State of Developer Experience* reports.
- Kamran Ayub, "DevRel metrics" reference (kamranayub.com).

## See also

- [`../03-frameworks/aaarrrp.md`](../03-frameworks/aaarrrp.md)
- [`../03-frameworks/orbit-model.md`](../03-frameworks/orbit-model.md)
- [`../03-frameworks/maturity-model.md`](../03-frameworks/maturity-model.md)