# DevRel Career Ladders by Company

The four canonical publicly documented DevRel career ladders, plus the most widely cited additional frameworks. This file goes into the specifics. For the synthesis across all of them see [`./career-ladders.md`](career-ladders.md).

The four public ladders aggregated at **[devrel-ladders.com](https://www.devrel-ladders.com/)** (curated by Tony Barnes / @tbarn since 2021) are:

1. **Slack** — Bear Douglas (2019).
2. **Camunda** — Mary Thengvall (2020).
3. **DevEx Ladder** — Sarah Drasner (Netlify, now Google).
4. **GitLab** — handbook (continuously maintained).

To this we add:

5. **HashiCorp** — Adam Fitzgerald's DevRelCon 2021 talk *Practical Career Matrices for DevRel*, which described the framework Fitzgerald shipped at both Amazon and HashiCorp.
6. **Hyperscalers (AWS, Microsoft, Google)** — what's publicly known about how these companies grade DevRel on top of their engineering ladders.
7. **Adjacent public references** — IBM (engineering-graded), Red Hat, Oracle ACE program-as-ladder, MongoDB Champions tiers.

---

## 1. Slack — Bear Douglas (2019)

**Author.** Bear Douglas, Developer Advocacy Lead at Slack.

**Published.** March 14, 2019 on slack.engineering, updated January 28, 2022.

**Companion artefact.** Public Google Sheet linked from the post (referenced as "the full path here").

**Team context at time of publication.** 12-person generalist team. "Everyone writes docs, everyone builds tools and sample code, everyone gathers and shares developer feedback, and everyone works on events."

### Levels

Four levels on the IC track:

1. **New Grad** — entry-level, typically a Computer Science new graduate.
2. **Mid-level** — "a few years' experience."
3. **Senior**.
4. **Staff**.

### Three components per level

Every cell in the path is described against three components, adapted from the Slack Engineering path (credited to Ross Harmes, Matt Schweitz, and Lauren Ficklin):

| Component | What it measures |
|---|---|
| **Technical quality** | Depth and accuracy of technical work — docs, code, demos, sample apps |
| **Collaboration** | Internal advocacy, working effectively with product/engineering/marketing, mentoring |
| **Execution** | Shipping work; scope of ownership; quality of delivery |

The three components are meant to encompass "growth in skills, in scope of work, and systems thinking — contextualizing our daily work in the broader landscape of businesses and technology."

### Distinctive philosophy

Douglas was explicit about **describing behaviours, not activities**. Earlier versions of her path had included items like *"running community events, like meetups"* as level criteria; this turned into the trap of "checkboxes" — a team member running the meetup would worry about losing their checkbox toward promotion if they handed it off. Behavioural language solves this: the path describes *what kind of developer relations professional one is at this level*, not *what activities they do*.

The most-quoted lines:

> If you're a great external communicator but you can't get anything shipped for developers because you have no credibility with the product team, you aren't becoming more senior in the organization. The same is true if you're technically brilliant, but you never mentor anyone around you.

### What's distinctive

- **Single generalist path** appropriate for a smaller team.
- **Behavioural framing** that resists checklist-of-activities thinking.
- **Transparency** — a Slack intern was able to accurately infer the levels of teammates after reading the path. Douglas argued this is a feature, not a leak: *"If someone you work with casually can figure out what level you're at, it shouldn't feel risky, like you've been exposed — it's a sign that your team is on the same page about what levels are."*
- **Acknowledgement that DevRel careers come from many directions.** Douglas was explicit that people enter DevRel from engineering, support, ops, customer-facing operations, and many other backgrounds, and that the path is "the jumping off point for conversations with your manager" — not a single linear trajectory.

---

## 2. Camunda — Mary Thengvall (2020)

**Author.** Mary Thengvall, then Director of Developer Relations at Camunda.

**Published.** June 29, 2020 on marythengvall.com.

**Companion artefact.** Public Google Sheet (still hosted at docs.google.com/spreadsheets, linked from the post).

**Team context at time of publication.** Spanned three pillars: Developer Advocacy, Developer Experience, Developer Community — plus supporting roles (Program Manager). Single path served all three.

### Levels

Four stages, each with **junior / mid / senior salary bands within the stage**:

| Stage | Title | Typical |
|---|---|---|
| **DR1** | Associate DevRel Professional | Entry / new to industry |
| **DR2** | DevRel Professional | Most common entry from outside DevRel; 2–5 years experience |
| **DR3** | Senior DevRel Professional | Owns programs; many practitioners remain here for career |
| **DR4** | Principal DevRel Professional | Industry influence required; rare |

Within each stage there is also implicit *junior / mid / senior* compensation banding, providing room for growth without level change. Senior-of-stage means roughly 70% of the way toward the next stage.

### Two dimensions: topics × complexity

Thengvall's framework introduces a separate **complexity** axis that distinguishes what kind of work each level owns. A *topic* is a project, program, or work output; complexity progresses through three levels:

- **Linear complexity.** Builds on existing structures and processes. Anyone on the team can handle. E.g., guesting on a podcast, running a pre-built demo. All DR1+.
- **Structural complexity.** Expands or significantly adds to existing programs. E.g., adding a client SDK for a new language; building out an existing tutorial library. Typically DR2+.
- **Foundational complexity.** Scoped from soup to nuts — ideation through execution. E.g., launching Hacktoberfest participation; designing the Camunda Question Corner. Typically DR3+.

Nathen Harvey's pithy summary of the model (cited approvingly in the original post):

> A Level 1 Dev Advocate can run the demo someone else on the DevRel team built.
> Level 2 can build the demo.
> Level 3 can design the demo.
> Level 4 can coach the person designing, building, or running the demo.

### Twelve attributes across four areas

Each level's expectations are scored across 12 named attributes in four areas:

| Area | Attributes |
|---|---|
| **Functional Skills** | Product Knowledge, Feedback |
| **Delivery** | Implementation, Transparency |
| **Teamwork** | Communication, Collaboration |
| **Leadership** | Mentoring, Empathy, Influence |

Some attributes (Transparency) plateau by DR2. Others (Mentoring, Influence) only become substantive at DR3 and DR4. Critically, Thengvall **does not specify technical skills** ("up to speed on Python 3.7") at any level; instead she requires four behavioural outcomes:

- Relate to community on a deep technical level.
- Provide valuable technical content meeting customer needs.
- Connect technical community members.
- Stay up-to-date on relevant components.

### Distinctive philosophy

- **"Path, not ladder."** Thengvall's deliberate framing: a journey rather than a single-file competitive climb. *"While you're joined by your coworkers, there's no competition... A 'ladder' on the other hand is more difficult to navigate as a group... If someone does pass up other people along the way, there's a good chance someone has gotten hurt or stepped on."*
- **Aim to avoid the Peter Principle.** Thengvall explicitly requires that "employees exhibit the full qualities of the stage they wish to move into before they can apply for promotion." Promotion follows demonstrated performance at the next level, not aspiration.
- **External influence required at DR4.** "Industry thought leader" is *not* enough — DR4s must also be empathetic, must mentor, must give back to the broader DevRel community.
- **No requirement to reach DR4.** Many practitioners remain at DR3 for the rest of their careers and that is explicitly fine.

---

## 3. Sarah Drasner's DevEx Ladder

**Author.** Sarah Drasner, then VP of Developer Experience at Netlify, now Director at Google (Web, Android, iOS, Multiplatform infrastructure).

**Published.** Open-sourced at [career-ladders.dev/devex](https://career-ladders.dev/devex), with companion ladders for Engineering and Documentation. Discussed in detail in Drasner's April 15, 2021 CSS-Tricks essay *The Importance of Career Laddering*.

**Companion artefact.** The full ladder is published on the site; the Engineering ladder and Documentation ladder are siblings.

**Note on naming.** Drasner uses "DX Engineer" rather than "Developer Advocate" because the role hybrid encompasses both engineering work and DevRel work. She is explicit: *"Developer Experience is a hybrid of Engineering and Developer Advocacy/Developer Relations. If you are using these ladders for Advocacy, you may need to remove some Engineering tasks."*

### Levels

Six IC levels plus a Tech Lead overlay:

| Level | Typical experience |
|---|---|
| **DX Engineer I** | 2+ years |
| **DX Engineer II** | 4+ years |
| **Senior DX Engineer** | 6+ years |
| **Staff DX Engineer** | 8+ years |
| **Principal DX Engineer** | 10+ years |
| **Distinguished DX Engineer** | 12+ years |

### The Drasner mantra

The single most-cited framing in the field:

- **Senior.** *"You're the best 'you' you can be — you perform your role exceedingly well and you've reached a high potential for your own output."*
- **Staff.** *"Your focus is really to expand beyond yourself. You start teaching people the great things you learned and help serve their needs."*
- **Principal.** *"You're creating systems that scale beyond yourself. You're no longer helping folks be like you — you're helping them where they are."*

This three-sentence model is operationally complete for senior-level conversations.

### What's distinctive

- **Engineering-hybrid framing.** DX Engineers are expected to write code, file bug reports, build integrations, and contribute to product engineering — not just produce content. This matches the Vercel / Netlify model where Developer Experience reports to engineering or product, not marketing.
- **Tech Lead as cross-cutting overlay.** *"A Tech Lead is responsible for leading a particular project, and responsible for the quality of its technical deliverables. Anyone can be a tech lead at any stage in their career."* Project leadership is decoupled from level.
- **Explicit experience anchors.** The "typically requires a minimum of N years" line is concrete and easy to use in interviews.
- **Each level has a controlling principle.** Senior masters individual contribution; Staff scales own skills to help others; Principal removes themselves and meets others where they are; Distinguished figures out industry-wide unlocks at scale.
- **Companion Documentation ladder.** Drasner also publishes a Docs ladder. The combined trio (Engineering / DevEx / Docs) is unusually comprehensive for an open-source resource.

### The 30/60/90 operationalisation

Drasner pairs the ladder with a quarterly process:

1. **The big picture.** *"Where do you want to be in five years?"*
2. **Career laddering review.** Read out current-level items, self-assess, identify next-level items.
3. **30/90 plan** (she finds 60 less useful). Goals over 30 and 90 days.
4. **Iterate every month.** Review progress; carry over what isn't done; celebrate what is.

The ladder is the substrate; the 30/90 plan is how it gets executed in 1:1s.

---

## 4. GitLab — Handbook Job Description Library

**Authors.** Multiple, since GitLab's handbook is collaboratively maintained. John Coghlan, formerly Manager of Developer Evangelism at GitLab, gave a notable DevRelCon 2021 talk *GitLab's DevRel Career Ladder*.

**Published.** Public, continuously maintained at handbook.gitlab.com/job-description-library (formerly about.gitlab.com).

**Companion artefact.** Each role has its own page, with full job description and performance indicators per level.

### Job families and levels

Unlike Slack and Camunda, GitLab uses **multiple distinct job families** under the DevRel umbrella, each with its own levels.

#### Developer Advocate

| Level | Notable expectations | Approx. years |
|---|---|---|
| **Developer Advocate** | Owns content stream; CFP discipline; meaningful social presence; 1+ year giving talks | 2–5 |
| **Senior Developer Advocate** | Represents GitLab in analyst engagements; technical guidance on analyst briefings; coordinates across many teams; "leader within DevRel and the wider community" | 2–3 years in DevRel + technical background |
| **Staff Developer Advocate** | Influences content strategy across DevRel + Marketing + GitLab; works with executives; positions of influence in OSS (maintainer, TAG leadership); keynote-level events | 4–5 years of demos/content + 6 years enterprise software marketing |
| **Principal Developer Advocate** | Drives thought leadership; partners with Sales on strategic opportunities; influences roadmap across multiple feature areas; technical advisor to customers | 5+ years content + 6 years enterprise software marketing |
| **Director, Developer Advocacy** (people manager) | Owns advocacy team strategy; defines content/distribution; partners with Product/Engineering for community feedback into roadmap | 7+ years leading DevRel + team management experience |

GitLab's three primary performance indicators (consistent across all advocate levels):

- Unique Wider Community Contributors per Month.
- New Unique Web Visitors per Month.
- Impressions per Month (combined from social, events, content).

#### Developer Evangelist (Community Engagement specialty)

A separate job family for community engagement specifically. Responsibilities:

- Responding to questions about GitLab on Hacker News.
- Engaging on Stack Overflow.
- Managing the GitLab Forum.
- Leading community-response situations.

This is GitLab's recognition that community engagement is a distinct skill from content-driven advocacy.

#### Developer Relations Program Manager

A separate family with four levels:

| Level | Differentiator |
|---|---|
| **Associate Program Manager** | Operations, tooling, workflow maintenance |
| **Program Manager** | Executes campaigns and content; community engagement; some strategic input |
| **Senior Program Manager** | Fully owns one or more program strategies and results; 5–7 years experience |
| **Manager, DevRel Programs** | People manager; owns outcomes across all programs; hiring; translates strategy to tactics |

Note: GitLab's Program Manager family **does not** include Staff and Principal levels. The senior IC ceiling is "Senior Program Manager," and the next step is into management.

#### Contributor Success Engineer

Yet another job family — community contributors who help GitLab grow code contributions to the open-core project. Reports up through the same Director of DevRel.

#### Management track

GitLab's management ladder for DevRel:

- Manager, DevRel Programs (or Manager, Developer Advocacy).
- Director, Developer Relations.
- Senior Director, Developer Relations.
- **VP, Developer Relations and Community** (reports to the CMSO — Chief Marketing & Strategy Officer).
- **VP, Strategy & Developer Relations** — an even more senior strategy-cross-functional role.

### What's distinctive

- **Multiple job families.** GitLab's DevRel function is structurally large enough to warrant distinct ladders for advocates, evangelists, program managers, and contributor success engineers. Each is a separate page in the handbook.
- **Public job-description detail.** Every level has a full JD, including responsibilities, requirements, performance indicators, and interview process. This is unusually thorough for a public resource.
- **Performance indicators per role family.** Different families have different metrics (advocates measure community contributors and web visitors; program managers measure new program members and renewal rates).
- **Management track integrates with broader GitLab leveling.** Director and VP roles map to GitLab's standard management ladder, used across marketing and engineering.
- **Two senior leadership variants.** GitLab maintains *both* a "VP Developer Relations and Community" job description *and* a "VP Strategy & Developer Relations" — suggesting that at the largest scale, DevRel splits into operational and strategic leadership.

---

## 5. HashiCorp / Adam Fitzgerald

**Author of public discussion.** Adam Fitzgerald, who led DevRel at Amazon and then at HashiCorp.

**Public artefact.** Adam Fitzgerald, *Practical Career Matrices for DevRel*, DevRelCon 2021 (video and transcript at developerrelations.com). The talk includes a worked sample career matrix as a Google Sheet linked from the Discord channel.

HashiCorp's full internal ladder is not public, but Fitzgerald's talk describes the architecture in unusual detail and is the most explicit reference point for how a large-org DevRel ladder is constructed.

### Structure

Six columns (levels) labeled by **company-principle theme**:

| Level | HashiCorp theme |
|---|---|
| 1 | **Learn** — learning the role and responsibilities |
| 2 | **Coordinate** — coordinating execution |
| 3 | **Execute** — on the hook to deliver |
| 4 | **Own** — owns direction and responsibility |
| 5 | **Evolve** — sets next stage of evolution |
| 6 | **Lead** — overall function direction |

The theme names are HashiCorp-specific (they map to HashiCorp's principles), but the underlying structure — increasing scope per column — is the canonical pattern.

### Eight row themes

For Developer Advocates specifically (other job families use different rows):

| Row | Description |
|---|---|
| **Technical expertise** | General + specific knowledge |
| **Storytelling** | Translating technical capability to relevant narrative |
| **Ambassadorship** | Representing developers to the company and vice versa |
| **Effective communication** | Cross-marketing-org expectation |
| **Growth mindset** | Cross-marketing-org expectation |
| **Customer focus** | Cross-marketing-org expectation |
| **Driving outcomes** | Cross-marketing-org expectation |
| **Setting direction** | Cross-marketing-org expectation |

The first three rows are DevRel-specific. The latter five are shared with the broader marketing org.

### Fitzgerald's company-stage advice

The talk includes explicit guidance on how to size a career matrix to your company stage:

- **< 5-person DevRel team.** 3 columns. Single generalist Developer Advocate matrix. Sample published with the talk has 5 broad job functions (technical expertise, outbound interaction, inbound interaction, customer focus, execution) and 3 levels (Developer Advocate / Senior / Director).
- **5–20 people.** 4 columns. Split into multiple job families (Advocate / Technical Content / Community Program Manager). Separate IC and management columns.
- **20+ people.** *"Don't listen to me. You shouldn't even be talking to me. You're going to be talking to your HR business partner."* HRBPs at this scale have base templates from elsewhere in the company.

### Impact hours as a measurement aid

Fitzgerald advocates for measuring **impact hours** as a way to confirm level placement empirically. The idea: track the actual time-on-target work an advocate is delivering at a given quality bar. Aggregated impact hours tend to bucket people organically into levels. *"If somebody's got impact that is higher than their current level, this is a fantastic signal you should be considering for a promotion."*

This is the only explicitly numerical/objective tool in the public DevRel laddering literature. He used it at both Amazon and HashiCorp.

### Difference documents

Fitzgerald's most-quoted operational advice: after writing the career matrix, *write the difference documents between adjacent levels.* What is the difference between Senior and Staff? What does a Developer Advocate need to develop to become a Senior Developer Advocate? These difference docs become:

- The outline for promotion justifications.
- The outline for personal/professional development plans.
- The basis for 1:1 conversations about progression.

A ladder without difference docs is half built.

---

## 6. Hyperscalers — AWS, Microsoft, Google

These companies have the largest DevRel functions in the industry but mostly **do not publish DevRel-specific ladders**. They use their engineering ladders, with DevRel roles slotted in.

### AWS / Amazon

- **Six SDE bands** (L4 through L8+).
- **DevRel professionals are graded against the SDE ladder.** Title is "Developer Advocate" / "Senior Developer Advocate" / "Principal Developer Advocate" / "Senior Principal Developer Advocate" / "Distinguished Engineer." Compensation bands match SDE I / II / III / Principal / Senior Principal / Distinguished.
- Approximate compensation (per levels.fyi, 2024–2026):

| Level | SDE equivalent | Approximate TC |
|---|---|---|
| L4 | SDE I / Developer Advocate (Entry) | ~$165K |
| L5 | SDE II / Developer Advocate | ~$235K |
| L6 | SDE III / Senior Developer Advocate | ~$300K+ |
| L7 | Principal Developer Advocate | ~$500K+ |
| L8 | Senior Principal | ~$700K+ |
| L10 | Distinguished | Varies |

- **Jeff Barr's promo** to his Chief Evangelist role was, per Fitzgerald's talk, graded against the career matrix Fitzgerald wrote during his Amazon tenure.

### Microsoft / Cloud Advocates

- Microsoft uses 50s–60s level numbers across SDE bands. SDE roles run roughly L59–L67 with sub-levels.
- **Cloud Advocates** are graded against the SDE ladder. Titles are Cloud Advocate / Senior Cloud Advocate / Principal Cloud Advocate / Partner GM Cloud Advocate (e.g., John Papa).
- Microsoft's Cloud Advocate team was substantially restructured during the 2023 layoffs and the level structure has evolved since.

### Google

- Google uses L3 through L8+ for software-engineering roles (with L9+ for the most senior).
- Google's DevRel work is graded against the SWE ladder. Developer Advocates / Developer Programs Engineers are L3 through L7+; senior roles (Sarah Drasner's Director role, for example) move into the management track.
- The Pragmatic Engineer's *Inside Google's Engineering Culture* (September 2025) confirms a dual-track IC/management ladder applies to DevRel.

### Why this matters

The implication for the field: at hyperscaler scale, **DevRel compensation and seniority is driven by the engineering ladder**. DevRel-specific ladders are useful at small and mid-sized companies precisely because at that scale, the engineering ladder doesn't fit DevRel well (engineering doesn't optimise for content production, community engagement, or external influence) and a DevRel-specific framework is necessary. At hyperscaler scale the existing framework absorbs DevRel.

This is consistent with the **State of DevRel 2024** observation that DevRel teams reporting through engineering (rather than marketing) tend to have compensation parity with senior engineers; teams reporting through marketing tend to fall under marketing-comp bands which can be 10–20% below engineering at IC4+ levels.

---

## 7. Adjacent public references

### IBM

IBM uses bands that span ranges (e.g. Band 8, 9, 10 / Principal corresponds to multiple Microsoft levels). DevRel and Developer Advocate roles are graded against IBM's broader band system. Specific public ladder documents are not available.

### Red Hat

Red Hat operates Developer Advocates under their Marketing / Open Source organisation. Levels follow Red Hat's standard banding (Associate / Senior / Principal / Distinguished). Specifics are not public.

### Oracle ACE Program

Oracle's ACE program is **not an internal employee ladder** but a parallel structure for external community experts. The four-tier system (Apprentice / Associate / Pro / Director) gives community members a recognised progression structure — effectively a recognition-program ladder rather than an employment ladder, but worth noting because it mirrors the IC ladder structure for external members.

### MongoDB Champions

Similar pattern to Oracle ACE — external community members progress through recognition tiers (Champion levels are nominated annually). Internal MongoDB DevRel roles use a standard ladder; the public-facing piece is the Champions program.

### Stripe, Twilio, Vercel, Cloudflare, JetBrains, etc.

Internal ladders exist; they are not public. From job postings and public role descriptions, the common pattern is:

- 4–5 IC levels: Developer Advocate / Senior / Staff / Principal / (occasionally Distinguished).
- 3–4 management levels: Manager / Director / Senior Director / VP.
- DevRel-specific job families at the largest of these (Vercel and Stripe have distinct DevRel Engineer roles vs Developer Advocates).
- Compensation tracks engineering at the same level when reporting through engineering/product (most common at Vercel and similar PLG companies).

---

## What to do with this reference

Three uses:

1. **Building your own.** Start with the framework closest to your company size. < 5 person team: Slack or Fitzgerald's small-org template. 5–15: Camunda or Drasner. 15+: GitLab or HashiCorp.
2. **Calibrating across companies.** Use this file when evaluating a job offer or hiring across companies. A "Senior Developer Advocate" at company A may be a "Staff" at company B; the underlying axes of evaluation are similar but the level labels and compensation may differ substantially.
3. **Industry benchmarking.** If your company's DevRel ladder differs significantly from this set of public examples, that may be intentional and good (you have unique structure), or it may be a signal that your ladder needs review.

## Primary sources

- Bear Douglas, "Defining a career path for Developer Relations," Slack Engineering, March 14, 2019 (updated January 28, 2022). Public spreadsheet linked from the post.
- Mary Thengvall, "The Camunda Developer Relations Career Path," marythengvall.com, June 29, 2020. Public Google Sheet linked from the post.
- Sarah Drasner, *Career Ladders* site at career-ladders.dev, with Engineering / DevEx / Documentation ladders. Companion essay: "The Importance of Career Laddering," CSS-Tricks, April 15, 2021.
- GitLab Handbook job-description-library, multiple pages (Developer Advocate, Developer Evangelist, Developer Relations Program Manager, Director of Developer Relations, VP Developer Relations and Community).
- John Coghlan, *GitLab's DevRel career ladder*, DevRelCon talk archived at devrelacademy.com and YouTube.
- Adam Fitzgerald, *Practical Career Matrices for DevRel*, DevRelCon 2021. Talk video and full transcript at developerrelations.com/talks/practical-career-matrices-for-devrel.
- *State of Developer Relations* 2021 (stateofdeveloperrelations.com).
- *devrel-ladders.com* — curated aggregator, maintained by Tony Barnes (@tbarn) since 2021.
- levels.fyi for AWS, Microsoft, Google compensation banding context.

## See also

- [`./career-ladders.md`](career-ladders.md) — Synthesis across all of these.
- [`./building-a-career-ladder.md`](building-a-career-ladder.md) — Practical guide to writing one.
- [`./hiring-and-career.md`](hiring-and-career.md)
- [`./job-titles-and-roles.md`](job-titles-and-roles.md)
- [`./job-openings.md`](job-openings.md) — Live market snapshot.