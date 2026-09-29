# Appendix A8 — AI Content Labeling Rules

> **⚠ DRAFT — not legal advice.** This appendix translates the EU AI Act transparency duties into an editorial workflow. It needs Legal sign-off before it becomes binding. Edge cases go to Legal, not to this file.

## Purpose

A decision system for one question: **does this piece of content need an AI disclosure, and in what form?**

It covers:

- **Classification** — which of 8 classes a piece falls into
- **Disclosure markers** — what must be attached to it before publishing
- **Channel rules** — exact placement and wording per channel

This sits at the end of the writing process, next to the quality gate (→ [06-writing-process.md](06-writing-process.md), [A3-quality-review-checklist.md](A3-quality-review-checklist.md)).

Channel rules below are written for **Stripo** (blog, landing pages, YouTube, webinars). The classes, markers and decision tree are product-agnostic and apply to Yespo and Claspo as-is; only the channel section needs adaptation.

Applies from **2 August 2026** (EU AI Act, Article 50).

---

## Two rules that decide almost everything

1. **EU law does not require a label on every piece of content touched by AI.** It requires disclosure in specific situations: direct AI interaction, realistic synthetic media, deepfakes, and unreviewed public-interest text.
2. **Substantive human review removes the public-interest text obligation.** It does *not* remove the deepfake obligation or the machine-readable provenance obligation.

Almost all blog and landing content is AI-assisted and human-edited marketing content → in most cases **no public-facing label is required**. The real exposure sits in **realistic imagery, voice cloning, AI avatars, and AI dubbing** — that is, YouTube and webinars.

---

## Roles: where we sit

| Role | Who | What it triggers |
|---|---|---|
| **Deployer** | Content, PR, video, design teams — everyone publishing with AI tools (→ [09-team-and-roles.md](09-team-and-roles.md)) | Deepfake disclosure, public-interest text disclosure, biometric/emotion notices |
| **Provider** | Product teams shipping AI features to users (AI assistant, AI-generated templates) | "You are interacting with AI" notice, machine-readable marking of outputs — **owned by Product + Legal, not by this appendix** |
| **Private person** | A teammate using AI for personal, non-professional content | Out of scope |

Everything published under a brand account is **professional deployer** activity. There is no "it's just my personal LinkedIn" exception when the account is monetised or represents the company.

---

## Classes

| Class | Code | What it means | Public label |
|-------|------|---------------|--------------|
| Out of scope | `OUT` | No AI in the published artifact — AI used only for research, ideation, keyword clustering, internal analysis | No |
| AI-assisted | `ASSIST` | AI as an editing aid: proofreading, rephrasing, outline, title, summary, translation of human-written copy, colour/lighting fixes, upscaling, caption generation | No |
| AI text, reviewed | `TEXT_HR` | Substantially AI-drafted text that passed substantive human review with a named responsible editor | No |
| AI text, public interest | `TEXT_PI` | Substantially AI-drafted text on a matter of public interest, published to inform the public, **without** substantive review | **Yes** |
| Synthetic media, non-realistic | `MEDIA_NR` | AI illustrations, abstract visuals, icons, stylised 3D, animation that no one would mistake for a photograph | No (credit recommended) |
| Synthetic media, realistic | `MEDIA_R` | Photorealistic image/video/audio of a scene, place, product or event that did not occur as shown | **Yes** |
| Deepfake | `DEEPFAKE` | AI media resembling a real (or plausibly real) person, object, place, entity or event closely enough to look authentic — incl. voice clones, face swaps, AI avatars of real colleagues | **Yes** |
| Direct AI interaction | `BOT` | Chatbot, AI agent, AI avatar host or assistant talking to a human | **Yes**, at first interaction |

### Class notes that matter for us

- **`ASSIST` is broad but not infinite.** The test is function and effect: a grammar pass is editing aid; generating three new sections of argument is not.
- **`TEXT_PI` needs *all* conditions at once**: AI-generated + published + purpose is to inform the public + matter of public interest + no substantive review. A product announcement, a how-to, or a marketing landing page normally fails the "public interest" test even when fully AI-drafted.
- **Public-interest areas we actually write about**: consumer protection, data protection and privacy law, accessibility rights, email regulation and compliance (GDPR, CAN-SPAM, EAA), economic and industry developments. When an article sits in one of those and was not properly reviewed — label it. Better: review it.
- **`DEEPFAKE` has no "it was obviously an ad" exception.** Artistic, satirical and fictional work still gets disclosed, just in a way that does not ruin the work (caption, credits, description).

---

## Disclosure markers

Each published piece is tracked against these:

