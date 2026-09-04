---
title: "4. Handover"
description: "Your team owns the system: documentation, a recorded walkthrough, an ownership map, and a support tail with a defined end."
weight: 54
draft: false
image: "img/mood/key.webp"
eyebrow: "Method"
headline_2: "How we leave."
phase: 4
duration: "1 to 3 weeks, plus optional support tail"
output: "Documentation, runbook, recorded walkthrough, training session, ownership map"
---

Most consultancies describe how they arrive. This page describes how they should
leave, because the exit is the part that determines whether the work was worth
anything in twelve months.

## What is handed over

**The documentation set.**

- Architecture, at the level someone new can navigate
- Decision records: what was chosen, what was rejected, and why. This is the
  document that matters most in a year, when the reasons have been forgotten and
  someone is about to undo a decision without knowing what it was protecting
- A runbook covering the failures we have already seen
- Known limitations, stated plainly, including the ones we would fix with more
  time

**A live walkthrough, recorded.** With the receiving team, in their environment,
where they drive and we watch. Questions get answered while the person who built
it is still in the room, and the recording is there for the engineer who joins in
six months.

**An ownership map.** Every component with a named owner on your side. A component
without an owner is an outage waiting for a calendar slot.

## The support tail

Optional, and if taken, bounded. A defined number of weeks at a defined level: we
answer questions and fix things we broke. We do not add features during it, and we
do not quietly become the operations team. The end date is in the agreement from
the start.

## What we take with us

Nothing that should stay. Credentials are revoked on the last day and we confirm
that in writing. Your code, your infrastructure definitions, your data. Where we
have used a pattern or a component of our own, it is handed over under terms that
let you keep using and changing it, and those terms are in the statement of work
rather than discovered later.

## If the team needs skills rather than notes

Handover transfers a system. It does not transfer a capability the team never had.
When the receiving team needs to learn the discipline rather than the codebase,
that is training, and it is run on
[incredible.training](https://incredible.training/) rather than stretched out of a
handover session.

## If you want a senior voice afterwards

That is a [retainer](/engagements/retainer/), bought deliberately, rather than a
handover that never quite finishes.

## Related

[Production](/method/production/) is the phase before this.
[Who does the work](/team/) covers who does the handover, which is the same person who did
the build.
