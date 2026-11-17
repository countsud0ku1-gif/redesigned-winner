# Mobile Command Center: web app 0.2

The installable version of the prototype. Upload this folder's contents to any web host. Keep `index.html` at the top level.

## What's new

- **Installable:** has its own icon, opens full screen and works offline (`manifest.webmanifest`, `sw.js`, `icons/`).
- **Backups as files:** in Settings → Your data, *Export backup* saves a `.json` file and *Import backup* restores from a file or pasted text.
- **Demo mode:** adding `?demo` to the link opens the app with sample data. It uses separate storage, so your real data is never shown or changed.
- **QR codes:** Settings → Share & install shows a QR code for the demo link or the full app.

## Moving your data from the Claude prototype

1. Open the prototype in Claude, go to Settings → Your data, tap **Export backup**, then **Copy backup**.
2. Open the hosted app, go to Settings → Your data, tap **Import backup**, paste, and tap **Import**.

## Shipping an update

Change the files, then bump `CACHE` at the top of `sw.js` (for example `mcc-v3`) so phones pick up the new version.
