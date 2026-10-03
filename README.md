# gavz app website

A static site for gavz Mac apps, hosted with GitHub Pages. Plain HTML and one shared CSS file; no JavaScript, dependencies, analytics or external fonts.

## Local preview

```sh
python3 -m http.server 8080 --directory .
```

Open http://localhost:8080/. Directory URLs resolve to `index.html`, including:

- `/orbit/`, `/orbit/support/`, and the existing `/orbit/privacy.html`.
- `/blackbox-audio/`, `/blackbox-audio/support/`, `/blackbox-audio/privacy/`.
- `/privacy/` for the website and app privacy overview.

`assets/site.css` controls spacing, typography, light/dark appearance and mobile layouts. Icons are copies of the apps’ existing artwork. Their source repositories remain unchanged.

## Release updates

BlackBox is currently marked “Coming to the Mac App Store”, with a US$4.99 launch price. When it is available, add its App Store link to the home and product pages. Orbit already links to its current App Store entry.

The listing uses `https://gavz.app/blackbox-audio` and its `/support` and `/privacy` paths. After reviewing and publishing, check those public URLs and HTTPS. GitHub Pages should serve the repository root; configure the `gavz.app` custom domain and DNS in the hosting settings if not already configured.

Copyright footers currently use 2026. Support email remains `support@gavz.app`.
