# Building a Career Ladder for Your DevRel Team

A practical guide. If you've read [`./career-ladders.md`](career-ladders.md) (the synthesis) and [`./career-ladders-by-company.md`](career-ladders-by-company.md) (the references), this file is the operational how-to.

## When to write one

The question every founder or DevRel lead eventually faces: *do I need a formal career ladder, or am I overengineering this?*

A heuristic. You need a ladder when **any of these** are true:

- You have more than three DevRel team members.
- A team member has asked, in their last two 1:1s, what they need to do for the next promotion.
- You are hiring "Senior Developer Advocates" and your job posting reads the same as your "Developer Advocate" posting.
- A peer manager in product or marketing has asked you what level your senior person operates at relative to engineering.
- Someone resigned in part because they couldn't see a path forward.
- You are about to do a compensation review and have nothing to anchor decisions to.

You probably do **not** need a formal ladder when:

- You are the founder or first DevRel hire at a pre-Series-A company.
- Your team is two people and you talk every day.
- You expect the team to triple in the next six months — in which case write a *draft* ladder you'll iterate aggressively.

The Mary Thengvall observation: small functional teams led by a caring manager can survive without a formal ladder for the first few years; ladders become essential as the team scales beyond a few individuals.

## The architecture: rows and columns

Every DevRel ladder, whatever its surface form, decomposes into a two-dimensional matrix:

```
                  Column 1     Column 2     Column 3     Column N
                  (Level 1)    (Level 2)    (Level 3)    (Level N)
   ┌────────────┬─────────────┬─────────────┬─────────────┬────────────┐
   │ Row 1      │             │             │             │            │
   │ (Function) │   cell      │   cell      │   cell      │   cell     │
   ├────────────┼─────────────┼─────────────┼─────────────┼────────────┤
   │ Row 2      │   cell      │   cell      │   cell      │   cell     │
   ├────────────┼─────────────┼─────────────┼─────────────┼────────────┤
   │ Row 3      │   cell      │   cell      │   cell      │   cell     │
   └────────────┴─────────────┴─────────────┴─────────────┴────────────┘
```

The two design decisions are: **how many columns** and **what rows**. The cells are filled in last.

### Choosing the number of columns

Adam Fitzgerald's empirical rule, from running DevRel at Amazon and HashiCorp:

| Team size | Recommended columns |
|---|---|
| 1–5 people | 3 columns (Developer Advocate / Senior / Leadership) |
| 5–15 people | 4 columns + branching by job family |
| 15–50 people | 5–6 columns + 2–3 job families |
| 50+ people | 6+ columns; HRBP guidance; align to company-wide leveling |

The constraint that determines what you can usefully describe is **your ability to discriminate between adjacent levels**. If you genuinely cannot articulate the difference between Senior and Staff in your context, don't add Staff — you'll have a ghost level that confuses people.

A second, often forgotten constraint: **compensation banding**. If you have salary band data for, say, 4 distinct DevRel levels but not 6, your ladder should match. Salary bands and ladder columns must align, or compensation conversations become farcical.

### Choosing the rows

Most public DevRel ladders use 5–8 rows. The canonical structure pulls from the four axes covered in [`./career-ladders.md`](career-ladders.md):

1. **Technical expertise** (depth of product / platform knowledge).
2. **Output / execution** (what the practitioner ships).
3. **Communication / storytelling** (external voice).
4. **Internal influence / ambassadorship** (representing developers to the company).
5. **Mentorship and team uplift** (scope beyond self).
6. **Strategic impact** (where seniority matters most).

For a small team you can collapse these into 4–5 rows; for a larger team you may want to split internal-influence into separate inbound/outbound rows, or split execution into content/code/events.

