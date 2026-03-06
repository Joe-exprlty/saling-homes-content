# SALING HOMES — BLOG POST MASTER FILE

**Version 1.3 | February 2026** **sellingpdxhomes.com | Joe Saling | Saling Homes at eXp Realty**

---

## VERSION HISTORY

| Version | Date | Changes |
| :---- | :---- | :---- |
| 1.0 | February 2026 | Initial release. Four categories, shared rules, schema, SEO suite, linking rules, pre-publish checklist. |
| 1.1 | February 2026 | Added Lofty HTML structure rule (style block after content). Added external link attribute requirements. Locked CTA URL standards. Added FAQ minimum count (6 questions). Added data verification timestamp requirement. Upgraded author bio standard to styled box. Scoped CSS requirement clarified. Added cross-article pattern notes from content audit. |
| 1.2 | February 2026 | Added full Mobile Design Standards section. Two breakpoints (768px and 480px). Mobile font sizes, layout rules, touch target sizing, contrast requirements, and required CSS pattern. Added mobile check to pre-publish checklist. |
| 1.3 | February 2026 | Added Category 5: Marblism Compliance Pass. Defines the surgical compliance workflow for Marblism-produced HTML posts. Preserves Marblism content and images. Fixes design system, Lofty structure, CSS scoping, schema, FAQ alignment, author bio, EHO, mobile, and external link attributes. Flags unverified statistics and missing exception boxes for Joe's input. |

---

## HOW TO USE THIS FILE

Upload this file at the start of every blog post conversation alongside Sellingpdxhomes\_SEO\_Complete.xlsx. This file governs all five blog post categories. Do not ask Joe to re-explain structure, voice, or linking rules. Everything is here.

At the start of every conversation ask: "What type of post are you building today?" Then present the five options clearly. When Joe selects a category, read the shared rules in this file first, then read the category-specific section. Apply both. When anything conflicts between the shared rules and a category section, the category section wins.

Every build runs in two phases. Do not skip Phase 1\. Do not begin Phase 2 until Joe types YES.

---

## THE FOUR BLOG POST CATEGORIES

**Category 1: Education Posts** Evergreen or semi-evergreen posts that make complex topics accessible. Tax law, buying process, earnest money, inspection reports, what to expect at closing. The Portland Homeowner Tax Deductions 2026 post is the reference example. Heavy structure, cited sources, disclaimer required.

**Category 2: Analysis and Strategy Posts** Joe's point of view on a market dynamic, employer corridor, buyer persona, or strategic question. The Intel and Nike Tech Corridor post is the reference example. Most editorial latitude. Most shareable. Most likely to earn AI citations.

**Category 3: Neighborhood Vibe Posts** What it actually feels like to live somewhere. Serves buyers who are past the data stage and into the feeling-it-out stage. Personal observation combined with local research. Links to city guides and neighborhood pages. Closest to Joe's most natural voice.

**Category 4: Rewrite and Restyle** Take an existing blog post and rebuild it to full current standards. Upgrades schema, adds missing components, applies the brand design system, and restructures for AEO, GEO, and EEAT authority signals. The input is existing HTML. The output is a fully rebuilt post that meets every standard in this master file.

**Category 5: Marblism Compliance Pass** Take a full HTML post produced by Marblism and apply a targeted compliance pass. Content, images, voice, and structure from Marblism are preserved. Nothing is rewritten unless it contains a forbidden word, a factually unsupported statistic, or a Fair Housing violation. The compliance pass applies the Saling Homes design system, fixes the Lofty HTML structure, scopes the CSS, upgrades the schema, aligns the FAQ, adds missing required components, and flags citation gaps for Joe to review. The output is compliant HTML ready for Lofty with Marblism's content intact.

---

## SHARED RULES — APPLY TO ALL FIVE CATEGORIES

These rules govern every post regardless of category. Read them before reading any category section.

### Voice and Tone

Every post is written in Joe's voice as defined in the Tone and Positioning Guide. The core principles are educational over salesy, direct but warm, confident without arrogant, personal and human.

The register shifts by category. Education posts are the most structured and formal. Analysis posts have the most editorial latitude and can use humor, rhetorical questions, and Joe's genuine opinions. Neighborhood vibe posts are the most conversational and personal. Rewrite and Restyle posts inherit the voice register of their original category.

No post uses the following words under any circumstances: stunning, breathtaking, charming, nestled, vibrant, gem, hidden gem, wonderful, amazing, incredible, world-class, unmatched, guru, ninja, expert (as a self-description), don't miss, act now, limited time.

No post uses pressure language of any kind. CTAs are always invitations, never demands.

No post makes promises about outcomes: "We'll get you the best deal" or "Prices will rise" are never written.

### Post Length by Category

Market Reports: 1,200 to 1,800 words. Data drives length, not padding.

Education Posts: 1,500 to 2,500 words depending on topic complexity. Every section must earn its length. Cut anything that does not directly serve the reader's understanding.

Analysis Posts: 1,000 to 2,000 words. Longer is not better. The argument drives length.

Neighborhood Vibe Posts: 800 to 1,400 words. Tighter than any other category. Every sentence must be specific to this place. Generic sentences get cut.

### Schema Markup — Required on Every Post

Every post requires schema markup in the Lofty head injection field. Never put schema in the body of the post.

Required on every post: Article schema and BreadcrumbList schema.

Article schema required fields: headline, image, author (name: Joe Saling), publisher (name: Saling Homes at eXp Realty), datePublished, dateModified, description, keywords. Include @id, jobTitle, telephone, and email in the author block for full EEAT signal. Use the @graph structure to combine Article, BreadcrumbList, and FAQPage in a single JSON-LD block.

BreadcrumbList schema: Home \> Blog \> Post Title. Use the actual published URL in the item field. Never use a placeholder URL in schema.

FAQPage schema: include only when a visible FAQ accordion exists on the page. The questions and answers in the schema must match the visible questions and answers exactly, word for word. Never include FAQPage schema for questions that do not appear on the page.

### Lofty HTML Structure Rule — Critical

This is the single most important technical rule for Lofty CMS. Violating it strips all styling from the post.

The HTML for every post must follow this exact structure:

```
<div id="[post-id]">
    [All article content goes here]
</div>

<style>
    [All CSS goes here — AFTER the closing content div]
</style>

<script type="application/ld+json">
    [Schema goes here — AFTER the style block]
</script>
```

