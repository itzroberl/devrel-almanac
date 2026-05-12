# AAARRRP: A Developer Relations Strategy Framework

**AAARRRP** is Phil Leggetter's adaptation of Dave McClure's *Pirate Metrics* (AARRR), expanded specifically for developer relations work. It first appeared on leggetter.co.uk in 2016 and has since become one of the two or three most widely adopted strategic frameworks in the field, alongside the Orbit Model and the Four Pillars.

## What the acronym stands for

AAARRRP represents seven distinct business goals a DevRel team can serve:

| Letter | Goal | Definition |
|---|---|---|
| **A**wareness | Users become aware of the product. |
| **A**cquisition | Users sign up for the product. |
| **A**ctivation | Users successfully use the product. |
| **R**etention | Users keep using the product, often with growing depth. |
| **R**eferral | Users tell other developers about the product. |
| **R**evenue | Users perform monetising behaviour. |
| **P**roduct | Users (with DevRel's help) shape what the product becomes. |

Two letters distinguish AAARRRP from the original AARRR:

- **Awareness** is added in front because developer audiences are highly fragmented; you cannot acquire developers who do not know you exist, and "awareness" needs to be tracked independently of "acquisition."
- **Product** is added at the end to acknowledge that DevRel does not merely promote an existing product — it actively shapes the product through feedback, beta testing, contributor relationships, and direct participation in the roadmap.

## Funnel or loop?

AAARRRP can be modelled either way:

```
Funnel form:
  Awareness → Acquisition → Activation → Retention → Referral → Revenue → Product

Loop form:
  Awareness → Acquisition → Activation → Retention
                                            ↓
                              Product   ←   Referral / Revenue
                                ↓
                              (back to product features → Awareness)
```

Most early-stage companies use the funnel form; mature platforms run AAARRRP as a flywheel.

## Mapping activities to goals

The framework's practical power is that it forces a DevRel team to **map every activity to one or more goals**. A weekly Twitch stream might serve Awareness and Referral; a quarterly hands-on workshop might serve Activation and Retention; an ambassador program might serve Referral, Product, and Awareness simultaneously.

Leggetter introduced two analytical tools:

- **Goal Alignment** — count how many of the seven goals an activity serves. Activities that score 1 or 2 are tactical; activities that score 4+ are strategic.
- **Goal Weighting** — for each activity, assign a primary, secondary, and tertiary goal. Force the team to prioritise.

An illustrative example matrix (the team should produce its own):

| Activity | Awareness | Acquisition | Activation | Retention | Referral | Revenue | Product |
|---|---|---|---|---|---|---|---|
| Quickstart docs | – | – | ●●● | ● | – | – | – |
| Conference keynote | ●●● | ● | – | – | ●● | – | – |
| Sample app on GitHub | ●● | – | ●●● | – | ● | – | ● |
| Discord office hours | – | – | ●● | ●●● | – | – | ●● |
| Ambassador program | ● | – | – | ●● | ●●● | – | ●● |
| Customer reference content | ●● | ● | – | – | ●●● | ●● | – |
| Product feedback survey | – | – | – | – | – | – | ●●● |

When prioritising next quarter's work, the team can:

- Identify the most under-served goal and add activities that serve it.
- Identify activities that serve too few goals and cut or redesign them.
- Map activities to the business's current strategic priorities (e.g. "this year we need Acquisition more than Retention").

## Choosing where to invest based on company stage

| Company stage | Most-needed goals | Typical activity emphasis |
|---|---|---|
| Pre-PMF, early access | Product, Awareness | Beta programs, deep customer interviews, founder-led evangelism |
| Public launch / early commercial | Awareness, Acquisition | Big launch content, conference launches, paid distribution, AMAs |
| Growth (PLG) | Activation, Retention | Quickstart and onboarding work, sample apps, embedded community help |
| Scale | Referral, Revenue | Ambassador and customer-advocate programs, customer-success content, partner-channel work |
| Mature category leader | Product, Retention | Power-user programs, advisory boards, large-scale conferences and certification |

The framework does not say one goal is more important than another. It says: **be deliberate about which goals you serve, in what order, with what mix of activity**.

## How AAARRRP relates to other frameworks

- **Orbit Model.** AAARRRP is a goals framework; Orbit is a community-membership framework. They compose: Awareness/Acquisition are observable through new Explorer-orbit members; Retention through Participant-to-Contributor movement; Referral through Advocate behaviour. See [`./orbit-model.md`](orbit-model.md).
- **Four Pillars (Lewko & Parton).** Four Pillars defines the *functions* (Education, Marketing, Success, Programs); AAARRRP defines the *goals* those functions serve. See [`./four-pillars.md`](four-pillars.md).
- **Pirate Metrics (AARRR).** The original. AAARRRP keeps the funnel logic and adds developer-specific stages.
- **DevRel Capability Maturity Model.** Where AAARRRP tells you *what* to do, the maturity model tells you *how organised* your function is in doing it. See [`./maturity-model.md`](maturity-model.md).

## Common misuses

- **"AAARRRP says we should do everything."** No. It says *be deliberate* about which goals you serve. A team that tries to serve all seven equally will be mediocre at all seven.
- **"Every activity must score on every goal."** No. Single-goal activities are fine; they just need to be clearly *the right* single goal for that quarter.
- **"AAARRRP is a measurement framework."** Partial. It is a *strategy* framework that surfaces the goals; you still need a measurement framework (instrumenting onboarding funnels, defining DQLs, tracking community contributions) to know whether you are progressing. See [`../04-metrics/metrics-overview.md`](../04-metrics/metrics-overview.md).

## Primary sources

- Phil Leggetter, "AAARRRP: A Developer Relations Strategy Framework," leggetter.co.uk, 2016 (and ongoing updates).
- Phil Leggetter, "Introducing AAARRRP" talk, DevRelCon (multiple editions).
- Dave McClure, "Startup Metrics for Pirates: AARRR!" 500 Startups, 2007.

## See also

- [`./orbit-model.md`](orbit-model.md)
- [`./four-pillars.md`](four-pillars.md)
- [`./maturity-model.md`](maturity-model.md)
- [`../04-metrics/metrics-overview.md`](../04-metrics/metrics-overview.md)