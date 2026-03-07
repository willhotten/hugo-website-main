# Hugo website (Blowfish migration)

## Objective
Migrate this site to the Blowfish Hugo theme and improve design while keeping content accurate and changes reviewable.

## How to run
- Dev server: `hugo server -D --disableFastRender`
- Build: `hugo --gc --minify`

## Allowed edits
- `config/`, `content/`, `assets/`, `static/`, `layouts/` (only if necessary)

## Avoid / do not edit
- `themes/` (no direct edits; treat as vendored)
- `resources/_gen/`, `public/` (generated outputs)

## Definition of done for each ticket
- Build succeeds
- Changes are minimal & coherent
- Provide a short summary + list of files changed