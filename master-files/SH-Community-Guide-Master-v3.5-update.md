# Saling Homes - Community Guide Master
## Version Log Addendum: v3.5
**March 2026 | sellingpdxhomes.com | Joe Saling | Saling Homes at eXp Realty**

---

## How to Use This Document

This file documents all changes between v3.4 and v3.5. Apply every change to SH-Community-Guide-Master-v3.4.md. The end state is SH-Community-Guide-Master-v3.5.md saved to Drive, replacing v3.4.

**Starting point:** SH-Community-Guide-Master-v3.4.md
**End state:** SH-Community-Guide-Master-v3.5.md

---

## Summary of Changes

Six changes in this version:

1. Pre-GO output block defined (replaces empty POST-BUILD DELIVERABLES section)
2. Post-GO output block defined (HTML + schema + link table)
3. Meta title rule updated (60-char clean snippet, 70-75 char total)
4. Image brief format defined with slot-specific dimensions and Phase 1-determined count
5. Neighborhood list with spoke status added to pre-GO output
6. Lofty search URL construction rule added to Linking Rules

---

## Change 1 - Pre-GO Output Block

### What to replace

Find this line in the master file:

```
Do not write any HTML until Joe types YES. When Joe types YES, deliver the SEO suite immediately before starting the build.
```

Replace with:

```
Do not write any HTML until Joe types YES. When Joe types YES, deliver the full Pre-GO Output Block. Do not begin the HTML build until Joe types GO.
```

### What to add

Replace the entire SEO SUITE section and the empty POST-BUILD DELIVERABLES section with the following two new sections:

---

## PRE-GO OUTPUT BLOCK

Deliver this complete block immediately after Joe types YES. Do not begin any HTML until Joe types GO. This block gives Joe everything needed to review data, send images to Marbalism, and confirm the build is ready to proceed.

Deliver the six parts in this exact order.

---

### Part 1: SEO Suite

Present as a clean labeled block formatted for direct copy-paste into Lofty.

```
SEO SUITE: [CITY NAME], OREGON

Page Slug:
/living-in-[city-slug]-oregon

Meta Title:
[Title text]
Snippet preview (chars 1-60): [first 60 characters of title]
Full title ([X] chars): [WITHIN LIMIT / OVER LIMIT — rewrite if over 75]

Meta Description:
[Description text]
Character count: [X] — [WITHIN 145-155 / FLAG: over or under with rewrite]

Keywords:
[keyword 1]
[keyword 2]
[keyword 3]
[keyword 4]
[keyword 5]
[keyword 6]
[keyword 7]
[keyword 8]
[add more as needed]
```

**Meta title rules:**
- First 60 characters must be complete and meaningful as a standalone snippet. Google displays approximately 60 characters in search results before truncating.
- Total title can run up to 70-75 characters. Content beyond 60 characters is bonus keyword territory — useful for ranking but may not display in search results.
- If the title exceeds 75 characters, rewrite it. No exceptions.
- Format: [City Name] Oregon: [Descriptor] | Saling Homes

**Meta description rules:**
- 145 to 155 characters. Hard limits. Rewrite until it fits.
- Must include: city name, one specific local detail (trail name, school district, landmark), soft invitation to read.
- No exclamation points. No superlatives.
- Count characters before delivering.

**Keywords rules:**
- Each keyword hard stopped at 60 characters.
- Keywords support and reinforce the meta title and description.
- Include: neighborhood names, school district name, commute destinations confirmed in Phase 1, lifestyle terms specific to this city, property type terms.
- No generic Portland metro terms that apply to every city.
- Minimum 8 keywords, no maximum.

---

### Part 2: Image Briefs

Phase 1 determines the actual number of images required. The minimum is 7. Some cities require more based on the number of distinctive neighborhoods, transit infrastructure, landmarks, or signature events confirmed in Phase 1. Do not cap at 7 if more are genuinely needed.

Present a brief for every required image. Number them sequentially.

**Dimensions by slot — use these exactly, do not substitute:**

