# SALING HOMES - COMMUNITY GUIDE MASTER FILE

**Version 3.5 | March 2026**
**sellingpdxhomes.com | Joe Saling | Saling Homes at eXp Realty**

---

## HOW TO USE THIS FILE

This file is fetched from Google Drive at the start of every session via the Drive startup sequence in the project instructions. It is the single source of truth for every build. Do not ask Joe to re-explain the architecture, design system, voice rules, or image system. Everything is here. When something conflicts between this file and anything else in the conversation, this file wins. When something is not covered here, check the Master Master file (also fetched during startup).

Every build runs in two phases. Do not skip Phase 1. Do not begin Phase 2 until Joe approves Phase 1 output.

---

## PHASE 1 - RESEARCH AND APPROVAL

When Joe gives you a city name, stop. Do not write any HTML. Do the following in order.

### Step 1: Confirm Hard Data

Research and present the following for the named city. Cite your source next to each number.

- Median home price (most recent available, note the date)
- Effective property tax rate (Washington County or Clackamas County as applicable)
- School district name and statewide ranking
- Commute time to downtown Portland (drive, peak hours) - required for every city
- Commute time to Portland International Airport (drive) - required for every city
- Top 2 to 3 major employer destinations specific to this city's workforce. Research which employers people in this community actually commute to. Do not default to Nike and Intel unless they are genuinely relevant to this city's commute patterns.
- City population
- Transit reality research: identify what TriMet actually serves this city. Name specific bus lines, MAX stops, or park-and-ride facilities. Note the nearest MAX station even if it requires a short drive. Note whether WES commuter rail serves this city - WES stops only at Beaverton, Merlo Road, Tigard, and Wilsonville. For all other cities do not mention WES.

### Step 2: Confirm Neighborhoods

List 10 to 13 neighborhoods with a one-sentence description and estimated price range for each. Cover the full range of buyer profiles: premium addresses, established family neighborhoods, affordable entry points, walkable urban areas, 55-plus communities if present, and new construction areas. Ask Joe to confirm, correct, or add neighborhoods before proceeding.

### Step 3: Confirm Restaurants and Local Businesses

List a minimum of 14 local restaurants, coffee shops, or bars organized by category: 6 restaurants, 3 bars, 2 cafes, 1 wildcard (food cart, pop-up, or unexpected local spot), 2 anchors (the breakfast/lunch or coffee spots that define the daily rhythm of the city). For each one include the name, address or cross streets, one signature dish or drink, and the website URL. No chains. No generic descriptions. If you cannot find a specific dish or drink for a listing, flag it and ask Joe to fill in the detail.

### Step 4: Confirm Schools

List the top 3 to 6 schools in the district. For each include the school name, level, GreatSchools rating, Niche rating, address, and one specific program that distinguishes it.

### Step 5: City Physical Research

Before writing any image briefs or any content, research and confirm the following physical characteristics of the city.

- Do residential streets have sidewalks?
- What is the dominant home construction era?
- What architectural style dominates residential areas?
- What trees are most common on residential streets?
- Does the city have overhead utility lines on residential streets or are they underground?
- What is the terrain?
- What is the signature geographic feature?
- What does the downtown commercial core look like?
- What is the signature community event?
- What is the primary trail or park system?

### Step 6: Compile Link Inventory

Before presenting the Phase 1 summary, research and compile every outbound link you plan to use in the page, organized by the ten amenity categories defined in the Linking Rules section of this file. Present the full link inventory as a clean list. Flag any category where you could not find strong local links.

### Step 7: Present Phase 1 Summary

Present all confirmed data in one clean block. End with this exact line:

**Does this data meet the Hyper-Utility goal? Type YES to begin Phase 2.**

Do not write any HTML until Joe types YES. When Joe types YES, deliver the full Pre-GO Output Block. Do not begin the HTML build until Joe types GO.

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
- First 60 characters must be complete and meaningful as a standalone snippet. Google truncates display at approximately 60 characters.
- Total title can run up to 70-75 characters. Content beyond 60 is bonus keyword territory useful for ranking but may not display in search results.
- If title exceeds 75 characters, rewrite it. No exceptions.
- City name must come first.
- Do not use the word "guide". Do not use the word "best".
- Format: [City Name] Oregon: [Descriptor] | Saling Homes
- Always show both the snippet preview (chars 1-60) and full character count in the output.

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

**Dimensions by slot - use these exactly, do not substitute:**

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

Mid range: $[X]K - $[X]K
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

## INTERNAL LINK REFERENCE

