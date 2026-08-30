repo: the45workshop-dev/website
branch: main

## Last sync
date: 2026-08-30T04:54:01Z
commit: e03691cd5851

### Updated in this project
- Repo now holds the .dc.html sources and `img/`, but not yet the generated `site/` build.
- Generated `site/` — a GitHub Pages build with one `index.html` per route for clean URLs, plus `CNAME` and `.nojekyll`.
- Compressed all site photography into `img/` (JPEG, max 1800px, ~2 MB total); `uploads/` originals excluded from Git.
- Added `README.md` and per-page SEO metadata with LocalBusiness structured data on Home.

## Screen map
| Screen | Files |
| --- | --- |
| Home | Home.dc.html |
| Start Here | StartHere.dc.html |
| Builds | Builds.dc.html |
| Our Work | Portfolio.dc.html |
| Services | Services.dc.html |
| About | About.dc.html |
| Consultation | Consultation.dc.html |
| Runtime + design system | support.js, image-slot.js, _ds/ |
| Deploy config | site/CNAME, site/.nojekyll, robots.txt, sitemap.xml |
| Generated build | site/ (regenerated from the .dc.html sources) |
