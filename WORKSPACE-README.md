# Water Softener Albuquerque NM — Workspace

## Boilerplate build status (informational — not per-city data)
This section tracks what the *template itself* contains, independent of any
city. Update it when the boilerplate gains or loses a component; do not fill
in per-city data here — that's the rest of this file, below.

| Component | Status |
|---|---|
| Keystatic CMS | ❌ REMOVED — phone-call-based rank-and-rent model, site.config.ts edited directly, see PROVISION.md "CMS — No Keystatic" |
| Output mode | Static (`output: "static"`, `@astrojs/vercel`, zero serverless functions) |
| Full design system (global.css) | ✅ commit 3b6e9cf |
| Layout.astro (utility bar + Services-dropdown nav + minimal footer) | ✅ synced from Henderson structural improvements |
| Homepage (10 sections: hero, services grid, GPG data, 2 alternating image-text, CityMap placeholder, service areas, why-choose-us, FAQ accordion, slim CTA bar) | ✅ synced from Henderson structural improvements |
| New pages: repair, about, contact | ✅ created this pass |
| 6 expansion pages (salt-based-installation, salt-free-installation, water-softener-sizing, new-construction-installation, control-head-repair, free-water-test) | ✅ added 2026-09-23, ported from the Minneapolis site build — linked contextually from installation/repair/water-quality, not in main nav/footer |
| PageHero.astro (split inner-page hero: breadcrumbs, H1, opening paragraph, CTAs left; real photo or GPG stat-card right) | ✅ added 2026-09-24, wired into all 21 inner pages, replacing the old single-column `.page-header` + placeholder-image-section pattern. No real photography exists on the boilerplate, so every page renders the GPG stat-card fallback — a per-city task is to add real photos and pass them via the `image` prop, same as Tampa did |
| Opening paragraph pattern (Glendale Elite: Brand IS on homepage, Brand OFFERS inside the hero on inner pages) | ✅ updated 2026-09-24 — superseded the old separate `.page-opening` section below the header; now lives inside `PageHero`'s `opening` slot, brand name underlined and linked to `/`. Homepage still uses the older separate-section placement (`.page-opening` under the hero) — syncing it into the homepage hero itself is a separate, not-yet-requested task |
| QuoteForm.astro | ✅ commit 3b6e9cf, updated to use businessEmail |
| Breadcrumbs.astro | ✅ commit 3b6e9cf |
| LocalSchema.astro | ✅ (unchanged, already matched Henderson) |
| GPGSlider.astro | ✅ commit d084265 — wired into water-quality.astro this pass |
| GPGSliderMini.astro | ✅ commit d084265 — wired into comparison.astro this pass |
| SystemTour.astro | ✅ commit d084265 — wired into installation.astro this pass |
| QuickFacts.astro | ✅ added this pass (2026-09-25) — not from Henderson/Indianapolis, built new for this site to satisfy quality-gate Rule 14; imported on every EAV-scored inner page except comparison.astro |
| CLAUDE.md | ✅ (pre-existing, unchanged) |
| BRAND-GUIDE.md | ✅ (pre-existing, unchanged) |
| PROVISION.md (Step 5b added, Keystatic step removed, CMS section added) | ✅ this pass |
| HendersonMap.astro | ❌ city-specific, not copied — use CityMap.astro, build per city (needs real pin coordinates) |
| InstallationProcess.astro | ❌ city-specific — build per city (needs local copy) |
| Testimonials.astro | ❌ city-specific — build per city (needs local placeholder copy) |

**Next action**: Ready to provision the next city. The boilerplate now
ships 22 fixed pages (up from 16) — see PROVISION.md Step 5 for the full
list and Step 5c for the QDP-gated service-area pages that extend a city
toward the Core 30 target (`local-gbp-core30` skill in Local-SEO-Toolkit).

GPGSlider/GPGSliderMini/SystemTour all read city data from `site.config.ts`
automatically (city, gpgLow/gpgHigh, gpgLabel, waterSource, waterAuthority) —
no manual editing needed beyond filling in the config. See PROVISION.md
Step 5b for where to add each one.

