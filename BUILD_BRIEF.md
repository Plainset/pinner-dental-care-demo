# Build Brief — Pinner Dental Care

Spec redesign. Built 2026-07-27 from `active leads/LEAD_REGISTER.md` lead #7.
No outreach authorised; this is a build only.

## Read this before anything else — what this build is and is not

The register classifies this lead `dated_only` (0 points, hard exclusion) and records that
Alex deferred it, with his own note: *"website is decent, just awkward — we can make it
better design wise."*

**That assessment is right and this build does not overturn it.** Their live site is
substantial, current and professionally photographed: a Webflow build with correct meta
descriptions on every page, a blog running monthly to **March 2026**, a team page with named
clinicians and qualifications, a practice gallery, live job vacancies, published opening
hours, a cancellation policy and an online booking portal. There is **no defect** here.

So this is a **design concept**, built to answer the thing Alex actually said he wanted —
"better design wise" — and not an audit-first pitch. It cannot enter the audit campaign and
should not be presented as though it found something wrong.

## Regulated health content — the rules this build works under

Dentistry is GDC-regulated and advertising is constrained. This build therefore:

- Makes **no clinical claim of its own.** Every treatment description is the practice's own
  wording, condensed.
- Makes **no claim of superiority** — no "best", no "leading", no comparative claim.
- Uses **no before-and-after imagery** and promises no outcome.
- Uses the word **"specialist" only where the practice itself uses it**, and never attaches
  it to a named individual.
- Reproduces qualifications **exactly as published** and adds none.
- Carries no pricing, because their pricing sits behind a dedicated page this build does not
  reproduce and quoting a partial fee list for regulated treatment would be worse than
  quoting none.

## Contact
- Phone: **020 8868 9998**; out of hours **07483 911127**
- Address: **3 Barters Walk, Pinner HA5 5LU** — "next door to Sainsbury's"
- Email: no address published; the practice routes enquiries through a form and its online
  booking portal
- Source: https://www.pinnerdentalcare.co.uk/contact-us , read 2026-07-27
- Opening hours (published): Monday–Friday 8:00am–6:00pm; Saturday 9:00am–4:00pm; Sunday
  closed. The practice notes hours may vary around public holidays.

## Business State Check
- Status: **open and actively trading.** Blog posts monthly to March 2026; live job
  vacancies; online booking portal in use.
- Checked: their own site, crawled in a real browser 2026-07-27, every page 200.
- Single location. The multi-location rule does not apply.
- Build decision: **proceed as a design concept**, per the framing above.

## Page Plan
- Scope: 3 pages — `index.html` (Home), `treatments.html` (Treatments),
  `visit.html` (Visit &amp; contact)
- Their live site has far more (referrals, pricing, blog, careers, testimonials, gallery).
  A concept does not need to reproduce a whole practice site; it needs to show the design
  thinking. Out-of-scope sections are named here so nothing looks accidentally dropped.

## Allowed Facts
| Fact | Source | Used where |
|---|---|---|
| "Private dentist in Pinner offering general, cosmetic, restorative, and emergency dental care" | homepage meta | index |
| Strapline "A Healthy Smile is a Happy Smile" | homepage | index |
| **4.9 from 213 Google reviews**, shown on their homepage as "Top Rated on Google" | homepage | index |
| 3 Barters Walk, Pinner HA5 5LU, next door to Sainsbury's | contact page | visit, footer |
| 020 8868 9998; out of hours 07483 911127 | contact page | all pages |
| Opening hours Mon–Fri 8–6, Sat 9–4, Sun closed; may vary around public holidays | contact page | visit |
| Cancellation: 48 hours for standard appointments; one week for specialist and consultant appointments; deposits non-refundable on shorter notice | contact page | visit |
| Founded by husband-and-wife team Dr Rosh and Rupal Patel | our-team | index |
| Dr Rosh Patel — BDS Newcastle University 2006, principal dentist and co-founder; "over 20 years of experience in dentistry" | our-team | index |
| Rupal Patel — co-founder | our-team | index |
| Dr Ash Parmar — BDS hons (Sheffield), MJDF, PGCert Endodontics, PGDip Implant Dentistry | our-team | index |
| **Nine** treatment areas: routine dental care; general dentistry; dental hygiene; cosmetic dentistry; orthodontics; implants; oral surgery; dental emergencies; **dentistry for children** | homepage treatments overview + /patient-information/dentistry-for-children | treatments, index |
| Children's dentistry: gentle preventative care for children of all ages, from a baby's first check-up to teenage orthodontics, focused on prevention, education and building trust | /patient-information/dentistry-for-children | treatments |
| Bus routes H11, H12, **H13 and 183** serve Pinner Station (Stop C) | contact page | visit |
| Parking: Sainsbury's car park at 12 Barters Walk adjacent to the practice; Pinner Village Hall car park on Bridge Street; Love Lane car park — restrictions and time limits vary | contact page | visit |
| Dr Ash Parmar is a general and cosmetic dentist on the team, **not a founder** | our-team | index |
| Their own descriptions of each area (routine check-ups and hygiene; preventative and restorative including endodontics and fillings; whitening, composite bonding, veneers and smile makeovers; Invisalign and ceramic braces) | homepage | treatments |
| Dental hygiene is offered alongside routine care | homepage treatments overview | treatments |
| Implant treatment for replacing missing teeth and wider smile restoration | homepage treatments overview | treatments |
| Oral surgery is performed at the practice, and it also accepts referrals in | /dental-treatments/oral-surgery | treatments |
| Dental emergencies: urgent appointments, with a separate out-of-hours number | homepage + contact page | treatments |
| "0% finance available" / patient finance | homepage | treatments |
| Online booking through a secure portal | homepage | all pages |
| Patients come from Pinner, Harrow, Northwood, Ruislip, Hatch End and North West London | homepage | index |
| 3-minute walk from Pinner Underground (Metropolitan Line), with the practice's own verbatim walking directions | contact page | visit |

