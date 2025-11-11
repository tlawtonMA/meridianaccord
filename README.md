# Meridian Starter (GitHub + Cloudflare Pages)

Free Eleventy (11ty) starter for a nonprofit site.
- Custom HTML/CSS sections (paste directly into pages)
- Header: logo left; nav right (About, Research, Policy Areas, Engage)
- Add new pages by adding files in `src/`
- Cloudflare Pages-ready (build: `npm run build`; output: `_site`)
- CMS-ready (Decap CMS) — enable later by editing `admin/config.yml`

## Cloudflare Pages (private preview)
1) Create a **private** GitHub repo and upload the **contents** of this folder.
2) Cloudflare → Workers & Pages → Create application → Pages → Connect to Git.
3) Build settings:
   - Build command: `npm run build`
   - Output directory: `_site`
   - Framework preset: None
4) Deploy. Use the preview URL while private.

## Add Pages
Create a new file like `src/your-page.njk`:
```njk
---
layout: base.njk
title: Your Page
---
<h1>Your Page</h1>
<p>Paste your custom HTML here.</p>
```
