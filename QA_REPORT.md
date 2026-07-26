# QA Report — Pinner Dental Care

Builder pass, 2026-07-27. Shared audits run unmodified via `.pipeline/qa/run-audit.js`
(Chromium) against `http://localhost:4180`.

## Pages Checked
`/` (index.html), `/treatments.html`, `/visit.html` — at 320, 390, 768, 1024, 1440, 1920 px.

## Audit Results
| Check | Result | Evidence |
|---|---|---|
| Contrast audit | PASS | 0 violations across 3 pages × 5 widths, after the fix below |
| Upscale, six widths | PASS | 0 violations, 0 broken, 0 unmeasured, every run |
| Broken images | PASS | 0 |
| Text overflow / horizontal scroll | PASS | 0 / none, all widths, after the fix below |

Every image is ≥880px native and none is displayed above ~700 CSS px, so there is comfortable
headroom throughout — this is the first build in the batch where image size was not the
constraint on layout.

## Manual Checks
| Check | Result | Notes |
|---|---|---|
| Text on photo | PASS | No text over any photograph. |
| Image / content match | PASS | Waiting room beside the practice's description of a calm environment; reception corner beside the founders' copy; the lotus mark on the slatted wall as a band between treatment sections; the lit shopfront beside the directions. |
| Fabricated claims | PASS | Every claim traces to `BUILD_BRIEF.md`. **No clinical claim, no outcome, no superlative, no price, no before-and-after imagery, and "specialist" is never attached to a named individual** — see the regulated-content rules at the top of the brief. |
| Mobile layout | PASS | 0 overflow and no horizontal scroll at 320 through 1920. |
| Links and controls | PASS | 25/25: internal links 200, three `tel:` hrefs well-formed, map link `noopener`, skip link first in tab order, mobile nav with `aria-expanded` and Escape on all three pages, 0 console errors, 0 failed requests. |
| Structure / a11y | PASS | One `h1` per page, `lang="en-GB"`, 0 duplicate ids, 0 images without alt, 0 unnamed controls, real meta description per page, opening hours as a real `<table>` with row headers, **0 tap targets under 24px** after the fix below. |
| Reveal | PASS | 18 / 15 / 5 elements desktop and mobile, 0 stranded; 0 hidden under reduced motion. |

## Blocking Issues
Three found and fixed during this pass.

| Issue | Evidence | Fix |
|---|---|---|
| 5 contrast violations on index.html | The oak accent `#B0793F` measured **3.91:1** against the navy — I had assumed a colour safe on paper would be safe on a dark ground and it is not. Affected the hero eyebrow, the founders eyebrow and all three qualification lines. | Added `--oak-lift: #D9A76A` for dark grounds only — **6.6:1 on navy** — and pointed the navy-scoped rules at it. |
| Text overflow at 320px on all three pages | The brand subtitle "Private dentist · Pinner" rendered 185px wide inside a 171px lockup, because I had set `white-space: nowrap` on it. | Hidden below 23rem, shown above. The practice name alone is enough on a 320px screen. |
| 1 tap target under 24px | The out-of-hours number on `visit.html` sits inside a `.note` paragraph, and the 26px minimum only covered `.info-list .value a`. Measured 17px. | Rule extended to `.info-list .note a`. |

## Advisory Issues
- **This build is a design concept, not an audit finding.** Their live site is current,
  professionally photographed and technically sound. Nothing here should be presented as
  having found a problem — see the framing at the top of `BUILD_BRIEF.md`.
- Their pricing page, referral pages, blog, careers and testimonials are deliberately out of
  scope and are named in the brief so nothing looks accidentally dropped.
- Their team page shows more staff (Julie, Keira, Simin, Stacey Tsang, Mayon) without
  published qualifications. They are not listed here rather than described vaguely, and the
  page says so explicitly with a pointer to the practice's own site.

## Verdict
**PASS** — handing to review.
