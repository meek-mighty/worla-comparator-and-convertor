# Worla's Comparator – hosting package

`index.html` is self-contained (all libraries embedded). Upload this whole folder to any static host.

## Make the logo appear when the site is searched or shared
1. Open `index.html` and replace **YOUR-DOMAIN** (3 places: og:image, twitter:image, logo) with your real domain, e.g. `worla.com`.
2. Keep these files in the same folder as `index.html`: `logo.png`, `og-image.png`, `favicon.ico`, `favicon-64.png`, `apple-touch-icon.png`.
3. Browser tab, bookmarks and phone home screen show the emblem; WhatsApp / LinkedIn / Slack / X / Facebook link previews show the full Worla logo card.
4. Google shows a favicon and logo only after it has crawled your live site: submit the URL in Google Search Console ("URL inspection -> Request indexing"). Timing is up to Google.

## Optional OCR (photos & scanned PDFs)
Keep the `vendor/` folder next to `index.html` and serve over http(s). Delete it if you don't need image/scan conversion.

## Run locally
    python3 -m http.server 8080     # http://localhost:8080
## Deploy
Netlify / Cloudflare Pages / Vercel (drag the folder), GitHub Pages, Azure Static Web Apps, IIS, Nginx/Apache, or Docker (`docker build -t worla . && docker run -p 8080:80 worla`).
