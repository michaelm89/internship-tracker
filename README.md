# Summer 2027 internship tracker

A single-page dashboard. Everything (layout, logic, data) lives in `index.html`. No build step, no server.

## Put it on GitHub Pages

1. Create a new repository on github.com (for example `internship-tracker`).
2. Upload `index.html` and this `README.md` to the repository root (Add file > Upload files > Commit).
3. Open Settings > Pages. Under "Build and deployment", set Source to "Deploy from a branch", pick `main` and `/ (root)`, then Save.
4. After a minute the site is live at `https://<your-username>.github.io/internship-tracker/`.

## Privacy

A GitHub Pages site is public to anyone with the link, even when the repository is private (private-repo Pages also needs a paid plan). The page asks search engines not to index it and contains no contact details, but the fit notes do describe your resume. If that matters, keep the file local and open it in a browser instead; it works the same way offline.

## How it stores your changes

Statuses and notes you set are saved in the browser you used (localStorage). They are not written back to GitHub. Use "Back up my statuses" to download a small JSON file, and "Restore from backup" on another device. "Download CSV" exports every role with your statuses, which opens in Excel.

## Updating the role list

The roles sit in one block inside `index.html`, between the comments `DATA: replace this block` and `END DATA`. Replace the JSON in that block with a refreshed list and commit. Each role keeps its saved status as long as its company, title, location and link are unchanged.
