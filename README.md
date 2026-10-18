# gavz app website

A static site for gavz Mac apps, hosted with GitHub Pages. Plain HTML and one shared CSS file; no JavaScript, dependencies, analytics or external fonts.

## Local preview

```sh
python3 -m http.server 8080 --directory .
```

Open http://localhost:8080/. Directory URLs resolve to `index.html`, including:

- `/orbit/`, `/orbit/support/`, and the existing `/orbit/privacy.html`.
- `/blackbox-audio/`, `/blackbox-audio/support/`, `/blackbox-audio/privacy/`.
- `/fidget-desktops/snowfall/`, `/fidget-desktops/snowfall/help/`, `/fidget-desktops/snowfall/support/`, `/fidget-desktops/snowfall/privacy/`.
- `/privacy/` for the website and app privacy overview.

`assets/site.css` controls spacing, typography, light/dark appearance and mobile layouts. Icons are copies of the apps’ existing artwork. Their source repositories remain unchanged.

## Release updates

BlackBox is currently marked “Coming to the Mac App Store”, with a US$4.99 launch price. When it is available, add its App Store link to the home and product pages. Orbit already links to its current App Store entry.

The listing uses `https://gavz.app/blackbox-audio` and its `/support` and `/privacy` paths. After reviewing and publishing, check those public URLs and HTTPS. GitHub Pages should serve the repository root; configure the `gavz.app` custom domain and DNS in the hosting settings if not already configured.

Copyright footers currently use 2026. Support email remains `support@gavz.app`.

## Snowfall release preparation

Snowfall is marked coming soon, at US$2.99 for a one-time purchase with no IAP or subscription. App Store app ID: `6824011223`; add the public store link only after it is released. The approved larger-snowflake icon is included on the product page as `assets/snowfall.png`, exported from Icon Composer. Five screenshots/one preview will be added after release testing and media approval; the current pages have no placeholder screenshots/videos.

The product, support and privacy URLs used in App Store Connect are under `/fidget-desktops/snowfall`. The pages document main-display support, snowball gestures, reset, local screen processing and permission denial/revocation. Reconfirm privacy/feature statements against the final shipping build before release.

Gavin will review, commit and push these changes. Allow approximately ten minutes for GitHub Pages deployment, then verify all three public URLs, HTTPS and content. Local preview alone does not confirm publication.

The 18 October 2026 product-copy revision leads with interactive snow, buildable snowmen and the robin’s personality. Settings remain documented in Help and support; the product page keeps customisation secondary. The experience-focused revision is prepared locally and needs a commit/push followed by live verification.

### Snowfall Help

The app’s Help menu opens `https://gavz.app/fidget-desktops/snowfall/help/`. This guide covers settings, brushing, snowballs/snowmen, robin behaviour, permissions, reset and troubleshooting. Linked from the product and support pages. The Help page and product/support links were verified live over HTTPS on 17 October 2026. The approved-icon addition and the 18 October 2026 settings-copy refresh were committed in `a2d52b3`. Help/support cover Robin visits, Clear spells, Animation smoothness, Settings access via the Dock and Command-Tab while open, and current mouse gestures. The later experience-focused product revision above still needs a commit/push and live verification.

- [ ] After final screenshots and videos are approved, add relevant images and short gesture demonstrations to Help and the product page, using the actual release behaviour. Preserve the readable text guide alongside media.
