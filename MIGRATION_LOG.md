# Migration Log

## Current State
- Hugo site is running on the `blowfish` theme.
- Theme is configured via `config/_default/hugo.toml` and `config/_default/params.toml`.
- The previous phantom `blowfish` language configuration was removed by deleting `config/_default/hugo.blowfish.toml`.
- Single-page rendering was fixed by aligning the local `layouts/_default/single.html` override with Blowfish's expected block structure.
- Page-level metadata has been added for homepage, research, CV, and teaching.
- Header and head customisations now use Blowfish's active extension points (`layouts/partials/header/basic.html` and `layouts/partials/extend-head.html`) rather than stale legacy hooks.
- Public-facing email actions on the homepage, research page, and CV page now avoid exposing the raw address in initial HTML while preserving click-to-email behaviour.
- Favicon restored via `layouts/partials/favicons.html` (Blowfish-native hook); the previous implementation was in a LoveIt-era partial that was removed during cleanup.
- Mobile layout hardened: research and teaching grids use `minmax(min(320px, 100%), 1fr)` to prevent overflow on narrow viewports; 480px heading breakpoint added.
- Featured research card now links to a real draft PDF (`static/pdfs/fornaro_2026_financial.pdf`) and includes a collapsible abstract using native HTML `<details>`.
- Netlify deployment configured via `netlify.toml` pinning Hugo version.

## Ticket Status
- `01 Homepage Hero` — Completed
- `02 Featured Research Module` — Completed
- `03 Research Grid` — Partial
- `04 CV Page` — Completed
- `05 Nav Microinteractions` — Completed
- `06 SEO and OG Images` — Completed
- `07 Research Credibility Pass` — Partial
- `08 Teaching Simplification Pass` — Completed
- `09 Cross-Page Consistency Pass` — Completed

Status convention:
- `Not Started` = no meaningful implementation yet
- `In Progress` = actively being worked on
- `Partial` = some acceptance criteria satisfied, but not all
- `Completed` = acceptance criteria satisfied
- `Deferred` = intentionally postponed
- `Dropped` = intentionally not being taken forward in current form

## Status Notes
- `02 Featured Research Module` is complete: real draft PDF linked, collapsible abstract added, description and copy finalised.
- `03 Research Grid` is visually established, but research metadata can still be strengthened once coauthors, dates, and real outputs are confirmed.
- `04 CV Page` is complete; the page now restores contact through a subdued email action, keeps the PDF as the primary CTA, and uses a clearer chronology-first scan pattern in place of faux-logo marks.
- `07 Research Credibility Pass` removed dead research actions, improved academic phrasing, added confirmed coauthors and year for the featured paper, and now uses real imagery for the featured project and selected early-stage projects. It remains partial because final metadata and output links still depend on confirmed titles, coauthors, dates, and materials for the non-featured projects.
- `08 Teaching Simplification Pass` is complete; future work is limited to swapping placeholder states for real slide links as materials are uploaded.
- `09 Cross-Page Consistency Pass` is complete; remaining site work is primarily future content and materials rather than shared UI inconsistency.

## Confirmed Fixes
- Theme is set to `blowfish`.
- The extra `BLOWFISH` output site was removed; build output is now a single `EN` site.
- `Research`, `CV`, and `Teaching` content render correctly in generated HTML.
- Generic SEO descriptions were replaced with page-specific descriptions.
- Author metadata now resolves to `Will Hotten`.
- Footer theme credit can be disabled through current params.
- Homepage, Research, CV, and Teaching now point to explicit branded OG image assets.
- Main navigation is now sourced from `config/_default/menus.en.toml` rather than duplicated in `config/_default/hugo.toml`.
- Homepage, Research, CV, Teaching, and the shared header have all received local design refinements in `assets/css/custom.css` and page content files.
- Stale `customHead` configuration and unused legacy head partials were removed so local customisations now map cleanly to Blowfish's actual render path.
- Homepage, research, and CV contact actions now use delayed client-side mailto assembly so the deployed HTML no longer contains the raw email address.

## Current Warnings
- Hugo emits a version-compatibility warning for Blowfish:
  - `Module "blowfish" is not compatible with this Hugo version: 0.141.0/0.155.3 extended`
- This warning does not currently block successful builds.

## Current Design Decisions
- Homepage should be stage-independent and not centred on a job market paper.
- `Featured Research` is the neutral module name that can later become `Job Market Paper`.
- Type direction is:
  - `Fraunces` for headings
  - `Inter` for body
  - `IBM Plex Mono` for meta/UI accents
- Accent colour should remain restrained acid green.
- Portrait treatment should remain black and white and rectangular.
- Motion should stay minimal and CSS-led.
- Research/project thumbnails should use a shared wide crop and restrained greyscale treatment, with real photography used where available and abstract placeholders retained for genuinely early-stage work.

## Remaining Open Decisions
- Final portrait crop and treatment.
- Whether the footer should expose direct social/contact links inline or via icons only.
- Research cards for non-featured projects can be strengthened once final titles, coauthors, and output links are confirmed.
- Key figure for the featured paper (IRF or similar) to be added once a web-ready image is prepared.
- Slides links on the teaching page to be swapped from placeholder states to real uploaded files as materials are finalised.
- Teaching page slide links should be swapped from placeholder states to real uploaded files as materials are finalised.

## Build Command
- `hugo --gc --minify --cacheDir /tmp/hugo_cache`
