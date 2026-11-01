# Helix — CSS motion component

## Files

- [helix-motion.html](helix-motion.html): reusable component markup.
- [helix-motion.css](helix-motion.css): scoped CSS animation.
- [preview.html](preview.html): standalone browser preview.

The component uses CSS for motion and inline SVG for the static ELI lettering. It requires no JavaScript, external fonts, or SMIL. Its background is transparent and its proportions adapt to the container width.

## Integration

Load `helix-motion.css` in the page head and insert the contents of `helix-motion.html` into the page.

```html
<link rel="stylesheet" href="helix-motion.css">
<!-- Insert the markup from helix-motion.html here. -->
```

Open `preview.html` in a browser to see the complete example.

## Behavior

HELIX holds, compresses horizontally into HX, holds as the symbol, and expands back. ELI fades early in the contraction and reappears late in the expansion. A damped horizontal bounce settles the mark without changing its height.

Both states use the same 100-unit visible cap height. The final HX geometry matches the approved [symbol](../logos/symbols/helix-symbol-ink.svg). The inline ELI outlines use the same 28-unit stems as the masters. A shared interpolated CSS progress property controls the compression, fade and polygon vertices; the sampled damped bounce keeps a constant cap height.

`prefers-reduced-motion` disables animation and shows the final HX symbol.

| CSS variable on `.helix-motion` | Default |
| --- | --- |
| `--helix-ink` | `#292c29` |
| `--helix-duration` | `4s` |
| `--helix-delay` | `.3s` |

## Landing integration

The sibling landing project uses copied motion styles plus its own `navigation.css` and `navigation.js` for scroll-triggered motion. That navbar variant is not the repeating preview in this folder. The landing hero uses a static HX image.

## History

Earlier SVG animations, snapshots, and motion samples are preserved in [archive/animation](../archive/animation/). The current spring is reconstructed from the reference, not extracted from its original source code.
