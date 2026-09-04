---
title: "Developer Platforms and Automation"
description: "Internal developer portals, configuration automation and container platforms, for teams whose real bottleneck is that shipping anything takes three weeks."
weight: 63
draft: false
image: "img/mood/seams.webp"
eyebrow: "Platform"
headline_2: "The bottleneck is rarely the model."
delivered_by: "Associate network, led on architecture in house"
platforms: ["Backstage", "Red Hat Developer Hub", "Ansible", "Ansible Automation Platform", "OpenShift"]
targets: ["AWS", "Azure", "On-premises"]
---

AI work sits on top of a delivery platform, and most of the time that platform is
the actual constraint. This page is for the reader whose problem is not a model.
It is that a change takes three weeks and four tickets, and nobody can say which
of the four is the slow one.

## The position, stated plainly

An internal developer platform is worth building when developer friction is
measurable, and it is an expensive vanity project when it is not.

The way to tell before quoting anything: measure lead time from commit to
production, count the handoffs, and find out how a new engineer gets an
environment. If that last answer is "asks someone in a chat and waits", there is a
platform problem. If changes reach production the same day and onboarding is
self-service, there is not, and building a portal will produce a portal.

## Internal developer portals

**Backstage and Red Hat Developer Hub.** One is the upstream project with maximum
flexibility and the maintenance burden that implies. The other is a supported
distribution with an opinion, which is worth a great deal to a team that does not
want to own a portal as a product.

The honest note: the portal is the easy part. The service catalogue and the
ownership model are the hard part, and they are organisational rather than
technical. A catalogue nobody maintains becomes a directory of systems that no
longer exist, which is worse than no catalogue, because people trust it.

Start with golden paths rather than with a catalogue: one templated way to create
a service that is genuinely faster than the manual route. Adoption follows utility.

## Configuration automation

Ansible and Ansible Automation Platform for estates where infrastructure as code
has to reach machines rather than only cloud APIs. Frequently the pragmatic answer
in mixed estates where a Terraform-only story does not survive contact with the
older half of the environment.

## Container platforms

OpenShift on cloud or on your own hardware, for teams standardising on a platform
they can operate in both places. See
[Hybrid and open source](/platforms/hybrid-and-open-source/).

## How this is delivered

Architecture and the decision about whether to build at all are led in house.
Depth on the specific platforms comes from the
[associate network](/team/network/), introduced by name before anyone starts.

## What we will tell you not to do

Do not build a platform for three teams. Do not build a portal before you have a
golden path worth putting in it. Do not make the platform team a ticket queue,
which recreates the problem it was built to remove with a nicer interface.

## Related

[Cloud architecture](/services/cloud-architecture/),
[Automation](/services/automation/), and
[Architecture audit](/engagements/architecture-audit/) for an independent read on
whether the friction is real.
