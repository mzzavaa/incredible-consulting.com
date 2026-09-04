---
title: "Security and Compliance"
description: "Access, data handling, confidentiality, subprocessors, and how AI systems are built so a compliance review does not stop them three weeks before launch."
weight: 93
draft: false
image: "img/mood/clamp.webp"
eyebrow: "FAQ"
headline_2: "What happens to your data."
topic: "security"

# CONFIRM BEFORE PUBLISHING. This page states operating practice, not
# certifications. Deliberately absent because they cannot be claimed without
# evidence: ISO 27001 or SOC 2 status, professional indemnity cover and limits,
# a named subprocessor list, and background check policy for associates. If any
# of those exist, add them here and to /pricing/procurement/. If they do not,
# leave the page as it is: an unclaimed certification is fine, a claimed one that
# does not exist is not. Delete this block once checked.
---

## What access do you need?

As little as possible, for as short a time as possible. Most discovery and audit
work needs read-only access. Build work needs a scoped account in a development
environment, issued by you, with credentials that expire. Production access is
usually not required at all: deployments run through your pipeline rather than
from a laptop.

Where an environment is locked down enough that access itself is slow, that is a
cost driver and it is named in the proposal.

## What happens to our data?

It stays in your environment wherever the work allows. Where sample data must be
copied out for prototyping, it is agreed in writing first, minimised, and deleted
at the end of the engagement, with deletion confirmed in writing.

Nothing from an engagement is used as public material, in a talk, a blog post or a
case study, without written permission. That is why no client is named anywhere on
this site.

## Do you sign an NDA?

Yes, and usually yours as-is. A data processing agreement is signed where the work
involves personal data. See
[Procurement and contracting](/pricing/procurement/).

## Who else sees our data?

Only people named in the statement of work. Associates are engaged under
back-to-back terms that carry your confidentiality, data processing and
intellectual property terms through unchanged. If a subprocessor would be involved
in handling your data, it is named before the work starts, not disclosed
afterwards.

## Where is data processed?

An engagement design input rather than an afterthought. For EU workloads that
usually means EU regions and, for the sensitive core, private infrastructure with
a designed join to anything public. See
[Hybrid and open source](/platforms/hybrid-and-open-source/).

## Do models train on our data?

Not in the configurations used here. Enterprise model platforms and business
tiers of hosted services come with explicit data processing terms, including no
training on customer content and region options. Which terms apply is checked and
written into the architecture documentation rather than assumed, and it is one of
the questions the [governance work](/services/ai-governance/) answers explicitly.

## How do you stop an agent doing something it should not?

Least privilege on every tool it can reach, a bounded set of operations rather
than broad credentials, an approval step in front of anything irreversible, and
logs good enough to reconstruct what happened. Prompt injection is treated as an
attack path against those tools rather than as a curiosity. See
[Production](/method/production/).

## What about the EU AI Act?

Most systems in most companies are not high risk, and establishing that with
reasoning is part of the work rather than an assumption. Where obligations do
apply, they are mapped onto concrete engineering controls: which step, which
person, which log, and what happens when they disagree with the system. See
[AI governance](/services/ai-governance/).

This is an engineering and documentation position for your counsel to review. It
is not legal advice, and where a genuine legal question arises it goes to a
lawyer.

## Do you do penetration testing?

Not in house. Security testing is available through named specialist partners in
the [associate network](/team/network/), and an
[architecture audit](/engagements/architecture-audit/) will say plainly where a
finding needs a specialist rather than bluffing it.

## What about this website?

It is a static site. No cookies, no analytics, no tracking, no forms, and no
external fonts or scripts. The only outbound requests your browser makes are ones
you click. See [Privacy](/legal/privacy/).
