# DevRel Career Ladders

A career ladder is an internal document that describes the expectations of a staff member at any given stage of their career — what's needed to perform well at this level, and what's required to be considered for the next. For most engineering disciplines, ladders are standard infrastructure. For Developer Relations, they remain comparatively rare: the **2021 State of Developer Relations** survey found only **34% of DevRel respondents had a defined career path** in their organisation. As of 2024–2026 the share is growing, but DevRel ladders are still less mature than their engineering counterparts.

This file is the synthesis: the canonical axes, the level archetypes, and what's common versus distinctive across the publicly documented examples. For per-company specifics see [`./career-ladders-by-company.md`](career-ladders-by-company.md). For practical guidance on writing one for your team see [`./building-a-career-ladder.md`](building-a-career-ladder.md).

## Why DevRel needs ladders

Sarah Drasner, who open-sourced her DevEx ladders at [career-ladders.dev](https://career-ladders.dev), made the argument cleanly: ambiguity about expectations and compensation is one of the leading causes of demoralisation, burnout, and attrition. Engineers usually know where they stand; DevRel professionals frequently do not.

Three concrete failure modes ladders address:

1. **Title inflation and compression.** Without ladders it is common for job postings to use "Senior Developer Advocate" and "Associate Developer Advocate" almost interchangeably, with little structural difference. Candidates and incumbents cannot tell what is expected.
2. **No path beyond Senior.** Many DevRel professionals hit a Senior title and then have no visible next step short of management. A real ladder defines Staff, Principal, and Distinguished as legitimate IC destinations.
3. **Cross-functional opacity.** When DevRel sits inside Marketing or Engineering, peers in adjacent functions cannot calibrate seniority of DevRel members without explicit levels.

The strongest single argument for documenting a ladder publicly: **it is a recruiting advantage**. Mary Thengvall, who introduced the Camunda DevRel career path in 2020, has observed that companies with public ladders consistently outperform similar-stage companies without them in attracting senior DevRel talent.

## "Path" vs "ladder" vs "matrix"

A semantic note worth getting out of the way. Different practitioners prefer different terms:

- **Career path** (Mary Thengvall, Bear Douglas / Slack). Emphasises journey; everyone can advance; no competition. *A journey, not a race.*
- **Career ladder** (Sarah Drasner, common engineering usage). Single-direction climb with explicit rungs.
- **Career matrix** (Adam Fitzgerald, HashiCorp / formerly Amazon). A two-dimensional grid: rows are job functions; columns are levels.

The terms are functionally interchangeable in practice. The matrix framing is operationally the most useful — it forces explicit description of each cell — but it can read as cold to junior practitioners. Most public examples (Slack, Camunda, Drasner, GitLab) ultimately ship the same thing: a table of levels × responsibilities with prose descriptions in each cell.

## The canonical axes

Across every public DevRel ladder examined for this almanac, four axes recur. Different companies weight them differently, but the underlying vocabulary is shared.

### 1. Technical depth and expertise

How deep is the practitioner's knowledge of the product, the platform, and the surrounding technology landscape? Can they hold their own with senior engineers in customer organisations? Do they understand the product portfolio, the architectural choices, the competitive landscape?

- **Slack**'s ladder calls this **"technical quality."**
- **Camunda**'s ladder names it **"Functional Skills"** with sub-attributes Product Knowledge and Feedback.
- **HashiCorp**'s career matrix (per Adam Fitzgerald) calls it **"technical expertise"**, with general and specific sub-rows.
- **Drasner**'s DevEx ladder embeds it across multiple bullet points per level.

### 2. Execution / delivery / output

What gets shipped? Can the practitioner reliably produce content, demos, talks, integrations, sample apps, and the rest of the DevRel output catalogue? Can they own multi-quarter initiatives end-to-end?

- **Slack**: **"execution"** is one of three top-level components.
- **Camunda**: **"Delivery"** with sub-attributes Implementation and Transparency.
- **HashiCorp**: **"driving outcomes"** plus discipline-specific rows for outbound interaction, inbound interaction, etc.
- **Drasner**: spread across role-specific bullets.

### 3. Collaboration, communication, and ambassadorship

How does the practitioner work with internal teams (product, engineering, marketing, sales) and represent the company externally? Are they a credible voice? Do they build effective feedback loops?

- **Slack**: **"collaboration."**
- **Camunda**: **"Teamwork"** with Communication and Collaboration sub-attributes.
- **HashiCorp**: **"effective communication"**, **"storytelling"**, and **"ambassadorship"** as three separate rows.
- **Drasner**: extensively embedded in level descriptions ("Adapts their communication style to most effectively communicate with the target audience").

### 4. Scope and leadership

How far does the practitioner's impact extend — themselves, their immediate team, multiple teams, the company, the industry? Do they mentor? Do they set direction?

- **Slack**: implicit in level descriptions; staff and above expected to "level the team up."
- **Camunda**: **"Leadership"** with Mentoring, Empathy, and Influence sub-attributes.
- **HashiCorp**: explicit column theme — *Learn → Coordinate → Execute → Own → Evolve → Lead* across six levels.
- **Drasner**: the canonical framing. *Senior = best you; Staff = expand beyond yourself; Principal = systems that scale beyond yourself.*

## The level archetypes

Despite different naming, every ladder converges on a small set of archetypes. Here is the synthesis, with the most common cross-company correspondences.

### Archetype 1 — New / Associate / Apprentice

**Other names.** Developer Advocate Apprentice, Junior Developer Advocate, DevRel Associate, Developer Advocate I, Slack new-grad level, Camunda DR1, HashiCorp "Learn" level, Drasner DX Engineer I, Oracle ACE Apprentice.

**Hallmark.** Learns the role. Executes work designed by others. Builds technical credibility. Typically 0–2 years of professional experience or recent graduates.

**Examples of work.**
- Runs a demo someone else built.
- Writes blog posts based on existing material.
- Answers community questions on monitored forums.
- Submits CFP talks and delivers them at smaller events.
- Files bug reports on the company's product.

### Archetype 2 — Developer Advocate / Intermediate

**Other names.** Developer Advocate (canonical), Developer Advocate II, Camunda DR2, HashiCorp "Coordinate" / "Execute", Drasner DX Engineer II, Oracle ACE Associate.

**Hallmark.** Owns a content stream and a community segment. Builds demos. Works with minimal supervision. Typically 2–5 years experience.

**Examples of work.**
- Builds the demo (rather than just running one).
- Writes original technical content at scale.
- Speaks at multiple industry events per year.
- Engages community in real time (Discord, forums).
- Contributes meaningful PRs to OSS or sample code.

### Archetype 3 — Senior

**Other names.** Senior Developer Advocate, Senior Developer Evangelist, Camunda DR3, HashiCorp "Own", Drasner Senior DX Engineer, Oracle ACE Pro.

**Hallmark.** Owns a domain or substantial program. Becomes the go-to person for one or more products/programs. Proactively engages — defines quarterly goals, brings new ideas, mentors juniors. Drasner's framing: *the best you can be as an individual contributor.* Typically 5–8 years experience.

**Examples of work.**
- Designs the demo (rather than building one to spec).
- Owns a content category end-to-end (e.g. "all AI/ML developer content").
- Represents company in analyst briefings and major executive engagements.
- Holds positions of influence in OSS projects (maintainer status, TAG leadership).
- Mentors 1–2 junior advocates.

Many DevRel professionals remain at Senior for the rest of their careers. Mary Thengvall's Camunda framing is explicit: "There is no expectation or requirement that they advance to a Principal role."

### Archetype 4 — Staff

**Other names.** Staff Developer Advocate, HashiCorp "Evolve", Drasner Staff DX Engineer. Sometimes folded into Senior at smaller companies; sometimes split into Senior Staff at larger ones.

**Hallmark.** Scope expands beyond self to the team. *"The majority of one's time is spent scaling their own skills to help others"* (Drasner). Drives cross-team coordination, defines next phases of programs, mentors at scale. Typically 8–12 years experience.

**Examples of work.**
- Coaches others on designing demos, building content, running programs.
- Influences content strategy across DevRel, marketing, and the broader company.
- Coordinates cross-team initiatives requiring multi-stakeholder alignment.
- Speaks as keynote at large industry events.
- Designs sales enablement training that scales across the global sales org.

### Archetype 5 — Principal

**Other names.** Principal Developer Advocate, HashiCorp "Lead", Drasner Principal DX Engineer, Oracle ACE Director.

**Hallmark.** Scope expands beyond the team to industry-level influence. Helps others where they are, not where the principal is. Sets direction for an entire function or technology area. Typically 12+ years experience.

**Examples of work.**
- Drives industry conversations about modern practices (Drasner: "Helping others be the best they can be, removing themselves and meeting others where they are").
- Partners with Engineering on roadmap input for multiple feature areas.
- Leads analyst and executive engagements representing the company.
- Sets strategy for the entire DevRel function or a major sub-function.
- Built recognised public works (books, courses, OSS projects) attracting community to the company.

### Archetype 6 — Distinguished / Fellow

**Other names.** Distinguished DX Engineer (Drasner), Distinguished Developer Advocate (rare), Microsoft Technical Fellow equivalent.

**Hallmark.** Industry-shaping; effectively a public figure in their domain (Kelsey Hightower is the canonical example). Sets strategy that shapes the company's market position. Typically 15+ years experience and a substantial public record.

Few DevRel ladders include this level; those that do (Sarah Drasner's, some at hyperscalers) treat it as exceptional.

### Archetype 7 — People-management track

Parallel to the IC ladder, every well-formed DevRel ladder includes a management track:

| IC level | Management equivalent |
|---|---|
| Senior | Manager (3–7 reports, one team) |
| Staff | Senior Manager (2–3 teams, ~10–20 people) |
| Principal | Director (full sub-org, 20–60 people) |
| (Principal/Distinguished) | Senior Director / VP |
| (Distinguished) | SVP / CDRO / C-suite |

GitLab's public ladder is explicit about this: there is a *Manager, Developer Relations Programs* role, a *Director, Developer Relations*, a *Senior Director*, a *VP Developer Relations and Community*, and finally a *VP Strategy & Developer Relations* role. Camunda's earlier ladder stops at DR4 / Principal for the IC track and treats management as a separate (less documented) discipline.

The IC track and the management track are not the same ladder. Some companies (especially the smaller ones) treat the role of Senior or Staff DevRel as a "player-coach" — managing two or three people while also producing — but at scale the separation is enforced.

## Comparison matrix across the four public ladders

| | **Slack** (Bear Douglas, 2019) | **Camunda** (Mary Thengvall, 2020) | **DevEx Ladder** (Sarah Drasner) | **GitLab** (handbook, current) |
|---|---|---|---|---|
| **Public location** | slack.engineering, with linked spreadsheet | marythengvall.com + Google Sheet | career-ladders.dev/devex | handbook.gitlab.com job-description-library |
| **Levels** | 4 (new grad, mid, senior, staff) | 4 (DR1–DR4), each with junior/mid/senior sub-bands | 6 (I, II, Senior, Staff, Principal, Distinguished) + Tech Lead | 4 IC (DA, Senior, Staff, Principal) + 4 management (Manager, Director, Sr Dir, VP) |
| **Top-level axes** | Technical quality, Collaboration, Execution | Functional skills, Delivery, Teamwork, Leadership | Multiple bullets per level (less explicit axes) | Implied from job-description bullets per level |
| **Sub-attributes** | Implied within axes | 12 named attributes (Product Knowledge, Feedback, Implementation, Transparency, Communication, Collaboration, Mentoring, Empathy, Influence) | Embedded in level descriptions | Embedded in JD prose |
| **Experience guidance** | Implicit | Implicit, with junior/mid/senior bands per stage | Explicit (2/4/6/8/10/12 years per level) | Years explicit per JD (e.g. 4–5 yrs for Staff) |
| **Specialty tracks** | Generalist (12-person team) | Three pillars (Advocacy, Experience, Community) sharing one path | Single path with Tech Lead overlay | Multiple distinct families (Advocate, Evangelist, Program Manager, Contributor Success Engineer) |
| **Management track** | Implied separate, not shown | Implied separate, not shown | Tech Lead notes ("can be at any level") | Explicit, integrated (Manager → Director → VP) |
| **Distinctive choice** | "Behaviors not activities" — describes seniority abstractly to avoid prescribing tasks | Adds *complexity* dimension (linear / structural / foundational topics) | Each level has a guiding mantra ("the best you can be" / "scaling your own skills" / "helping others where they are") | Maps to a broader marketing/eng ladder; many distinct DevRel job families |

The lesson from the matrix is that **the four canonical public ladders agree on the underlying structure** — four to six levels, with axes covering technical depth, execution, collaboration, and scope — but **diverge in how prescriptive they are about activities**. Slack is the most behavioural ("don't write a checklist"); Camunda is the most attribute-driven; GitLab is the most prescriptive per JD; Drasner's is the most mantra-driven.

## What's common

Across every public ladder, several things recur:

1. **The shape of progression is roughly four to six levels** on the IC track, mapping to four to five management levels above.
2. **Scope is the primary axis** of seniority. The canonical Drasner framing — yourself → your team → systems beyond yourself — appears (sometimes in different language) in every ladder.
3. **Technical credibility is required at every level.** No public DevRel ladder treats Developer Advocate as a marketing role without technical depth. Slack requires "technical quality" from new grads upward; Camunda expects all DRs to "relate to community on a deep technical level."
4. **External influence is expected at Senior and above.** Speaking at industry events, OSS contribution, content with reach. The expectation grows monotonically with level.
5. **Mentorship and team-uplevelling enter at Senior or Staff** and become primary at Principal. *"If you are technically brilliant but you never mentor anyone around you, you are not becoming more senior in the organization"* (Slack).
6. **Internal advocacy matters as much as external.** Slack's framing: "If you're a great external communicator but you can't get anything shipped for developers because you have no credibility with the product team, you aren't becoming more senior." Every public ladder reinforces this.
7. **Ladders are described as guidelines, not checklists.** Both Slack and Camunda are explicit that activities are imprecise descriptors; behaviours and outcomes matter more.

## What's distinctive

The places where companies diverge are often the most useful insights:

### Specialty tracks vs single path

- **Slack** maintains a single path for a 12-person generalist team.
- **Camunda** uses a single path spanning three distinct pillars (Advocacy, Experience, Community). The path is uniform; the day-to-day work differs.
- **GitLab** uses *separate job families*: Developer Advocate, Developer Evangelist (Community Engagement specialty), DevRel Program Manager, plus Contributor Success Engineer. Each has its own levels.
- **HashiCorp** (per Adam Fitzgerald at DevRelCon 2021) splits at mid-size (5–20 people) into separate Advocate / Content / Community Program career matrices.

The pattern: small teams use a single path; teams above ~15 people benefit from specialty tracks; the largest DevRel orgs have multiple job families with parallel ladders.

### Complexity as an explicit dimension

Camunda's career path introduces a separate **complexity** dimension layered on top of levels:

- **Linear complexity** — work that builds on existing structures (DR1 can do).
- **Structural complexity** — work that expands existing programs/projects (DR2+).
- **Foundational complexity** — work scoped from "soup to nuts" (DR3+).

This is Thengvall's most distinctive contribution. It captures the difference between *"can run a demo someone else built"* and *"can design the demo from scratch"* and *"can coach others designing demos"* — without conflating the four levels with specific activities.

### Number of levels — driven by company maturity

Adam Fitzgerald's empirical observation from running DevRel at Amazon and HashiCorp:

- **Small org (< 5 DevRel):** 3 columns (Developer Advocate / Senior / Leadership). Job functions broad.
- **Mid-size (5–20):** 4 columns + multiple job families. Beginning of specialisation.
- **Large org (20–100+):** 6+ columns; multiple job families; people-management track separated from IC.
- **Hyperscaler:** Use the company's existing leveling system (AWS uses L4–L8 SDE bands; Microsoft uses 59–67 SDE bands; Google uses L3–L8 SWE bands). DevRel is graded against engineering, not DevRel-specific.

This last point is critical and often overlooked: at AWS, Microsoft, Google, and Meta, DevRel roles ride on top of the engineering ladder. The titles may be different ("Developer Advocate" rather than "Software Engineer") but the level (and corresponding compensation band) is graded on the same scale.

### Living document vs static

Most public ladders are revised annually at most. Adam Fitzgerald's advice from DevRelCon 2021: *"If you're rewriting it all the time, you're not getting the value out of it. The value you have out of it is you're setting a collection of goalposts that you're helping your team shoot for."* Major revisions more frequently than annual signal a strategy problem, not a ladder problem.

## The Drasner framing — the simplest summary

Sarah Drasner's distillation, from her 2021 CSS-Tricks essay, deserves to be reproduced in full because it is the most-cited single sentence in the DevRel-career-laddering conversation:

> To get to **Senior**, you're the best "you" you can be — you perform your role exceedingly well and you've reached a high potential for your own output.
>
> To get to **Staff**, your focus is really to expand beyond yourself. You start teaching people the great things you learned and help serve their needs.
>
> To get to **Principal**, you're creating systems that scale beyond yourself. You're no longer helping folks be like you — you're helping them *where they are*. A lot of your activities are enabling the success of everyone around you.

This three-sentence model is operationally complete. Every public DevRel ladder is consistent with it.

## What's missing — and what would help

Three honest gaps in the field as of 2026:

1. **No widely accepted compensation bands.** Radford and similar enterprise compensation services do not yet have rich DevRel-specific bands; "advocacy" and "evangelism" data exists but is sparse. Most companies set compensation by mapping DevRel to the engineering ladder informally. The **Developer Relations Foundation** (Linux Foundation, founded August 2025) has standardising career frameworks among its stated goals; this gap is on its roadmap.
2. **Most ladders are still internal.** The public ones (Slack, Camunda, Drasner, GitLab) are exceptions. The 2021 baseline of 34% formal-ladder adoption has improved, but the share with *public* ladders remains small.
3. **AI-era roles aren't yet in most ladders.** Agent Experience Engineer, MCP Engineer, AI Developer Educator — these emerging role types (see [`../16-devrel-in-the-ai-era/agent-experience-ax.md`](../16-devrel-in-the-ai-era/agent-experience-ax.md)) post-date most published ladders.

## See also

- [`./career-ladders-by-company.md`](career-ladders-by-company.md) — Slack, Camunda, GitLab, Drasner DevEx, HashiCorp, Microsoft, Google, AWS, Stripe, Twilio, MongoDB and others in detail.
- [`./building-a-career-ladder.md`](building-a-career-ladder.md) — Practical guide to writing one for your team.
- [`./hiring-and-career.md`](hiring-and-career.md) — How hiring intersects with the ladder.
- [`./job-titles-and-roles.md`](job-titles-and-roles.md) — Title taxonomy.
- [`./org-structures.md`](org-structures.md) — Sizing, reporting, and team composition.

## Primary sources

- Bear Douglas, "Defining a career path for Developer Relations," Slack Engineering blog, 2019 (updated 2022).
- Mary Thengvall, "The Camunda Developer Relations Career Path," marythengvall.com, June 2020.
- Sarah Drasner, *Career Ladders* open-source repository at career-ladders.dev (DevEx ladder).
- Sarah Drasner, "The Importance of Career Laddering," CSS-Tricks, April 2021.
- Adam Fitzgerald, "Practical career matrices for DevRel," DevRelCon 2021 (developerrelations.com).
- GitLab Handbook, Job Description Library (Developer Advocate, Developer Evangelist, DevRel Program Manager, Director of Developer Relations, VP Developer Relations and Community).
- John Coghlan, "GitLab's DevRel career ladder" (talk; devrelacademy.com).
- *State of Developer Relations* report 2021 (stateofdeveloperrelations.com) — 34% formal-ladder baseline.
- *devrel-ladders.com* curated aggregator.