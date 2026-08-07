88+ COCKTAILS — Deploy Guide (Path 1: PWA)
===========================================

WHAT'S IN THIS FOLDER
  index.html            The complete app (all 88 drinks built in)
  manifest.webmanifest  Tells phones this is an installable app
  sw.js                 Service worker — makes it work offline
  icon-*.png            App icons (the 88+ seal)
  apple-touch-icon.png  iPhone home-screen icon

STEP 1 — PUT IT ON THE WEB (pick one, both free)

  Option A: Netlify Drop (fastest, ~1 minute)
    1. Go to  https://app.netlify.com/drop  in your browser
    2. Drag this ENTIRE FOLDER onto the page
    3. It gives you a live URL like  https://something-random.netlify.app
    4. (Optional) Create a free account to keep the site permanently
       and rename the URL to something like  88cocktails.netlify.app

  Option B: GitHub Pages (better if you'll keep iterating)
    1. Create a free account at github.com, make a new public repo
       (e.g. "88-cocktails")
    2. Upload all files in this folder to the repo
    3. Repo Settings -> Pages -> Source: "main" branch, root -> Save
    4. Your app appears at  https://YOURNAME.github.io/88-cocktails/

STEP 2 — PUT IT ON YOUR PHONE

  iPhone:  Open the URL in Safari -> tap the Share button ->
           "Add to Home Screen" -> Add.
  Android: Open the URL in Chrome -> menu (three dots) ->
           "Add to Home screen" / "Install app".

  It launches full-screen with the 88+ seal icon, works offline
  after the first visit, and REMEMBERS your bar inventory between
  sessions (saved on the device).

NOTES
  - Your inventory edits live only on the phone that made them.
  - To update the app later, replace the files at the same URL —
    phones pick up the new version on next launch. If a change
    doesn't appear, bump the cache name in sw.js ('cocktails88-v1'
    -> 'v2') before uploading.
  - To share with friends: just send them the URL.