A file named Sellingpdxhomes_SEO_Complete.xlsx is saved in this project. Read this file directly during Phase 1 Step 6. Never invent a URL. If a URL is not found in this file and is not a standard pattern from the Internal Links section of this file, flag it for Joe to confirm before including it.

---

## PHASE 2 - THE BUILD

Build the full HTML page using the approved Phase 1 data. Follow every rule in this file exactly. Do not improvise design decisions. Do not add sections not listed here. Do not skip sections listed here.

After the HTML, deliver the Schema Block and Link Table as defined in the Post-GO Output Block above.

---

## CONTENT ARCHITECTURE

Build every section in this exact order. Do not reorder. Do not skip any.

A. Editorial Hook
B. Insider Snapshot
C. Neighborhood Navigation Grid
D. Mid-Page CTA Block
E. Cost of Living Deep-Dive
F. City Comparison Table
G. Culinary and Social Landscape
H. Commerce and Shopping
I. Healthcare Access
J. Nature as Infrastructure
K. Academic Excellence
L. Logistics and Commuting
M. FAQ Section
N. Major Employers
O. Things To Do and Local Events
P. Joe's Take
Q. About Joe and CTA
R. Advisor CTA Dark Box
S. Explore More Card Grid
T. Footer Navigation Bar
U. EHO Bar

### Dining Section Standard (v3.3)

The Culinary and Social Landscape section requires a minimum of 14 spots total. The 3 most distinctive are shown visible on load. The remaining 11 are in a collapsed "See all [City Name] dining" expandable block. The breakdown by category must be: 6 restaurants, 3 bars, 2 cafes, 1 wildcard (food cart, pop-up, or unexpected local spot), 2 anchors (the breakfast/lunch or coffee spots that define the daily rhythm of the city). No chains. Every entry must include a specific dish or drink. If you cannot confirm a signature item, flag it for Joe before Phase 2.

### Collapsible Content Sections (v3.3)

Three sections use a visible/collapsed pattern to reduce initial page length while preserving full content:

- **Editorial Hook:** Paragraph 1 visible. Paragraphs 2 and 3 inside a "Read more about [City Name]" expand toggle.
- **Neighborhoods:** 4 cards visible. Remaining cards inside a "Show all [City Name] neighborhoods" expand toggle. Target 10 to 13 total neighborhoods per guide. Research must cover the full range of buyer profiles: premium addresses, family neighborhoods, affordable entry points, walkable urban areas, 55-plus communities if present, and new construction areas. Each card requires a 3 to 4 sentence description with specific local detail, a price range, and a link to either the spoke page (if it exists) or the city listing search. Match the listing search link to the neighborhood character — condos and townhomes neighborhoods link to the condo search, not single-family.
- **Dining:** 3 items visible. Remaining 11 items inside a "See all [City Name] dining" expand toggle. The collapsed dining grid uses 3 columns.

Use a `<details>/<summary>` pattern for all three. Style the summary as a small gold text link with a chevron icon. Do not use JavaScript for these toggles.

### Listing Search Grid (v3.3)

Include a listing search grid block between the Neighborhoods section and the Mid-Page CTA. This block shows: Homes for Sale (primary featured link), Condos, New Construction, Luxury, and three price range tiles (Under $[XXX]K, $[XXX]K-$[XXX]K, $[XXX]K+). Use confirmed Phase 1 price data to set the ranges. This block uses internal links only - all from the SEO spreadsheet or standard URL patterns.

---

## DESIGN SYSTEM

### CSS Variables (unchanged)

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

### Button CSS - CRITICAL FIX (v3.1, updated v3.4)

The global `.sh-guide a` rule sets `color: var(--gold-light)` on all anchor elements. This overrides button text color unless explicitly countered. Use this exact selector chain on every build. Do not simplify it.

