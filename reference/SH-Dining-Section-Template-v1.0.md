**SALING HOMES**

City Guide — Dining Section Template and Standards

*Version 1.0  |  March 2026  |  Applies to: SH-Community-Guide-Master v3.3 \+ Template v1.3*

# **Purpose of This Document**

This document defines exactly how the dining section of every Saling Homes city guide should be structured, what it should contain, and how it should be built in HTML. Use it alongside SH-Community-Guide-Master as the definitive reference for dining section builds. When anything in this document conflicts with an older version of the master file, this document wins for the dining section specifically.

# **Section Overview**

| Section ID | dining |
| :---- | :---- |
| **Section Label** | Dining & Coffee |
| **H2 Pattern** | Where \[City Name\] Eats and Gathers |
| **Entry Target** | 14 (cities with sufficient depth) | 8 minimum (smaller cities) |
| **Layout** | 3-column grid. 1 visible row (3 entries). Remaining entries in collapse. |
| **Position in Guide** | Section E — after Mid-Page CTA, before Shopping |

# **Category Breakdown**

Every city guide dining section must include entries from all five categories. The counts below are for a 14-entry build. Scale proportionally for smaller cities.

| Category | Count | Rules |
| :---- | :---- | :---- |
| **Restaurants** | 6 | No two entries the same cuisine. Covers the key buyer question: what can I eat within 10 minutes of home? Local or strong regional brand only. |
| **Bars / Gastropubs** | 3 | Taphouse, brewpub, and gastropub count as separate sub-types. At least one should have outdoor seating. No sports bars with no food program. |
| **Coffee / Cafe** | 2 | At least one must serve food (not coffee-only). No drive-through-only stands. Should represent the work-from-home buyer's morning routine. |
| **Wildcard / Experiential** | 1 | Something that makes the city memorable: game bar, distillery tasting room, dessert destination, food cart pod, unique concept. One entry only. |
| **Locked** | 2 | Joe confirms these before research begins. They count toward the category they belong to. They do not automatically go in the visible row. |

# **The Visible Row — Above the Fold**

The visible row is the most important editorial decision in the dining section. These are the 3 entries a buyer sees before any interaction. They determine whether the buyer believes this city has a real food culture.

**Selection Rules**

* Must be the 3 highest-signal entries from the full 14, judged by cross-platform presence (Yelp \+ TripAdvisor \+ Google Maps combined)

* At least one must be distinctly associated with this city specifically, not just this metro market

* At least one should carry name recognition that stops a relocating buyer mid-scroll

* The row collectively should signal: this city has food worth driving to, not just convenient options

* Locked entries do not automatically qualify for the visible row — signal strength is the deciding factor

**What to Avoid**

* All three entries from the same category (three bars, three coffee shops, etc.)

* Dessert or snack destinations in the visible row — they don't set the right tone

* Entries that only appear on one platform or have fewer than 50 reviews

# **Entry Format**

Every entry — visible or collapsed — follows the same format. No exceptions.

**Required Fields**

* Name (H4)

* Description: 2 to 4 sentences. Must include one specific dish, drink, or feature that only someone who has been there would know. No generic language. No sentences that could appear on the restaurant's own website.

* Link: official website preferred. Yelp or Google Maps acceptable if no website exists.

**Description Writing Rules**

* Name a specific dish, signature drink, or defining feature in every entry

* Include the physical context: location on a specific street, inside a mall, on a waterfront, etc.

* One sentence on who this place is right for or what kind of visit it suits

* Never use: 'cozy', 'vibrant', 'amazing', 'incredible', 'mouthwatering', or any word found in the restaurant's own marketing copy

* Never open with the restaurant name as the subject of the first sentence

**Example Entry (Correct)**

**Din Tai Fung**

Oregon's first location of the globally acclaimed Taiwanese dumpling house, inside Washington Square. Each Kurobuta pork xiao long bao is hand-folded with exactly 18 pleats and served in bamboo steamers. Watch the process through the open-view kitchen window. Reservations recommended; Golden Hour happy hour runs Monday through Thursday 3 to 6 pm.

**Example Entry (Wrong)**

**Din Tai Fung**

