# Decoy Studio

A browser-based social post designer built specifically for **Mixfont’s Decoy Font**, an experimental COLR color font that combines high-frequency outlined decoy letters with a low-frequency hidden message.

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

## Font research

Decoy Font was released by Mixfont in 2026 as a hybrid-image typography experiment. Its thin high-frequency outline layer shows decoy letters up close, while the low-frequency blurred mass resolves into the typed message from farther away or while squinting. The TTF uses COLR/CPAL color-font tables and contextual substitutions so repeated letters can rotate through different decoys.

The encoded character set is intentionally focused: A–Z, a–z, spaces, and a non-breaking space. Decoy Studio filters unsupported characters from the Decoy layer while allowing punctuation in the ordinary kicker and footer text. The font works best on light backgrounds.

The app loads the official font file from Mixfont’s CDN. Decoy Font is free for personal, commercial, and client projects under its published DejaVu-derived license.

- Experiment: https://www.mixfont.com/experiments/decoy-font
- Font license: https://www.mixfont.com/experiments/decoy-font/DecoyFont-LICENSE.txt
- Font file: https://static.mixfont.com/assets/20260714-232642-decoyfont-htoqkd3x.ttf

Decoy Font may confuse casual OCR or visual extraction, but it is not encryption and should not be used as a security boundary.

## Application license

The application code in this repository is released under the MIT License.
