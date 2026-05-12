# Perspectives and Debates

The DevRel-in-the-AI-era conversation has been substantive, contested, and dispersed across blog posts, podcasts, conference talks, and trade-press essays. This file collects the major named voices and the arguments they make, in a way that lets a reader find the underlying perspectives quickly.

For brevity, this file does not exhaustively recap each piece. It identifies who has staked out which positions and what the threads connecting them are.

## The "DevRel must adapt — and is more important than ever" camp

The dominant strand of optimistic argument.

### Angie Jones — *How DevRel is Leading AI Adoption* (2025)

Direct response to the "DevRel is dead" framing of 2022–2024:

> "A couple years ago, everyone was asking if DevRel was dead… Well, plot twist: we're not dead. We're standing on the biggest stage of our careers."

Her argument:

- Developers using AI need to see **real engineers learning AI-augmented practice in public**, not polished demos.
- AI is non-deterministic; developers learn most from failure-recovery sequences, which only humans can model authentically.
- DevRel's job is to **define the culture of AI adoption** — what good looks like, how to evaluate, how to debug, when to override.
- Content produced now ripples forward through companies as developers move jobs.

### AngelHack — *Developer Relations in 2026: Four Strategies For The AI Era*

Argues that the LLM is now the "first-touch user" of any developer product, reframing the function:

- "Gaps in your docs don't just frustrate developers anymore. They create gaps in AI-assisted adoption before a human ever enters the picture."
- API design is now a DevRel problem, not just an engineering one.
- "Prompts are the new support tickets" — when ~65% of developers report AI coding assistants missing relevant context, that signals a documentation problem.
- Higher-trust DevRel work (community strategy, developer-empathy research, product-feedback synthesis) is increasingly *the* DevRel job; the lower-leverage activities (tutorial production, generic content) commoditise.

### Doc-E AI — *The Future of AI in Developer Relations*

Positions AI as augmenting DevRel work rather than replacing it:

- AI tools assist with content drafting, community-signal detection, personalisation at scale.
- Humans remain irreplaceable for trust, authenticity, technical credibility, and strategic relationships.
- The successful 2025–2026 DevRel professional uses AI as leverage but maintains human-led work at the audience interface.

### Shawn "swyx" Wang and the AI Engineer position

While not strictly framed as a DevRel argument, swyx's positioning of the **AI Engineer identity** (and the entire *Latent Space* corpus) functions as a perspective on what DevRel for AI products should look like:

- A new category of developer is forming; they need different content, different community spaces, different tooling.
- The AI Engineer Summit, the Latent Space podcast, and the AI Engineer Foundation have institutionalised the identity.
- DevRel teams whose products serve AI Engineers must engage on AI-Engineer-specific channels.

## The "DevRel as practised had to die — and is being rebuilt" camp

A more bracing strand of argument, dating from the 2022–2024 layoff wave but with continued relevance.

### MB Consulting — *RIP DevRel 2010–2024: Why It Died and How to Stop Killing It*

A 2024 post-mortem arguing:

- DevRel died not because of AI, but because companies systematically misused it.
- "DevRel is not marketing. Sure, it can work *with* marketing, but reducing it to a lead-generation tool is like asking a Michelin-starred chef to sling burgers at a drive-thru."
- The DevRel-as-content-marketing pattern is what's being cut. The DevRel-as-strategic-function pattern survives.

This argument is structurally compatible with the "DevRel is more important than ever" camp; it just attributes the failure to misuse, not to AI itself.

### Mary Thengvall's evolving framing

Through her *DevRel Weekly* newsletter, *Community Pulse* podcast appearances, and consulting work, Thengvall has been consistent that:

- DevRel that can't articulate business value will keep getting cut.
- AI doesn't change the fundamental need for the function; it changes the operational mix.
- The vocabulary of Developer Qualified Leads (DQLs) and AAARRRP-style strategy frameworks remains the right substrate.

The combination — strategic clarity plus AI-era operational adaptation — is the through-line of her current work.

### James Governor and RedMonk

The RedMonk perspective, articulated across blog posts and conference talks by Governor and Stephen O'Grady, has consistently been:

- Developers remain the most important constituency in tech procurement — the *Kingmakers* thesis from 2013 has only been reinforced by AI.
- AI tools amplify whichever developer products are already authoritative on the open web.
- The companies that built strong open-source-led, community-led, content-rich DevRel functions in 2015–2022 are reaping disproportionate AI-era benefits.

## The "Agent Experience is the new DX" camp

A more operational perspective focused on what concretely changes for DevRel teams.

### Anthropic developer-facing essays

Through 2024–2026, Anthropic's engineering blog has argued (through both explicit posts and implicit through-tool design):

- Documentation written for agents matters as much as documentation written for humans.
- MCP is a primary developer-facing surface, not a side project.
- Cookbook-style repositories with complete runnable examples outperform polished marketing material for adoption.
- The same content can serve both audiences if the structural craft is right.

### Mintlify product team

Mintlify's blog and product evolution from 2024 onward represents another operational argument:

- Documentation is increasingly read by machines; tools should serve that reality.
- `llms.txt` and `llms-full.txt` auto-generation should be a default feature, not a premium add-on.
- Documentation platforms must serve dual audiences and shouldn't ask the customer to choose.

### Latent Space community

