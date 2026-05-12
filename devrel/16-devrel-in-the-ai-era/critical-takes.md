# Critical Takes

A fair AI-era DevRel reference must take the sceptical arguments seriously. Some of them are strong; some of them are weak. This file lays them out, plus the rebuttals where they apply.

The aim is intellectual honesty. Not all the 2024–2026 hype about AI-era DevRel survives careful examination.

---

## Critical take 1 — "DevRel is dead because AI can do it"

The strong-form version: AI can generate documentation, answer community questions, produce tutorial content, and explain products to developers. So why pay for DevRel?

### Where this take is right

- A substantial fraction of pre-2023 DevRel work was producing tutorial-style content, FAQ answers, and "X for beginners" posts. AI assistants now generate this kind of content competently. Teams that built their value around this work *are* in genuine trouble.
- First-line community support — "How do I X?" questions — is increasingly handled by AI before reaching humans. Community managers whose value was answering basic questions need to redefine their value.
- Anyone whose DevRel work is volume-of-content-produced is competing directly with AI's near-zero marginal cost.

### Where this take is wrong

- AI does not generate trust. A community manager who shows up reliably for years builds a kind of trust no AI can synthesise.
- AI does not have a reputation that compounds. A founder who writes thoughtfully across a decade accrues authority no LLM can replicate.
- AI does not have *taste*. The hard editorial decisions — which controversial position to take, which engineering trade-off to discuss honestly, which design pattern to recommend — require human judgement.
- AI cannot moderate communities at scale. Conflict resolution, code-of-conduct enforcement, nurturing emerging contributors — these are deeply human.
- AI cannot represent the developer to the company. The bidirectional bridge function of DevRel requires someone with both technical credibility and political access internally.

The rebuttal in summary: AI commoditises the *production* work of DevRel. It does not commoditise the *trust, taste, judgement, and relationship* work, which is where the function's actual leverage was always supposed to be. Teams structured around the former are dying; teams structured around the latter are doing fine.

---

## Critical take 2 — "Most AI-era DevRel advice is unvalidated"

A subtler but more important critique. Specifically:

- `llms.txt` is widely adopted but two 2026 studies found no measurable AI-citation lift correlated with publishing it. Server logs from real production sites report essentially zero AI bot fetches of `llms.txt` files.
- The 2024–2026 GEO/AEO tooling category (Profound, AthenaHQ, Otterly.AI, etc.) reports wildly different numbers using different methodologies. Their absolute claims should be treated cautiously.
- Single-anecdote "we tripled our AI citations by doing X" posts are almost always unreproducible and often retroactive.
- Sentiment about AI tools systematically overstates measured productivity (Faros AI, JetBrains HAX, Anthropic skill-formation research).

### Where this take is right

- Much of the 2024–2026 AI-DevRel advice is performative. People are doing things that look like AI optimisation without evidence they actually work.
- The tooling category is young and immature. Its measurements are noisy.
- DevRel teams that bet heavily on `llms.txt` as their primary AI strategy are likely overinvesting.

### Where this take is wrong

- "Unvalidated" doesn't mean "useless." `llms.txt` is cheap; the forcing function of producing it improves documentation hygiene regardless of direct AI-citation effect.
- The absence of measurable effect in 2026 may just mean the measurement methods are bad. Several decades of SEO research had this same problem.
- Some AI-era practices *do* show measurable effects (clean OpenAPI specs, runnable code samples, schema markup, consistent canonical naming, dated content). The critique applies more strongly to specific tools and conventions than to the broad direction.

The rebuttal in summary: take the empirical critique seriously, instrument what you can, don't fall for confident-sounding claims with thin evidence, but don't conclude that nothing about the AI era is real. The macro trend — developers researching via AI assistants — is well-documented; only the specific tactical interventions are uncertain.

---

## Critical take 3 — "Developer-experience surveys are no longer reliable"

A specific empirical critique from operational engineering teams.

The argument:

- Developer-sentiment surveys are widely used to assess AI-tool effectiveness.
- Telemetry consistently shows that the sentiment overstates the reality. Code churn rises, edit frequency rises, errors rise, but developers report feeling more productive.
- Several research efforts (Faros AI, JetBrains HAX study with 800 developers across two years, Anthropic skill-formation research) all confirm this gap.

### Where this take is right

- Surveys are insufficient on their own.
- DevRel teams that rely on "we asked developers and 80% love it" are probably overstating their impact.
- The post-launch NPS that gets reported up to executives is often misleading.

### Where this take is wrong

- It doesn't argue against measurement; it argues for *better* measurement. Surveys plus telemetry plus behavioural data triangulate to truth.
- The gap doesn't mean developer perception is worthless. Felt productivity is a real outcome; it affects retention, advocacy, and product loyalty. Just not the only outcome.

The rebuttal in summary: instrument both. Don't trust either alone.

---

## Critical take 4 — "AI-generated DevRel content fails"

A point most working practitioners agree with but worth stating explicitly.

The argument:

- DevRel teams have experimented with using LLMs to scale content production. Most attempts have failed.
- AI-generated technical content is detectable, anodyne, and often subtly wrong.
- Developer audiences are sophisticated and notice. Engagement collapses.
- Trying to scale DevRel through AI-generated content has been a consistent failure mode in 2024–2026.

### Where this take is right

- Empirically true. Most pure-AI-generated content marketing produces worse outcomes than less-of-it-but-real-voice content.
- The temptation to use AI to "scale" DevRel work is widespread and usually wrong.

### Where this take is wrong