## Do Not Claim
| Claim | Reason |
|---|---|
| Any price, fee or finance APR | Their pricing lives on a page this build does not reproduce. A partial fee list for regulated treatment is worse than none. |
| Any clinical outcome, success rate or "results" | GDC-regulated. Nothing of the kind is published and nothing may be inferred. |
| "Specialist" attached to any named individual | Only a GDC-registered specialist may be described that way. The practice refers to "specialists" and "consultants" collectively; this build does the same and names no one as one. |
| Superlatives — best, leading, top, award-winning | No comparative or superiority claim is made. The 4.9/213 figure is reported as Google's number, attributed. |
| GDC registration numbers | Not published on their site; not invented. |
| Any before-and-after image or smile-transformation imagery | None used. |
| Named team members beyond the three whose qualifications are published | Their team page shows more people (Julie, Keira, Simin, Stacey Tsang, Mayon) but without qualifications; they are not listed here rather than described vaguely. |
| That any treatment is available on the NHS | The practice describes itself as private. Nothing about NHS provision is stated. |

## Asset Manifest
All photographs are the practice's own, from their own Webflow CDN. No patients appear in
any of them; every person shown is a named member of staff photographed for the practice.

| File | Source | Native size | Watermark checked | Intended section | Copy match |
|---|---|---|---|---|---|
| waiting-room.jpg | DSC01592 | 1600×1066 | yes | index hero | the waiting area — slatted wood wall, practice logo, window onto Barters Walk |
| shopfront-evening.jpg | DSC01705 | 1600×1066 | yes | visit | the practice frontage lit at dusk, name and phone number on the glass |
| logo-detail.jpg | DSC01629 | 1600×2401 | yes | treatments band | the practice's lotus mark on the slatted wall |
| founders.jpg | Rosh_and_Rupal | 1125×1500 | yes | index — beside the founders copy | Dr Rosh and Rupal Patel together |
| reception-corner.jpg | DSC01653 | 1600×2400 | yes | visit — below the shopfront | a corner of the reception: armchair, framed print, orchid against a dark blue wall |
| rosh-patel.jpg | Rosh.jpg | 1125×1500 → 880×1173 | yes | index — team | Dr Rosh Patel |
| rupal-patel.jpg | Rupal_Patel | 1125×1500 → 880×1173 | yes | index — team | Rupal Patel |
| ash-parmar.jpg | Ash_Parmar | 1125×1500 → 880×1173 | yes | index — team | Dr Ash Parmar |

Rejected:
- `AdobeStock_2133…` — stock photography on their own site ("Excited couple celebrating").
  Licensed to them, not to us, and generic. Not used.
- The treatment icon set (1440×1440 white-on-white logos) — several have alt text reading
  "Blank white image with no visible content", which is what they are. Useless.
- `Screenshot 2026-…` files — screenshots of third-party review widgets.
- `Emergency_Cut_out.webp` and `Girl_pointing…` — cut-out marketing images of people who are
  not identifiable staff; provenance unclear.

## Design Notes
- Palette: deep clinical navy `#152B3E` with a warm oak `#B0793F` drawn from the slatted
  timber in their own interior photographs, on a soft warm white. Deliberately calm — the
  practice's own copy leans on "calm", "welcoming" and "comfortable", and a dental site that
  shouts works against its own message.
- Type: a quiet humanist sans throughout, with generous line height. No display serif —
  this is the one build in the batch where restraint is the point.
