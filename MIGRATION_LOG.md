# Migration Log

## Current State
- Hugo site is running on the `blowfish` theme.
- Theme is configured via `config/_default/hugo.toml` and `config/_default/params.toml`.
- The previous phantom `blowfish` language configuration was removed by deleting `config/_default/hugo.blowfish.toml`.
- Single-page rendering was fixed by aligning the local `layouts/_default/single.html` override with Blowfish's expected block structure.
- Page-level metadata has been added for homepage, research, CV, and teaching.

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

## Remaining Open Decisions
- Final portrait crop and treatment.
- Final visual system for research thumbnails.
- Whether the featured research module should eventually expose PDF, slides, and code as real links or placeholder states.
- Whether the footer should expose direct social/contact links inline or via icons only.
- Research page content will likely need a later content pass once paper titles, abstracts, coauthors, and output links are final.
- Research cards should add coauthor lines only when confirmed, rather than carrying placeholders.
- Featured research links should be upgraded from placeholder states to real paper/slides links once those outputs exist.
- Teaching page slide links should be swapped from placeholder states to real uploaded files as materials are finalised.

## Build Command
- `hugo --gc --minify --cacheDir /tmp/hugo_cache`
