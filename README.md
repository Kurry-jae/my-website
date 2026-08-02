# Asaase Kitchen — Sakaman

Website for Asaase Kitchen — Sakaman, a Ghanaian restaurant inside JP Sakaman Service Station, Accra.

- 🍽️ Dine-in · 🥡 Takeaway · 🚚 No-contact delivery
- ⭐ 4.6/5 from 650 Google reviews
- 📞 +233 55 533 3555

## Structure

Single-page static site — everything (HTML, CSS, JS) lives in `index.html`. No build step, no dependencies to install.

## Running locally

Just open `index.html` in a browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploying with GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, select the `main` branch and `/ (root)` folder.
4. Save — your site will be live at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Custom domain (asaasekitchen.com)

1. In **Settings → Pages**, add `asaasekitchen.com` under **Custom domain**.
2. At your domain registrar, point DNS:
   - `A` records for the apex domain to GitHub Pages' IPs (185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153), or
   - a `CNAME` record from `www` to `<your-username>.github.io`.
3. Wait for DNS to propagate, then enable **Enforce HTTPS** in the Pages settings.