## Site identity
- Domain:           albuquerquewatersoftener.com
- City:             Albuquerque, NM
- GPG:              6-10 (Moderately Hard to Hard)
- Water source:     Santa Fe Group Aquifer groundwater blended with San Juan-Chama surface water (since 2008)
- Water authority:  Albuquerque Bernalillo County Water Utility Authority (ABCWUA)
- Primary keyword:  albuquerque water softener (0 vol/mo — open data gap, no keyword-tool access from this build)
- GitHub repo:      assignmenthelptalk/albuquerquewatersoftener (not yet created — gh CLI unavailable, see Notes)
- Vercel project:   albuquerquewatersoftener
- Vercel URL:       https://albuquerquewatersoftener.vercel.app
- Live domain:      https://albuquerquewatersoftener.com

## Folder structure
- Local-SEO-Toolkit/
    data/albuquerquewatersoftener/topical-map.md        ← topical map
    data/albuquerquewatersoftener/briefs/               ← EAV briefs per page
    data/albuquerquewatersoftener/quality-report-*.json ← quality gate reports
- waterSoftenerProjects/albuquerquewatersoftener/
    src/site.config.ts                     ← city config (only file changed per city)
    src/pages/                             ← all page files (no CMS layer)
    dist/                                  ← built static HTML (after npm run build)

## Page status
| Page                           | Written | Score  | Ship-ready |
|--------------------------------|---------|--------|------------|
| homepage                       | ✅      | 82/100 | ✅         |
| water-quality                  | ✅      | 80/100 | ✅         |
| hard-water                     | ✅      | 85/100 | ✅         |
| installation                   | ✅      | 85/100 | ✅         |
| comparison                     | ✅      | 81/100 | ✅         |
| faq                            | ✅      | 90/100 | ✅         |
| neighbourhood                  | ✅      | 92/100 | ✅         |
| repair                         | ✅      | 89/100 | ✅         |
| about                          | ✅      | —      | n/a (no EAV brief, not scored) |
| contact                        | ✅      | —      | n/a (no EAV brief, not scored) |
| quote                          | ✅      | 83/100 | ✅         |
| products                       | ✅      | 83/100 | ✅         |
| whole-home-filtration          | ✅      | 80/100 | ✅         |
| reverse-osmosis                | ✅      | 80/100 | ✅         |
| resin-bed-replacement          | ✅      | 84/100 | ✅         |
| brine-tank-cleaning            | ✅      | 83/100 | ✅         |
| salt-based-installation        | ✅      | 87/100 | ✅         |
| salt-free-installation         | ✅      | 89/100 | ✅         |
| water-softener-sizing          | ✅      | 84/100 | ✅         |
| new-construction-installation  | ✅      | 86/100 | ✅         |
| control-head-repair            | ✅      | 80/100 | ✅         |
| free-water-test                | ✅      | 82/100 | ✅         |

22 pages total (excludes `thank-you` and the QDP-gated `[serviceArea]`
dynamic route — see PROVISION.md Step 5c). 20/20 EAV-scored pages are
ship-ready (average 84/100); about/contact carry no EAV brief so
`score-built-site` doesn't score them (see PROVISION.md and PAGE_MAP in
`score-built-site.js`) — both were still written from `site.config.ts`
identity fields per PROVISION.md's instruction, with no invented facts.
✅ = done | 🔄 = in progress | ⏳ = not started | ❌ = blocked

## Quality gate (last run: 2026-09-25)
Score threshold: 80/100 — **20/20 scored pages ship-ready, average 84/100**
Run: cd C:\Users\lenevo\Local-SEO-Toolkit
     npm run score-built-site -- --business albuquerquewatersoftener --dist C:\Users\lenevo\waterSoftenerProjects\albuquerquewatersoftener\dist
Full report: Local-SEO-Toolkit\data\albuquerquewatersoftener\quality-report-2026-09-25.json

## Current task
Content pass complete as of 2026-09-25 (Steps 5, 5b, 6, 6b all done — see
checklist below and the dated note in Notes for full detail). All 22 pages
written, build is clean (0 errors/0 warnings, 23 pages), and all 20
EAV-scored pages are ship-ready at 80+ (average 84/100). GitHub repo still
not created — `gh` CLI is not installed in this environment (see Notes).
Next actions: either install/auth `gh` or create the GitHub repo manually
via github.com, then proceed to Step 7 (deploy to Vercel).

