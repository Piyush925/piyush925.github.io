# Piyush Khandelwal — Portfolio

Static, dependency-free portfolio (plain HTML + CSS + a little JS). Light/dark theme, screenshot lightbox, fully responsive.

```
index.html      # the whole site
favicon.svg
assets/         # optimised WebP screenshots
.nojekyll       # tells GitHub Pages to serve files as-is
```

## Publish on GitHub Pages

**Option A — user site (`https://piyush-ca.github.io`)**

1. Create a public repo named exactly `piyush-ca.github.io`.
2. Push these files to the `main` branch root:
   ```bash
   git init && git add . && git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/piyush-ca/piyush-ca.github.io.git
   git push -u origin main
   ```
3. Repo → **Settings → Pages** → Source: *Deploy from a branch* → `main` / `(root)`.
4. Live in ~1 minute at `https://piyush-ca.github.io`.

**Option B — project site** (`https://piyush-ca.github.io/portfolio`): same steps with any repo name. All paths are relative, so it works under a sub-path too.

## Editing

- Text lives directly in `index.html` (sections: hero, work, also built, impact, approach, contact).
- Add a screenshot: drop a `.webp`/`.png` into `assets/` and copy an existing `<figure>` block.
- Colours/fonts are CSS variables at the top of the `<style>` block.
