# Depreciation Calculator — India

Work out depreciation and tax saved on business assets in India.

A single-page, offline-capable PWA. No build step, no dependencies — plain
HTML/CSS/JS served as static files.

## Files

| Path | Purpose |
| --- | --- |
| `index.html` | The whole app (inline CSS + JS) |
| `manifest.json` | PWA manifest — name, colours, icons |
| `sw.js` | Service worker, caches the app for offline use |
| `icons/` | App icons (192, 512, 1024, apple-touch) |
| `vercel.json` | Cache headers for Vercel |

## Deploying to Vercel

The repo is ready to import as-is — there is no build step.

1. Go to <https://vercel.com/new> and sign in with GitHub.
2. Import `arham1154/Depreciation-`.
3. Leave the defaults: Framework Preset **Other**, Root Directory `./`,
   Build Command empty, Output Directory empty.
4. Click **Deploy**.

Every push to `main` redeploys automatically; other branches get preview URLs.

## Running locally

A plain `file://` open works, but service workers need HTTP:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```
