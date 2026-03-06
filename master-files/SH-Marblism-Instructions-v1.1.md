# SALING HOMES — CONTENT INSTRUCTIONS FOR MARBLISM

**Version 1.1 | February 2026** **Joe Saling | Saling Homes at eXp Realty | sellingpdxhomes.com**

These instructions apply to every blog post you produce for Saling Homes. They are organized into sections. Read all sections before building any post. When anything in these instructions conflicts with a default Marblism pattern, these instructions take priority.

---

## SECTION 1: BRAND DESIGN SYSTEM

### Fonts

Use these two Google Fonts on every post. Include this link in the document head:

```
https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&family=Source+Sans+3:wght@300;400;600&display=swap
```

Headings (H1, H2, H3): Playfair Display Body text, buttons, labels, captions, navigation: Source Sans 3

Do not use Montserrat. Do not use any other font family.

### Font Sizes and Line Height

H1: 2.8rem to 3.2rem, weight 700 H2: 1.9rem to 2.2rem, weight 700 H3: 1.4rem to 1.6rem, weight 600 Body text: 1.15rem, line-height 1.9 Captions: 0.85rem, uppercase, letter-spacing 0.08em Buttons: 1rem, weight 600

### Color System

Use these exact values. Do not substitute or approximate.

```
--gold: #C9A84C
--gold-rich: #D4AF37
--gold-light: #C9952A
--gold-pale: #FBF5E6
--near-black: #222222
--text-body: #444444
--text-muted: #767676
--border: #E2DDD6
--bg-soft: #F7F5F2
```

