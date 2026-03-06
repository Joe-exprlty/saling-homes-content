# SALING HOMES — NEIGHBORHOOD GUIDE MASTER FILE

**Version 1.1 | February 2026** **sellingpdxhomes.com | Joe Saling | Saling Homes at eXp Realty**

---

## HOW TO USE THIS FILE

Upload this file at the start of every neighborhood guide conversation alongside SH-Neighborhood-Guide-Template.html. The SEO spreadsheet Sellingpdxhomes\_SEO\_Complete.xlsx is already saved in the project and will be read directly.

This file governs neighborhood guide builds only. For full city guides use SH-Community-Guide-Master-v2.9.md instead.

Every build runs in two phases. Do not skip Phase 1\. Do not begin Phase 2 until Joe types YES.

---

## WHAT A NEIGHBORHOOD GUIDE IS

A neighborhood guide is a permanent webpage, not a blog post. It lives inside the site architecture at a fixed URL, accumulates authority over time, and gets updated rather than replaced when details change.

The reader has already decided on the city. They are now narrowing down where specifically to live within that city. Every word on the page should serve that decision.

The city guide is the hub. The neighborhood guide is a spoke. It does not repeat what the city guide covers. It links to the city guide for district-level school information, healthcare access, employer data, commute tables, and cost of living context. It covers only what is specific to this neighborhood and no other.

---

## THE CONDITIONAL CONTENT RULE

This is the most important rule in this file. Read it before doing anything else.

Every lifestyle section in a neighborhood guide is conditional. Before writing any section Claude asks one question: does this specific neighborhood have something genuinely worth naming here, or does the nearest relevant option belong to the broader city?

If the answer is the city: skip the section entirely. Replace it with one natural sentence linking to the relevant section of the parent city guide. Example: "For dining and coffee near Sexton Mountain, the closest options are along Scholls Ferry Road. See the Beaverton dining guide for specifics."

If the answer is the neighborhood: include the section with real local content only.

Never write placeholder content. Never write "residents enjoy nearby dining options." Never pad a section to make the page feel more complete. A shorter honest page serves the reader better than a longer padded one. This is not a failure of the gap protocol. It is the gap protocol working correctly.

---

## PHASE 1 — RESEARCH AND APPROVAL

When Joe names a neighborhood, stop. Do not write any HTML. Do the following in order.

### Step 1: Confirm the Neighborhood Identity

Research and confirm the following before anything else.

What city does this neighborhood belong to. What is the parent city guide URL on sellingpdxhomes.com. If the city guide does not exist yet, flag this for Joe. A neighborhood guide without a parent city guide loses most of its internal linking value.

Is this a formally named neighborhood with recognized boundaries, or is it a colloquial area name that buyers use. Both can be built as neighborhood guides but the content approach differs. A formally named neighborhood like Sexton Mountain has defined character and clear boundaries. A colloquial area like West Beaverton requires more care in defining what the page is actually about.

What is the approximate geographic boundary. Name the major roads that define the edges.

What is the dominant home type and construction era. This shapes the price discussion and the image briefs.

### Step 2: Confirm Hard Data

Research and confirm the following. Cite your source next to each number.

- Typical home price range for this neighborhood specifically, not the city-wide median. Note whether this is above, below, or at the city median and by how much.  
- Dominant home type: single family, townhome, condo, mix.  
- Dominant construction era: example 1990s to 2005\.  
- Approximate number of homes or households if available.  
- Walk score or walkability description if available.

### Step 3: Confirm Schools

This is the highest-value content a neighborhood guide delivers that a city guide cannot.

Research and confirm the following.

- Which specific elementary school serves this neighborhood boundary. Name it, note its GreatSchools and Niche ratings, and include one distinguishing program or characteristic.  
- Which specific middle school serves this neighborhood boundary.  
- Which specific high school serves this neighborhood boundary.  
- Are there any boundary edge cases. Do different parts of this neighborhood feed into different schools. If yes, note exactly where the boundary splits and what it means for a buyer choosing between two streets.  
- Are there any private, charter, or magnet options within a reasonable drive that residents of this neighborhood commonly use. Note only the ones that genuinely come up in buyer conversations.

