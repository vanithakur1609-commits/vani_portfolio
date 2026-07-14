# Learning in Progress — Vani Kumari

A five-page static site: Home, About, Now, Notes, Projects. Plain HTML/CSS, no build step.

## Before you publish — things to fill in

Search each file for square brackets and replace them:

- **Every page's footer**: `[yoursubstack]` → your real Substack handle, `[email protected]` → your real email
- **about.html / now.html**: `[add date when you publish]`
- **now.html**: the two `[Add: ...]` lines under Reading and Stuck on
- **projects.html**: the `[Add link...]` placeholders once you have URLs for write-ups or PDFs

## Publish free on GitHub Pages

1. Create a new **public** repo on GitHub — name it anything, e.g. `learning-in-progress`.
2. Upload all 6 files in this folder (`index.html`, `about.html`, `now.html`, `notes.html`, `projects.html`, `style.css`) to the repo root.
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch** → branch `main` → folder `/ (root)` → **Save**.
5. Wait ~1 minute. Your site is live at:
   `https://[your-github-username].github.io/learning-in-progress/`

## Adding a custom domain later (still free)

1. Buy a domain (e.g. from Namecheap or Google Domains) — this is the only cost in the whole setup.
2. In the repo, add a file named `CNAME` containing just your domain, e.g. `vanisharma.com`.
3. At your domain registrar, add a `CNAME` record pointing to `[your-username].github.io`.
4. Back in **Settings → Pages**, enter the custom domain and enable **Enforce HTTPS**.

## Adding a new Note or Project later

Copy one `<div class="card">...</div>` block in `notes.html` or `projects.html` and edit the text inside — no other file needs to change.
