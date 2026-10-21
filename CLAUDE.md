# CLAUDE.md

Notes for Claude Code when working in this repo.

## Project

- Repo: `datasailsolutions/datasailsolutions.github.io` (datasailsolutions business GitHub account).
  Work in this existing repo; never create a new one.
- `main` publishes https://datasailsolutions.github.io/ via GitHub Pages: one hand-written
  `index.html` (inline `<style>`, no JS, no build step). It covers the SMS reminder service
  and links to `/sms-consent/`. Don't remove or reword the SMS consent/opt-out language
  without being asked.
- `static-pages` branch: `app-ads.txt` only.

## datasailsolutions.com is a different site

The live consulting site at datasailsolutions.com is **not** in this repo. It's served by
nginx on its own host (checked 2026-10-21: no CNAME here, different HTML). Its pages
(`index.html`, `services.html`, `projects.html`, `about.html`, `contact.html`,
`css/styles.css`, `js/main.js`, `assets/`) use a card/section design:

- Homepage "Core services": `<article class="service-card">` with `<div class="card-icon">NN</div>`,
  `<h3>`, one short `<p>` (~15–25 words). `.card-grid` is a fixed 4-column grid on desktop.
- Services page: `<article class="detail-row">` with a `section-kicker` number, `<h2>`, one
  `<p>`, and four `<li>` bullets.
- Voice: plain, practical, "AI-first, grounded in business outcomes", no hype.

If asked to change datasailsolutions.com copy, say that the source isn't here, prepare the edit
against the live HTML, and give the user a patch to apply on the real source or server.

## Verifying changes

No build step. Check that the HTML is well-formed (balanced tags) and open it in a browser.
Keep design, layout, and typography unchanged unless asked.