The style block goes AFTER the closing content div. Never before it. The schema block goes AFTER the style block. Never before it. Schema also goes in the Lofty head injection field. Both locations are required. Never wrap script tags in paragraph tags. Scripts are not paragraph children.

### CSS Scoping Rule — Required

All CSS must be scoped to the post's unique wrapper ID. Never use universal resets (asterisk selectors), body selectors, or html selectors. These bleed into the rest of the Lofty page and break other content.

Correct: `#post-tax-2026 h2 { font-size: 1.75rem; }` Wrong: `h2 { font-size: 1.75rem; }` Wrong: `* { margin: 0; padding: 0; }` Wrong: `body { font-family: 'Source Sans 3'; }`

The wrapper ID is derived from the post slug. Example: post slug `/blog/portland-homeowner-tax-deductions-2026` becomes wrapper ID `post-tax-2026`.

### External Link Attributes — Required on Every External Link

Every link to an external domain must include all three of the following attributes with no exceptions:

```html
target="_blank" rel="noopener noreferrer" title="Descriptive Title of Destination"
```

The title attribute must describe the destination specifically. "Bankrate Mortgage Interest Deduction Guide" is correct. "Click here" is not.

Internal links (links to sellingpdxhomes.com pages) do not use target="\_blank" and do not require title attributes.

### CTA URL Standards — Locked

These are the only valid CTA URLs for sellingpdxhomes.com. Never invent a URL. Never use a variation of these.

| CTA Purpose | Correct URL |
| :---- | :---- |
| Primary seller CTA | /evaluation |
| Market data CTA | /snapshot |
| Contact Joe | /contact |
| Thinking about selling | /sell |
| Browse listings | /listings |
| City guide index | /cities/\[city-slug\] |
| Neighborhood guide | /neighborhoods/\[neighborhood-slug\] |

The URL /home-valuation does not exist. Use /evaluation. The URL /listing/condos and /listing/open-house/beaverton exist for search feeds. Confirm in SEO spreadsheet before using.

### SEO Suite — Deliver Before Phase 2 Build

Deliver the SEO suite as plain text immediately after Joe approves Phase 1\. Do not begin the HTML build until the SEO suite is delivered and Joe has had the opportunity to review it.

**Slug:** /blog/\[post-slug\]. Keep slugs short, keyword-forward, and specific. No dates in slugs unless the post is a market report where the date is the primary identifier. Example: /blog/january-2026-portland-metro-market-update is correct. /blog/portland-home-buying-tips-2026 is not because the date will make the post feel stale.

**Meta Title:** 55 to 60 characters maximum including spaces. Lead with the primary keyword. Include Portland or the specific city name where it fits naturally. Do not use the word guide unless it is genuinely descriptive. Count characters before delivering.

**Meta Description:** 145 to 155 characters maximum including spaces. Two to three sentences. Include the primary keyword, one specific local detail, and a soft invitation to read. No exclamation points. No pressure language. Count characters before delivering.

**Primary Keyword:** One phrase of two to four words that the post is genuinely trying to rank for. Research search intent before selecting. The keyword must reflect what a real person would type, not what sounds good in a real estate context.

**Secondary Keywords:** Three to five supporting phrases that appear naturally in the content. Do not force them. If a secondary keyword does not fit naturally it does not belong in this post.

**Internal Links:** Minimum three internal links per post. Read Sellingpdxhomes\_SEO\_Complete.xlsx to find relevant pages. Never invent a URL. If no relevant internal link exists in the spreadsheet for a given section, use the closest available option or flag it for Joe.

**Update Cadence:** Note whether this post is evergreen, semi-evergreen, or time-sensitive. For time-sensitive posts note the recommended review date.

### Design System — Inherited from City Guide

All posts use the same CSS variables and typography as the city guide template.

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

Body: Source Sans 3, 1.15rem, line-height 1.9, color \#444444 H1: Playfair Display, 700 weight H2: Playfair Display, 700 weight H3: Playfair Display, 600 weight

All posts include the Google Fonts link in the Lofty head injection field.

All posts wrap content in a div with a unique ID scoped to that post to prevent CSS conflicts with other Lofty content. Example: `<div id="post-tax-2026">`. The ID is prefixed with "post-" followed by an abbreviated version of the post slug.

### Required Components — Every Post

Every post regardless of category must include all of the following.

**Hero image:** Full width, WebP format preferred. Alt text must describe the actual image content with the city or neighborhood name included. Use loading="eager" on hero images only. All other images use loading="lazy".

**Quick Answer box:** A gold-bordered callout near the top of the post that answers the post's primary question in three to five sentences. A reader who only reads this box should leave with the core information. This box is specifically structured to be captured by Google Featured Snippets and AI Overview panels. Never skip this box.

**Table of Contents:** Required for posts over 1,000 words. Gold-accented, linked to section anchors. Position after the Quick Answer box. For Market Reports the TOC is labeled "Key Takeaways and Quick Navigation."

**FAQ Accordion:** Minimum six questions using the HTML details and summary pattern. Research actual buyer search intent for this specific topic before writing questions. Answers are three to five sentences each. Direct. No hedging. Include FAQPage schema in head injection only when this section is present. The questions and answers in the schema must match the visible FAQ exactly.

**Data Verification Timestamp:** Required on every post. A clearly labeled note stating when the data in the post was last verified. Format: "Data verified: \[Month Year\]." Place this in the Data Sources block or as a standalone line immediately above the author bio. This is required on every post including Neighborhood Vibe posts.

**Author Bio:** Every post ends with Joe's bio formatted as a styled box with a gold left border. Include: Joe's name and title, three to four sentences of credentials (10 years Portland metro real estate, 20 years sales leadership and marketing, education-first approach), phone number as a tel: link, email address, and website. Do not mention commission. Link to /about for the full bio. The plain text footer approach is not sufficient. The styled box is required.

**Data Sources block:** Required for Market Reports and Education Posts. Recommended for Analysis Posts. Not required for Neighborhood Vibe Posts. List every source cited in the post with outbound links. Include the date each source was accessed. Use the format: "Data Sources and References (as of \[Month Year\]):"

**Disclaimer:** Required for Education Posts only. Standard language: "The information in this post is for general educational purposes and does not constitute financial, legal, or tax advice. Consult a qualified professional for guidance specific to your situation." Appears both near the top and repeated at the bottom.