Flag any school information you cannot confirm. Joe has local knowledge that may fill gaps here.

### Step 4: Conditional Lifestyle Research

For each category below, research whether genuine neighborhood-specific content exists. Report findings honestly. If a category yields nothing specific to this neighborhood, say so directly. Joe will decide whether to fill gaps from local knowledge or skip the section.

**Walkable dining and coffee:** Are there any restaurants, coffee shops, or cafes that residents of this specific neighborhood would consider their local spot? Not options in the broader city. Options that someone living on this neighborhood's streets would walk or make a short drive to as their regular. If yes, name them, find their websites, and note what makes each one the neighborhood's own. If no, note the nearest options and which city guide section covers them.

**Parks and trails with direct neighborhood access:** Is there a park entrance, trail head, or greenspace that residents of this neighborhood access directly, meaning walkable from most streets in the neighborhood? Not a park across the city. Not a regional trail that requires driving to a trailhead. Direct neighborhood access only. If yes, name it and describe what it offers. If no, note the nearest option and drive time.

**Neighborhood gathering points:** Is there a community center, pool, HOA amenity, farmers market, or regular neighborhood event that gives this neighborhood a social identity? If yes, describe it. If no, skip this category entirely.

**Street character and physical feel:** This is always present. Every neighborhood has a physical character worth describing. Lot sizes, setbacks, sidewalk presence, tree canopy, terrain, typical garage configuration, whether streets are quiet or cut-through routes. Use Phase 1 physical research questions from the city guide master file as a guide. This content is always genuine because it is observational.

### Step 5: Compile Link Inventory

Read Sellingpdxhomes\_SEO\_Complete.xlsx from the project. Find the following types of links relevant to this neighborhood and its parent city.

- The parent city guide URL. This is a required link on every neighborhood page.  
- Listing search pages for this neighborhood or this city if neighborhood-specific searches exist.  
- Any neighboring neighborhood guide pages that already exist on the site.  
- Relevant buyer or seller guide pages from the Buyers, Resource, and Lead Magnet categories.  
- Any blog posts from the spreadsheet that are specifically relevant to this neighborhood, its schools, or its lifestyle profile.

Present the full link inventory to Joe as part of the Phase 1 summary.

### Step 6: Present Phase 1 Summary

Present all confirmed data in one clean block organized by the steps above. Be explicit about what was found and what was not found. Flag every gap. End with this exact line:

**Does this data meet the standard for a useful neighborhood guide? Type YES to begin Phase 2\.**

Do not write any HTML until Joe types YES.

When Joe types YES, deliver the SEO suite immediately before starting the build.

---

## SEO SUITE

Deliver this block in plain text immediately after Joe approves Phase 1\.

Page Slug: /neighborhoods/\[neighborhood-slug\]-\[city-slug\] or /living-in-\[neighborhood-slug\]-\[city-slug\] depending on existing URL patterns on the site. Ask Joe to confirm which pattern to use if unclear.

Meta Title: \[Neighborhood Name\], \[City Name\] Oregon: Homes, Schools and Local Life | Saling Homes Rules: 55 to 60 characters maximum. Neighborhood name first. Do not use the word guide or best.

Meta Description: 2 to 3 sentences, 145 to 155 characters maximum. Must include the neighborhood name, the parent city name, one specific local detail unique to this neighborhood such as a school name, a trail, or a price characteristic, and a soft invitation. No exclamation points. No pressure language. Count characters before delivering.

Note on meta keywords: do not generate meta keywords.

---

## PHASE 2 — THE BUILD

Build the full HTML page using the approved Phase 1 data and the SH-Neighborhood-Guide-Template.html component library. Follow every rule in this file exactly.

Do not recreate components from memory. Use the patterns in the template file.

After the HTML deliver the image briefs and content expansion plan as defined at the end of this file.

---

## CONTENT ARCHITECTURE

Build every required section. Include conditional sections only when Phase 1 research confirmed genuine neighborhood-specific content exists for that category. Do not add sections not listed here.

### A. Editorial Hook

Required. Always present.

