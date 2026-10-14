VocabMaster PWA — Free setup
=============================

Files:
- index.html: your vocabulary app
- manifest.webmanifest: app name, install mode and icons
- sw.js: offline app-shell caching
- icons/: home-screen icons

IMPORTANT:
A PWA must be served from HTTPS (or localhost). Opening index.html directly from Downloads will NOT enable installation or service workers.

Free publishing steps (GitHub Pages):
1. Sign in or create a free GitHub account.
2. Create a NEW public repository, e.g. vocabmaster.
3. Upload all CONTENTS of this folder (index.html, manifest.webmanifest, sw.js, icons folder) to the repository root.
4. In the repository, open Settings -> Pages.
5. Under Build and deployment, select "Deploy from a branch"; choose branch "main" and folder "/ (root)", then Save.
6. Wait for the published HTTPS URL shown by GitHub Pages (usually https://YOUR-USERNAME.github.io/vocabmaster/).
7. Open that URL in Chrome on Android. Tap the three-dot menu -> Install app (or Add to Home screen) -> Install.
8. Open the new VocabMaster icon from the home screen.

The app can work offline after the first successful load, once the service worker has cached the files.
The first publish needs internet. Local browser progress uses localStorage and may not sync across devices.
