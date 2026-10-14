# diya mohan — personal site

Plain HTML, no build step. Vercel serves it as-is.

## Put it on Vercel (about 5 minutes)

**Option A: GitHub (recommended, so every push redeploys)**
1. Create a new GitHub repo, e.g. `diya-portfolio`, and upload `index.html`, `favicon.svg`, `vercel.json`.
2. Go to vercel.com → Add New → Project → Import that repo.
3. Framework preset: **Other**. Leave build command and output directory empty. Click Deploy.
4. You'll get a URL like `diya-portfolio.vercel.app`. Rename it under Settings → Domains if you want something like `diyamohan.vercel.app`.

**Option B: from your terminal**
```
npm i -g vercel
cd diya-portfolio
vercel        # first time: log in, accept defaults
vercel --prod
```

## Editing
- All text lives in `index.html`. Search for the section ids: `about`, `work`, `projects`, `stack`, `outside`, `contact`.
- Add GitHub: find the commented-out `github` link in the contact section, put in your username, and remove the `<!-- -->`.
- New project: copy one `<article class="proj">` block. Status pill options: `in progress`, `shipped`, or use `state soon` for upcoming.
- `src/body.html` is the same page without the `<head>` wrapper (used for the Claude preview). You can ignore it.
