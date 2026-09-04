---
title: "Multi-Agent Automation Hub"
description: "Five half-automated back-office workflows consolidated behind one conversational entry point, with infrastructure as code, a deployment pipeline, and cost measured per task."
weight: 42
draft: false
image: "img/mood/sphere.webp"
social_image: "images/statements/type-per-task-ai-cost.webp"
eyebrow: "Case study"
headline_2: "One door, five crews."
client: "Internal product, offered as a reference build"
industry: "Professional services operations"
status: "active"
status_label: "In production"
engagement_type: "Proof of concept into production"
tech: ["AWS Bedrock", "AgentCore", "CrewAI", "Terraform", "CodeBuild", "Lambda", "Claude"]
outcome: "Recurring back-office work handled by agents behind a single conversational entry point"
---

{{< poster src="images/statements/type-per-task-ai-cost.webp" alt="Real world impact, three. Per task AI cost, measured, not estimated. Multi-Agent Automation Hub." >}}

## Why this one is ours

This is an internal product rather than a client engagement, and it is published
as a reference build for exactly that reason: everything can be described,
including the parts that went wrong, without asking anyone's permission.

It is also the honest answer to a question buyers ask: do you run this yourself,
or do you only recommend it to other people.

## The problem

Five unrelated operational workflows, each about half automated. A proposal
assembly process, a client follow-up and deliverables process, a content
pipeline, a research process, and a status and reporting loop. Each had a good
tool at either end and a person in the middle moving things across.

Individually, none justified a project. Together they consumed a substantial part
of every week, and the cost was invisible because it was spread across every day.

## What was built

**One entry point.** A single conversational interface instead of five tools. A
request arrives in plain language, an orchestration agent works out which crew
owns it, and the crew runs.

**Specialised crews rather than one large agent.** Each crew has a narrow job, its
own tools, and its own definition of a finished output. Hierarchical where a
supervisor is genuinely needed, sequential where the steps depend on each other,
parallel where they do not. Small specialists are easier to evaluate and far
easier to debug than one agent with thirty tools.

**Documentation as the system of record.** Outputs are written back into the
workspace where the work already lives, as structured pages rather than chat
history, so the result of a run is an artefact somebody can find next month.

**Infrastructure as code.** Terraform in reusable modules, separate development
and production environments from the same source, container images built by a
pipeline. The whole thing can be destroyed and rebuilt, and that has been tested
rather than assumed.

## Cost control

Cost per task is measured, not estimated per month. Model routing sends the
reasoning-heavy steps to a strong model and everything else to a cheap one, and
the split is visible in the same dashboard as the error rate. A run that suddenly
costs three times as much is a signal, and it is only a signal if somebody is
measuring it.

## What broke first

**The orchestrator was too clever.** The first version tried to decompose any
request. It was impressive in a demo and unpredictable in use. Narrowing it to a
router over well-defined crews made it duller and considerably more useful.

**Silent failure.** Early runs could half-succeed and write a partial artefact
that looked complete. The fix was structural: a crew now either produces a
validated output or fails loudly, with no in-between state.

**Prompts as configuration.** Prompts embedded in code meant every wording change
was a deployment. They moved out, into versioned configuration, with the same
review as any other change.

## Where the pattern transfers

Any organisation with several coordination-heavy processes that each individually
look too small to automate. The value is in the shared runtime, the shared
deployment path and the shared observability, not in any single workflow.

## Related

[Automation](/services/automation/),
[AI and agent systems](/services/ai-and-agents/),
[Proof of concept](/engagements/proof-of-concept/), and
[AWS and Bedrock](/platforms/aws-and-bedrock/).
