# Decoy Studio

A focused browser-based post creator built for **Mixfont’s Decoy Font**. The tool produces clean social graphics containing only a Decoy Font message over a single solid background color.

## Simplified editor

- Solid-color backgrounds only — no gradients, patterns, grain, frames, shapes, headers, or footers
- Message-first workflow split into three clear tabs: Message, Canvas, and Type
- Instagram portrait, square, Story, wide, and fully custom canvas sizes
- Curated light background colors plus a custom color picker and HEX input
- Automatic warning when a background is too dark for the font’s black and gray layers
- Drag-to-position text, keyboard nudging, alignment, size, spacing, rotation, opacity, and auto-fit controls
- Edit, Step Back, and Squint preview modes for testing the optical effect
- Exact-resolution PNG export and clipboard copy
- Editable project save/load
- Responsive desktop and mobile layouts

## How Decoy Font works

Decoy Font is a hybrid-image type experiment released by Mixfont in 2026. It combines a high-frequency layer made from thin outlined decoy letters with a low-frequency blurred layer containing the real typed message. The outlines dominate nearby; the actual message becomes easier to read at a smaller scale, from farther away, or while squinting.

The font uses COLR/CPAL color-font tables and contextual substitutions. Repeated letters can cycle through different decoy forms. Its supported text is intentionally focused on A–Z, a–z, spaces, and line breaks, and it works best on light solid backgrounds.

Decoy Font can interfere with casual OCR or visual extraction, but it is not encryption and must not be used to protect sensitive information.

Original experiment: <https://www.mixfont.com/experiments/decoy-font>

## Run locally

No build step is required:

```bash
python -m http.server 4173
```

Then open `http://localhost:4173`.

## Validation

The current build was browser-tested for successful font loading, preset and custom canvas resizing, background-color updates, phrase insertion with line breaks, responsive mobile layout, and clean RGB PNG export at the exact selected dimensions.

## License

The application code is released under the MIT License. Decoy Font retains its original DejaVu-derived font license.
