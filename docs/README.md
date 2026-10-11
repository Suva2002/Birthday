# Meghana's 25th Birthday

A birthday page with a live countdown, a 3D heart, candles and a tune, a letter, 25 wishes, a photo wall and fireworks.

## Folder layout

```
index.html              main page (must stay at the top level)
3d/
  three.min.js          Three.js r150, bundled so nothing is fetched from a CDN
  heart3d.js            the 3D heart in the hero
images/                 the photos (01-... to 16-...)
resources/
  css/styles.css        all styling
  js/main.js            countdown, cake, wishes, photo viewer, fireworks, confetti
  js/photos.js          the photo list and captions (edit captions here)
.nojekyll               tells GitHub Pages to serve the files as they are
```

## Put it on GitHub Pages

1. Create a new repository on GitHub (public is simplest).
2. Upload the CONTENTS of this folder so that `index.html` sits at the top level of the repository. Do not upload the zip file itself, and do not wrap everything in an extra folder.
3. Open the repository, then Settings, then Pages. Under "Build and deployment" choose "Deploy from a branch", pick the `main` branch and the `/ (root)` folder, then Save.
4. Wait a minute or two. The site appears at `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`.

## If it does not work on GitHub

- The file must be named `index.html`, all lowercase, at the top level.
- File and folder names are case sensitive on GitHub. `images/01-always-better-together.jpg` is not the same as `Images/01-Always-Better-Together.jpg`.
- Keep the folders exactly as listed above. The page loads everything with relative paths such as `images/...` and `resources/...`.
- After changing files, hold Shift and press Reload to skip the browser cache.
- Open the browser console (F12) and look for red "404" lines. They name the file GitHub could not find.

## Change things

- Captions or photo order: `resources/js/photos.js`
- Swap a photo: replace the file in `images/` with one of the same name (about 1200 px on the long side keeps it fast).
- Letter, wishes and colours: the letter text is in `index.html`, the wishes are at the top of the "wishes" block in `resources/js/main.js`, and the colours are the first lines of `resources/css/styles.css`.
- Birthday date for the countdown: search for `2026-10-13T00:00:00+05:30` in `resources/js/main.js`.
