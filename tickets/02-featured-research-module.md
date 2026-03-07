# Ticket 02: Featured Research Module

## Goal
Refine the `Featured Research` section into a stable, reusable module that can later be renamed to `Job Market Paper` without structural change.

## Scope
- Homepage featured research module.
- Content and layout only for that component.

## Acceptance Criteria
- Module label is `Featured Research`.
- Includes:
  - paper title
  - concise contribution summary
  - status tag
  - slots for PDF, slides, and code actions
- Layout remains visually prominent but not promotional.
- The module can be renamed later without requiring new markup.

## Constraints
- Do not hard-code job-market-specific language.
- Keep buttons and metadata consistent with the broader design system.
- Avoid over-branding the current academic stage.
