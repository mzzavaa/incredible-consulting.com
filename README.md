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
sell mastery". Guilds is display vocabulary for the disciplines, over content
directories that keep their plain names: see `data/guilds.yaml`.

**There is deliberately no title for the people.** An earlier version of this
site called them Masters. That was dropped: a rank is self-awarded and the work
is not, and the word read as grandiose in English while the rest of the site is
scrupulously plain. The roster admits a person on a system they shipped rather
than on a title, which is what `/team/` and `data/roster.yaml` say. The absence
of logos, testimonials and certifications follows the same rule and is a
consequence of it, not a slogan: an intermediate version of the homepage led with
that absence, and it read as defensive rather than confident. The homepage sells
the offer; the roster page carries the standard.

## Who delivers

Linda Mohamed: more than twelve years in software development and IT, six of
them building on cloud and AI and ML, six inside enterprise IT consulting before
going independent. AWS Community Hero, AWS User Group Vienna organiser, active in
the Förderverein AWS Community DACH. German and English. Deepest on AWS,
comfortable on hybrid and self-hosted, honest about where Azure and Google Cloud
depth comes from the network rather than from her.

The full profile is `content/team/linda-mohamed.md`, rendered by
`layouts/team/page.html`. The roster is `data/roster.yaml`, and it holds exactly
one entry on purpose: an invented second name would defeat the point of the
model. The standard for joining the roster, and how associates are contracted,
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

Every page below carries finished, visitor-facing copy. Pages marked CONFIRM
carry a `CONFIRM BEFORE PUBLISHING` block in their front matter listing the
specific claims that are drafted from normal practice rather than from a stated
policy. Read those blocks before the site goes live, then delete them.

```
content/
  _index.md                        Homepage. Composed in layouts/home.html, no body copy
  services/
    _index.md                      Catalogue, and the four recurring problem shapes
    ai-and-agents.md
    cloud-architecture.md
    automation.md
    data-platforms.md
    ai-governance.md
  engagements/
    _index.md                      Which model fits, and the price basis for each
    workshop-series.md             Modules and the first-workshop agenda
    proof-of-concept.md
    architecture-audit.md
    fractional-leadership.md
    retainer.md
  industries/
    _index.md                      Delivered vs transferred, stated per sector
    energy-and-utilities.md        Delivered
    manufacturing-and-logistics.md Transferred
    financial-services.md          Transferred
    public-sector.md               Adjacent
  case-studies/
    _index.md                      Includes why no client is named
    geo-ai-platform.md
    automation-hub.md
    video-intelligence-pipeline.md
  method/
    _index.md                      Three workshops, results ladder, four phases
    discovery.md
    prototype.md
    production.md
    handover.md
  platforms/
    _index.md                      Where the depth is, and the neutrality position
    aws-and-bedrock.md
    hybrid-and-open-source.md
    developer-platforms.md
  team/
    _index.md                      How an engagement is staffed, and the roster standard
    linda-mohamed.md               The founder profile
    network.md                     CONFIRM. Associates, and joining the roster
  pricing/
    _index.md                      Sessions, results, hours
    packages.md                    CONFIRM. The four packages
    rate-card.md                   CONFIRM. Rates, terms, cancellation
    funding.md                     Cloud funding and credits
    procurement.md                 CONFIRM. Entity, contracts, insurance, VAT
  faq/
    _index.md
    delivery-and-scope.md
    pricing-and-contracts.md       CONFIRM
    security-and-compliance.md     CONFIRM. States practice, claims no certification
  contact/
    _index.md                      CONFIRM. Two working day reply commitment
    book-a-call.md                 CONFIRM. The free 30 minute idea call
    request-a-proposal.md          CONFIRM. Five working day proposal turnaround
  legal/
    _index.md
    imprint.md                     Shortcode, German, discharges the ECG obligation
    privacy.md                     Shortcode. Describes a site with no cookies or forms

data/
  site.yaml                        Per-site identity read by the theme
  guilds.yaml                      Display vocabulary. Every url must resolve
  roster.yaml                      The roster. Real, named, consenting people only
  engagements.yaml                 Engagement model schema
  case-studies.yaml                Delivered work schema. Keep in sync with the pages
  results.yaml                     Headline metrics, each traceable to an engagement
  comparison.yaml                  Traditional consulting versus this
  process.yaml                     The four homepage steps
  testimonials.yaml                Empty on purpose. See the note in the file

layouts/
  home.html                        Homepage composition, including the founder band
  team/page.html                   Person profile: portrait, facts, stat band, prose

assets/
  images/                          Photographs, processed by Hugo. See below
```

## Copy status and the honesty rules

