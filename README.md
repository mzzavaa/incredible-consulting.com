# incredible-consulting.com: Commercial Consulting Arm

**Domain:** incredible-consulting.com
**Role:** Consulting · Commercial delivery arm of the Incredible group (canonical consulting domain)
**Priority:** Phase 1
**Strategy doc:** internal, not linked from here

## What Incredible Consulting is

An independent AI and cloud consulting practice, based in Austria, working across
the DACH region and the EU. It is founder-led: Linda Mohamed is the founder and
the named lead on every engagement, with an associate network of independent
specialists brought in by name when a project needs depth she does not carry
herself.

The practice sells three things, in this order of frequency:

1. **Facilitated workshops** that turn a vague ambition into a goal, a ranked set
   of use cases, a technical concept and a costed roadmap.
2. **Prototypes and proofs of concept** built on the client's own data, with an
   evaluation harness and a production cost estimate attached.
3. **Delivery and leadership** on the way to production: architecture,
   automation, data platforms, audits, retainers and fractional leadership.

It does not sell staff augmentation, unmanaged offshore delivery, or decks.

The positioning line the group uses is "most consulting firms sell capacity, we
sell mastery". The vocabulary that follows from it, Guilds for disciplines and
Masters for the people, is display language over content directories that keep
their plain names. See `data/guilds.yaml` and `data/masters.yaml`.

## Who delivers

Linda Mohamed: more than twelve years in software development and IT, six of
them building on cloud and AI and ML, six inside enterprise IT consulting before
going independent. AWS Community Hero, AWS User Group Vienna organiser, active in
the Förderverein AWS Community DACH. German and English. Deepest on AWS,
comfortable on hybrid and self-hosted, honest about where Azure and Google Cloud
depth comes from the network rather than from her.

The full profile is `content/team/linda-mohamed.md`, rendered by
`layouts/team/page.html`. The roster is `data/masters.yaml`, and it holds exactly
one entry on purpose: an invented second name would defeat the point of the
model. The admission standard for new Masters, and how associates are contracted,
is `content/team/network.md`.

The personal CV, speaking record and writing are **not** reproduced here. They
live on the personal site and the profile links out to them.

## What it costs

Published on the site rather than hidden behind a form, and taken from the 2026
intro deck. All figures net, excluding VAT, valid for 2026.

| Unit | Price |
|---|---|
| Workshop session, 2 to 4 hours, including preparation and documentation | about EUR 2,000 |
| Result document or artefact, including one feedback round | about EUR 1,000 |
| Hourly, for ad hoc consulting, deep dives and reviews | EUR 250 |
| Discovery package, 1 session and 2 results | about EUR 4,000 |
| Concept package, 1 session and 3 results | about EUR 5,000 |
| Prototype package, 2 sessions and 3 results | about EUR 7,000 |
| Comprehensive package, 4 sessions and 8 results | about EUR 16,000 |

Prices assume up to 5 participants per workshop and 1 to 3 use cases per result
document. Cloud provider funding, cash contributions of up to about EUR 10,000
per proof of concept and EUR 50,000 to EUR 500,000 for migration programmes, is
covered on `/pricing/funding/` and is checked during scoping rather than sold as
an extra.

If any of these numbers change, they change in `content/pricing/` and in this
table together. A price stated in one place and not the other is a bug.

## The method

Three workshops, then four delivery phases.

- **Workshop 1, goal and impact, 1 to 3 hours.** Goals, requirements and use
  cases. Output: goal definition and use cases with their users.
- **Workshop 2, data and feasibility, 2 to 4 hours.** Define the prototype from
  managed services, identify and test the data. Output: technical concept, or a
  recorded demo.
- **Workshop 3, need and implementation, 1 to 2 hours.** Cost estimate for
  infrastructure and operation, with ROI analysis. Output: demo result and a
  roadmap with costs.

Then discovery, prototype, production, handover, with a go or stop decision
between each. The results ladder the whole site is organised around is: clarity,
concept, prototype or demo, MVP or proof of concept, functional product. The
first three rungs are what the packages deliver; the last two are built with the
client's team or an implementation partner. That boundary is stated on the site
because it is where most consulting promises quietly break.

The frameworks behind the method are published openly on
incredible-consulting.org. This site describes the method as a commercial
promise and links there rather than republishing it.

## Key Features / Sections

- Services across four pillars: AI and agents, cloud architecture, automation, data platforms, plus AI governance
- Engagement models: workshop series, proof of concept, fractional leadership, architecture audit, retainer
- Industries: energy and utilities, financial services, manufacturing and logistics, public sector
- Case studies with outcomes stated before technology, backed by `data/results.yaml`
- The delivery method, three workshops and four phases
- Team, associate network, and the named lead on every engagement
- Published pricing, packages, rate card, cloud funding, and a procurement pack
- FAQ covering delivery, commercials, and security
- Contact: a free 30 minute idea call and a structured proposal request

## Monetization

Direct lead generation for paid consulting engagements. Sessions, results,
packages, project work, retainers, and fractional leadership. This is the
commercial centre of the portfolio; every other Incredible domain routes
qualified consulting demand here.

## Content map

