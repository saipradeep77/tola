# Tola — Marketing Site

Static marketing site for Tola, a full-stack AI automation agency for Irish business.

## Stack

Pure HTML + CSS, no build step. Hosted on Vercel.

- `index.html` — main landing page (capability-led, full-stack positioning)
- `solicitors.html` — niche page for Irish law firms
- `vercel.json` — clean URL config + redirects

## Local preview

Just open `index.html` in a browser. No server needed.

For a more accurate preview matching production:

```bash
npx serve .
```

## Deploying

Connected to Vercel via GitHub. Pushes to `main` deploy automatically.

## Adding a niche page

1. Copy `solicitors.html` to `<niche>.html`
2. Update copy, calculator inputs, FAQs for the niche
3. Update `index.html` industry grid card link to `/<niche>`
4. Remove the matching redirect from `vercel.json`
5. Commit and push

## Domains

- Production: `tola.ie`
- Cold-email send domains served separately (Cloudflare): `gettola.com`, etc.
