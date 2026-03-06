# SALING HOMES — MARKET REPORT MASTER FILE

**Version 1.1 | February 2026** **sellingpdxhomes.com | Joe Saling | Saling Homes at eXp Realty**

---

## HOW TO USE THIS FILE

Upload this file at the start of every market report conversation alongside the 26 RMLS PDF files and Sellingpdxhomes\_SEO\_Complete.xlsx. This file is the single source of truth for every market report build. Do not ask Joe to re-explain the data structure, workflow, voice rules, or schema requirements.

Every build runs in two phases. Do not skip Phase 1\. Do not begin Phase 2 until Joe types YES.

At the start of every conversation ask: "Which month and year are we writing the market report for?"

---

## THE DATA ARCHITECTURE

### Self-Expanding Document Rule

Read every document in this project before beginning Phase 1\. Do not limit yourself to named or expected file types. For each document you find, identify what data it contains, what time period it covers, and how it relates to the market report being built. Apply all relevant data to the analysis automatically.

This rule exists so that when Joe adds a new file to the project, whether it is a new monthly RMLS report, an updated SentriLock dataset, a Fed statement, an economic report, or any other relevant document, Claude reads it and applies it without requiring any changes to this master file. The project is self-expanding by design. New documents are always incorporated.

When you encounter a document that does not match any named data type in this architecture section, use your judgment to determine what it contains and how it adds context to the reporting period being analyzed. Flag it in the Phase 1 summary so Joe knows it was read and applied.

### Known Data Sources Currently in This Project

The following data sources are currently part of this project. Additional sources may be added at any time and will be read automatically under the self-expanding document rule above.

**RMLS Monthly Market Action Reports** Each PDF covers one reporting period and follows an identical 13-page structure containing three data layers.

Layer 1: Portland Metro Residential Highlights (Page 2). The primary metro-level summary. Extract these fields from every relevant month: New Listings with percent change from prior month and same month prior year. Pending Sales with percent change from prior month and same month prior year. Closed Sales with percent change from prior month and same month prior year. Average Sale Price with year-over-year rolling 12-month comparison. Median Sale Price with year-over-year rolling 12-month comparison. Inventory in Months with current month figure, same month prior year, and same month two years prior. Total Market Time with change from prior month and same month prior year. Year-to-Date figures for all of the above where provided.

Layer 2: Sub-Market Area Data (Page 10). The 15 Portland Metro sub-market zones. Extract for each zone: New Listings current month vs same month prior year, Pending Sales current month vs same month prior year and year-to-date comparison, Closed Sales current month and year-to-date, Average Sale Price current month and year-to-date, Median Sale Price year-to-date, Total Market Time. The 15 standard zones are: N Portland, NE Portland, SE Portland, Gresham/Troutdale, Milwaukie/Clackamas, Oregon City/Canby, Lake Oswego/West Linn, W Portland, NW Washington County, Beaverton/Aloha, Tigard/Wilsonville, Hillsboro/Forest Grove, Mt. Hood, SW Washington, and Columbia County.

Layer 3: Affordability Index (Page 9). Updated quarterly. Contains: median household income (HUD source, year noted), Freddie Mac 30-year fixed rate for the period, affordability percentage, purchase-ready active listings count and inventory in months.

File naming convention: YY\_MM\_PortlandMetroArea.pdf. Example: 25\_12\_PortlandMetro\_Area.pdf equals December 2025\. Use filenames to map each report to its reporting period.

The Inventory in Months table on page 2 of every RMLS report shows a three-year monthly comparison. Always extract this full table. It reveals seasonal patterns and year-over-year trends in a single view that cannot be replicated from any single month's data.

**SentriLock Lockbox Daily Activity Data** This document contains daily lockbox opening counts for the Portland Metro from 2013 through the most recent available period. Every lockbox opening represents a buyer's agent showing a home to a buyer. This is the most direct measure of buyer foot traffic available in the market and it is data that national competitors cannot access or replicate.

The SentriLock data serves four specific purposes in every market report.

First, showing volume as a leading indicator. Showings lead closed sales by 30 to 60 days. When showing activity rises in a given month, expect stronger closed sales 30 to 60 days later. When showing activity falls, expect softer closings ahead. Always compare the current reporting month's showing total to the same month in prior years and note the direction and magnitude of the difference.

