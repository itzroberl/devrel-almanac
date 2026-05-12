# Content Strategy

Content is the most-consumed output of any DevRel program. Done well, it compounds for years and quietly drives most of the team's measurable impact. Done badly, it produces noise no one reads, no one shares, and no one converts from.

## What "content" covers

For DevRel purposes, content includes:

- Documentation (covered separately in [`./documentation-as-product.md`](documentation-as-product.md)).
- Blog posts and long-form writing.
- Tutorials and quickstarts.
- Sample applications and demo repositories.
- Video (tutorials, conference talks, screencasts, shorts).
- Podcasts (own and guest appearances).
- Newsletters.
- Social posts (X, Bluesky, LinkedIn, Mastodon).
- Webinars, livestreams, and event recordings.

These should be coordinated, not produced in parallel silos. A weekly content meeting that pulls together everything the team is producing is the minimum operational discipline.

## The four jobs content does

Map every piece of content to at least one of these jobs:

1. **Awareness.** Reach developers who do not yet know your product exists.
2. **Activation.** Help developers who have signed up successfully use the product.
3. **Retention.** Help developers go deeper or solve new problems with the product.
4. **Trust / authority.** Demonstrate that your team understands the domain at the highest level.

A piece of content that serves none of these is a candidate for not being made. A piece that serves multiple is high-leverage.

(For a more granular goals model, see [`../03-frameworks/aaarrrp.md`](../03-frameworks/aaarrrp.md).)

## Content formats and what they're good for

| Format | Primary job | Strengths | Costs |
|---|---|---|---|
| Reference docs | Activation, retention | Always-on; AI-readable | High maintenance |
| Quickstart | Activation | Drives first hello-world | Must be perfect; high stakes |
| Tutorial (written) | Activation, awareness | SEO-friendly; long shelf life | Time-consuming |
| Long-form essay / thought piece | Awareness, trust | High shelf-life; reach | Risk of empty thought leadership |
| Comparison / benchmark | Awareness | High click-through; HN-friendly | Must be honest |
| Sample app | Activation | Highest signal of "yes, you can build with this" | Expensive to maintain |
| Video tutorial | Awareness, activation | YouTube search; broad reach | Production cost |
| Short video (60-second) | Awareness | Algorithmic boost; share-friendly | Hard to do well |
| Live stream | Trust, awareness | Authentic; community-forming | Slow audience growth |
| Conference talk | Awareness, trust | Compounds (recordings); credibility | Travel cost |
| Podcast guest | Awareness, trust | High-trust reach | Time |
| Podcast (own) | Trust, retention | Brand build | Slow; high failure rate |
| Newsletter | Retention, awareness | Direct relationship | Cadence demand |
| Case study | Trust, awareness | Credibility | Requires customer cooperation |
| Release notes | Retention | Required if you ship | Should be excellent |

## Diátaxis: a useful documentation framework that applies broadly

Daniele Procida's Diátaxis framework distinguishes four documentation types by user need:

- **Tutorials** — Lessons. Goal: learning. Hand-holding.
- **How-to guides** — Recipes. Goal: solve a specific problem. Concise.
- **Explanation** — Background. Goal: understanding. Why something exists.
- **Reference** — Information. Goal: lookup. Comprehensive and exact.

Most DevRel content failure traces to mixing these. A "tutorial" that is actually reference is unhelpful for learning; a "reference" that is actually explanation is unfindable when you need an answer.

Apply Diátaxis to *all* content, not just docs. A blog post is usually a how-to or an explanation, occasionally a tutorial. Be explicit which.

## Voice and authorship

- **Named authors outperform corporate accounts.** Always credit the writer.
- **Engineers should write under their own names.** Ghostwriting for engineers is detectable and corrosive.
- **The author should be reachable.** A real bio with links to their personal sites / handles signals authenticity.

## SEO discipline

- **Target a specific search query** per long-form piece.
- **Avoid keyword stuffing.** Google penalises it; AI assistants are even less forgiving.
- **Optimise for the question, not the keyword.** "How do I deploy Next.js to AWS?" matters more than "AWS Next.js deployment."
- **Update old content.** A 2021 post that ranks well is a maintenance opportunity, not a finished project.
- **Internal linking matters.** Every post should link to 3–5 other posts on your site.

## AI-readiness

From 2024 onward, content is consumed by both humans and LLMs. Practical implications:

- **Use semantic HTML / Markdown.** Clear headings, lists, tables.
- **Be explicit about versions** and dates.
- **Code samples should be runnable and complete.**
- **Avoid burying key information in images** without alt text.
- **State conclusions early.** AI assistants extract the first informative paragraph.

See [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md).

## Distribution

A common mistake: assume publishing equals distribution. It doesn't.

For every piece of long-form content, plan distribution:

- Your own newsletter.
- Cross-post to dev.to / Hashnode with canonical URLs.
- LinkedIn carousel or essay version.
- X / Bluesky thread or post.
- Reddit (in appropriate subreddit, if the post is genuinely useful).
- Internal Slack channels asking employees to share.
- Targeted email to high-relevance individuals.
- (Where appropriate) Hacker News submission.

A weak post with strong distribution outperforms a strong post with weak distribution. Both is the goal.

## Cadence

- **Weekly cadence outperforms monthly perfection** for most teams.
- **Set a publishing schedule** the team commits to.
- **Front-load batched recording** (video, podcast) to absorb production variance.
- **Maintain a 4–6-week content calendar.**

## Content audit

Once a year, audit existing content:

- Remove or update anything stale.
- Identify your highest-performing pieces; clone the format.
- Identify topical gaps.
- Consolidate duplicates.

The most underrated DevRel activity is cleaning up old content. A maintained corpus of 200 evergreen posts is worth more than 800 dated posts.

## See also

- [`./documentation-as-product.md`](documentation-as-product.md)
- [`../03-frameworks/aaarrrp.md`](../03-frameworks/aaarrrp.md)
- [`../08-tools/documentation-tools.md`](../08-tools/documentation-tools.md)
- [`../09-platforms/youtube-tech.md`](../09-platforms/youtube-tech.md)