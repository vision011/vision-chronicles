# Vision Chronicles

A personal video blog. Static site, $0 to run: videos are uploaded as unlisted
YouTube videos and embedded via iframe, so YouTube covers storage and
bandwidth. The page itself is plain HTML/CSS.

## Structure

- `index.html` — the whole site (layout + styles, single file)

## Running it locally

Just open `index.html` in a browser. No build step, no server required.

## Adding a new post

1. Upload your video to YouTube as **Unlisted**.
2. Copy the video ID from the URL (`youtube.com/watch?v=VIDEO_ID`).
3. Duplicate a `<article class="card">` block in `index.html`, swap in the
   new `iframe src="https://www.youtube.com/embed/VIDEO_ID"`, and update the
   tag, date, title, and description.

## Deploying for free

Push this repo to GitHub, then enable one of:

- **GitHub Pages** — Settings → Pages → deploy from the `main` branch
- **Cloudflare Pages** — connect the repo, no build command needed
- **Netlify** — drag-and-drop the folder or connect the repo

A custom domain (optional) typically runs $10–15/year on top of the free hosting.

## Roadmap ideas

- Swap placeholder posts for real videos
- Add working category filters (currently visual only)
- Move post data into a JSON/Markdown file instead of hardcoded HTML
- Add an RSS feed
