# Organisational Structures for Developer Relations

Where DevRel sits and how it is sized determines almost everything that follows: budget, goals, headcount progression, the kinds of metrics it is held to, and its ability to influence product. There are no universally correct answers, but there are correct answers for a given company. This file maps the common structural choices and their trade-offs.

## Reporting line options

### Option 1 — Report to Marketing

**Used by.** Roughly one-third of surveyed organisations as of 2024 (SlashData / State of Developer Relations).

**Strengths.**
- Marketing has the budget, the brand machinery, the demand-gen infrastructure, and the launch coordination.
- DevRel can plug into existing campaigns, paid distribution, and event sponsorships.
- Career path into marketing leadership is clear.

**Weaknesses.**
- Pressure to contribute to top-of-funnel pipeline metrics distorts content toward conversion rather than education.
- Developers' authenticity radar fires when DevRel content reads as marketing.
- Engineers in DevRel roles report cultural drift away from product/engineering credibility.

**Best fit.** Early-stage companies needing brand reach; companies where the existing marketing team is technically literate.

### Option 2 — Report to Product

**Used by.** ~22% (2024 SlashData).

**Strengths.**
- Tight integration with the product roadmap; developer feedback flows into PRD.
- DevRel can credibly say "we represent developers" because the team has product authority.
- Aligns naturally with product-led growth motions where the product is the salesperson.

**Weaknesses.**
- Marketing distribution can suffer; great content doesn't reach the audience.
- Sales sees DevRel as not contributing to pipeline.
- DevRel becomes feature-launch support rather than category leadership.

**Best fit.** PLG companies where activation is the primary growth driver.

### Option 3 — Report to Engineering

**Used by.** Smaller share, more common at infrastructure and developer-tools companies.

**Strengths.**
- Maximum technical credibility.
- Direct line to engineers, which is where the answers and the future product lives.
- Engineers in DevRel roles feel like peers, not "marketing in a hoodie."

**Weaknesses.**
- Engineering leaders rarely measure or value the public-facing work the same way marketing does.
- Less budget flexibility.
- Can over-index on "we built a thing, let's tell developers about it" rather than "developers need X, we should build it."

**Best fit.** Companies where the product is deeply technical and where credibility with skeptical engineering audiences is more important than reach (HashiCorp, Datadog, Vercel-style).

### Option 4 — Report directly to CEO or CTO

**Used by.** 20.3% in 2024, up from 14.1% in 2023 (SlashData).

**Strengths.**
- Strategic autonomy. DevRel can serve product, marketing, sales, and engineering without being captured by any one of them.
- Signals organisational seriousness; attracts senior talent.
- Removes the structural conflicts above.

**Weaknesses.**
- Demands a strong VP/Head of DevRel who can operate at peer level with other VPs.
- Risk of "founder hobby" if the CEO is personally interested but the function lacks operational rigour.
- Easier to lose in restructures, since DevRel is not a settled column on the org chart.

**Best fit.** Mid-stage developer-product companies, especially after a Series B/C, where the function has proved out and needs structural independence to scale.

### Option 5 — Standalone CDRO / Chief Developer Officer

**Used by.** Rare; mostly developer-product companies whose entire business depends on developer adoption.

**Strengths.**
- Maximum signal. DevRel is a peer to CMO, CTO, CPO.
- Owns its own metrics framework, budget, and headcount.
- Career attractor for senior DevRel leaders who have plateaued elsewhere.

**Weaknesses.**
- Only works if the CEO genuinely treats the CDRO as a peer.
- Otherwise becomes a fancy title without authority.

## Sizing benchmarks

Headcount distribution from State of Developer Relations 2024:

| Team size | Share |
|---|---|
| 1 person | 18.2% (down from 22% in 2023) |
| 2–5 people | 35.2% |
| 6–15 people | ~22% |
| 16–50 people | ~12% |
| 51–100 people | ~8% |
| 100+ people | 4.6% (up from 3% in 2023) |

The lone-evangelist model is fading; even small DevRel functions now usually pair an advocate with a community manager or developer educator. The 100+ teams are concentrated at the hyperscalers (AWS, Microsoft, Google) and at category-leading developer-product companies (GitHub, MongoDB, HashiCorp, Twilio, Stripe).

Growth expectations (2024 SlashData):

