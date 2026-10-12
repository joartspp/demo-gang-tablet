# KKTown Gang Tablet — Prototype

Static prototype of the gang management tablet (mock data, runs fully in the browser).
Refresh resets all data. Scenario switcher (visitor / member / assistance / leader / president) is the bar at the bottom-left.

## Deploy to GitHub Pages

1. Create a NEW public repo (e.g. `gang-tablet-prototype`) — do not use the game server repo.
2. Put the contents of this folder in the repo root (`index.html`, `assets/`, `.nojekyll`).
3. Repo → Settings → Pages → Source: "Deploy from a branch" → Branch `main` / `(root)` → Save.
4. Open `https://<username>.github.io/<repo>/` after ~1 minute.

## Rebuild after the UI changes

```
cd resources/[Script]/[reworkable]/kkcore-gang-manage/ui_dev
npx vite build --mode proto --outDir <path-to-this-folder> --emptyOutDir
```
(keep `.nojekyll` and this README: re-add them after `--emptyOutDir`)