A useful starting template for a small team (Fitzgerald's published sample):

| Row | What it covers |
|---|---|
| Technical expertise (general + specific) | Knowledge of product portfolio and competitive landscape |
| Outbound interaction (talks, content, social) | External communication output and quality |
| Inbound interaction (community, feedback) | Engagement with developers; feedback loops to product |
| Customer focus | Understanding and serving developer needs |
| Execution | Reliability of delivery; scope of ownership |

For a larger team you may also want rows for:

- Storytelling / narrative quality (separate from raw content output).
- Mentorship and team uplift.
- Cross-functional collaboration (specifically with product, sales, marketing).
- Setting direction / strategic impact.
- Programmatic ownership (for community managers / program managers).

### Writing cell language

The single biggest determinant of whether your ladder works in practice. Three principles:

1. **Be specific about behaviour, not activity.** Activities lead to checkboxes ("I ran X meetups"). Behaviours describe a kind of practitioner ("Independently identifies and supports community emergence in new geographies"). Bear Douglas's framing at Slack is the canonical example.
2. **Use objective language wherever possible.** Avoid "great" and "excellent." Use measurable language: "Demonstrates technical depth such that customer architects engage at peer level," not "Strong technical skills."
3. **Imply mastery cascades upward.** Cell content at Level N should imply mastery of Level N−1. Don't repeat the same items at every level; let each level inherit the level below and add new expectations.

A useful exercise: read the cells across a row from left to right. The trajectory should be unmistakable — a Level 1 entry should sound like the same person at an earlier stage, not a different person doing different work.

### Example cell content (technical expertise row)

For a hypothetical 4-column matrix:

| Developer Advocate | Senior | Staff | Principal |
|---|---|---|---|
| Maintains working knowledge of the core product surface. Reliably answers basic technical questions in community. | Maintains comprehensive knowledge of the complete product portfolio and how features apply to key use cases. Customer technical leads regard them as a peer. | Articulates long-term product and company technical vision in ways that resonate with customer architects. Trusted by engineering as a source of customer-grounded technical input on roadmap. | Sets industry conversation about the technology category. Provides expert guidance to executive team on capturing developer mindshare. Engineering teams seek their guidance on major architectural directions. |

Each step is a behavioural change, not an activity change. The progression — from working knowledge to comprehensive knowledge to long-term vision to industry-setting — captures scope expansion without referring to specific activities.

## Where to start

You have two paths.

### Path A: Adapt an existing public ladder

The fastest path. Pick whichever public ladder is closest to your context:

- **Small generalist team (< 5):** Fitzgerald's published 3-column template.
- **Mid-size team (5–15), three pillars:** Camunda's path.
- **DevEx-flavoured team in a PLG company:** Drasner's DevEx ladder.
- **Multiple job families:** GitLab's structure.
- **Larger org needing many levels:** HashiCorp's 6-column matrix.

Take the structure. Edit cells to match your company's principles, your product, your goals. The output is a v1 you can ship in a week.

### Path B: Co-design with the team

Slower but more durable. Convene the team. Read existing ladders. Then:

1. Brainstorm the rows together (what dimensions do we want to be evaluated on?).
2. Brainstorm the columns (how many levels do we have? how do we describe them?).
3. Have each team member write their own cells for their current level, then exchange and refine.
4. Have the manager write the cells for the level above each team member.
5. Reconcile. Iterate.

This process surfaces hidden tensions early and produces a ladder with shared ownership. It typically takes 4–8 weeks.

## Connect it to compensation

A ladder without compensation banding is decorative. Before you ship it, work with HR (or your founders) to establish:

- **Salary range per level** — base + equity + bonus where applicable.
- **Sub-banding within levels** — Camunda's junior/mid/senior salary banding within each DR stage works well for stretching a small number of explicit levels.
- **Geographic adjustments** — if you have global team members.
- **Re-banding cadence** — how often the salary ranges are reviewed.

If you cannot get HR to commit to bands, your ladder is at risk: a manager who promotes someone only to discover the compensation doesn't move is in a bad position. The ladder must be backed by money.

## Connect it to promotion

The hard step: how do people *actually* get promoted using the ladder?

Three components:

### 1. Difference documents (Fitzgerald's most-quoted advice)

After the ladder is written, write a **difference doc** for each adjacent pair of levels: "what changes between Developer Advocate and Senior Developer Advocate?" The difference doc is roughly half a page per pair. It becomes:

- The outline of the promo justification template.
- The outline of a development plan for someone aiming at the next level.
- The substance of every promotion-readiness 1:1.

A ladder without difference docs is half built. Reserve a week to write them after the ladder ships.

### 2. Promotion readiness criteria

Multiple public ladders agree: people must demonstrate the qualities of the next level *before* promotion, not after. Camunda's standard: "at least 70% of the way toward the next stage" plus demonstrated work at that level.

Establish your own threshold. Common conventions:

- Demonstrated work at the next level for at least 6 months.
- Preponderance of the row criteria at next level showing operationally.
- A sponsor (not the direct manager) who attests to the readiness.

### 3. Promotion cadence

Decide your philosophy. Two extremes:

- **Microsoft-style.** Lots of sub-levels; promotions happen annually or biennially; constant small-step movement.
- **Amazon-style.** Large levels with substantial gaps; promotions every 2–4 years at junior levels, every 4–8 years at senior levels.

DevRel teams typically sit in between. Most public ladders effectively imply 18–36 months between adjacent levels for performers.

Critical: **once promotion criteria are met, deliver the promotion.** Drasner's emphasis: "If you guide employees on this journey, you need to give them the promotion at the end... if that person has earned it on their end."

## Operationalising in 1:1s

The ladder is useless if it never enters the 1:1 conversation. Drasner's 30/90 model is the cleanest operationalisation:

- **Quarterly:** Review the ladder. Read out current-level criteria; self-assess; identify what's progressing toward next level.
- **Monthly:** Set 30/90 plans aligned to next-level gaps. Review last month's progress; celebrate completed items.
- **Every 6–12 months:** Recalibrate. Has the team scaled? Have rows or columns shifted? Update the ladder.

A 30/60/90 variant works too; many practitioners find the 60-day check redundant.

## Keeping it living

Adam Fitzgerald's advice: **don't update more often than annually**, but treat it as a living document — not a static one.

- **Annual review.** Cadence keeper. Bring the team in. Update language where the company has changed. Add a column if you've grown enough to warrant it. Remove a row if a function has migrated to a different team.
- **Out-of-cycle changes.** Only for material structural changes (acquisition, restructure, splitting into multiple teams). Document why and over-communicate.
- **Avoid drift in cell language.** The temptation is to tweak phrases in cells based on the last performance review. Resist — this is how ladders become political. Cell-level changes happen at annual cadence only.

## Common pitfalls

1. **The activity-checklist trap.** Cells say "runs meetups," "writes blog posts." A team member doing the activities still doesn't get promoted because the cells didn't actually capture *what was supposed to change at promotion*. Fix: rewrite as behaviours.
2. **The unread document.** The ladder is written, posted somewhere, never referenced in 1:1s, never discussed at promo time. Fix: operationalise via 30/90s.
3. **The unbacked ladder.** Promotion criteria are clear, but HR hasn't established the salary bands behind them. Fix: get the bands before publishing.
4. **The fictitious levels.** Levels are written for roles you don't have ("Distinguished Developer Advocate") with cells that aren't grounded in real differentiation. Fix: don't write levels you can't fill in concretely.
5. **The goalpost shift.** Levels are revised mid-cycle in ways that move criteria for someone who was on track. Even when justified, this is corrosive. Fix: revisions happen at annual cadence; in-flight cases follow the version they started under.
6. **The Peter Principle.** People get promoted because they've been at the current level "long enough." Fix: Thengvall's criterion — promotion requires demonstrating next-level performance, not just tenure.
7. **The marketing-comp trap.** Ladder is co-located with marketing. Marketing comp bands cap below engineering at IC4+. DevRel team members earning less than engineering peers at the same level. Fix: negotiate engineering parity, or move the reporting line. See [`./org-structures.md`](org-structures.md).
8. **The single-track trap.** Your team has a Community Manager, an Educator, an Advocate, and a Program Manager — but the ladder is written only for advocates. Three of four people can't see themselves in it. Fix: GitLab-style multiple job families.

## Sharing it publicly

Should the ladder be public?

The argument for: **it's a recruiting advantage.** Bear Douglas, Mary Thengvall, Sarah Drasner, and the GitLab team have all argued that public ladders attract senior talent. Candidates can self-assess. Companies that publish are signalling seriousness.

The argument against: published ladders are easily compared, sometimes unfavourably. A weaker ladder published is worse than a strong ladder internal.

A useful middle path: **publish the structure (rows, columns, level names, salary banding ranges)**, but keep the per-cell prose internal until you've iterated on it for two annual cycles. This is roughly what Camunda did (the column structure is public, the full prose is in a linked Google Sheet that requires effort to read).

## Templates and starting points

Three workable starting templates:

### Template A — Small team (3 columns × 5 rows)

Based on Fitzgerald's published example. Levels: **Developer Advocate / Senior / Director**. Rows: Technical Expertise, Outbound Interaction, Inbound Interaction, Customer Focus, Execution.

Best for: 1–5 person teams.

### Template B — Mid-size with attribute structure (4 columns × 4 areas × 12 attributes)

Based on Camunda. Levels: **DR1 / DR2 / DR3 / DR4** with junior/mid/senior banding within each. Areas: Functional Skills, Delivery, Teamwork, Leadership. Attributes: Product Knowledge, Feedback, Implementation, Transparency, Communication, Collaboration, Mentoring, Empathy, Influence.

Best for: 5–15 person teams; teams spanning advocacy + experience + community.

### Template C — Multi-family with management track

Based on GitLab. Job families: **Developer Advocate**, **Developer Evangelist (Community Engagement)**, **DevRel Program Manager**, **Contributor Success Engineer**. Each family has 4–5 IC levels plus a manager track to Director / VP.

Best for: 15+ person teams; companies with multiple distinct DevRel functions.

### Template D — Six-column with company-principle column themes

Based on HashiCorp (Adam Fitzgerald). Levels: **Learn / Coordinate / Execute / Own / Evolve / Lead**. Rows: Technical Expertise (general + specific), Storytelling, Ambassadorship, Effective Communication, Growth Mindset, Customer Focus, Driving Outcomes, Setting Direction.

Best for: Larger, mature DevRel orgs where you want company-principle alignment.

## Final checklist

Before shipping a ladder, confirm:

- [ ] Number of columns matches our discrimination ability and salary bands.
- [ ] Rows cover technical, output, communication, scope dimensions.
- [ ] Cells describe behaviours, not activities.
- [ ] Mastery cascades upward — each cell implies mastery of the cell to its left.
- [ ] Salary bands per column are defined and reviewed.
- [ ] Difference documents exist between adjacent levels.
- [ ] Promotion readiness criteria are documented (e.g., "demonstrated at next level for 6 months").
- [ ] 1:1 cadence operationalises the ladder (30/90 or equivalent).
- [ ] Management track exists in parallel to the IC track.
- [ ] Multiple job families are represented if the team is large enough to warrant.
- [ ] The team has read and feels represented by the ladder.
- [ ] Public release strategy is decided (full / partial / private).
- [ ] Annual review cadence is in the calendar.

A ladder that ships with these in place will work.

## See also

- [`./career-ladders.md`](career-ladders.md) — Synthesis of public examples.
- [`./career-ladders-by-company.md`](career-ladders-by-company.md) — Slack, Camunda, Drasner, GitLab, HashiCorp in detail.
- [`./hiring-and-career.md`](hiring-and-career.md) — How hiring uses the ladder.
- [`./org-structures.md`](org-structures.md) — Where DevRel reports affects compensation parity.
- [`./job-titles-and-roles.md`](job-titles-and-roles.md) — Title vocabulary.
- [`../10-tactics/anti-patterns.md`](../10-tactics/anti-patterns.md) — Several apply to ladders specifically.

## Primary sources

- Adam Fitzgerald, *Practical Career Matrices for DevRel*, DevRelCon 2021 (developerrelations.com).
- Bear Douglas, "Defining a career path for Developer Relations," Slack Engineering, 2019.
- Mary Thengvall, "The Camunda Developer Relations Career Path," 2020.
- Sarah Drasner, "The Importance of Career Laddering," CSS-Tricks, April 2021.
- GitLab Handbook, job-description-library.
- John Coghlan, *GitLab's DevRel career ladder*, DevRelCon.