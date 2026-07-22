# Decoy Studio

A browser-based social post designer built specifically for **Mixfont's Decoy Font**, an experimental COLR color font that combines high-frequency outlined decoy letters with a low-frequency hidden message.

## Features

- Instagram, Stories/Reels, X, LinkedIn, YouTube, presentation, and custom canvas sizes
- Six responsive art-direction templates
- Decoy Font message editing with unsupported-character feedback
- Drag-to-position, keyboard nudging, alignment, scale, tracking, rotation, and opacity controls
- Near / medium / far distance simulation and squint preview
- Safe-zone guides
- Exact-resolution PNG export and clipboard copy
- Save and load editable project JSON files
- Fully static and ready for Vercel

## Run locally

No build step is required. Serve the directory with any static server:

```bash
python -m http.server 4173
```

Then open `http://localhost:4173`.

## Font support and limitations

The included font is **Decoy Font Regular**, created by Mixfont in 2026. It uses COLR/CPAL color-font tables and contextual substitutions. Current Chromium, Safari, and Firefox releases provide the best experience.

The font's encoded character set is intentionally focused: A–Z, a–z, spaces, line breaks, and a non-breaking space. Decoy Studio filters unsupported characters from the Decoy layer while allowing punctuation in the ordinary kicker and footer text.

Decoy Font may confuse casual OCR or visual extraction, but it is not encryption and should not be used as a security boundary.

## License

Decoy Font is free to use, install, and share. Its letterforms derive from DejaVu Sans Mono and are distributed under the included license. See [`DecoyFont-LICENSE.txt`](./DecoyFont-LICENSE.txt).

The application code in this repository is released under the MIT License.
