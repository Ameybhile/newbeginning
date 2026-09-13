# Static site

Single page, no build step, no dependencies.

## Deploy to GitHub Pages
1. Create a repository. Pick a name that isn't guessable — it becomes the URL.
2. Copy `index.html` and the `img/` folder into it.
3. `git add . && git commit -m "init" && git push`
4. Settings -> Pages -> Source: `main` / root.
5. Live at `https://<user>.github.io/<repo>/` within a minute or two.

## Editing
- All copy is plain HTML in `index.html`. Search for the date headings to find each section.
- To swap a photo, replace the file in `img/` keeping the same filename, or change the `src`.
- Data that updates by itself (clocks, the running counter, the streak) lives in the
  `<script>` block at the bottom. `START` and `STREAK_ANCHOR` are the only two dates it needs.
- Fonts load from Google Fonts. Everything degrades to system serif/cursive if that's blocked.
