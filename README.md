# Dr Petrus Stone — Neurosurgeon Website

A clean, mobile-friendly, bilingual (English / Afrikaans) website for Dr Petrus Stone's neurosurgery practice in Bloemfontein, Free State.

## What's included

- Responsive single-page design
- English / Afrikaans language switcher
- Neurosurgery-focused SEO (meta tags, Open Graph, JSON-LD, sitemap, robots.txt)
- Embedded Facebook Page feed
- Contact details, map, patient forms and media links
- Dr Stone's official Mediclinic portrait and qualifications

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `neurochirurgie-site`).
2. Upload **all** files from this folder to the root of the repository:
   - `index.html`
   - `css/`
   - `js/`
   - `images/`
   - `robots.txt`
   - `sitemap.xml`
   - `CNAME`
3. Go to **Settings → Pages** in the GitHub repo.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose the `main` branch and `/(root)` folder, then click **Save**.
6. After a minute, the site will be live at:
   ```
   https://YOUR_USERNAME.github.io/neurochirurgie-site
   ```

## Use the custom domain (neurochirurgie.co.za)

1. In **Settings → Pages**, add `neurochirurgie.co.za` as a **Custom domain** and save.
2. In your domain/DNS provider's control panel, add GitHub Pages DNS records. GitHub will show the required values after you add the custom domain. Typically you add either:
   - Four `A` records pointing to GitHub's IPs, or
   - A `CNAME` record pointing to `YOUR_USERNAME.github.io`
3. Make sure the `CNAME` file in this repo contains:
   ```
   neurochirurgie.co.za
   ```
4. Wait for DNS propagation (usually minutes to a few hours), then visit:
   ```
   https://neurochirurgie.co.za
   ```

## Important note before sharing the GitHub Pages link

If you share the temporary `github.io` link **before** the real domain is connected, Facebook/Twitter preview images may not appear because the Open Graph and canonical URLs in `index.html` currently point to `https://neurochirurgie.co.za/`. The website itself will work fine; only the social previews are affected. Once the custom domain is live, everything will be correct.

## Local preview

```bash
cd /Users/leipoldt/Documents/neurochirurgie
python3 -m http.server 8080
# open http://localhost:8080
```

## Credit

Content based on the original site at [neurochirurgie.co.za](https://neurochirurgie.co.za) and the official [Mediclinic doctor profile](https://www.mediclinic.co.za/en/corporate/doctors/4/dr-petrus-stone.html).