A continuing thread of AI Engineer Summit talks and Latent Space podcast episodes have developed the practical AX vocabulary — tool naming, MCP design, evals, observability — that DevRel teams at AI-adjacent companies now use as the operational baseline.

## The "Sentiment vs telemetry" camp

A specific empirical sub-debate visible across 2024–2026.

### Faros AI's *Sentiment surveys aren't enough in the AI era*

Argues that developer sentiment about AI productivity ("I love this tool, it makes me so much faster") consistently overstates measured productivity gains, especially when measured behaviourally rather than perceptually.

Implications for DevRel: don't trust your post-event surveys. Don't trust your post-launch NPS. Supplement everything with telemetry.

### JetBrains HAX study (April 2026)

Two-year telemetry study of 800 developers using AI assistants. Headline finding:

- Developers using AI write more code, but spend over a third of their time editing AI suggestions.
- Edit frequency increased substantially even though developers perceived minimal change.
- Time savings averaged 3.6 hours per week; daily users showed 60% higher PR throughput.
- Trust gaps persist.

For DevRel, the implication is the sentiment-telemetry gap is real and structural. Treat survey data as one signal, not the signal.

### Anthropic's skill-formation research

Flags that AI assistance both accelerates productivity on already-known skills *and* may hinder the formation of new ones. For DevRel teams in education-adjacent products, this is a genuine strategic question; for infrastructure teams, it's a forecast of customer-support patterns.

## The critical / sceptical camp

Genuine challenges to the dominant 2024–2026 enthusiasm.

### Signals.sh — *Does llms.txt actually work?* (2026)

Two empirical studies through 2026 found no measurable lift in AI citations correlated with publishing `llms.txt`. Zero documented AI bot fetches of `llms.txt` files in production server logs.

Implication: much of the "AI-era DevRel" advice is unvalidated. Some of it is performative.

### The "DevRel is dead because AI" thread

A persistent strand of argument visible in trade press and individual Substacks through 2024–2026, varying in seriousness:

- AI generates all the content DevRel produces, so why pay for DevRel?
- AI answers developer questions, so community management is obsolete.
- AI writes the docs, so technical writers are unnecessary.

These arguments are mostly weak in their strong form (AI doesn't generate trust, doesn't moderate communities at scale, doesn't replace authentic engineering brand) but contain a kernel of truth: certain DevRel activities *have* been substantially commoditised by AI, and teams that haven't reorganised around the activities that remain valuable are in genuine difficulty.

### The "DevRel as marketing channel" critique

Continues from the 2022–2024 layoff debate. Argues that AI accelerates the demise of DevRel-as-content-marketing because AI can produce more content faster and cheaper. The corollary: DevRel that survives in the AI era must do work AI can't — strategic relationships, community trust, founder-led storytelling, deep technical empathy.

## The "founder-led" camp

A more specific perspective, mostly visible in founder-led AI-product companies.

### Patrick Collison (Stripe), Guillermo Rauch (Vercel), Mitchell Hashimoto

Founder-led DevRel patterns intensify in the AI era because the founder's voice is authentically uncopyable. AI can generate competitive product summaries; it cannot generate Patrick Collison's voice. For early-stage AI-product companies particularly, founder-as-DevRel is increasingly the default — see [`../06-people/founders-as-devrel.md`](../06-people/founders-as-devrel.md).

### Harrison Chase (LangChain), Jerry Liu (LlamaIndex), Clem Delangue (Hugging Face)

AI-product founders functioning as the primary DevRel voice for their respective companies through 2023–2026. Their pattern: heavy in-public writing, frequent podcast appearances, candid discussion of product evolution, sustained presence in technical communities.

The argument running through this group's work: in AI's rapidly-evolving moment, the founder is the only credible voice on what the product is going to be next quarter.

## What's *not* contested

Despite the disagreement, several things have wide consensus across the camps:

- LLM-mediated discovery is now a substantial fraction of developer research and is growing.
- Documentation is increasingly read by AI agents, and writing for them matters.
- The lowest-leverage activities of pre-AI DevRel (generic listicles, content marketing) are being cut.
- Authentic human voices — founders, senior engineers, trusted educators — matter more than ever.
- The function is going to keep evolving; this is the early-middle of a multi-year transition.

The disagreement is on the operational specifics, not the macro picture.

## Where to read further

- *Latent Space* (podcast and newsletter) — swyx and Alessio Fanelli. The defining AI-engineering publication.
- *DevRel Weekly* — Mary Thengvall's curated newsletter.
- *Community Pulse* podcast — DevRel-community perspectives.
- *Angie Jones's blog* (angiejones.tech) — *How DevRel is Leading AI Adoption*.
- *AngelHack blog* — *Developer Relations in 2026* essay.
- *MB Consulting blog* — *RIP DevRel* post-mortem and follow-ups.
- *Anthropic engineering blog* — Practical agent-design and documentation essays.
- *RedMonk blog* — Industry analysis.
- *AllThingsOpen DevRel track* and *DevRelCon* talk archives — primary venues for the discourse.

## See also

- [`./critical-takes.md`](critical-takes.md)
- [`./early-signals-what-works.md`](early-signals-what-works.md)
- [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md)
- [`./inspiration-stays-human.md`](inspiration-stays-human.md)
- [`../11-trends/layoffs-and-renaissance.md`](../11-trends/layoffs-and-renaissance.md)