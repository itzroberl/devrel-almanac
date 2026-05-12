# Developer Relations at AI / ML Companies

AI companies built or rebuilt their developer-relations functions over an unusually compressed window (roughly 2022–2026). Many of these teams did not exist in 2021; by 2026 several were among the most visible DevRel functions in the industry.

---

## OpenAI

OpenAI's developer organisation is structurally central to the company. The platform — APIs, fine-tuning, agent tooling, Realtime API — runs the developer business, and DevRel and developer product are tightly fused.

- **Romain Huet.** Head of Developer Experience. Previously held senior developer-product roles at Stripe.
- **Olivier Godement.** Head of Product, OpenAI Platform.
- **Logan Kilpatrick.** Developer Relations Lead at OpenAI from November 2022 through March 2024. Joined Google AI Studio as Product Lead in April 2024, where he leads work on Gemini developer enablement at Google DeepMind. One of the most-followed AI-DevRel voices on X / Bluesky.
- **Greg Brockman.** President; gives the "Developer State of the Union" at DevDay.
- **Mark Chen, Jakub Pachocki, and other research leadership** also operate as public-facing technical voices.

### OpenAI DevDay

- **DevDay 2023** (November 6, 2023, San Francisco) — first edition; introduced GPT-4 Turbo, Assistants API, GPT Store.
- **DevDay 2024** — distributed format (San Francisco, London, Singapore).
- **DevDay 2025** (October 6, 2025, Fort Mason, San Francisco) — 1,500+ developers in person, 780K+ YouTube keynote views. Announcements: Apps in ChatGPT, AgentKit, Sora 2, expanded Realtime API, audio model improvements.
- **DevDay programming** consistently includes hands-on labs, technical deep-dives by research engineers, and customer talks from major API integrators.

### OpenAI Cookbook and developer surfaces

- **OpenAI Cookbook** (github.com/openai/openai-cookbook) — Large open-source collection of recipes and reference implementations. Substantial community contribution. One of the most-consulted AI-developer-documentation surfaces.
- **OpenAI Forum** — Community space for technical discussion.
- **OpenAI Discord** — Active developer community.
- **OpenAI Platform docs** at platform.openai.com — Considered category-leading for AI API documentation; combines reference with conceptual content and Realtime / agentic patterns.

### Strategic position

OpenAI's developer-platform business is reported to be a substantial fraction of total revenue, growing rapidly. The developer organisation operates under product leadership rather than under marketing, which is structurally aligned to the PLG model — see [`../11-trends/plg-and-devrel.md`](../11-trends/plg-and-devrel.md).

---

## Anthropic

Anthropic's developer organisation has grown rapidly with Claude's adoption. The company's developer engagement has emphasised written content (deep technical posts on tool use, agentic workflows, prompt engineering) and high-quality documentation rather than evangelism at scale.

- **Alex Albert.** Head of Claude Relations / Developer Relations (in various phrasings); one of the most public Anthropic developer-facing voices. Substantial X / Bluesky presence and frequent author on the Anthropic blog.
- **Mike Krieger.** Chief Product Officer; one of the founders of Instagram. Substantial executive presence in developer-facing communications.
- **Dario Amodei (CEO) and Jack Clark (Co-founder / Policy)** also operate as public-facing voices, particularly on safety-and-policy-adjacent content that intersects with developer concerns.

### Claude Code

Anthropic's terminal-based AI coding agent.

- **Launched.** Public preview early 2025; v1.0 (general availability) May 2025.
- **GitHub adoption.** 82K stars, 6.4K forks, 558 commits, 51 contributors as of early 2026.
- **Features.** Terminal-native, IDE integrations, GitHub PR tagging (`@claude`), programmatic tool calling for agentic workflows, project-level memory via `CLAUDE.md` convention.
- **Significance.** Has become one of the most-adopted AI coding tools in the senior-engineer demographic; competes directly with Cursor, GitHub Copilot, Aider, and Continue.

### Anthropic Engineering Blog and *Building agents with Claude*

Substantial output on prompt engineering, tool use, agentic patterns, and safety. The blog is one of the canonical references for AI-application engineers in the 2024–2026 window. The *Building agents with Claude* series and the related cookbook (anthropic-cookbook on GitHub) have become reference material for AI-engineering teams.

### Model Context Protocol (MCP)

Anthropic launched the **Model Context Protocol** in November 2024 as an open standard for connecting AI systems to external applications. The ecosystem grew from ~100 servers in November 2024 to 17,000+ by early 2026. MCP has rapidly become a developer-relations surface in its own right — a new category of "executable documentation" — and is increasingly cross-supported by OpenAI, Google, and other model providers.

