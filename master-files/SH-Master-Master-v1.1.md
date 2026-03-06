# SALING HOMES \- MASTER MASTER FILE

**Version 1.1 | March 2026** **Joe Saling | Saling Homes at eXp Realty | sellingpdxhomes.com**

---

## PURPOSE OF THIS FILE

This file is the connective tissue across all five Saling Homes content projects. Every project loads this file at the start of every session. It tells each project what the other projects do, where to find governing files, what URLs are valid, what brand rules are universal, and when to redirect Joe to a different project instead of attempting work that belongs elsewhere.

This file does not replace any master file. It sits above them. When this file and a project master file conflict, the project master file wins for that project's specific work. When something is not covered in a project master file, look here first.

This file does NOT track version numbers. The SH-Content-System-Version-Log is the single source of truth for which version of each master file is current. Check the Version Log at the start of every session to determine which files to fetch.

---

## THE FIVE PROJECTS AND WHAT EACH ONE DOES

### 1\. Blog Post Project

**Builds:** Standalone blog posts at /blog/\[post-slug\] **Five categories:** Education Posts, Analysis and Strategy Posts, Neighborhood Vibe Posts, Rewrite and Restyle, Marblism Compliance Pass **Governed by:** SH-Blog-Master (current version listed in Version Log) **Does NOT:** Build city guides, neighborhood guides, or market reports. If Joe asks for any of those here, redirect him.

### 2\. City Guide Project

**Builds:** Full city guides at /living-in-\[city\]-oregon **Covers:** Neighborhoods, schools, dining, transit, employment, cost of living, parks, Joe's Take **Governed by:** SH-Community-Guide-Master (current version listed in Version Log) **HTML template:** SH-Community-Guide-Template (current version listed in Version Log) **Does NOT:** Build blog posts, neighborhood spoke pages, or market reports. If Joe asks for those here, redirect him.

### 3\. Neighborhood Guide Project

**Builds:** Neighborhood spoke pages that link back to parent city guide hubs **URL pattern:** /neighborhoods/\[neighborhood-slug\]-\[city-slug\] **Governed by:** SH-Neighborhood-Guide-Master (current version listed in Version Log) **HTML template:** SH-Neighborhood-Guide-Template (current version listed in Version Log) **Dependency:** Every neighborhood guide requires a parent city guide. If the city guide does not exist yet, flag this before building. **Does NOT:** Build city guides, blog posts, or market reports. If Joe asks for those here, redirect him.

### 4\. Market Report Project

**Builds:** Monthly RMLS-based market reports at /blog/\[month\]-\[year\]-portland-metro-real-estate-market-update **Data sources:** RMLS PDF files, SentriLock lockbox activity data, Freddie Mac, NAR, web search for external context **Governed by:** SH-Market-Report-Master (current version listed in Version Log) **Does NOT:** Build city guides, neighborhood guides, or general blog posts. If Joe asks for those here, redirect him.

### 5\. Content System HQ

**Purpose:** Architectural decisions, cross-project gap analysis, master file maintenance, version control, system improvements, brand strategy, lead generation, website design, follow-up systems. **Does NOT:** Build content of any kind. If Joe asks for content to be built here, redirect him to the correct project. Exception: troubleshooting existing content by reviewing pasted HTML is acceptable here.

---

## GOOGLE DRIVE REFERENCE LIBRARY

**SH Master Files folder ID:** 1mFuA1Iaj-xa7xxmdUX9L\_SyErgRj1kNb

All master files, templates, and this file are stored in this folder. At the start of every session:

1. Fetch and read SH-Content-System-Version-Log from this folder.  
2. Check the Section 1 table for the current version of whatever master file this project uses.  
3. Fetch and read that master file from Drive.  
4. If the project uses an HTML template, fetch that as well.

Do not rely on memory or previously seen versions. The Version Log is the source of truth for which file versions are current. If Drive is unavailable, tell Joe before proceeding.

