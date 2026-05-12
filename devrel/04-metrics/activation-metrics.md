# Activation Metrics

For product-led developer products, activation is the most important DevRel-influenced outcome. It is also the most clearly measurable, which is part of why PLG companies have come to treat DevRel as core revenue infrastructure rather than as marketing brand-build.

## Time to first hello world (TTFHW)

The single most important DevRel-related activation metric. Measures elapsed time from "developer arrives at your docs / site / signup" to "developer has produced visible output from your product."

### Definitions matter

Define carefully:

- **Start.** Account creation? First docs visit? First SDK install?
- **End.** First successful API call? First app that runs locally? First deploy?
- **Successful path only?** Or all signups, including those who abandon?

Most teams use:

- **Start = account creation.**
- **End = first successful API call** (for API products) or **first successful build / deploy** (for platforms).
- **Median across all signups in the period**, with separate tracking for completed vs. abandoned funnels.

### Targets

- **API products.** Under 5 minutes for the median is the gold standard. Under 15 minutes is acceptable. Over 30 minutes is structural.
- **Platforms with more setup.** Under 30 minutes is good. Over an hour is usually painful.

### How to improve TTFHW

In rough order of impact:

1. **Reduce signup friction.** Email-only signup; defer credit-card collection.
2. **Pre-generate API keys** at signup; no separate "create key" step.
3. **Show a working sample on the first screen.** Curl, then SDK, with API key auto-filled in the docs.
4. **Embed runnable sandboxes** in the quickstart.
5. **Fix the quickstart itself.** Most quickstarts are too long and assume too much.

## Activation rate

The percentage of new signups who reach a defined activation milestone within a defined window.

### Definition

- **Milestone.** Product-specific. Common patterns:
    - "First successful API call" (Twilio, Stripe, Algolia).
    - "First deploy" (Vercel, Netlify, Heroku-style).
    - "First query result returned" (MongoDB Atlas, Neon, Supabase).
    - "First production-grade integration" (a higher bar; better signal but slower).
- **Window.** Often 7 days; sometimes 30. Match it to how long it actually takes serious evaluators in your category.

### Benchmarks (rough, varies massively by category)

- **B2B SaaS overall.** 15–25% activation rate, 25–40% for mature products. (Per analytics-vendor data.)
- **Mobile apps.** 20–35%.
- **Fintech / regulated products.** 10–20% due to compliance friction.

For developer products specifically, top-quartile performers achieve substantially higher activation rates than these general benchmarks suggest — Stripe, Twilio, Postman, and similar companies report activation rates significantly above the SaaS-overall figures on their best-performing onboarding flows.

### Why it matters

Activation is the single largest leverage point in a PLG funnel. Doubling activation rate doubles every downstream metric. Investing in better docs, faster quickstart, better samples, and clearer error messages compounds across all subsequent stages.

## Developer-qualified leads (DQLs)

A concept introduced by Mary Thengvall in 2019 to give DevRel teams a vocabulary for business value parallel to marketing-qualified leads (MQLs) and sales-qualified leads (SQLs).

A DQL is an external person who can contribute value to the company in ways that extend beyond a sales prospect. Categories:

- **Builders.** Developers who integrate your product into a meaningful application.
- **Contributors.** Developers who contribute to your open-source efforts or community.
- **Evangelists.** Developers who recommend your product publicly.
- **Partners.** Developers at companies that could integrate with or build on you.
- **Influential community members.** Developers with reach in their networks.

### How to use

- Define your specific DQL criteria.
- Score qualification (a Builder DQL ≠ an Evangelist DQL).
- Track DQL volume per quarter.
- Track conversion of DQLs to long-term value (revenue, sustained contribution, etc.).
- Use the vocabulary in conversations with marketing and sales to signal that DevRel produces value comparable to other functions.

### Operational pitfalls

- **DQL inflation.** If your bar is too low, you produce many "DQLs" with little downstream value. Set high standards.
- **DQL vs. MQL confusion.** Different criteria; don't conflate.
- **Attribution complexity.** A single DQL may have been influenced by multiple DevRel activities; choose an attribution model and apply it consistently.

## Onboarding funnel metrics

For mature programs, instrument the full onboarding funnel and track conversion at each step:

```
Visit docs site
  ↓ (X%)
View quickstart
  ↓ (X%)
Create account
  ↓ (X%)
Generate API key / install SDK
  ↓ (X%)
Run first sample
  ↓ (X%)
Make first authenticated API call
  ↓ (X%)
Make first authenticated API call in production
```

Each step has a drop-off rate. Identifying which step has the worst drop-off tells you where to invest.

## Time-to-Value variants

Beyond TTFHW, several related metrics measure deeper adoption:

- **Time to First Production Use.** First API call from a production environment.
- **Time to First Profitable App.** First app that generates measurable user activity / revenue.
- **Time to Habit.** First time a developer uses the product within 24h of the previous use.

Each measures something slightly different. TTFHW is the standard; the others are more sophisticated but require more instrumentation.

## Cohort analysis

A single TTFHW number hides variation. Cohort by:

- **Source.** Where the signup came from (docs, blog, conference, paid ad, referral).
- **Stack.** What language / framework they identified.
- **Geography.**
- **Time period.** Signups in week N vs. week N+1.

Cohort analysis often reveals that a single low-performing source is dragging the median; fixing that source produces disproportionate improvement.

## Tools

For instrumenting these metrics:

- **Product analytics.** Mixpanel, Amplitude, PostHog, Heap, June.
- **Data warehouse.** Snowflake, BigQuery, with raw event logs.
- **Survey tools.** Asking activated developers about their experience.

See [`../08-tools/analytics-tools.md`](../08-tools/analytics-tools.md).

## See also

- [`./metrics-overview.md`](metrics-overview.md)
- [`./community-metrics.md`](community-metrics.md)
- [`./business-impact.md`](business-impact.md)
- [`../10-tactics/documentation-as-product.md`](../10-tactics/documentation-as-product.md)
- [`../11-trends/plg-and-devrel.md`](../11-trends/plg-and-devrel.md)