# Abadis Med redesign: Siamak's branch preview

Live: https://siaamak-ghodsi.github.io/abadis-med-redesign-live/

This repo holds no site code. A GitHub Actions workflow (`.github/workflows/deploy.yml`) checks out
[`ShushtarWolf/abadis-med-website-redesign`](https://github.com/ShushtarWolf/abadis-med-website-redesign)
at branch **`siamak/redesign`** (Siamak's changes, kept separate from `main`) and publishes its `site/` folder
to GitHub Pages here.

- The shared `main` preview stays at https://shushtarwolf.github.io/abadis-med-website-redesign/ (unchanged by this repo).
- Runs every ~5 minutes (GitHub cron is best-effort; delays of 5–15+ min are normal) and skips when the branch hasn't changed.
- Deploy now: Actions → "Deploy Siamak preview" → Run workflow (or `gh workflow run deploy.yml -R siaamak-ghodsi/abadis-med-redesign-live`).
- `deployed-sha.txt` on the live site shows which upstream commit is published.
