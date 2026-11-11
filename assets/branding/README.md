# Create Your First App — Brand Assets

Identity for **Create Your First App (CYFA)**, an open-source toolkit that helps beginners build applications with AI coding agents and helps experienced developers move faster.

## The symbol

| Element | Meaning |
| --- | --- |
| `〈 〉` angle brackets | Code and the developer's craft. Wide, open brackets also read as a shared workspace: open-source collaboration. |
| Rounded square tile | The application: a finished, tappable thing taking shape from an idea. Its soft corners echo app icons. |
| Upward chevron (negative space) | Progression and building. It is cut out of the tile, so the symbol keeps its meaning in one colour. The upward cue also stands for the learner levelling up and AI-assisted acceleration. |

Everything sits on a 64 × 64 grid. The brackets share one stroke weight, the tile is centred on the grid, and the chevron is cut out with `fill-rule="evenodd"`, so no masks, filters or gradients are needed.

## Color palette

| Name | HEX | Role |
| --- | --- | --- |
| Deep Navy | `#101426` | Wordmark and monochrome logo on light backgrounds; dark surfaces |
| Electric Violet | `#7257F5` | Application tile (primary accent) |
| Blue | `#4388F5` | Code brackets |
| White | `#FFFFFF` | Wordmark on dark backgrounds |
| Violet (dark-mode tint) | `#8A73FF` | Tile in `logo-light.svg` |
| Blue (dark-mode tint) | `#5C9DFF` | Brackets in `logo-light.svg` |

Measured contrast (WCAG): violet on white 4.8:1, blue on white 3.5:1, navy on white 18.3:1, violet on navy 3.8:1, blue on navy 5.3:1. Graphic marks need 3:1; the dark-mode tints raise the symbol to 5.2:1 and 6.7:1 on navy.

## Assets

| File | Use |
| --- | --- |
| `logo.svg` | Default horizontal logo (symbol + wordmark) for light backgrounds. Same artwork as `logo-dark.svg`. |
| `logo-dark.svg` | Horizontal logo with **dark text**, for **light** backgrounds. |
| `logo-light.svg` | Horizontal logo with **white text**, for **dark** backgrounds. |
| `logo-monochrome.svg` | Single colour (`#101426`). Stamps, one-colour print, watermarks. To recolour, replace every `#101426`. |
| `logo-icon.svg` | Standalone symbol. Avatars, app icons, social profile images. Works on light and dark backgrounds. |
| `favicon.svg` | Symbol with heavier brackets and a larger tile, tuned for 16–32 px. Works on light and dark browser tabs. |

All SVGs are self-contained with transparent backgrounds: no raster images, no filters, no external fonts. The wordmark is outlined to paths from Inter SemiBold (SIL Open Font License).

## Recommended sizes

| Placement | Asset | Size |
| --- | --- | --- |
| GitHub README header | `logo-dark.svg` / `logo-light.svg` | 320–400 px wide |
| Website navigation | `logo.svg` | 28–40 px tall (about 200–285 px wide) |
| Social avatar / app icon | `logo-icon.svg` | 512 × 512, with padding if the platform crops to a circle |
| Favicon | `favicon.svg` | scalable; checked at 16, 32 and 64 px |
| Minimum full logo | any horizontal logo | 24 px tall |
| Minimum icon | `logo-icon.svg` | 24 px (use `favicon.svg` below that) |

Keep clear space around the logo equal to the tile's width (20 units of the 64-unit grid). Do not stretch, rotate, add effects, or change the colours of individual parts.

## Usage examples

**GitHub README (follows the viewer's light/dark theme):**

```html
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/branding/logo-light.svg">
    <img alt="Create Your First App" src="assets/branding/logo-dark.svg" width="360">
  </picture>
</p>
```

**Plain Markdown:**

```markdown
![Create Your First App](assets/branding/logo-dark.svg)
```

**Website navigation:**

```html
<a href="/"><img src="/assets/branding/logo.svg" alt="Create Your First App" height="36"></a>
```

**Favicon:**

```html
<link rel="icon" type="image/svg+xml" href="/assets/branding/favicon.svg">
```
