# SQL Café

A free course that teaches SQL in eight short, friendly lessons, explained through a café menu.
Live at **https://learn.masshai.com**, made by [MASSH AI Services](https://masshai.com).

Each lesson has a story, a word-by-word code reader, an animated playground that runs real SQL in the browser, missions, a quiz and a pocket card.

| Lesson | Topic |
| --- | --- |
| 1 | SELECT, FROM, WHERE |
| 2 | ORDER BY, LIMIT |
| 3 | COUNT, SUM, AVG, MIN, MAX |
| 4 | GROUP BY, HAVING |
| 5 | JOIN, LEFT JOIN, IS NULL |
| 6 | INSERT, UPDATE, DELETE |
| 7 | CREATE TABLE, kinds of data, rules |
| 8 | Final project: ten café jobs and a certificate |

Everything runs in the browser. There is nothing to install and no data leaves the visitor's computer. Progress is saved in the visitor's own browser.

Want SQL or data training for your team? Please get in touch through [masshai.com](https://masshai.com/#contact).

---

## Publishing notes (for the owner)

### 1. Upload to GitHub
1. Create a new **public** repository called `sql-cafe`. Your existing portfolio repository is not affected.
2. Choose **uploading an existing file** and drag in every file from this folder: `index.html`, `lesson-1.html` to `lesson-8.html`, `README.md`, `CNAME`, `robots.txt`, `sitemap.xml` and `.nojekyll`.
3. Press **Commit changes**.
4. **Settings → Pages**: Source **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.

### 2. Point learn.masshai.com at it (Cloudflare)
1. Cloudflare dashboard → **masshai.com** → **DNS** → **Add record**.
2. Type **CNAME**, Name **learn**, Target **YOUR-GITHUB-USERNAME.github.io** (your username, not the repository name).
3. Set the cloud to **DNS only** (grey), not Proxied, then **Save**. Don't change any other records.
4. Back in GitHub: **Settings → Pages → Custom domain** should already show `learn.masshai.com` (from the `CNAME` file). Wait for the DNS check to pass, then tick **Enforce HTTPS**. This can take from a few minutes to a few hours.

### 3. Updating a lesson later
Lessons are edited in the `sql-cafe` folder. Run `build-site.ps1` there to rebuild this folder, then upload the changed files to the repository again.