| Marker | Code | What it means |
|--------|------|---------------|
| Human review | `HR` | Substantive editorial review completed; named editor accepts responsibility |
| Visible label | `VIS` | Person-facing disclosure at or immediately beside the content, visible at first exposure |
| Machine-readable provenance | `C2PA` | Content Credentials / signed provenance metadata preserved in the file |
| Platform flag | `PLAT` | The channel's own AI control is switched on (e.g. YouTube "AI use" = Yes) |
| Accessible disclosure | `A11Y` | Disclosure also present in alt text, caption, on-screen text and transcript — not colour or icon alone |

**A visible label and machine-readable provenance are separate duties.** Metadata alone never satisfies a deepfake or public-interest-text disclosure; a viewer must not have to inspect a file to learn it is synthetic.

---

## Decision tree

Run this before publishing. Stop at the first match.

```
1. Does the thing talk back to a human? (chatbot, AI agent, AI avatar host)
   → YES → BOT: disclose at the start of the first interaction
   → NO ↓

2. Does it show or voice a real (or plausibly real) person, place, event or entity
   in a way that could pass as authentic?
   → YES → DEEPFAKE: visible disclosure, first exposure, no exceptions
   → NO ↓

3. Is it AI-generated media that looks photorealistic?
   → YES → MEDIA_R: visible disclosure + C2PA
   → NO ↓

4. Is it AI-generated media that is obviously illustration / animation / abstract?
   → YES → MEDIA_NR: keep C2PA, credit in caption (recommended, not mandatory)
   → NO ↓

5. Is it substantially AI-generated TEXT?
   → NO  → ASSIST or OUT: no label
   → YES ↓

6. Is the text published to inform the public on a matter of public interest?
   → NO  → TEXT_HR: no label (still get it reviewed)
   → YES ↓

7. Did it pass substantive human review with a named responsible editor?
   → YES → TEXT_HR: no Art. 50(4) label required
   → NO  → TEXT_PI: visible disclosure
```

---

## What counts as substantive human review

The exception only works if the review is real. Tick all of these:

- [ ] Facts and figures verified against primary sources
- [ ] Sources evaluated, not just present (source, sample, period recorded)
- [ ] Material errors corrected, not just typos
- [ ] Professional judgment applied to the argument and the recommendations
- [ ] A named editor accepts responsibility for the substance
- [ ] Review date and reviewer name recorded

Spelling, grammar, a style pass or a formal "approved" click is **not** substantive review. If only those happened, the piece is still `TEXT_PI` when it is public-interest text.

This is the same bar the quality gate already sets (→ [05-content-quality.md](05-content-quality.md), [A3-quality-review-checklist.md](A3-quality-review-checklist.md)): every important claim needs a source, own data, or an example; every number needs period and sample. A piece that passes the quality review has, in practice, passed substantive review.

---

## Channel rules

### Matrix

| Channel | Text | Images | Video | Audio / voice | Interactive |
|---|---|---|---|---|---|
| **Blog** | `ASSIST` / `TEXT_HR` default → no label. `TEXT_PI` only for unreviewed public-interest pieces | Illustrations `MEDIA_NR` → credit in caption. Photoreal visuals `MEDIA_R` → visible label next to image | Embedded video follows the YouTube row | AI voiceover of a real person → `DEEPFAKE` | AI assistant widget → `BOT` |
| **Landing pages** | Marketing copy — normally `ASSIST`/`TEXT_HR`, no label | Same as blog. Product screenshots must stay authentic — no AI-fabricated UI presented as real | Same as blog | Same as blog | Demo chatbot → `BOT` |
| **YouTube** | Titles, descriptions, scripts, thumbnails: `ASSIST` for YouTube purposes — but see divergence note | Thumbnails: photoreal fabrications of real people or events → `DEEPFAKE` under EU rules even though YouTube exempts thumbnails | Realistic AI footage, AI B-roll of real places, AI avatars → `PLAT` + `VIS` | AI music, AI dubbing, cloned voices → `PLAT` + `VIS` | — |
| **Webinars** | Slides and scripts — `ASSIST`, no label | AI visuals in slides → follow image rules | AI avatar presenter, AI-generated demo footage → `DEEPFAKE` | AI dubbing or voice clone of a speaker → `DEEPFAKE`, spoken + written notice | Live AI Q&A bot → `BOT` |

### Blog