Second, the buyer paradox signal. When showing activity is high but pending and closed sales are soft, buyers are actively looking but not committing. This is a powerful diagnostic that explains market behavior. The January 2026 post referenced this dynamic. SentriLock data is what proves it with numbers rather than just asserts it.

Third, seasonal pattern validation. The SentriLock dataset going back to 2013 shows the normal seasonal shape of Portland Metro buyer activity. Spring peaks, summer plateaus, fall declines, holiday troughs. When current showing activity deviates meaningfully from the historical seasonal pattern for that month, it is a signal worth calling out. Example: if January 2026 showings are 20% below the January average from 2015 through 2019, that deviation from the pre-pandemic norm is meaningful context.

Fourth, historical range context. With data from 2013 onward the dataset spans multiple market cycles including the post-recession recovery, the pre-pandemic boom, the COVID disruption and rebound, and the rate-driven slowdown. Use this range to place current showing levels in genuine historical perspective. A statement like "January 2026 showings were the lowest January total since 2023 but still above the 2013 through 2016 baseline range" is only possible with this dataset.

Extract the following from the SentriLock data for every report: monthly total for the reporting period, same month prior year total and percent change, same month two years prior total, the monthly average for the same month across all available years excluding COVID-affected 2020, and the highest and lowest January (or relevant month) totals in the dataset with their years.

Note that the SentriLock file currently runs through December 2025\. When Joe adds updated SentriLock data for 2026 months, read the new file automatically under the self-expanding document rule. Do not wait for instruction to use it.

**SEO Spreadsheet** Contains verified internal URLs for sellingpdxhomes.com organized by category, city, and page type. Read this to find confirmed internal links for every report. Never invent a URL that does not appear in this spreadsheet.

---

## THE CONTEXT FRAMEWORK

Context is the entire point of this project. RMLS data tells what happened. Context explains why it happened, what it means historically, and what the trajectory suggests for the near future. Every market report post uses three layers of context.

### Layer 1: Internal Historical Context (From the RMLS Files)

For every market report compare the current month against four reference points:

**Same month, prior year:** The most meaningful single comparison. Filters out seasonal noise. If December 2025 closed sales are up 6.5% from December 2024, that is a genuine year-over-year gain, not a seasonal effect.

**Prior month, current year:** Shows the current seasonal trend direction. December always slows from November. The question is whether the slowdown is larger or smaller than expected.

**Same month, two years prior:** Establishes whether the current market is recovering toward, at, or above pre-period norms. If December 2023 inventory was 2.7 months and December 2025 is 2.9 months, inventory has risen modestly over two years but remains historically low.

**Year-to-date vs prior year-to-date:** The most reliable indicator of annual market direction. Single months can be distorted by weather, holidays, or data timing. Year-to-date smooths those distortions.

Extract these four reference points for every primary metric before writing any content. Do not start Phase 2 without them.

### Layer 2: Trend Narrative (Derived From Multiple Months)

For every report identify the trend direction across the most recent three to six months of RMLS data. Read the relevant monthly files to answer these questions before writing:

Is inventory rising, falling, or holding? At what pace? Is the pace accelerating or decelerating?

Are pending sales (the leading indicator of buyer demand) rising or falling relative to the same period last year? Pending sales lead closed sales by 30 to 60 days. A trend in pending sales predicts what closed sales will show in the next one to two months.

Is the gap between average and median sale price widening or narrowing? A widening gap (average rising faster than median) indicates upper-end activity driving the market. A narrowing gap suggests more balanced activity across price ranges.

Is total market time trending longer or shorter over the past three to six months? Longer market time is a leading indicator of price pressure building on sellers.

State each trend direction clearly in Phase 1 and cite which months the trend spans.

### Layer 3: External Context (Web Search Required)

After extracting RMLS data and identifying internal trends, use web search to find the following external context for the reporting period. This is what transforms a data summary into a post that explains the why behind the numbers.

**Mortgage rate environment:** Search for the Freddie Mac Primary Mortgage Market Survey for the reporting month. Note the 30-year fixed rate, direction of change from prior month, and direction of change from same month prior year. A rate that moved from 7.2% to 6.2% year-over-year is a meaningful affordability shift that directly explains buyer activity changes.

**Federal Reserve policy:** Search for any Fed rate decisions or guidance statements during or immediately before the reporting period. Buyers respond to Fed signals even before rate changes take effect.