**v3.4 note:** Button background was restored to brand gold (`var(--gold-rich)`) after production testing. The v3.1 dark amber (#7A5C00) was rejected on brand grounds. The WCAG AA contrast concern remains valid in principle but brand gold is the accepted standard. Do not change back to dark amber without explicit instruction from Joe.

```css
.btn-primary,
a.btn-primary,
.sh-guide a.btn-primary,
.sh-hero a.btn-primary,
.mid-cta a.btn-primary,
.advisor-cta a.btn-primary {
  display: inline-block;
  background: var(--gold-rich);
  color: #ffffff !important;
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.95rem;
  font-weight: 700;
  letter-spacing: 0.05em;
  padding: 16px 36px;
  border-radius: 6px;
  text-decoration: none;
  border-bottom: none !important;
  box-shadow: 0 4px 16px rgba(212,175,55,0.35);
  transition: background 0.2s, transform 0.15s, box-shadow 0.2s;
}

.btn-primary:hover,
a.btn-primary:hover,
.sh-guide a.btn-primary:hover,
.sh-hero a.btn-primary:hover,
.mid-cta a.btn-primary:hover,
.advisor-cta a.btn-primary:hover {
  background: var(--gold-light);
  color: #ffffff !important;
  transform: translateY(-2px);
  box-shadow: 0 8px 24px rgba(212,175,55,0.45);
  border-bottom: none !important;
}
```

### Secondary Button CSS (v3.4)

The hero section uses a two-button CTA layout: a primary gold button (Contact Joe) and a secondary ghost button (Browse Homes). The btn-secondary component is used in the hero section only. Do not use it on light backgrounds. Mid-page CTA and advisor CTA dark box use btn-primary only.

```css
.btn-secondary,
a.btn-secondary,
.sh-guide a.btn-secondary,
.sh-hero a.btn-secondary {
  display: inline-block;
  background: transparent;
  color: #ffffff !important;
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.95rem;
  font-weight: 700;
  letter-spacing: 0.05em;
  padding: 16px 36px;
  border-radius: 6px;
  text-decoration: none;
  border: 2px solid rgba(255,255,255,0.45) !important;
  transition: border-color 0.2s, background 0.2s;
}

.btn-secondary:hover,
a.btn-secondary:hover,
.sh-guide a.btn-secondary:hover,
.sh-hero a.btn-secondary:hover {
  border-color: rgba(255,255,255,0.9) !important;
  background: rgba(255,255,255,0.08);
  color: #ffffff !important;
}
```

Hero CTA HTML pattern (two-button):

```html
<div class="sh-hero-cta">
  <a class="btn-primary" href="/contact">Contact Joe</a>
  <a class="btn-secondary" href="/listing/single-family-home/[city-slug]">Browse Homes in [City Name]</a>
</div>
```

Hero CTA flex CSS (required for two-button layout):

```css
.sh-hero-cta {
  margin-top: 28px;
  display: flex;
  gap: 16px;
  align-items: center;
  flex-wrap: wrap;
}

@media (max-width: 640px) {
  .sh-hero-cta { flex-direction: column; }
  .sh-hero-cta .btn-primary,
  .sh-hero-cta .btn-secondary { display: block; width: 100%; text-align: center; }
}
```

### Orphaned CSS Brace Rule - CRITICAL (v3.1)

When removing any CSS block during editing, always check the lines immediately following the removed block for orphaned closing braces `}`. A single orphaned brace after a valid CSS rule will invalidate every CSS rule that follows it in the stylesheet. The browser will silently ignore all subsequent rules, causing backgrounds, colors, and layouts to disappear entirely. After any CSS removal, scan the surrounding 10 lines and confirm brace counts are balanced.

### Sticky Navigation - INCLUDED IN TEMPLATE (v3.4)

The sticky pill navigation bar is included in every build. In the HTML, the nav comes immediately after the hero closing tag. A spacer div comes immediately after the nav.

**HTML placement order:**
1. Hero section (`.sh-hero`)
2. Nav element (`id="sh-nav-bar"`)
3. Spacer div (`id="sh-nav-spacer"`)
4. All page sections

**Why this order:** The nav fix/release script uses an IntersectionObserver on the hero. When the hero scrolls out of view, the script adds `is-fixed` to the nav and sets the spacer height to prevent content jump. This approach replaced `position: sticky` which fails consistently in Lofty due to overflow on parent containers.

**Nav fix/release CSS (required):**

```css
.sh-nav.is-fixed {
  position: fixed !important;
  top: 0 !important;
  box-shadow: 0 2px 12px rgba(0,0,0,0.1) !important;
}

.sh-nav.lofty-offset {
  top: 60px !important;
}
```

**Spacer HTML (place immediately after nav closing tag):**

```html
<div id="sh-nav-spacer" style="height:0;"></div>
```

**Nav fix/release script (place at the very end of the page body, before `</div><!-- /.sh-guide -->`):**

```javascript
(function() {
  var nav = document.getElementById('sh-nav-bar');
  var spacer = document.getElementById('sh-nav-spacer');
  var hero = document.querySelector('.sh-hero');
  if (!nav || !spacer || !hero) return;

  function setNavHeight() {
    spacer.style.height = nav.offsetHeight + 'px';
  }

  var heroObserver = new IntersectionObserver(function(entries) {
    entries.forEach(function(entry) {
      if (!entry.isIntersecting) {
        setNavHeight();
        nav.classList.add('is-fixed');
        var loftyHeader = document.querySelector('header.site-header, .lofty-header, #header, .site-header');
        if (loftyHeader && loftyHeader.offsetHeight > 0) {
          nav.classList.add('lofty-offset');
          nav.style.top = loftyHeader.offsetHeight + 'px';
        } else {
          nav.style.top = '0px';
        }
      } else {
        nav.classList.remove('is-fixed');
        nav.classList.remove('lofty-offset');
        nav.style.top = '';
        spacer.style.height = '0';
      }
    });
  }, { threshold: 0, rootMargin: '0px' });

  heroObserver.observe(hero);

  window.addEventListener('resize', function() {
    if (nav.classList.contains('is-fixed')) {
      setNavHeight();
    }
  }, { passive: true });
})();
```

**Required IDs:** The nav must have `id="sh-nav-bar"`. The spacer must have `id="sh-nav-spacer"`. Without both IDs the script exits silently and the nav will not fix on scroll.

**Bullet suppression - REQUIRED (v3.2):** Lofty's theme injects bullets onto list items through four CSS paths. All four must be suppressed on every build:

```css
.sh-nav ul {
  list-style: none !important;
  list-style-type: none !important;
}

.sh-nav li {
  list-style: none !important;
  list-style-type: none !important;
  background-image: none !important;
}

.sh-nav li::before,
.sh-nav li::after {
  display: none !important;
  content: none !important;
}
```

**Do not include:**
- The reading progress bar `<div id="sh-progress">` and its scroll script
- The Intersection Observer active-state script from old template versions

These two elements were removed permanently in v3.1/v3.2 and do not return.

### Lofty Container Fix (unchanged)

Every dark full-width section must use these negative margins:
```
margin-left: -20px;
margin-right: -20px;
```

### SVG Rule (unchanged)

All viewBox attributes must be lowercase: viewBox not ViewBox.

---

## IMAGE SYSTEM

### Image Count

Phase 1 determines the actual number of images required per city guide. The minimum is 7. Some cities require more based on the number of distinctive neighborhoods, transit infrastructure, landmarks, or signature events confirmed in Phase 1 physical research. Do not cap at 7 if more images are genuinely needed to represent the city.

### Required Image Slots

Every city guide requires at minimum these 7 slots. Additional slots are added as Phase 1 warrants.

| Slot | Photo ID format | Section | Dimensions |
|------|----------------|---------|------------|
| Editorial Hook | hero-street-[city] | Editorial Hook | 640 x 480px |
| Landmark / full-width | landmark-[city] | Neighborhoods | 1200 x 600px |
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

Use `flex: 0 0 320px` and a fixed pixel width of 320px on `.editorial-img`. Never use percentage widths on images inside flex containers.

---

## EMAIL ADDRESS IN ABOUT JOE SECTION - LOFTY/CLOUDFLARE NOTE (v3.1)

Cloudflare's email obfuscation script automatically rewrites `mailto:` links and visible email addresses on published Lofty pages. The email will display as `[email protected]` on the live page. This is Cloudflare's spam-protection behavior and is expected.

The HTML file is correct. Do not attempt to fix this in the code. It is a server-level rewrite that happens after publish.

If Joe specifically requires the unobfuscated email to display visibly, the workaround is to break the address into HTML spans:
```html
<span>joe</span>&#64;<span>sellingpdxhomes.com</span>
```
This defeats Cloudflare's detection pattern. Use only if Joe requests it.

---

## MARKET UPDATES LINK - FIXED URL (v3.1)

The Market Updates link in the Explore More section Buyer Resources column must use this exact absolute URL:

```
https://www.sellingpdxhomes.com/blog?categoryId=57180
```

Do not use `/blog` as a relative path. It does not resolve to the market updates category on the live site.

---

## LINKING RULES (unchanged from v3.0)

### Internal Links: Minimum 5 Per Page

```
/listing/single-family-home/[city-slug]
/listing/luxury-home/[city-slug]
/listing/new-construction/[city-slug]
/listing/condos/[city-slug]
/listing/open-house/[city-slug]
/listing/price-reduced/[city-slug]
/living-in-[city]-oregon
/[city-slug]_snapshot
/resources
/sell
/contact
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

Never link to Zillow, Redfin, or Realtor.com.

All external links must include: `target="_blank" rel="noopener noreferrer" title="Descriptive Title"`

---

## VOICE AND TONE RULES (unchanged from v3.0)

---

## FAIR HOUSING COMPLIANCE (unchanged from v3.0)

---

## SCHEMA MARKUP

Schema markup is delivered after the HTML build as part of the Post-GO Output Block. Paste both schema blocks into a Lofty embed block placed at the very top of the page content, before all other HTML. Google reads JSON-LD schema correctly whether it is in the page head or body. Lofty does not have a per-page head injection field — the embed block is the correct method. Do not reference a "head injection field" anywhere in builds or instructions.

Two schema blocks required: RealEstateAgent and FAQPage. FAQPage questions must match visible accordion exactly.

---

## PRE-DELIVERY CHECKLIST

**Content:** (unchanged from v3.0)

**Template Components - UPDATED v3.5:**

- Pre-GO output block delivered before HTML build: SEO suite, image briefs, SNS image brief, neighborhood spoke list, price range tiers with encoded URLs
- Image brief count matches Phase 1 determined count (minimum 7, more if warranted)
- All image briefs include file name, dimensions, slot type, full scene description, and exclusion list
- SNS image brief present at 1200x630
- Neighborhood list includes spoke slug and build status for every neighborhood in guide
- Price range tiers based on Phase 1 market research, not generic round numbers
- Price range URLs built using Lofty Listing Search URL Reference Guide
- Hero CTA uses two-button layout: btn-primary (Contact Joe, links to /contact) and btn-secondary (Browse Homes, links to /listing/single-family-home/[city-slug])
- btn-secondary CSS present in stylesheet with full selector chain
- Hero CTA flex CSS present with mobile stack behavior
- Mid-page CTA block present after Neighborhoods
- Listing search grid present between Neighborhoods and Mid-Page CTA
- Sticky pill navigation bar present immediately after hero closing tag with id="sh-nav-bar"
- Spacer div present immediately after nav with id="sh-nav-spacer"
- Nav fix/release script present at end of page body
- is-fixed and lofty-offset CSS classes present in nav CSS block
- Nav bullet suppression CSS present (list-style, list-style-type, background-image, ::before/::after all set to none !important)
- NO progress bar (removed permanently)
- NO Intersection Observer active-state script (removed permanently)
- Comparison table appears after Cost of Living
- School table has both desktop and mobile card versions
- Commute table has both desktop and mobile card versions
- Comparison table has both desktop and mobile card versions
- Dining section has 3 visible items and 11 collapsed items (14 total minimum)
- Dining collapsed grid uses 3 columns
- Neighborhoods has 4 visible cards and collapsed remainder
- Editorial hook paragraph 1 visible, paragraphs 2-3 in expand toggle
- Joe's Take ends with attribution line only
- Explore More uses two-column card grid format
- Market Updates link uses https://www.sellingpdxhomes.com/blog?categoryId=57180

**Links:** (unchanged from v3.0)

**Technical - UPDATED v3.5:**

- Google Fonts link in head for Playfair Display and Source Sans 3
- All 9 CSS variables defined in root block
- NO progress bar
- NO Intersection Observer active-state script
- Tables wrapped in scroll container
- All viewBox attributes lowercase
- Schema delivered in Post-GO output block, not pre-GO
- Schema instructs paste into Lofty embed block at top of page
- Link table delivered with HTML: internal links table and external links table, both in page order
- All links in HTML appear in link table
- Button CSS uses full selector chain with !important on color and border-bottom
- Button background var(--gold-rich), hover var(--gold-light). Do not use #7A5C00 or #5C4500.
- No orphaned CSS braces after any removed block

**Images - UPDATED v3.5:**

- All image placeholder slots present in correct sections (minimum 7, more if Phase 1 warrants)
- NO duplicate images across any two slots - every slot uses a unique image
- school-exterior and signature-event slots ordered separately from initial 5 if needed
- All img tags have descriptive alt text
- All img tags have loading="lazy" except hero
- editorial-img uses fixed 320px width not percentage

**Mobile:** (unchanged from v3.0)

**Authority signals:** (unchanged from v3.0)

**Fair Housing:** (unchanged from v3.0)

---

## AGENT INFORMATION (unchanged)

Name: Joe Saling
Company: Saling Homes at eXp Realty
Phone: (503) 910-7364
Email: joe@sellingpdxhomes.com
Website: www.sellingpdxhomes.com

---

## VERSION LOG

### v3.5 - March 2026

Six changes from the v3.5 update document.

**Change 1 - Pre-GO Output Block defined:** Replaces the empty POST-BUILD DELIVERABLES section and moves the SEO suite into a structured pre-GO block. The block has six parts delivered in order after Joe types YES: SEO suite, image briefs with slot-specific dimensions and Phase 1-determined count, SNS image brief, neighborhood spoke list with build status, price range tiers with encoded Lofty search URLs, and a closing prompt to send briefs to Marbalism and type GO.

**Change 2 - Post-GO Output Block defined:** When Joe types GO, deliver in order: full HTML, schema block (labeled copy-paste block for Lofty embed), and link table (internal and external, both in page order).

**Change 3 - Meta title rule updated:** First 60 characters must be complete and meaningful as a standalone snippet. Total title runs up to 70-75 characters. Output must show snippet preview (chars 1-60) and full character count. Rewrite required if over 75 characters.

**Change 4 - Image brief format standardized:** Slot-specific dimensions table added. Phase 1 determines actual image count — minimum 7, no cap if more are warranted. Required brief fields: file name, dimensions, slot type and section, full scene description paragraph, exclusion list.

**Change 5 - Neighborhood count raised to 10-13:** Phase 1 Step 2 and Collapsible Content Sections both updated. Research must cover full range of buyer profiles. Neighborhood cards must include price range and correct listing search link matched to neighborhood character.

**Change 6 - Lofty Search URL Construction rule added to Linking Rules:** Never guess at a search URL structure. Never construct a condition URL from memory. Use the Lofty Listing Search URL Reference Guide in project files. Base URL for condition-filtered searches is https://www.sellingpdxhomes.com/cities/[city-or].

**Change 7 - Schema placement corrected:** Schema no longer references "head injection field." Correct method is Lofty embed block at top of page. Schema delivered in Post-GO block, not pre-GO. Three pre-delivery checklist items moved to Post-GO verification.

### v3.4 - March 2026

Three changes from the Tigard v2 production session.

**Change 1 - Button color restored to brand gold:** Background reverted from #7A5C00 (dark amber, v3.1) to var(--gold-rich)/var(--gold-light). Production testing rejected dark amber on brand grounds. Gold is the accepted standard. WCAG contrast tradeoff is documented and accepted. Do not change back to dark amber without explicit instruction.

**Change 2 - Nav fix/release script replaces position:sticky:** position:sticky fails consistently in Lofty due to overflow on parent containers. Replaced with IntersectionObserver approach: nav watches hero bottom edge, adds .is-fixed class when hero scrolls out, spacer div prevents content jump. Nav now placed after hero in HTML (not before). Required IDs: id="sh-nav-bar" on nav, id="sh-nav-spacer" on spacer. Script placed at end of page body.

**Change 3 - btn-secondary ghost button added:** Hero section now uses two-button CTA layout. btn-secondary is a transparent/outline button for dark backgrounds only. Used in hero section exclusively. Full selector chain and !important flags required same as btn-primary.

### v3.3 - March 2026

Three content architecture additions from Northwest Portland guide session.

**Addition 1 - Dining section standard:** Minimum 14 spots required per guide. Breakdown: 6 restaurants, 3 bars, 2 cafes, 1 wildcard, 2 anchors. 3 visible on load, 11 in collapsed expand block. Collapsed grid uses 3 columns.

**Addition 2 - Collapsible content sections:** Editorial hook, Neighborhoods, and Dining all use details/summary expand toggles to reduce initial page length. No JavaScript - native HTML only.

**Addition 3 - Listing search grid:** Added between Neighborhoods and Mid-Page CTA. Shows primary Homes for Sale link plus Condos, New Construction, Luxury, and three price range tiles using confirmed Phase 1 data.

### v3.2 - March 2026

Nav restored after v3.1 removal. Bullet suppression CSS added. Position sticky retained (later replaced in v3.4).

### v3.1 - March 2026

Six fixes from Tigard city guide build session: button selector chain, button contrast (dark amber, later reversed in v3.4), Cloudflare email obfuscation documentation, Market Updates absolute URL fix, duplicate image rule, orphaned CSS brace warning.

### v3.0 - March 2026

Template updated from v1.1 to v1.2. Full mobile design standards. Seven layout brief changes. Eight mobile improvements.

### v2.9 - February 2026

Full Mobile Design Standards added.

---

*Saling Homes Community Guide Master File v3.5 | March 2026*
*Stored in SH Master Files folder in Google Drive. Fetched at the start of every session via the Drive startup sequence.*