- Default class for our articles: `TEXT_HR`. No banner, no badge, no "written with AI" disclaimer on standard marketing and how-to content.
- **Do add a visible line** when the article is public-interest (law, privacy, accessibility rights, consumer protection, industry economics) *and* was not substantively reviewed. The correct fix is usually to review it, not to label it.
- AI illustrations: add the credit in the image caption, keep C2PA in the source file, mirror the disclosure in `alt`.
- Photoreal AI image: visible label immediately beside the image — not in the footer, not in the privacy policy.
- CMS strips metadata on upload in most stacks. Keep the original C2PA-signed file in the asset library even when the published copy loses it.

**Placement:** caption directly under the image; for whole-article disclosure — a line directly under the H1, above the intro, never below the fold.

### Landing pages

- Copy: no label needed for `ASSIST`/`TEXT_HR` marketing text.
- Never present AI-generated interface imagery as a real product screenshot. This is a trust rule before it is a compliance rule.
- Customer photos, testimonial portraits, "team" photos: if AI-generated and photorealistic → `MEDIA_R`, visible label. Preferred option: don't do it.
- Any embedded AI chat or demo assistant needs the `BOT` notice from the first message, persistent afterwards.

### YouTube

YouTube's own rules and the EU rules overlap but do not match. **Apply whichever is stricter.**

What YouTube requires:

- Creators must disclose AI content that makes a real person appear to say or do something they didn't, alters footage of a real event or place, or generates a realistic scene that never happened.
- Disclosure is made at upload: Studio → Attributes → "AI use" → Yes.
- For photorealistic content the label can appear on the player; for non-photorealistic or animated content it appears in the expanded description.
- YouTube may apply the label automatically — for content made with YouTube's GenAI tools, content carrying C2PA metadata, or content its systems detect. Automatic labels on YouTube-tool or C2PA content cannot be removed by the creator.
- Repeated non-disclosure can lead to labels applied manually, content removal, or suspension from the Partner Program.

What YouTube does **not** require disclosure for: script and outline generation, thumbnails, titles, infographics, captions, idea generation, upscaling and audio repair, cloning your own voice for voiceover or dubbing, non-realistic content.

**Divergence to watch — three cases where YouTube says "no need" and EU rules still bite:**

| Case | YouTube | EU AI Act | Our rule |
|---|---|---|---|
| Cloning a speaker's own voice for dubs | No disclosure needed | Voice clone of an existing person = deepfake → disclose | Disclose: `PLAT` + spoken/written notice |
| AI thumbnail showing a real person or real event realistically | No disclosure needed | Deepfake → disclose | Disclose in the description + avoid making them |
| AI B-roll of a real place | Disclosure needed if realistic | Deepfake / realistic synthetic media → disclose | Disclose, both layers |

**Placement:** "AI use" = Yes at upload; plus a plain line in the first two lines of the description (above the fold); plus an on-screen notice in the first seconds for realistic footage; plus the same statement in the pinned comment if the video is heavily reshared.

### Webinars

Treat a webinar as three deliverables with three disclosure paths: **the live session**, **the recording**, **the derivative cuts** (recaps, Shorts, quote cards).

- **Live, human speakers, AI-made slides** → `ASSIST`. No disclosure.
- **AI avatar presenting**, or a synthetic co-host → `DEEPFAKE`/`BOT`. Say it out loud in the opening, put it on the registration page, and keep it in the on-screen lower third.
- **AI dubbing or AI translation with a cloned speaker voice** → `DEEPFAKE`. Notice before playback starts, plus a written line in the player and the description.
- **AI-generated demo footage** of a product flow that was never recorded → `MEDIA_R`. On-screen label while it plays.
- **Recording published to YouTube** → re-apply the YouTube rules; the label does not travel with the file.
- **Derivative cuts** → the disclosure must be repeated on every cut. A label on the 60-minute recording does not cover a 30-second Short.
- **Registration and follow-up emails**: if the session includes any `DEEPFAKE`-class element, state it on the registration page before sign-up.

### Reposting and syndication

Scaling a piece across channels re-opens the disclosure question every time (→ [A5-scaling-playbook.md](A5-scaling-playbook.md)).

- A label applied by one platform does not travel to another. Re-apply on every surface: guest posts, partner blogs, newsletters, social.
- If the receiving platform strips metadata or hides the label, the visible disclosure must be repeated manually.
- Guest posts on external platforms: the writer brief must state which class the piece is and which disclosure line goes with it.

---

## Wording bank

Use plain, specific wording. Avoid "enhanced", "synthetic", "digitally created" — they don't tell an ordinary reader that AI was involved.

