# Modern Palette 1000

A public, framework-agnostic color system for websites and applications.

**1000 unique colors · 40 families · 25 shades per family · 250 four-color themes · 10 theme categories · MIT**

## Files

- `modern-palette.css` — all colors + all themes.
- `modern-palette.min.css` — minified all-in-one build.
- `colors.css` — the 1000 colors only.
- `themes.css` — the 250 themes only.
- `palette.json` — machine-readable colors and themes.
- `preview.html` — offline visual browser; click a swatch to copy it.
- `VALIDATION.txt` — generated integrity report.
- `LICENSE` — MIT License.

## Quick start

```html
<link rel="stylesheet" href="modern-palette.css">
```

```css
.card {
  background: var(--mp-snow-050);
  color: var(--mp-slate-900);
  border-color: var(--mp-gray-200);
}

.button {
  background: var(--mp-royal-blue-700);
  color: var(--mp-white);
}
```

## Naming

`--mp-{family}-{shade}`

Examples:

```css
var(--mp-red-500)
var(--mp-blue-700)
var(--mp-royal-blue-800)
var(--mp-black-950)
var(--mp-emerald-700)
var(--mp-gold-500)
```

Every family uses the same 25 shade labels:

`025, 050, 075, 100, 150, 200, 250, 300, 350, 400, 450, 500, 550, 600, 650, 700, 750, 800, 825, 850, 875, 900, 925, 950, 975`

Lower = lighter. Higher = darker.

## Families

Snow/White, Ivory, Gray, Zinc, Slate, Charcoal, Black/Onyx, Taupe, Stone, Sand, Cream, Brown, Cocoa, Red, Crimson, Burgundy/Wine, Rose, Pink, Coral, Orange, Amber, Yellow, Lime, Olive, Sage, Green, Emerald, Mint, Teal, Cyan, Aqua, Sky, Blue, Royal Blue, Navy/Midnight, Indigo, Violet, Purple/Royal Purple, Mauve, Gold/Champagne.

## Themes

Every theme contains exactly four tokens:

```css
--mp-theme-bg
--mp-theme-surface
--mp-theme-primary
--mp-theme-accent
```

Use:

```html
<body class="mp-theme-luxury-01">
```

```css
body { background: var(--mp-theme-bg); }
.card { background: var(--mp-theme-surface); }
.button { background: var(--mp-theme-primary); }
.badge { background: var(--mp-theme-accent); }
```

Categories: Light, Dark, Luxury, Royal, Corporate, Soft/Calm, Earthy, Ocean, Warm, Creative.

There are 25 themes per category = **250 themes**.

### Design rule

Themes contain no standalone HEX colors. Every theme slot references one of the 1000 palette variables.

## Offline preview

Open `preview.html`. No internet or external dependency is required.

## العربية

مكتبة ألوان عامة للمواقع والتطبيقات:
- 1000 لون فريد.
- 40 عائلة لونية.
- 25 درجة لكل عائلة.
- 250 ثيمًا جاهزًا.
- كل ثيم 4 ألوان فقط من مكتبة الألف لون.
- ألوان أساسية وهادئة وداكنة وملكية وفاخرة وترابية وبحرية.
- تعمل دون مكتبات خارجية.
- MIT للاستخدام والنشر العام.

## License

MIT

## Accessibility

The theme mixes are color palettes, not automatic WCAG guarantees. Before using any pair for body text, controls, or critical status indicators, validate the final foreground/background contrast for the intended font size and interface context.

## Contributing

Contributions are welcome. Please preserve the naming system, avoid duplicate HEX values, and keep theme colors referenced from the core 1000-color palette.
