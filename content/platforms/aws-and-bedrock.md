---
title: "AWS and Bedrock"
description: "The default platform for AI and cloud delivery here: agent runtimes, serverless pipelines, event-driven architecture, and cost engineering for AI workloads."
weight: 61
draft: false
image: "img/mood/tourbillon.webp"
eyebrow: "Platform"
headline_2: "Production depth, not certification slides."
platform: "aws"
depth: "primary"
tech: ["Bedrock", "AgentCore", "Lambda", "Step Functions", "EventBridge", "S3", "Athena", "Textract", "Rekognition", "Terraform"]
---

For teams already on AWS, or deciding whether to be.

## The services used most

**Bedrock and agent runtimes.** Model access without operating inference
infrastructure, and a serverless runtime for deploying agent crews so that an
agent system does not become a fleet of containers somebody has to keep alive.
Guardrails at the platform layer rather than reimplemented per application.

**Serverless compute and orchestration.** Lambda for the work, Step Functions for
the workflow, EventBridge and queues for the routing. State machines rather than
functions calling functions: a failure halfway through is visible, resumable, and
does not require re-running the expensive earlier steps.

**Storage and data.** Object storage as the substrate, open table formats over it,
query-in-place for analysis, and a managed spatial database where the workload is
geographic. Partitioning decided early, because scanning is what costs money.

**Document and media services.** Text extraction for the mechanical part of
document intelligence, speech to text and visual analysis for media pipelines,
with a model used only for the judgement that genuinely needs one.

**Terraform for everything.** Reusable modules, separate environments from one
source, container images built by a pipeline. Not the console, and not a
click-path documented in a wiki.

## Patterns worth naming

**Scale-to-zero for spiky work.** Media pipelines, event-driven ingest, and
anything that runs a handful of times a month. The cost of idle infrastructure is
the thing that quietly kills internal platforms.

**Model routing.** A strong reasoning model where the task needs it, a cheaper
utility model everywhere else, measured per task. Most workloads that appear
expensive are one routing decision away from being affordable.

**Bounded tool surfaces.** Agents reach systems through defined operations,
increasingly through Model Context Protocol servers, rather than through broad
credentials. This is what makes an agent system reviewable by a security team.

**Evaluation in production.** Sampling live outputs and scoring them, alongside
cost and latency, in the same place someone is already looking.

## Cost engineering specific to AI workloads

Inference cost behaves differently from compute cost: it scales with usage in a
way that is invisible until a bill arrives, and the drivers are prompt size,
output size, retries and model choice rather than instance hours. Caching, prompt
discipline, routing and a hard budget alarm are all part of the build, not a
later optimisation phase.

## Where AWS is the wrong answer

When the data cannot leave your infrastructure, when your team operates a
different platform competently and switching buys nothing, or when the workload is
steady, large and predictable enough that owned hardware is genuinely cheaper. All
three happen. See [Hybrid and open source](/platforms/hybrid-and-open-source/).

## Related

[AI and agent systems](/services/ai-and-agents/),
[Cloud architecture](/services/cloud-architecture/), and the delivered examples in
[Case studies](/case-studies/).
