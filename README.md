# Anurag — Performance Marketer Portfolio

A single-page portfolio site built with plain HTML/CSS/JS (no build step, no dependencies) — ready to host on GitHub Pages.

## Deploy on GitHub Pages

1. Create a new repository on GitHub, e.g. `anurag-portfolio`.
2. Add these two files (`index.html`, `README.md`) to the repo — either via the GitHub web UI ("Add file → Upload files") or with git:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/anurag-portfolio.git
   git push -u origin main
   ```
3. On GitHub: go to your repo → **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. Wait a minute — your site will be live at:
   `https://<your-username>.github.io/anurag-portfolio/`

## Using a custom domain (optional)

If you want it on your own domain instead of the github.io URL:
1. In repo **Settings → Pages → Custom domain**, enter your domain and save (this creates a `CNAME` file).
2. At your domain registrar, add a `CNAME` record pointing to `<your-username>.github.io`.

## Editing content later

Everything — text, links, colors — lives in `index.html`. Key spots:
- Colors: the `:root { ... }` block near the top of the `<style>` section.
- Section text: search for the section by its `id` (`hero`, `about`, `skills`, `work`, `experience`, `contact`).
- LinkedIn/email links: in the `<footer>` section near the bottom.

No build tools, no npm install — just edit and push.