- Image layout: wrapper `aspect-ratio` + `object-fit: cover`. Every native size is ≥880px, so
  there is comfortable headroom at every breakpoint.
- Engine: `engine.css` vendored; `data-reveal` motion overridden at site level as on the
  previous builds.

## Builder QA
See `QA_REPORT.md`.


## Reviewer round 1 — what changed (2026-07-27)

Scored 8.0 but **failed on one accuracy defect**, correctly.

**The practice offers nine treatment areas; I carried eight.** I missed **Dentistry for
Children**, which has its own page on their site and is advertised on their shopfront glass
— glass that is visible in a photograph this build uses. Worse, the page asserted
"Everything the practice offers, described in its own words", and that was untrue twice
over: the list was incomplete, and four of the eight descriptions were my own condensation
rather than their wording.

Fixed:
1. **Ninth card added** — Dentistry for Children, from their own copy. "Eight areas of care"
   → "Nine areas of care". The completeness claim is gone: the page now says "The care the
   practice offers, in summary", which is what it actually is.
2. **All four bus routes** — H11, H12, **H13 and 183**. My brief had recorded only the first
   two, so the error started here, not on the page. A visitor on the H13 or the 183 was
   being told their route did not serve the practice.
3. **Parking added to the Visit page** — the three car parks the practice names (Sainsbury's
   at 12 Barters Walk, Pinner Village Hall, Love Lane). A Visit page without parking
   under-served its one job.
4. **"The founders" no longer names someone who isn't one.** Dr Ash Parmar is a general and
   cosmetic dentist, not a founder. The section is now "The people / Who you will meet", the
   founding is described in the lede, and he has a role line like the other two.
5. **`founders.jpg` is now actually used** — beside the husband-and-wife copy it was always
   meant to illustrate. It and `shopfront-day.jpg` were catalogued as placed but never
   referenced; `shopfront-day.jpg` and `reception-corner.jpg` are deleted and the manifest
   corrected.
6. **The band crop on `treatments.html` cut the lotus mark in half** — a 16/6 frame centred
   on a 1600×2401 portrait source. Now `object-position: 50% 32%`.
7. **Cards re-columned to 3 with subgrid.** `auto-fit` resolved to four columns above 1280px,
   orphaning a row of two, and card heights within a row differed by up to 52px.
8. **Uppercase dropped from the qualification line.** "BDS hons(Sheffield)" was rendering as
   "BDS HONS(SHEFFIELD)"; for a regulated qualification string that is worth getting right.

The reviewer verified the regulated-content discipline term by term and found **no breach** —
and noted that the practice's own live site carries "gold standard", "outstanding dentistry",
"Real Patients, Real Results" and a before-and-after section, none of which this build
reproduces.


## Reviewer round 2 — PASS at 9.0/10, and the last changes

Professionalism 9, state 9.5, aesthetics & imagery 8.5. **Zero blocking defects.**

The reviewer enumerated every treatment URL on the live site — thirteen, of which two are not
treatments and two are sub-pages their own nav indents beneath a parent (Invisalign under
Orthodontics, EMS Airflow under Dental Hygiene) — and confirmed **exactly nine distinct
areas**, mapping one-for-one onto the build. It also checked the ninth card's wording against
their children's-dentistry page specifically because "a baby's first check-up to teenage
orthodontics" reads like invention, and found it sourced.

It re-ran the regulated-content sweep over the new copy: three benign hits, "specialist"
still exactly once in the practice's own cancellation wording. And it measured the subgrid
fix properly — **card-height spread 0px, `<h3>` offset spread 0px, `<p>` offset spread 0px in
every row at every width**, against up to 52px before.

Applied after the pass:

1. **`reception-corner.jpg` restored.** The reviewer's best point: my round-1 fix moved
   `founders.jpg` into place (right) but deleted the one interior that broke the
   slatted-oak-wall pattern (wrong half). It now sits on the Visit page below the shopfront —
   outside, then inside. The home page remains wall-heavy because that is how the practice's
   own photography is shot; this at least stops the site as a whole being one wall.
2. **Card 09 trimmed** from ~30 words to ~15, so it no longer forces dead space into the two
   short cards beside it.
3. **Band `object-position` 32% → 28%**, clearing the outer roundel's top arc.
4. **Whitening added to the cosmetic card** — their own copy lists it first, and it is the
   cosmetic treatment most people search for.
5. **Four unrowed card descriptions added to Allowed Facts** (hygiene, implants, oral surgery,
   emergencies), including the reviewer's finding that the practice performs oral surgery
   in-house *and* accepts referrals in.

Left undone and recorded: `visit.html` has no map. That is the real remaining gap on that
page, and it belongs with the canonical/OG/`LocalBusiness` schema work in a deploy checklist
rather than in a concept that is not deployed.
