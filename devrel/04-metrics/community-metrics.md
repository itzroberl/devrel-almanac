# Community Metrics

Layer 2 of the metrics stack: how is the developer community around your product doing? These metrics are leading indicators for Layer 1 business outcomes. A weakening community in Q1 produces weakening retention in Q2 and weakening revenue in Q3.

## Active members

The foundational metric for any community.

### Definitions

- **DAU / WAU / MAU.** Daily, weekly, monthly active users.
- **What "active" means.** Posted? Reacted? Logged in? Each is a different threshold. Pick one and apply it consistently.
- **Per-channel and aggregate.** Track per Discord server, Discourse forum, GitHub repo, etc., and a deduplicated aggregate.

### What's healthy

- **DAU/MAU ratio of 20–40%** indicates a sticky community.
- **Sustained MAU growth** quarter over quarter for a growing product.
- **Sustained MAU at scale** for a mature product (decline is a serious signal).

## Contributor return rate at 90 days

What percentage of community members who contributed something in a 90-day period return to contribute again in the next 90-day window?

- **Healthy.** 25–40% return rate for sustained programs.
- **Unhealthy.** Under 15% suggests members try, get a bad first-contribution experience, and never come back.

This is one of the most diagnostic community-health metrics because it measures whether the community actually retains contributors rather than churning them.

### What counts as a contribution?

Define carefully. Common definitions:

- A merged code PR.
- A reviewed PR.
- An answer that the asker accepted.
- A community-channel message at a defined threshold of quality.
- A submitted talk.
- A published content piece tagged to the company.

Many teams use a **quality-weighted contribution score**: different contribution types are worth different points. A talk delivered = 50; a merged PR = 30; a substantive forum answer = 10; a Discord message = 1.

## First-response time

How long does it take for a community-posted question to receive a substantive response?

- **Goal.** Under 4 working hours during business hours for first response; under 24 hours always.
- **Important.** Track median, p90, p99. The p99 (worst case) often matters more — it's the user whose first impression is "no one answered me."

## Member NPS

Net Promoter Score asked specifically of community members: "How likely are you to recommend this community / product to a peer?"

- **Scale.** 0–10.
- **NPS = % promoters (9–10) – % detractors (0–6).**
- **Benchmarks.** For developer products, scores above +40 are healthy; +60 is excellent; +20 or lower is a yellow flag.

NPS is most useful when:

- Run quarterly.
- Followed up with qualitative free-text question.
- Trended over time (the trajectory matters more than the absolute number).
- Stratified by member type (advocates vs. casual users).

## Sentiment

What's the emotional valence of conversations about your product?

- **Manual.** Review a sample of community posts and AI-assist or analyst-classify into positive / neutral / negative.
- **Automated.** AI-driven sentiment analysis over message corpora (Common Room and similar tools provide this).

Most useful trended over time and cross-referenced with product/event launches. A sentiment dip following a release tells you something specific.

## Orbit metrics

If you operate the Orbit Model (see [`../03-frameworks/orbit-model.md`](../03-frameworks/orbit-model.md)):

- **Orbit-level distribution.** How many Explorers, Participants, Contributors, Advocates?
- **Transition rates.** Explorer → Participant, Participant → Contributor, Contributor → Advocate, over each period.
- **Reverse-transition rates.** Outflow from Advocate / Contributor / Participant orbits.

Healthy communities show inflow at every transition; struggling communities show outflow at one transition that bottlenecks the rest.

## Member-generated content volume

How much content (posts, videos, talks, PRs, sample apps) is your community producing?

- **Volume per period.**
- **Reach of that content** (where measurable).
- **Cross-platform.** Some members are loud on Discord but produce no public content; others are quiet but write influential blog posts.

This is one of the strongest signals of Advocate-orbit health.

## Cross-platform identity resolution

To compute most of these metrics rigorously, you need to resolve the same human being's identity across platforms. The same person may be:

- A GitHub username.
- A Discord ID.
- An email address.
- A Twitter / Bluesky handle.
- A LinkedIn name.

Without identity resolution, you can only measure per-platform activity. With it, you can measure the human.

Tools that help: Common Room, LFX Community Data Platform, custom warehouse joins. See [`../08-tools/community-crm-platforms.md`](../08-tools/community-crm-platforms.md).

## Geographic and demographic distribution

For global programs, monitor:

- **Geographic spread.** Country / region distribution of active members.
- **Language distribution.** What languages do community posts happen in?
- **Time-zone distribution.** Is your community always-on or concentrated?

Useful for identifying regions where investment would expand the community vs. regions where existing investment is paying off.

## Survey-based metrics

Annual or biannual surveys of the community surface things metrics cannot:

- What are members' goals?
- What blocks them?
- What do they wish your product did?
- Why did they choose your product over alternatives?
- What would make them recommend it more?

The SlashData *State of the Developer Nation* survey methodology is a good reference for designing one.

## Anti-patterns

- **Tracking only growth, not retention.** A community can grow rapidly while bleeding members at the back end.
- **Treating Discord member count as community health.** Many of those members will never post.
- **Conflating engagement with sentiment.** Loud is not the same as positive.
- **Reporting community metrics without business connection.** "MAU is up 20%" produces "and so?" from executives unless connected to downstream outcomes.

## See also

- [`./metrics-overview.md`](metrics-overview.md)
- [`./activation-metrics.md`](activation-metrics.md)
- [`./business-impact.md`](business-impact.md)
- [`../03-frameworks/orbit-model.md`](../03-frameworks/orbit-model.md)
- [`../08-tools/community-crm-platforms.md`](../08-tools/community-crm-platforms.md)