| Slot type | Dimensions | Notes |
|-----------|-----------|-------|
| Editorial inline | 640 x 480px | Renders in 320px wide CSS container at 2x retina |
| Landmark / full-width | 1200 x 600px | Spans full content width below neighborhood grid |
| Joe portrait | 400 x 500px | Renders in 200px wide container, portrait orientation |
| SNS / Open Graph | 1200 x 630px | Social sharing image, see Part 3 |

**Required brief format for every image:**

```
Image [N]: [Descriptive title]
File name: [city-feature-cityslug].webp
Dimensions: [W x H px]
Slot: [Slot type] — [Section name]

[Full scene description paragraph. Must include all of the following drawn from Phase 1 physical research:
- Specific named location (street, trail, park, building — not generic)
- Architectural style and construction era confirmed in Phase 1
- Tree species confirmed in Phase 1
- Whether utility lines are visible or underground per Phase 1
- Terrain and elevation character per Phase 1
- Lighting direction, time of day, season
- Mood description in one sentence
- What this image must communicate to a relocation buyer]

Exclude: [Specific exclusion list — at minimum: other city signage, tropical vegetation, generic suburban elements that could be any city, anything contradicting Phase 1 physical research]
```

**Brief quality standard:** Every brief must be specific enough that Marbalism could photograph the correct location without asking a follow-up question. If Phase 1 physical research is incomplete, do not write briefs — flag the gap and ask Joe before proceeding.

**File naming convention:** [city-feature-cityslug].webp. Examples: hero-street-tigard.webp, landmark-view-lake-oswego.webp, joe-in-beaverton.webp

**school-exterior and signature-event** almost always require a second Marbalism order. Flag this clearly in the image brief block. Order all briefs at once but note to Joe which slots may arrive separately.

---

### Part 3: SNS Image Brief

Every city guide requires one dedicated social sharing image for Open Graph (Facebook, Instagram, LinkedIn previews).

```
SNS IMAGE: [CITY NAME]
File name: sns-[city-slug].webp
Dimensions: 1200 x 630px
Slot: Open Graph social sharing image

[Scene description. This should be the single most compelling visual representation of this city. Options in priority order:
1. The landmark or signature geographic feature at its most dramatic
2. The primary trail or park at peak Pacific Northwest character
3. A residential street scene that immediately communicates the neighborhood quality

The image must work as a standalone ambassador for the city — someone seeing this on a social feed with no context should immediately understand why this city is worth clicking on.

Same format as image briefs: specific location, Phase 1 physical research details, lighting, mood, exclusion list.]
```

---

### Part 4: Neighborhood List with Spoke Status

List every neighborhood confirmed in Phase 1 and included in the neighborhood section of the guide. For each one provide the spoke page slug and build status.

```
NEIGHBORHOOD SPOKE STATUS: [CITY NAME]

Neighborhood name | Spoke slug | Status
---
[Neighborhood 1] | /living-in-[neighborhood-slug]-oregon | NEEDS TO BE BUILT
[Neighborhood 2] | /living-in-[neighborhood-slug]-oregon | NEEDS TO BE BUILT
[Neighborhood 3] | /living-in-[neighborhood-slug]-oregon | EXISTS — link from card
[etc.]

Spokes to build: [X]
Spokes that exist: [X]
Total neighborhoods in guide: [X]
```

**Linking rule:** If a spoke page exists, the neighborhood card in the guide links directly to that spoke page URL. If no spoke exists, the card links to the city listing search. Check the SEO spreadsheet for existing spoke URLs before assigning status. Never invent a spoke URL — if it is not in the SEO spreadsheet, mark it as NEEDS TO BE BUILT.

---

### Part 5: Price Range Tiers

Research the actual market for this city using Phase 1 median price data and confirmed neighborhood price ranges. Define three tiers that reflect real buyer segments in this city, not generic round numbers.

