# Blackvault website

Static site (HTML, CSS, JS). No build step.

## Before launch
Domain and email addresses are set to blackvault.co.ke (see `assets/main.js`). Create or forward the five mailboxes before launch.

## Deploy: GitHub + Cloudflare Pages
1. Create a GitHub repository and upload everything in this folder.
2. Cloudflare dashboard > Workers & Pages > Create > Pages > Connect to Git > select the repository.
3. Framework preset: None. Build command: leave empty. Output directory: `/`.
4. Deploy. Then Custom domains > Set up a custom domain.

`_headers` adds security headers on Cloudflare Pages.

## Launch checklist
- Optional direct form delivery: paste a Formspree URL into `FORM_ENDPOINT` in `assets/main.js`.
- Add a new venture: copy `_venture-template.html`, edit it, link it from `index.html`, add it to `sitemap.xml`.
- Cloudflare: turn on Web Analytics and "Always Use HTTPS".
- Add registration number, registered address, directors and licences only once confirmed, and have a lawyer review the text.

## Pages
- `index.html` Home (hero, about, featured Agri Ventures, ventures, mission and vision, philosophy, insights, contact)
- `agri-ventures.html` Blackvault Agri Ventures Ltd (green theme)
- `finance-capital.html`, `technology-innovation.html`, `energy-resources.html`, `infrastructure-industrial.html` (themed, marked "In development")
- `404.html`, `_venture-template.html` (copy to make new venture pages)

## Files
- `assets/styles.css` all styling and per-venture themes (`body.ag`, `th-fin`, `th-tech`, `th-en`, `th-inf`)
- `assets/main.js` contact config, menu, scroll effects, ventures panel
- `_headers` security headers for Cloudflare Pages; `sitemap.xml`, `robots.txt`, `site.webmanifest`

## Domain and email
Domain: blackvault.co.ke. The addresses enquiries@, opportunities@, partnerships@, corporate@ and agri@blackvault.co.ke are set in `assets/main.js`. Create them (or forward them) before launch, for example with Cloudflare Email Routing.
