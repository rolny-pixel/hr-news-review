# One-time setup (about 10 minutes)

The cloud agent updates this site every morning by committing a new file to GitHub. GitHub Pages then shows it at your own web address.

1. **GitHub account.** Sign in at https://github.com, or create a free account.
2. **New repository.** Click **+ → New repository**.
   - Name: `hr-news-review`
   - Visibility: **Public** (free GitHub Pages needs a public repo; the page is hidden from search engines, but anyone with the link can open it).
   - Tick **Add a README file**, then **Create repository**.
3. **Upload the files.** In the repo click **Add file → Upload files** and drag in everything from this folder:
   `index.html`, `PROFILE.md`, `SETUP.md` and the whole `editions` folder. Click **Commit changes**.
4. **Turn on the website.** Repo **Settings → Pages**. Under *Build and deployment* choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
   After a minute your page is at `https://<your-github-name>.github.io/hr-news-review/`.
5. **Let Claude write to the repo.** Install the Claude GitHub app: https://github.com/apps/claude → **Install** → *Only select repositories* → `hr-news-review`.
6. **Gmail.** Check that Gmail is connected at https://claude.ai/customize/connectors.
7. Send Claude the repository link (for example `https://github.com/yourname/hr-news-review`). Claude then creates the 7:00 routine.
