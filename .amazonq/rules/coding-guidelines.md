# Coding Guidelines

## Stack
Plain HTML5 + CSS3 + vanilla JS. No frameworks, no build tools, no npm.

## File structure
```
/
  index.html          ← Home
  services.html
  about.html
  industries.html
  contact.html
  faq.html
  assets/             ← images, logo, favicon
  shared/
    header.html       ← reference only (not server-side includes; copy into each page)
  robots.txt
  sitemap.xml
  docs/
  .amazonq/
```

## HTML rules
- `<!DOCTYPE html>`, `lang="en"` on every page
- Unique `<title>` and `<meta name="description">` per page
- Semantic elements: `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, `<article>`
- Correct heading hierarchy: one `<h1>` per page
- All images: meaningful `alt` text, `loading="lazy"` except above-the-fold
- Active nav link: `aria-current="page"`

## CSS rules
- All CSS inline in `<style>` in each page's `<head>` (keeps zero-dependency approach)
- CSS custom properties (variables) defined in `:root` — same set on every page
- Mobile-first media queries at `980px` and `640px`
- No external CSS frameworks

## JS rules
- All JS inline in `<script>` before `</body>`
- No external JS libraries
- Use `IntersectionObserver` for scroll reveal and counter animation
- Form submission via `fetch` to FormSubmit.co endpoint
- No secrets, API keys, or credentials in any frontend file

## Naming
- Files: lowercase, hyphenated (`services.html`, `hero-guards.jpg`)
- CSS classes: lowercase, hyphenated (`.service-card`, `.section-head`)
- IDs: camelCase (`siteHeader`, `quoteForm`)

## Quality checks before committing
- Open each page in browser, check console for errors
- Test mobile layout at 375px width
- Test all internal links
- Validate contact form: required fields, success state, error state
- Check no horizontal scroll on any viewport
