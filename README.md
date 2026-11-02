# austintecks.info

Plain HTML + CSS. No build step, no framework.

```
index.html              home page (the list of works)
styles.css              all styling: colours, fonts, spacing
<work-slug>/index.html  one folder per page, so URLs match the old Canva site
assets/img/             logo, favicon, images
```

All videos are YouTube embeds.

## Editing

- **Change a caption or title:** open that work's `index.html` and edit the text.
- **Change colours or font:** edit the variables at the top of `styles.css`.
- **Add a work:** copy an existing work's folder, rename it, edit the text and media, then
  add a link to it in `index.html` and update the `back` / `next` links on its neighbours.
- **YouTube video:** the embed uses the video's ID, e.g. `youtube-nocookie.com/embed/WWiuHsedhUk`.

## Previewing locally

```bash
python3 -m http.server 8420
```

Then open http://localhost:8420.

## Hosting

Any static host works (GitHub Pages, Netlify, Cloudflare Pages). Upload the whole folder
and point the austintecks.info domain at it.
