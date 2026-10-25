# LQ PixelCraft

One browser app to prepare an image from start to finish:

- **Remove BG**: automatic AI cut-out, or a color eraser (tap the background; tolerance, soft edge, connected-only)
- **Touch-up brush**: erase or restore by hand (size, softness), with 2×–4× zoom and a Move mode for scrolling
- **Crop**: drag handles, with Free, 1:1, 4:3, 3:4, 16:9, 9:16
- **Resize / upscale**: ½× to 4× or exact width and height, with optional sharpening
- **Save**: PNG (keeps transparency) or JPEG (quality + fill color), Download or Share

Undo (last 8 steps), Reset to original, and preview on checker/white/black/green to check cut-out edges.

Everything runs on the device. The only network use is the one-time download of the background-removal model (cached afterwards).

## Publish (GitHub Pages)

1. Put `index.html` and your 180×180 icon named `lq-pixelcraft-icon.png` in the same repo folder.
2. Commit both files. Wait 1–2 minutes for Pages.
3. On iPhone: delete any old shortcut, quit Safari, open the page, Share → Add to Home Screen.

## Notes

- Images are capped at about 16 megapixels (iOS canvas limit). Upscaling beyond that is limited automatically.
- Upscaling is smooth multi-step scaling plus sharpening, not AI super-resolution.
- Automatic background removal uses `@imgly/background-removal` loaded from jsDelivr.
