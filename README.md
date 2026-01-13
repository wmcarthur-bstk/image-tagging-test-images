# Image Tagging Test Images

This repo contains example images and curated image URLs for testing the Image Tagging / Image Analysis workflows.

## Repo structure

### `listing-images/`
- Contains **10,000+ real images** for broad testing (varied quality, angles, lighting, etc.).
- These are stored as normal image files in the repo.
- You can use them by:
  - Opening an image file in GitHub, then **Open image in new tab**, or
  - Right-clicking and selecting **Copy image address** (or “Copy image link”).

> Tip: When you copy the image address from GitHub, you’ll usually get a `raw` URL that can be used directly in tools like Postman or the Image Tagging API.

### `curated-urls/`
- Contains **plain text files** with **hand-picked image URLs**, grouped by:
  - **Category** (e.g., `interior`, `exterior`, `floorplan`, etc.)
  - **Sub-type** within the file (e.g., `kitchen`, `bathroom`, `bedroom`, etc.)
- Each sub-type typically includes **~10 URLs** designed to be fast, consistent test cases.

## Recommended usage

### Quick smoke tests (fast + consistent)
Use `curated-urls/`:
1. Pick a category file (e.g., `interior.txt`)
2. Copy 1–3 URLs from the sub-type you care about (e.g., `kitchen`)
3. Run them through your API / UI flow and verify expected tags and analysis output

### Broader coverage testing (lots of variety)
Use `listing-images/`:
- Grab a handful of images from different folders to simulate real-world uploads
- Useful for checking edge cases: low light, blurry, watermarking, weird angles, mixed rooms, etc.

## Notes
- URLs and images are intended for **internal testing**.
- If you find an image that’s especially useful (good example or a tricky edge case), consider adding it to the relevant file in `curated-urls/` so others can reuse it easily.
