# Matthew Olson — Anthropic application

A single-page application site bringing together my résumé, cover letter, and "Why Anthropic" for the Forward Deployed Engineer role at Anthropic.

**Live page:** _(set your GitHub Pages URL once you've published — typically `https://<username>.github.io/<repo>/`)_

## What's here

```
.
├── index.html                  # the application page
├── 404.html                    # branded not-found page
├── og-image.png                # 1200×630 link-preview card
├── Matthew-Olson-Resume.pdf    # downloadable résumé, linked from the page
└── README.md
```

A single hand-crafted HTML file. No build step, no framework — just HTML, CSS, and a small amount of JavaScript for the interactive bits (smooth-scroll nav highlight, collapsible experience timeline, animated impact counters, reading-progress bar, keyboard navigation).

Designed in Anthropic's brand palette using Poppins (display) and Lora (body) loaded from Google Fonts.

## Deploying to GitHub Pages

1. Push this folder to a public GitHub repo.
2. In the repo's **Settings → Pages**, set the source to the `main` branch and `/ (root)`.
3. Your page goes live at `https://<username>.github.io/<repo-name>/`.

## After deploying — one small thing to update

The Open Graph / Twitter Card meta tags in `index.html` use a relative path for the link-preview image (`og-image.png`). Most modern social platforms (LinkedIn, Slack, Discord, iMessage) resolve this correctly. A few older crawlers don't.

If you want belt-and-suspenders, set those to absolute URLs once you know your final URL — find `og:image` and `twitter:image` in the `<head>` of `index.html` and change `og-image.png` to e.g. `https://yourname.github.io/yourrepo/og-image.png`.

You can test the link preview with [opengraph.xyz](https://www.opengraph.xyz/) once it's live.

## License

MIT — see `LICENSE`.
