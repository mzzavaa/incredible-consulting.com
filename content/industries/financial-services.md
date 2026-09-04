---
title: "Financial Services"
description: "Regulated architecture, data residency and document-heavy processes, with the honest note that the delivered depth here is transferred from adjacent regulated work."
weight: 33
draft: false
image: "img/mood/plumb-line.webp"
eyebrow: "Sector"
headline_2: "Regulated by default."
sector: "financial-services"
position: "Transferred"
---

**Stated plainly first:** there is no named banking or insurance engagement to
point at. What exists is regulated-architecture work, residency and hybrid design,
and document-heavy AI delivery in other sectors with comparable constraints. If
your requirement is a consultancy with a reference in your exact regulatory
setting, that is a fair requirement and this is not it.

## The problems that recur

**Data that cannot go to a public region.** Core banking, claims, and customer
records in banking, insurance and pension work frequently cannot leave controlled
infrastructure. The architecture question is not whether to use public cloud but
where the line runs and how the two sides are joined. See
[Hybrid and open source](/platforms/hybrid-and-open-source/).

**Document-heavy processes.** Contracts, policies, claims, compliance packs, KYC
files. This is the strongest AI use case shape in the sector, and also the one
with the least tolerance for a confident wrong answer, which is why the
verifiable-extraction work matters more than model choice.

**Explainability as a hard requirement.** Not a preference. A decision affecting a
customer needs to be reconstructable: what the system saw, what it produced, and
who reviewed it. That is a logging and workflow design problem before it is a
model problem.

**Model risk and the EU AI Act.** Sitting alongside existing model governance
rather than replacing it. Most systems are not high risk, and establishing that
with reasoning is the work. See [AI governance](/services/ai-governance/).

**Legacy that cannot be interrupted.** The interesting systems are the ones that
must not stop, which pushes work toward the edges: integration, augmentation and
parallel running rather than replacement.

## What transfers

The verifiable-selection pattern from
[the video pipeline](/case-studies/video-intelligence-pipeline/) is directly
applicable to document extraction: a model selects from a source, and the
selection must be checkable against that source structurally rather than by asking
a second model whether the first was right.

The hybrid split designed for sensitive infrastructure data in
[the grid engagement](/case-studies/geo-ai-platform/) is the same architecture
question with different regulators.

## Where to start

An [architecture audit](/engagements/architecture-audit/) if a system already
exists and the concern is whether it will hold. A
[workshop series](/engagements/workshop-series/) if the question is which use case
is worth the compliance effort at all, since in this sector the review cost is
frequently larger than the build cost and belongs in the ranking.

## Related

[AI governance](/services/ai-governance/),
[Cloud architecture](/services/cloud-architecture/),
[Security and compliance](/faq/security-and-compliance/).
