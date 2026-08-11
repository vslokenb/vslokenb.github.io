# vslokenb.github.io

Personal site — plain HTML and CSS, no build step. Pushing to `main` publishes it
at https://vslokenb.github.io.

## Files

| File | What's in it |
| --- | --- |
| `index.html` | All page content. Edit the text directly. |
| `style.css` | All styling. The palette is six variables at the top. |
| `assets/photo-1.jpg` | Portrait beside the bio (placeholder — replace). |
| `assets/photo-2.jpg` | Wide photo below the intro (placeholder — replace, or delete the `<figure class="wide-photo">` block in `index.html` if you only want one photo). |
| `assets/cv.pdf` | The embedded CV (placeholder — replace with your own, same filename). |

## Customizing

**Photos.** Overwrite the two files in `assets/` keeping the same names. The
portrait is cropped to a 12 × 14.5 rem box and the wide photo to a max height of
26 rem, both via `object-fit: cover`, so any aspect ratio works — the crop is
centered. Resize to about 1600 px on the long edge before committing so the page
stays fast.

**CV.** Drop your PDF in as `assets/cv.pdf`. The page both embeds it and offers a
download link; mobile browsers that can't render an embedded PDF fall back to
the link automatically. Update the "Last updated" date in `index.html`.

**Recent / Elsewhere.** Copy any `<li>` in the `.updates` list or any
`<article class="link-card">` to add entries, delete them to remove. The link
grid reflows on its own.

**Colors.** Change the variables in the `:root` block at the top of `style.css` —
everything else derives from them.

**Font.** EB Garamond, loaded from Google Fonts in the `<head>`, with Garamond
and Times New Roman as fallbacks.

## Previewing locally

```bash
python3 -m http.server 4174
```

Then open http://localhost:4174.
