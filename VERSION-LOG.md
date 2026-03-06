# Saling Homes Content System - Version Log & File Registry

Joe Saling | Saling Homes at eXp Realty | sellingpdxhomes.com | Last Updated: March 2026

This file is the single source of truth for the Saling Homes content system. Every project reads this file at the start of every session to determine which master file versions to fetch.

---

## 1. Current Master Files and Templates

| File Name | Version | Last Updated | Status |
|-----------|---------|--------------|--------|
| SH-Master-Master | v1.2 | March 2026 | Current |
| SH-Blog-Master | v1.3 | February 2026 | Current |
| SH-Community-Guide-Master | v3.5 | March 2026 | Current |
| SH-Community-Guide-Template | v1.5 | March 2026 | Current |
| SH-Neighborhood-Guide-Master | v1.1 | February 2026 | Current |
| SH-Neighborhood-Guide-Template | v1.0 | February 2026 | Current |
| SH-Market-Report-Master | v1.2 | March 2026 | Current |
| SH-Market-Report-Template | v1.0 | March 2026 | Current |
| SH-Market-Report-Template-Brief | v1.0 | March 2026 | Current |
| SH-Marblism-Instructions | v1.1 | February 2026 | Current |

All files are stored in the SH Master Files folder in Google Drive (folder ID: 1mFuA1Iaj-xa7xxmdUX9L_SyErgRj1kNb) and mirrored in this GitHub repository.

*System prompts are static. They do not change when master files are updated.*

---

## 2. Reference Documents

| Document | Purpose | Stored In |
|----------|---------|-----------|
| saling-homes-brand-guide.docx | Source of truth for colors, fonts, design elements | Content System HQ + Google Drive |
| saling-homes-tone-positioning.docx | Source of truth for voice, forbidden words, CTA language | Content System HQ + Google Drive |
| Sellingpdxhomes_SEO_Complete.csv | URL validation for all internal links. Required in every content project | All five projects + Google Drive |
| Lofty-Listing-Search-URL-Reference.md | URL construction guide for condition-filtered city search pages | GitHub repo reference/ folder + Google Drive |
| VERSION-LOG.md (this file) | Single source of truth for current versions, file locations, and change history | GitHub repo + Google Drive |

---

## 3. Full Version History

