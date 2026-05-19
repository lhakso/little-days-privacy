# little-days-privacy

Source for the public LittleDays privacy policy site, served via GitHub Pages.

This is a **separate, public repo**. The LittleDays iOS source code lives in a different, **private** repo — keep them apart.

## Publishing (one-time setup)

1. From this directory: `git init && git add . && git commit -m "initial privacy site"`.
2. Create a new **public** GitHub repo named `little-days-privacy` under the `lukehakso` account.
3. Push: `git remote add origin git@github.com:lukehakso/little-days-privacy.git && git push -u origin main`.
4. In the repo on GitHub: **Settings → Pages**. Set **Source** to `Deploy from a branch`, **Branch** to `main`, folder to `/ (root)`. Save.
5. After about a minute, the site will be live at:

   **https://lukehakso.github.io/little-days-privacy/**

The iOS app's Settings → Privacy Policy row links to that URL.

## Editing later

1. Edit `privacy.md` **and** `index.md` — keep them in sync (Jekyll needs a real file at root for the homepage).
2. Bump the **Effective date** at the top of both files.
3. Commit and push. GitHub Pages auto-rebuilds in ~1 minute.
