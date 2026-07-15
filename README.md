# GetSiteNow — auto-deploy setup (one time)

Goal: connect this folder to GitHub so every future change goes live on
getsitenow.in by itself — no terminal, no dragging.

The 3 files that MUST always ship together:
  index.html · logo.png · logo-light.png
(vercel.json and robots.txt come along too.)

────────────────────────────────────────────────────────
STEP 1 — Put these files on GitHub  (no terminal needed)
────────────────────────────────────────────────────────
1. Go to github.com and sign in (make a free account if you don't have one).
2. Click the + (top right) → "New repository".
3. Name it:  getsitenow
   Set it Public or Private — both work. Click "Create repository".
4. On the new empty repo page, click the link
   "uploading an existing file".
5. Open this `site` folder on your Mac, select ALL the files inside
   (index.html, logo.png, logo-light.png, vercel.json, robots.txt)
   and drag them onto the GitHub upload area.
6. Click "Commit changes".

────────────────────────────────────────────────────────
STEP 2 — Connect the repo to your EXISTING Vercel project
────────────────────────────────────────────────────────
(This keeps your getsitenow.in domain exactly where it is.)
1. Go to vercel.com → open your "getsitenow" project.
2. Settings → Git → "Connect Git Repository".
3. Choose GitHub, authorise it, and pick the "getsitenow" repo.
4. Vercel builds from the repo. When it's done, getsitenow.in shows it.

Done. From now on, any change pushed to the repo deploys automatically.

────────────────────────────────────────────────────────
HOW TO UPDATE LATER  (after the site is edited)
────────────────────────────────────────────────────────
Easiest, no terminal:
  • On the GitHub repo page → "Add file" → "Upload files" → drag the new
    index.html in → "Commit changes". Vercel auto-deploys in ~30 seconds.

Even smoother for ongoing edits:
  • Install "GitHub Desktop" (desktop.github.com). It links this folder to
    the repo. After an edit: open GitHub Desktop → Commit → Push. Live in seconds.