- **MCP Registry** (registry.modelcontextprotocol.io and adjacent indexes) — Discovery surface for MCP servers.
- **MCP SDKs** in Python, TypeScript, Go, Rust, Java, C# — All published openly, several with substantial external contributor communities.
- **Claude Desktop's MCP support** has been a major adoption driver since 2025.

---

## Hugging Face

Hugging Face (founded 2016) operates the largest open-source ML community in the world; its DevRel function is community-led at depth that no AI-product peer matches.

- **Clem Delangue.** Co-founder and CEO; deeply visible in developer communities.
- **Julien Chaumond.** Co-founder and CTO.
- **Omar Sanseviero.** Long-tenured Head of ML Growth and developer-relations leader; left Hugging Face in 2024 for Google DeepMind (developer-relations and growth work in AI).
- **Daniel van Strien.** Machine Learning Librarian, focused on datasets and community contribution patterns.
- **Patrick von Platen.** Core engineer on the diffusers library; substantial developer-facing impact through library design.

### Hugging Face Hub

The hub itself functions as a developer-relations surface — model cards, dataset cards, Spaces (gradio/streamlit apps), and community discussions are the primary engagement points.

### Hugging Face open-source libraries

`transformers`, `diffusers`, `datasets`, `tokenizers`, `accelerate`, `peft`, `trl`, `gradio` (acquired). Each library has its own contributor community and effectively its own DevRel surface.

---

## NVIDIA (AI focus)

NVIDIA's developer program (covered in [`./big-tech.md`](big-tech.md)) has rapidly become AI-centric. Notable AI-specific DevRel surfaces:

- **GTC.** GPU Technology Conference; the largest concentration of AI-developer content globally.
- **NVIDIA Inception.** 25,000+ AI/data startups participate.
- **CUDA developer community.** Decades old, central to all GPU-accelerated computing.
- **NVIDIA AI Enterprise** developer education.

---

## Cohere

- **Developer Platform.** Cohere's APIs (Command R, Command R+, Aya, Embed, Rerank).
- **DevRel team.** Smaller than OpenAI/Anthropic but active in technical content. Conferences include Cohere events at NeurIPS, etc.

---

## Mistral AI

