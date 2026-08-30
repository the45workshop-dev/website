# 45° Workshop

Marketing site for 45° Workshop — custom coffee carts, mobile bars, and event bar rentals built in San Jose, CA.

Static HTML. No build step.

## Pages

| URL | File |
| --- | --- |
| `/` | `Home.dc.html` |
| `/start` | `StartHere.dc.html` |
| `/builds` | `Builds.dc.html` |
| `/our-work` | `Portfolio.dc.html` |
| `/services` | `Services.dc.html` |
| `/about` | `About.dc.html` |
| `/contact` | `Consultation.dc.html` |

The deployable site is generated into `docs/` as one `index.html` per route, giving clean URLs on any static host.

## Structure

- `_ds/` — design system stylesheet and component bundle
- `img/` — optimized site photography (JPEG, max 1800px)
- `uploads/` — original full-resolution source photos, excluded from Git
- `support.js` — page runtime
- `_redirects`, `robots.txt`, `sitemap.xml` — deploy and SEO config

## Local preview

```
python3 -m http.server 8000
```

Then open http://localhost:8000/ from inside `docs/`.

## Deployment

GitHub Pages, served from the `docs/` folder on `main` (Pages only supports `/` or `/docs`).

Repo Settings to Pages: source `main`, folder `/docs`.

`docs/CNAME` holds the custom domain (45workshop.com). `docs/.nojekyll` stops Jekyll from touching the files. DNS is managed in AWS Route 53 and points at GitHub's Pages IPs.

Pushes to `main` publish within a minute or two.

## Workflow

Branch off `main`, commit, open a pull request, review the Cloudflare preview link, then merge.

```
git checkout -b my-change
git commit -am "Describe the change"
git push -u origin my-change
```

## Contact

the45workshop@gmail.com