**Regional employment:** Search for recent Intel, Nike, or Oregon employment news within the past three months. These two employers are the largest drivers of west-side Portland Metro buyer demand. A hiring announcement, layoff, or return-to-office mandate at either company directly affects demand in Hillsboro, Beaverton, and Tigard.

**Oregon housing legislation or policy:** Search for any Oregon state housing bills, rent control changes, property tax adjustments, or buyer assistance programs that became effective or were announced in the reporting period or the prior quarter.

**Portland Metro economic context:** Search for any significant Portland Metro economic news including downtown recovery indicators, major employer announcements, population migration data, or regional development news that affects housing demand.

**National market context:** Search for the most recent NAR Existing Home Sales report and the S\&P CoreLogic Case-Shiller Home Price Index for context on how Portland Metro compares to national trends. Note whether Portland is outperforming, underperforming, or tracking the national market.

**Consumer platform directional check:** Search Zillow and Redfin for their current Portland Metro market assessments. Do not use their specific price figures as primary data points since their methodologies differ from RMLS and can produce figures that diverge significantly from actual closed sales. Use them for one specific purpose only: directional validation. If Zillow's market temperature, Redfin's demand index, and RMLS closed sale trends are all pointing in the same direction, that convergence is a credibility signal worth calling out explicitly in the post. When all three independent sources reach the same conclusion about market direction, say so. It shows Joe is not working from a single source and validates the analysis for readers who are already using those platforms to track the market themselves.

For every external data point: cite the source name, the specific figure, and the date of the source. Do not use external data without a named source. Do not estimate external figures.

---

## PHASE 1 — RESEARCH AND APPROVAL

When Joe provides the reporting month and year, execute the following steps in order. Present all findings in one clean structured block. Do not write any HTML during Phase 1\.

### Step 1: Read All Documents in the Project

Read every document in this project before extracting any data or writing anything. This includes all RMLS PDF files, the SentriLock lockbox activity file, the SEO spreadsheet, and any other files present. Do not skip any file. Do not limit yourself to expected file types or named sources.

For each document identify: what data it contains, what time period it covers, and how it is relevant to the reporting period being analyzed. Apply all relevant data automatically. Flag any document that does not fit a known category in the Phase 1 summary so Joe knows it was read and how it was applied.

This step is not negotiable. Reading everything before writing anything is what makes the historical context layer possible.

### Step 2: Extract Current Month RMLS Data

From the RMLS file for the reporting month extract all Layer 1, Layer 2, and Layer 3 data fields as defined in the Data Architecture section. Present every figure exactly as it appears in the report. Do not round or estimate. Use the exact figures from the document.

Also extract the full Inventory in Months table showing all three years for all months available.

### Step 3: Extract SentriLock Showing Data

From the SentriLock document extract the following for the reporting month:

Monthly total for the reporting period and same month in all available prior years. Calculate year-over-year change from same month prior year and same month two years prior. Calculate the historical monthly average for that month across all available years excluding 2020 which was COVID-distorted. Identify the highest and lowest totals ever recorded for that month in the dataset and note the year each occurred.

Note whether current showing activity is above, below, or tracking the historical seasonal average and by what margin. Note whether the relationship between showing activity and closed sales is normal (showings up, closings follow) or paradoxical (showings up but closings flat or declining, which signals buyer hesitation).

If an updated SentriLock file covering more recent months has been added to the project, use the most current data available.

### Step 4: Build the Four-Point Historical Comparison

For each primary RMLS metric (new listings, pending sales, closed sales, average price, median price, inventory, market time) present: current month figure, same month prior year figure and percent change, prior month current year figure and percent change, same month two years prior figure and percent change, year-to-date current year vs year-to-date prior year and percent change.

### Step 5: Identify the Three to Six Month Trend

Using the RMLS files and SentriLock data for the most recent three to four months answer the four trend questions from the Context Framework Layer 2 section. Also note whether showing activity has been trending in the same direction as pending sales or diverging. A divergence between showings and pendings is one of the most useful diagnostic signals in the dataset.

### Step 6: Sub-Market Highlights

From the current month RMLS file extract sub-market data for all 15 zones. Identify the three showing strongest year-over-year performance and three showing weakest. Note any sub-market trending significantly differently from the metro average.

### Step 7: Affordability Snapshot

Extract affordability data and calculate the monthly payment on the current median-priced home at the current Freddie Mac rate with 20% down. Note improvement or deterioration from the same period prior year.

