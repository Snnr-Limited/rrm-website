# RRM Website

Marketing website for **RRM (Restaurant Regulation Management)** — a product by
[Snnr Limited](https://snnr.co) that helps restaurants go paperless with their
food safety and compliance workflows.

## What is this website for?

This is the public-facing landing page for RRM. Its job is to:

- Explain what RRM does — replacing paper-based Food Control Templates with
  digital forms that staff can complete from a phone, tablet, or browser.
- Show the two surfaces of the product:
  - A **web dashboard** for owners and auditors (compliance history, template
    management, one-click auditor exports, team management).
  - A **mobile app** for kitchen staff (daily checklists, offline support,
    automatic sync).
- Preview the upcoming roadmap features, clearly marked as *Coming Soon*:
  - **IoT sensor automation** for temperature and acidity logging.
  - **AI voice input** for hands-free form entry.
  - **Camera / visual capture** for deliveries and legacy paper forms.
- Drive sign-ups for the free trial and let visitors request a demo.

## Audience

- Restaurant owners and operators looking to digitise compliance.
- Food safety auditors who need audit-ready reports.
- Kitchen managers and staff who fill in daily Food Control Templates.

## Tech

A small, dependency-free static site:

- `src/index.html` — page markup and content.
- `src/styles.css` — styling (uses the Nunito Sans web font).

No build step is required. Open `src/index.html` in a browser, or serve the
`src/` directory with any static file server:

```bash
# from the repo root
cd src && python3 -m http.server 8000
# then visit http://localhost:8000
```
