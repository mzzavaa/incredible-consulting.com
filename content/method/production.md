---
title: "3. Production"
description: "The hardening phase most prototypes never survive: infrastructure as code, observability, guardrails, security review, and a cost model that holds at volume."
weight: 53
draft: false
image: "img/mood/tourbillon.webp"
eyebrow: "Method"
headline_2: "The phase that gets skipped."
phase: 3
duration: "4 to 12 weeks"
output: "Deployed system, infrastructure as code, monitoring, runbooks, security and cost review"
---

A prototype that gets promoted to production without this phase is a prototype
running in production. It usually works for a while, which is the problem: the
failure arrives later, with users attached.

This is scoped and quoted as its own piece of engineering work, because that is
what it is.

## What gets done

**Infrastructure as code.** Terraform, in reusable modules, with separate
environments built from the same source. The environment can be destroyed and
rebuilt, and that is tested rather than assumed.

**Observability that answers questions.** Logs, traces, and metrics chosen because
somebody will look at them. For AI systems that includes evaluation in production,
not only in the test harness: sampling live outputs and scoring them, so quality
drift is visible before a user reports it. Cost telemetry per task belongs in the
same dashboard.

**Guardrails and failure behaviour.** Rate limits, timeouts, input validation, and
a defined answer to what the system does when it is unsure. Failing safely and
visibly beats guessing confidently.

**Security review and access model.** Least privilege on every tool an agent can
reach, secrets managed rather than configured, an explicit answer to what the
system can do irreversibly, and an approval step in front of it. Prompt injection
is treated as an attack path, not a curiosity.

**Load and failure testing.** Against the agreed metric and at the expected
volume, plus the failure cases: the dependency is down, the model is slow, the
queue is backed up.

**A cost model that holds.** Recalculated against the real system rather than the
prototype, at expected and at peak volume, with the scaling behaviour stated.

## Go-live

A written plan with a rollback, a defined first-day owner, and a period where the
system runs alongside the process it replaces rather than instead of it. Nothing
is switched over on a Friday.

## What we will refuse

Going live without monitoring, without a rollback, or without a named owner on
your side. Not as a negotiating position: those three are what separate a launch
from an incident with a delay built in.

## Related

[Cloud architecture](/services/cloud-architecture/) covers the platform work.
[Handover](/method/handover/) is the phase after this.
[AI governance](/services/ai-governance/) covers the documentation a regulated
launch needs alongside it.
