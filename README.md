# AMICO Lab website

Single-page static site for https://amicolab.org/ — no build step, ready for GitHub Pages.

## Structure
- `index.html` — the whole site (styles inline): research, brain fingerprinting 101,
  selected work + recent publications, news, people (incl. alumni & collaborators),
  where we are, join us.
- `assets/` — optimized images and videos (all self-hosted except the VideoPress
  connectome embed and Google Fonts).
- `404.html` — redirects old URLs (e.g. /amicolab-team/) to the homepage.

## Deploy to GitHub Pages
1. Create a public repo (e.g. `amicolab-site`), push this folder's contents.
2. Repo → Settings → Pages → Source "Deploy from a branch", branch `main`, folder `/ (root)`.
3. Test at https://YOURUSERNAME.github.io/amicolab-site/
4. When happy: Settings → Pages → Custom domain `amicolab.org`, and at GoDaddy set
   the four GitHub Pages A records (185.199.108.153 / .109.153 / .110.153 / .111.153)
   plus a `www` CNAME to YOURUSERNAME.github.io. Keep "Enforce HTTPS" on once offered.
5. Original raw media and the old multi-page draft are kept locally in
   `../amicolab-site-backup/` (not part of the repo).

## Notes
- The rotating-connectome video in "Research" still uses the VideoPress embed;
  a self-hosted copy exists at assets/connectome.mp4/webm if WordPress is ever cancelled.
- CHBH building photo © Associated Architects — confirm permission before launch,
  or swap for an official UoB photo.
