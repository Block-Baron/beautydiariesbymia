# Beauty Diaries by Mia

Static single-file website for Beauty Diaries by Mia — step-by-step beauty tutorials behind the Pinterest pins: makeup, hairstyles, skincare, nails and outfits.

## Setup

- This is a static single-file site. There is no build step and no dependencies to install.
- To view it locally, open `index.html` in a browser.
- The live site is served via Vercel at https://beautydiariesbymia.vercel.app/

## How to add a new post

1. Add the post's 3 photos to `assets/`, continuing the numbering from img-150 onwards (img-150, img-151, img-152, and so on).
2. In `index.html`, add a new object to the `ARTICLES` array, first — at the top of the array, before the current first post — with the post's `id`, `title`, `category`, `cat`, `time`, `level`, `blurb`, `intro`, `images`, `needs`, `steps`, `tips` and `avoid` fields, and its Pinterest `pin` URL.
3. Move `newest: true` to the new post, and remove it from the previous newest post, so only the newest post carries it.
4. Set the category and `cat` mapping correctly: `category` is the display name and `cat` is the filter key. Use `Makeup Looks` / `makeup`, `Hairstyles` / `hair`, `Skincare & Glow` / `skincare`, `Nail Art Ideas` or `Manicure Inspiration` / `nails`, `Chic Fashion` or `Everyday Outfits` / `fashion`, or `Party & Date Night Looks` / `party`.
5. Check that the total `time` matches the sum of the step times, then commit.
