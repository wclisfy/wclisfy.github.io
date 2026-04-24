# wclisfy.github.io — Personal website

Willis Chun Lai Wong's academic homepage.
Built with plain Jekyll, deployed via GitHub Actions.

Live at <https://wclisfy.github.io>.

---

## What changed in this overhaul

- New **warm & creative** theme (see `assets/css/style.css` + `_layouts/default.html`) replacing minimal-mistakes.
- Real content: generative morphology, Cantonese reduplication, 5 conference presentations (FoCaL-7, WICL-7, FoCaL-8, SICOGG27, IcoLL2026).
- SEO wired up: `jekyll-seo-tag`, `jekyll-sitemap`, JSON-LD `Person` schema, `robots.txt`, `/feed.xml`.
- Working papers and abstracts live in `/docs/` and are linked from `/research/` and `/cv/`.

## Deploy (you already have the pipeline)

Your repo already has `.github/workflows/github-pages.yml` which on every push to `main`:

1. Builds Jekyll with `bundle exec jekyll build`.
2. Deploys `_site/` to the `gh-pages` branch via `peaceiris/actions-gh-pages`.

So all you need to do is **commit + push to `main`**:

```bash
cd ~/Documents/GitHub/wclisfy.github.io
git add -A
git commit -m "Overhaul site: warm theme, real content, SEO"
git push origin main
```

Then on GitHub:

- **Settings → Pages** → Source: *Deploy from a branch* · Branch: **`gh-pages`** · `/ (root)`.
  (If it's still on `main`, switch it to `gh-pages` — that's where the workflow publishes.)
- Watch the **Actions** tab; the build usually takes ~1 minute.

## Get found on Google

1. Go to <https://search.google.com/search-console> → Add property (URL prefix: `https://wclisfy.github.io/`).
2. Pick **HTML tag** verification; copy the `content="..."` value into `_config.yml`:
   ```yaml
   google_site_verification: "paste-here"
   ```
3. Commit + push. Back in Search Console, click **Verify**.
4. Sidebar → **Sitemaps** → submit: `sitemap.xml`.
5. Sidebar → **URL Inspection** → paste `https://wclisfy.github.io/` → **Request Indexing**. Repeat for `/about/`, `/research/`, `/cv/`.
6. Also do it on Bing: <https://www.bing.com/webmasters>. (Bing powers DuckDuckGo too.)

**Timeline:** Google usually picks a new page up within a few days to ~2 weeks.
Searching **"Willis Chun Lai Wong linguist"** or **"wclisfy"** will find you fastest once indexed.

## Edit the site

- `_config.yml` — site title, tagline, socials, affiliation.
- `index.md` / `about.md` / `research.md` / `cv.md` — page content.
- `_data/publications.yml` — add each new paper/talk here; `/research/` updates automatically.
- `docs/` — drop PDFs here (manuscripts, abstracts, handouts). Use dash-separated filenames so URLs stay clean, e.g. `2026-RNR-workshop-abstract.pdf`.
- `assets/img/avatar.jpg` — profile photo (square). If missing, the hero still renders.
- `assets/cv.pdf` — optional printable CV; the button on `/cv/` becomes live when present.

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve
# open http://localhost:4000
```

Requires Ruby (`brew install ruby` on Mac).

## File map

```
wclisfy.github.io/
├── _config.yml
├── _data/
│   ├── navigation.yml
│   └── publications.yml
├── _layouts/default.html
├── .github/workflows/github-pages.yml
├── assets/
│   ├── css/style.css
│   └── img/favicon.svg
├── docs/*.pdf            # manuscripts, abstracts, handouts
├── index.md · about.md · research.md · cv.md
├── 404.md · robots.txt
├── Gemfile · .gitignore
└── README.md
```
