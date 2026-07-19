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

An Astro static site deployed to GitHub Pages:

- `src/pages/index.astro` — landing page.
- `src/layouts/BaseLayout.astro` — shared page shell, metadata, navigation, and footer.
- `src/styles/global.css` — global styling (uses the Nunito Sans web font).
- `src/content/blog/` — Markdown blog posts managed by Astro content collections.
- `src/pages/blog/` — blog listing and individual post routes.

## Local development

```bash
# from the repo root
npm install
npm run dev
```

Astro will print the local preview URL, usually `http://localhost:4321`.

## Markdown blog posts

Add new blog posts as Markdown files in `src/content/blog/`. Each post needs
frontmatter like:

```md
---
title: "Post title"
description: "Short summary for listings and metadata."
publishDate: 2026-07-19
author: "Snnr Limited"
tags:
  - product
slug: post-url-slug
---

Write the post body in Markdown.
```

Draft posts can be hidden from the build with `draft: true`.

## Build and deploy

```bash
npm run build
```

The GitHub Actions workflow builds Astro and uploads `dist/` to GitHub Pages.
The Astro config uses root-relative URLs so the site runs from the domain root
rather than a `/rrm-website/` subpath. The custom domain is pinned by
`public/CNAME`.
