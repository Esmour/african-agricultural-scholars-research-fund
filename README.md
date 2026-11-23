# African Agricultural Scholars Research Fund (AASRF)

A responsive Hugo website for the African Agricultural Scholars Research Fund.

## Local preview

1. Install Hugo (extended version recommended).
2. From this folder run:

   ```bash
   hugo server
   ```

3. Open the local address printed by Hugo (normally http://localhost:1313).

## Production build

```bash
hugo --minify
```

Hugo writes the production site to `public/`.

## Cloudflare Pages settings

Use the same GitHub-connected Cloudflare Pages workflow as the portfolio site:

- Framework preset: Hugo
- Build command: `hugo --minify`
- Build output directory: `public`
- Root directory: `/` (blank)
- Production branch: `main`
- Environment variable: `HUGO_VERSION` set to a current supported Hugo version (for example `0.145.0`)

Connect the new GitHub repository to Cloudflare Pages. Each push to `main` will trigger a deployment.

## Custom domain

In Cloudflare Pages, open the project → Custom domains → Set up a custom domain and add:

`african-agricultural-scholars-research-fund.org`

Also add `www.african-agricultural-scholars-research-fund.org` if you want the www version. Set one as canonical and redirect the other to it. Follow the DNS instructions shown in Cloudflare; do not copy DNS records from the portfolio domain.

## Content notes before public launch

- The website intentionally states that no grant call is currently open.
- The initiative's legal status, governance arrangements and grant procedures are described as being in development; update these statements only after they are formally established.
- Founding-member biographies and affiliations should be checked and approved by each member.
- Add real member photographs and confirm consent before publishing.
- Confirm the official contact mailbox and ensure it is monitored.
- Review the official organisation name, legal structure, privacy requirements and any donation mechanisms before collecting personal or financial information.

## Structure

- `content/` — page content in Markdown
- `layouts/` — Hugo templates
- `static/css/site.css` — responsive visual system
- `static/js/site.js` — mobile navigation
- `static/images/` — logo and local image assets
