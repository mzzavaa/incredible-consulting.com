---
title: "AI Governance and Compliance"
description: "EU AI Act readiness, model risk documentation, and the audit trail your legal team will ask for, mapped onto engineering controls rather than policy prose."
weight: 15
draft: false
image: "img/mood/plumb-line.webp"
eyebrow: "AI Guild"
headline_2: "Ship it, and be able to explain it."
pillar: "governance"
typical_duration: "3 to 8 weeks"
typical_deliverable: "Risk classification, control set, documentation pack, review cadence"
tech: ["EU AI Act", "ISO 42001", "AWS Well-Architected", "Bedrock Guardrails", "Langfuse"]
---

The common failure is not that a company builds an AI system it should not have
built. It is that a system nobody could describe reaches legal review three weeks
before launch, and there is no documentation of what data it used, what it does
when it is unsure, or who decided that was acceptable.

This is the work that prevents that conversation, done as engineering rather than
as a policy document nobody reads.

## What gets delivered

**Risk classification.** Every existing and planned AI use case placed against
the obligations that actually apply to it. Most systems in most companies are not
high risk, and saying so with reasoning is as valuable as flagging the ones that
are.

**Obligations mapped to controls.** Not "ensure appropriate human oversight" but
which step, which person, which log, and what happens when they disagree with the
system. The output is a control set an engineer can implement and an auditor can
check.

**Documentation pack.** What the system does, what data trained or grounds it,
known limitations, evaluation results, and the decisions taken with their
alternatives. Written once, during the build, rather than reconstructed afterwards
from memory.

**Evidence.** Logging, evaluation traces and guardrail behaviour retained so a
claim about the system can be checked instead of asserted.

**Review cadence.** Who signs off, how often it is revisited, and what triggers an
early review. A model swap is a review trigger; a prompt change on a
consequential path usually is too.

## Agentic systems specifically

An agent with tool access raises a question that a chatbot does not: what can it
reach, with whose authority, and what stops it doing something irreversible. That
is simultaneously a security question and a compliance one, and it is answered the
same way in both directions: bounded tools, least privilege, an approval step in
front of anything with consequences, and a log good enough to reconstruct what
happened.

## Where the data actually goes

For teams weighing a hosted model against a self-hosted one, the honest comparison
is not capability, it is the data processing story: what is retained, whether it
trains anything, where it is processed, and what the contract says. Both answers
can be correct. See [Hybrid and open source](/platforms/hybrid-and-open-source/).

## What this is not

Not legal advice. The output is an engineering and documentation position your
counsel can review, and where a genuine legal question arises it goes to a lawyer
rather than to us.

## Related

[Security and compliance FAQ](/faq/security-and-compliance/),
[Public sector](/industries/public-sector/), and
[Financial services](/industries/financial-services/). The frameworks and
checklists behind this are published openly on incredible-consulting.org rather
than kept proprietary.
