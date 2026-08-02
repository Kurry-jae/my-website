# Asaase Kitchen — Sakaman

Website for Asaase Kitchen — Sakaman, a Ghanaian restaurant inside JP Sakaman Service Station, Accra.

- 🍽️ Dine-in · 🥡 Takeaway · 🚚 No-contact delivery
- ⭐ 4.6/5 from 650 Google reviews
- 📞 +233 55 533 3555

## Pages

| Page | File |
|---|---|
| Home | `index.html` |
| About Us | `about.html` |
| Menu | `menu.html` |
| Download Menu | `download.html` |
| Contact Us | `contact.html` |

Shared styling lives in `styles.css`. The downloadable PDF menu is `asaase-kitchen-menu.pdf` — the "Download Menu" tab and every download button across the site link to it.

No build step, no dependencies — just static files.

## Running locally

Open `index.html` in a browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploying with GitHub Pages

1. Push all files to the repo (keep them at the root — `index.html`, `about.html`, `menu.html`, `download.html`, `contact.html`, `styles.css`, `asaase-kitchen-menu.pdf`).
2. Go to **Settings → Pages**.
3. Under **Source**, select the `main` branch and `/ (root)` folder → **Save**.
4. Your site will be live at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Custom domain (asaasekitchen.com)

1. In **Settings → Pages**, add `asaasekitchen.com` under **Custom domain**.
2. At your domain registrar, point DNS:
   - `A` records for the root domain to GitHub Pages' IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - a `CNAME` record from `www` to `<your-username>.github.io`
3. Wait for DNS to propagate, then enable **Enforce HTTPS** in the Pages settings.

## Updating the menu

If dish names or prices change, update the relevant section in `menu.html` and regenerate `asaase-kitchen-menu.pdf` to keep the downloadable version in sync.
