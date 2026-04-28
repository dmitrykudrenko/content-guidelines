# Appendix A1 — Content Maturity Map

> Status: `DRAFT`

## What is a Content Maturity Map

A Content Maturity Map is a structured roadmap for developing a topic from initial ideas (notes) to a comprehensive eBook. It tracks:

- **Topic tree** — how a broad topic breaks into sections and individual content pieces
- **Maturity stage** — where each piece sits on the evolution ladder (→ [08-content-evolution.md](08-content-evolution.md))
- **Enrichment markers** — what has been added to elevate quality and VI level
- **Overall progress** — how close the topic is to becoming a complete eBook

This is the operational tool that makes the Principle of Evolution (→ [07-creation-principles.md](07-creation-principles.md)) actionable.

## Maturity Stages

| Stage | Code | What it means |
|-------|------|--------------|
| Idea | `IDEA` | Topic identified, no content created yet |
| Note | `NOTE` | A complete thought published — initial take on a subtopic |
| Article | `ARTICLE` | Several notes combined into a structured, comprehensive piece |
| Scaling | `SCALING` | Article adapted for multiple channels and/or updated with fresh data |
| Product | `PRODUCT` | Content enriched with product implementation, own case studies, internal data |
| eBook | `EBOOK` | Comprehensive compilation of all materials on the topic |

## Enrichment Markers

Each content piece should be tracked against these enrichment dimensions:

| Marker | Code | What it means |
|--------|------|--------------|
| Statistics & data | `STATS` | Contains industry data, benchmarks, or quantitative evidence |
| Expert quotes | `QUOTES` | Includes quotes or insights from industry experts or thought leaders |
| Product examples | `PRODUCT_EX` | Shows how to implement using our product (screenshots, steps) |
| External case studies | `EXT_CASES` | References success stories or data from other companies |
| Own case studies | `OWN_CASES` | Includes our own experiments, A/B tests, or client results |
| Visual assets | `VISUALS` | Has custom diagrams, infographics, or illustrations |
| Cross-references | `XREFS` | Links to related content within our ecosystem |

Enrichment markers map directly to AVI types (→ [02-valuable-information.md](02-valuable-information.md)):

- **Systematization** ← clear structure, visual assets, cross-references
- **Unique Knowledge** ← own case studies, expert quotes, original statistics
- **Product Mastery** ← product examples, own case studies

## Structure: Notes Feed Into Articles

The key principle: **an article is not written from scratch — it grows from 3+ notes** that explore the topic from different angles. The maturity map must show this hierarchy:

```
Section
  └── Article (combines notes into a structured whole)
        ├── Note 1 (angle A) ← absorbed into article
        ├── Note 2 (angle B) ← absorbed into article
        └── Note 3 (angle C) ← still standalone, pending
```

Each note explores one facet of the article's topic. Once 3+ notes exist and cover the topic sufficiently, they are combined ("absorbed") into an article. The note titles get crossed out to show they've been incorporated, but remain visible for traceability.

**Stages of a note within an article:**
- `IDEA` — topic identified, not written yet
- `NOTE` — published as a standalone note
- `DONE` — absorbed into the parent article (crossed out in the map)

**Stages of an article:**
- `ARTICLE` — notes combined into a structured piece
- `SCALING` — adapted for multiple channels, updated with fresh data
- `PRODUCT` — enriched with product implementation, own cases, internal data

## Template

### Topic: [TOPIC NAME]

**Target:** eBook / Product-level article / Article series
**Owner:** [Name]
**Timeline:** [Start] → [Target completion]

#### Section 1: [Section Name]

**Article: [Article Title]** — Stage: `[STAGE]`
Enrichments: Stats [_] | Quotes [_] | Product [_] | Ext. cases [_] | Own cases [_] | Visuals [_]
← 3 notes → article:

| # | Note Title | Stage | Absorbed? |
|---|-----------|-------|-----------|
| 1 | [Note exploring angle A] | `DONE` | ✓ |
| 2 | [Note exploring angle B] | `DONE` | ✓ |
| 3 | [Note exploring angle C] | `NOTE` | pending |

**Article: [Article Title]** — Stage: `[STAGE]`
Enrichments: Stats [_] | Quotes [_] | Product [_] | Ext. cases [_] | Own cases [_] | Visuals [_]
← 3 notes → article:

| # | Note Title | Stage | Absorbed? |
|---|-----------|-------|-----------|
| 1 | [Note] | `IDEA` | - |
| 2 | [Note] | `IDEA` | - |
| 3 | [Note] | `IDEA` | - |

#### eBook Target

| Criteria | Status |
|----------|--------|
| All articles at `PRODUCT` stage | ☐ |
| At least 5 own case studies total | ☐ |
| Visual assets for every section | ☐ |
| Expert review completed | ☐ |
| Design and layout ready | ☐ |

## Transition Criteria

When is a piece ready to move to the next stage?