- **Open-weight models** (Mistral, Mixtral) with substantial community adoption.
- **La Plateforme** (Mistral's commercial API).
- **Developer documentation** at docs.mistral.ai.

---

## Together AI

- **API platform** for open-source models.
- **Together Forum.**
- **Active DevRel** via tutorials, fine-tuning recipes, and open-source contributions.

---

## Replicate

- **API for running ML models** in the cloud.
- **DevRel and content** emphasises copy-paste-ready examples; one of the most accessible model-API onboarding flows.
- **Cog.** Open-source tool for packaging models, central to Replicate's developer ecosystem.

---

## Modal Labs

- **Serverless compute for AI/ML.**
- **DevRel team** has built a strong reputation for technical content and onboarding tutorials.

---

## LangChain

LangChain (founded 2022 by Harrison Chase) became the de facto orchestration framework for LLM applications during 2023.

- **Harrison Chase.** Founder, primary public face.
- **LangChain libraries.** Python and JavaScript libraries, then LangGraph for agentic workflows, then LangSmith for tracing and evaluation.
- **LangChain Academy.** Free training courses.
- **Community.** Discord, GitHub, very active.

---

## LlamaIndex

LlamaIndex (founded by Jerry Liu) became the dominant data framework for LLM applications, especially RAG.

- **LlamaHub.** Connector library / contribution surface.
- **LlamaCloud, LlamaParse.** Commercial offerings.
- **Active conference presence** and community-driven recipe library.

---

## Pinecone, Weaviate, Chroma, Qdrant

Vector databases for AI applications. Each has its own DevRel function:

- **Pinecone.** James Briggs (Senior Developer Advocate) is one of the most visible vector-DB educators on YouTube.
- **Weaviate.** Strong open-source community; weaviate.io tutorials and the Weaviate Podcast.
- **Chroma.** Open-source vector DB; growing community.
- **Qdrant.** Open-source; community-led.
- **Milvus / Zilliz.** Open-source vector DB; Milvus Community Calls.

---

## ML / AI tooling adjacent

- **Weights & Biases.** *Fully Connected* annual conference; developer education across LLM ops, experiment tracking. Lukas Biewald (founder).
- **Hugging Face.** (above).
- **MosaicML / Databricks.** (now part of Databricks).
- **Anyscale (Ray).** *Ray Summit* annual conference, active open-source DevRel.
- **MLflow (Databricks).** Open-source; community-led.
- **Comet, Neptune.ai.** Smaller ML-experiment-tracking DevRel.
- **Arize AI, WhyLabs.** AI observability; growing DevRel functions.
- **Braintrust, LangSmith (LangChain), Helicone, Langfuse.** LLM evaluation and observability; active developer-focused product marketing.

---

## AI coding tools

A category that did not exist in 2021 and is now substantial. AI coding tools have their own DevRel functions, many of which were built from scratch 2023–2026.

- **GitHub Copilot.** Microsoft / GitHub; large dedicated DevRel team and integrated marketing function. Substantial customer-education investment around Copilot for Business and Copilot Enterprise.
- **Cursor (Anysphere).** Founded 2022; rapid growth through 2024–2026; relatively small but high-leverage DevRel function operating primarily through founder-led content and engineering-led blogging.
- **Windsurf (Codeium).** AI IDE; substantial developer-marketing and content output.
- **Aider** (Paul Gauthier). Open-source CLI coding assistant; community-led, but Gauthier's posts and benchmarks are widely cited.
- **Continue.dev.** Open-source coding assistant; growing developer-community function.
- **Replit AI Agent.** Replit's agentic coding product; deep integration with broader Replit DevRel.
- **Tabnine.** Long-running AI coding assistant company; established enterprise developer-engagement function.
- **Sourcegraph Cody / Amp.** Sourcegraph's AI coding products; built on Sourcegraph's existing developer-tools DevRel infrastructure.
- **JetBrains AI Assistant / Junie.** Built on JetBrains' established DevRel function (see [`./devtools-platforms.md`](devtools-platforms.md)).
- **Augment Code, Codeium (separate from Windsurf), Magic.dev, Cline.** Emerging AI coding products with varying DevRel investment.

---

## AI infrastructure and inference platforms

Companies whose products are AI-specific infrastructure rather than models or coding tools. Substantial DevRel investment because developers building AI applications need to evaluate infrastructure decisions.

- **Modal Labs.** Serverless compute for AI; strong tutorial-and-recipe DevRel approach.
- **Together AI.** Open-model API platform; published model cookbook approach.
- **Replicate.** API for running ML models; pioneer of the "copy-paste-ready" AI-API onboarding.
- **Anyscale (Ray).** Distributed Python and ML; long-running open-source DevRel via the Ray community.
- **Fireworks AI, Groq, SambaNova.** Inference-optimised platforms; varying DevRel maturity.
- **RunPod.** GPU cloud; community-focused DevRel.
- **Lambda Labs.** GPU cloud and on-prem; education-focused DevRel.
- **CoreWeave, Crusoe.** Compute-infrastructure; nascent DevRel.

---

## AI engineering frameworks and orchestration

- **LangChain.** (above).
- **LlamaIndex.** (above).
- **Haystack** (deepset). Open-source LLM orchestration framework; substantial European community.
- **CrewAI, AutoGen (Microsoft), Phidata, Mastra.** Agent frameworks with varying community sizes.
- **Vercel AI SDK** (covered in [`./devtools-platforms.md`](devtools-platforms.md)).
- **Inngest, Trigger.dev, Convex.** Workflow / backend platforms with strong AI-engineering positioning.

---

## Cross-company observations

- **AI DevRel is extraordinarily front-loaded toward documentation and quickstarts.** The space is moving fast; deep multi-week onboarding loses to fast iteration.
- **Cookbook-style repositories have become canonical.** OpenAI Cookbook, Anthropic's recipe-style posts, LangChain templates, LlamaIndex examples — all built on github-as-the-primary-DevRel-surface.
- **MCP is reshaping the field.** AI-developer products increasingly expose MCP interfaces; DevRel teams design for both human developers and AI agents consuming their products.
- **LLM-first discovery.** Developers increasingly research products via ChatGPT, Claude, and Perplexity. DevRel teams optimise documentation for LLM ingestion as a primary objective. See [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md).
- **AI Engineer identity.** Shawn "swyx" Wang's *AI Engineer* conferences and the *Latent Space* publication anchor a distinct sub-field within DevRel for practitioners working at AI-adjacent companies.
- **Cross-pollination with traditional DevRel.** Many senior DevRel professionals at non-AI companies have specialised into AI-engineering DevRel since 2023, and many companies have hired AI-DevRel specialists onto previously-non-AI DevRel teams.

## See also

- [`./big-tech.md`](big-tech.md)
- [`./devtools-platforms.md`](devtools-platforms.md)
- [`../11-trends/ai-and-llms.md`](../11-trends/ai-and-llms.md)
- [`../06-people/current-leaders.md`](../06-people/current-leaders.md)