| File | Version | Date | What Changed |
|------|---------|------|--------------|
| SH-Blog-Master | v1.0 | Feb 2026 | Initial release. Four categories, shared rules, schema, SEO suite, linking rules, pre-publish checklist. |
| SH-Blog-Master | v1.1 | Feb 2026 | Lofty HTML structure rule. External link attributes. CTA URL standards locked. FAQ minimum raised to 6. Data verification timestamp. Author bio as styled box. |
| SH-Blog-Master | v1.2 | Feb 2026 | Full Mobile Design Standards added. Two breakpoints (768px and 480px). |
| SH-Blog-Master | v1.3 | Feb 2026 | Category 5: Marblism Compliance Pass added. Surgical compliance workflow for Marblism HTML. |
| SH-Community-Guide-Master | v2.9 | Feb 2026 | Full Mobile Design Standards added. Extended 680px breakpoint. New 480px phone breakpoint. |
| SH-Community-Guide-Master | v3.0 | Mar 2026 | Template updated from v1.1 to v1.2. Full mobile design standards. Seven layout brief changes. Eight mobile improvements. |
| SH-Community-Guide-Master | v3.1 | Mar 2026 | Button selector chain fix. Button contrast fix (dark amber). Cloudflare email documentation. Market Updates absolute URL fix. Duplicate image rule. Orphaned CSS brace warning. |
| SH-Community-Guide-Master | v3.2 | Mar 2026 | Nav restored after v3.1 removal. Bullet suppression CSS added (four paths). |
| SH-Community-Guide-Master | v3.3 | Mar 2026 | Dining section standard (14 spots, 6/3/2/1/2 category breakdown). Collapsible content sections. Listing search grid added. |
| SH-Community-Guide-Master | v3.4 | Mar 2026 | Button color restored to brand gold. Nav fix/release script replaces position:sticky. btn-secondary ghost button component added. |
| SH-Community-Guide-Master | v3.5 | Mar 2026 | Pre-GO output block defined: SEO suite, image briefs with slot-specific dimensions and Phase 1-determined count, SNS image brief, neighborhood spoke list, price range tiers with encoded Lofty URLs. Post-GO output block defined: HTML, schema block, internal and external link table. Meta title rule updated to 60-char clean snippet with 70-75 char total limit. Image brief format standardized. Neighborhood count raised to 10-13. Lofty search URL construction rule added to Linking Rules. Schema placement corrected from head injection to Lofty embed block. |
| SH-Community-Guide-Template | v1.0 | Feb 2026 | Initial release. |
| SH-Community-Guide-Template | v1.1 | Feb 2026 | Full Mobile Design Standards added. |
| SH-Community-Guide-Template | v1.2 | Mar 2026 | Seven layout brief changes applied: hero CTA button, nav trimmed to 7 items, comparison table moved, mid-page CTA added, Joe's Take contact block removed, Explore More restyled, mobile improvements. |
| SH-Community-Guide-Template | v1.3 | Mar 2026 | Collapsible sections, listing search grid, dining expand block, btn-secondary component, nav is-fixed script. |
| SH-Community-Guide-Template | v1.4 | Mar 2026 | Full placeholderization from Tigard v2 production baseline. Button colors restored to gold. Nav fix/release script. All Marblism images replaced with placeholder SVGs. |
| SH-Community-Guide-Template | v1.5 | Mar 2026 | Schema comment block updated: removed "HEAD INJECTION FIELD" reference, replaced with "LOFTY EMBED BLOCK AT TOP OF PAGE". |
| SH-Neighborhood-Guide-Master | v1.0 | Feb 2026 | Initial release. |
| SH-Neighborhood-Guide-Master | v1.1 | Feb 2026 | Full Mobile Design Standards added. City guide link format locked to /living-in-[city]-oregon. |
| SH-Market-Report-Master | v1.0 | Feb 2026 | Initial release. |
| SH-Market-Report-Master | v1.1 | Feb 2026 | Full Mobile Design Standards added. |
| SH-Market-Report-Master | v1.2 | Mar 2026 | Content Architecture replaced with pointer to Template Brief and HTML Template. Tariff/construction cost context added. Pre-publish checklist updated. |
| SH-Market-Report-Template | v1.0 | Mar 2026 | Initial release. Pre-built HTML/CSS template for monthly market reports. |
| SH-Market-Report-Template-Brief | v1.0 | Mar 2026 | Initial release. Three-act content architecture defined. |
| SH-Marblism-Instructions | v1.0 | Feb 2026 | Initial release. |
| SH-Marblism-Instructions | v1.1 | Feb 2026 | Section 8: Mobile Design Standards added. |
| SH-Master-Master | v1.0 | Mar 2026 | Initial release. Cross-project governing file. |
| SH-Master-Master | v1.1 | Mar 2026 | Removed hardcoded version numbers. Added Version Log check instruction. |
| SH-Master-Master | v1.2 | Mar 2026 | Market Report Template and Brief references added. Drive startup instruction updated. |
| Lofty-Listing-Search-URL-Reference | v1.0 | Mar 2026 | Initial release. Base URL structure, full condition object reference, value format rules, property types, listing statuses, keyword patterns, common search examples, encoded/decoded example. |
| All System Prompts | static | Mar 2026 | Removed version numbers. Replaced with Drive startup sequence that reads Version Log for current master file versions. |

---

## 4. Pending Items

| Item | Affects | Priority | Status |
|------|---------|----------|--------|
| No automated workflow to update city guide when new neighborhood guide is published | Cross-project | Low | Pending - manual step for Joe |

---

## 5. How to Keep This File Current

- When a master file is updated: increment its version number, update Section 1 table, add a row to the Version History, commit the new file to the repo.
- When a pending item is resolved: remove it from Section 4 and add the resolution to Section 3.
- When a new file is created: add it to the appropriate table and note it in Section 3.
- This file lives in the repo root. It is also uploaded to Google Drive and the Content System HQ project.

---

*Saling Homes Content System Version Log | Joe Saling | joe@sellingpdxhomes.com | (503) 910-7364*