### Idea → Note
- [ ] Core thesis formulated
- [ ] At least one type of AVI present
- [ ] Published (Principle of Publishing — don't hold back)

### Note → Article
- [ ] 3–5 notes on the topic exist
- [ ] Combined into a structured outline
- [ ] At least 2 enrichment markers filled
- [ ] Reviewed by a peer

### Article → Scaling
- [ ] Adapted for at least 2 additional channels (social, newsletter, webinar, etc.)
- [ ] Updated with fresh statistics or examples since original publication
- [ ] Cross-referenced with related articles

### Scaling → Product
- [ ] Product implementation section added (how-to with screenshots)
- [ ] At least 1 own case study or A/B test result
- [ ] Internal statistics included
- [ ] Reviewed by product team

### Product → eBook
- [ ] All sections of the topic at Product stage
- [ ] External validation (expert quotes, industry cases)
- [ ] Comprehensive visual assets
- [ ] Professional design and layout
- [ ] Regular update schedule defined

## Filled Example

### Topic: Email Personalization

**Target:** eBook
**Owner:** M. Writer
**Timeline:** Q1 2025 → Q3 2025

#### Section 1: Understanding personalization

**Article: Types of personalization in email marketing** — Stage: `SCALING`
Enrichments: Stats [✓] | Quotes [✓] | Product [✓] | Ext. cases [✓] | Own cases [_]
← 3/3 notes absorbed:

| # | Note Title | Stage | Absorbed? |
|---|-----------|-------|-----------|
| 1 | ~~Basic personalization: merge tags and variables~~ | `DONE` | ✓ |
| 2 | ~~Dynamic content: conditions and visibility rules~~ | `DONE` | ✓ |
| 3 | ~~AI-driven personalization: predictions and recommendations~~ | `DONE` | ✓ |

**Article: Personalization vs. segmentation: clearing the confusion** — Stage: `ARTICLE`
Enrichments: Stats [✓] | Quotes [✓] | Product [_] | Ext. cases [_] | Own cases [_]
← 2/3 notes absorbed, 1 pending:

| # | Note Title | Stage | Absorbed? |
|---|-----------|-------|-----------|
| 1 | ~~Why marketers confuse personalization with segmentation~~ | `DONE` | ✓ |
| 2 | ~~Segmentation as a foundation for personalization~~ | `DONE` | ✓ |
| 3 | When segmentation is enough and when you need personalization | `NOTE` | pending |

#### Section 2: Technical implementation

**Article: Merge tags and dynamic blocks in Stripo** — Stage: `PRODUCT`
Enrichments: Stats [✓] | Quotes [_] | Product [✓] | Ext. cases [_] | Own cases [✓]
← 3/3 notes absorbed:

| # | Note Title | Stage | Absorbed? |
|---|-----------|-------|-----------|
| 1 | ~~How merge tags work across ESPs~~ | `DONE` | ✓ |
| 2 | ~~Building reusable dynamic modules~~ | `DONE` | ✓ |
| 3 | ~~Fallback values: what to show when data is missing~~ | `DONE` | ✓ |

**Article: AMP for email: real-time personalization** — Stage: `NOTE`
Enrichments: Stats [_] | Quotes [_] | Product [_] | Ext. cases [_] | Own cases [_]
← 1/3 notes written, 2 ideas:

| # | Note Title | Stage | Absorbed? |
|---|-----------|-------|-----------|
| 1 | What AMP emails can do that HTML can't | `NOTE` | - |
| 2 | Real-time content: live pricing, inventory, polls | `IDEA` | - |
| 3 | AMP adoption barriers and workarounds | `IDEA` | - |

#### Section 3: Results and measurement

**Article: Our A/B test results: personalized vs. generic emails** — Stage: `PRODUCT`
Enrichments: Stats [✓] | Quotes [_] | Product [✓] | Ext. cases [_] | Own cases [✓]
← 3/3 notes absorbed:

| # | Note Title | Stage | Absorbed? |
|---|-----------|-------|-----------|
| 1 | ~~Test setup: what we measured and how~~ | `DONE` | ✓ |
| 2 | ~~Subject line personalization: +18% open rate~~ | `DONE` | ✓ |
| 3 | ~~Content personalization: impact on click-through~~ | `DONE` | ✓ |

**Article: Personalization ROI: industry benchmarks** — Stage: `ARTICLE`
Enrichments: Stats [✓] | Quotes [✓] | Product [_] | Ext. cases [✓] | Own cases [_]
← 2/3 notes absorbed, 1 pending:

| # | Note Title | Stage | Absorbed? |
|---|-----------|-------|-----------|
| 1 | ~~What reports say: McKinsey, Litmus, HubSpot data~~ | `DONE` | ✓ |
| 2 | ~~ROI by personalization type: basic vs. advanced~~ | `DONE` | ✓ |
| 3 | Cost of personalization: tools, data, team time | `NOTE` | pending |

#### eBook Target

| Criteria | Status |
|----------|--------|
| All articles at `PRODUCT` stage | ☐ (2/6) |
| At least 5 own case studies total | ☐ (2/5) |
| Visual assets for every section | ☐ (0/3) |
| Expert review completed | ☐ |
| Design and layout ready | ☐ |

---

## TODO

- [ ] Create a maturity map for 1 real Stripo topic as a pilot
- [ ] Create a maturity map for 1 real Yespo topic as a pilot
- [ ] Define who maintains and updates the maps
- [ ] Decide on a tool for tracking (Notion / spreadsheet / this md format)