A cozy Taiwanese restaurant in Washington Square Mall with amazing soup dumplings and incredible service. Perfect for families and date nights alike. The vibrant atmosphere makes this a must-visit destination.

*Wrong because: 'cozy', 'amazing', 'incredible', 'vibrant', 'must-visit' are all generic. No specific dish detail. No physical context. No useful information for a relocating buyer.*

# **Establishment Selection Criteria**

Every entry must pass all three gates before inclusion. No exceptions.

| Gate | Requirement | How to Verify |
| :---- | :---- | :---- |
| **1** | **Independently owned or strong regional brand** | Check website About page. No national chains. Regional chains with strong local identity (Thirsty Lion, McMenamins) are acceptable. |
| **2** | **Verifiably open as of research date** | Check Yelp or Google Maps listing for current hours. If hours are missing or the listing shows 'permanently closed,' do not include. |
| **3** | **Appears on at least one major platform top list** | Yelp top 10 (updated within 12 months), TripAdvisor city rankings, Google Maps top-rated results, or named in local media. Cross-platform signal preferred over single-platform. |

# **HTML Structure**

The dining section HTML follows this exact pattern. Copy from the template. Do not rebuild from memory.

**Intro Paragraph**

2 to 3 sentences. What does the dining scene say about the character of this city? Reference one specific local detail (street name, food pod, signature venue). Update the entry count to match the actual number used.

**Visible Grid**

\<div class="dining-visible-grid"

  style="display:grid;grid-template-columns:repeat(3,1fr);gap:24px;margin-bottom:20px;"\>

  \[3 dining-item entries\]

\</div\>

**Collapse Toggle**

\<details\>

  \<summary ...\>See all \[City Name\] dining

    \<svg ...chevron /\>\</summary\>

  \<div style="margin-top:16px;"\>

    \<div class="dining-collapse-grid"

      style="display:grid;grid-template-columns:repeat(3,1fr);gap:24px;"\>

      \[remaining dining-item entries\]

    \</div\>

  \</div\>

\</details\>

**Individual Entry**

\<div class="dining-item"\>

  \<h4\>\[Name\]\</h4\>

  \<p\>\[2-4 sentence description with specific dish/detail\]\</p\>

  \<a href="\[URL\]" target="\_blank" rel="noopener"\>Visit website \&rarr;\</a\>

\</div\>

**Mobile Breakpoint**

Both grids collapse to single column at 720px. This is handled in the template CSS:

@media (max-width: 720px) {

  .dining-visible-grid { grid-template-columns: 1fr \!important; }

  .dining-collapse-grid { grid-template-columns: 1fr \!important; }

}

# **Phase 1 Research Checklist — Dining**

Complete this during Phase 1 before writing any HTML. Present findings in the Phase 1 summary block.

* Confirm 2 locked entries with Joe before research begins

* Search Yelp top 10 restaurants (filter: updated within 12 months)

* Search TripAdvisor top restaurants for the city

* Search Google Maps top-rated results

* Cross-reference all three lists and identify entries appearing on 2 or more

* Identify top coffee/cafe options from Yelp coffee category search

* Confirm each entry is independently owned or qualifies as regional brand

* Confirm each entry shows current hours and open status

* For each entry: find one specific dish, drink, or feature to name in the description

* Flag any entry where you cannot find a specific signature item — ask Joe to fill in

* Compile website URLs for all entries. Use Yelp link only if no official website found.

* Select 3 entries for the visible row based on signal strength criteria above

# **Pre-Delivery Checklist — Dining Section**

* 14 entries present (or 8 minimum for smaller city)

* All 5 categories represented

* No two restaurant entries share the same cuisine

* 3 entries in visible grid, remainder in collapse

* Visible row: 3 highest-signal entries, at least one city-specific

* Collapse toggle label: 'See all \[City Name\] dining'

* Every entry has a specific dish, drink, or feature named

* No generic descriptors: cozy, vibrant, amazing, incredible, mouthwatering

* All links verified working

* No chains in the list

* All entries confirmed open as of research date

* Intro paragraph references actual entry count

* Mobile breakpoint CSS present for both grids

*Saling Homes City Guide — Dining Section Standards  |  Version 1.0  |  March 2026*

*joe@sellingpdxhomes.com  |  www.sellingpdxhomes.com*