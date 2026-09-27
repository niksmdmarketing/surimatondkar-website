# surimatondkar.com

Author website for Suri Matondkar. Plain HTML + CSS, no build step, hosted on GitHub Pages at **surimatondkar.com**.

## Files

| File | What it is |
| --- | --- |
| `index.html` | Home: logo, photo + intro, and the four navigation bars |
| `about.html` | About |
| `awards.html` | Awards and shortlists |
| `work.html` | Work: publications |
| `contact.html` | Email + LinkedIn |
| `styles.css` | All styling — colours are at the top under `:root` |
| `images/` | Photos |
| `CNAME` | Tells GitHub Pages to serve the site at surimatondkar.com |

To edit text, open the page's `.html` file and change the words between the tags. The header (logo + Instagram link) is repeated in each page, so change the Instagram link in all five files.

To preview locally, open `index.html` in a browser.

## Going live

1. **GitHub Pages:** repo → Settings → Pages → Source: "Deploy from a branch", Branch: `main`, folder `/ (root)`. Custom domain: `surimatondkar.com`, then tick "Enforce HTTPS" once it's available.
   GitHub Pages on a *private* repo needs a paid GitHub plan; on a free account make the repo public (it only contains the public website).
2. **DNS (at WordPress.com, where the domain is registered):** Upgrades → Domains → surimatondkar.com → DNS records. Add:
   - `A` records for `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` for `www` → `niksmdmarketing.github.io`

   Remove any existing `A`/`CNAME` records for `@` and `www` that point to WordPress. DNS changes can take up to 24–48 hours.