**CTA block:** Every post ends with a CTA before the author bio. The CTA is always an invitation, never a demand. The language shifts by category. Market reports invite buyers and sellers to have a conversation. Education posts invite readers to reach out with questions. Analysis posts invite readers to explore listings or get a home valuation. Neighborhood vibe posts invite readers to see the area for themselves. Use only the verified CTA URLs in the CTA URL Standards table above.

**EHO statement:** Required on every post. A single line at the bottom: "Saling Homes at eXp Realty is committed to equal housing opportunity. We do not discriminate on the basis of race, color, religion, sex, handicap, familial status, or national origin."

### Outbound Linking Rules

Every post links to a minimum of five authoritative external sources. For Market Reports these are always RMLS, NAR, Freddie Mac, and at least two local sources. For Education Posts these are IRS publications, state agency sites, and authoritative financial reference sites. For Analysis Posts these are employer sites, city government pages, regional economic data sources. For Neighborhood Vibe Posts these are the city parks department, specific restaurant or business websites, and relevant local event pages.

Never link to Zillow, Redfin, or Realtor.com in any post body. Never link to competitor agent sites.

Do not link to a source you cannot verify. If a statistic cannot be traced to a primary or authoritative secondary source, remove the statistic or flag it for Joe to verify before publishing.

All external links must include the full attribute set: `target="_blank" rel="noopener noreferrer" title="Descriptive Title"`.

### Unverified Statistics Rule

Never publish a statistic presented as fact without a named, linkable source. If a data point cannot be traced to a primary or authoritative secondary source, one of three things happens: remove it, cite the source, or reframe it as an estimate with honest language ("based on RMLS data" or "estimates suggest"). A statistic presented as fact with no source is a credibility liability.

### Image System

Every post uses a maximum of four images. The hero image is always present. Additional images are included only when they genuinely add context that the text cannot provide.

Every image slot generates a Marbalism brief in the post-build deliverables. Briefs are a minimum of 80 words. Every brief must be specific enough that the image could not be used for any other post. Include the city or neighborhood name, time of day, season, and specific visual details that are true to this location.

File naming: \[photo-id\]-\[post-slug-abbreviated\].webp Example: hero-market-jan2026.webp

Alt text format: \[Description of what is shown\], \[City or location\], Oregon. Never write "photo of" or "image of." Start with the subject.

### Lofty Technical Rules

All CSS is scoped to the post's unique wrapper ID to prevent conflicts. No universal resets. No body or html selectors.

All viewBox attributes are lowercase.

Dark background sections use the margin fix: margin-left \-20px, margin-right \-20px.

Schema goes in the Lofty head injection field and also at the end of the post body after the style block.

Tables are wrapped in a scroll container for mobile.

The style block goes after the closing content div. The schema block goes after the style block. This sequence is mandatory.

---

## CATEGORY 1: EDUCATION POSTS

### Purpose

Make a complex topic accessible to a Portland-area homeowner or buyer who has no professional background in real estate, tax law, or finance. The reader leaves knowing enough to have a more informed conversation with their CPA, lender, or agent. Not enough to act without professional guidance. The disclaimer exists for this reason.

### Update Cadence

Semi-evergreen. Education posts age slowly but must be reviewed when laws, processes, or programs change. The post metadata includes a "Last Reviewed" date that updates with each review. The slug never includes a year so the post does not feel dated when it is reviewed and updated.

Exception: if the post topic is fundamentally tied to a specific year or law, the year may appear in the slug. Example: /blog/portland-homeowner-tax-deductions-2026 is correct because the 2026 changes are the entire topic.

### Phase 1 Research

Before writing any HTML confirm the following.

What is the primary topic and the primary question this post answers. State both in one sentence each.

What is the primary search query this post targets. Research actual search volume and intent before confirming. The post must answer the question people are actually asking, not a variation Joe prefers.

What has changed recently on this topic that makes the post timely. Education posts perform best when they answer a question that has a new or updated answer. A post about how earnest money works is useful but undifferentiated. A post about how earnest money rules changed in Oregon after a specific regulatory change is timely and specific.

What are the five most authoritative sources for this topic. For tax topics these are the IRS, Oregon Department of Revenue, H\&R Block, NerdWallet, and Bankrate. For process topics these are Oregon REALTORS, the Oregon Real Estate Agency, and the CFPB. For financial topics these are Bankrate, NerdWallet, the CFPB, and relevant federal agency sites. Confirm that all sources are current before citing them.

What are the six to eight questions people actually search for on this topic. These become the FAQ section. Research them before confirming. Do not invent questions that feel smart but are not actually searched.

Present all confirmed research in one clean block. End with: "Does this research cover the topic accurately? Type YES to begin Phase 2."

### Content Architecture

Build in this exact order.

**Hero image:** Relevant to the topic. For tax posts: a person reviewing documents at a desk. For process posts: a relevant transaction moment. Always location-specific in the alt text even if the image itself is generic.

**H1:** \[Primary Topic\]: \[What Changed / What You Need to Know / How It Works\]. Never a clever or abstract headline for education posts. The reader needs to know immediately whether this post answers their question.

**Disclaimer:** Immediately below the H1. Standard language as defined in the shared rules. Style it as a small, clearly labeled box so it is visible but does not interrupt the reading experience.

**Opening paragraph:** Two to three sentences at 1.1rem weight 500\. State what the post covers, why it is timely, and what the reader will know by the end. Include Joe's honest acknowledgment of the limits of his expertise on this specific topic. The tax post example does this well: "I am a real estate advisor, not a CPA."

**Quick Answer box:** The direct answer to the post's primary question in three to five sentences. A reader who only reads this box should leave with the core information.

**TOC:** Required. Label it "Key Takeaways and Quick Navigation."

**Change Summary Table:** For posts about updated rules or changed laws, include a table near the top showing the before and after. Columns: Topic, Before, After, Status. Use badge labels for status: New, Changed, Expired, Permanent, Unchanged. The Portland Homeowner Tax Deductions post is the reference example for this table.

**Body sections:** Each major point gets its own H2 section. Within each section use callout boxes by color to separate types of information. Use gold-bordered callouts for examples and calculations relevant to Portland. Use green-bordered callouts for favorable information or action steps. Use orange-bordered callouts for warnings or important caveats. Use red-bordered callouts for expired benefits or negative changes. Use dark-bordered callouts for technical rules or definitions.