### Step 8: Web Search for External Context

Execute web searches for all seven external context categories defined in the Context Framework Layer 3 section including the Zillow and Redfin directional check. Present each finding with source and date.

### Step 9: Identify the Story

State the central narrative of this month's report in one sentence. Ground it in the actual data including the SentriLock showing context where it is relevant. This becomes the H1 headline anchor.

### Phase 1 Close

Present all findings in this order: story sentence, current month RMLS data, SentriLock showing data and what it signals, four-point historical comparison, trend narrative, sub-market highlights, affordability snapshot, external context. Then end with:

"Does this data and context accurately reflect the market for \[Month Year\]? Once you confirm, type YES and I will deliver the updated SEO suite followed by the full HTML post."

---

## PHASE 2 — THE BUILD

When Joe types YES:

First deliver the SEO suite as defined below.

Then build the full HTML post following the content architecture defined in this file.

Then deliver image briefs and follow-up content ideas.

---

## SEO SUITE

Deliver as plain text before building any HTML.

**Slug:** /blog/\[month\]-\[year\]-portland-metro-real-estate-market-update Example: /blog/december-2025-portland-metro-real-estate-market-update Always include the month and year in market report slugs. These posts are indexed by period.

**Meta Title:** 55 to 60 characters maximum. Lead with the month and year. Include the primary insight from the story sentence where it fits. Example: "December 2025 Portland Metro Market Update: Prices Hold Steady"

**Meta Description:** 145 to 155 characters. State the month, the primary metric movement, and what it means for Portland Metro buyers or sellers. Soft invitation to read. No exclamation points. Count characters before delivering.

**Primary Keyword:** \[Month\] \[Year\] Portland Metro real estate market update. Always.

**Secondary Keywords:** Portland home prices \[year\], Portland housing inventory, Portland Metro market trends, Portland Metro closed sales, is now a good time to buy in Portland.

**Internal Links:** Read Sellingpdxhomes\_SEO\_Complete.xlsx to find minimum three relevant internal links. Required links for every market report: the current market snapshot page, the buyer resources page, and the seller evaluation page. Add any city-specific guide links that are relevant based on notable sub-market performance in this month's report.

**Update Cadence:** Time-sensitive. Published within the first two weeks of the month following the reporting period. Not updated after publication. New period means new post.

---

## CONTENT ARCHITECTURE

Build in this exact order. Do not reorder. Do not skip any required section.

### Hero Section

Full-width dark hero panel using the near-black gradient background. Contains:

- Gold badge label: "RMLS Market Action Report — \[Month\] \[Year\]"  
- H1 headline: "\[Month\] \[Year\] Portland Metro Real Estate Market Update: \[Story sentence condensed to headline format\]"  
- One-sentence subhead stating the primary data point  
- Reading progress bar

### Opening Paragraph

Three sentences at 1.1rem font-weight 500\. This is the post's most important paragraph for AI citation capture. It must state: what month this covers, the single most significant data finding, and what that finding means for Portland Metro buyers or sellers right now. Write it to function as a complete standalone answer that could be extracted by Google or any AI system.

### Quick Answer Box

Gold-bordered callout. Label: "The Short Version." Four to five sentences answering: what happened to prices, what happened to inventory, what the market means for buyers right now, what the market means for sellers right now. This box is structured specifically for Google Featured Snippet capture. Every sentence must be factually grounded in the RMLS data. No hedging. No filler.

### Key Market Indicators Box

Dark background, gold accent border. Two-by-two grid of four stat cells. Each cell contains: metric name, current month figure, directional arrow (gold up or red down), and percent change from same month prior year. Required cells: Median Sale Price, Inventory in Months, Closed Sales, Total Market Time.

Below the four cells: a fifth full-width cell showing the Freddie Mac 30-year rate for the reporting period and the year-over-year rate change.

### Table of Contents

Gold-accented, linked to section anchors. Label: "Key Takeaways and Quick Navigation."

### Market Overview Section

H2: "What Happened in \[Month\] \[Year\]"

Four to five paragraphs. This is the analytical core of the post. Build it around the story sentence identified in Phase 1\. Cover:

Paragraph 1: The headline finding. What is the single most significant development this month and what does the data show. State it directly without hedging.