```
PRICE RANGE TIERS: [CITY NAME]

Entry level: Under $[X]K
[One sentence on what a buyer gets at this price point in this city — specific neighborhood or housing type]
Search URL: https://www.sellingpdxhomes.com/cities/[city-or]?listingSource=all%20listings&condition=[encoded-condition-with-price-max]&uiConfig=%7B%7D&zoom=15&page=1

Mid range: $[X]K – $[X]K
[One sentence on what a buyer gets at this price point]
Search URL: https://www.sellingpdxhomes.com/cities/[city-or]?listingSource=all%20listings&condition=[encoded-condition-with-price-min-and-max]&uiConfig=%7B%7D&zoom=15&page=1

Upper range: $[X]K+
[One sentence on what a buyer gets at this price point]
Search URL: https://www.sellingpdxhomes.com/cities/[city-or]?listingSource=all%20listings&condition=[encoded-condition-with-price-min]&uiConfig=%7B%7D&zoom=15&page=1
```

Build each URL using the Lofty Listing Search URL Reference Guide in the project files. Price range tiles show all property types for the whole city — do not add a property type filter. Include all three active listing statuses: Active, Active Bumpable, BumpableBuyer.

---

### Part 6: End of Pre-GO Block

Close the block with this exact line:

```
Review complete? Send image briefs to Marbalism. Type GO when ready to build.
```

---

## POST-GO OUTPUT BLOCK

When Joe types GO, deliver three things in this order:

**1. Full HTML**
Build the complete city guide HTML using the approved Phase 1 data and the template. Follow all rules in this master file exactly.

**2. Schema Block**
Deliver immediately after the HTML. Present as a clearly labeled copy-paste block.

```
SCHEMA MARKUP: [CITY NAME]
Paste into a Lofty embed block at the very top of the page, before all other content.

[RealEstateAgent schema block]
[FAQPage schema block — questions must match the visible FAQ accordion exactly]
```

Schema placement note: Lofty does not have a per-page head injection field. Use a Lofty embed block placed at the top of the page content. Google reads JSON-LD schema correctly in the page body. Do not reference a "head injection field" anywhere in the build.

**3. Link Table**
Deliver immediately after the schema block. Present as two clean tables for Joe to test every link before publishing.

```
LINK TABLE: [CITY NAME]

INTERNAL LINKS
| # | Anchor Text | URL | Section |
|---|-------------|-----|---------|
| 1 | [text] | [url] | [section name] |
[all internal links in page order]

EXTERNAL LINKS
| # | Anchor Text | URL | Section | Opens new tab |
|---|-------------|-----|---------|---------------|
| 1 | [text] | [url] | [section name] | Yes |
[all external links in page order]
```

Every link in the HTML must appear in this table. If a link appears in the HTML but not the table, it was missed. Use this table to test every URL before publishing.

---

## Change 2 - Meta Title Rule Update

### What to replace

Find this text in the SEO SUITE section (now part of Pre-GO Output Block Part 1):

```
Meta Title: [City Name] Oregon: Neighborhoods, Schools and Real Estate | Saling Homes
Rules: 55 to 60 characters maximum. City name must come first. Do not use the word guide. Do not use the word best. Count the characters before delivering.
```

Replace with:

```
Meta Title rules:
- First 60 characters must be complete and meaningful as a standalone snippet. Google truncates display at approximately 60 characters.
- Total title can run up to 70-75 characters. Content beyond 60 is bonus keyword territory useful for ranking but may not display in search results.
- If title exceeds 75 characters, rewrite it. No exceptions.
- City name must come first.
- Do not use the word "guide". Do not use the word "best".
- Format: [City Name] Oregon: [Descriptor] | Saling Homes
- Always show both the snippet preview (chars 1-60) and full character count in the output.
```

---

## Change 3 - Image System Section Update

### What to replace

Find the entire IMAGE SYSTEM section in the master file and replace it with:

```
## IMAGE SYSTEM

### Image Count

Phase 1 determines the actual number of images required per city guide. The minimum is 7. Some cities require more based on the number of distinctive neighborhoods, transit infrastructure, landmarks, or signature events confirmed in Phase 1 physical research. Do not cap at 7 if more images are genuinely needed to represent the city.

### Required Image Slots

Every city guide requires at minimum these 7 slots. Additional slots are added as Phase 1 warrants.

| Slot | Photo ID format | Section | Dimensions |
|------|----------------|---------|------------|
| Editorial Hook | hero-street-[city] | Editorial Hook | 640 x 480px |
| Landmark | landmark-[city] | Neighborhoods | 1200 x 600px |
| Dining | dining-local-[city] | Culinary Section | 640 x 480px |
| Primary trail/park | [trail-name]-[city] | Nature Section | 640 x 480px |
| Secondary park | [park-name]-[city] | Nature Section | 640 x 480px |
| School exterior | school-exterior-[city] | Schools Section | 640 x 480px |
| Signature event | [event-name]-[city] | Events Section | 640 x 480px |
| SNS / Open Graph | sns-[city] | Social sharing | 1200 x 630px |

school-exterior and signature-event almost always require a second Marbalism order. Flag this in the image brief block. Leave placeholder SVGs rather than reuse images from other slots.

### No Duplicate Images

Every image slot must use a unique image. Never reuse an image from another slot as a temporary placeholder. Duplicate images on a single page undermine credibility with relocation buyers.

### Brief Quality Standard

Every brief must be specific enough that Marbalism could photograph the correct location without asking a follow-up question. Briefs are written from Phase 1 physical research data. If Phase 1 Step 5 is incomplete, do not write briefs — flag the gap first.

Required brief fields: file name, dimensions, slot type and section, full scene description paragraph, exclusion list.

See Pre-GO Output Block Part 2 for the complete brief format.

### Lofty-Safe Image Layout Rules

Use flex: 0 0 320px and a fixed pixel width of 320px on .editorial-img. Never use percentage widths on images inside flex containers.
```

---

## Change 4 - Neighborhood Count Standard

### What to replace

Find this text in the Collapsible Content Sections subsection:

```
- **Neighborhoods:** 4 cards visible. Remaining cards (up to 8 total) inside a "Show all [City Name] neighborhoods" expand toggle.
```

Replace with:

```
- **Neighborhoods:** 4 cards visible. Remaining cards inside a "Show all [City Name] neighborhoods" expand toggle. Target 10 to 13 total neighborhoods per guide. Research must cover the full range of buyer profiles: premium addresses, family neighborhoods, affordable entry points, walkable urban areas, 55-plus communities if present, and new construction areas. Each card requires a 3 to 4 sentence description with specific local detail, a price range, and a link to either the spoke page (if it exists) or the city listing search. Match the listing search link to the neighborhood character — condos and townhomes neighborhoods link to the condo search, not single-family.
```

### What to update in Phase 1 Step 2

Find:

```
List 6 to 8 neighborhoods with a one-sentence description and estimated price range for each.
```

Replace with:

```
List 10 to 13 neighborhoods with a one-sentence description and estimated price range for each. Cover the full range of buyer profiles: premium addresses, established family neighborhoods, affordable entry points, walkable urban areas, 55-plus communities if present, and new construction areas. Ask Joe to confirm, correct, or add neighborhoods before proceeding.
```

---

## Change 5 - Linking Rules Update

### What to add

In the LINKING RULES section, after the internal links list and before "Never link to Zillow," add:

```
### Lofty Search URL Construction

When a city guide requires a filtered search link beyond the standard internal page patterns above — including price range tiles, waterfront properties, view homes, new construction condition searches, or any other condition-based search — build the URL using the Lofty Listing Search URL Reference Guide saved in the project files.

Never guess at a search URL structure. Never construct a condition URL from memory.

If the Lofty Listing Search URL Reference Guide is not available in the project files, ask Joe to add it before building any condition-based links.

The base URL for all city search pages is:
https://www.sellingpdxhomes.com/cities/[city-or]

City slug format is [cityname]-or. Examples: tigard-or, beaverton-or, lake-oswego-or.

Price range tile searches use the /cities/[city-or] base with a price condition only — no property type filter. Show all property types for the whole city.

Standard listing page links (/listing/single-family-home/[city], /listing/condos/[city], etc.) remain correct for linking to those dedicated SEO pages. The /cities/ base is used for condition-filtered searches, not as a replacement for listing page links.
```

---

## Change 6 - Schema Placement Correction

### What to replace

Find this text in the SCHEMA MARKUP section:

```
Schema markup always goes in the Lofty head injection field, never in the page body.
```

Replace with:

