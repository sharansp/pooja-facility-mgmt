# Pooja Facility Management Services — website

Marketing website for Pooja Facility Management Services Pvt Ltd
(security, housekeeping, facility management — Pune, since 2008).

## Structure
- `index.html` — single-page site (all CSS/JS inline, no build step)
- `assets/` — logo, favicon and photos

## Running locally
Just open `index.html` in a browser. No build tools or server required.

## Contact form
The enquiry form on the Contact section submits to
[FormSubmit.co](https://formsubmit.co), which forwards submissions by email
with no backend or signup required. On the **first** real submission after
deploying, FormSubmit sends a one-time confirmation email to
`pooja.servises@gmail.com` — click the link in that email to activate delivery.
To change the destination email, edit `FORM_ENDPOINT` near the bottom of
`index.html`.

## Deploying with GitHub Pages
1. Push this folder to `main` on the GitHub repo.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source: Deploy from a branch**,
   branch **main**, folder **/ (root)**.
4. Save — the site will be live at `https://<username>.github.io/<repo>/`
   within a minute or two.