Paragraph 2: The inventory story. What did inventory do, at what pace, and how does the current inventory level compare to the three reference points (same month prior year, same month two years prior, and the long-term norm for this market). What does the current inventory level mean mechanically for buyers and sellers.

Paragraph 3: The demand story. What did pending sales show. Since pending sales lead closed sales by 30 to 60 days, what does the current pending sales figure predict for next month's closed sales. Is buyer demand strengthening, softening, or holding.

Paragraph 4: The price story. Are prices compressing or expanding. Is the gap between average and median widening or narrowing and what does that indicate about which price segments are most active. Compare to the same month prior year and note whether the trajectory is improving or deteriorating for buyers.

Paragraph 5: The context bridge. Connect one or two of the external context findings from Phase 1 to the data patterns observed. Example: if inventory rose month-over-month while pending sales held, and the Freddie Mac rate dropped 0.3 points during the period, connect those three facts into a coherent explanation of what buyers were doing and why.

**Source Convergence callout (include only when Zillow and Redfin directional findings align with RMLS):** A gold-bordered callout box labeled "Multiple Sources, Same Story." Two to three sentences stating that RMLS closed sales data, Zillow's market assessment, and Redfin's demand indicators are all pointing in the same direction this month. Name the specific direction each source indicates. This box signals to the reader that the analysis is not drawn from a single source and validates Joe's conclusions for the large portion of readers who are already tracking the market on those consumer platforms. Do not include this box if the sources are contradicting each other. Honest disagreement between sources is noted in the body text instead, with an explanation of why RMLS figures are used as the primary reference.

### Trend Callout Box

Dark background. Gold accent. Label: "The \[3/6\]-Month Trend." Three to four bullet points stating the trend direction for inventory, pending sales, prices, and market time over the identified trend period. Each bullet is one sentence. No hedging. State the direction and the magnitude. Example: "Inventory has risen in seven of the last eight months, adding 1.2 months of supply since April 2025."

### Buyer Activity Section

H2: "What Buyers Are Actually Doing: The Showing Data"

This section uses the SentriLock data to tell the story behind the RMLS transaction numbers. It is one of the most differentiated sections in the post because no national competitor has access to this data or presents it this way.

Open with the monthly showing total for the reporting period and the year-over-year comparison. State the direction and magnitude plainly. Then place that number in historical context using the full SentriLock dataset. Compare to the historical monthly average for that month excluding 2020\. Note whether showing activity is above or below the pre-pandemic baseline range.

Then address the relationship between showings and transactions. If showings are up but closings are flat or down, name the buyer paradox explicitly. Buyers are looking but not committing. Explain what that typically signals in the Portland market based on historical patterns in the dataset. If showings and closings are moving in the same direction, note that alignment and what it predicts for the coming months given the 30 to 60 day lag.

Include a small inline table or callout showing: current month showings, same month prior year showings, year-over-year change, and the historical monthly average for that month. Keep it compact. Two to three rows maximum.

Close the section with one forward-looking sentence. Based on current showing activity and the historical lag between showings and closings, what does the data suggest buyers will do over the next 30 to 60 days.

### Affordability in Context Section

H2: "What Affordability Looks Like Right Now"

Gold-bordered box containing the affordability calculation: median home price, Freddie Mac rate, 20% down payment assumption, resulting monthly payment (principal and interest only, note that taxes and insurance are additional), median household income, and the percentage of gross monthly income that payment represents.

Below the box: two to three paragraphs of honest affordability analysis. Is Portland getting more or less affordable and at what pace. Compare to same period prior year. Note what a one-point rate change in either direction would do to the monthly payment and affordability percentage. This section is the most useful content for buyers who are calculating whether they can afford to move from renting to owning.

Do not cheerfully conclude that affordability is good or bad. Present the math, explain what it means, and let the reader draw their own conclusion about their specific situation.

### What This Means for Buyers Section

H2: "For Buyers: What This Market Means Right Now"

Open with a direct sentence on whether current conditions favor buyers, sellers, or neither, and why.

Green-bordered callout box labeled "When This Market Works in Your Favor." Three to four specific conditions that make this a favorable moment for a specific buyer profile. Each condition is grounded in the data. Example: "If you have been waiting for more options, inventory at \[X\] months means you have roughly \[X\]% more active listings to choose from than at this point last year."

Orange-bordered callout box labeled "When You Should Wait." One to two honest statements about buyer profiles for whom this is not the right moment. This box is the most trust-building element in the post. Example: "If you need to sell your current home first and your home is in a slower sub-market, the math on a contingent offer is harder this month than it was six months ago."

