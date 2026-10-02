# HEAD-END: SOVEREIGN v12.1 — GitHub Pages Setup

## Upload
Upload every file from this package to the **root** of your GitHub repository. `index.html` must be at the repository root, not inside another folder.

Expected root files:

- `index.html`
- `manifest.webmanifest`
- `service-worker.js`
- `.nojekyll`
- `README.md`
- `GITHUB-PAGES-SETUP.md`
- `icon-192.png`
- `icon-512.png`
- `apple-touch-icon.png`

## Enable GitHub Pages
1. Open the repository on GitHub.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch `main`.
5. Select folder `/(root)`.
6. Save.
7. Wait for GitHub to publish the site.

Your address will normally be:

`https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`

## Updating from v12 / v11
Replace the old root files with the v12.1 files and commit the changes to `main`.

v12.1 uses a new service-worker cache key and explicitly checks for a newer service worker after load so installed/PWA copies can update. If a device still shows an older build, fully close and reopen the site or refresh it once while online.

## Secret Gorilla World archive
The archive is intentionally locked on a fresh save. Players must use **Search Area** and find the hidden `SOVEREIGN training case // Gorilla World 05-28-2016` note. Investigating or preserving the note unlocks all 15 archive perspectives.

## iPhone / iPad
Open the deployed HTTPS address in **Safari**. Do not run `index.html` from the Files app / Quick Look. Safari provides the browser storage, service-worker, PWA and audio behavior expected by the game.

Use **Share → Add to Home Screen** for an app-like shortcut.


## v12.1 verification note
All application URLs remain repository-relative (`./...`) so a project site hosted under `YOUR-USERNAME.github.io/YOUR-REPOSITORY/` does not accidentally request files from the domain root. The package includes `.nojekyll`, which allows GitHub Pages to publish the static files directly.