**Portland-specific example:** Every major concept must have a Portland-specific calculation or example. Not a generic national example. A household earning $124,000, a home purchased in Concordia in 2024 for $485,000, a married couple selling in Woodstock after 14 years. Make the math real for the actual reader.

**Exception box:** Required on every education post. An orange or red-bordered callout that explicitly covers when the rules or guidance in this post do not apply. This is a non-negotiable credibility element. A reader who is an exception to the main guidance should know that before acting on anything in the post.

**FAQ Accordion:** Six to eight questions minimum. Use the questions confirmed in Phase 1 research. Visible questions must match FAQPage schema exactly.

**CTA block:** Invite readers to have a conversation about how this topic affects their specific situation. Link to /contact. Do not link to listings. This reader is not necessarily in buying mode.

**Data Sources block:** Required. List every source with outbound links. Include "Data verified: \[Month Year\]" at the top of this block.

**Disclaimer:** Repeat the disclaimer at the bottom of the post in addition to the top placement.

**Author Bio:** Styled box format as defined in shared rules.

**EHO statement.**

### Tone Notes for Education Posts

The most structured tone. Joe acknowledges the limits of his expertise early and clearly. He is the guide who helps the reader understand the landscape, not the expert who tells them what to do. Every section teaches something. The reader should feel more capable after reading than before, not more dependent on Joe for answers.

---

## CATEGORY 2: ANALYSIS AND STRATEGY POSTS

### Purpose

Connect a market dynamic, employer trend, economic pattern, or strategic question to the real decision a buyer or seller is facing. Joe's perspective is the product. The data supports the argument. This category has the most editorial latitude and produces the most shareable content.

### Update Cadence

Semi-evergreen with periodic reviews. The employer corridor post does not expire but should be reviewed when major employer news affects the market. The slug never includes a year.

### Phase 1 Research

Before writing any HTML confirm the following.

What is the central argument of this post. State it in one sentence. If it cannot be stated in one sentence the argument is not clear enough to build around.

Who are the two to three buyer or seller personas this post specifically addresses. The Intel and Nike post addressed families, downsizers, and investors. Every analysis post should identify its personas in Phase 1 so the content structure serves them specifically.

What is the primary data point or market dynamic that the argument rests on. Confirm this data point with a named, linkable source before building. An argument built on unverified data is a credibility liability.

What are the three to five most important local details that make this argument specific to Portland or to the specific city or neighborhood being analyzed. Generic analysis that could apply to any metro area is the enemy of this post type. Every analysis post must have local specificity that could not have been written by someone who has never worked in this market.

What is the honest counterargument or the scenario in which this analysis does not hold. Every analysis post must acknowledge the strongest case against Joe's position and the conditions under which the recommendation would change. This is not a weakness. It is what distinguishes honest analysis from a sales pitch.

What are the six to eight questions people actually search for on this topic. These become the FAQ section.

Present all confirmed research in one clean block. End with: "Does this argument and data meet the standard for an honest, useful analysis post? Type YES to begin Phase 2."

### Content Architecture

This category has the most flexible structure of the four. The argument drives the organization. However certain elements are always present.

**Hero image:** Relevant to the specific market dynamic or location being analyzed.

**H1:** Lead with the most provocative or specific version of the argument. The Intel and Nike post headline is a good reference. It names the specific employers, the specific dynamic, and the specific geography. Never a generic headline.

**Quick Answer box:** The core argument in three to five sentences. A reader who only reads this box should understand Joe's position.

**TOC:** Required.

**Opening:** More editorial latitude than other categories. The Intel and Nike post opens with a SimCity metaphor. That kind of writing works here because the reader has opted in to Joe's perspective. The opening should earn the reader's attention rather than just state what the post covers.

**Body sections:** One section per persona or per major argument point. Each section has three elements: the observation (what Joe has seen or what the data shows), the implication (what this means for this specific buyer or seller), and the win strategy (what to actually do about it). The win strategy boxes from the Intel and Nike post are the reference pattern.

**Data callout boxes:** Dark background, gold accent. Use sparingly for the most important statistics. Every statistic in a dark callout must be sourced and the source named in the callout or in the data sources block.

**Exception box:** Required. Named honestly: "When This Analysis Does Not Apply" or "What This Argument Does Not Cover." One to two paragraphs in an orange-bordered callout covering the scenarios where the main argument breaks down: remote work reducing the commute advantage, single-employer concentration risk, rising property taxes, overbuilt rental supply, newer competing construction. This is a non-negotiable credibility element.

**FAQ Accordion:** Six to eight questions minimum. Visible questions must match FAQPage schema exactly.

**CTA block:** Invite readers to explore listings or get a home valuation. Link to /listings and /evaluation.

**Data Sources block:** Required when major statistics are cited. Include "Data verified: \[Month Year\]."

**Author Bio:** Styled box format as defined in shared rules.

**EHO statement.**

### Tone Notes for Analysis Posts

The most editorial of all four categories. Joe can use humor, rhetorical questions, metaphors, and direct opinions. The SimCity opening in the Intel and Nike post is the right register. The reader has chosen to read Joe's analysis specifically. They are not looking for a neutral overview. They want to know what Joe actually thinks and why.

However this latitude has one hard limit. Joe's opinions must be grounded in real market experience and verifiable data. Opinions that cannot be supported by evidence are not published. The goal is informed perspective, not entertainment.

---

## CATEGORY 3: NEIGHBORHOOD VIBE POSTS

### Purpose

Help buyers who are past the data stage and into the feeling-it-out stage understand what it actually feels like to live in a specific neighborhood, street, or part of a city. This category serves a buyer who knows they want to live in Beaverton but cannot decide between Sexton Mountain and Murray Hill. Data alone does not answer that question. Observation does.

These posts also serve buyers who have never visited the Portland Metro area and are trying to form a picture of what daily life would look like. They are not looking for statistics. They are looking for the kind of detail that only comes from someone who has been there.

### Update Cadence

Mostly evergreen. A neighborhood's character changes slowly. These posts should be reviewed annually or when significant development changes the physical character of the area. The slug never includes a year.

### Phase 1 Research

Before writing any HTML confirm the following.

What specific neighborhood, area, or community is this post about. If it is about a neighborhood that has a corresponding neighborhood guide on the site, confirm that URL from the SEO spreadsheet. The post links to the neighborhood guide.