- It doesn't argue against AI assistance, only against AI *replacement*. AI as drafting tool, editing tool, signal-detection tool — these work fine. AI as primary author of the public surface — this fails.

The rebuttal in summary: use AI to leverage human work, not to replace it.

---

## Critical take 5 — "DevRel is being absorbed into other functions, not surviving as its own thing"

A structural critique. Some patterns:

- Many companies are merging DevRel into Product Marketing, Developer Experience Engineering, or Customer Engineering.
- Job titles like "Developer Advocate" are sometimes being replaced with "DX Engineer" or "Developer Experience Engineer" reporting through Product.
- The pure-DevRel function has been contracting; adjacent functions have absorbed parts of its responsibility.

### Where this take is right

- This is happening at some companies. Particularly at later-stage developer-product companies, the DevRel-Function-As-Such is sometimes being unbundled into specialist roles (DX Engineer, Documentation Engineer, Community Manager) reporting through different leaders.
- The dual-audience thesis (see [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md)) accelerates this trend because the work split increasingly justifies specialist hiring.

### Where this take is wrong

- Specialisation isn't extinction. The function is being unbundled, but the underlying work is mostly being done by people who would have been called DevRel in 2018. The label changes; the discipline persists.
- At earlier-stage companies, the integrated DevRel function is still typical and effective. Specialisation is a scale-stage choice.

The rebuttal in summary: the function is evolving and specialising, not disappearing. Career advice for DevRel practitioners is to develop deep skill in one of the sub-disciplines (community, education, documentation, advocacy, marketing, AX engineering) rather than trying to remain a generalist forever.

---

## Critical take 6 — "AI is hollowing out junior developer skill formation"

A specific concern that applies to DevRel-adjacent products.

The argument:

- AI tools accelerate productivity on tasks developers already know.
- They may hinder skill formation on tasks developers don't yet know — the developer accepts AI output, the work gets done, but no skill is acquired.
- For junior developers in particular, this risks producing a cohort that can't operate without AI assistance.

### Where this take is right

- The empirical evidence (Anthropic's 2026 skill-formation research, anecdotal evidence from senior engineering managers across many companies) supports the concern.
- DevRel teams in education-adjacent products face a real strategic question.

### Where this take is wrong

- Every previous developer-tool generation faced this critique. Calculators, IDEs, search engines, Stack Overflow — each was accused of hollowing out skill. Each was assimilated; the next generation of developers became more productive *and* developed different (sometimes deeper) skills.
- Plausibly the same will be true of AI. The senior developer of 2035 will have skills the senior developer of 2025 doesn't.

The rebuttal in summary: take the concern seriously without being alarmist. For DevRel teams in education contexts, design content that explicitly teaches *first principles* alongside AI usage. Don't pretend AI-assisted shortcuts are equivalent to having learned the underlying material.

---

## Critical take 7 — "The 2026 AI-DevRel hype cycle will look embarrassing in 2030"

A meta-critique sometimes made by senior practitioners.

The argument:

- Every wave of developer-relations transformation (cloud, mobile, OSS, microservices, DevOps, blockchain, AI) generates a wave of certain-sounding advice. Most of the advice doesn't survive the cycle.
- Much of the 2024–2026 AI-DevRel writing — including this section, in honest self-awareness — will look quaint or wrong in 2030.
- "AI Engineer," "Agent Experience," `llms.txt`, even MCP itself may turn out to be names for things that were temporarily prominent.

### Where this take is right

- Probably true at the level of specific tools and terms. MCP may not be the protocol name in 2030; specific tools that look central now may be footnotes.

### Where this take is wrong

- The underlying directions — agents reading docs, AI mediating developer discovery, the dual-audience structural split, AX as a discipline — are probably durable even if their names change.
- "Some of this will look embarrassing" is not the same as "all of this is wrong." The honest version is: act on what's strong; instrument the rest; be willing to revise.

The rebuttal in summary: epistemic humility is warranted. Don't bet the strategy on any single 2024–2026 convention. But don't use uncertainty as an excuse for inaction — the macro shift is real even if the tactical details will evolve.

---

## The honest synthesis

If you take all seven critiques seriously, the position that emerges is roughly:

1. **AI does substantially change DevRel.** Not in the "DevRel is dead" sense, but in the "what DevRel does, who it talks to, and what it measures changes" sense.
2. **Much of the 2024–2026 advice is performative.** Particularly the specific tactical claims about `llms.txt`, GEO tools, and specific AI-citation tactics. Be cautious; instrument; don't trust confident-sounding marketing.
3. **The most durable changes are structural.** The dual-audience split, the rise of MCP as an integration standard, the importance of authentic human voice, the centrality of clean documentation. These will outlast the tactical fashion.
4. **DevRel functions are unbundling.** The integrated generalist DevRel role is contracting at scale; specialist roles (DX, AX, community, education) are growing.
5. **Sentiment is unreliable.** Use telemetry.
6. **Founders matter more.** Authentic voice is harder to replicate when everything else is mass-produced.
7. **Be patient about evidence.** Several years of research will sort what works from what doesn't. In the meantime, instrument what you can, default to discipline over fad, and don't over-commit to any single convention.

This is more cautious than the marketing version of AI-era DevRel and probably closer to how seasoned practitioners actually navigate the moment.

## See also

- [`./perspectives-and-debates.md`](perspectives-and-debates.md)
- [`./early-signals-what-works.md`](early-signals-what-works.md)
- [`./metrics-in-ai-era.md`](metrics-in-ai-era.md)
- [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md)
- [`../11-trends/layoffs-and-renaissance.md`](../11-trends/layoffs-and-renaissance.md)