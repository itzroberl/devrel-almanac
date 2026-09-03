# Documentation Tools and Platforms

Documentation is the single most important DevRel surface for most developer-product companies. In product-led growth motions, the docs *are* the salesperson. The documentation-tools market has matured into a serious category, with billions of dollars in market cap and multiple distinct competitive lanes.

The category in 2026 splits roughly into:

- **API reference generators** (OpenAPI-driven).
- **General-purpose docs site builders.**
- **Hybrid platforms** combining reference, conceptual content, tutorials, and developer hub features.

---

## Mintlify

- **Founded.** 2021.
- **Positioning.** "Docs your users will love." AI-native, design-led, hosted.
- **Strengths.** Beautiful default design; quick setup; strong AI integration (Mintlify AI search, Q&A).
- **Used by.** Anthropic, Perplexity, Resend, Cursor, and many AI-era developer-product companies.
- **Notable feature.** AI-assisted writing and AI-readable output formatting that many AI-company DevRel teams prioritise.

---

## Docusaurus

- **Founded.** Originally by Meta (Facebook) in 2017; donated as open source.
- **Architecture.** React-based static site generator; uses MDX (Markdown with React components).
- **Strengths.** Full control, version-controlled docs, free, large ecosystem of plugins.
- **Used by.** Hundreds of developer-product companies including Supabase, Algolia, Babel, Redocly, many CNCF projects.
- **Best for.** Teams that want to own their docs pipeline and customise heavily.

---

## ReadMe

- **Founded.** 2014 (Greg Koberger).
- **Positioning.** Interactive API documentation with a developer hub.
- **Strengths.** Try-It-Now consoles, personalised API key handling per logged-in user, OpenAPI ingestion.
- **Used by.** Hundreds of API companies including various fintech and developer-product companies.
- **Pricing.** Mid-to-high-end SaaS; enterprise focus.

---

## GitBook

- **Founded.** 2014.
- **Positioning.** "Knowledge platform" — combines docs-as-code (Git-backed) with WYSIWYG editing and AI-powered search.
- **Strengths.** Editor-friendly; good for teams with non-engineer writers.
- **Used by.** Wide range, especially smaller startups and internal team docs.

---

## Stoplight

- **Founded.** 2015; acquired by SmartBear in 2023.
- **Positioning.** API design and documentation; visual OpenAPI editor.
- **Strengths.** Schema-first design; mock servers; collaborative API design.
- **Used by.** API-product teams that want strong design-time tooling.

---

## Redocly

- **Founded.** 2015 (as Redoc, an open-source OpenAPI documentation tool).
- **Open source.** Redoc remains widely used as a standalone OpenAPI renderer.
- **Commercial.** Redocly platform adds versioning, custom theming, and enterprise features.
- **Used by.** Many large API-driven products; particularly common in enterprise contexts where Stoplight competes.

---

## Apiary

- **Founded.** 2011; acquired by Oracle 2017.
- **Status in 2026.** Still operational but no longer a category leader; many of its early customers migrated to Stoplight, Redocly, or Postman.

---

## Bump.sh

- **Founded.** 2019, France.
- **Positioning.** API documentation as a continuous deployment artefact.
- **Strengths.** Diff visualisation across API versions; good change-management.

---

## Theneo

- **Founded.** 2021.
- **Positioning.** AI-first documentation generation from OpenAPI specs.
- **Strengths.** Speed of initial scaffold; AI-assisted writing.

---

## Notion as docs platform

- **Notable.** Some smaller companies use Notion (with Notion's developer-API surface) as their public docs. Works for simple cases; lacks API-doc-specific features.

---

## VuePress, Hugo, Jekyll, Astro, Eleventy

- **General-purpose static site generators** widely used for docs.
- **Astro Starlight** has emerged as a popular Docusaurus alternative for technical docs in 2024–2026.
- **Hugo** powers many DevOps / SRE / Kubernetes docs (e.g., kubernetes.io).
- **Jekyll** remains the substrate for many older corporate docs sites and most of github.io.

---

## API reference generators (specialised)

- **Swagger UI** — Original OpenAPI renderer; ubiquitous; basic styling.
- **Redoc** — Above.
- **RapidDoc** — Alternative OpenAPI renderer.
- **Slate** — Markdown-driven, three-column docs (historic; less actively maintained now).
- **Docsy** — Hugo-based theme widely used by CNCF projects.
- **[Sourcey](https://sourcey.com/oss)**. Open-source generator for combining OpenAPI, MCP,
  Doxygen XML, godoc, rustdoc, MkDocs, and Markdown in one self-hosted static HTML site. Its
  mixed-source workflow is useful when reference and guides need one build; choose another tool
  when a hosted editor or non-HTML output is required.

---

## Adjacent tools

- **Snyk Open Source / Sourcegraph Cody / Sourcegraph Code Search** — used by some DevRel teams for code-aware doc validation.
- **Vale** — Open-source prose linter; used by many docs teams for consistency.
- **Algolia DocSearch** — Free Algolia program for open-source docs sites; provides search backend for many of the largest open-source docs (React, Vue, Astro, MDN historically).
- **MkDocs and MkDocs Material** — Python-ecosystem favourite, particularly for project docs.

---

## Documentation strategy considerations

Three architectural choices that matter more than tool selection:

1. **Reference vs. conceptual vs. tutorials.** Different audiences and different goals. The Diátaxis framework (by Daniele Procida) is the dominant conceptual model: Reference, How-to, Tutorial, Explanation. Most tools support all four but tools that *enforce* the separation are rare.
2. **Single-source-of-truth.** OpenAPI specs as source-of-truth produce always-correct reference docs and reduce maintenance burden. Worth the discipline.
3. **AI-readiness.** From 2024 onward, documentation is consumed both by humans and by LLMs (developers asking ChatGPT/Claude/Perplexity about your product). Structure, semantic markup, and consistent formatting matter for AI ingestion. See [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md) and [`../10-tactics/documentation-as-product.md`](../10-tactics/documentation-as-product.md).

---

## How to choose

| If you… | Consider |
|---|---|
| Want fastest path to good-looking docs and have an OpenAPI spec | Mintlify |
| Want maximum control and have engineering capacity | Docusaurus or Astro Starlight |
| Have a complex API + need interactive consoles | ReadMe |
| Want non-engineers to contribute | GitBook |
| Are designing the API from scratch | Stoplight |
| Need one self-hosted site from mixed API, code-reference, and Markdown sources | Sourcey |
| Run open-source on Hugo/Jekyll already | Stay on your generator; add Docsy or similar themes |
| Want enterprise versioned multi-product portal | Redocly |

The most common mistake is **switching docs tools mid-stream**. Migrations are painful. Choose deliberately and live with the choice.

## See also

- [`../10-tactics/documentation-as-product.md`](../10-tactics/documentation-as-product.md)
- [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md)
- [`./code-sandboxes.md`](code-sandboxes.md)
