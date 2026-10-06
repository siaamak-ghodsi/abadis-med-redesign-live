# Abadis Med — redesign live preview

Live: https://siaamak-ghodsi.github.io/abadis-med-redesign-live/

This repo holds no site code. A GitHub Actions workflow (`.github/workflows/deploy.yml`) checks out
[`ShushtarWolf/abadis-med-website-redesign`](https://github.com/ShushtarWolf/abadis-med-website-redesign) (`main`)
and publishes its `site/` folder to GitHub Pages here.

- Runs every ~5 minutes (GitHub cron is best-effort; delays of 5–15+ min are normal) and skips when upstream `main` hasn't changed.
- Deploy now: Actions → "Deploy Abadis redesign" → Run workflow (or `gh workflow run deploy.yml -R siaamak-ghodsi/abadis-med-redesign-live`).
- `deployed-sha.txt` on the live site shows which upstream commit is published.
