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