- One H1 headline naming the neighborhood and the parent city. Frame the buyer decision. No generic phrases. No superlatives. No forbidden words: stunning, breathtaking, charming, nestled, vibrant, gem, hidden gem, wonderful, amazing, incredible.  
- Two to three paragraphs describing what this neighborhood feels like, who it suits, and what makes it different from adjacent neighborhoods. Every sentence must be specific to this neighborhood. If a sentence could describe any neighborhood in this city, rewrite it.  
- One natural reference to Joe's direct experience with this specific neighborhood. It should feel like an observation, not a credential statement.  
- City guide link: include a clear callout early in this section. Example: "For a complete picture of \[City Name\] including schools, healthcare, commute times, and cost of living, read the full \[City Name\] city guide." Link to the parent city guide. This is a required link on every neighborhood page.  
- Image slot: hero-street-\[neighborhood-slug\].webp positioned right of first paragraph.

### B. Neighborhood Snapshot Box

Required. Always present.

A compact styled data box, smaller than the city guide AEO box, covering neighborhood-specific numbers only. Do not repeat city-wide data that already lives in the city guide.

Six data cells: Typical Price Range, Dominant Home Type, Construction Era, Walk Score or Walkability Description, Elementary School, and one neighborhood-specific data point confirmed in Phase 1 such as lot size range, HOA presence, or proximity to a specific landmark.

Attribution line below heading: "Data compiled and verified by Joe Saling, Saling Homes at eXp Realty — \[Month Year\]"

### C. What You Get for Your Money Here

Required. Always present.

This is the content that a city guide cannot provide and that buyers at the neighborhood level are specifically searching for.

- Open with the typical price range for this neighborhood and how it compares to the city median. Is this neighborhood a relative value, at market, or at a premium, and why.  
- Describe what a buyer actually gets at three price points within this neighborhood range: entry level, mid range, and upper range. Lot size, square footage, garage, yard, age of home. Be specific. A buyer reading this should be able to picture what $650,000 buys on a typical street in this neighborhood.  
- Note any factors that create price variation within the neighborhood. Views, proximity to a park, school boundary edges, lot size variation, age of construction.  
- Link to the relevant listing search from the SEO spreadsheet.

### D. Schools Serving This Neighborhood

Required. Always present.

This is the highest-value section on the page for the buyer profile reading neighborhood guides.

- Do not repeat district-level stats. Those live in the city guide. Link to the schools section of the parent city guide for district context.  
- Name each school serving this neighborhood boundary. For each: school name, level, GreatSchools rating linked, Niche rating linked, one specific program or characteristic worth knowing.  
- State any boundary edge cases explicitly. If different streets feed into different elementary schools, name the dividing road and explain what it means for a buyer choosing between two homes.  
- Note any private, charter, or magnet options that residents of this neighborhood commonly use. One sentence each. Only include genuinely relevant options.  
- Close with a link to the district boundary map tool so buyers can look up a specific address.

### E. Daily Life and Walkability

Required. Always present.

This section covers what daily life actually looks like for someone living in this neighborhood. It is not a dining guide or a shopping guide. It is an honest assessment of what is accessible and how.

- Open with an honest walkability statement. Can residents walk to coffee, groceries, or a park? Or is this a drive-for-everything neighborhood? State it directly. Buyers calibrating lifestyle expectations need this answer before anything else.  
- If walkable options exist and were confirmed in Phase 1: name them, describe them specifically, and link to their websites. Apply the same standard as the city guide dining section: specific dish or drink, real vibe, actual location context.  
- If walkable options do not exist: acknowledge it honestly in one sentence and note the nearest commercial corridor and drive time. Link to the relevant section of the parent city guide.  
- Note any grocery access specifically. Grocery proximity affects daily life more than restaurant proximity for most buyers.  
- Apply the conditional content rule strictly. If this neighborhood's daily life requires a car for everything, say so and move on. Do not pad this section.

### F. Parks, Trails and Outdoor Access

Conditional. Include only if Phase 1 confirmed direct neighborhood access to a park, trail, or greenspace.

If genuine neighborhood access exists:

- Name the park or trail access point specifically.  
- Describe what it offers: distance, surface, what you see, who uses it, what time of year it is best.  
- Note the access point closest to the neighborhood, not just the park's general location.  
- Image slot: \[trail-or-park\]-\[neighborhood-slug\].webp  
- Link to the parks department page for this specific park.

If no direct neighborhood access exists:

- Skip this section entirely.  
- In the Daily Life section note the nearest park or trail and its drive time.  
- Link to the parks and trails section of the parent city guide.

### G. Neighborhood Character and Street Life

Required. Always present.

This is observational content that only someone who has spent time in this neighborhood can write well. It is also the content that AI systems recognize as genuine local expertise rather than aggregated data.

- Lot sizes and setbacks: do homes sit close together or is there breathing room between them.  
- Street character: are these quiet residential streets, cut-through routes, cul-de-sac clusters, or a mix.  
- Sidewalk presence: do residents walk to school and around the neighborhood, or are sidewalks absent.  
- Tree canopy: mature trees that create a sense of enclosure, newer development with young trees, or open and sunny.  
- Terrain: flat, rolling, elevated ridge with views, canyon edges.  
- Garage configuration: attached two-car standard, RV parking common, detached garages, no garages.  
- The feeling of the neighborhood at different times of day. Morning dog walkers, after-school activity, quiet evenings.  
- Use Phase 1 physical research to ground every detail. If physical research was not done for this neighborhood specifically, flag it and ask Joe to confirm before building.

### H. Community Life

Conditional. Include only if Phase 1 confirmed a genuine neighborhood gathering point such as an HOA amenity, community pool, neighborhood association, farmers market, or regular neighborhood event.

If genuine community infrastructure exists:

- Describe it specifically. What it is, when it happens, who it draws, what it says about the neighborhood's social character.  
- Link to the HOA, community association, or event page if one exists.

If no community infrastructure exists:

- Skip this section entirely. Do not invent community life that does not exist.

### I. How This Neighborhood Compares

Required. Always present.

A buyer narrowing down within a city is almost always comparing two or three neighborhoods simultaneously. This section serves that decision directly.

- Research which neighborhoods buyers actually compare this one against. These are not always geographic neighbors. A buyer looking at Sexton Mountain is likely also looking at South Beaverton and possibly Murray Hill. Use Phase 1 research and market knowledge to identify the genuine comparisons.  
- Build a compact comparison block: this neighborhood plus two to three alternatives. Columns: Price Range, Home Age, Walkability, Park Access, Feel. Keep it tight. This is not the full comparison table from the city guide. It is a quick reference for a buyer who is close to a decision.  
- Close with one honest paragraph on what the decision usually comes down to between these neighborhoods. Specific. No hedging.  
- Link to each neighboring neighborhood guide if the page exists on the site. If it does not exist yet, note that the city guide neighborhood section has more context.

### J. Joe's Take on This Neighborhood

Required. Always present.

Shorter than the city guide version. Two paragraphs only.

- Paragraph 1: what Joe has observed about this neighborhood that buyers do not discover until they have walked the streets. One specific local observation that only someone who has shown homes here would know. A price pattern, a school boundary nuance, a street that most buyers overlook, a view that only exists on one side of the ridge.  
- Paragraph 2: who this neighborhood is genuinely right for, and one candid sentence about who might be better served in an adjacent neighborhood. Framed around lifestyle fit only. No neighborhood comparisons by name in the candid sentence.  
- Close with Joe's signature: Joe Saling, Saling Homes at eXp Realty.

### K. Start Your Search

Required. Always present.

A focused CTA block linking directly to listing searches for this neighborhood.

- Primary link: listing search for this neighborhood or the closest available search feed.  
- Secondary links: open houses, price-reduced listings, and the parent city listing search.  
- One sentence invitation in Joe's voice. Not a pressure statement. An invitation.  
- Link to /contact for buyers who want personalized guidance.

---

## REQUIRED LINKS

### Internal Links

Every neighborhood guide must contain all of the following internal links.

Parent city guide: linked naturally in the Editorial Hook section and again in any section that defers to the city guide for broader context. This link appears at least twice on every page.

