---
title: "Automation"
description: "Removing the manual work between your systems: internal workflows, document handling, and the operations that still run on copy and paste."
weight: 13
draft: false
image: "img/mood/gears.webp"
eyebrow: "Automation Guild"
headline_2: "The work between the systems."
pillar: "automation"
typical_duration: "4 to 10 weeks"
typical_deliverable: "Automated workflow in production, runbook, monitoring"
tech: ["Lambda", "Step Functions", "EventBridge", "SQS", "Amazon Textract", "Python", "Terraform"]
---

Every organisation has a set of processes that are half automated. Two good
systems at either end and a person in the middle moving data between them,
checking a spreadsheet, forwarding an email, and re-keying the same number for
the third time. Nobody owns it because it is not anybody's system. It is often
the cheapest large improvement available.

## How the work starts

**Measure where the hours go.** Not a guess, and not a workshop where people
estimate their own effort. Sample the actual process, count the handoffs, and find
the steps that are frequent, rule-based and slow.

**Rank candidates by hours saved against build cost.** Most processes should not
be automated. The ranking makes that argument in numbers instead of opinion, and
the recommendation to leave something alone is a legitimate output.

**Automate the handover, not the task.** In coordination-heavy processes the
expensive part is rarely any single step. It is the waiting between steps, the
approval that sits for two days, and the rework when something arrives in the
wrong shape.

## The patterns that get built

- **Event-driven pipelines.** A file lands, an event fires, a workflow runs, a
  result is written back. Step Functions for the orchestration, Lambda for the
  work, EventBridge and queues for the routing.
- **Document workflows.** Extract, structure, validate. Text extraction for the
  mechanical part, a model for the judgement part, and a validation step that
  fails loudly rather than passing something wrong down the line.
- **Approval and exception flows.** The happy path automated, the exceptions
  routed to a person with the context attached, and a record of both.

## Where AI belongs, and where it does not

AI belongs where the input is genuinely unstructured or the judgement is genuinely
fuzzy. Everywhere else, plain code is cheaper to run, faster, deterministic, and
possible to debug at two in the morning. A workflow that puts a language model in
front of a lookup table is a liability, not innovation. Expect that argument.

## What happens when it breaks

Automation moves the failure rather than removing it, so the failure needs an
owner. Every delivered workflow ships with monitoring, an alert that goes to a
named person, a runbook that describes the three failures we already know about,
and a manual fallback for the day the automation is wrong.

## Related

[Multi-Agent Automation Hub](/case-studies/automation-hub/) is a delivered
example. [AI and agent systems](/services/ai-and-agents/) covers the cases where
the coordination itself is the hard part. [Retainer](/engagements/retainer/)
covers care and feeding once it is live.
