# Tribu — logo guidelines (compact)

## 1. The logo

**Idea:** the seal of acceptance. SUNAT answers an accepted Document with a CDR; the mark turns that stamp into the brand. The stepped T reads as an Andean chakana without drawing one literally, and the clay diamond is the dot of the `i` — the one warm detail.

**Versions**

| Version | Use |
|---|---|
| Horizontal (`tribu-horizontal.svg`) | Primary. README, website header, docs, email signature |
| Stacked (`tribu-stacked.svg`) | Square or narrow spaces, covers, stickers |
| Symbol (`tribu-symbol.svg`) | App icon, avatar, favicon, one-line contexts |
| Wordmark (`tribu-wordmark.svg`) | When the seal is already present nearby |

All masters are SVG, outlined, and have no live text. RGB files for screens; for print, use the SVG or a PDF exported from it and proof the CMYK values below.

## 2. Clear space

Keep **1 × the width of the T stem** clear on every side. In the 256-unit master that is **40 units** (15.6% of the symbol's height). The clear space scales with the logo; never use a fixed millimetre value.

Do not place text, rules, other logos, or a crop edge inside that zone. On a busy photo, put the lockup in a solid Sand container instead of shrinking the clear space.

## 3. Minimum size

| Version | Screen | Print |
|---|---|---|
| Horizontal | 120 px wide | 35 mm wide |
| Stacked | 96 px wide | 28 mm wide |
| Wordmark | 80 px wide | 24 mm wide |
| Symbol | 24 px | 8 mm |
| Symbol, small cut | 16 px | 5 mm |

Below 24 px use `tribu-symbol-small.svg` (or `web/favicon.svg`), where the T hole is drawn bolder. Do not use the horizontal or stacked lockup below its minimum; switch to the symbol.

## 4. Colour

| Name | HEX | RGB | CMYK (approx.) | Role |
|---|---|---|---|---|
| Seal | `#0F4C46` | 15 76 70 | 80 0 8 70 | Primary; symbol, wordmark, large surfaces |
| Clay | `#B5502F` | 181 80 47 | 0 56 74 29 | Accent; the i-diamond, highlights, links |
| Ink | `#14211F` | 20 33 31 | 39 0 6 87 | Body text, dark surfaces |
| Sand | `#F4EFE7` | 244 239 231 | 0 2 5 4 | Warm paper background, app icon tile |
| White | `#FFFFFF` | 255 255 255 | 0 0 0 0 | Paper, reversed text |

CMYK values are conversions from RGB, not a certified print match; proof against a physical swatch before a large print run. No official Pantone number is assigned — match to the HEX under D50.

**Contrast:** Seal on White 9.8:1 · Ink on White 16.6:1 · Clay on White 5.1:1 · Clay on Sand 4.4:1 (use Ink, not Clay, for small text on Sand).

**Approved pairs**

- Seal on White or Sand (primary).
- White on Seal or Ink (reversed).
- Black on White (one-colour print).
- Seal mono on White or Sand (one-colour brand).
- On photos: White on a calm area, or the Seal lockup inside a Sand container.

Do not put Seal on Clay; the contrast is too low. Do not use Clay as the background for the seal.

## 5. Typography

- **Wordmark:** Manrope 700, outlined in the SVG. You do not need the font to use the logo.
- **Headlines / UI:** Manrope 600–700. **Body:** the system sans stack: `ui-sans-serif, system-ui, -apple-system, "Segoe UI", sans-serif`.
- **Licence:** Manrope is SIL Open Font License 1.1. The wordmark is a custom outline and is not redistributed as a font.

Never retype the wordmark; always place the SVG. If Manrope is unavailable in a document, use the system stack for text, but keep the wordmark as artwork.

## 6. Don'ts

- Don't stretch, squash, rotate, skew, or crop the lockup.
- Don't add outlines, shadows, glows, gradients, bevels, or transparency.
- Don't change the T hole, the step at its foot, or the diamond i-dot.
- Don't replace the diamond with a round or square dot.
- Don't recolour outside the palette; don't make the diamond a second colour in the one-colour versions.
- Don't rearrange the symbol and wordmark, or resize one without the other.
- Don't place the seal on a busy photo without a container.
- Don't rebuild the wordmark by typing it in Manrope or any other font.

## 7. GitHub

The canonical files live in the public [`tribu-pe/brand`](https://github.com/tribu-pe/brand) repository.

- **Organization avatar:** `github/avatar-512.png`. Upload it in the organization profile settings. GitHub crops it to a circle.
- **Repository social preview:** `github/social-tribu-1280x640.png` for `tribu-pe/tribu` and `github/social-pdf-1280x640.png` for `tribu-pe/pdf`. GitHub recommends 1280×640, PNG/JPG, under 1 MB. Upload it in each repository's settings.
- **README header:** place the horizontal lockup at 320 px above the H1, with the white variant for dark mode:

```html
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tribu-pe/brand/main/logo/tribu-horizontal-white.svg">
    <img src="https://raw.githubusercontent.com/tribu-pe/brand/main/logo/variants/tribu-horizontal-color-1200.png" alt="Tribu" width="320">
  </picture>
</p>
```

The `tribu-pe/.github` repository uses the same header in `profile/README.md`.

## 8. Files

```
brand/
  logo/
    tribu-symbol.svg          standard symbol (Seal)
    tribu-symbol-small.svg    bolder T hole, for 16–23 px
    tribu-wordmark.svg        wordmark only
    tribu-horizontal.svg      primary lockup
    tribu-stacked.svg         stacked lockup
    variants/                 black, white, mono, square, favicon, app icon, PNGs
  web/                        favicon.ico/svg, apple-touch, 192/512, maskable, manifest, head snippet
  github/                     avatar, social previews and their SVG sources
  presentation/               final board and slide PNGs
  guidelines.md
  README.md
  TRADEMARK.md
```

**Web:** copy `web/favicon.ico`, `web/favicon.svg`, `web/apple-touch-icon.png`, `web/icon-192.png`, `web/icon-512.png`, `web/maskable-512.png` and `web/site.webmanifest` to the site root. The `<head>` snippet is in `web/head-snippet.html`.

**App icon:** `logo/variants/tribu-symbol-app-icon.svg` is the Sand tile with the Seal. Use it for the PWA icon; the GitHub avatar is `github/avatar-512.png`.

Questions or a new use case: open an issue in the repository.
