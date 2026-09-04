---
title: "Platforms and Stack"
description: "What we build on and the honest reasons why: AWS as the primary depth, hybrid and self-hosted where sensitivity demands it, and the delivery platform underneath both."
weight: 60
draft: false
image: "img/mood/seams.webp"
social_image: "images/statements/photo-architecture-and-trust.webp"
eyebrow: "Stack"
headline_2: "Deepest on AWS. Honest about the rest."
---

Technical buyers want to know the stack before the call, so it is written down
here rather than discovered in a discovery meeting.

## Where the depth actually is

**AWS is primary,** and it is where the depth is genuinely deepest: Bedrock and
agent runtimes, serverless data and media pipelines, event-driven architecture,
Terraform, and the cost engineering that keeps any of it affordable. The AWS
Community Hero recognition comes from sustained work in that ecosystem rather
than from a partner tier.

**Azure and Google Cloud are covered through the
[associate network](/team/network/)** rather than claimed as equal in-house
depth. Saying so costs a few enquiries and is more useful than the alternative,
which is finding out mid-engagement.

**Hybrid and self-hosted is a real practice, not a fallback.** For sovereignty,
data residency, latency or cost at volume there are workloads that should not run
in a public region, and pretending otherwise wastes everyone's time. See
[Hybrid and open source](/platforms/hybrid-and-open-source/).

**The delivery platform underneath** is often the actual bottleneck. If shipping
anything takes three weeks and four tickets, no model is going to help. See
[Developer platforms](/platforms/developer-platforms/).

## The three pages

- [**AWS and Bedrock**](/platforms/aws-and-bedrock/). The default platform and
  the patterns used most.
- [**Hybrid and open source**](/platforms/hybrid-and-open-source/). Workloads
  that cannot or should not sit in a public cloud.
- [**Developer platforms**](/platforms/developer-platforms/). Internal developer
  portals, configuration automation, and container platforms.

## How a platform gets chosen

Not by preference. The questions, in order: where does the data have to live, what
does the team already operate competently, what does it cost at your volume rather
than at demo volume, and what does the exit look like if the vendor changes the
terms.

## Vendor neutrality, stated honestly

There is a visible AWS relationship here, and that is a fact a buyer should weigh
rather than a secret. Two things follow. Where an engagement is genuinely a
platform selection, the evaluation criteria are agreed in writing before any
assessment starts, and the reasoning is written down so it can be challenged.
Where provider funding is in play, note that funding pulls an architecture toward
that provider, which is why the neutrality question is settled before a funding
application rather than after. See [Cloud funding and credits](/pricing/funding/).

## Lock-in we cannot exit

The test applied to any managed service: if this vendor doubled the price or
withdrew the service, what would it take to move. Sometimes the answer is
"considerable, and it is still worth it", which is a fine answer as long as it was
made deliberately and written down.
