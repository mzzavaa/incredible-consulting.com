---
title: "Serverless Video Intelligence Pipeline"
description: "Hours of raw footage turned into publishable cuts by a serverless pipeline, with layered validation to stop the agents selecting scenes that were never in the video."
weight: 43
draft: false
image: "img/mood/lens.webp"
social_image: "images/statements/type-six-validation-layers.webp"
eyebrow: "Case study"
headline_2: "Six checks before publication."
client: "Media and events workload"
industry: "Media production"
status: "completed"
status_label: "Completed"
engagement_type: "Fixed-scope build"
tech: ["Lambda", "Step Functions", "Amazon Transcribe", "Amazon Rekognition", "AWS Bedrock", "FFmpeg", "Remotion", "S3"]
outcome: "Publishable cuts produced from hours of footage without a manual editing pass"
---

{{< poster src="images/statements/type-six-validation-layers.webp" alt="Real world impact, two. Six validation layers before publication. Serverless Video Intelligence Pipeline." >}}

## The problem

Event footage has a short shelf life. Hours of interviews and floor recordings are
worth something in the days after an event and very little a month later, and the
editing capacity to turn them around does not exist in that window.

The specific shape: dozens of short interviews, each asking the same question,
where the useful output is a compilation of the answers with the question shown
once. Mechanically simple, tedious at scale, and entirely dependent on knowing
what is actually said and shown in each clip.

## The pipeline

Serverless throughout, because the workload is spiky by nature: nothing for weeks,
then several hours of footage at once.

1. **Ingest.** Footage lands in object storage, which triggers the workflow. No
   server waiting for work.
2. **Transcription.** Speech to text across the whole recording, with timings, so
   later stages reason over words rather than pixels.
3. **Visual analysis.** Paginated label detection over the footage, which matters
   more than it sounds: naive implementations quietly analyse the first page of
   results and miss most of the video.
4. **Selection.** A crew of agents making the editorial decisions: which segments
   answer the question, where each answer starts and ends, and what order they go
   in.
5. **Assembly.** Cutting and concatenation, then rendering the framing, titles and
   transitions programmatically so the output is reproducible rather than
   hand-placed.
6. **Output.** Back to object storage, ready to publish.

Orchestration is a state machine rather than a chain of functions calling each
other, so a failure at stage four does not mean re-running stages one to three,
and a stuck run is visible as a stuck run.

## The validation problem

This is the interesting part. An agent asked to select the best moments from a
video will, if unconstrained, describe an excellent moment that does not exist.
Given a transcript and a request, generating a plausible timestamp is easier than
finding the real one.

The answer was layered validation before anything is assembled: every selected
segment has to correspond to a real timestamp in the transcript, the words claimed
have to be the words present, the segment boundaries have to fall inside the
recording, and the frames at those timestamps are checked for what is actually
there. A selection that fails any layer is rejected rather than corrected, because
a plausible correction is exactly the failure mode being defended against.

The general lesson transfers well beyond media: when a model selects from a
source, the selection must be verifiable against the source, and verification must
be structural rather than a second model being asked whether the first one was
right.

## Cost profile

Scale-to-zero between events. The pipeline costs nothing while idle, which is most
of the time, and the cost of a run is a function of footage length rather than of
uptime. For a workload that fires a handful of times a year this is the difference
between a viable pipeline and a video processing server nobody wants to own.

## Where this generalises

Any pipeline where a model selects from a large source and the selection must be
provably real: document extraction with a citation requirement, log analysis with
evidence, transcript-based reporting. The media part is incidental. The
verifiable-selection pattern is the deliverable.

## Related

[AI and agent systems](/services/ai-and-agents/),
[Automation](/services/automation/),
[AWS and Bedrock](/platforms/aws-and-bedrock/), and
[Production](/method/production/).
