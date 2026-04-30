# Appendix A7 — Good vs. Bad Content Examples

> **⚠ DRAFT — illustrative example.** This is an AI-generated draft intended as a possible illustration and a TODO starting point. It is not a ready-to-use instruction. Review, adapt, and validate before adopting.

## Purpose

Concrete side-by-side examples showing what "valuable information" looks like in practice vs. generic content that "could be written by ChatGPT" (→ [01-mission-and-vision.md](01-mission-and-vision.md), [02-valuable-information.md](02-valuable-information.md)).

Each example targets one AVI type and shows the transformation from bad → good.

---

## Example 1: Systematization (AVI-01)

**The test:** Does the content offer a new framework or categorization that enhances the reader's understanding?

### ❌ Without Systematization

> **5 Ways to Improve Your Email Design**
>
> 1. Use a clean layout
> 2. Choose readable fonts
> 3. Add compelling images
> 4. Make your CTA stand out
> 5. Optimize for mobile
>
> By following these tips, you'll create better emails that engage your subscribers.

**Why it fails:** This is a flat list of generic tips. No framework, no hierarchy, no way to think about the problem systematically. Any AI can produce this list.

### ✅ With Systematization

> **The Email Design Decision Framework: Structure → Style → Signal**
>
> Every email design decision falls into one of three layers, and they must be addressed in order:
>
> **Layer 1 — Structure (layout and hierarchy)**
> Before choosing colors or fonts, solve the information architecture. How many content blocks? What's the visual hierarchy? Single-column or hybrid? This layer determines whether the email is scannable — and 67% of emails are scanned, not read (Litmus 2024).
>
> **Layer 2 — Style (visual identity)**
> Once structure is set, apply brand-consistent styling. This includes typography (2 fonts max), color palette (primary + accent + neutral), and image treatment (photography vs. illustration vs. none). Style without structure is decoration. Structure without style is a wireframe.
>
> **Layer 3 — Signal (conversion elements)**
> CTA placement, urgency indicators, social proof, and personalization tokens. These work only if Layers 1 and 2 are solid — a beautiful button in a broken layout gets no clicks.
>
> Most teams jump straight to Layer 3 (making the button bigger) when their real problem is Layer 1 (the email has no visual hierarchy).

**What makes it valuable:** The reader gets a reusable mental model (Structure → Style → Signal) that helps them diagnose and solve future design problems — not just follow a checklist.

---

## Example 2: Unique Knowledge (AVI-02)

**The test:** Does the content contain information that only we can provide — our data, our experiments, our perspective?

### ❌ Without Unique Knowledge

> **Why You Should Use Dynamic Content in Emails**
>
> Dynamic content allows you to show different content to different subscribers based on their data. According to industry reports, personalized emails generate 6x higher transaction rates. Marketers who use dynamic content see better engagement and higher ROI. Consider implementing dynamic content blocks in your next campaign.

**Why it fails:** Every claim is from "industry reports" (unspecified). There's nothing here that the reader can't find in 10 other blog posts. No original data, no firsthand experience, no non-obvious insight.

### ✅ With Unique Knowledge

> **We Tested Dynamic Content Blocks Across 847 Campaigns. Here's What Actually Moves the Needle.**
>
> Between January and September 2024, we analyzed 847 campaigns sent through Stripo-built templates — 312 with dynamic content blocks, 535 without.
>
> The expected result: dynamic content outperformed static. Click-through rate was 18% higher on average.
>
> The unexpected result: the number of dynamic blocks matters — but not linearly. Emails with 1–2 dynamic blocks saw +12% CTR. Emails with 3–4 blocks saw +24%. But emails with 5+ blocks actually dropped to +8%, likely due to increased rendering issues across email clients.
>
> Our practical takeaway: the sweet spot is 3–4 dynamic blocks per email. Beyond that, the complexity tax (rendering bugs, longer QA, fallback management) eats into the personalization benefit.
>
> We also found that fallback content quality matters more than personalization sophistication. Campaigns where the fallback was a thoughtful default (not "Dear Customer") retained 91% of the dynamic content's performance lift even when personalization data was missing.

