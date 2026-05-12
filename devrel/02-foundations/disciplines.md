# Disciplines Within Developer Relations

DevRel is an umbrella covering several adjacent disciplines. Job titles and team boundaries vary by company, but the underlying functions are stable. This file defines each one, the work it does, the kind of person who does it well, and how it relates to the others.

## 1. Developer Advocacy

**Definition.** A public-facing technical practitioner who teaches, demonstrates, and listens — representing the developer community to the company and the company's capabilities to the community.

**Primary work.**

- Writes blog posts, tutorials, and sample code.
- Speaks at conferences, meetups, and user groups.
- Streams or records video content.
- Maintains a personal voice in public technical forums.
- Triages community feedback and represents it inside the company.
- Reviews docs, SDKs, and APIs for "developer feel."

**Best fit person.** A practising engineer who genuinely enjoys writing, speaking, and teaching, who maintains technical credibility through ongoing hands-on work.

**Often confused with.** Evangelism (more outbound, often more product-pitched). Technical marketing (more campaign-driven, more decision-maker-targeted).

## 2. Developer Evangelism

**Definition.** Originally synonymous with advocacy, the "evangelist" label now usually signals a stronger outbound and adoption-oriented bias. Where advocacy puts the developer's interests first, evangelism more often leads with the company's product or platform's importance.

The distinction is a soft one and many practitioners use the labels interchangeably. In practice:

| Advocate | Evangelist |
|---|---|
| Listens then talks | Talks then listens |
| Helps developers win with the product | Helps the product win developers |
| Often reports to product or engineering | Often reports to marketing |
| Measured by satisfaction, retention, product feedback | Measured by reach, signups, awareness |

Both are legitimate. They are not "good" and "bad" versions of each other; they are differently positioned tools for differently sized adoption problems. Early-stage products with low awareness often need more evangelism; mature products with engaged user bases often need more advocacy.

Historically, "evangelist" was the dominant term from Apple's Guy Kawasaki (early 1980s) through Microsoft's global Developer & Platform Evangelism organisation of the 1990s–2000s. The shift toward "advocate" began in the late 2000s and accelerated through the 2010s as the field matured.

## 3. Developer Experience (DevEx / DX)

**Definition.** The end-to-end experience a developer has when they discover, evaluate, learn, integrate, ship, operate, and (sometimes) leave a product.

DevEx covers:

- Time to first hello world (TTFHW).
- Quality of docs, SDKs, and CLIs.
- Error messages, debuggability, and observability.
- Onboarding flows and free-tier friction.
- API ergonomics and breaking-change discipline.
- Local dev environment quality.

DevEx is owned by some combination of product, engineering, and DevRel. At larger companies it often has its own org: "VP of Developer Experience" is now a common title at infrastructure and developer-tools companies.

Two related strands exist:

- **External DevEx** — the experience of customers of a developer product. This is the DevRel-adjacent meaning.
- **Internal DevEx (Platform Engineering)** — the experience of a company's own engineers using its internal platforms. Driven by separate frameworks (DORA, SPACE, DXI, DX Core 4) and separate vendors (LinearB, Swarmia, DX, Sleuth).

See [`../11-trends/devex-movement.md`](../11-trends/devex-movement.md) and [`../03-frameworks/space-and-dxi.md`](../03-frameworks/space-and-dxi.md).

## 4. Developer Education

**Definition.** Producing the content and curricula that take a developer from "never heard of this" through "shipped to production" and onward to expert.

**Primary work.**

- Documentation strategy and information architecture.
- Tutorials, quickstarts, getting-started flows.
- Reference docs and API documentation.
- Video courses and screencasts.
- Workshops (live and self-paced).
- Sample applications.
- Certification programs.

**Best fit person.** Often a hybrid technical writer / instructional designer who can write code, prose, and curricula. At larger companies this is its own org (e.g. Stripe, Twilio, AWS, MongoDB all maintain large developer-education orgs separate from advocacy).

**Why it is increasingly central.** In product-led growth, the docs are the salesperson. A clear quickstart and a working code sample drive activation; a confusing onboarding loses the deal silently. See [`../10-tactics/documentation-as-product.md`](../10-tactics/documentation-as-product.md).

## 5. Developer Marketing

**Definition.** Marketing whose audience is developers. Sometimes labelled B2D (Business-to-Developer).

**Primary work.**

