NET TAKE HOME SALARY CALCULATOR — INSTALL ON YOUR ANDROID PHONE
================================================================

This folder is a Progressive Web App (PWA). Once hosted on any free
static host, it installs on your phone with its own icon and works
FULLY OFFLINE afterwards.

OPTION A — GitHub Pages (free, 5 minutes, recommended)
------------------------------------------------------
1. Create a free account at github.com (if you don't have one).
2. Create a new repository, e.g. "salary-calculator" (Public).
3. Upload ALL files in this folder (index.html, manifest.json,
   sw.js, icon-192.png, icon-512.png) to the repository:
   "Add file" -> "Upload files".
4. Go to Settings -> Pages -> Source: "Deploy from a branch",
   Branch: main, folder: / (root). Save.
5. After a minute your app is live at:
   https://<your-username>.github.io/salary-calculator/
6. Open that link in CHROME ON YOUR PHONE.
   Chrome will show "Add to Home screen" / "Install app"
   (or use the three-dot menu -> "Install app").
7. Done. The icon appears on your home screen, opens full-screen
   like a native app, and works without internet from then on.

OPTION B — Netlify Drop (no account needed to try)
--------------------------------------------------
1. On a computer, open https://app.netlify.com/drop
2. Drag this whole folder onto the page.
3. It gives you a link like https://random-name.netlify.app
4. Open the link in Chrome on your phone -> Install app.

OPTION C — No hosting at all (quick and dirty)
----------------------------------------------
Copy just index.html to your phone (USB / email to yourself) and
open it with Chrome. Everything works, but there is no home-screen
icon or full-screen mode. Fine for occasional use.

WHY NOT AN APK?
---------------
A signed APK needs the Android SDK to build. If you want a true
APK (e.g., to share the file directly with colleagues without any
hosting), ask me for the "Android Studio WebView project" and I
will generate a complete ready-to-build project - you would open
it in Android Studio and press Build. The PWA above is usually the
easier path.

UPDATING THE APP
----------------
If the calculator logic changes (new tax slabs, etc.), replace
index.html on your host and bump the cache name in sw.js
(nth-calc-v1 -> v2). Installed phones pick up the update on next
launch with internet.
