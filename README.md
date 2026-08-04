# Street Photography Portfolio — GitHub Pages Setup

## What you have
- `index.html` — the whole site (HTML/CSS/JS in one file, no build step needed)
- `images/` — folder where your photos go

Until you add real photos, the grid automatically falls back to placeholder
images, so the site works right away.

## 1. Create the GitHub repo
1. Go to github.com → **New repository**.
2. Name it exactly `yourusername.github.io` (replace `yourusername` with your
   actual GitHub username) if you want it at the root of your GitHub domain.
   *Or* name it anything else (e.g. `street-portfolio`) if you're fine with
   the site living at `yourusername.github.io/street-portfolio`.
3. Set it to **Public**. Don't add a README (you already have one).

## 2. Upload the files
Easiest way (no command line needed):
1. Open your new repo on github.com.
2. Click **Add file → Upload files**.
3. Drag in `index.html`, `README.md`, and your `images` folder (with your
   actual photos inside — name them anything, just update the `photos` array
   near the bottom of `index.html` to match).
4. Commit the changes.

## 3. Turn on GitHub Pages
1. In the repo, go to **Settings → Pages**.
2. Under "Build and deployment", set **Source** to `Deploy from a branch`.
3. Set **Branch** to `main` and folder to `/ (root)`. Save.
4. Wait ~1 minute, refresh — GitHub will show you the live URL.

## 4. Add your own photos
Open `index.html`, find the `photos` array near the bottom (search for
`PHOTO LIST`). Each entry looks like:

```js
{ src: "images/photo-01.jpg", tag: "0A", title: "Crosswalk, Knez Mihailova" }
```

- `src` — path to your image inside the `images/` folder
- `tag` — the small frame number shown on hover (purely cosmetic, like a
  film negative number — set it to whatever you like)
- `title` — caption shown on hover and in the lightbox

Add, remove, or reorder entries freely — the grid and lightbox update
automatically.

## Tips
- Keep photos under ~1–2MB each (resize to ~2000px on the long edge) so the
  site loads fast.
- JPG works best for photos.
- To use a custom domain later, add a `CNAME` file — ask me if you want help
  with that step.
