# BROJECTS — Franklin's Build Log

Personal hardware & DIY blog. Built with plain HTML/CSS, hosted free on GitHub Pages.

---

## File Structure

```
brojects/
├── index.html              ← Homepage (edit to add new posts here)
├── about.html              ← About page
├── css/
│   └── style.css           ← Shared styles for the whole site
├── posts/
│   ├── NEW-POST-TEMPLATE.html   ← Copy this for every new post
│   ├── raspberry-pi-nas.html
│   ├── laptop-capacitor.html
│   ├── smart-home-dashboard.html
│   └── mechanical-keyboard.html
└── README.md               ← This file
```

---

## How to Deploy (GitHub Pages — Free)

### First time setup

1. Go to [github.com](https://github.com) and create a free account
2. Click **New repository** → name it `brojects` → set to **Public** → click **Create**
3. Upload all these files (drag and drop into the repo, or use GitHub Desktop)
4. Go to **Settings → Pages**
5. Under **Source**, select `Deploy from a branch`
6. Choose `main` branch → `/ (root)` → click **Save**
7. Wait ~60 seconds → your site is live at:
   ```
   https://YOUR-USERNAME.github.io/brojects
   ```

### Every time you update the site

Just edit a file and upload the updated version to GitHub.
Or use Git from your terminal:
```bash
git add .
git commit -m "Added new post"
git push
```

---

## How to Write a New Post

1. Copy `posts/NEW-POST-TEMPLATE.html`
2. Rename it: `posts/my-new-build.html`
3. Open it and edit every section marked `<!-- EDIT -->`
4. Open `index.html` and add a new post card in the "Recent builds" section:

```html
<a class="post-card" href="posts/my-new-build.html">
  <div class="post-tag">
    <span class="tag">Hardware</span>
    <span class="tag">Your Tag</span>
  </div>
  <div class="post-title">My New Build Title</div>
  <div class="post-excerpt">Short description of the build.</div>
  <div class="post-meta">
    <span>Month DD, 2025 — X min read</span>
    <span class="read-more">Read build</span>
  </div>
</a>
```

5. Upload both files to GitHub → done.

---

## Free CMS Option (Netlify CMS)

If you want a browser-based editor instead of editing HTML by hand:

### Option A: Netlify (easiest)
1. Go to [netlify.com](https://netlify.com) → sign up free
2. Drag your project folder into the deploy dropzone
3. Your site gets a free `.netlify.app` URL
4. Enable **Netlify CMS** from the dashboard for a simple browser editor

### Option B: Tina CMS (free tier, works with GitHub Pages)
1. Go to [tina.io](https://tina.io) → connect your GitHub repo
2. Follow the setup wizard — it adds a `/admin` route to your site
3. Visit `yoursite.github.io/brojects/admin` to write posts in a visual editor

Both are free for personal use.

---

## Custom Domain (Optional)

If you buy a domain (e.g. `brojects.dev` — about $10/year on Namecheap):

1. In your GitHub repo → **Settings → Pages → Custom domain**
2. Type your domain and click Save
3. In your domain registrar's DNS settings, add:
   ```
   Type: CNAME
   Name: www
   Value: YOUR-USERNAME.github.io
   ```
4. Wait up to 24 hours for DNS to propagate → your site is live on your domain

---

## Editing Tips

- **Add/change tags**: Edit the `<span class="tag">` elements inside `.post-tag`
- **Featured post**: Add `class="post-card featured"` to any post card on index.html
- **Update stats**: Edit the numbers in the `<span class="stat-num">` elements
- **Update ticker**: Edit the text inside `.ticker-inner` in index.html
