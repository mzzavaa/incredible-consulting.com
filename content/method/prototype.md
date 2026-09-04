---
title: "2. Prototype"
description: "Build the smallest thing that proves the answer, with an evaluation harness attached from the first week and the shortcuts written down."
weight: 52
draft: false
image: "img/mood/pour.webp"
eyebrow: "Method"
headline_2: "Turn opinion into evidence."
phase: 2
duration: "3 to 8 weeks"
output: "Working prototype, evaluation results, production cost estimate"
---

The purpose of this phase is not to impress anyone. It is to find out whether the
thing works, as cheaply as possible, and to make that finding hard to argue with.

## How it runs

**Something running, every week.** A demo of the actual system, not a status
update. Weekly cadence is a forcing function: it prevents the four-week silence
that ends in a rewrite, and it surfaces disagreements about what good looks like
while they are still cheap.

**Evaluation before optimisation.** The harness is built in week one, before the
system is any good. A fixed set of cases, an agreed definition of a correct
output, and a score recorded every run. Adding the metric at the end produces a
metric the system happens to pass.

**Real data, real constraints.** Sample data from your systems, with the awkward
records included. A prototype that only works on the clean examples has proved
nothing.

**Deliberate shortcuts, listed.** Hardcoded values, a single environment, no
authentication, one region, a manual step in the middle. All legitimate here, all
written down, so nobody later mistakes them for design.

**Your repository from the first commit.** Not a handover at the end. You can
read the code as it is written, and if the engagement ended tomorrow you would
have everything.

## The second gap

Between the build and the decision there is another deliberate pause: internal
review, testing with people who will actually use the thing, and alignment with
security, legal and operations. This is where the objection that would have
appeared two weeks before go-live appears instead with time to answer it.

## What you get

- A working prototype on your data, in your environment
- Evaluation results, including the failure cases, not only the wins
- The production cost estimate at your expected volume, produced here rather than
  guessed later
- A list of the shortcuts and what each would cost to do properly
- A go, stop, or go-with-changes recommendation against the kill criteria

## If the kill criteria are met

We say so and stop, and the remaining budget stays with you. This is written into
the engagement at the start precisely so that stopping does not require anybody to
lose an argument.

## Related

[Proof of concept](/engagements/proof-of-concept/) is the commercial wrapper.
[Production](/method/production/) is what a passing prototype leads into.