Gold (\#D4AF37) is used for: divider lines, bullet accents, borders, callout left borders, hover states, FAQ icons, back to top links, TOC links.

Near-black (\#222222) is used for: hero sections, dark callout boxes, H1 and H2 text, button backgrounds on dark sections.

White (\#FFFFFF) is used for: card backgrounds, body areas, text on dark backgrounds.

Never use gold as a text color on a light background. Gold is for accents and borders only. Text on light backgrounds uses \#444444. Text on dark backgrounds uses \#FFFFFF.

### Callout Box Colors

Gold left border (\#D4AF37), pale gold background (\#FBF5E6): Portland-specific examples, calculations, favorable information.

Green left border (\#86d3a3), pale green background (\#f3faf6): Action steps, positive outcomes, what to do.

Orange left border (\#f3b38c), pale orange background (\#fff4ee): Warnings, important caveats, expiring benefits.

Red left border (\#e57373), pale red background (\#fff5f5): Expired benefits, negative changes, things that no longer apply.

Dark left border (\#222222), light grey background (\#f2f2f2): Technical rules, definitions, precise legal or process language.

### Buttons

Primary button: background \#D4AF37, text color \#000000, border-radius 12px, font-weight 600, box-shadow 0 4px 16px rgba(212,175,55,0.3). Hover: background \#B8961F.

Secondary button: background \#FFFFFF, text color \#222222, border 2px solid \#E2DDD6, border-radius 12px, font-weight 600\. Hover: border-color \#D4AF37, text color \#D4AF37.

Never use gold text on a gold button background. Primary button text is always \#000000 or \#FFFFFF, never gold.

---

## SECTION 2: HTML STRUCTURE AND CSS RULES

### Mandatory HTML Sequence

Every post must follow this exact structure. The CMS strips style blocks placed before content.

```
<div id="post-[slug]">
    [All article content goes here]
</div>

<style>
    [All CSS goes here — always AFTER the closing content div]
</style>

<script type="application/ld+json">
    [Schema goes here — always AFTER the style block]
</script>
```

The style block goes after the closing content div. Never before it. The schema block goes after the style block. Never before it. Never wrap script tags inside paragraph tags.

### CSS Scoping — Critical

All CSS must be scoped to the post wrapper ID. The wrapper ID is derived from the post slug, prefixed with "post-".

Example: a post with slug /blog/portland-homeowner-tax-deductions-2026 uses wrapper ID post-tax-2026.

Correct: \#post-tax-2026 h2 { font-size: 1.9rem; } Wrong: h2 { font-size: 1.9rem; } Wrong: \* { margin: 0; padding: 0; } Wrong: body { font-family: 'Source Sans 3'; }

Never use universal selectors (asterisk), body selectors, or html selectors. These bleed into the rest of the CMS page and break other content on the site.

### External Links

Every link to an external domain must include all three of these attributes:

```
target="_blank" rel="noopener noreferrer" title="Descriptive Title of Destination"
```

The title attribute must describe the destination specifically. Example: title="Bankrate Mortgage Interest Deduction Guide"

Internal links (links to sellingpdxhomes.com pages) do not use target="\_blank" and do not require title attributes.

### Image Rules

Keep all images you generate. Do not remove or replace them.

Hero image: use loading="eager" All other images: use loading="lazy"

Alt text format: \[Description of what is shown\], \[City or location\], Oregon. Never write "photo of" or "image of." Start with the subject. Example: "Residential street lined with Douglas fir trees, Bull Mountain, Tigard, Oregon"

Caption style: 0.85rem, italic, color \#999999, margin-top 4px.

---

## SECTION 3: REQUIRED COMPONENTS

Every post must include all of the following components. Do not skip any.

### Quick Answer Box

A gold-left-bordered callout positioned near the top of the post, before the Table of Contents. Answers the post's primary question in three to five sentences. Background \#FBF5E6, left border 4px solid \#D4AF37.

Label it: "Quick Answer" in small uppercase gold text above the answer.

A reader who only reads this box should leave with the core information. This box is specifically structured to be captured by Google Featured Snippets and AI Overview panels.

### Table of Contents — Key Takeaways

Label the TOC "Key Takeaways and Quick Navigation" for market and data posts. Label it "Key Takeaways" for education and analysis posts.

Style: gold left border, light grey background, numbered list, gold anchor links. Position after the Quick Answer box.

Keep your existing back to top links throughout the post. They are good and should remain.

### FAQ Accordion

Minimum six questions using the HTML details and summary element pattern. Research actual questions people search for on this topic. Do not invent questions that sound good but are not actually searched.

FAQ icon style: a circular dark (\#222222) button with gold (\#D4AF37) plus sign that rotates to an X when open.

The questions and answers in the visible FAQ accordion must match the FAQPage schema exactly, word for word. This is a hard requirement. Generate both at the same time from the same list.

### Exception Box

Required on every education post and every analysis post. An orange-bordered callout that explicitly covers when the guidance in this post does not apply, when the analysis breaks down, or what conditions would change the recommendation.

Label it clearly: "When This Does Not Apply" or "Important Exceptions" or "What This Analysis Does Not Cover."

This is a credibility element. A reader who is an exception to the main guidance should know that before acting on anything in the post.

### Data Verification Timestamp

Every post must include a clearly labeled statement of when the data was verified. Place it in the Data Sources section or as a standalone line before the author bio.

Format: "Data verified: \[Month Year\]"

### Data Sources Block

Required on education posts and analysis posts. List every source cited in the post with outbound links. Include the data verification timestamp at the top of this block.

Format: "Data Sources and References (as of \[Month Year\]):"

### Author Bio Box

Every post ends with a styled author bio box before the EHO statement. This is not a plain text footer. It is a styled box with a gold left border (4px solid \#D4AF37), light grey background (\#f7f7f7), border-radius 16px, padding 22px 26px.

Use this exact content:

**About Joe Saling**

Joe Saling is a Real Estate Advisor at Saling Homes at eXp Realty, serving buyers and sellers across the Portland Metro area. With 10 years in Portland real estate and 20+ years in sales, marketing, and leadership, Joe specializes in helping clients understand the market and make confident, well-informed decisions. His approach is education first — no pressure, no surprises.

Joe Saling | Saling Homes at eXp Realty | 503-910-7364 | [joe@sellingpdxhomes.com](mailto:joe@sellingpdxhomes.com) | [www.sellingpdxhomes.com](http://www.sellingpdxhomes.com)

Phone should be a tel: link. Email should be a mailto: link. Website should open in a new tab.

Do not mention commission. Do not mention specific service areas. Do not add anything not listed above.

### EHO Statement

Required at the bottom of every post, after the author bio. Plain text, small font (0.85rem), color \#767676.

Use this exact language:

"Saling Homes at eXp Realty is committed to equal housing opportunity. We do not discriminate on the basis of race, color, religion, sex, handicap, familial status, or national origin."

### Disclaimer

Required on education posts only (tax law, buying process, legal topics, financial guidance). Appears twice: once near the top immediately below the H1, and once at the bottom before the author bio.

Use this exact language:

"The information in this post is for general educational purposes and does not constitute financial, legal, or tax advice. Consult a qualified professional for guidance specific to your situation."

Style: small clearly labeled box, 0.9rem, color \#555555. Does not need to be prominent but must be visible.

---

## SECTION 4: CITATIONS AND DATA STANDARDS

### The Core Rule

Every statistic or data point presented as fact must have a named, linkable source attached to it. Not a general reference at the bottom of the post. A direct inline link or a numbered citation that connects this specific number to this specific source.

If a statistic cannot be traced to a primary or authoritative secondary source, one of three things must happen:

1. Find and link the source inline.  
2. Reframe it as an estimate with honest language: "Based on regional market data, estimates suggest..." or "Industry analysis indicates approximately..."  
3. Remove it.

Never present an unverified number as a confirmed fact. This is the single most important credibility rule.

### Authoritative Sources by Post Type

Education posts (tax, finance, legal): IRS publications, Oregon Department of Revenue, H\&R Block, NerdWallet, Bankrate, CFPB.

Analysis posts (market dynamics, employer corridors): RMLS, Oregon Employment Department, Bureau of Labor Statistics, Portland Business Journal, city government economic development pages, employer investor relations pages for campus investment data.

Neighborhood and local posts: City of \[City\] official website, school district official website, Oregon Department of Education, TriMet, specific business websites for named locations.

### Minimum Citation Count

Every post must include a minimum of five authoritative outbound links to named sources. Informational links to company homepages (Intel.com, Nike.com) count as informational context, not data citations. The five minimum must be sources that support specific claims made in the post.

### External Link Format

All outbound links must use:

```
target="_blank" rel="noopener noreferrer" title="Descriptive Title"
```

---

## SECTION 5: SCHEMA MARKUP

### Structure

Use the @graph structure to combine all schema types in a single JSON-LD block. This is the correct format. Separate schema blocks are acceptable but the @graph approach is preferred.

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Article",
      "@id": "https://www.sellingpdxhomes.com/blog/[post-slug]",
      "headline": "[H1 text]",
      "description": "[Meta description text]",
      "image": "[Hero image URL]",
      "datePublished": "[YYYY-MM-DD]",
      "dateModified": "[YYYY-MM-DD]",
      "keywords": "[primary keyword, secondary keyword 1, secondary keyword 2]",
      "author": {
        "@type": "Person",
        "name": "Joe Saling",
        "url": "https://www.sellingpdxhomes.com/about",
        "jobTitle": "Real Estate Advisor",
        "telephone": "+15039107364",
        "email": "joe@sellingpdxhomes.com",
        "worksFor": {
          "@type": "Organization",
          "name": "Saling Homes at eXp Realty",
          "url": "https://www.sellingpdxhomes.com"
        }
      },
      "publisher": {
        "@type": "Organization",
        "name": "Saling Homes at eXp Realty",
        "url": "https://www.sellingpdxhomes.com"
      }
    },
    {
      "@type": "BreadcrumbList",
      "itemListElement": [
        { "@type": "ListItem", "position": 1, "name": "Home", "item": "https://www.sellingpdxhomes.com" },
        { "@type": "ListItem", "position": 2, "name": "Blog", "item": "https://www.sellingpdxhomes.com/blog" },
        { "@type": "ListItem", "position": 3, "name": "[Post Title]", "item": "https://www.sellingpdxhomes.com/blog/[post-slug]" }
      ]
    },
    {
      "@type": "FAQPage",
      "mainEntity": [
        {
          "@type": "Question",
          "name": "[Question exactly as it appears in the visible FAQ accordion]",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "[Answer exactly as it appears in the visible FAQ accordion]"
          }
        }
      ]
    }
  ]
}
```

### FAQ Schema Alignment Rule

The questions and answers in the FAQPage schema must match the visible FAQ accordion exactly, word for word. Generate both from the same list at the same time. Never write the schema separately from the visible FAQ. Mismatched FAQ schema is treated as a quality signal against the page by search engines.

### Schema Placement

Schema goes at the end of the post body, after the style block, following the mandatory HTML sequence in Section 2\. Do not place schema before the article content. Do not wrap schema script tags in paragraph tags.

---

## SECTION 6: VOICE AND FORBIDDEN WORDS

### Voice

Educational over salesy. Direct but warm. Confident without arrogant. Personal and human. Joe is the trusted advisor who helps clients understand the landscape so they can make their own informed decisions. He is never the closer pushing for action.

CTAs are always invitations, never demands. "When you're ready, I'm here" is correct. "Act now" is never correct.

Joe acknowledges the limits of his expertise where relevant. On tax posts: "I am a real estate advisor, not a CPA." On legal topics: "Consult a qualified professional." This honest calibration is a feature, not a weakness.

### Forbidden Words

Never use any of the following words or phrases in any post:

stunning, breathtaking, charming, nestled, vibrant, gem, hidden gem, wonderful, amazing, incredible, world-class, unmatched, guru, ninja, expert (as a self-description for Joe), don't miss, act now, limited time, once in a lifetime, you need to, trust me, everyone knows, it is what it is, seamlessly, game-changer (unless used ironically), synergy, leverage (as a verb in marketing context).

### CTA Language

CTAs are section-specific. Use these patterns:

Education posts: "If this raises questions about your specific situation, I'm happy to talk through it." Link to /contact.

Analysis posts: "Ready to explore what this means for your search?" Link to /listings or /evaluation.

Neighborhood posts: "Want to see it for yourself?" Link to /contact.

All posts: Never link to Zillow, Redfin, or Realtor.com anywhere in the post body.

### Standard CTA URLs

These are the only valid CTA destination URLs. Do not create variations.

Primary seller CTA: /evaluation Market data CTA: /snapshot Contact: /contact Thinking about selling: /sell Browse listings: /listings

---

## SECTION 7: JOE'S INFORMATION

Fixed. Do not alter any of this. Use exactly as written.

**Name:** Joe Saling **Title:** Real Estate Advisor **Company:** Saling Homes at eXp Realty **Phone:** (503) 910-7364 | tel link: tel:5039107364 **Email:** [joe@sellingpdxhomes.com](mailto:joe@sellingpdxhomes.com) | mailto link: [mailto:joe@sellingpdxhomes.com](mailto:joe@sellingpdxhomes.com) **Website:** [www.sellingpdxhomes.com](http://www.sellingpdxhomes.com) | [https://www.sellingpdxhomes.com](https://www.sellingpdxhomes.com) **About page:** [https://www.sellingpdxhomes.com/about](https://www.sellingpdxhomes.com/about)

**Standard signature block (use in author bio):**

Joe Saling Saling Homes at eXp Realty 503-910-7364

**Standard credentials (use in author bio, do not expand or alter):**

10 years in Portland metro real estate. 20+ years in sales, marketing, and leadership. Education-first approach. Buyer advocate.

**What not to include:**

Do not mention commission percentage. Do not list specific service area neighborhoods. Do not use the words guru, expert, ninja, or specialist as self-descriptions. Do not promise outcomes.

---

## SECTION 8: MOBILE DESIGN STANDARDS

Joe's site is mobile-user heavy. Mobile is the primary design target. Desktop is secondary. Every post you produce must be fully functional and readable on a phone screen before anything else.

### Breakpoints — Required on Every Post

Include two media query breakpoints in every post.

768px breakpoint: Tablet adjustments. Grids collapse. Floated images go full width.

480px breakpoint: Phone-specific. This is the most important breakpoint. Most of Joe's traffic comes from iPhone 14, 15, and SE screen sizes (375px to 430px wide). Build for that range first.

### Mobile Font Sizes at 480px

H1: 1.9rem H2: 1.45rem H3: 1.2rem Body text: 1.05rem minimum, line-height 1.85 Captions: 0.82rem Buttons: 1rem, weight 600 FAQ summary text: 0.95rem TOC links: 0.9rem

Never let body text drop below 1rem on mobile. Smaller than 1rem is inaccessible.

### Mobile Layout Rules

Images: All floated images go to width 100%, float none at 480px. Never float images on mobile. Floated images break text flow on small screens.

Grids: Every multi-column grid collapses to a single column at 480px. No exceptions.

Tables: Every table is wrapped in a div with overflow-x auto at all screen sizes. This is non-negotiable. Tables that overflow the viewport on mobile break the entire page.

Callout boxes: Padding reduces to 16px 18px at 480px. Full width.

CTA buttons: Stack vertically at 480px. Each button becomes width 100%, display block, margin-bottom 12px. Side-by-side buttons on mobile are too small to tap accurately.

### Touch Target Sizing

Every tappable element must be minimum 44px tall. This is the Apple Human Interface Guideline minimum.

FAQ accordion rows: min-height 48px, padding 14px 16px, tap target is the full row width.

Buttons: min-height 48px, padding 14px 24px.

Back to top links: display block, min-height 44px, line-height 44px.

### Mobile Color and Contrast

Gold (\#D4AF37) on a white background fails WCAG AA contrast. Never use gold as body text color. Gold is for borders, accents, bullet dots, and icons only.

Body text color on white: \#444444. Text on dark backgrounds: \#FFFFFF. Both pass WCAG AA at all sizes including mobile.

Do not reduce contrast on mobile. If text is small it needs more contrast, not less.

### Required Mobile CSS

Include these two media query blocks in the style section of every post. Adapt the wrapper ID and class names to match the specific post.

```css
@media (max-width: 768px) {
  #[post-id] h1 { font-size: 2.1rem; }
  #[post-id] .editorial-img,
  #[post-id] .editorial-img.left {
    width: 100%;
    float: none;
    margin: 0 0 20px 0;
  }
  #[post-id] .two-col-grid,
  #[post-id] .three-col-grid { grid-template-columns: 1fr; }
  #[post-id] .cta-buttons { flex-direction: column; }
  #[post-id] .cta-buttons a { width: 100%; text-align: center; }
}

@media (max-width: 480px) {
  #[post-id] h1 { font-size: 1.9rem; }
  #[post-id] h2 { font-size: 1.45rem; }
  #[post-id] h3 { font-size: 1.2rem; }
  #[post-id] { font-size: 1.05rem; line-height: 1.85; }
  #[post-id] .callout-gold,
  #[post-id] .callout-dark,
  #[post-id] .callout-green,
  #[post-id] .callout-orange,
  #[post-id] .callout-red { padding: 16px 18px; }
  #[post-id] .faq-acc summary { min-height: 48px; padding: 14px 16px; }
  #[post-id] .btn-primary,
  #[post-id] .btn-secondary {
    display: block;
    width: 100%;
    text-align: center;
    margin-bottom: 12px;
    min-height: 48px;
  }
  #[post-id] .data-table-wrap {
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
  }
  #[post-id] .back-to-top a {
    display: block;
    min-height: 44px;
    line-height: 44px;
  }
}
```

---

*Saling Homes Content Instructions for Marblism | Version 1.1 | February 2026* *Questions: Joe Saling | [joe@sellingpdxhomes.com](mailto:joe@sellingpdxhomes.com) | (503) 910-7364*  