Three rules govern what may be written on these pages, and they are why several
of them read less confidently than a normal consulting site:

1. **No client is named, anywhere.** Permission has not been sought. Sector and
   workload shape are described instead, and `data/testimonials.yaml` and the
   homepage `logos` list stay empty until written approval exists.
2. **Delivered work and transferred capability are labelled differently.** The
   industry pages say which is which, out loud, in the first paragraph. Energy is
   delivered, manufacturing and financial services are transferred, public sector
   is adjacent.
3. **A number that cannot be traced to a named engagement does not ship.** This is
   why two of the three headline metrics in `data/results.yaml` are phrases rather
   than figures.

The `CONFIRM BEFORE PUBLISHING` blocks are the fourth rule in practice: where a
page needed a commercial or security answer that no source material supplied, the
answer was drafted from normal practice and flagged in place rather than quietly
invented. Grep for them before launch:

```
grep -rn "CONFIRM BEFORE PUBLISHING" content/
```

## Images

Three libraries, in two places, for three different jobs.

### 1. The mood library, shared

`themes/incredible/assets/img/mood/` holds 26 text-free brand images, near-black
with one brass light source. They live in the theme so every site in the family
draws on the same set, and they are documented image by image, with the subject
position of each, in
[the library README](themes/incredible/assets/img/mood/README.md).

Every page on this site sets one as its hero:

```
image: "img/mood/prism.webp"
```

**The composition rule that governs the choice:** the hero scrim is opaque on the
left, because the headline sits there. A hero image must put its subject on the
right or in the centre. `tools.jpg` is the one image in the set with a left-hand
subject; it is for figures, never for a hero.

### 2. The statement library, this site only

`assets/images/statements/` holds 34 images with wording baked into the pixels,
in three visual treatments: `line-` (gold line art), `photo-` (brass still life),
`type-` (typographic). Their words are specific to this domain, which is why they
are not in the shared theme.

Baked-in text is an accessibility cost, so it is spent deliberately in exactly
two places:

- **Social cards.** `social_image` in front matter, resolved by the theme's
  `head.html` into `og:image`. A share preview is an image, so an image that
  carries the message is the right tool. Pages without one fall back to their
  hero, and the site default is in `data/site.yaml`.
- **Seven on-page posters,** through `layouts/shortcodes/poster.html`. The
  shortcode refuses to build without `alt`, and the alt must transcribe the
  wording in full. A poster may only be used where the page does not print the
  same words beside it: it makes a claim the page then explains.

Posters are on `/services/`, `/method/`, and each of the three case studies.
Unused statement images stay in the library on purpose. Eight are deliberately
not used, and the reason matters more than the list:

- `line-independent-masters.jpg`, `photo-independent-masters.jpg`,
  `type-independent-masters.jpg` and `photo-the-assembly.jpg` print
  "Independent Masters" or "Independent masters" in the artwork. That vocabulary
  was retired: see the first section of this README.
- `line-challenge-to-impact.jpg` and `photo-challenge-to-impact.jpg` print "We
  find the right Masters" in the process step. `type-challenge-to-impact.jpg`
  prints "specialists" in the same slot and is used instead, on `/method/`.
- `type-seven-guilds.jpg` shows Security and Transformation guilds, which have no
  pages, see `data/guilds.yaml`.
- The `days-to-minutes` variants that print "Spatial analytics platform"
  contradict the client descriptor now used on the case study.
- `photo-right-expertise.webp` and `type-uncover-the-impossible.webp` print
  "Request an introduction", which was the booking button's label until it became
  "Book an idea call". `photo-right-expertise.webp` was also the same photograph
  as the `/contact/` hero, so that page was showing one picture twice.

This is the standing cost of baked-in text: a wording decision orphans artwork.
Weigh that before adding a statement image to a new page.

### 3. The founder photographs

`assets/images/` holds three real photographs of a real person.

| File | Ratio | Used by |
|---|---|---|
| `linda-mohamed-portrait.jpg` | 4:5 | `/team/linda-mohamed/` portrait slot |
| `linda-mohamed-vienna.jpg` | 16:9 | Homepage founder band, and her social card |
| `linda-mohamed-community-day.jpg` | 3:2 | `/team/linda-mohamed/` documentary figure |

Provenance: frames from the founder's own 2026 intro deck, colour graded to sit
on the near-black canvas and not otherwise altered. Do not replace these with
generated faces. The mood and statement libraries are rendered brand imagery, not
photographs of real places or people; their source is the Engineering Mastery
deck series of September 2026.

All three libraries are processed by Hugo into WebP at several widths, so nothing
above about 2600px on the long edge belongs in any of them. Masters are 1376 by
768 and are stored as JPEG because they are photographic.

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
