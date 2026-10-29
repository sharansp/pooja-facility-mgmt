# Project Rules — Pooja Facility Management Services

## Current phase
Phase 1 — Public marketing website (plain HTML/CSS/JS, no build step).

## Architecture decision (recorded)
- **Now:** Multi-page static HTML site (6 pages). No framework, no build tools.
- **Future:** Migrate to React + Vite + React Router when dashboard modules are needed.
  The public site pages will become React components at that point.
  Backend will be a separate service (Node.js/Express or similar) with a proper database.
  Authentication, payroll, staff records, and admin dashboard are future phases only.

## Do not
- Invent business statistics, awards, certifications, testimonials, or client names not already in the codebase.
- Add placeholder links that look functional but go nowhere.
- Build any login, dashboard, or database functionality in this phase.
- Store staff or customer records in browser storage.

## Content that requires company confirmation before publishing
- Social media profile URLs (currently `#` placeholders).
- Website domain (currently listed as `www.poojafacility.com` — confirm before go-live).
- Any new client names beyond those already listed.
- Business hours.

## Shared across all pages
- Header and footer HTML must be identical on every page.
- All internal links use relative paths (e.g. `services.html`, `../assets/logo-icon.png`).
- Active nav link gets `aria-current="page"` and a visual underline.
- FormSubmit endpoint: `pooja.servises@gmail.com` — do not change without instruction.
