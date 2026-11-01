# Helix — Brand assets

**Crea con propósito.**

Damos forma a ideas que convierten lo complejo en nuevas posibilidades.

This repository contains the approved Helix identity, reusable logo assets, brand guidelines, and motion component. Helix is a software company based in Mexico, with initial products focused on healthcare and insurance and room to explore new categories, including games.

![Helix — HX symbol and HELIX wordmark](logos/horizontal/helix-logo-clay.svg)

## Start here

| Need | File |
| --- | --- |
| Primary horizontal logo | [Clay symbol + Ink wordmark](logos/horizontal/helix-logo-clay.svg) |
| Dark monochrome logo | [Ink horizontal logo](logos/horizontal/helix-logo-ink.svg) |
| Light monochrome logo | [Ivory horizontal logo](logos/horizontal/helix-logo-ivory.svg) |
| Standalone HX symbol | [Ink](logos/symbols/helix-symbol-ink.svg) · [Clay](logos/symbols/helix-symbol-clay.svg) · [Ivory](logos/symbols/helix-symbol-ivory.svg) |
| GitHub organization avatar | [1024 × 1024 PNG](social/github/helix-github-avatar.png) · [SVG source](social/github/helix-github-avatar.svg) |
| Brand guidelines | [Brand guide](guidelines/brand-guide.md) |
| Visual overview | [Brand board](guidelines/brand-board.svg) |
| CSS logo animation | [Implementation and usage](animation/README.md) |

## Repository structure

```text
branding/
├── README.md
├── .gitignore
├── logos/
│   ├── horizontal/         # Approved HX + HELIX compositions
│   └── symbols/            # Approved standalone HX symbol
├── guidelines/
│   ├── brand-guide.md
│   ├── brand-board.svg
│   └── symbol-preview.svg
├── social/
│   └── github/             # Organization avatar, PNG and SVG
├── animation/              # Current HTML/CSS component and preview
└── archive/
    ├── README.md
    ├── original-symbol/    # Original identity
    ├── explorations/       # Earlier logo and palette directions
    └── animation/          # Superseded motion studies and snapshots
```

## Identity essentials

- **Name:** Helix in running text; HELIX in the wordmark.
- **Tagline:** Crea con propósito.
- **Mission:** Damos forma a ideas que convierten lo complejo en nuevas posibilidades.
- **Character:** calm, curious, precise, and approachable.
- **Symbol:** the intertwined HX, with the diagonal cut through the H preserved.
- **Alignment:** HX and HELIX have the same visible height in horizontal compositions. The animation also preserves a constant height between states.

| Color | Hex | Role |
| --- | --- | --- |
| Ivory | `#F5F2EB` | Main background |
| Ink | `#292C29` | Text and monochrome marks |
| Clay | `#A45C47` | Primary brand accent |
| Sage | `#7E8B76` | Secondary decorative accent |
| Mist | `#E4E7DE` | Secondary surfaces |

## Using the assets

Use the SVG files for interfaces, websites, and scalable artwork. The logos are vector paths and do not require an installed typeface. Use the PNG avatar when a service requires a raster image.

Use Ink or Clay on light backgrounds and Ivory on dark backgrounds. Preserve the proportions, clear space, and transparent diagonal openings. Do not stretch, rotate, add outlines, or redraw the cuts. See the [brand guide](guidelines/brand-guide.md) for sizing and typography guidance.

## Motion

Open [`animation/preview.html`](animation/preview.html) in a browser to view the current CSS animation. It has a four-second cycle, horizontal accordion compression, and a damped bounce. It includes a reduced-motion fallback. The README explains how to integrate it.

The landing page is maintained separately in the sibling `landing/` folder. Its navbar uses a scroll-triggered version; its hero shows the static HX symbol. The landing is not part of this branding repository. Sync copied assets when changing the masters here.

## Maintaining the identity

1. Edit the approved masters in `logos/`.
2. Update the brand board and applicable social exports or motion geometry.
3. Check that HX and HELIX retain equal visible heights and that diagonal cuts remain open at small sizes.
4. Sync the landing's copied assets when needed.
5. Keep superseded designs in `archive/`; they are not production assets.

## Ownership

These assets represent the Helix brand. No open-source license is granted by this repository.

Target GitHub repository: [HX-Devs/branding](https://github.com/HX-Devs/branding).
