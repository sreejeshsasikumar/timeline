# Chestertons · Website Redesign Dashboard

Executive dashboard tracking the website redesign decision, vendor quotes, financials, timeline, and project status. Built as a single self-contained HTML page with no build step required.

**Live preview:** open `index.html` in any modern browser, or enable GitHub Pages on this repo.

## What's inside

- `index.html` — the dashboard (single file, ~4,000 lines, embeds all CSS and JS)
- `quotes/` — original vendor proposal PDFs from DevSpace, Digital Gravity, PIXL, and StarBerry

## Sections

1. **Decision** — build in-house vs outsource, with full TCO comparison
2. **Vendors** — four vendor cards with linked PDF quotes
3. **Audit** — strengths and red flags per vendor with verdict pills
4. **Quotes** — the full quote library with downloadable PDFs
5. **Financials** — three-tab cost view: Design Only, Design + Dev, Compare
6. **Timeline** — Gantt + milestone roadmap with calendar dates
7. **Team · Status · Risk · Deliverables** — internal capability and live status

## Authentication

Edit access on the timeline is gated by client-side auth (demo only).

| Username | Password         |
|----------|------------------|
| admin    | chestertons2026  |
| sree     | digital-lead     |

> ⚠ Demo credentials only. Replace before production. Hard-coded in `index.html`.

Edits and auth state persist via `localStorage`. For multi-user editing, wire a backend (Supabase + Vercel serverless function recommended).

## Tech stack

- Vanilla HTML, CSS, JavaScript (no build step)
- Chart.js loaded via CDN for the TCO chart
- Google Fonts: Inter + Playfair Display

## Hosting

The dashboard works as a static site. Recommended hosting:

- **GitHub Pages** — Settings → Pages → deploy from `main` branch root
- **Vercel** — `vercel deploy` from project root
- **Netlify** — drag the folder onto the dashboard

## License

Internal use only. Not for redistribution.

---

Built by the Chestertons Digital & Technology team.
