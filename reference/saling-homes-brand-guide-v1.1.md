# SALING HOMES
## Brand Style Guide
### Version 1.1 | March 2026

Joe Saling | Saling Homes at eXp Realty
www.sellingpdxhomes.com
(503) 910-7364 | joe@sellingpdxhomes.com

---

## BRAND OVERVIEW

Saling Homes is a buyer-focused real estate brand serving the Portland metro area. Our brand communicates trust, expertise, and a premium client experience. Every interaction, from our website to printed guides, should feel consistent, professional, and approachable.

This guide establishes the visual standards for representing the Saling Homes brand across all channels: website, social media, presentations, printed materials, email campaigns, and signage.

---

## BRAND VOICE & POSITIONING

Our brand voice is educational, confident, and approachable. We explain complex topics in plain language. We advocate for our clients without being pushy. We lead with value and expertise, not sales pressure.

**Brand Tagline:**
*"I believe in listening to your needs, and then educating and advocating on your behalf."*

**Key Brand Attributes:**

We are transparent about process, costs, and compensation. Clients trust us because we do not hide the details.

We bring 10+ years of real estate experience and 20+ years in sales and leadership. That shows in how we handle problems, not in how we talk about ourselves.

No jargon, no pressure. We make complicated things feel manageable and we meet people where they are.

The dark/gold palette and clean design set us apart from typical real estate branding. It feels polished without trying too hard.

---

## COLOR PALETTE

Our palette is built on contrast between deep near-black and warm gold. This combination reads as confident and premium while standing apart from the blues and greens common in real estate branding.

**The CSS Variable System**

All color values are implemented through CSS custom properties. These are the governing values for every web build. Use these exact hex values. Do not substitute approximations.

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

**Primary Colors**

| Swatch | Name | Hex | Usage |
|--------|------|-----|-------|
| | Near Black | #222222 | Navigation, hero sections, headings, stage badges, footer backgrounds. The dominant dark color that grounds the brand. |
| | Gold Rich | #D4AF37 | Primary button backgrounds, key accent elements. The signature gold at full saturation. |
| | Gold | #C9A84C | Dividers, bullet accents, borders, icons. Mid-tone gold for supporting elements. |
| | White | #FFFFFF | Card backgrounds, body areas, intro sections. Provides breathing room and contrast. |

**Text Colors**

| Swatch | Name | Hex | Usage |
|--------|------|-----|-------|
| | Body Text | #444444 | Primary body copy. Used for all paragraph text throughout the site and documents. |
| | Muted | #767676 | Captions, fine print, timestamps, metadata. For information that is present but not primary. |

**Accent and Utility Colors**

| Swatch | Name | Hex | Usage |
|--------|------|-----|-------|
| | Gold Light | #C9952A | Button hover states. Also used as text color on dark backgrounds where full gold-rich is too bright. |
| | Gold Pale | #FBF5E6 | Very pale gold for subtle background highlights on cards or callout boxes. |
| | Border | #E2DDD6 | Card borders, divider lines, table borders. Soft structural element. |
| | Background Soft | #F7F5F2 | Page backgrounds and section backgrounds. Keeps content areas feeling soft and professional without being stark white. |

**Button Color Rules**

