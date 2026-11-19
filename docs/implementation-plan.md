# Implementation Plan

## Phase 1 — Project setup and shared layout ✅ (current)
- Create all missing `docs/` and `.amazonq/rules/` documentation
- Audit existing `index.html` and record what to preserve
- Define shared header/footer HTML, CSS variables, and JS snippets
- Create `robots.txt` and `sitemap.xml`

## Phase 2 — Five new pages
Build each page using the shared layout from Phase 1:
1. `services.html` — full service cards with benefits and enquiry CTA
2. `about.html` — company story, mission/vision, values, full leadership section
3. `industries.html` — sector cards with descriptions and CTA
4. `contact.html` — full contact form + office details map placeholder
5. `faq.html` — accordion FAQ + CTA

## Phase 3 — Navigation wiring and cross-page links
- Update `index.html` nav links to point to the new pages
- Ensure active nav state (`aria-current="page"`) on each page
- Update footer links across all pages
- Test all internal links

## Phase 4 — SEO and performance
- Unique `<title>` and `<meta description>` on every page
- Open Graph tags for social sharing
- `robots.txt` and `sitemap.xml` with correct domain
- `loading="lazy"` on below-fold images
- Verify heading hierarchy on each page

## Phase 5 — QA and deployment
- Test all 6 pages at 375px, 768px, 1280px
- Test contact form (validation, success, error states)
- Check browser console — zero errors
- Verify GitHub Pages deployment
- Document how to update content

## Future phase — React migration (when dashboard is needed)
See `docs/architecture.md` for the recommended stack.
