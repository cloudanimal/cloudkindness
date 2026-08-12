# Cloud Kindness

Marketing site for **Cloud Kindness**, a boutique AI and security consultancy led by Joe Cook.

Static site, no build step. Hosted on GitHub Pages with the custom domain `cloudkindness.com`.

## Structure

```
index.html          Single-page site
assets/styles.css   Styles (light + dark theme via CSS variables)
assets/main.js      Theme toggle, mobile nav
assets/favicon.svg  Brand mark
CNAME               Custom domain for GitHub Pages
robots.txt          Crawl directives
sitemap.xml         Sitemap
```

## Local preview

Open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8080
```

## Deploy (GitHub Pages)

1. Create the repo (for example `cloudanimal/cloudkindness`) and push this folder.
2. In repo Settings, Pages: deploy from branch `main`, folder `/ (root)`.
3. The `CNAME` file points Pages at `cloudkindness.com`.
4. At your DNS registrar, point the apex domain at GitHub Pages:
   - A records to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - and a `www` CNAME to `cloudanimal.github.io` (optional)
5. Enable "Enforce HTTPS" once the certificate is issued.

## Open item

- Finalize the contact method. Current call-to-action opens email to `josephwcook@gmail.com`.
  Options discussed: branded `joe@cloudkindness.com`, a contact form, or a booking link.