Neighboring neighborhood guides: linked in the How This Neighborhood Compares section. Include only pages that exist on the site. Find them in the SEO spreadsheet. Do not link to pages that do not exist yet.

Listing searches: linked in the What You Get for Your Money section and the Start Your Search section. Use URLs from the SEO spreadsheet. Do not invent listing search URLs.

Buyer and seller resources: linked in the site-wide link block at the bottom of the page. Use the fixed site-wide tier from the neighborhood template. These links are identical on every page.

District boundary map: linked in the Schools section. This is a required outbound link because it lets buyers verify which schools serve a specific address they are considering.

### Outbound Links

Apply the same placement rule as the city guide. Every outbound link must earn its place by answering the obvious next question a buyer would have immediately after reading the paragraph where it appears.

Required outbound links for every neighborhood guide: GreatSchools pages for each named school, Niche pages for each named school, district boundary map tool, and the website of any named local business included in the Daily Life section.

Optional outbound links when genuine content exists: parks department page for any named park, HOA or community association website, TriMet route page if transit is genuinely relevant to this neighborhood.

Never link to Zillow, Redfin, or Realtor.com anywhere in the content body.

---

## DESIGN SYSTEM

All design values are inherited from the city guide. Use the same CSS variables, typography, component patterns, and Lofty fixes defined in SH-Community-Guide-Template.html.

Do not introduce new colors, fonts, or layout patterns. Neighborhood guides must look like they belong to the same site as city guides.

The neighborhood guide uses a subset of the city guide components. Components used: progress bar, internal nav bar, hero section, section wrapper, snapshot box (compact version), editorial image with placeholder, dining item (for local spots if applicable), trail stat block (compact version if applicable), FAQ accordion (if applicable), Joe's Take opinion box, site-wide link block, footer nav bar, EHO bar, back to top links.

Components not used in neighborhood guides: full AEO box, neighborhood card grid, full dining two-column grid, retail tag cluster, full school table, commute table, employer card grid, events list, full comparison table, advisor CTA dark box.

---

## IMAGE SYSTEM

Neighborhood guides use a maximum of four image slots. Apply the same placeholder pattern and Marbalism brief standard as the city guide. Every brief must be specific enough that the image could only be this neighborhood, not any neighborhood in this city.

Required image slots:

hero-street-\[neighborhood-slug\].webp: A residential street that captures the character of this specific neighborhood. Use Phase 1 physical research to specify sidewalk presence, home construction era, tree species, terrain, and utility line configuration. This image must be identifiably different from a hero street image of an adjacent neighborhood.

school-\[neighborhood-slug\].webp: The elementary school serving this neighborhood boundary. Clean exterior, no students, natural daylight.

Conditional image slots (include only if the section exists):

trail-or-park-\[neighborhood-slug\].webp: The direct-access park or trail entrance closest to this neighborhood. Only if section F is included.

character-\[neighborhood-slug\].webp: A second street or viewpoint shot that captures something specific about the physical character of this neighborhood. A ridge view, a cul-de-sac cluster, a tree-lined street that is iconic to this area. Only if a genuinely distinctive second shot exists.

---

## VOICE RULES

Inherited from the city guide. All forbidden words apply. All Joe's voice principles apply.

Two additional rules specific to neighborhood guides.

Never compare this neighborhood to another neighborhood by name in the content body. The How This Neighborhood Compares section handles comparisons in a structured format. Comparisons in running text feel like steering and create fair housing risk.

Never describe a neighborhood's character using demographic or socioeconomic language. Character is described through physical details, lifestyle logistics, and the type of daily life the neighborhood enables. Never through who lives there.

---

## FAIR HOUSING COMPLIANCE

All city guide fair housing rules apply. The EHO bar is required at the bottom of every neighborhood guide with all 7 protected classes named: race, color, religion, sex, handicap, familial status, and national origin.

The neighborhood comparison section requires extra care. Compare on price range, home age, walkability, park access, and physical feel only. Never on demographics, school ratings as a proxy for demographics, or any language that implies a buyer should choose a neighborhood based on who lives there.

