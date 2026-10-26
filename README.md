# Hoorin Money — GitHub Pages files

## Upload
1. Create a GitHub repository named `hoorin-money` (Public is simplest for GitHub Pages).
2. Upload **all files in this folder**, keeping the filenames and folder structure.
3. Ensure the app HTML is named `index.html` in the repository root.
4. In **Settings → Pages**, choose **Deploy from a branch**, branch `main`, folder `/(root)`, then Save.
5. Open the published Pages URL and wait for the deployment to finish.

## Included files
- `index.html` — Hoorin Money app. Includes a fix for the missing currency-rate element that could stop the initial render and make buttons appear broken.
- `manifest.webmanifest` — installable PWA metadata.
- `sw.js` — service worker for caching the app shell for offline reopening.
- `icon.svg` — app icon.
- `.nojekyll` — disables unnecessary Jekyll processing.

## Google Drive backup
Google Drive backup requires a Google OAuth **Web application** client ID configured in Google Cloud Console. Add the exact published GitHub Pages origin (for example `https://YOUR-USERNAME.github.io`) to **Authorized JavaScript origins**. Do not put a client secret in this HTML. Drive access is authorized in the open browser session; this static app cannot guarantee backups while fully closed.

## Important
- This is a static GitHub Pages app; it has no private server or database.
- Financial entries are stored in the browser's local storage on the device. Export JSON and maintain Drive backups; clearing browser/site data or uninstalling can erase local data.
- The service worker and PWA installation require HTTPS, which GitHub Pages provides.
