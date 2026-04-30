# Appendix A3 — Quality Review Checklist

> **⚠ DRAFT — illustrative example.** This is an AI-generated draft intended as a possible illustration and a TODO starting point. It is not a ready-to-use instruction. Review, adapt, and validate before adopting.

## Purpose

A structured checklist for reviewing content before publication. Expands the quick-check from [05-content-quality.md](05-content-quality.md) into a comprehensive review tool. Each item links back to the principle it enforces.

## The Checklist

### 1. Valuable Information Gate (→ [02-valuable-information.md](02-valuable-information.md))

- [ ] **ChatGPT test:** Could an AI write this without our specific experience, data, or perspective? If yes → needs rework.
- [ ] **VI level check:** Does the article meet the minimum VI level required for its content type? (→ [04-content-types-and-formats.md](04-content-types-and-formats.md))
- [ ] **AVI presence:** At least one type of AVI is clearly identifiable:
  - [ ] Systematization — new framework, categorization, or structured analysis
  - [ ] Unique Knowledge — our data, insights, or perspective no one else has
  - [ ] Product Mastery — practical implementation with our product

### 2. Relevance & Depth

- [ ] **Problem fit:** The article directly addresses a problem our target audience faces
- [ ] **Timeliness:** All data, statistics, and references are current (not older than 18 months unless historical)
- [ ] **Depth:** Goes beyond surface-level — provides actionable insights, not just descriptions
- [ ] **Completeness:** No major aspects of the topic are left unaddressed

### 3. Structure & Readability

- [ ] **Logical flow:** Each section follows naturally from the previous one
- [ ] **Clear introduction:** States the problem and what the reader will gain
- [ ] **Subheadings:** Break up the text every 200–300 words
- [ ] **Paragraph length:** No paragraph longer than 5 lines on screen
- [ ] **Clear conclusion:** Summarizes key takeaways and provides a next step / CTA

### 4. Evidence & Credibility

- [ ] **Claims are backed:** Every statement of fact has a source, data point, or clear reasoning
- [ ] **Sources are credible:** No unverified blog posts or outdated reports as primary sources
- [ ] **Own data is labeled:** Internal statistics and test results are clearly marked as ours
- [ ] **External data is cited:** Industry reports and third-party data include source and date

### 5. Visual & Formatting

- [ ] **Visuals add value:** Images, diagrams, or charts illustrate key points (not decorative)
- [ ] **Screenshots are current:** Product screenshots match the current UI
- [ ] **Alt text:** All images have descriptive alt text
- [ ] **Consistent formatting:** Headings hierarchy, bold/italic usage, list formatting

### 6. Engagement & CTA

- [ ] **Reader engagement:** Article invites questions, comments, or next steps
- [ ] **Clear CTA:** The reader knows what to do next (try the feature, read related article, sign up)
- [ ] **Internal links:** Cross-references to related content on our blog
- [ ] **SEO alignment:** Title, meta description, and target keyword are set (→ [10-seo-strategy.md](10-seo-strategy.md))

### 7. Brand & Vision Alignment (→ [07-creation-principles.md](07-creation-principles.md))

- [ ] **Narrative fit:** The article supports at least one brand narrative (→ [03-narratives.md](03-narratives.md))
- [ ] **Tone consistency:** Professional but accessible; not salesy, not academic
- [ ] **Product mention is natural:** Product references feel helpful, not forced

## Scoring

| Score | Meaning | Action |
|-------|---------|--------|
| All checks pass | Ready to publish | Proceed |
| 1–2 items missing | Minor revision | Fix and re-check those items |
| 3–5 items missing | Significant revision | Return to author with specific feedback |
| 6+ items missing | Major rework | Re-evaluate the brief; consider restarting from outline |

## Before / After Examples

### Example 1: Missing Systematization

**Before (generic, no AVI):**
> "Email personalization is important. There are many ways to personalize your emails. You can use the subscriber's name, their location, or their purchase history. Personalization helps increase engagement and drive more conversions."

**After (with Systematization AVI):**
> "Email personalization operates on three distinct levels, each requiring different data and producing different results. Level 1: Variable replacement (merge tags — name, company). Level 2: Content adaptation (dynamic blocks — show different content based on segment). Level 3: Behavioral response (triggered sequences — react to individual actions in real time). Most teams plateau at Level 1 because they lack the data infrastructure for Level 2. Here's how to diagnose which level you're actually operating at, and what it takes to move up."

**What changed:** Generic advice → structured framework with clear categories, progression logic, and diagnostic value. The reader gets a mental model, not just tips.

### Example 2: Missing Unique Knowledge

**Before (could be written by anyone):**
> "A/B testing your subject lines can improve your open rates. Try testing different lengths, emojis, and personalization tokens."

**After (with our unique data):**
> "We tested subject line personalization across 1.2M emails in Q4 2024. Adding {{first_name}} improved open rates by 12% in B2C segments but only 3% in B2B. The surprise: subject lines with a specific number ('5 templates for...') outperformed personalized ones by 8% in B2B. Our takeaway: personalization type must match the audience's decision mode — emotional (B2C) vs. analytical (B2B)."

**What changed:** Generic advice → specific data from our experiments with exact numbers, segmented insights, and a non-obvious conclusion.

### Example 3: Missing Product Mastery

**Before (product mentioned but not shown):**
> "Stripo allows you to create dynamic content blocks. This feature helps you personalize emails for different segments."

**After (with implementation guidance):**
> "To create a dynamic content block in Stripo: (1) select any module in your template, (2) click the Conditions icon in the module settings panel, (3) set the visibility condition — e.g., 'Show only if {{loyalty_tier}} = Gold.' The block will display for Gold-tier subscribers and hide for everyone else. For fallback: duplicate the module, set the opposite condition, and populate with default content. This ensures every recipient sees a complete email. Here's what this looks like in practice: [screenshot of the Stripo editor with a configured condition panel]."

**What changed:** Feature mention → step-by-step implementation with specific UI references, a practical pattern (fallback via duplication), and visual proof.

---

## TODO

- [ ] Validate with real content team — are there missing checks?
- [ ] Add product-specific checks for Stripo / Yespo / Claspo
- [ ] Create a scoring spreadsheet or Notion template
- [ ] Define who performs the review and turnaround time expectations
