# Tribu brand

The seal of acceptance: a stepped T inside the double ring of a rubber stamp. The capsule is that seal stretched to hold the name, and the letters share the T's height, weight and curves.

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="logo/variants/tribu-horizontal-white.svg">
    <img src="logo/tribu-horizontal.svg" alt="Tribu" width="420">
  </picture>
</p>

These are the canonical brand files. [Guidelines](guidelines.md) explain how to use them; [TRADEMARK.md](TRADEMARK.md) explains what is allowed.

## Logo

### Capsule — primary

<img src="logo/tribu-horizontal.svg" alt="Tribu horizontal lockup" width="420">

### Stacked

<img src="logo/tribu-stacked.svg" alt="Tribu stacked lockup" width="220">

### Symbol

<img src="logo/tribu-symbol.svg" alt="Tribu symbol" width="96">

| Version | File | Use |
|---|---|---|
| Capsule (horizontal) | `logo/tribu-horizontal.svg` | README, website header, docs, email signature |
| Stacked | `logo/tribu-stacked.svg` | Seal over the wordmark, for square or narrow spaces, covers, stickers |
| Symbol | `logo/tribu-symbol.svg` | App icon, avatar, favicon, one-line contexts |
| Wordmark | `logo/tribu-wordmark.svg` | The name on its own, when the seal is used apart or is already nearby |
| Small symbol | `logo/tribu-symbol-small.svg` | 16–23 px; no inner ring and a bolder T |

`logo/variants/` holds black, white, mono, square, favicon and app-icon SVGs, plus PNGs.

## Colour

| Name | HEX | Role |
|---|---|---|
| Seal | `#0F4C46` | Primary; symbol, wordmark, large surfaces |
| Clay | `#B5502F` | Accent; highlights, links |
| Ink | `#14211F` | Body text, dark surfaces |
| Sand | `#F4EFE7` | Warm paper background, app icon tile |
| White | `#FFFFFF` | Paper, reversed text |

CMYK values and contrast pairs are in [guidelines.md](guidelines.md#4-colour).

## GitHub

| Asset | File | Use |
|---|---|---|
| Organization avatar | `github/avatar-512.png` | Upload in the organization profile settings. GitHub crops it to a circle. |
| `tribu` social preview | `github/social-tribu-1280x640.png` | Repository settings → Social preview. |
| `pdf` social preview | `github/social-pdf-1280x640.png` | Same; the preview is only shared from a public repository. |

The README header uses the horizontal lockup at 320 px, with the white variant for dark mode:

```html
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tribu-pe/brand/main/logo/variants/tribu-horizontal-white.svg">
    <img src="https://raw.githubusercontent.com/tribu-pe/brand/main/logo/variants/tribu-horizontal-color-1200.png" alt="Tribu" width="320">
  </picture>
</p>
```

The `tribu-pe/.github` repository uses the same header in `profile/README.md`.

## Web

`web/` contains `favicon.ico`, `favicon.svg`, the 16/32/48 PNGs, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `maskable-512.png`, `site.webmanifest` and `head-snippet.html`. Copy them to the site root.

## Presentation

`presentation/` contains the five-slide board (`tribu-board.html`) and its PNGs in `slides/`.

## Files

```text
brand/
  logo/
    tribu-symbol.svg          standard symbol (Seal)
    tribu-symbol-small.svg    no inner ring and a bolder T, for 16–23 px
    tribu-wordmark.svg        wordmark only
    tribu-horizontal.svg      capsule, the primary lockup
    tribu-stacked.svg         stacked lockup
    variants/                 black, white, mono, square, favicon, app icon, PNGs
  web/                        favicon.ico/svg, apple-touch, 192/512, maskable, manifest, head snippet
  github/                     avatar, social previews and their SVG sources
  presentation/               final board and slide PNGs
  guidelines.md
  README.md
  TRADEMARK.md
```
