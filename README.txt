FOUNDRY — files for GitHub Pages + PWABuilder

Upload everything in this folder to the root of your Foundry-OS repo
(replace the existing index.html, manifest.json and icons):

  index.html      the app
  manifest.json   app name, icons, fullscreen mode
  sw.js           offline support (PWABuilder checks for this)
  icon-192.png    app icon
  icon-512.png    app icon
  .nojekyll       empty file; stops GitHub Pages hiding the .well-known folder

After PWABuilder gives you assetlinks.json, it goes at:
  https://<your-username>.github.io/.well-known/assetlinks.json
That is the ROOT of the domain, so it lives in a separate repo named
<your-username>.github.io (with its own empty .nojekyll file), not in Foundry-OS.
