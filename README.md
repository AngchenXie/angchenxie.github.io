# angchenxie.github.io

Personal website — a single hand-written static page, no build step.

```
index.html          all content lives here
assets/site.css     all styling
assets/img/         portrait, favicons, paper teasers (.mp4 + .jpg poster)
images/             originals the assets were derived from (not served)
assets/CV_*.pdf     CV
.nojekyll           tells GitHub Pages to serve the files as-is
```

Preview locally:

```sh
python3 -m http.server 8765   # then open http://localhost:8765
```

Adding a paper: copy an `<article class="card pub">` block in `index.html`,
swap the title/authors/venue/links, and drop a 5s muted `.mp4` teaser plus a
`.jpg` poster frame into `assets/img/`. Teasers load only when scrolled into
view, and are skipped entirely for visitors who prefer reduced motion.

The previous Academic Pages version of this site is preserved at the
`v1-academicpages` tag.