**What makes it valuable:** Specific numbers from our own data. A non-obvious finding (diminishing returns after 4 blocks). A practical recommendation backed by evidence. No one else can write this paragraph.

---

## Example 3: Product Mastery (AVI-03)

**The test:** Does the content show how to implement a solution using our product, with enough detail that the reader can actually do it?

### ❌ Without Product Mastery

> **How to Create Responsive Emails**
>
> Responsive email design ensures your emails look great on any device. Use a responsive email builder like Stripo to create mobile-friendly templates. Make sure to test your emails on different devices before sending. Stripo offers a preview feature that helps you check how your email looks on desktop and mobile.

**Why it fails:** The product mention is surface-level. "Use Stripo" and "Stripo offers a preview feature" don't help the reader actually do anything. This reads like a feature list, not a guide.

### ✅ With Product Mastery

> **Building a Responsive Email in Stripo: The 3-Container Method**
>
> Most responsive email problems come from using a single container and hoping the email client will figure out the stacking order on mobile. It won't — Outlook, Gmail, and Apple Mail all handle it differently.
>
> Here's the method we use internally for every Stripo template:
>
> **Step 1: Outer container — full-width wrapper**
> Start with a 1-column structure. In Stripo, drag a "1 Column" structure to your canvas. Set width to 600px (desktop) — Stripo auto-generates the `max-width: 100%` responsive fallback. Don't set a fixed height.
>
> **Step 2: Inner containers — content modules**
> Inside the outer container, use the "2 Columns" structure for side-by-side content. In the Stripo editor, click the structure settings → Mobile formatting → check "Stack on mobile." This makes the 2-column layout collapse to single-column at 480px viewport width.
>
> **Step 3: Content modules — independent blocks**
> Each module (image + text + CTA) should be self-contained. In Stripo, click any module → Module settings → toggle "Save as module." Now you can reuse this responsive block across campaigns, and any update propagates to all instances.
>
> **Testing checkpoint:** Before sending, use Stripo's built-in preview: click the eye icon → select "Mobile" → verify that columns stack correctly and no text is smaller than 14px on mobile. Then send a test via your ESP — Stripo's preview covers rendering, but the ESP test catches delivery-specific issues.
>
> [Screenshot: Stripo editor showing the 3-container structure with mobile preview toggle highlighted]

**What makes it valuable:** Specific steps inside the product. Exact UI references (button names, settings panels). A reusable method ("3-Container Method") with reasoning for each step. The reader can open Stripo right now and follow along.

---

## The Combination Effect

The strongest content combines all three AVI types. Each example above works alone, but together they create a piece at VI Level 3:

1. **Systematization** gives the reader a framework (Structure → Style → Signal)
2. **Unique Knowledge** gives the reader evidence (our 847-campaign data)
3. **Product Mastery** gives the reader a tool (the 3-Container Method in Stripo)

An article with all three is hard to replicate, hard to ignore, and hard to outrank.

---

## Quick Self-Diagnostic for Authors

Before submitting your draft, try this:

| Question | If YES | If NO |
|----------|--------|-------|
| Could ChatGPT write this paragraph without my input? | Remove or rewrite — add your data, experience, or framework | Keep — it has unique value |
| Does the reader get a new way to think about the problem? | Systematization is present ✓ | Consider adding a framework or categorization |
| Does the article contain data or insights only we have? | Unique Knowledge is present ✓ | Add our own experiment, stat, or perspective |
| Can the reader open our product and follow along? | Product Mastery is present ✓ | Add specific steps, screenshots, UI references |

---

## TODO

- [ ] Replace illustrative examples with real excerpts from Stripo / Yespo / Claspo blog
- [ ] Add examples for each product (not just Stripo)
- [ ] Create a shorter "cheat sheet" version for quick reference
- [ ] Use these examples in onboarding for new content team members