## Local data
- Neighbourhoods:  Nob Hill, North Valley, Sandia Heights, Four Hills, Taylor Ranch
- ZIP codes:       87106, 87107, 87111, 87120, 87123
- County:          Bernalillo County
- Population:      557,161 (2024 Census estimate)

## SpringWell affiliate links
- /follow/softener/ — salt-based softener (wired into homepage + comparison)
- /follow/combo/    — softener + filtration combo
- /follow/ro/       — reverse osmosis system

## Provisioning checklist
Mirrors PROVISION.md step-for-step, in the same order — check PROVISION.md
itself if a step here needs more detail than fits on one line.

- [ ] Step 1 — GitHub repo created (`gh repo create`) — blocked: `gh` CLI not installed in this environment
- [x] Step 2 — Boilerplate copied into the repo + `npm install`
- [x] Step 3 — `src/site.config.ts` filled in with real city data
- [ ] Step 4 — ~~Keystatic~~ REMOVED — no CMS step, see PROVISION.md "CMS — No Keystatic"
- [x] Step 5 — Content written for all 22 pages (see Page status table above)
- [x] Step 5b — GPGSlider wired into water-quality.astro, GPGSliderMini into comparison.astro, SystemTour into installation.astro
- [x] Step 6 — `npm run build` — 0 errors, 0 warnings confirmed (23 pages built)
- [x] Step 6b — All 20 EAV-scored pages scored 80+ via the quality gate (average 84/100)
- [ ] Step 7 — Deployed to Vercel (static output, no environment variables needed)
- [ ] Step 8 — Custom domain added (Vercel dashboard + Namecheap DNS)
- [ ] Step 9 — Google Search Console property added, sitemap submitted
- [ ] Step 10 — Citations submitted (Google Business Profile, Yelp, BBB, Angi, HomeAdvisor, Bing Places, Apple Maps, Foursquare, Manta, Hotfrog)

## Notes
_Add any city-specific notes, open data gaps, or decisions made here._