What is the central observation Joe wants to make about this place. This is not a data point. It is an impression, a feeling, a specific detail that Joe has noticed from showing homes here or from personal experience in this area. State it in one sentence. This observation becomes the spine of the post.

What are the five to eight specific physical details that make this neighborhood identifiable. Lot sizes, tree canopy, sidewalk presence, terrain, home construction era, street character, the view from a specific intersection, the sound of the neighborhood on a Saturday morning. These must be real and specific. Do not generalize.

What are the two to three local spots that residents actually use. Not the best restaurants in the city. The places that people who live on these specific streets actually go. The coffee shop that the neighborhood orbits around on weekday mornings. The trail entrance that dog walkers use before work. The grocery store that determines which side of the neighborhood is more convenient to live on.

Who is this neighborhood actually right for. And who might be better served looking elsewhere. Both questions must be answered honestly. The candid answer is what makes this post useful and trustworthy.

What are the two to three neighborhoods that buyers typically compare this one against when making their decision. These become the comparison references in the post.

Present all confirmed research in one clean block. End with: "Does this capture the neighborhood accurately? Type YES to begin Phase 2."

### Content Architecture

**Hero image:** A residential street that is identifiably this neighborhood and no other. Phase 1 physical research must inform the image brief specifically.

**H1:** What \[Neighborhood Name\] in \[City Name\] Is Actually Like. Or a specific observation framed as a headline. Example: "Bull Mountain Is Not a Suburb. It Is Something Else." The headline should surprise or intrigue the reader who already thinks they know this neighborhood.

**No byline box.** These posts feel more personal and less formal than the other three categories. The author attribution comes at the end in the bio rather than appearing in a structured byline at the top.

**Opening paragraph:** Two to three paragraphs written in the most personal register of all four categories. Joe is talking directly to the reader who is sitting on the fence about this neighborhood. The opening should place the reader in the neighborhood physically. What do they see when they turn onto the main residential street. What does the light do at a specific time of day. What does the neighborhood smell like in spring. This is not purple prose. It is specific, observational, and true.

**Quick Answer box:** Here the Quick Answer answers the question "Is \[Neighborhood\] right for me?" in three to four sentences. Honest. Direct. Includes both who it suits and who it does not.

**No TOC required.** These posts are short enough that a TOC adds friction rather than value. If the post exceeds 1,200 words consider whether it needs to be tighter rather than adding a TOC.

**The Physical Character section:** This is the heart of the post. Describe the neighborhood as if walking its streets. Use the Phase 1 physical research. Every detail must be specific to this neighborhood. If a sentence could describe any neighborhood in this city, cut it or rewrite it.

Cover in this order without using these as explicit subheadings: the terrain and elevation, the street character (quiet or cut-through, grid or cul-de-sac), the sidewalk presence and what it means for daily life, the tree canopy and what season the neighborhood looks best, the home construction era and what it means for lot sizes and layouts, the one street or intersection that best captures the neighborhood's character.

**The Daily Life section:** What does a typical week look like for someone who lives here. Where do they get coffee on a Tuesday morning. Where do they walk the dog. What is the grocery situation. How long does it take to get to the freeway. Write this as a narrative not a list. Two to three paragraphs.

If a local spot genuinely serves this neighborhood name it specifically. One sentence description. Link to its website. If no genuinely local spot exists say so honestly and note where residents actually go.

**The Schools paragraph:** One paragraph only. Name the elementary, middle, and high school. One sentence each on what distinguishes them. Link to the neighborhood guide if it exists or to the city guide schools section for more detail. Do not repeat the full school analysis. That lives in the guide. Direct the reader there.

**Joe's Honest Read section:** This is the equivalent of Joe's Take from the city and neighborhood guides but shorter and more personal. Two paragraphs maximum.

Paragraph 1: the specific local observation that only someone who has shown homes here would know. A pricing pattern, a street that most buyers overlook, a view that only exists from one side of the ridge, a school boundary nuance that changes a home's value by $30,000.

Paragraph 2: who this neighborhood is genuinely right for. Then the candid line. One sentence about who might be better served in an adjacent neighborhood, framed around lifestyle fit only. This is the most important sentence in the post.

**The Comparison paragraph:** One paragraph. Name the two to three neighborhoods buyers typically compare this one against. One sentence on what the decision usually comes down to. Link to the neighborhood guide or city guide for each comparison neighborhood if the page exists. Use /living-in-\[city\]-oregon as the slug for city guide links.

**Internal links:** Link to the neighborhood guide for this area if it exists. Link to the parent city guide using /living-in-\[city\]-oregon. Link to the listing search for this neighborhood. These three links are required. Add any additional relevant internal links from the SEO spreadsheet.

**CTA block:** Invite the reader to come see the neighborhood for themselves. Link to /contact. One sentence. Personal. Not a demand.

**Data Verification Timestamp:** Required. Add "Information current as of \[Month Year\]" as a simple line before the author bio.

**Author Bio:** Styled box format as defined in shared rules.

**EHO statement.**

### Tone Notes for Neighborhood Vibe Posts

The most personal and conversational tone of all four categories. Joe is talking to a single person, not a market segment. The reader should feel like they are getting a text from a friend who knows the neighborhood well and is giving them an honest answer about whether they would be happy there.

No pressure language of any kind. No "you should buy here before prices go up." No "this neighborhood won't last." The reader is making a life decision. Joe's job is to give them an accurate picture so they can make it well.

Specific language over general language at all times. "The houses on the ridge side of the neighborhood sit about fifteen feet above street level and have unobstructed views of the valley" is better than "the neighborhood has great views." "The coffee shop three blocks from the main park entrance has been there since 2011 and the owner knows most of the regulars by name" is better than "there is a neighborhood coffee shop."

---

## CATEGORY 4: REWRITE AND RESTYLE

### Purpose

Take an existing blog post that was written before the current content system and rebuild it to full current standards. The existing post may have good content, good data, or good local detail but is missing the schema, structure, design, or AEO/GEO/EEAT signals that make it competitive. The goal is to preserve everything that is working and upgrade everything that is not.

This category is not a light edit. It is a full rebuild that treats the existing content as raw material, not as a finished draft.

### What Gets Upgraded in Every Rewrite

Every rewrite adds or improves the following, regardless of how much or how little the original post had:

Schema markup: Article schema and BreadcrumbList schema added to Lofty head injection field and at the end of the post body after the style block. FAQPage schema added if an FAQ section is present or being added. All schema written to spec as defined in the shared rules. Use @graph structure.

HTML structure: Style block moved to after the closing content div. Schema moved to after the style block. Universal CSS resets removed and replaced with scoped selectors.

Quick Answer box: Added near the top of the post if not present. Structured specifically for Google Featured Snippet capture and AI Overview inclusion. Three to five sentences answering the post's primary question directly.

FAQ accordion: Added or expanded to minimum six questions if not present. Questions researched for actual search intent not invented. FAQPage schema added to match. Visible questions aligned to schema exactly.

Exception box: Added if not present. Orange or red-bordered callout covering when the main guidance does not apply. Required for Education and Analysis posts.

Brand design system: Full CSS variable block applied. Playfair Display headings. Source Sans 3 body. Gold accents, callout boxes, and component patterns consistent with all other Saling Homes content. Scoped wrapper ID applied. No universal resets.

EEAT signals: Author bio upgraded to styled box format. Data Sources block added where applicable. Data verification timestamp added. Joe's direct observations or local expertise woven into the content to signal genuine first-hand knowledge. Disclaimer added for any post touching financial, legal, or tax topics.

External links: All existing external links updated to include full attribute set: `target="_blank" rel="noopener noreferrer" title="Descriptive Title"`.

CTA URLs: All CTA links verified against the CTA URL Standards table. /home-valuation corrected to /evaluation. Any non-standard URLs corrected.

Internal links: Minimum three internal links confirmed in the SEO spreadsheet. Existing internal links verified and updated if URLs have changed. City guide links updated to use /living-in-\[city\]-oregon format.

Outbound links: All existing outbound links verified active. Any dead links removed or replaced. Minimum five authoritative outbound links present.

Unverified statistics: Any statistic presented as fact without a source is either sourced, reframed as an estimate, or removed.

AEO structure: H2 and H3 hierarchy reviewed and restructured to match question-based search intent where appropriate. Opening paragraph rewritten to lead with the primary search query answer.

GEO signals: Portland-specific local details added or strengthened. Named places, specific addresses, local programs, and Oregon-specific context that AI systems use when composing location-specific answers.

Mobile and Lofty technical: Scoped CSS wrapper ID, lowercase viewBox attributes, table scroll containers, lazy loading on all non-hero images, Lofty margin fix on dark sections.

### Phase 1 — The Audit

When Joe provides the existing HTML, do the following before building anything.

Read the existing post completely. Extract: the core topic and primary argument, all data points and their sources, all named places and local details, all existing internal and outbound links, the current structure and section order.

Run the audit. Check the existing post against every item in the upgrade list above. Present findings in two columns: what is working and worth preserving, and what is missing or substandard and needs to be added or rebuilt.

Identify the post's category. Which of the three active blog categories does this post belong to: Education, Analysis, or Neighborhood Vibe? The rewrite will follow the content architecture of that category.

Identify the primary search query this post is targeting. Research whether the current H1 and meta title are optimized for that query or whether they need to be updated.

Flag any content that needs Joe's input. Missing local details Claude cannot verify. Statistics that cannot be traced to a source. Personal observations that only Joe can provide. Present these as specific questions, not general gaps.

Deliver the audit as a clean structured block. End with: "This audit covers \[number\] items to upgrade and \[number\] items to preserve. Do you have any corrections or additional context to provide before I rebuild? If not, type YES and I will deliver the updated SEO suite followed by the full rebuilt HTML."

### Phase 2 — The Rebuild

When Joe types YES, deliver the updated SEO suite first. Then build the full rebuilt HTML following the content architecture for the post's identified category. Then deliver image briefs for any new image slots added and follow-up content ideas.

The rebuilt post is a complete replacement for the original. It is not a patched version of the original HTML. The content is preserved and improved. The structure, design, and technical implementation are rebuilt from the current standard.

### Tone Notes for Rewrite and Restyle

The rebuilt post inherits the voice and tone register of its category. An education post rewrite is structured and clear. An analysis post rewrite can have Joe's editorial voice. A neighborhood vibe rewrite is personal and conversational.

The one exception: if the original post had a distinctive opening or memorable local observation that worked well, preserve the spirit of it even when rewriting the language. The goal is to upgrade, not to replace Joe's voice with a generic one.

---

## CATEGORY 5: MARBLISM COMPLIANCE PASS

### Purpose

Marblism produces well-structured, well-voiced blog content with good visual layout, strong Key Takeaways sections, back to top navigation, and useful content organization. The Marblism Compliance Pass preserves all of that and applies only what is missing: the Saling Homes design system, Lofty-safe HTML structure, scoped CSS, upgraded schema, FAQ alignment, required components, and citation verification.

This is a surgical pass, not a rebuild. The distinction matters. Category 4 treats the existing HTML as raw material. Category 5 treats the existing HTML as a near-finished post that needs compliance work, not content work.

### The Core Rule

Preserve everything that Marblism produced unless it violates one of three conditions:

1. It contains a forbidden word from the shared rules list.  
2. It presents a statistic as fact with no source attached.  
3. It contains Fair Housing language that steers buyers based on demographics.

Everything else stays. Marblism's sentence structure, paragraph flow, section order, callout content, images, and local detail are all preserved. Do not improve the writing. Do not restructure sections. Do not add content beyond the required components listed below.

### What the Compliance Pass Fixes — Always

Apply every item on this list to every Marblism post without exception.

**HTML Structure:** Restructure the post to follow the mandatory Lofty sequence. Content div first with a unique wrapper ID. Style block after the closing content div. Schema block after the style block. This is the most likely structural issue in any Marblism post and must be corrected before anything else.

**CSS Scoping:** Identify and remove any universal resets (asterisk selectors), body selectors, or html selectors. Scope all CSS to the unique wrapper ID. Adapt the wrapper ID from the post slug prefixed with "post-".

**Font and Color System:** Replace whatever font stack Marblism used with the Saling Homes system. Playfair Display for all headings. Source Sans 3 for all body text, buttons, and labels. Apply the full CSS variable block. Map Marblism's existing colors to the correct Saling Homes values. Gold accents replace any brand-inconsistent accent colors. Near-black (\#222222) replaces any dark hero or callout backgrounds.

