# GCR Graphix — Marketing Website

Public landing page for the poster generation service. Lives in its own folder, separate from the admin portal in `src/`.

## What this site shows

- Personalized festival posters (Diwali, Holi, shop promos) with user name & photo
- WhatsApp → download → approve → Facebook post workflow
- Social page management for shop & business pages

## Local preview

Open `index.html` in a browser, or run a simple server:

```bash
cd marketing
python3 -m http.server 8080
```

Then visit http://localhost:8080

## Free hosting on GitHub Pages

This repo includes `.github/workflows/deploy-marketing.yml` which deploys the `marketing/` folder automatically.

### One-time setup

1. Push this repo to GitHub (if not already).
2. Go to **Settings → Pages** on your GitHub repo.
3. Under **Build and deployment → Source**, choose **GitHub Actions**.
4. Push to `main` — the workflow runs and publishes the site.

### Your live URL

After deploy, the site will be at:

```
https://vishal073.github.io/poster_generator_admin_portal/
```

(Replace `vishal073` and repo name if yours differ.)

### Custom domain (optional)

In **Settings → Pages**, add your domain (e.g. `gcrgraphix.com`) and point DNS to GitHub Pages.

## Before going live

1. **WhatsApp number** — In `index.html`, replace `919876543210` in the Contact link with your real business number.
2. **Email** — Update `hello@gcrgraphix.com` if needed.

## Folder structure

```
marketing/
├── index.html              # Landing page
├── favicon.png             # Browser tab icon (from logo)
├── images/
│   ├── logo.png            # GCR Graphix app icon (shown circular)
│   └── posters/            # Example poster images
│       ├── poster-1.jpg
│       ├── poster-2.jpg
│       └── poster-3.jpg
├── css/style.css
├── js/main.js
└── README.md
```

Replace files in `images/posters/` with your own example posters anytime.