- **2026-09-25 — all 22 pages written, built, and scored (Steps 5/5b/6/6b
  complete).** Wrote real Albuquerque-specific content for every page,
  modeled structurally on the Indianapolis site's proven section order,
  heading patterns, and closing-sentence style (never copied its prose —
  every factual claim here traces to `site.config.ts` or the EAV briefs in
  `Local-SEO-Toolkit\data\albuquerquewatersoftener\briefs\`). Every
  business-operational fact the briefs flagged `[NEEDS DATA: ...]` — install
  duration, warranty terms, pricing, financing, permits, maintenance
  frequency, sizing guidance, trial period — was written as
  `[PLACEHOLDER — confirm <what's missing>]` rather than invented; **38
  placeholders** remain across the 22 pages for a future tenant to fill.
  Added a new shared `src/components/QuickFacts.astro` (imported on every
  EAV-scored inner page except `comparison.astro`, whose brief explicitly
  forbids city-specific demographic data on that page) that weaves all 7 of
  the brief's real, non-placeholder EAV values — GPG range, water source,
  water authority, population, county, and the *full* ZIP/neighbourhood
  lists — into one paragraph, so Rule 14 (EAV triples woven naturally)
  passes reliably; the homepage gets the same 7 values inline instead since
  it doesn't use `PageHero`/`QuickFacts`. Wired `GPGSlider.astro` into
  `water-quality.astro`, `GPGSliderMini.astro` into `comparison.astro`, and
  `SystemTour.astro` into `installation.astro` per Step 5b. `npm run build`
  is clean: 0 errors, 0 warnings, 0 hints, 23 pages. Registered the site in
  Local-SEO-Toolkit (`node scripts/validate-content.js --register`) so
  `score-built-site` could run — it wasn't in `config/businesses.json` yet.

  **Quality gate: 20/20 EAV-scored pages ship-ready, average 84/100** (see
  `Local-SEO-Toolkit\data\albuquerquewatersoftener\quality-report-2026-09-25.json`).
  First pass scored 63/100 average, 2/20 ship-ready; reached 84/100 average,
  20/20 ship-ready after several iteration rounds fixing, in rough order of
  impact: (1) the brand name "Water Softeners of {city}" itself matches the
  Rule 5/7 plural-service-noun trigger ("Softeners") on every page, so every
  page's opening sentence needed a "such as ..." example within 2 sentences;
  (2) `QuickFacts.astro` originally used `.slice(0, 3)` for ZIP codes and
  neighbourhoods, but Rule 14 requires the brief's *complete* comma-joined
  value verbatim, not a partial list — switched to `.join(", ")` on the full
  arrays; (3) several pages opened authority sentences with capitalized
  "Per {waterAuthority}" — Rule 21/24/39's authority-signal regex requires
  lowercase `per` (no `i` flag) or matches `according to` case-insensitively,
  so capitalized sentence-initial "Per X" silently failed the check even
  though it reads identically to a person — switched to "According to X"
  everywhere; (4) list intros ending in a bare colon (no trailing period)
  fail Rule 9's first-40-words-need-a-period check even when they pass Rule
  26's own colon-based list-intro check — needed a short period-ended
  sentence *before* the colon-ended one; (5) the naive `/ing$/` list-item
  heuristic behind Rule 8 flags non-verb words that merely end in "-ing"
  ("Everything", "Rising"), and a sentence-initial capitalized breadcrumb
  label starting with a listed verb word ("Compare", "Sizing") gets merged
  with the badge row into one pseudo-sentence — both needed rewording, not
  the actual list content; (6) a lead-in `<p>` sitting before a section's
  own `<h2>` (rather than after it) gets counted as the *end* of the
  *preceding* `<h2>`'s body by the section splitter — this is the same
  "eyebrow" gotcha PROVISION.md Step 6c documents, generalized to any
  orphan paragraph, and repeatedly misattributed authority/forward-pointer
  sentences to the wrong heading (often `QuickFacts`) until each orphan
  paragraph got its own closing authority+forward-pointer sentence too.
  **Two pages needed real back-and-forth to clear 80** (both eventually
  passed): `reverse-osmosis` (final: 80/100) and `control-head-repair`
  (final: 80/100) — both carry the standard SpringWell/affiliate-adjacent
  content and FAQ-question phrasing that trip the *accepted* Rule 2/6/12
  false positives PROVISION.md Step 6c calls out (the affiliate disclosure
  sentence, and FAQ `<summary>` questions) — those specific failures were
  left as-is rather than reworded, and the remaining points were found
  elsewhere (numeric density, list intros, orphan-paragraph authority
  signals) to clear the threshold without touching the accepted exceptions.
  Also left as accepted, permanent deductions on the pages that carry them:
  the affiliate disclosure sentence ("We may earn a commission ... if you
  purchase through them") on `comparison`, `products`, `whole-home-filtration`,
  and `reverse-osmosis`; FAQ `<summary>` questions read as static/passive by
  Rules 6/15/20 on several pages; and breadcrumb anchor text (Rule 13/27)
  on `resin-bed-replacement` and `brine-tank-cleaning`, whose "Repair"
  crumb doesn't match the destination page's full SEO title — per
  PROVISION.md Step 6c, forcing full-title breadcrumb labels would degrade
  navigation UX, so this project accepts the deduction instead. Out of
  scope for this pass, per the task brief: the `AlbuquerqueMap.astro`
  neighbourhood Leaflet map (needs verified GPS pins), `Testimonials.astro`,
  `InstallationProcess.astro`, and real header photography — every page
  correctly falls back to the `PageHero` GPG stat-card and the homepage's
  `placehold.co` hero image, matching how every other unfinished site in
  this portfolio currently looks.

- **2026-09-25 — site provisioning started.** Copied boilerplate to
  `waterSoftenerProjects/albuquerquewatersoftener` and filled `site.config.ts`
  with verified data: GPG range (6-10, "Moderately Hard to Hard") and water
  source sourced from ABCWUA's own drinking-water FAQ page (abcwua.org),
  which states hardness "will range from moderately hard to hard" and that
  groundwater and San Juan-Chama surface water have been blended since
  December 2008 — third-party estimates (HardWaterHQ, WaterHardness.org,
  TapWater.org) independently cluster in the same 6-10 GPG band, so this
  range was used in place of a single point figure ABCWUA doesn't publish.
  Population is the 2024 Census estimate (557,161). Neighbourhoods and ZIPs
  cross-checked against real-estate/neighborhood-guide sources and ZIP
  boundary maps: Nob Hill 87106, North Valley 87107, Sandia Heights 87111,
  Four Hills 87123, Taylor Ranch 87120 — note Taylor Ranch is NOT 87124
  (that ZIP belongs to Rio Rancho, a separate incorporated city, which
  matters if Rio Rancho is ever evaluated as a QDP service-area candidate).
  `searchVol` left at 0 — no keyword-tool access from this build, same open
  gap as every other site in this portfolio. `phoneNumber`/`businessEmail`
  left as placeholders pending a tenant, per the established pattern.
  **Blocker:** GitHub CLI (`gh`) is not installed in this Claude Code
  environment, so Step 1 (`gh repo create`) could not run. Either install
  `gh` and run `gh auth login`, or create the repo manually at
  github.com/assignmenthelptalk and provide the clone URL so `git remote
  add origin` can be run against the local repo once initialized.

- **2026-09-24 — all 21 inner pages migrated to `PageHero.astro`.**
  `PageHero.astro` existed in the boilerplate from an earlier pass but was
  never wired into any page — every inner page still used the old
  single-column `.page-header` section plus a separate
  `.page-header-image-section` pointing at a `placehold.co` placeholder
  image. This pass replaced that pattern on all 21 inner pages with
  `<PageHero breadcrumbs={...} heading={...} primaryCta={...}
  secondaryCta={...}>`, moved each page's existing opening paragraph
  (Glendale Elite "Brand OFFERS" pattern) into the hero via a named
  `opening` slot, and dropped the `subheading` prop entirely (removed
  from `PageHero.astro` and every call site) so hero content now runs H1
  straight into the opening paragraph. No `image` prop is passed on any
  page, since the boilerplate has no real photography — every hero
  renders the GPG stat-card fallback; a per-city task when provisioning
  is to generate real header photos and pass them via `image`, same as
  the Tampa site did. `.brand-link` inside the hero is styled white with
  a permanent underline (not the default blue/no-underline used
  elsewhere) since the hero has a dark gradient background. Six pages
  (control-head-repair, free-water-test, new-construction-installation,
  salt-based-installation, salt-free-installation, water-softener-sizing)
  had their opening paragraph further down the page body rather than
  immediately after the header — caught and fixed a duplication bug
  where the first migration pass copied that text into the hero slot but
  left the original paragraph in place; both copies are now correctly
  merged into one. Also fixed an orphaned empty `<div class="container">`
  left behind in `quote.astro` by the migration (`quote.astro` has two
  sibling `.container` divs inside its second section — one for the
  moved paragraph, since removed, and one for the `.quote-grid` form
  layout). `npm run build` confirms 0 errors/0 warnings/0 hints, 23
  pages. The homepage was **not** touched in this pass — it still uses
  the older layout (opening paragraph in a separate section below the
  hero, not inside it); Tampa's homepage was restructured to move its
  opening paragraph into the hero itself, but syncing that specific
  change to the boilerplate homepage was not part of this pass.

- **2026-09-23 — boilerplate expanded from 16 to 22 fixed pages.** Ported
  6 pages from the Minneapolis site build after validating they contain no
  hardcoded city data: `salt-based-installation`, `salt-free-installation`,
  `water-softener-sizing`, `new-construction-installation` (linked from
  `installation.astro`'s new "Installation Options" section),
  `control-head-repair` (linked from `repair/index.astro`), and
  `free-water-test` (linked from `water-quality.astro`). None are in the
  main nav or footer, matching the existing `brine-tank-cleaning`
  precedent — reachable via contextual links + sitemap only. `npm run
  build` confirmed 0 errors, 0 warnings, 23 pages (22 content + thank-you).
  `Layout.astro` was intentionally left untouched (Minneapolis's copy has
  since diverged with a per-city Leaflet map link and `site.businessName`
  usage that are out of scope for this pass — a separate task if this
  boilerplate should pick those up too). This is the fixed-page half of
  the portfolio's Core 30 target; see PROVISION.md Step 5c for the
  QDP-gated service-area pages that make up the rest, and the
  `local-gbp-core30` skill in Local-SEO-Toolkit for the planning workflow
  behind the 30 figure.