**External Link Attributes:** Add `target="_blank" rel="noopener noreferrer" title="Descriptive Title"` to every external link that is missing any of these attributes. Write the title attribute to describe the specific destination.

**CTA URLs:** Verify all CTA destination URLs against the CTA URL Standards table in the shared rules. Correct /home-valuation to /evaluation. Correct any other non-standard URLs. Do not change the CTA button text or surrounding copy, only the href.

**Author Bio:** Replace whatever author credit Marblism included with the standard styled author bio box. Gold left border, light grey background, border-radius 16px. Use the fixed author content from the shared rules. Phone as tel: link. Email as mailto: link.

**EHO Statement:** Add the standard EHO statement at the bottom of every post after the author bio if not already present. Use the exact language from the shared rules.

**Data Verification Timestamp:** Add the data verification timestamp to the Data Sources section or as a standalone line before the author bio. Format: "Data verified: \[Month Year\]." Confirm with Joe what month and year to use if not specified.

**Mobile CSS:** Add both required breakpoints (768px and 480px) scoped to the wrapper ID. Follow the mobile CSS pattern from the Mobile Design Standards section. Adapt class names to match whatever class names Marblism used in the post.

**Schema:** Replace or upgrade whatever schema Marblism included. Build the full @graph structure with Article, BreadcrumbList, and FAQPage (if FAQ is present). Populate all required author fields: name, url, jobTitle, telephone, email, worksFor. Use the actual post URL for @id and BreadcrumbList. Schema goes in the Lofty head injection field and also at the end of the body after the style block.

**FAQ Alignment:** Compare the visible FAQ accordion questions and answers to the FAQPage schema exactly, word for word. If they do not match, align the schema to the visible FAQ. Never alter the visible FAQ content to match the schema. Visible content is what the reader sees. Schema must reflect it accurately.

### What the Compliance Pass Flags — Does Not Fix Automatically

These items require Joe's input or verification before they can be resolved. Flag them clearly in the audit output and do not attempt to fix them without Joe's confirmation.

**Unverified statistics:** Any statistic presented as a specific fact (a percentage, a dollar figure, a count) with no source attached. Flag the specific claim, note that no source was found, and present three options: find and add a source inline, reframe as an estimate, or remove. Joe decides which path to take.

**Images:** Marblism's images are kept exactly as-is. Do not remove, replace, or reposition any image Marblism inserted. If an image has missing or generic alt text, flag it and suggest improved alt text in the format Subject, Location, Oregon. Joe approves before changes are made.

**Disclaimer:** If the post covers tax law, financial guidance, legal topics, or buying process and no disclaimer is present, flag this and ask Joe to confirm before adding. Marblism may have intentionally excluded it.

**Exception box:** If the post is an Education or Analysis post and no exception box is present, flag this as a gap. Do not add one without knowing what the exceptions actually are. Ask Joe to provide the exception content before inserting the box.

### Phase 1 — The Audit

When Joe pastes the Marblism HTML, do the following before building anything.

Read the full HTML. Extract the core topic, primary argument, content category (Education, Analysis, or Neighborhood Vibe), all images, all statistics, all data citations, all existing links, and the current FAQ questions.

Run the compliance check. Compare the post against every item in the two lists above: what gets fixed automatically and what gets flagged. Present the findings in two clearly labeled sections.

Section 1 — Will Fix: list every compliance item that will be corrected in the pass. Be specific. "HTML structure: style block currently before content div, will be moved to after closing div" is better than "HTML structure issues found."

Section 2 — Needs Your Input: list every flagged item with the specific content, the reason it is flagged, and the options for resolving it. Be specific. "Paragraph 3 states 'appreciation rates in the Intel corridor have outpaced the metro by 5-8% annually' with no source. Options: (1) find and cite a source, (2) reframe as 'estimates suggest,' (3) remove the figure."

End the audit with: "This compliance pass will fix \[number\] items automatically and needs your input on \[number\] items. Please respond to each flagged item above, then type YES and I will deliver the updated SEO suite and compliant HTML."

### Phase 2 — The Compliance Build

When Joe provides input on flagged items and types YES, deliver the updated SEO suite first. Then deliver the compliant HTML with all automatic fixes applied and all flagged items resolved per Joe's instructions. Then note any images that need alt text improvements and any follow-up content ideas that emerge naturally from the post topic.

The compliant HTML preserves Marblism's section order, paragraph structure, callout content, and local detail. The only changes are the compliance items listed above plus Joe's instructions on flagged items. If the output looks significantly different from what Marblism produced in terms of content and flow, something went wrong. The design will look different (Saling Homes system vs Marblism defaults) but the words and structure should feel familiar.

### Tone Notes for Marblism Compliance Pass

Do not improve Marblism's writing. Do not add transitional sentences. Do not restructure arguments. Do not punch up language. The compliance pass is not an editing pass. If Marblism's voice on a particular post is slightly less polished than the Saling Homes standard, that is acceptable. What is not acceptable is missing schema, broken Lofty structure, generic fonts, and unverified statistics. Fix the compliance gaps. Leave the content alone.

---

## PHASE 2 — THE BUILD

When Joe types YES, deliver the SEO suite first. Then build the full HTML post. Then deliver image briefs and any recommended follow-up post ideas.

The HTML follows the component patterns established in the city guide template for shared components including callout boxes, FAQ accordions, tables, author bio, CTA blocks, and EHO bar.

Each blog post has a unique wrapper ID scoped CSS block that inherits the CSS variables from the root. Define the wrapper ID based on the post slug prefixed with "post-". Apply all CSS inside that wrapper ID selector to prevent conflicts with Lofty's default styles. Never use universal resets or body selectors.

The HTML structure follows the mandatory Lofty sequence: content div first, style block after the closing div, schema block after the style block.

---

## POST-BUILD DELIVERABLES

After the HTML deliver the following two blocks in plain text.

### Image Brief Block

One brief per image slot used. Minimum 80 words per brief. Every brief must include: the specific visual content, the location name, the time of day and season, the specific physical details that make this image unique to this post, the file name using the naming convention, and the Marbalism-ready prompt formatted for image generation.

### Follow-Up Content Ideas

Two to three ideas for posts that naturally extend this one. For each include: the title, which category it belongs to, the primary search query it targets, and which section of the current post it links back to and with what anchor text.

---

## MOBILE DESIGN STANDARDS

