# Sample Apps and Demos

A working sample application is the most credible evidence a developer can get that your product does what you say it does. Sample apps and demos are central to DevRel work, but they are also one of the most consistently mismanaged assets in the field.

## Why sample apps matter

- **They prove the product works** in a way prose cannot.
- **They reduce TTFHW** from "build something from scratch" to "clone and run."
- **They are durable.** A well-maintained example repo serves new users for years.
- **They are evaluable.** A potential customer or partner can read your sample apps to assess product quality without talking to sales.
- **They feed AI assistants.** LLMs trained on or referencing public code use your sample apps as reference for how to use your product.

## Categories of sample apps

| Type | Purpose | Example |
|---|---|---|
| **Quickstart sample** | First five minutes | A 50-line script that calls your API and returns visible output |
| **Cookbook recipe** | Specific use case | "Build webhooks that trigger Slack messages" |
| **Integration sample** | Show product working with another product | "Stripe + Next.js + Vercel" |
| **Reference app** | Complete working application | A whole chat app, e-commerce app, dashboard |
| **Industry vertical sample** | Domain-specific | "Insurance claims processor using our API" |
| **Architectural pattern sample** | Show best practice | "Event-driven architecture with our SDK" |

A mature DevRel program runs all of these. Most teams cover quickstart and cookbook well, neglect reference apps, and rarely produce vertical samples.

## Where to host them

- **GitHub.** Your `/examples` or `examples` repo, or per-language repos.
- **CodeSandbox / StackBlitz embedded** in docs.
- **One-click deploys** (Vercel "Deploy" button, Netlify "Deploy to Netlify" button, Heroku-style buttons).
- **In-browser playgrounds** (your own product if it supports them).

For most teams, GitHub is the canonical home; embedded sandboxes and one-click deploys are layered on top.

## Maintenance is everything

The single most common failure: shipping sample apps and then letting them rot.

- **API versions drift.** Yesterday's sample uses today's deprecated SDK.
- **Dependency drift.** A 2-year-old example pulls 2-year-old vulnerable dependencies.
- **Documentation drift.** The blog post that links to it references behaviour that no longer matches the repo.

A maintenance-free sample app is not free — it accumulates debt. Plan for it:

- **CI on every example repo.** If the test fails, the example is broken.
- **Quarterly audit.** Each sample gets touched at least once a quarter.
- **Owner per example.** A specific DevRel team member responsible.
- **Deprecation policy.** Old samples are explicitly retired, not just left to rot.

The maintenance overhead is the reason most teams should have fewer, better samples rather than more, worse ones.

## What makes a good sample

- **It does one thing well.** Don't combine 5 features into one demo.
- **It is complete.** Includes all imports, .env file template, deploy instructions.
- **It is readable.** Documented; idiomatic; not cleverly optimised at the cost of clarity.
- **It is realistic.** Uses real-world patterns, not "hello world" toys.
- **It works.** CI ensures it.
- **It is up-to-date.** Last commit within the last 90 days, ideally.

## Recipe model: Cookbook repositories

Several leading companies operate "cookbook" repositories that house dozens or hundreds of small recipes:

- **OpenAI Cookbook** (github.com/openai/openai-cookbook).
- **Anthropic Cookbook.**
- **Stripe samples.**
- **Twilio Code Exchange.**
- **Algolia Recipes.**

The cookbook model spreads the maintenance burden across many small examples, each with a clear scope. It is the dominant pattern for AI-era developer companies.

## Reference apps

A reference app is a complete working application that demonstrates how to build a real thing with your product. Examples:

- **Vercel Commerce** — a complete e-commerce template.
- **Supabase examples** — full-stack auth-included apps in multiple frameworks.
- **Stripe SaaS demo** — full subscription-business reference.

Reference apps are expensive to build and maintain but disproportionately valuable to evaluators. They turn "can this product do real work?" from a question into a demonstration.

## Templates and starters

Adjacent to sample apps: templates and starters.

- **Next.js templates** (vercel.com/templates).
- **Astro themes.**
- **Supabase quickstarts** for various stacks.
- **Vite templates** for various frameworks.

Templates lower TTFHW dramatically. For framework-and-platform products, they are essential.

## AI-readiness

Sample apps are heavily consumed by AI coding assistants. To make them AI-friendly:

- **Public on GitHub** (not behind login).
- **Permissive licence** (MIT, Apache 2.0).
- **Clear README** describing what the sample does.
- **Logical file structure** that AI can navigate.
- **No half-finished code** — a partial example confuses LLMs.

Many AI-era DevRel teams now publish their sample apps with explicit "designed to be ingested by AI assistants" framing — and structure them accordingly.

## Sample app strategy summary

1. Decide what types of samples you need (quickstart, cookbook, integration, reference).
2. Pick a hosting pattern (single `/examples` repo or per-purpose repos).
3. Assign owners.
4. CI every sample.
5. Audit quarterly; retire ruthlessly.
6. Optimise for AI ingestion as well as human reading.
7. Link samples from docs at every relevant point.

## See also

- [`./documentation-as-product.md`](documentation-as-product.md)
- [`../08-tools/code-sandboxes.md`](../08-tools/code-sandboxes.md)
- [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md)
- [`../04-metrics/activation-metrics.md`](../04-metrics/activation-metrics.md)