---

## SCHEMA MARKUP

Required on every neighborhood guide in the Lofty head injection field.

RealEstateAgent schema: same structure as the city guide. Update addressLocality to the parent city name. Update knowsAbout to include the neighborhood name plus "Oregon real estate", the parent city name plus "homes", the school names serving this neighborhood boundary, and any neighborhood-specific term such as a trail name or community feature that is specific to this area.

FAQPage schema: include only if the page contains an FAQ accordion. If no FAQ section is built for this neighborhood page, omit the FAQPage schema entirely. Never include schema for content that does not appear on the page.

---

## POST-BUILD DELIVERABLES

After the HTML deliver these two blocks in plain text.

### Image Brief Block

Deliver one brief per image slot used. Follow the same Marbalism brief format as the city guide. Minimum 100 words per brief. Must include all physical research details from Phase 1\. Must be specific enough that the image could only be this neighborhood.

File naming: \[photo-id\]-\[neighborhood-slug\].webp Example: hero-street-sexton-mountain.webp

### Content Expansion Plan

Deliver a minimum of 5 blog post ideas that extend this specific neighborhood guide. Organize into two tiers.

Tier 1: Publish first. Posts that answer the highest-volume buyer questions for this specific neighborhood. Typically 2 posts covering the school boundary question and the price-versus-value question in detail.

Tier 2: Publish when ready. Posts that build lifestyle authority and long-tail topical depth. Typically 3 posts covering street character, park access, or the neighborhood comparison question in more depth than the guide can cover.

For each blog post idea include: Title, Extends (which section), Captures (the search query or AI question), Links back to (the neighborhood guide section and anchor text).

---

## MOBILE DESIGN STANDARDS

Joe's site is mobile-user heavy. Every neighborhood guide must be fully optimized for mobile screens before it is optimized for anything else. Desktop is secondary. Mobile is primary.

### Breakpoints

Use two breakpoints on every neighborhood guide.

768px: Tablet adjustments. Grids collapse. Floated editorial images go full width. Snapshot grid drops to single column.

480px: Phone-specific adjustments. This is the most important breakpoint. Most of Joe's mobile traffic is on screens between 375px and 430px. Design for that range first.

### Mobile Font Sizes

Required at the 480px breakpoint. Never let body text drop below 1rem on mobile.

H1: 1.9rem H2: 1.45rem H3: 1.2rem Body text: 1.05rem, line-height 1.85 Captions: 0.82rem Buttons and nav links: 1rem, weight 600 FAQ summary text: 0.95rem

### Mobile Layout Rules

Editorial images: width 100%, float none, margin 0 0 20px 0 at 480px. Never float images on mobile.

Snapshot grid (AEO box): single column at 480px.

All multi-column grids: collapse to single column at 480px. No exceptions.

Tables: wrapped in overflow-x auto scroll container at all screen sizes.

Callout boxes: padding reduces to 16px 18px at 480px.

CTA buttons: stack vertically at 480px. Each button goes width 100%, display block, margin-bottom 12px.

Navigation bar: horizontally scrollable at 480px with overflow-x auto and \-webkit-overflow-scrolling touch. Never wrap nav items to a second line on mobile.

Hero section: padding reduces to 40px 20px at 480px.

### Touch Target Sizing

Every tappable element must be minimum 44px tall.

FAQ accordion summaries: min-height 48px, padding 14px 16px, full width tap target.

Buttons and CTA links: min-height 48px.

Nav links: min-height 44px.

### Mobile Color and Contrast

