---
title: "Multi-Agent Automation Hub"
description: "A conversational orchestration layer routing operational work to specialised agent crews on AWS."
weight: 42
draft: false
client: "Internal product, offered as a reference build"
industry: "Professional services operations"
status: "active"
status_label: "In production"
engagement_type: "Proof of concept into production"
tech: ["AWS Bedrock", "AgentCore", "CrewAI", "Terraform", "CodeBuild", "Claude"]
outcome: "Recurring back-office work handled by agents with a single conversational entry point"
---

**Purpose.** Shows what an agent platform looks like once it stops being a demo: infrastructure as code, CI/CD, and cost control.

**Contains.**
- The problem: five unrelated operational workflows, each half automated
- The architecture: one runtime, several specialised crews, one orchestration agent
- Deployment: Terraform and a build pipeline, not a notebook
- Cost per task and how model routing keeps it down
- What broke first and what we changed
- How the same pattern maps onto a client estate

**Primary CTA.** Ask how this maps to your operations.
**Links to.** /services/automation/, /industries/manufacturing-and-logistics/, /engagements/proof-of-concept/.