**SEO spreadsheet:** Sellingpdxhomes\_SEO\_Complete.xlsx is a project file in every project. Read it directly when validating internal links. Never invent a URL that is not in this spreadsheet or the standard URL patterns listed below.

---

## UNIVERSAL URL PATTERNS

These URL patterns are valid across all projects. Use them. Do not invent variations.

**City guides:** /living-in-\[city\]-oregon Example: /living-in-tigard-oregon, /living-in-beaverton-oregon

**Neighborhood guides:** /neighborhoods/\[neighborhood-slug\]-\[city-slug\] Example: /neighborhoods/sexton-mountain-beaverton

**Blog posts:** /blog/\[post-slug\] Example: /blog/january-2026-portland-metro-market-update

**Market reports:** /blog/\[month\]-\[year\]-portland-metro-real-estate-market-update Example: /blog/january-2026-portland-metro-real-estate-market-update

**Listing searches:**

- /listing/single-family-home/\[city-slug\]  
- /listing/luxury-home/\[city-slug\]  
- /listing/new-construction/\[city-slug\]  
- /listing/condos/\[city-slug\]  
- /listing/open-house/\[city-slug\]  
- /listing/price-reduced/\[city-slug\]  
- /listing/single-level-home/\[city-slug\]

**Standard CTAs (these are the only valid CTA URLs):**

- /evaluation \- Home valuation / seller CTA  
- /snapshot \- Market data  
- /contact \- Contact Joe  
- /sell \- Thinking about selling  
- /listings \- Browse listings  
- /resources \- Buyer's guide  
- /home-buying-process \- How it works  
- /blog \- Market updates  
- /cities \- Explore all communities  
- /about \- About Joe

**City market snapshots:** /\[city-slug\]\_snapshot Example: /tigard\_snapshot

NEVER use /home-valuation. The correct URL is /evaluation. NEVER link to Zillow, Redfin, or Realtor.com in any content body.

---

## UNIVERSAL BRAND RULES

These rules apply to every piece of content across all five projects. They are not repeated in full in each master file but they govern everything.

### Design System \- Fixed Values

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

Headings: Playfair Display (400, 600, 700 weights) Body, buttons, nav, UI: Source Sans 3 (300, 400, 600 weights) Google Fonts link required in every page head.

Gold is never used as body text on light backgrounds. Gold is for accents, borders, dividers, and icons only.

### Forbidden Words \- All Content

