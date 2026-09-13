# Video Squisher — public site (GitHub Pages)

Static marketing/download page for **🎬 Video Squisher by KitKarl**.
Contains **no application source code** — the app itself is closed-source and
distributed as binaries from https://download.kitkarl.com

## Publishing

This repo is built to live at `github.com/<you>/videosquisher` so Pages
serves it at `https://<you>.github.io/videosquisher/`.

1. Create an empty **public** repo named exactly `videosquisher` on GitHub.
2. From this folder:

   ```
   git remote add origin https://github.com/<you>/videosquisher.git
   git push -u origin main
   ```

3. Repo → Settings → Pages → Source: **Deploy from a branch** → `main` / root.
4. Site is live at `https://<you>.github.io/videosquisher/` in a minute or two.

## Content sources (keep in sync)

- All copy comes from `PRODUCT_INFO_SHEET.md` in the main project (pitches,
  features, Free/Pro table, FAQ, do-not-say list).
- Brand colors and logo: app theme (teal `#2A9D8F` on cream/charcoal) and
  `assets/icon.png`.
- Screenshots: refresh from `flatpak/screenshots/` at release time.
- Honesty rules from the info sheet §8 apply here too: never say "lossless",
  never promise an average compression %.

## Third-party notice

The app bundles GPL-licensed FFmpeg; attribution ships inside every
installer. This page only links to the app and contains no GPL code.

## SEO decisions (do not casually undo)

- `index.html` carries `<link rel="canonical" href="https://www.kitkarl.com/squisher">`
  — deliberate: the GitHub page defers search-ranking credit to the official
  marketing page so the two don't compete. Remove only if this page becomes
  the primary site.
- `robots.txt` + `sitemap.xml` (single URL) live at the repo root; both use
  the absolute URL `https://kitkarl-git.github.io/videosquisher/` — update
  them if the site ever moves to a custom domain.
- Open Graph / Twitter tags make shares in Discord/Slack/WhatsApp/iMessage
  render a screenshot card; `og:image` is `screenshots/1-main-window.jpg`.