```
content/
  _index.md                        Homepage. Carries the hero and founder band params
  services/
    _index.md                      Service catalogue
    ai-and-agents.md
    cloud-architecture.md
    automation.md
    data-platforms.md
    ai-governance.md
  engagements/
    _index.md                      Model comparison
    workshop-series.md             COPY. Modules and first-workshop agenda
    proof-of-concept.md
    fractional-leadership.md
    architecture-audit.md
    retainer.md
  industries/
    _index.md
    energy-and-utilities.md
    financial-services.md
    manufacturing-and-logistics.md
    public-sector.md
  case-studies/
    _index.md
    geo-ai-platform.md
    automation-hub.md
    video-intelligence-pipeline.md
  method/
    _index.md                      COPY. Three workshops, results ladder, four phases
    discovery.md
    prototype.md
    production.md
    handover.md
  platforms/
    _index.md                      Stack and vendor position
    aws-and-bedrock.md
    hybrid-and-open-source.md
    developer-platforms.md
  team/
    _index.md                      COPY. How an engagement is staffed
    linda-mohamed.md               COPY. The Master profile
    network.md                     COPY. Associates, and joining the roster
  pricing/
    _index.md                      COPY. Sessions, results, hours
    packages.md                    COPY. The four packages
    rate-card.md                   COPY. Rates, terms, cancellation
    funding.md                     COPY. Cloud funding and credits
    procurement.md
  faq/
    _index.md
    delivery-and-scope.md
    pricing-and-contracts.md
    security-and-compliance.md
  contact/
    _index.md
    book-a-call.md                 COPY. The free 30 minute idea call
    request-a-proposal.md
  legal/
    _index.md
    imprint.md
    privacy.md

data/
  site.yaml                        Per-site identity read by the theme
  guilds.yaml                      Display vocabulary. Every url must resolve
  masters.yaml                     The roster. Real, named, consenting people only
  engagements.yaml                 Engagement model schema
  case-studies.yaml                Delivered work schema
  results.yaml                     Headline metrics, each traceable to an engagement
  comparison.yaml                  Traditional consulting versus this
  process.yaml                     The four homepage steps
  testimonials.yaml                Empty on purpose. See the note in the file

layouts/
  home.html                        Homepage composition, including the founder band
  team/page.html                   Master profile: portrait, facts, stat band, prose

assets/
  images/                          Photographs, processed by Hugo. See below
```

## Copy status

Pages marked COPY in the map above carry finished, visitor-facing copy. The rest
are still briefs: a spec of what the page must contain, in the four-part format
described in the portfolio `CLAUDE.md`. Briefs render in development inside a
marked `.spec` block and are suppressed in production builds, so an unfinished
page shows its hero and its metadata and nothing pretending to be copy.

To finish a page, replace the brief body with real prose. Nothing else changes:
the same template renders both.

## Images

`assets/images/` holds real photographs of a real person. They are processed by
Hugo into WebP at several widths, so nothing above about 2600px on the long edge
belongs here.

| File | Ratio | Used by |
|---|---|---|
| `linda-mohamed-portrait.jpg` | 4:5 | `/team/linda-mohamed/` portrait slot |
| `linda-mohamed-vienna.jpg` | 16:9 | Homepage founder band |
| `linda-mohamed-community-day.jpg` | 3:2 | `/team/linda-mohamed/` documentary figure |

Provenance: all three are frames from the founder's own 2026 intro deck,
colour graded to sit on the near-black canvas and not otherwise altered. They are
her own photographs, published with her knowledge, which is the standard the
group `IMAGE-BRIEF.md` sets: generated portraits are acceptable as a design
placeholder and misleading as published content. Do not replace these with
generated faces.

Composition constraint: the hero scrim is opaque on the left, so a photograph
used as a hero background must put its subject on the right. All three of these
put the subject left of frame, which is why two of them render as contained,
captioned figures and none of them is a page hero. The remaining image slots on
the site render their written specification instead of a grey box, so a missing
photograph stays visible and gets commissioned deliberately.

## Relationship to other Incredible domains

- **incredible-company.com** is the group parent. Corporate identity, group story, and anything about the holding brand lives there, not here. Linked from the footer and from /legal/.
- **incredible-consulting.org** publishes the open methodology and the public-good work. This site links out to it from /method/ and /services/ai-governance/ instead of republishing the method in the open.
- **incredibleconsulting.org** is a defensive typo-catch domain with a minimal landing page. It should redirect or point here as the canonical consulting site.
- **incredible.builders** is the practitioner and open source community. Open source projects, community contributions, and hands-on builder content belong there; this site links to it from /platforms/ and /team/network/.
- **incredible.community** owns people, events, and membership. Meetups, user groups, and community programmes are linked, never duplicated here.
- **incredible.training** owns commercial learning and enablement. When the need is skills rather than delivery, /engagements/workshop-series/ and /method/handover/ hand the visitor over there.
- **lindamohamed.work** remains the personal portfolio: speaking, writing, and the individual track record. /team/linda-mohamed/ links to it rather than reproducing it.

## Conventions

- No em-dashes anywhere in this repository. Use a comma, colon, semicolon, parentheses, or two sentences.
- No emojis in content, config, layouts, README, or CSS.
- Middle dots as separators are fine: "Consulting · Vienna · AI and Cloud".
- Voice: direct, concrete, practitioner-level. No hype, no marketing filler.
- Numbers over adjectives. Name the constraint. State what an offer does not include.
- Say the price, or say why there is no price. This site says the price.
- No client names or logos without written permission. `logos` in `content/_index.md` and `data/testimonials.yaml` are empty for that reason and the sections do not render while they are.
- Theme colours are near-black and brass: see `themes/incredible/assets/css/tokens.css`. Note the mismatch with the green palette comment in `hugo.toml` and the portfolio `CLAUDE.md`; the theme tokens are what actually renders. Resolve the two rather than copying either one further.

## Local development

```
make dev      # hugo server with drafts, first free port from 1313
make build    # hugo --gc --minify --panicOnWarning
make check    # strict build to a temp dir, prints OK or FAIL
make clean    # remove public, resources/_gen, .hugo_build.lock
```

The theme is a git submodule. After cloning:

```
git submodule update --init --recursive
```