Never use: stunning, breathtaking, charming, nestled, vibrant, gem, hidden gem, wonderful, amazing, incredible, world-class, unmatched, guru, ninja, expert (as Joe's self-description), don't miss, act now, limited time, seamlessly, game-changer, synergy.

### Voice Rules \- All Content

Educational over salesy. Direct but warm. Confident without arrogant. Personal and human. CTAs are invitations, never demands. "When you're ready, I'm here" not "Act now." No promises about outcomes. No pressure language of any kind.

### Fair Housing \- All Content

Never describe a neighborhood, city, or area using demographic language. Never imply a buyer should choose a location based on who lives there. Every page ends with the EHO statement naming all 7 protected classes: race, color, religion, sex, handicap, familial status, and national origin.

### Lofty Technical Rules \- All Content

Mandatory HTML sequence for every post and page:

1. Content div with unique wrapper ID  
2. Style block AFTER the closing content div  
3. Schema block AFTER the style block

All CSS scoped to wrapper ID. No universal resets. No body or html selectors. All viewBox attributes lowercase. Dark full-width sections use margin fix: margin-left \-20px, margin-right \-20px. Schema also goes in Lofty head injection field.

### External Links \- All Content

Every external link must include all three attributes: target="\_blank" rel="noopener noreferrer" title="Descriptive Title of Destination". No exceptions.

### Mobile \- All Content

Mobile is primary. Desktop is secondary. Two required breakpoints: 768px and 480px. Body text never below 1rem on mobile (use 1.05rem minimum). All tables in overflow-x auto scroll containers. All floated images go full width at 480px. All multi-column grids collapse to single column at 480px. CTA buttons stack vertically at 480px, width 100%, min-height 48px. Touch targets minimum 44px tall.

---

## HOW THE HUB AND SPOKE SYSTEM WORKS

City guides are hubs. Neighborhood guides are spokes. Blog posts can link to either.

**City guide to neighborhood guide:** When a neighborhood guide exists for a neighborhood mentioned in a city guide, the city guide neighborhood card links to that neighborhood guide page. When Joe creates a new neighborhood guide, the parent city guide neighborhood grid should be updated to add that link.

**Neighborhood guide to city guide:** Every neighborhood guide links back to its parent city guide at least twice. Once in the Editorial Hook section with a clear callout, and again naturally in any section that defers to the city guide for broader context (schools district data, healthcare, commute tables, cost of living).

**Blog posts to city and neighborhood guides:** Blog posts that cover topics specific to a city or neighborhood link to the relevant city guide using /living-in-\[city\]-oregon and to neighborhood guides where they exist. Blog posts never use /cities/\[city-slug\] format for city guide links. Always use /living-in-\[city\]-oregon.

**When a new city guide is built:** After publishing, check whether any existing blog posts or neighborhood guides should add a link to it. This cross-linking maintenance is what builds site authority over time.

**When a new neighborhood guide is built:** After publishing, update the parent city guide's neighborhood card grid to include a link to the new spoke page.

---

## CROSS-PROJECT REDIRECT RULES

If Joe asks for work that belongs in a different project, do not attempt it. Redirect him clearly.

| If Joe asks for this... | Redirect to... |
| :---- | :---- |
| A blog post (any category) | Blog Post Project |
| A Marblism compliance pass | Blog Post Project |
| A full city guide | City Guide Project |
| A neighborhood page | Neighborhood Guide Project |
| A monthly market report | Market Report Project |
| Content system architecture, version control, gap analysis | Content System HQ |
| Troubleshooting existing HTML | Content System HQ is acceptable |

**How to redirect:** State clearly which project handles this work and why. Do not start the work and then abandon it. Redirect before doing anything.

---

## REQUIRED COMPONENTS \- UNIVERSAL CHECKLIST

Every piece of content across all projects must have all of the following before publishing. Project master files have additional requirements on top of these.

- Quick Answer box near the top (answers primary question in 3-5 sentences, structured for Featured Snippet capture)  
- Data verification timestamp ("Data verified: \[Month Year\]")  
- Author bio as styled box with gold left border (not plain text)  
- EHO statement at bottom with all 7 protected classes named  
- Schema in Lofty head injection field  
- Mobile CSS with both 768px and 480px breakpoints  
- Minimum 3 internal links confirmed in SEO spreadsheet  
- All external links with target="\_blank" rel="noopener noreferrer" title="Descriptive Title"  
- No forbidden words  
- No pressure language in CTAs

---

## AGENT INFORMATION

Fixed across all content. Do not alter.

Name: Joe Saling Company: Saling Homes at eXp Realty Phone: (503) 910-7364 | tel link: tel:5039107364 Email: [joe@sellingpdxhomes.com](mailto:joe@sellingpdxhomes.com) Website: [www.sellingpdxhomes.com](http://www.sellingpdxhomes.com) About page: [https://www.sellingpdxhomes.com/about](https://www.sellingpdxhomes.com/about) Experience: 10+ years Portland metro real estate, 20+ years sales leadership and marketing

**Standard author bio content (use in all content):** Joe Saling is a Real Estate Advisor at Saling Homes at eXp Realty, serving buyers and sellers across the Portland Metro area. With 10 years in Portland real estate and 20+ years in sales, marketing, and leadership, Joe specializes in helping clients understand the market and make confident, well-informed decisions. His approach is education first \- no pressure, no surprises.

Do not mention commission. Do not list specific service area boundaries. Do not use guru, expert, ninja, or specialist as self-descriptions.

---

*Saling Homes Master Master File v1.1 | March 2026* *Store in SH Master Files folder. Load at the start of every session in every project.*  
