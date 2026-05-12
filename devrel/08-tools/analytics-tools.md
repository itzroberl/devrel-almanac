# Analytics Tools

DevRel teams measure two distinct things and need different tooling for each:

- **Product analytics** — what developers do inside the product (signup, activation, retention).
- **Community analytics** — what developers do in spaces *around* the product (GitHub, Discord, social, conferences).

This file covers the major tools in each lane.

---

## Product analytics

### Mixpanel

- **Founded.** 2009.
- **Positioning.** Product analytics for tracking events, funnels, cohorts, retention.
- **Strengths.** Mature funnel and retention analysis; strong cohort segmentation.
- **Used by.** Many SaaS products including developer products for onboarding-funnel analysis.

### Amplitude

- **Founded.** 2012.
- **Positioning.** Product analytics with stronger emphasis on experimentation and behavioural cohorts.
- **Strengths.** Big-data scale; AI-assisted analysis; experimentation tooling.
- **Used by.** Many large product-led-growth companies.

### Heap

- **Founded.** 2013.
- **Positioning.** Auto-capture analytics — track everything and define events retroactively.
- **Strengths.** No upfront instrumentation; flexible event definition.
- **Used by.** Companies prioritising agility over schema discipline.

### PostHog

- **Founded.** 2020.
- **Open source.** Yes — self-hostable.
- **Positioning.** All-in-one product analytics, session replay, feature flags, A/B testing, surveys.
- **Strengths.** Open source friendly to developer-product companies; strong default privacy posture; growing rapidly in 2024–2026 among developer-first companies.
- **Used by.** Many YC-stage and developer-product startups.

### June, Mixpanel-alternatives

- **June, Fathom (analytics), Plausible, Umami.** Smaller alternatives; some privacy-focused.

### Snowplow

- **Open-source event-data pipeline.** Used by larger orgs to own their own event-collection layer rather than outsourcing.

---

## Web analytics (for content)

- **Google Analytics 4 (GA4).** Default for many docs sites; non-trivial migration from older Universal Analytics.
- **Plausible.** Privacy-first, simple metrics.
- **Fathom.** Similar.
- **Cloudflare Web Analytics.** Free, privacy-respecting, simple.
- **Vercel Analytics, Netlify Analytics.** Platform-bundled analytics.

---

## Search and SEO tools

- **Ahrefs, Semrush, Moz.** SEO tools for understanding how developers find content.
- **Google Search Console.** Free, essential for any docs site.
- **Algolia DocSearch logs.** What developers search inside your docs.

---

## Community analytics

### CNCF DevStats

- **Premise.** Tracks all CNCF projects' contribution activity (PRs, issues, comments, reviews) by contributor, country, organisation, over time.
- **Free, open-source.** Dashboards at devstats.cncf.io.
- **Significance.** The reference standard for measuring open-source health in a foundation-led project.

### LFX Community Data Platform

- **The Linux Foundation's evolution of crowd.dev.** Free for open-source projects. See [`./community-crm-platforms.md`](community-crm-platforms.md).

### CHAOSS (Community Health Analytics for Open Source Software)

- **A Linux Foundation project.** Defines metric standards for open-source community health.
- **Practitioner-led**; provides metrics models that DevStats and other tools implement.

### GrimoireLab

- **Open-source analytics platform** for software-development data; underpins DevStats and Bitergia services.

### Bitergia Analytics

- **Commercial.** Analytics services built on GrimoireLab; used by many large open-source foundations.

### Orbit (model) implementations

- **Orbit Model** as a measurement framework can be implemented in any analytics stack. See [`../03-frameworks/orbit-model.md`](../03-frameworks/orbit-model.md).

### Common Room, Savio

- **Covered in [`./community-crm-platforms.md`](community-crm-platforms.md).**

### GitHub Octoverse / GitHub Insights

- **Octoverse** is GitHub's annual state-of-software report; built on GitHub's internal analytics.
- **GitHub Insights** (formerly part of Pull Panda; integrated into GitHub Enterprise) provides repo-level analytics for individual repositories.

### Discord and Slack analytics

- **Native Discord analytics** are limited; many teams supplement with custom bots writing to a warehouse.
- **Slack Analytics** is limited at the Free tier and substantial at Enterprise Grid.
- **Common Room and Orbit-derived tools** sit on top of these to provide cross-channel views.

### Stack Overflow / Reddit / dev.to analytics

- **Stack Overflow tag-watching** and search-data; modest in 2026 given platform decline.
- **Reddit's official analytics** for subreddit moderators; less useful for content discovery.
- **dev.to dashboard** for authors and organisations.

---

## Data warehouse + BI stack (for serious DevRel orgs)

The most sophisticated DevRel teams stop relying on individual SaaS dashboards and pull data into a warehouse:

- **Warehouse.** Snowflake, BigQuery, Databricks, Redshift, PostgreSQL.
- **Ingestion / ELT.** Fivetran, Airbyte, Stitch; raw GitHub / Discord / Slack / Discourse / Postman / Salesforce API pulls.
- **Transformation.** dbt for SQL modelling.
- **BI / visualisation.** Looker, Mode, Hex, Metabase, Superset, Tableau, Power BI.

This approach scales indefinitely and gives the team full control of definitions (what counts as "active contributor," "qualified developer lead," etc.).

The trade-off is that it requires data-engineering capability the team may not have.

---

## What to track

The metrics most often tracked by mature DevRel teams (see [`../04-metrics/`](../04-metrics/) for detail):

- **Funnel:** awareness → signup → first hello world → activation → retention.
- **Community:** active users, contributor return rate, sentiment, NPS.
- **Content:** views, completion rate, search queries, AI-assistant retrieval frequency.
- **Events:** registration vs. attendance, post-event activation, share-rate.
- **Pipeline / revenue:** DevRel-influenced revenue, DQL pipeline.

A common failure mode is to instrument everything possible and report on nothing. Pick the 10–20 metrics that connect cleanly to AAARRRP goals and refresh weekly. Everything else is for ad-hoc analysis only.

## See also

- [`../04-metrics/metrics-overview.md`](../04-metrics/metrics-overview.md)
- [`../04-metrics/activation-metrics.md`](../04-metrics/activation-metrics.md)
- [`../04-metrics/community-metrics.md`](../04-metrics/community-metrics.md)
- [`./community-crm-platforms.md`](community-crm-platforms.md)