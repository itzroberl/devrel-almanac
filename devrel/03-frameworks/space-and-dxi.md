# SPACE, DXI, and DX Core 4: Developer Experience Frameworks

While AAARRRP, Orbit, and the Four Pillars define how DevRel teams operate, three additional frameworks define how **developer experience itself** is measured. These were developed primarily for *internal* developer productivity (helping companies measure their own engineers), but have increasingly informed *external* developer-experience work — and therefore inform DevRel.

## SPACE (2021)

The **SPACE framework** was published in 2021 by Nicole Forsgren, Margaret-Anne Storey, Chandra Maddila, Thomas Zimmermann, Brian Houck, and Jenna Butler — a research collaboration between Microsoft Research, GitHub Next, the University of Victoria, and others. It is the most widely cited modern framework for developer productivity.

SPACE stands for five dimensions:

| Letter | Dimension | Example measures |
|---|---|---|
| **S** | Satisfaction and well-being | NPS, burnout surveys, engagement scores |
| **P** | Performance | Code quality, delivery against goals, customer impact |
| **A** | Activity | Commits, PRs merged, deployments |
| **C** | Communication and collaboration | Code review effectiveness, doc reuse, knowledge sharing |
| **E** | Efficiency and flow | Focus time, interruption rate, lead time |

The framework's central claim is that **no single dimension is enough**, and that "productivity" measured along one dimension alone is at best misleading and at worst harmful. Measuring activity alone rewards busy-looking developers; measuring satisfaction alone rewards comfortable teams that ship slowly.

SPACE requires:

- A mix of *perceptual* (survey-based) and *behavioural* (system-derived) measures.
- Measurement at the team level, not the individual level (to avoid micro-management failure modes).
- Triangulation between dimensions — improvements in one should not come at the cost of degradation in another.

**Why it matters for DevRel.** DevRel teams building developer products (internal or external) increasingly use SPACE-derived measurements to assess whether their work is actually making developers more productive, not just more engaged with the product.

## DXI — Developer Experience Index (2023+)

The **Developer Experience Index (DXI)** is a composite metric developed by Abi Noda's team at getdx.com (DX), based on a research dataset spanning over 800 organisations and 4 million observations. It builds on SPACE but distils it into a more actionable composite index.

The DXI is calculated from 14 standardised survey items covering areas including:

- Code quality and codebase health.
- Onboarding friction.
- Build, test, and CI/CD speed.
- Focus time and interruption load.
- Documentation quality.
- Tooling adequacy.
- Deployment confidence.

Each item is scored on a Likert scale; the composite is a 0–100 number. The headline empirical claim, reported by DX from its dataset: **a one-point improvement in DXI score correlates with roughly 13 minutes of developer time saved per developer per week, or about 10 hours per year per developer.**

For a 500-engineer organisation, a 5-point DXI improvement therefore translates to roughly 25,000 hours of recovered engineering time annually. The compounding business case is what made the DXI rapidly influential.

**Why it matters for DevRel.** External developer products live or die on developer experience. The DXI provides a measurement vocabulary that translates DevEx improvements into financial terms executives understand.

## DX Core 4 (2024)

The **DX Core 4** is DX's attempt to unify three previously distinct frameworks into one — combining:

- **DORA metrics** (Deployment Frequency, Lead Time for Changes, Mean Time to Restore, Change Failure Rate) — the four key software delivery metrics from Forsgren's *Accelerate*.
- **SPACE** — the dimensions of productivity.
- **DXI** — the perceptual measurement.

DX Core 4 organises measurement around four balanced dimensions:

1. **Speed** — How fast does the team deliver? (DORA-flavoured.)
2. **Effectiveness** — Are developers able to do their best work? (DXI-flavoured.)
3. **Quality** — Are we delivering reliably? (Change failure rate, defect rate.)
4. **Impact** — Is the work moving the business? (Customer-facing outcomes.)

The framework is designed to be the unifying measurement layer for engineering organisations and is increasingly adopted by DevEx and platform-engineering teams.

## How these relate to DevRel

For external developer-product DevRel teams, these frameworks have three implications:

1. **They give DevRel a productivity vocabulary that pairs with strategy frameworks.** AAARRRP says "we want to drive Activation." DXI says "Activation depends on TTFHW, which depends on docs quality, which is measurable." The two compose.
2. **They legitimise investment in docs, SDKs, and onboarding as productivity work, not marketing.** If your product saves customer developers measurable hours per week, you have a story that survives the budget conversation.
3. **They surface the internal/external DevEx distinction.** DevRel does not own internal-engineering productivity (that's platform engineering / DPE). DevRel *does* own the experience external developers have using the product. Knowing which conversation you are in is essential.

## Survey design matters

All three frameworks rely heavily on survey-based measurement. A few hard-won lessons from teams who have implemented them well:

- **Run the same surveys every quarter.** Year-over-year trend matters more than the absolute number.
- **Aggregate to team or product area, never to individual developer.** Individual-level measurement turns into surveillance.
- **Pair perception data with behavioural data.** A team that reports high satisfaction but shows declining shipping is in trouble; a team that reports low satisfaction but ships steadily may be over-engineered.
- **Respond visibly.** Surveys that produce no action degrade response rate within two cycles.

## When these frameworks are *not* useful

- For very small teams (under 20 developers). The instrumentation overhead exceeds the value.
- For teams where the productivity bottleneck is upstream (poor product strategy, organisational politics). No framework will fix that.
- As a hiring or performance-review lens for individual contributors. Designed for team-level use.

## Primary sources

- Forsgren, Storey, Maddila, Zimmermann, Houck, Butler, "The SPACE of Developer Productivity," *Communications of the ACM*, 2021.
- Abi Noda et al., *The State of Developer Experience* report (DX / getdx.com, multiple editions).
- *Accelerate* (Forsgren, Humble, Kim), 2018 — the canonical DORA reference.
- DX, "DX Core 4 explained," getdx.com, 2024.
- Atlassian, *State of Developer Experience Report 2025*.

## See also

- [`./aaarrrp.md`](aaarrrp.md)
- [`../11-trends/devex-movement.md`](../11-trends/devex-movement.md)
- [`../04-metrics/metrics-overview.md`](../04-metrics/metrics-overview.md)