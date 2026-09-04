---
title: "Cloud Architecture"
description: "AWS and hybrid architecture, migrations, cost control, and reviews by someone who has operated the systems, not only drawn them."
weight: 12
draft: false
image: "img/mood/glass-stack.webp"
eyebrow: "Cloud Guild"
headline_2: "Architecture that survives real traffic."
pillar: "cloud"
typical_duration: "2 to 12 weeks"
typical_deliverable: "Target architecture, migration plan, Terraform baseline, cost model"
tech: ["AWS", "Terraform", "Lambda", "Step Functions", "EventBridge", "OpenShift", "Well-Architected"]
---

Architecture diagrams are cheap. The expensive part is the set of decisions
underneath them: what stays where, what it costs at your actual volume, who is on
call for it, and which parts you will regret in two years. This practice is about
making those decisions explicitly and writing down why.

## What gets delivered

**Target architecture and landing zone.** Account structure, network boundaries,
identity, and the guardrails that stop the interesting failures. Written as
infrastructure as code, in reusable modules, with dev and production environments
built from the same source.

**Migration and modernisation paths.** Including the honest do-not-migrate cases.
Some workloads are cheaper, safer and faster exactly where they are, and a
migration plan that says so is worth more than one that does not.

**Cost control.** Where the money actually goes, measured rather than estimated,
and what to change first. Scale-to-zero patterns for spiky workloads, the
pay-per-use against reserved capacity question answered with your numbers, and
cost telemetry wired in from the start rather than discovered on a bill.

**Operational readiness.** Observability that answers questions rather than
filling dashboards: logs, traces, alarms that someone actually responds to, and
the runbook for the failure you have already had once.

**Well-Architected review** as a fixed-scope option when the requirement is an
independent read against a recognised framework.

## The shared responsibility conversation

Most cloud disappointment traces back to one misunderstanding: which half of the
stack is yours. The provider secures the cloud, you secure what you put in it,
and the line moves depending on whether you are buying software, a platform, or
raw infrastructure. Getting that line drawn explicitly, early, with your security
people in the room, prevents the review that stops a launch three weeks out.

## Hybrid, and when it is the right answer

Sensitive workloads in banking, insurance, healthcare and the public sector often
cannot sit in a public region, and pretending otherwise wastes everyone's time.
The pattern that works is usually split rather than binary: public cloud for
public or low-sensitivity data where scale-to-zero and speed matter, private or
on-premises for the sensitive core, and a designed join between them. See
[Hybrid and open source](/platforms/hybrid-and-open-source/).

## Where this does not apply

If the platform is fine and the problem is that shipping anything takes three
weeks and four tickets, the bottleneck is delivery, not architecture. That is
[developer platforms](/platforms/developer-platforms/).

## Related

[Architecture audit](/engagements/architecture-audit/) is the fixed-scope entry
point. [Data platforms](/services/data-platforms/) covers the layer underneath
the analytics and AI work.
