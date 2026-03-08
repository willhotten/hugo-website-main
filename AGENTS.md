# Hugo website (Blowfish migration)

## Read First
- Read `DESIGN_BRIEF.md` before making design decisions.
- Read `MIGRATION_LOG.md` before touching config, layouts, or theme integration.
- Read the relevant file in `tickets/` before implementing the next step.

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

## Ticket tracking
- Every ticket in `tickets/` should include a `## Status` section.
- Allowed statuses are:
  - `Not Started`
  - `In Progress`
  - `Partial`
  - `Completed`
  - `Deferred`
  - `Dropped`
- `MIGRATION_LOG.md` must maintain a matching ticket status summary.
- If work only partially satisfies a ticket, update the ticket and `MIGRATION_LOG.md` with what remains.
- If we decide not to complete part of a ticket, record that explicitly in `MIGRATION_LOG.md` under status notes or open decisions rather than leaving it implicit.
- When starting a new ticket, set it to `In Progress`.
- When stopping with unresolved scope, do not mark `Completed`; use `Partial`, `Deferred`, or `Dropped` as appropriate.
