# incredible-consulting.com: Commercial Consulting Arm

**Domain:** incredible-consulting.com
**Role:** Consulting · Commercial delivery arm of the Incredible group (canonical consulting domain)
**Priority:** Phase 1
**Strategy doc:** internal, not linked from here

## Purpose
The revenue site. Where AI, cloud, automation, and data consulting is actually sold to CTOs, heads of data and platform, and innovation leads with a budget. It mirrors the depth of the personal services page on lindamohamed.work, but written for a company rather than an individual, and it ends every path at a booked call.

## Key Features / Sections
- Services across four pillars: AI and agents, cloud architecture, automation, data platforms
- Engagement models: workshop series, proof of concept, fractional leadership, architecture audit, retainer
- Industries: energy and utilities, financial services, manufacturing and logistics, public sector
- Case studies with outcomes stated before technology, backed by `data/results.yaml`
- The delivery method in four phases: discovery, prototype, production, handover
- Team, associate network, and the named lead on every engagement
- Published pricing bands, fixed-fee packages, and a procurement pack
- FAQ covering delivery, commercials, and security
- Contact: booking calendar and a structured proposal request

## Monetization
Direct lead generation for paid consulting engagements. Fixed-fee packages, project work, retainers, and fractional leadership. This is the commercial centre of the portfolio; every other Incredible domain routes qualified consulting demand here.

## Content map

```
content/
  _index.md                        Homepage
  services/
    _index.md                      Service catalogue
    ai-and-agents.md
    cloud-architecture.md
    automation.md
    data-platforms.md
    ai-governance.md
  engagements/
    _index.md                      Model comparison
    workshop-series.md
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
    _index.md                      How we deliver
    discovery.md
    prototype.md
    production.md
    handover.md
  platforms/
    _index.md                      Stack and vendor position
    aws-and-bedrock.md
    hybrid-and-open-source.md
  team/
    _index.md
    linda-mohamed.md
    network.md
  pricing/
    _index.md
    packages.md
    rate-card.md
    procurement.md
  faq/
    _index.md
    delivery-and-scope.md
    pricing-and-contracts.md
    security-and-compliance.md
  contact/
    _index.md
    book-a-call.md
    request-a-proposal.md
  legal/
    _index.md
    imprint.md
    privacy.md

data/
  engagements.yaml                 Engagement model schema, 3 seeded entries
  case-studies.yaml                Delivered work schema, 3 seeded entries
  results.yaml                     Headline metrics schema, 3 seeded entries
```

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
- Brand palette: green #3D8F37, dark #0a1a08, white #fff, background #f8f9f6. Font: Inter.
- Every page body is a brief, a short spec of the page, not finished copy. A later pass turns briefs into copy.

## Local development

```
make dev      # hugo server on the first free port from 1313
make build    # hugo --gc --minify
make clean    # remove public, resources/_gen, .hugo_build.lock
```