Two to three paragraphs of buyer strategy context. What should a buyer who is actively looking do differently given these conditions. Reference the sub-market data where relevant.

### What This Means for Sellers Section

H2: "For Sellers: What This Market Means Right Now"

Open with the inventory math. State how many active listings are on the market, how many homes closed last month, and what percentage of the active inventory transacted. This gives sellers a concrete sense of competition.

Dark-bordered callout box labeled "Seller Strategy for \[Month\] \[Year\]." Three to four specific strategic considerations given current conditions. Each is grounded in the data. Example: "With total market time at 81 days versus 74 days a year ago, pricing to the market rather than aspirationally matters more than it did last year."

Two to three paragraphs of seller context. What price segment is moving fastest. What sub-markets are showing the most buyer activity. What does the pending-to-closed ratio suggest about buyer follow-through.

### Sub-Market Spotlight Section

H2: "How Different Parts of Portland Metro Are Performing"

A table showing the 15 sub-market zones with columns for: sub-market name, current month median sale price (or YTD median where available), year-over-year price change, current month closed sales, and year-over-year closed sales change. Wrap the table in a scroll container for mobile.

Below the table: three to four paragraphs. Identify the two to three sub-markets showing notable outperformance and explain what is driving that activity. Identify any sub-market showing notable underperformance and note what the data shows. Do not make demographic or neighborhood quality judgments. Frame all sub-market observations around data patterns only.

For any sub-market where Joe has a city guide on the site, link to that guide inline. Use the URL patterns from Sellingpdxhomes\_SEO\_Complete.xlsx.

### Inventory in Months: The Full Picture

H2: "Inventory in Context: Where We Are in the Cycle"

Display the full three-year inventory table extracted from the RMLS report. Rows are months, columns are 2023, 2024, 2025\. Style it cleanly with alternating row shading.

One paragraph explaining what the table shows about the seasonal pattern and the year-over-year trend. Note whether 2025 inventory is running higher, lower, or flat relative to the same periods in 2023 and 2024\. Note the peak and trough months for each year visible in the data and what those patterns mean for buyers planning their search timing.

### Looking Ahead Section

H2: "What to Watch in the Coming Months"

A bulleted list of five to seven factors. Each bullet names one specific factor and explains in one sentence why it is relevant to Portland Metro buyers or sellers in the near term. Factors always include: pending sales as a leading indicator for next month's closed sales, the Freddie Mac rate trajectory, seasonal inventory patterns based on historical RMLS data, any external context findings from Phase 1 that have near-term implications.

Do not make specific price predictions. Frame every forward-looking statement as a factor to monitor, not a forecast. Example: "Pending sales fell 6.9% from December 2024, which suggests January 2026 closed sales may come in below December's pace unless rate movement brings additional buyers off the sidelines."

### FAQ Accordion

Five to seven questions. Research the actual questions buyers and sellers search for in the context of the current reporting period's market conditions. Always include these baseline questions adapted to current data:

- Is now a good time to buy a home in Portland?  
- How much have Portland home prices changed in the past year?  
- What does \[current inventory figure\] months of inventory mean for buyers?  
- Are Portland home prices going to fall?  
- How long are homes taking to sell in Portland right now?  
- How does Portland's market compare to the national market?  
- What neighborhoods in Portland are seeing the most activity?

Answers are four to six sentences each. Direct. Grounded in the data extracted in Phase 1\. No hedging beyond what is genuinely warranted by uncertainty. No pressure language. No predictions stated as certainties.

Include FAQPage schema in the Lofty head injection field only when this section is present. The questions in the schema must match the visible questions word for word.

### CTA Block

Two CTAs side by side. Left: "Browse Current Listings" linked to the listings search. Right: "Get a Home Valuation" linked to the evaluation page. Below both: one sentence inviting a conversation. "If anything in these numbers raises questions about your specific situation, reach out directly." Link "reach out" to /contact.

### Data Sources Block

Required on every market report. List all sources used with outbound links:

- RMLS Market Action Report for the specific reporting period  
- Freddie Mac Primary Mortgage Market Survey (specific date)  
- NAR Existing Home Sales report (most recent cited)  
- HUD Area Median Income for Portland Metro (year noted)  
- Any additional external sources used in the external context section

### Author Bio

