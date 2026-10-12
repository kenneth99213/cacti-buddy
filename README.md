# Plant Buddy

A cactus catalogue for your iPhone. Add each cactus with a name and photo, take progress photos over time (the newest one becomes its catalogue picture), log waterings and keep notes. Everything is stored on the phone, works offline, and needs no account.

## Put it on GitHub Pages

1. On github.com, click **New repository**. Name it `plant-buddy`, make it **Public**, and click **Create repository**.
2. On the new repo page, click **uploading an existing file**. Drag in everything from this folder: `index.html`, `manifest.webmanifest`, `sw.js`, `README.md` and the `icons` folder. Click **Commit changes**.
3. Go to **Settings → Pages**. Under **Branch**, pick `main` and `/ (root)`, then click **Save**.
4. After a minute or two the page shows your address, something like `https://YOUR-USERNAME.github.io/plant-buddy/`.

## Install it on your iPhone

1. Open that address in **Safari**.
2. Tap the **Share** button, then **Add to Home Screen**, then **Add**.
3. Always open Plant Buddy from the home screen icon. The home screen app keeps its own storage, separate from Safari tabs.

## Backups

Your cacti live only on that phone. Deleting the app icon, or clearing website data in Settings → Safari, erases them.

- Tap the download icon at the top of the catalogue, then **Export backup**. On iPhone the share sheet opens: choose **Save to Files** (iCloud Drive is a good spot).
- The backup is a normal `.zip` with a `data.json` file and a `photos` folder, so you can open it on any computer.
- To restore, tap the same icon, choose **Choose backup file**, and pick the zip. Plants in the backup are added back; a plant that exists in both gets the backup's version.
- The app reminds you if it's been more than 30 days since your last export.

## Updating the app later

Upload the changed files to the repo the same way. In `sw.js`, change `plant-buddy-v1` to `plant-buddy-v2` (and so on) whenever you update, so phones pick up the new version. The update shows on the second launch after you publish. Your plants are not affected by updates.
