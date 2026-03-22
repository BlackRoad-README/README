# Components

## Card

```css
border: 1px solid var(--border);
border-radius: 10px;
padding: 28px;
background: var(--card); /* #0a0a0a */
```

Hover: `border-color: #333`
Gradient accent: `::before { height: 2px; background: var(--grad); }`

## Button

- **Solid:** `background: var(--text); color: #000; border-radius: 6px;`
- **Outline:** `border: 1px solid var(--border); background: transparent;`
- **Ghost:** `color: var(--muted); border: none;`

## Metric Cell

```css
.metric-value { font-size: 32px; font-weight: 700; }
.metric-label { font-family: var(--jb); font-size: 10px; opacity: .25; text-transform: uppercase; }
```

## Terminal Block

Gradient accent bar on top (3px). Traffic light dots (red/yellow/green). JetBrains Mono for all content.

## Pill/Tag

```css
border: 1px solid var(--border);
border-radius: 20px;
padding: 8px 18px;
font-size: 12px;
```

Decorative dot: 6px circle with gradient fill.

## Hero

Centered text, 120px top padding, orbs (blurred circles, 6% opacity), badge with gradient dot.

## Nav

Fixed, 52px height, gradient bar on top (4px), logo mark (circles + squares), links at 50% opacity.

## Footer

Border-top, flex space-between, brand + links + copyright.

## Ecosystem Bar

Fixed bottom, #0a0a0a background, JetBrains Mono 0.6rem links.

→ [Tokens](../tokens/)
→ [Patterns](../patterns/)
