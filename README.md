# datasailsolutions.github.io

GitHub Pages repo for **Datasail Solutions** (Data Sail Solutions LLC).

## What this repo serves

- `main` → https://datasailsolutions.github.io/ — a single static page (`index.html`)
  describing Datasail Solutions and its optional SMS reminder messaging, with a link to
  the SMS consent policy at `/sms-consent/`. Keep it online: the SMS opt-in/consent wording
  can be referenced by messaging-provider compliance reviews.
- `static-pages` branch — holds `app-ads.txt`.

## What this repo does *not* serve

The main marketing site, **https://datasailsolutions.com**, ("AI-first business technology
consulting": home, Services, Example Projects, About, Contact) is **not** built from this
repo. As of 2026-10-21 it is served directly by nginx on a separate host (no CNAME here,
no GitHub Pages build). Edits to datasailsolutions.com copy need to be made in that site's
source and deployed to that server.

## Editing

Plain HTML with inline CSS, no build step. Edit `index.html`, open it in a browser to check,
and push to `main`; GitHub Pages republishes automatically.
