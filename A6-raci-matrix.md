# Appendix A6 — Content Workflow RACI Matrix

> **⚠ DRAFT — illustrative example.** This is an AI-generated draft intended as a possible illustration and a TODO starting point. It is not a ready-to-use instruction. Review, adapt, and validate before adopting.

## Purpose

Maps team roles (→ [09-team-and-roles.md](09-team-and-roles.md)) to content evolution stages (→ [08-content-evolution.md](08-content-evolution.md)). Answers: "Who does what at each stage of content creation?"

## RACI Legend

- **R** = Responsible — does the work
- **A** = Accountable — approves the result, has final say
- **C** = Consulted — provides input before the work is done
- **I** = Informed — notified after the work is done

## Matrix: Roles × Evolution Stages

| Role | Idea / Topic selection | 01 Note | 02 Article | 03 Scaling | 04 Product | 05 eBook |
|------|----------------------|---------|-----------|-----------|-----------|---------|
| **CMO** | A | I | I | I | C | A |
| **Head of Content** | R | A | A | A | A | R |
| **Lead Content Writer** | C | C | R (review) | C | C | C |
| **J. Writer** | — | R (notes) | — | — | — | — |
| **M. Writer** | — | — | R (writing) | C | C | — |
| **S. Writer** | — | — | C | — | R (deep) | R (writing) |
| **SEO Specialist** | R (keywords) | C | C (SEO review) | R (keyword update) | C | C |
| **Designer** | — | R (visuals) | R (visuals) | R (social assets) | R (visuals) | R (layout) |
| **SMM Manager** | — | I | I | R (social channels) | R (promotion) | R (promotion) |
| **PR Manager** | — | — | — | R (guest posts, media) | C (influencers) | R (media, launch) |
| **Outreacher** | — | — | — | C | R (influencers) | R (influencers) |
| **BA** | C | — | C | — | R (product input) | C |

## Matrix: Roles × Content Processes

| Role | Brief creation | Research | Writing | Visual design | SEO review | Quality review | Publishing | Promotion |
|------|---------------|----------|---------|--------------|-----------|---------------|-----------|-----------|
| **Head of Content** | A | C | C | I | I | A | A | I |
| **Lead Content Writer** | R | C | A (review) | C | I | R | R | I |
| **Writer (assigned)** | R | R | R | C | I | I | I | I |
| **SEO Specialist** | C | R (keywords) | — | — | R | C | — | — |
| **Designer** | I | — | — | R | — | — | — | R (assets) |
| **SMM Manager** | — | — | — | C | — | — | — | R |
| **PR Manager** | — | — | — | — | — | — | — | R |

## Workflow by Stage

### 01 Note — fast cycle (1–3 days)

```
Writer (J.) writes note
  → Lead Content Writer reviews (same day)
    → Head of Content approves
      → Published
        → Designer creates social visual
          → SMM promotes
```

### 02 Article — standard cycle (1–2 weeks)

```
Head of Content assigns topic + brief
  → SEO Specialist provides keywords
    → Writer (M.) researches and writes
      → Lead Content Writer reviews content
        → SEO Specialist reviews SEO
          → Head of Content final approval
            → Published
              → Designer creates visuals
                → SMM + PR promote
```

### 04 Product — extended cycle (2–4 weeks)

```
Head of Content + BA define product angle
  → Writer (S.) researches and writes
    → Product team reviews accuracy
      → Lead Content Writer reviews content
        → Head of Content approves
          → Designer creates rich visuals
            → Published
              → Full promotion cycle (SMM + PR + Outreacher)
```

### 05 eBook — project cycle (2–4 months)

```
CMO + Head of Content approve topic
  → Head of Content coordinates overall structure
    → S. Writer compiles and writes
      → External experts review / provide quotes
        → Lead Content Writer reviews
          → Designer creates full layout
            → Head of Content final review
              → CMO approves
                → Published
                  → Full launch campaign
```

## Handoff Points — Where Things Break

Common failure points and how to prevent them:

| Handoff | Risk | Prevention |
|---------|------|-----------|
| Writer → Reviewer | Review takes too long, content sits idle | Max 2 business days for review; use async comments |
| Content → Design | Designer lacks context, creates wrong visuals | Include visual brief in the article brief (→ [A2](A2-article-brief-template.md)) |
| Content → SEO | Keywords added after writing, feel forced | SEO input BEFORE writing begins (step 1 in the workflow) |
| Article → Scaling | No one owns the adaptation, article stays on blog only | Assign scaling owner at publication time |
| Scaling → Product | Product team not involved early enough | BA + Product team consulted at brief stage for Product-level content |

---

## TODO

- [ ] Validate with actual team — are the role assignments correct?
- [ ] Adjust for Stripo / Yespo / Claspo if teams differ
- [ ] Define SLAs for each handoff (max review time, max design time)
- [ ] Integrate with project management tool (Asana / Notion / Linear)