- **37%** of teams expected to grow.
- **35%** expected no change.
- **12%** expected to shrink.

This is materially more volatile than two years prior, reflecting both renewed investment post-2024 and continued correction at companies that over-hired in 2020–2022.

## Hiring sequences that work

The empirically supported sequence (SlashData, Jono Bacon, and field observation):

1. **First hire: a Community Manager**, not a Developer Advocate. Many founder-led companies make the mistake of hiring a visible evangelist first. That person needs an audience and a place to send them. Without community infrastructure, evangelism scatters.
2. **Second hire: a Developer Advocate / Evangelist**. Now you have a community to feed, the advocate produces the content, talks, and demos that bring people in and keep them engaged.
3. **Third hire: a Developer Educator or Technical Writer**. The advocate's content is high-bandwidth, low-recall; durable education and reference docs convert browsers into shippers.
4. **Fourth hire: a Director or Head of DevRel** to make the team coherent across these three functions.

Teams that followed this Community → Evangelist → Director sequence reported roughly **40% higher developer onboarding completion rates** than teams that hired evangelists first (State of DevRel 2024).

After the first four, specialisation drives further hiring:

- A second advocate, specialised by region (e.g. APAC) or by stack (e.g. mobile, AI).
- A Developer Marketing Manager to own launches and distribution.
- A Community Program Manager to operate ambassador/champion programs.
- A Developer Success Engineer to follow up on activation friction.

## Where DevRel intersects with other functions

A useful diagram (mental model, not org chart):

```
                  ┌──────────────────────┐
                  │     DEVELOPERS       │
                  └──────────┬───────────┘
                             │
                  ┌──────────▼───────────┐
                  │   DEVELOPER RELATIONS │
                  └──┬──────┬──────┬─────┘
                     │      │      │
                     ▼      ▼      ▼
                Product  Engineering  Marketing  Sales  Support
                     ▲      ▲      ▲      ▲      ▲
                     └──────┴──────┴──────┴──────┘
                            DEVELOPERS
```

Effective DevRel teams have **structured touch-points** with each of these:

- **With Product:** Quarterly "voice of developer" review; participation in roadmap meetings; embedded advocates per product area.
- **With Engineering:** Bug triage from community channels; advocate participation in API design reviews.
- **With Marketing:** Joint launch planning; shared content calendar; coordinated event presence.
- **With Sales:** Lead pass-through process for community members who become enterprise prospects; co-presenting at events.
- **With Support:** Routing rules for community questions; shared knowledge base contributions.

## Anti-patterns

- **"DevRel is marketing."** If every meeting is about pipeline, the team will produce marketing and lose developer trust.
- **"DevRel reports to whoever has open headcount."** A common origin story that becomes structural baggage.
- **"DevRel is the bug triage team."** A symptom of unclear inbound expectations; over time degrades into community support without the staffing for it.
- **"DevRel sets its own goals without anyone's input."** Autonomy is not the same as isolation; goals need to be co-signed by Product and Marketing or the team becomes irrelevant to the business.
- **"DevRel = the founder's stage presence."** The founder is not a substitute for a function. Founder evangelism is fantastic when paired with a team; corrosive when it's the only thing.

## Reporting structure by company maturity (heuristic)

| Stage | Typical structure |
|---|---|
| Seed / pre-PMF | One technical co-founder doing DevRel informally. No reporting line yet. |
| Series A | First DevRel hire, usually a generalist advocate or community manager. Reports to founder or VP Marketing. |
| Series B | 3–8 person team. Often still under Marketing, but adding Product touch-points. |
| Series C | 10–30 person team. Often restructured to report directly to CEO/CTO or to a VP of DevRel/DX. |
| Late stage / public | 30–200 person team with sub-functions: advocacy, education, community, programs, marketing. Led by a VP or SVP. |
| Hyperscaler | 200–1000+ across multiple business units, each with its own DevRel lead. |

## Primary sources

- SlashData, *State of Developer Relations* 2023, 2024.
- Jono Bacon, "DevRel Jobs" (jonobacon.com, 2023).
- Ted Neward, "Where DevRel Fits" (newardassociates.com, 2023).
- Phil Leggetter, "Developer Relations Strategy and Team Sequencing" (leggetter.co.uk).
- Mary Thengvall, *The Business Value of Developer Relations*.