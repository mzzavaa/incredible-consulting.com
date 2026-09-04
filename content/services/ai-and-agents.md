---
title: "AI and Agent Systems"
description: "Multi-agent systems, retrieval, and document intelligence taken from a prototype to something you can run in production and afford to keep running."
weight: 11
draft: false
image: "img/mood/lattice.webp"
eyebrow: "AI Guild"
headline_2: "Evidence before enthusiasm."
pillar: "ai"
typical_duration: "6 to 14 weeks"
typical_deliverable: "Working agent system, evaluation harness, deployment pipeline"
tech: ["AWS Bedrock", "AgentCore", "CrewAI", "LangGraph", "MCP", "Amazon Textract", "Claude"]
---

Most organisations have now run an AI pilot. A good number of them cannot say
whether it worked, because nobody agreed in advance what working would look like.
This practice exists to fix that: build the thing, measure it against a number
agreed before the build, and be willing to conclude that it is not worth
producing.

## What gets built

**Agent systems and orchestration.** Crews of specialised agents for
coordination-heavy processes: handoffs, approvals, internal operations, research
and reporting. Hierarchical and sequential crews, deployed on a serverless
runtime rather than a laptop. Frameworks are chosen rather than assumed, and the
comparison is usually run live in a workshop, on your use case, instead of argued
in the abstract.

**Retrieval and document intelligence.** Extract, structure and validate:
contracts, compliance packs, technical documentation, and the knowledge sitting
in inboxes. The engineering work is rarely the model, it is chunking, retrieval
quality, and knowing when the system should refuse to answer.

**Natural language interfaces over existing systems.** Turning a query language
or a specialist tool into a question anybody in the business can ask. This is
where the Model Context Protocol earns its place: a bounded, auditable surface
that an agent may call, rather than an agent with a database password.

**Model routing for cost.** A strong reasoning model where the task needs it, a
cheap utility model everywhere else, measured per task rather than estimated per
month.

## The evaluation question

The difference between a demo and a system is that a system knows when it is
wrong. Every build carries an evaluation harness from the first week: a fixed set
of cases, an agreed measure of a good answer, and a record of the score over
time. When outputs cannot be checked automatically, we build the human review
step into the workflow rather than pretending the problem does not exist.

Guardrails, refusal behaviour, human in the loop on anything consequential, and
prompt injection treated as a security issue rather than a curiosity. An agent
with tool access is a system with permissions, and it gets reviewed like one.

## What it costs to run

The production cost estimate is a deliverable of the prototype phase, not a
surprise afterwards. It covers inference, retrieval, storage and the orchestration
layer, at your expected volume, with the scale-to-zero option costed alongside the
always-on one.

## Where this does not apply

If the process is deterministic, a language model is the expensive way to do it.
A rules engine or a few hundred lines of Python will be cheaper, faster and easier
to debug, and we will say so. The most valuable outcome of a discovery workshop is
sometimes the discovery that the AI part was decoration.

## Related

[Proof of concept](/engagements/proof-of-concept/) is the usual first commitment.
[AWS and Bedrock](/platforms/aws-and-bedrock/) covers the platform depth.
[AI governance](/services/ai-governance/) covers the documentation and risk work
that regulated buyers need alongside it. See
[Conversational GIS for Grid Analysis](/case-studies/geo-ai-platform/) for a
delivered example.
