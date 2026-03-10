# Swapnil Aswale — Personal Portfolio

A single-page static portfolio website. No build tools, no frameworks — just HTML, CSS, and vanilla JS.

## Local Preview

Open `index.html` directly in a browser, or use a local server:

```bash
# Python
cd portfolio-website
python3 -m http.server 8080

# Node
npx serve .
```

Then visit `http://localhost:8080`.

## Deploy to GitHub Pages

### Option A: Dedicated repository

1. Create a new GitHub repository (e.g. `swapnilaswale.github.io` for a user site, or `portfolio` for a project site).
2. Copy the contents of this folder into the repo root.
3. Push to `main`.
4. Go to **Settings > Pages** and set source to **Deploy from a branch** > `main` > `/ (root)`.
5. Your site will be live at `https://<username>.github.io/` (user site) or `https://<username>.github.io/portfolio/` (project site).

### Option B: Subdirectory in an existing repo

1. Rename this folder to `docs/` at the repo root, or keep it as `portfolio-website/`.
2. Push to `main`.
3. Go to **Settings > Pages** and set source to the appropriate folder.

### Custom Domain

1. Add a `CNAME` file in this folder with your domain (e.g. `swapnilaswale.com`).
2. In your DNS provider, add a CNAME record pointing to `<username>.github.io`.
3. GitHub Pages will pick up the custom domain automatically.

## Structure

```
portfolio-website/
  index.html   — Single-page portfolio (all HTML, CSS, JS inline)
  README.md    — This file
```

## Updating Content

All content is in `index.html`. Edit the HTML directly — no build step required. The file is self-contained with inline CSS and JS.
