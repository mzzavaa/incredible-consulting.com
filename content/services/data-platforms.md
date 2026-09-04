---
title: "Data Platforms"
description: "Pipelines, storage and modelling that make data usable for analytics and for the AI systems built on top of it."
weight: 14
draft: false
image: "img/mood/prism.webp"
eyebrow: "Data Guild"
headline_2: "Fix the foundation first."
pillar: "data"
typical_duration: "6 to 16 weeks"
typical_deliverable: "Pipeline, modelled storage layer, quality checks, documentation"
tech: ["S3", "Glue", "Athena", "PostGIS", "Apache Iceberg", "Airflow", "dbt"]
---

Almost every stalled AI project is a data project wearing a costume. The model
works, the demo was convincing, and then it turns out the data exists in three
systems with three definitions of the same customer, refreshed nightly, monthly
and never.

This practice is the unglamorous half that makes the other half possible.

## What gets built

**Ingestion and pipelines.** Batch and streaming, orchestrated rather than
cron-scheduled, with retries and failure handling that are visible. Managed
orchestration where it fits, so the pipeline is not itself a system somebody has
to operate.

**Storage and modelling.** An open table format over object storage covers most
requirements now, and the lakehouse question can be answered plainly instead of
philosophically: keep the raw data, model the layer people query, and do not
build a warehouse for three dashboards.

**Quality and lineage.** Checks that fail visibly, and a record of where each
figure came from. A pipeline that silently produces wrong numbers is worse than
one that stops.

**Access, retention and residency.** Who can see what, how long it is kept, and
where it physically sits. For EU workloads this is a design input, not a
compliance afterthought.

## Making data AI-ready

Retrieval quality is a data problem before it is a model problem. That means
chunking that respects document structure, embeddings refreshed when the source
changes, metadata rich enough for an agent to choose the right source, and an
answer that can be traced back to the record it came from. A system that cannot
show its source will eventually invent one.

**Spatial data** is its own discipline and is one we go deep on: PostGIS,
coordinate systems that do not silently disagree, and the difference between a
query that samples sensibly across a large area and one that times out.

## Cost, from day one

Cost per query and cost per terabyte are tracked from the first week rather than
discovered later. Storage is cheap and scanning is not, and the difference is a
partitioning decision made early.

## Where this does not apply

If you have one source system, a few million rows, and a working database, you do
not need a platform. You need a query and possibly an index. We will say that
before quoting anything.

## Related

[AI and agent systems](/services/ai-and-agents/) is what usually sits on top.
[Cloud architecture](/services/cloud-architecture/) covers the layer underneath.
[Architecture audit](/engagements/architecture-audit/) is the way to get an
independent read on a platform you have inherited.