| Situation | EN | UK | RU |
|---|---|---|---|
| AI image | AI-generated image | Зображення згенеровано ШІ | Изображение сгенерировано ИИ |
| AI-edited image | Image altered using AI | Зображення змінено за допомогою ШІ | Изображение изменено с помощью ИИ |
| AI video | AI-generated video | Відео згенеровано ШІ | Видео сгенерировано ИИ |
| AI audio / voice | AI-generated audio | Аудіо згенеровано ШІ | Аудио сгенерировано ИИ |
| AI dubbing | Voice dubbed using AI | Озвучення виконано за допомогою ШІ | Озвучивание выполнено с помощью ИИ |
| AI avatar host | This presenter is an AI-generated avatar | Цей ведучий — аватар, згенерований ШІ | Этот ведущий — аватар, созданный ИИ |
| Public-interest text | This text was generated using AI | Цей текст згенеровано за допомогою ШІ | Этот текст сгенерирован с помощью ИИ |
| Mixed content | This content contains AI-generated or AI-modified material | Цей матеріал містить контент, створений або змінений ШІ | Этот материал содержит контент, созданный или изменённый ИИ |
| Chatbot | You are interacting with an AI assistant | Ви спілкуєтеся з ШІ-асистентом | Вы общаетесь с ИИ-ассистентом |

Visibility requirements for any of the above: clear, distinguishable from surrounding content, understandable, present at first exposure, accessible to assistive tech, appropriate to the medium.

---

## Worked example

### Q4 deliverability webinar and its derivatives

| # | Deliverable | AI involvement | Class | Markers | Visible label |
|---|---|---|---|---|---|
| 1 | Live webinar, 2 human speakers | Slides drafted with AI | `ASSIST` | — | — |
| 2 | Recording on YouTube (EN) | AI-cleaned audio, AI captions | `ASSIST` | `PLAT`(No) | — |
| 3 | UK dub with cloned speaker voice | Voice clone of a real speaker | `DEEPFAKE` | `VIS` `PLAT`(Yes) `A11Y` `C2PA` | Spoken notice before start + first line of description |
| 4 | 3 Shorts cut from the dub | Inherits the clone | `DEEPFAKE` | `VIS` `PLAT`(Yes) `A11Y` | On-screen label on each Short |
| 5 | Recap article on blog | AI-drafted from transcript, edited | `TEXT_HR` | `HR` | — |
| 6 | Hero illustration for the recap | Fully AI-generated, illustrative | `MEDIA_NR` | `C2PA` `A11Y` | Credit in caption |
| 7 | Landing page for the replay | AI-assisted copy | `ASSIST` | — | — |
| 8 | Thumbnail showing the speaker in a fabricated studio | Photoreal, real person | `DEEPFAKE` | `VIS` | **Recommendation: don't ship. Reshoot or use a real frame.** |

Line 8 is the pattern to internalize: the cheapest compliance decision is usually "don't fabricate a real person".

---

## Pre-publication checklist

- [ ] Class assigned (one of the 8 codes)
- [ ] For `TEXT_PI` risk: substantive review done, reviewer named, or label applied
- [ ] Visible label present at first exposure where required
- [ ] Label wording taken from the wording bank, in the content's language
- [ ] Disclosure duplicated in alt text / caption / on-screen text / transcript
- [ ] Platform control switched on (YouTube "AI use")
- [ ] C2PA-signed original kept in the asset library
- [ ] Derivative cuts inherit the disclosure

---

## Common mistakes

- Labeling everything "made with AI" out of caution. It devalues the label, hurts trust, and is not what the law asks for.
- Relying on metadata alone for a deepfake. A viewer should never have to inspect a file.
- Assuming the platform's automatic label will appear. It may not, and it is not our compliance evidence.
- Labeling the long recording and forgetting the cuts.
- Treating "the editor read it" as substantive review.
- Using vague wording ("enhanced", "digitally created") that doesn't say AI.
- Losing the C2PA original at CMS upload with no backup.

---

## Sources

- [Guidelines on transparency obligations for providers and deployers of certain AI systems](https://digital-strategy.ec.europa.eu/en/policies/guidelines-ai-transparency-obligations) — European Commission, last updated 6 Aug 2026
- [Q&A: Transparency obligations under Article 50 of the AI Act](https://digital-strategy.ec.europa.eu/en/faqs/transparency-obligations-under-article-50-ai-act) — European Commission
- [Code of Practice on Transparency of AI-generated Content](https://digital-strategy.ec.europa.eu/en/policies/code-practice-ai-generated-content) — European Commission
- [Regulation (EU) 2024/1689 (AI Act), Article 50](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng) — EUR-Lex
- [Disclosing use of GenAI content](https://support.google.com/youtube/answer/14328491) — YouTube Help
