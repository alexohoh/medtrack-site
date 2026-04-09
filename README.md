# MedTrack marketing site

Static HTML pages served directly by GitHub Pages — no Jekyll, no build step.
The `.nojekyll` file tells GitHub Pages to serve these files as-is.

## Files

- `index.html` — landing page with links to privacy + support
- `privacy.html` — full privacy policy (required by Apple for HealthKit apps)
- `support.html` — FAQ and support contact
- `.nojekyll` — disables GitHub Pages' Jekyll build pipeline

## Publishing

### Option A — alongside the MedTrack project (public repo)

1. Push the whole project to a public GitHub repo
2. Repo → **Settings** → **Pages**
3. Source: **Deploy from a branch**, Branch: `main`, Folder: `/docs`
4. Save. Site is live at:
   - `https://<username>.github.io/<repo>/` (landing)
   - `https://<username>.github.io/<repo>/privacy.html`
   - `https://<username>.github.io/<repo>/support.html`

### Option B — dedicated public site repo (keeps app code private)

1. Create a new public repo `medtrack-site`
2. Copy everything in this `docs/` folder to the repo root
3. Push
4. Repo → Settings → Pages → Source: `main` branch, `/ (root)` folder

## Updating

The files are plain HTML with inline CSS. Open any of them in a text editor
and change what you need. No rebuild required — GitHub Pages will serve the
new version within a minute of pushing.