Three sentences maximum. Joe Saling, Saling Homes at eXp Realty. 10 years Portland Metro real estate, 20 years sales and marketing leadership. Education-first approach. Phone, email, and website linked. Do not mention commission. Do not mention service areas.

### EHO Statement

"Saling Homes at eXp Realty is committed to equal housing opportunity. We do not discriminate on the basis of race, color, religion, sex, handicap, familial status, or national origin."

---

## DESIGN SYSTEM

All market reports inherit the full CSS design system from the Community Guide Master. CSS variables, typography, Lofty fixes, and component patterns are identical.

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

Google Fonts link required in Lofty head injection field on every post.

Each post uses a unique wrapper ID scoped CSS block. Wrapper ID format: market-report-\[month\]-\[year\]. Example: market-report-december-2025.

All viewBox attributes lowercase. Tables wrapped in scroll containers. Dark section margin fix applied.

Schema in Lofty head injection field only. Never in the post body.

---

## SCHEMA MARKUP

Required on every market report. In Lofty head injection field.

**Article schema:** headline (H1 text), image (hero image URL when available, placeholder acceptable for pre-publish), author name Joe Saling, publisher name Saling Homes at eXp Realty, datePublished (first day of the month following the reporting period), dateModified (same as published for market reports, never updated), description (meta description text), keywords (primary and secondary keywords).

**BreadcrumbList schema:** Home \> Blog \> \[Post Title\]. Use actual published URL.

**FAQPage schema:** Include only when FAQ accordion is present. Questions must match visible questions word for word.

---

## VOICE AND TONE

Market reports use the most measured and data-grounded tone of all content on the site. Joe is not cheerleading the market. He is not catastrophizing. He is reading the numbers honestly and explaining what they mean for a person making a real financial decision.

If the market is softening, say so directly and explain the mechanism. If prices are falling, name the sub-markets where this is most pronounced and the sub-markets where it is not. If affordability is improving, show the math. If inventory is rising and giving buyers more power, name that power specifically.

The reader of a market report is often in the middle of a decision. They need accurate information, not reassurance. The most trustworthy thing Joe can do is tell them what is actually happening, including when the news is not favorable.

No forbidden words. No pressure language. CTAs are invitations not demands.

---

## POST-BUILD DELIVERABLES

### Image Brief Block

Every market report uses one to two images maximum beyond the hero. For each image slot:

Marbalism prompt: minimum 80 words, location-specific to Portland Metro, season-appropriate to the reporting month, specific visual content that cannot be confused with any other post. Include the file name using naming convention: \[photo-id\]-market-\[month\]\[year\].webp

Required image: hero image. Portland Metro aerial, neighborhood street, or relevant economic landmark. Season-appropriate. Realistic. No generic stock imagery description. Name a specific Portland neighborhood or landmark that is identifiable in the image.

Optional second image: a sub-market spotlight image for the highest-performing sub-market in the report. Only include if it genuinely adds context.

### Follow-Up Content Ideas

Two to three post ideas that extend this month's report. For each: post type (from the Blog Post Master categories), working title, primary search query it targets, which section of the current market report it extends and with what anchor text link.

---

## LOFTY TECHNICAL RULES

All CSS scoped to the wrapper ID. All viewBox attributes lowercase. Dark background sections use the margin fix. Schema in head injection field not in body. Tables wrapped in scroll containers. Hero image uses loading="eager". All other images use loading="lazy".

---

## MOBILE DESIGN STANDARDS

Joe's site is mobile-user heavy. Every market report must be fully optimized for mobile screens before it is optimized for anything else. Desktop is secondary. Mobile is primary.

Market reports are data-dense by nature. This makes mobile optimization especially important. Tables, charts, and sub-market grids that work on desktop can become unusable on a phone without proper mobile handling.

### Breakpoints

768px: Tablet adjustments. Sub-market table gets scroll container treatment. Multi-column stat blocks collapse.

480px: Phone-specific. Most of Joe's mobile traffic is on screens between 375px and 430px. Design for that range first.

### Mobile Font Sizes at 480px

H1: 1.9rem H2: 1.45rem H3: 1.2rem Body text: 1.05rem, line-height 1.85 Table cells: 0.88rem Captions and labels: 0.82rem Buttons: 1rem, weight 600

### Mobile Layout Rules

