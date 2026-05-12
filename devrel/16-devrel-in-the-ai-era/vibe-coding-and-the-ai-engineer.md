# Vibe Coding and the AI Engineer

Two adjacent identity shifts in the developer population that DevRel teams must understand: the rise of the "AI Engineer" as a recognised category since 2023, and the cultural emergence of "vibe coding" as a practice since early 2025. Both shift who DevRel is talking to and what those people care about.

## The AI Engineer

Coined by **Shawn "swyx" Wang** in his June 2023 essay *The Rise of the AI Engineer*. The argument:

- A new role is forming between traditional ML engineers (who train models from scratch) and traditional software engineers (who don't touch ML at all).
- This role uses foundation-model APIs, prompt engineering, retrieval-augmented generation (RAG), evals, and agentic frameworks to build AI-powered applications.
- "A wide range of AI tasks that used to take five years and a research team can now be accomplished with API docs and a spare afternoon."
- Andrej Karpathy endorsed the framing publicly shortly after publication, which gave the identity legitimacy.

By 2026, "AI Engineer" is an established career identity:

- The **AI Engineer Summit** (founded by swyx) is one of the most-attended specialist developer conferences.
- The **Latent Space podcast and newsletter** (swyx + Alessio Fanelli) reaches over 10 million readers and listeners across 2025. The defining publication for the role.
- The **AI Engineer Foundation** institutionalises the identity.
- Job postings titled "AI Engineer" appear at most developer-product companies; pay tends to be competitive with senior software engineering.

For DevRel teams, AI Engineers are a distinct audience with distinct preferences:

- They consume content that assumes familiarity with embeddings, vector databases, RAG, agentic patterns, prompt engineering, evals, and the broader ML application stack.
- They evaluate products primarily through hands-on experimentation in notebook environments (Jupyter, Colab, Cursor, Claude Code).
- They participate in distinct community spaces (Latent Space Discord, OpenAI Discord, LangChain Discord, Hugging Face Hub).
- They are inundated with AI-product marketing and have well-developed filters against it.

DevRel teams whose products serve AI Engineers cannot rely on generic developer-marketing playbooks. They need AI-Engineer-specific content, presence on AI-Engineer channels, and AI-Engineer-credible spokespeople.

## Vibe coding

Coined by **Andrej Karpathy** on February 2, 2025 in a public post:

> "There's a new kind of coding I call 'vibe coding', where you fully give in to the vibes, embrace exponentials, and forget that the code even exists."

The practice: a developer describes intent in natural language, an AI agent generates the code, the developer accepts the changes without examining them in detail, runs the result, pastes any errors back, and iterates. The code is not really "written" in the traditional sense; the developer steers a conversation with the agent and accepts what works.

Karpathy explicitly framed this as appropriate for "throwaway weekend projects" rather than production systems. The framing got picked up far beyond its original scope — by late 2025, "vibe coding" was being used to describe everything from quick scripts to substantial production work, with mixed outcomes.

### Why this matters for DevRel

Vibe coding redefines what "developer" means at the margin. Two new audience patterns:

**Pattern 1: Existing developers vibe-coding adjacent work.**

A backend engineer who vibe-codes a quick admin panel. A frontend developer who vibe-codes a CLI tool. A senior engineer who vibe-codes prototypes for design exploration. This pattern is mainstream; most working developers in 2026 vibe-code at the margin.

For DevRel, this means: your product is increasingly evaluated through the lens of "can I get an AI agent to build with this in 30 minutes?" If the answer is "yes," you win. If the answer is "no" because the agent gets confused by your docs or your API ergonomics, you lose.

**Pattern 2: New developers who only vibe-code.**

People who never learned to write code in the traditional sense, but who use AI agents to build software. By 2026, this is a real and growing population. Designers building tools. Domain experts building internal apps. Founders building first MVPs.

For DevRel, this is a *new audience* that needs a different style of engagement:

- They don't read technical reference docs the way traditional developers do.
- They evaluate products by whether ChatGPT or Claude can successfully integrate them.
- They participate in different communities (Replit, Bolt, Lovable, Cursor-adjacent spaces).
- Their failure modes are different (they often can't debug deeply when the AI fails).

The 2025 essay "When Vibe Coding Goes Wrong" and many follow-ons in 2026 documented patterns: stripped tests, ignored security advice, leaked secrets, abandoned codebases. The risks are real. But the audience is large enough and growing fast enough that ignoring it is strategically untenable for many developer products.

### Implications for DevRel content

DevRel content patterns that work for vibe-coders:

- Quickstarts that an AI agent can read and faithfully execute (see [`./documentation-for-agents.md`](documentation-for-agents.md)).
- "Build this with AI" tutorial format — explicitly assume the reader is using Claude Code, Cursor, or ChatGPT.
- Sample apps that exhibit best practices the AI agent will copy.
- Plain-language explanations of concepts that agents tend to get wrong.
- Recovery patterns — when the AI agent inevitably produces broken code, what should the developer do?

Most teams in 2026 have not yet figured out the right balance. The DevRel teams winning at the vibe-coding audience are aggressively iterating on quickstarts, sample apps, and AI-readable docs while preserving the deeper material for traditional developers.

## The JetBrains Human-AI Experience (HAX) research

In April 2026, JetBrains published the *Human-AI Experience* study analysing two years of telemetry from approximately 800 developers using AI coding assistants. Headline findings relevant to DevRel:

- Developers using AI assistants write more code overall.
- They spend more than one-third of their time double-checking and editing AI suggestions.
- Editing frequency increased substantially among AI users, even though developers themselves perceived minimal change.
- Time savings averaged 3.6 hours per week for regular users; daily users showed 60% higher pull-request throughput.
- Significant trust gaps remained: even regular users reported incomplete trust in AI-generated code.

The implication: AI assistance reshapes developer behaviour in ways that often elude developers' own perceptions. *Actual* behaviour and *perceived* behaviour diverge. DevRel teams using user surveys to measure their product's AI-mediated experience get distorted signal; supplementing with telemetry is necessary.

This is the empirical grounding for the wider observation that *sentiment about AI productivity tends to overstate measured productivity*. DevRel teams that lean only on developer surveys overestimate how well their AI-mediated work is going.

## The skill-formation question

Anthropic's research on how AI assistance affects skill development (early 2026) flagged a genuine concern: AI both accelerates productivity on already-known skills *and* may hinder the acquisition of new ones.

The pattern observed: developers who lean heavily on AI for tasks they don't yet understand often end up *less* able to do those tasks unaided. The AI does the work; the developer doesn't form the skill.

For DevRel teams at education-adjacent products (JetBrains Academy, courses by Wes Bos / Scott Tolinski, Frontend Masters, etc.), this is a genuine strategic question: how do you teach developers to use AI productively *and* to retain skill formation? In 2026 the answer is still being worked out.

For DevRel teams at infrastructure / tool companies, the implication is more straightforward: assume that some fraction of your customer-developers will struggle to debug deeply because they have offloaded skill formation to AI. Build your product, docs, and community to compensate — clearer error messages, more accessible community help, more "first principles" content that re-teaches what AI tends to elide.

## The cultural texture

A few specific cultural shifts visible in the developer population around AI work:

- **The end of "I write all my code."** A statement that was identity-defining in 2022 is now rare. Most developers in 2026 acknowledge AI involvement in their work; the variation is in degree.
- **The new prestige of evals and observability.** Among AI Engineers, the ability to *evaluate* AI output is increasingly the prestige skill. Tools like Braintrust, LangSmith, Helicone, Langfuse are central. DevRel teams in this space talk about evals as much as DevRel teams in 2018 talked about CI/CD.
- **The "show your prompts" pattern.** Developers share prompts the way they used to share dotfiles. Public prompt libraries are a thing. DevRel teams produce sample prompts as deliverables.
- **The "skill collapse" anxiety.** Among senior developers, real concern that the next generation won't develop the depth they did. DevRel teams that help mitigate this — clear teaching content, transparent agent behaviour, debugging-with-AI guides — earn long-term goodwill.

## Practical takeaways for DevRel teams

1. **Identify whether your product serves AI Engineers, vibe-coders, traditional developers, or some mix.** Each requires different content.
2. **Treat agent-readable surfaces as primary, not as a future concern.** Your docs are being consumed by AI agents *today*.
3. **Don't abandon traditional-developer content.** The audience is still large, and its depth of trust matters.
4. **Sponsor Latent Space and AI Engineer Summit appropriately.** If your product is AI-Engineer relevant, this is the canonical channel.
5. **Track vibe-coding-mediated activation as a separate cohort.** It behaves differently from traditional developer activation.
6. **Engage the skill-formation question honestly.** Don't pretend AI just makes developers better; the truth is more nuanced and developers know it.

## See also

- [`./the-dual-audience-thesis.md`](the-dual-audience-thesis.md)
- [`./inspiration-stays-human.md`](inspiration-stays-human.md)
- [`./metrics-in-ai-era.md`](metrics-in-ai-era.md)
- [`../05-companies/ai-companies.md`](../05-companies/ai-companies.md)
- [`../06-people/influencers-by-platform.md`](../06-people/influencers-by-platform.md)

## Primary sources

- Shawn Wang, *The Rise of the AI Engineer*, June 2023 (latent.space / swyx.io).
- Andrej Karpathy, post on "vibe coding" via X / personal blog, February 2, 2025.
- JetBrains, *Understanding AI's Impact on Developer Workflows*, April 2026 (HAX study).
- Anthropic, *How AI assistance impacts the formation of coding skills*, 2026.
- Latent Space podcast and newsletter, 2023–2026.