Primary buttons use Gold Rich (#D4AF37) as the default background with white (#FFFFFF) text. Hover state uses Gold Light (#C9952A). This is the accepted brand standard.

Note: WCAG AA contrast ratio between #D4AF37 and white is approximately 2.5:1, which does not technically meet the 4.5:1 minimum for normal text. This tradeoff is accepted on brand grounds. Button labels use bold weight and generous padding to maximize legibility within the brand palette.

Secondary (ghost) buttons on dark backgrounds use a transparent background with a white semi-transparent border (rgba(255,255,255,0.45)) and white text. Hover state brightens the border to rgba(255,255,255,0.9).

Never use dark amber (#7A5C00) or any off-brand dark color as a button background. Brand gold is the standard.

---

## TYPOGRAPHY

We use two font families that complement each other: a serif for headings that conveys authority, and a clean sans-serif for body text that ensures readability.

**Playfair Display**

Role: Headings, titles, section headers
Weights: 400 (Regular), 600 (SemiBold), 700 (Bold)
Source: Google Fonts

Playfair Display brings a refined editorial quality to our headings. Use it for all heading levels (H1-H3), page titles, and feature callouts. Never use it for body text.

**Source Sans 3**

Role: Body text, buttons, navigation, UI elements
Weights: 300 (Light), 400 (Regular), 600 (SemiBold)
Source: Google Fonts

Source Sans 3 is our workhorse typeface. Use it for all body copy, bullet points, buttons, navigation labels, and any text that is not a heading.

**Type Scale (Web)**

| Element | Font | Size | Usage |
|---------|------|------|-------|
| Page Title (H1) | Playfair Display 700 | 2-3rem | Hero headings, page titles |
| Section Title (H2) | Playfair Display 700 | 1.6-2.2rem | Section headers, card titles |
| Subsection (H3) | Playfair Display 600 | 1.3-1.5rem | Card headings, step titles |
| Body Text | Source Sans 3 400 | 1-1.1rem | Paragraphs, descriptions |
| Detail Items | Source Sans 3 400 | 1-1.08rem | Bullet points, list items |
| Small / Caption | Source Sans 3 400 | 0.85-0.95rem | Badges, labels, fine print |
| Buttons | Source Sans 3 600 | 0.95-1.05rem | CTA buttons, navigation links |

**Mobile Typography Minimums**

Body text never below 1rem on mobile. Use 1.05rem as the working minimum. Headings scale down proportionally but never below 1.3rem for H3 and 1.5rem for H2 at 480px.

**Fallback Fonts**

- Headings: Georgia, Times New Roman, serif
- Body: Arial, -apple-system, sans-serif

---

## DESIGN ELEMENTS

**Gold Divider Lines**

A 60px wide, 3px tall gold (#D4AF37) horizontal rule is used as a visual separator below section titles.

**Gold Bullet Dots**

List items use a 7-8px solid gold (#D4AF37) circle as the bullet marker instead of default bullets. This applies to all detail lists on the website and in HTML embed blocks.

**Cards**

Content cards use white (#FFFFFF) backgrounds with a 1px border (#E2DDD6), 16px border radius, and a subtle box shadow (0 2px 12px rgba(0,0,0,0.04)). On hover, cards lift slightly with translateY(-4px) and a deeper shadow.

**Buttons**

Primary buttons: Gold Rich (#D4AF37) background, white text, 12px border radius, 600 weight. Hover darkens to Gold Light (#C9952A) with a slight lift. Box shadow: 0 4px 16px rgba(212,175,55,0.3), deepens to 0 8px 24px rgba(212,175,55,0.45) on hover.

Secondary buttons (dark backgrounds only): Transparent background, white text, 2px semi-transparent white border, 12px border radius. Hover brightens border. Used in hero sections only.

**Dark Sections**

Hero and highlight sections use a linear gradient background (160deg, #1a1a1a to #222222 to #2a2a2a) with subtle radial gold light effects for depth. Text on dark backgrounds uses white for headings and rgba(255,255,255,0.85) for body text.

**Badges and Labels**

Stage badges use a dark (#222222) background with white uppercase text, 6px border radius. Hero badges use a semi-transparent gold background with a gold border and light gold (#E8D48B) text.

**Icons**

SVG line icons (Lucide icon set or equivalent) are preferred over emojis. Icons use gold (#D4AF37) stroke color with 1.5px stroke width on dark backgrounds, and dark (#222222) stroke on light backgrounds. Typical sizes: 32px for feature cards, 18px inline with buttons.

---

## FAIR HOUSING STANDARDS

Fair housing compliance is a non-negotiable requirement across every piece of content Saling Homes produces. This applies to website pages, blog posts, social media, email, printed materials, and any other channel.

**The Core Rule**

Never describe a neighborhood, city, area, school, or community using language that references, implies, or signals the racial, ethnic, religious, national origin, familial, or any other protected class composition of the people who live there.

**The Seven Protected Classes**

Under the Fair Housing Act, it is illegal to discriminate based on:
1. Race
2. Color
3. Religion
4. Sex
5. Handicap (disability)
6. Familial status
7. National origin

Oregon state law adds additional protections. All content must comply with both federal and Oregon standards.

**What This Means in Practice**

Describe neighborhoods and cities using physical characteristics, amenities, infrastructure, and lifestyle factors. Never use these as proxies for demographics:

- School ratings presented without demographic context (acceptable to name ratings, not to imply demographic homogeneity)
- Crime statistics framed around neighborhood character (do not use)
- "Community feel" language that implies exclusivity (do not use)
- References to who the neighborhood is "right for" based on protected class (do not use)

**Language to Avoid**

Never use language that steers buyers toward or away from a location based on demographics, even subtly. This includes:

- "Family-friendly" used as a coded term (acceptable only when describing specific amenities like playgrounds or schools)
- "Up-and-coming" applied to neighborhoods in ways that imply demographic change
- Any description that could be read as signaling the racial or ethnic composition of an area
- Comparisons between neighborhoods that implicitly rank them by demographics

**The EHO Statement**

Every published page and post must end with the Equal Housing Opportunity statement. The required format names all seven protected classes:

*"Saling Homes at eXp Realty is committed to the principles of the Fair Housing Act. We do not discriminate on the basis of race, color, religion, sex, handicap, familial status, or national origin."*

This statement is required on: every city guide, every neighborhood guide, every blog post, every market report. It is not optional and it is not abbreviated.

**When in Doubt**

If any sentence in a piece of content could be read as directing a buyer toward or away from a location based on who lives there rather than what is there, rewrite it or remove it. The test is not intent. The test is whether the language could be interpreted as steering.

---

## USAGE GUIDELINES

**Do**

- Maintain the dark/gold contrast as the primary visual signature
- Use gold sparingly as an accent, not as a primary background color
- Keep typography consistent: Playfair for headings, Source Sans 3 for body
- Use SVG icons over emojis in all professional materials
- Ensure sufficient contrast for text readability
- Use the brand voice: educational, confident, and approachable
- Include the EHO statement on every published page

**Do Not**

- Introduce new colors outside this palette without brand approval
- Use gold text on light backgrounds (poor contrast - use gold for accents and borders only)
- Mix Playfair Display into body text paragraphs
- Use generic stock imagery without checking it aligns with the premium feel
- Use a salesy or high-pressure tone in copy
- Use demographic language to describe neighborhoods, schools, or communities
- Stretch or distort the SH logo

---

## QUESTIONS?

For questions about brand usage, design assets, or approvals, contact:

**Joe Saling**
Saling Homes at eXp Realty
(503) 910-7364 | joe@sellingpdxhomes.com
www.sellingpdxhomes.com

---

*Saling Homes Brand Style Guide v1.1 | March 2026*
*Updated: CSS variable system added as governing color reference. Button color rules documented. Body text color corrected to #444444. Background soft color corrected to #F7F5F2. Fair Housing Standards section added.*
