---
title: "Turning a static webpage into an Astro-powered site"
description: "How RRM moved from a single static webpage to an Astro site with Markdown-powered blog content."
publishDate: 2026-07-19
author: "Snnr Limited"
tags:
  - astro
  - website
  - product
---

RRM started with the simplest possible web presence: a static page that explained the product direction and gave the project a place to live online. That was enough for an early version, but it was not a great foundation for sharing product updates, compliance notes, release progress, or longer explanations about where Restaurant Regulation Management is heading.

Moving the website to Astro gives us a cleaner structure without making the site heavier than it needs to be. Pages can stay fast and mostly static, while the codebase now has reusable layouts, shared navigation, and a dedicated content collection for blog posts.

The most important change is that blog content now lives in Markdown. Instead of editing page markup every time we want to publish something new, a post can be added by creating a file in `src/content/blog/` with a title, description, publish date, author, and tags.

That gives the RRM website a practical path from a one-page placeholder to a content-driven product site. The first version can still be simple, but it is now ready for:

- product updates as the platform evolves;
- compliance explainers for restaurants moving away from paper-based workflows;
- roadmap notes about dashboards, daily records, IoT integrations, and AI-assisted processes;
- release notes that are easy to write, review, and publish.

Astro is a good fit for this stage because it keeps the site lightweight while giving the project room to grow. The website can remain fast and static where that makes sense, but the content model is now flexible enough to support regular updates as RRM develops.
