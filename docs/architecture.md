# Architecture

## Current phase — Static multi-page HTML site

```
/
  index.html          ← Home page
  services.html       ← Services page
  about.html          ← About Us page
  industries.html     ← Industries We Serve page
  contact.html        ← Contact Us page
  faq.html            ← FAQ page
  assets/             ← Images, logos, favicon
  robots.txt
  sitemap.xml
  docs/               ← Project documentation
  .amazonq/rules/     ← Development guidelines
```

- Zero dependencies. Open any `.html` file in a browser — it works.
- CSS and JS are inline per page (keeps the zero-build-step approach).
- Form submissions go to FormSubmit.co via `fetch` — no backend required.
- Hosted on GitHub Pages from the `main` branch root.

## Future phase — Full-stack application (when dashboard modules are needed)

When staff management, payroll, attendance, or customer portals are required, the project
will be migrated to a proper stack. The public website pages become the starting point.

### Recommended future stack
```
frontend/               ← React + Vite + React Router + TypeScript
  src/
    pages/              ← Public site pages (converted from HTML)
    components/
    layouts/
    data/
  public/

backend/                ← Node.js + Express (or NestJS)
  src/
    routes/
    controllers/
    services/
    middleware/         ← Auth (JWT), rate limiting, validation

database/               ← PostgreSQL (via Supabase or RDS)
  migrations/
  seeds/
```

### Future modules (do not build now)
- Admin dashboard
- Staff database and portal
- Attendance and shift management
- Salary and payroll
- Customer and property management
- Work orders and maintenance tickets
- Asset management
- Reports and notifications

### Security principles for future backend
- JWT authentication with refresh tokens
- Role-based access control (admin, manager, staff, client)
- All secrets in environment variables — never in frontend code
- HTTPS only, CORS restricted to known origins
- Input validation and parameterised queries (no SQL injection)
- Audit logs for sensitive operations (payroll, staff records)
