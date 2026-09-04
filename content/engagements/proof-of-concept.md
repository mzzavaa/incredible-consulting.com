---
title: "Proof of Concept"
description: "A time-boxed build that answers one question: does this work well enough to be worth productionising, measured against a number agreed before we start."
weight: 22
draft: false
image: "img/mood/emitter.webp"
eyebrow: "Engagement model"
headline_2: "Evidence, not a demo video."
model: "proof-of-concept"
duration: "4 to 10 weeks"
price_band: "Fixed scope, fixed fee"
best_for: "Teams that need evidence before a budget cycle"
---

For sponsors who need something that survives scrutiny from engineering and from
finance in the same meeting. A proof of concept here is a working system on your
data, not a scripted demonstration.

## Agreed before anything is built

**The question.** One sentence, and it has to be answerable. "Can an agent
resolve this class of request without a human" is a question. "Explore AI
opportunities" is not.

**The success metric.** A number, and the threshold that counts as a pass. Where
the output is a judgement rather than a measurement, the metric is agreement with
a human reviewer on a fixed set of cases.

**The kill criteria.** The conditions under which the honest recommendation is to
stop. Written down at the start, when nobody is invested yet.

**What is deliberately faked.** Every proof of concept cuts corners. The list of
which ones is a deliverable, so that nobody later mistakes a shortcut for
architecture.

## How it runs

Weekly, with something running to look at each time. No month-long silences, no
big reveal at the end. Source code sits in your repository from the first commit,
not handed over at the finish. The evaluation harness is built in the first week,
before the thing being evaluated is any good, because a metric added at the end
tends to be the one the system already passes.

## What you get

- A running system in your environment
- Source code, in your repository, with a README that lets a new engineer run it
- Evaluation results against the agreed metric, including the failures
- A production cost estimate at your expected volume
- A written recommendation: go, stop, or go with these three changes first

## What happens after

If it passes, the next step is the [production phase](/method/production/):
infrastructure as code, observability, security review, and a go-live plan. That
is a separate scope with its own fixed fee, quoted once the shape of the thing is
known rather than guessed at the start.

If it fails, you have spent a defined amount to find that out, which is the
entire point. A stopped proof of concept is a successful engagement with a
disappointing answer.

## Funding

Proof of concept work frequently qualifies for cloud provider funding, including
cash contributions of up to about EUR 10,000 per proof of concept. Eligibility is
checked during scoping, before the proposal. See
[Cloud funding and credits](/pricing/funding/).

## Related

[Workshop series](/engagements/workshop-series/) is the usual step before this.
[Prototype phase](/method/prototype/) describes how the build runs.
[Packages](/pricing/packages/) covers the pre-scoped combinations.