- Positioning and messaging tested against developer audiences.
- Developer-targeted content distribution (newsletters, podcasts, search, video, communities).
- Persona research grounded in actual developer interviews.
- Paid and organic acquisition channels respectful of developer norms.
- Coordinated launches (release notes, blog, video, social, community AMAs).
- Conference sponsorships, booth strategy, and side-events.

Developer marketing differs from consumer or traditional B2B marketing in tone, format, and channel. Developers prefer technically substantive content, will read 3,000-word architectural deep-dives, hate gated lead-magnet PDFs, and trust peers more than press releases.

**Best fit person.** A marketer who has shipped code or worked closely with engineers. Or an engineer with marketing instincts. The pairing of the two is often the most effective developer-marketing org structure.

## 6. Developer Success (Enablement / Support)

**Definition.** The function that ensures developers who start using the product actually succeed in shipping with it.

**Primary work.**

- Helping new customers onboard technically — sometimes via 1:1 conversations, sometimes by building scaled enablement programs.
- Tracking adoption signals after signup.
- Identifying and unblocking churn risks.
- Operating community Q&A, Discourse forums, and Discord/Slack help channels.
- Coordinating with engineering on common bug patterns.

Distinct from traditional support in that the goal is **adoption depth**, not ticket resolution. Common at API and infrastructure companies (Twilio, Stripe, MongoDB, HashiCorp), where the line between "support" and "consulting" is blurry.

## 7. Community Management

**Definition.** The operation and nurturing of the spaces where developers gather around the product, the company, or the broader technology.

**Primary work.**

- Running official Discord/Slack/Discourse spaces with clear rules and active moderation.
- Welcoming new members, surfacing useful answers, recognising contributors.
- Programming events (AMAs, office hours, contest weeks).
- Coordinating with advocacy on local user groups and ambassador programs.
- Reporting community health upward (retention, response time, sentiment).

Community managers do not have to be deeply technical; they have to be **tech-fluent**, empathetic, organised, and durable. Jono Bacon's *The Art of Community* (2012) and *People Powered* (2019) are still the canonical references.

See [`../10-tactics/community-building.md`](../10-tactics/community-building.md) and [`../08-tools/community-platforms.md`](../08-tools/community-platforms.md).

## 8. Developer Programs

**Definition.** Structured initiatives that recognise, equip, and compound the impact of the company's most engaged external community members.

**Examples.**

- Microsoft MVPs (since 1993, formalised 1999).
- AWS Heroes (since 2014).
- AWS Community Builders.
- Google Developer Experts (GDE).
- Google Developer Groups (GDG).
- MongoDB Champions.
- HashiCorp Ambassadors.
- GitHub Stars and GitHub Campus Experts.
- Oracle ACE Program (oldest at scale, established 1990s).
- IBM Champions.
- Cloudflare Developer Experts.
- Snyk Ambassadors.
- Auth0 Ambassadors.
- Datadog Ambassadors.
- JetBrains Academy Ambassadors and Content Creators.

Programs usually offer: early access, direct line to product, exclusive swag, travel sponsorship, a private community, and visibility through speaker placement and content amplification. They cost the company very little and produce disproportionate amplification — the highest-leverage tactic in DevRel when run well, and a corrosive disappointment when run badly.

See [`../10-tactics/ambassador-programs.md`](../10-tactics/ambassador-programs.md) for design principles, common failure modes, and case studies.

## How the disciplines compose

Not every company has all eight as distinct roles. A small startup may have one Developer Advocate who informally does six of these. A 200-person DevRel org at a large platform company will have separate teams (and separate VPs) for each.

A useful rule of thumb for sequencing as a program scales:

1. **0–1 people:** One generalist Developer Advocate who can write, code, and speak.
2. **2–5 people:** Add a Community Manager and a Developer Educator (docs/tutorials).
3. **5–15 people:** Add specialists by domain (e.g. AI, mobile, data), and a content/program manager.
4. **15+ people:** Add Developer Marketing, Developer Success, regional advocates, and a Director/VP layer.

See [`./org-structures.md`](org-structures.md) for sizing and reporting models. The empirical finding from State of Developer Relations 2024: teams that hire Community Manager → Evangelist → Director achieved roughly **40% higher onboarding completion rates** than teams that hired evangelists first.

## Primary sources

- Lewko & Parton, *Developer Relations: How to Build and Grow a Successful Developer Program* (Apress, 2021).
- Mary Thengvall, *The Business Value of Developer Relations* (Apress, 2018).
- SlashData / Developer Marketing Alliance, *State of Developer Relations* reports (2022–2024).
- Daily.dev, "Developer Advocates vs Technical Evangelists" (2024).