Joe's site is mobile-user heavy. Every post must be fully optimized for mobile screens before it is optimized for anything else. Desktop is secondary. Mobile is primary.

### Breakpoints

Use two breakpoints on every post.

768px: Tablet adjustments. Grids collapse. Floated images go full width. Multi-column layouts adjust.

480px: Phone-specific adjustments. This is the most important breakpoint. Most of Joe's mobile traffic is on screens between 375px and 430px (iPhone 14, 15, and SE sizes). Design for that range first.

### Mobile Font Sizes

Required at the 480px breakpoint. Never let body text drop below 1rem on mobile.

H1: 1.9rem H2: 1.45rem H3: 1.2rem Body text: 1.05rem, line-height 1.85 Captions: 0.82rem Buttons: 1rem, weight 600 FAQ summary text: 0.95rem TOC links: 0.9rem

### Mobile Layout Rules

Floated images: width 100%, float none, margin 0 0 20px 0 at 480px. Never float images on mobile.

Grids: All multi-column grids collapse to single column at 480px. No exceptions.

Tables: Every table wrapped in overflow-x auto scroll container at all screen sizes.

Callout boxes: Padding reduces to 16px 18px at 480px. Full width.

CTA buttons: Stack vertically at 480px. Each button goes width 100%, display block, margin-bottom 12px.

Navigation bars: Horizontally scrollable at 480px with overflow-x auto and \-webkit-overflow-scrolling touch. Never wrap nav items to a second line.

Hero sections: Padding reduces to 40px 20px at 480px.

### Touch Target Sizing

Every tappable element must be minimum 44px tall.

FAQ accordion summaries: min-height 48px, padding 14px 16px, full width tap target.

Buttons: min-height 48px, padding 14px 24px.

Back to top links: display block, min-height 44px.

### Mobile Color and Contrast

Never reduce contrast on mobile. Gold (\#D4AF37) on white fails WCAG AA. Never use gold as body text color on any background. Gold is for borders, accents, and icons only.

Body text: \#444444 on white. Text on dark backgrounds: \#FFFFFF. These combinations pass WCAG AA at all sizes.

### Required Mobile CSS Pattern

Every post includes this block scoped to the post wrapper ID. Adapt class names to match the post being built.

```css
@media (max-width: 768px) {
  #[post-id] .hero { padding: 48px 24px; }
  #[post-id] h1 { font-size: 2.1rem; }
  #[post-id] .editorial-img,
  #[post-id] .editorial-img.left {
    width: 100%;
    float: none;
    margin: 0 0 20px 0;
  }
  #[post-id] .two-col-grid { grid-template-columns: 1fr; }
  #[post-id] .cta-buttons { flex-direction: column; }
  #[post-id] .cta-buttons a { width: 100%; text-align: center; }
}

@media (max-width: 480px) {
  #[post-id] h1 { font-size: 1.9rem; }
  #[post-id] h2 { font-size: 1.45rem; }
  #[post-id] h3 { font-size: 1.2rem; }
  #[post-id] { font-size: 1.05rem; line-height: 1.85; }
  #[post-id] .callout-box { padding: 16px 18px; }
  #[post-id] .hero { padding: 40px 20px; }
  #[post-id] .faq-acc summary { min-height: 48px; padding: 14px 16px; }
  #[post-id] .btn-primary,
  #[post-id] .btn-secondary {
    display: block;
    width: 100%;
    text-align: center;
    margin-bottom: 12px;
    min-height: 48px;
  }
  #[post-id] .data-table-wrap { overflow-x: auto; -webkit-overflow-scrolling: touch; }
  #[post-id] .sh-nav {
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
    scrollbar-width: none;
  }
  #[post-id] .sh-nav::-webkit-scrollbar { display: none; }
}
```

---

## PRE-PUBLISH CHECKLIST

**Content:** Primary question answered in the first 200 words, Quick Answer box present and positioned before the TOC, all statistics traced to named sources, no forbidden words or pressure language, exception box present (Education and Analysis posts), candid counterargument or honest caveat present somewhere in the post, CTA is an invitation not a demand.

**Technical:** HTML structure is content div first, then style block, then schema block. Schema also in Lofty head injection field. All CSS scoped to wrapper ID — no universal resets or body selectors. All viewBox attributes lowercase. Scoped wrapper ID present. Google Fonts link in head. Tables wrapped in scroll container. All images have descriptive alt text. Hero image uses loading eager, all others use loading lazy. No placeholder URLs in schema.

**Mobile:** Both breakpoints present (768px and 480px). Body text minimum 1.05rem at 480px. All floated images removed at 480px. All multi-column grids collapse at 480px. CTA buttons stack vertically at 480px. All tables in scroll containers. FAQ accordion tap targets minimum 48px tall. No gold text on white backgrounds. Nav bar scrolls horizontally at 480px rather than wrapping.

**Links:** Minimum three internal links confirmed in SEO spreadsheet. City guide links use /living-in-\[city\]-oregon format. Minimum five outbound links to authoritative sources. All external links have target="\_blank" rel="noopener noreferrer" title="Descriptive Title". No links to Zillow, Redfin, or Realtor.com in body. All CTA URLs verified against CTA URL Standards table. All URLs verified before publishing.

**SEO:** Meta title 55 to 60 characters confirmed. Meta description 145 to 155 characters confirmed. Slug is keyword-forward and does not include unnecessary dates. FAQPage schema present only when FAQ accordion exists on page. FAQ schema questions match visible FAQ questions exactly.

**Required Components:** Data verification timestamp present. Author bio is styled box format with gold left border. FAQ accordion has minimum six questions. Exception box present on Education and Analysis posts. EHO statement at bottom.

**Fair Housing:** EHO statement present at bottom. No demographic language anywhere. No steering language in neighborhood vibe posts.

**Post-Build:** Image briefs delivered for all image slots. Follow-up content ideas delivered.

---

## AGENT INFORMATION

Fixed. Do not alter.

Name: Joe Saling Company: Saling Homes at eXp Realty Phone: (503) 910-7364 Email: [joe@sellingpdxhomes.com](mailto:joe@sellingpdxhomes.com) Website: [www.sellingpdxhomes.com](http://www.sellingpdxhomes.com)

---

*Saling Homes Blog Post Master File v1.1 | February 2026* *Upload alongside Sellingpdxhomes\_SEO\_Complete.xlsx at the start of every blog post conversation.*  
