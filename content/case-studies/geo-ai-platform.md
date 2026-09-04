---
title: "Conversational GIS for Grid Analysis"
description: "A multi-agent platform that turns complex spatial operations into plain German questions, built with a geospatial software company over a three workshop series."
weight: 41
draft: false
image: "img/mood/pantograph.webp"
social_image: "images/statements/type-days-to-minutes.webp"
eyebrow: "Case study"
headline_2: "Ask the map a question."
client: "Geospatial software platform, energy and infrastructure"
industry: "Spatial analysis · Energy and infrastructure"
status: "active"
status_label: "Active engagement"
engagement_type: "Workshop series and PoC development"
tech: ["AWS Bedrock", "AgentCore", "CrewAI", "LangGraph", "PostGIS", "MCP", "Lambda", "Python"]
outcome: "Domain experts run spatial queries without writing SQL or opening a GIS client"
---

{{< poster src="images/statements/type-days-to-minutes.webp" alt="Real world impact, one. Days to minutes. Spatial query turnaround. Conversational GIS for Grid Analysis." >}}

## The problem

Spatial analysis in energy and infrastructure is bottlenecked on a small number of
GIS specialists. A planner who wants to know which power lines in a region have
reported damage, with drone imagery attached, cannot answer that themselves. They
raise a request, it queues behind other requests, and the answer arrives days
later, by which point the question has often moved on.

The client had the data and the tooling. Field survey data, aerial imagery, public
geodata, and a mature desktop GIS with its own analysis plugins. What did not
exist was a way to ask across all of it in one question.

## The constraints

**German, not English.** The users work in German and the queries arrive in
German, including place names, regional terms and the grammatical constructions
that make naive keyword matching fail.

**Mixed sensitivity.** Public geodata is public. Customer survey data is not, and
in this sector some of it cannot leave the customer's own infrastructure.

**No invented geometry.** A language model that produces a plausible but fictional
coordinate is not a minor quality issue in grid planning. Every answer had to be
traceable to a real feature in a real dataset.

## What was built

A crew of specialised agents on a serverless agent runtime, reached through
natural language, over the client's existing spatial data.

**Query understanding.** A processing layer that reads a German question and
extracts the intent (count, export, analyse), the target objects (masts, lines,
damage reports) and any region or coordinates named in the text. Dynamically,
rather than through hardcoded phrase matching, so the vocabulary can grow without
a code change.

**Spatial analysis.** An analysis layer that adapts to the question: automatic
area calculation, feature filtering by tag, and sampling that stays sane over
large regions rather than attempting to load everything and timing out. Answers
are generated back in German.

**Visualisation.** Generated GeoJSON so results render on a map: the search area
as a polygon, matched features as points, planned routes as lines, with zoom
fitted to the area.

**A bounded tool surface.** The GIS layer is exposed to the agents through a
Model Context Protocol server rather than by giving an agent database access. The
agents can call defined operations and nothing else, which is what makes the
system reviewable.

## The hybrid decision

The workshop series did not end with a single-platform recommendation, and that
was the right answer. Public cloud is used for fast experimentation on public
geodata, where scale-to-zero means no idle infrastructure cost. Sensitive customer
data stays in private infrastructure. The design joins them: public topography
analysed in one place, private network data added in the other.

Choosing this deliberately, in a room with the people responsible for both sides,
took one workshop. Discovering it eighteen months into a migration would have
taken considerably longer.

## How it ran

Three workshops with gaps between them. The first established the strategy and a
shared technical picture. Between sessions the client's team gathered real
example data and documented which analyses were simple and which were hard.

The second was hands-on: the team brought laptops and wrote code together,
prioritising a large backlog of candidate use cases down to a handful worth
prototyping, and comparing two agent frameworks live on the actual use case
rather than arguing about them in the abstract.

The third covered return on investment, a now-next-later roadmap, and a prototype
readout per priority use case.

## What did not work first time

The first framework choice was not obviously correct, which is why the second
workshop ran the comparison as an experiment rather than accepting the initial
pick. Model size was a live question throughout: the large reasoning model gave
better German output and cost more per query than the workload could justify at
volume, which turned into a routing problem rather than a model-selection one.

## Status

Active. The use case backlog is triaged, the priority prototypes are running, and
the work is now about what has to be true to put this in front of the client's own
customers.

## Related

[AI and agent systems](/services/ai-and-agents/),
[Data platforms](/services/data-platforms/),
[Energy and utilities](/industries/energy-and-utilities/), and
[Prototype](/method/prototype/).