Sub-market table: always in an overflow-x auto scroll container. This is the most important mobile rule for market reports. Never let the table break the page layout on mobile.

Stat highlight boxes: single column at 480px regardless of desktop column count.

Chart or data callout boxes: full width at 480px, padding reduces to 16px 18px.

CTA buttons: stack vertically at 480px, width 100%, min-height 48px.

### Touch Target Sizing

FAQ accordion summaries: min-height 48px, padding 14px 16px, full width tap target.

Buttons: min-height 48px, padding 14px 24px.

### Mobile Color and Contrast

Gold (\#D4AF37) on white fails WCAG AA. Never use gold as body text. Gold is for borders, accents, and icons only. Body text \#444444 on white. Text on dark backgrounds \#FFFFFF.

### Required Mobile CSS Pattern

```css
@media (max-width: 768px) {
  #[post-id] h1 { font-size: 2.1rem; }
  #[post-id] .stat-grid { grid-template-columns: 1fr 1fr; }
  #[post-id] .data-table-wrap { overflow-x: auto; -webkit-overflow-scrolling: touch; }
  #[post-id] .cta-buttons { flex-direction: column; }
  #[post-id] .cta-buttons a { width: 100%; text-align: center; }
}

@media (max-width: 480px) {
  #[post-id] h1 { font-size: 1.9rem; }
  #[post-id] h2 { font-size: 1.45rem; }
  #[post-id] h3 { font-size: 1.2rem; }
  #[post-id] { font-size: 1.05rem; line-height: 1.85; }
  #[post-id] table { font-size: 0.88rem; }
  #[post-id] .stat-grid { grid-template-columns: 1fr; }
  #[post-id] .callout-box { padding: 16px 18px; }
  #[post-id] .faq-acc summary { min-height: 48px; padding: 14px 16px; }
  #[post-id] .btn-primary,
  #[post-id] .btn-secondary {
    display: block;
    width: 100%;
    text-align: center;
    margin-bottom: 12px;
    min-height: 48px;
  }
}
```

---

## PRE-PUBLISH CHECKLIST

**Data accuracy:** Every figure in the post traced to a named RMLS file or named external source. No estimated or rounded statistics. Year-over-year comparisons use same-month prior year, not rolling average, unless explicitly noted as a rolling comparison (which RMLS sometimes uses for price figures). All external context figures cited with source name and date.

**Content completeness:** All required sections present in the specified order. Quick Answer box present and positioned before TOC. Story sentence present in opening paragraph. Affordability calculation verified mathematically. Sub-market table includes all 15 zones or notes any zone not reported. Looking Ahead section has minimum five factors. FAQ has minimum five questions.

**Technical:** Schema in head injection field not in body. All viewBox attributes lowercase. Wrapper ID present. Google Fonts link in head. Tables in scroll containers. Hero image loading eager, all others loading lazy. FAQPage schema questions match visible FAQ questions word for word.

**Mobile:** Both breakpoints present (768px and 480px). Sub-market table in scroll container. Body text minimum 1.05rem at 480px. Stat grids collapse to single column at 480px. CTA buttons stack vertically at 480px. FAQ accordion tap targets minimum 48px. No gold text on white backgrounds.

**Links:** Minimum three internal links from SEO spreadsheet confirmed. All external source links verified active. Data Sources block complete with all sources linked. Zillow and Redfin may be linked only when cited for directional validation as defined in the Context Framework. Never link to Zillow or Redfin as a source for specific price figures or transaction counts.

**SEO:** Meta title 55 to 60 characters confirmed. Meta description 145 to 155 characters confirmed. Slug includes month and year. Primary keyword appears in H1, opening paragraph, and meta title.

**Fair Housing:** EHO statement present. No demographic language in sub-market analysis. All sub-market observations framed around data patterns only.

**Post-Build:** Image briefs delivered. Follow-up content ideas delivered.

---

## AGENT INFORMATION

Fixed. Do not alter.

Name: Joe Saling Company: Saling Homes at eXp Realty Phone: (503) 910-7364 Email: [joe@sellingpdxhomes.com](mailto:joe@sellingpdxhomes.com) Website: [www.sellingpdxhomes.com](http://www.sellingpdxhomes.com)

---

*Saling Homes Market Report Master File v1.1 | February 2026* *Upload alongside all 26 RMLS PDF files and Sellingpdxhomes\_SEO\_Complete.xlsx at the start of every market report conversation.*  