Gold (\#D4AF37) on white fails WCAG AA contrast. Never use gold as body text color on any background. Gold is for borders, accents, and icons only.

Body text: \#444444 on white. Text on dark backgrounds: \#FFFFFF. Both pass WCAG AA at all sizes including mobile.

### Required Mobile CSS Pattern

Every neighborhood guide includes this block inside the scoped CSS. Adapt class names to match the page being built.

```css
@media (max-width: 768px) {
  .sh-hero { padding: 48px 24px; }
  .sh-hero h1 { font-size: 2.1rem; }
  .aeo-grid { grid-template-columns: 1fr; gap: 20px; }
  .editorial-img,
  .editorial-img.left {
    width: 100%;
    float: none;
    margin: 0 0 20px 0;
  }
  .char-grid { grid-template-columns: 1fr; }
  .cta-buttons { flex-direction: column; }
  .cta-buttons a { width: 100%; text-align: center; }
}

@media (max-width: 480px) {
  .sh-hero h1 { font-size: 1.9rem; }
  .sh-section h2 { font-size: 1.45rem; }
  .sh-guide { font-size: 1.05rem; line-height: 1.85; }
  .aeo-box { padding: 24px 20px; }
  .callout-box,
  .joes-take,
  .cta-dark { padding: 24px 20px; }
  .faq-acc summary { min-height: 48px; padding: 14px 16px; }
  .btn-primary,
  .btn-secondary {
    display: block;
    width: 100%;
    text-align: center;
    margin-bottom: 12px;
    min-height: 48px;
  }
  .data-table-wrap { overflow-x: auto; -webkit-overflow-scrolling: touch; }
  .sh-nav {
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
    scrollbar-width: none;
  }
  .sh-nav::-webkit-scrollbar { display: none; }
  .sh-footer-nav a { font-size: 0.78rem; padding: 4px 8px; }
}
```

---

## PRE-PUBLISH CHECKLIST

Content: Editorial Hook present with parent city guide link, Snapshot Box present with attribution line, What You Get for Your Money present with listing search link, Schools section present with boundary edge cases noted, Daily Life section present with honest walkability statement, Neighborhood Character section present with physical research grounding, How This Neighborhood Compares present with 2 to 3 alternatives, Joe's Take present with 2 paragraphs and city-specific observation, Start Your Search CTA present.

Conditional sections: each conditional section either has genuine content or is replaced by a single honest link to the parent city guide. No padded or placeholder content anywhere on the page.

Technical: Google Fonts link in head, all 9 CSS variables defined, progress bar present, Lofty margin fix on all dark sections, all viewBox attributes lowercase, schema markup in head injection with correct neighborhood-specific knowsAbout field, FAQPage schema present only if FAQ accordion is on the page.

Mobile: Both breakpoints present (768px and 480px). Body text minimum 1.05rem at 480px. All floated editorial images removed at 480px. All grids collapse to single column at 480px. CTA buttons stack vertically at 480px. All tables in scroll containers. FAQ accordion tap targets minimum 48px. Nav bar scrolls horizontally at 480px. No gold text on white backgrounds.

Images: hero-street image slot present, school image slot present, conditional image slots present only for sections that exist, all img tags have descriptive alt text in format Subject, Neighborhood Name, City, Oregon, all img tags have loading="lazy" except above-fold hero, fixed 320px width on all editorial images.

Links: parent city guide linked using /living-in-\[city\]-oregon format at least twice, neighboring neighborhood guides linked in comparison section only for pages that exist, listing search links verified in SEO spreadsheet, GreatSchools and Niche links present for all named schools, district boundary map linked in schools section, no links to Zillow or Redfin or Realtor.com.

Fair Housing: no demographic language anywhere in content, comparison section uses only price, age, walkability, park access, and physical feel, EHO bar present with all 7 protected classes named.

Post-build deliverables: image briefs delivered for all image slots used, Content Expansion Plan delivered with minimum 5 blog ideas in two tiers.

---

## AGENT INFORMATION

Fixed across all pages. Do not alter.

Name: Joe Saling Company: Saling Homes at eXp Realty Phone: (503) 910-7364 Email: [joe@sellingpdxhomes.com](mailto:joe@sellingpdxhomes.com) Website: [www.sellingpdxhomes.com](http://www.sellingpdxhomes.com) Experience: 10+ years Portland metro real estate, 20+ years sales leadership and marketing

---

*Saling Homes Neighborhood Guide Master File v1.1 | February 2026* *Upload alongside SH-Neighborhood-Guide-Template.html at the start of every neighborhood guide conversation. Sellingpdxhomes\_SEO\_Complete.xlsx is already saved in the project and will be read directly.*  
