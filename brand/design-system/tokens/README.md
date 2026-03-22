# Design Tokens

## CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --bg: #000;
  --card: #0a0a0a;
  --elevated: #111;
  --hover: #181818;

  /* Text */
  --text: #f5f5f5;
  --sub: #737373;
  --muted: #444;

  /* Borders */
  --border: #1a1a1a;

  /* Brand Spectrum (shapes only — NEVER text) */
  --ember: #FF6B2B;
  --flare: #FF2255;
  --magenta: #CC00AA;
  --orchid: #8844FF;
  --arc: #4488FF;
  --cyan: #00D4FF;

  /* Gradient */
  --grad: linear-gradient(90deg, #FF6B2B, #FF2255, #CC00AA, #8844FF, #4488FF, #00D4FF);

  /* Typography */
  --sg: 'Space Grotesk', sans-serif;
  --jb: 'JetBrains Mono', monospace;
  --in: 'Inter', sans-serif;

  /* Border Radius */
  --radius-sm: 4px;   /* badges */
  --radius: 6px;      /* buttons, inputs */
  --radius-md: 8px;   /* large buttons */
  --radius-lg: 10px;  /* cards, nav */
}
```

## The Two Laws of Text

1. **Text is ONLY white or black** — no colored text ever
2. **Black text = white background, White text = black background**

## Border Radius by Component

| Component | Radius |
|-----------|--------|
| Cards | 10px |
| Buttons | 6px (sm: 5px, lg: 8px) |
| Inputs | 6px |
| Badges | 4px |
| Nav bar | 10px |
| Avatars | 50% |
| Dots | 50% |
| Dividers | 1-2px |

→ [Components](../components/)
→ [Colors](../../colors/)
→ [Typography](../../typography/)
