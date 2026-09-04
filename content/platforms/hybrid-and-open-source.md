---
title: "Hybrid and Open Source"
description: "OpenShift, Kubernetes and open weight models for workloads that cannot or should not sit in a public cloud, and an honest account of what that costs."
weight: 62
draft: false
image: "img/mood/sphere.webp"
eyebrow: "Platform"
headline_2: "When the data cannot leave."
platform: "hybrid"
depth: "secondary"
tech: ["OpenShift", "OpenShift AI", "Kubernetes", "open weight models", "Terraform", "Ansible"]
---

In banking, insurance, healthcare and the public sector there are workloads that
cannot sit in a public region, and no amount of architecture enthusiasm changes
that. The useful question is not whether to use public cloud, it is where the line
runs and how the two sides are joined.

## The split that usually works

Not binary. Split by sensitivity:

- **Public or low-sensitivity data in public cloud,** where scale-to-zero,
  managed services and speed of experimentation are worth the most.
- **The sensitive core in private infrastructure,** where compliance, control and
  data residency are the requirement.
- **A designed join between them,** so an analysis can use public reference data
  and private records without the private records leaving.

Deciding this deliberately, with the people responsible for both sides in the
room, is a one-workshop conversation. Discovering it midway through a migration
is considerably more expensive.

## Open weight models and self-hosting

**Where quality is now sufficient.** Extraction, classification, summarisation,
structured output over a known domain, and retrieval-grounded answering. For a
large class of production work the open models are good enough, and the
constraint has moved from capability to operations.

**Where it is not.** Long multi-step reasoning, difficult tool use, and tasks that
depend on the strongest available model. Being honest about this matters: a
self-hosted deployment that quietly underperforms is worse than a hosted one that
was rejected on principle.

**What self-hosting actually costs.** Not the licence, which is usually zero. The
GPU capacity, the person who keeps it running, model updates and the regression
testing that follows them, and the evaluation harness that tells you whether the
new version is better. Teams that budget for the hardware and not the operations
end up with an expensive model nobody dares to update.

**When it is clearly right.** Data that cannot leave, volume high enough that
per-token pricing dominates, latency requirements that a network round trip
cannot meet, and a sovereignty requirement that is contractual rather than
aesthetic.

## The data question, answered plainly

For a team weighing hosted against self-hosted, the comparison is not capability,
it is the data processing story: what is retained, whether anything is trained on
it, where processing physically happens, and what the contract actually commits
to. Business tiers of hosted services often come with explicit data processing
agreements, EU residency options and no training on customer data, which makes
them a legitimate answer in regulated settings. Local processing on infrastructure
you control is a different compliance story again. Both can be correct. The wrong
answer is choosing without reading either.

## Container platforms

OpenShift and Kubernetes for teams that already operate them, on cloud or on their
own hardware, with the AI serving layer on top rather than as a separate island.
Configuration automation so the environment is reproducible rather than
hand-tuned. This work is led on architecture in house and delivered with the
[associate network](/team/network/) where depth is needed.

## When hybrid is nostalgia

If the honest reason for staying on-premises is that a migration would be
uncomfortable, the architecture will show it: no residency requirement anyone can
cite, no volume argument, no latency constraint. That is a legitimate position and
it should be stated as a preference rather than dressed as a compliance
requirement, because the two lead to different designs.

## Related

[Cloud architecture](/services/cloud-architecture/),
[AI governance](/services/ai-governance/),
[Financial services](/industries/financial-services/), and
[Public sector](/industries/public-sector/).
