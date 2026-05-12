# Vanity Metrics

Numbers that look like they tell you something but don't. Every DevRel program produces some; the trick is to use them internally as health signals while never reporting them up as if they were business outcomes.

## GitHub stars

The canonical vanity metric.

### What stars don't mean

- **They don't mean usage.** A starred repository may have zero installs.
- **They don't mean adoption.** A developer can star a repo while never running it.
- **They don't mean active use.** A repo can have 50,000 stars and three commits per year.
- **They don't translate to revenue.** Many of the most-starred open-source projects have nothing to do with the commercial entities behind them — and vice versa.

### What stars do mean

- **Brand awareness in a specific niche.** A repo with 10K stars has been seen by a meaningful number of developers in that niche.
- **A discovery signal.** GitHub's trending pages rank by star velocity; high star velocity correlates with continued discovery.
- **Social proof.** First-time visitors look at star count as a heuristic for "is this serious?"
- **A consistent threshold marker.** When a repo crosses 1K, 10K, 100K stars, it gets a small boost of attention.

### Use them for

- Internal trend monitoring (is this repo gaining attention?).
- Comparative ranking of your own properties.
- Casual conversation: "we're at X stars."

### Don't use them for

- Reporting impact to executives.
- Comparing yourself to other companies' stars (different categories, different incentives).
- Deciding budget allocation.

## Social-media followers

X, Bluesky, LinkedIn, YouTube subscriber, Mastodon followers — all vanity at the count level.

### What they don't tell you

- **Engagement rate matters more than count.** 50K engaged followers > 500K passive.
- **Audience composition matters.** 10K developers who are decision-makers > 100K passive consumers.
- **Algorithmic visibility ≠ actual reach.** Most posts reach a small fraction of stated followers.

### What they do tell you

- **Trajectory.** A growing audience suggests reach growth; a flat one suggests stagnation.
- **Relative scale.** Helpful in comparing two of your own accounts.
- **Recognition threshold.** Some thresholds (10K, 100K) confer real opportunities — speaker invitations, sponsorship offers, recognition.

### Use them for

- Trend monitoring.
- Tracking your team members' growth (signals their work is landing).

### Don't use them for

- Reporting "reach" to executives.
- Comparing to competitors who play different platforms differently.
- Justifying activity spend in isolation.

## Conference attendance numbers

Booth scans, badge taps, "we reached 5,000 developers at re:Invent."

### Why they're often misleading

- **Most scans aren't qualified.** A swag-grab is not engagement.
- **The number says nothing about post-event behaviour.** Did any of them activate?
- **Aggregating across qualities of contact** disguises which conversations mattered.

### Better metrics

- **Qualified booth conversations.** Defined by length, depth, or outcome.
- **Post-event activation rate** of attendees who provided contact info.
- **Pipeline-influenced ARR** from event-sourced opportunities.

## Newsletter subscriber count

A growing list looks like value. It often is, but the count alone tells you less than:

- **Open rate.** Healthy is 30–50% for developer-focused newsletters.
- **Click-through rate.** 2–5% click-through is healthy.
- **Reply rate.** Subscribers who reply are far more valuable than passive ones.
- **Unsubscribe rate.** Above 1% per send is a yellow flag.
- **Cost per active subscriber.** If you're paying to acquire them.

## Blog page views

Aggregated views tell you that something happened. They don't tell you what.

- **Per-post view distribution.** A few posts often produce most traffic; investigate them.
- **Time on page.** A 30-second visit isn't reading.
- **Bounce rate.** Did the visitor go anywhere else?
- **Conversion from blog to signup / docs.** The actual outcome.

## Discord member count

A 50,000-member Discord can have 50 active members. The shape of the activity distribution matters more than the count.

- **DAU/MAU ratio.**
- **Post-frequency distribution.** Are the same five people posting everything?
- **First-response time.** Is the community helping each other?

## Why vanity metrics persist

Because they are **easy to measure** and **directionally not meaningless**. Stars do correlate weakly with usage; followers do correlate weakly with reach; views do correlate weakly with awareness. The problem is they correlate *too weakly* to substitute for the real outcome metric, and substituting them produces:

- False confidence when they go up.
- False alarm when they go down for reasons unrelated to your actual work.
- Mis-allocated budget when activities optimised for the vanity metric are not the same as activities optimised for the underlying outcome.

## The "and so?" test

A quick test for whether a metric is vanity:

> When you report this number to your executive, what is their natural next question?

If the answer is "and so?" or "compared to what?" — and you can't answer those questions in business terms — you have a vanity metric.

Real metrics have built-in answers:

- "Cost per activated developer was $X." → and X is below paid-acquisition cost, validating DevRel investment.
- "DevRel-influenced ARR was $Y." → and Y is Z% of total ARR, indicating function importance.
- "TTFHW reduced 18%." → and that drove activation rate up N points, which produces M more retained customers per quarter.

Vanity metrics don't have those built-in answers.

## Use them internally; don't report them up

The general rule:

- **Track everything** internally; use it for diagnosis.
- **Report only the business-grounded metrics** upward.
- **Translate vanity metrics into business terms** before they leave the team.

A weekly internal dashboard might track 50 metrics. A monthly executive report should contain 5 — the ones that map to AAARRRP goals and connect to revenue.

## See also

- [`./metrics-overview.md`](metrics-overview.md)
- [`./business-impact.md`](business-impact.md)
- [`../09-platforms/github-as-platform.md`](../09-platforms/github-as-platform.md)