```
Schema markup is delivered after the HTML build as part of the Post-GO Output Block. Paste both schema blocks into a Lofty embed block placed at the very top of the page content, before all other HTML. Google reads JSON-LD schema correctly whether it is in the page head or body. Lofty does not have a per-page head injection field — the embed block is the correct method. Do not reference a "head injection field" anywhere in builds or instructions.
```

---

## Pre-Delivery Checklist Updates

Add to the Template Components checklist:

```
- Pre-GO output block delivered before HTML build: SEO suite, image briefs, SNS image brief, neighborhood spoke list, price range tiers with encoded URLs
- Image brief count matches Phase 1 determined count (minimum 7, more if warranted)
- All image briefs include file name, dimensions, slot type, full scene description, and exclusion list
- SNS image brief present at 1200x630
- Neighborhood list includes spoke slug and build status for every neighborhood in guide
- Price range tiers based on Phase 1 market research, not generic round numbers
- Price range URLs built using Lofty Listing Search URL Reference Guide
```

Add to the Technical checklist:

```
- Schema delivered in Post-GO output block, not pre-GO
- Schema instructs paste into Lofty embed block at top of page
- Link table delivered with HTML: internal links table and external links table, both in page order
- All links in HTML appear in link table
```

Remove from the Technical checklist:

```
- Schema markup present (RealEstateAgent + FAQPage)
- FAQPage schema questions match visible FAQ exactly
- knowsAbout field contains city-specific terms
```

These three items move to the Post-GO output block verification, not the pre-delivery HTML checklist.

---

## Version Log Summary Row

Add this row to the Version Log:

| v3.5 | March 2026 | Pre-GO output block defined: SEO suite, image briefs with slot-specific dimensions and Phase 1-determined count, SNS image brief, neighborhood spoke list, price range tiers with encoded Lofty URLs. Post-GO output block defined: HTML, schema block, internal and external link table. Meta title rule updated to 60-char clean snippet with 70-75 char total limit. Image brief format standardized. Neighborhood count raised to 10-13. Lofty search URL construction rule added to Linking Rules. Schema placement corrected from head injection to Lofty embed block. |

---

## Files to Update

| File | Changes |
|------|---------|
| SH-Community-Guide-Master-v3.4.md | All 6 changes above. Save as v3.5. |
| SH-Community-Guide-Template-v1.4.html | Update schema comment block: remove "HEAD INJECTION FIELD" reference, replace with "LOFTY EMBED BLOCK AT TOP OF PAGE". |
| SH-Content-System-Version-Log | Update Community Guide Master to v3.5, Community Guide Template to v1.5 (minor schema comment fix). |

## New Project File to Add

| File | Where |
|------|-------|
| Lofty-Listing-Search-URL-Reference.md | City Guide Project files alongside SEO spreadsheet. Also save to SH Master Files folder in Google Drive. |

---

## HQ Execution Checklist

- [ ] Fetch SH-Community-Guide-Master-v3.4.md from Drive
- [ ] Apply Change 1: Replace workflow trigger sentence, add Pre-GO Output Block section, add Post-GO Output Block section
- [ ] Apply Change 2: Replace meta title rules in SEO suite
- [ ] Apply Change 3: Replace entire IMAGE SYSTEM section
- [ ] Apply Change 4: Update neighborhood count in Collapsible Content Sections and Phase 1 Step 2
- [ ] Apply Change 5: Add Lofty Search URL Construction subsection to Linking Rules
- [ ] Apply Change 6: Replace schema placement instruction
- [ ] Update Pre-Delivery Checklist per checklist updates above
- [ ] Update version number in file header to v3.5
- [ ] Update version number in file footer to v3.5
- [ ] Add v3.5 row to Version Log section
- [ ] Save as SH-Community-Guide-Master-v3.5.md
- [ ] Upload to SH Master Files folder in Drive, replacing v3.4
- [ ] Update template schema comment block, save as v1.5
- [ ] Upload Lofty Listing Search URL Reference Guide to City Guide Project and Drive
- [ ] Update SH-Content-System-Version-Log to reflect v3.5 as current

---

*Saling Homes Content System | Community Guide Master Version Log Addendum v3.5 | March 2026*
*Prepared for Content System HQ | joe@sellingpdxhomes.com*
