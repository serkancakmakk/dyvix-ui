---
title: Marquee overrides
---

# Marquee overrides

Marquee style overrides represent a set of typed CSS Variables that allow easier control for the developer rather than using normal styling.

## Usage

```tsx
<DyvixMarquee
  overrides={{
    '--dyvix-marquee-bg': 'rgba(15, 10, 30, 0.75)',
    '--dyvix-marquee-color': '#f3e8ff',
    '--dyvix-marquee-gap': '2rem',
    '--dyvix-marquee-font-size': '0.92rem',
    '--dyvix-marquee-border-color': 'rgba(217, 70, 239, 0.3)',
    '--dyvix-marquee-box-shadow': '0 0 15px rgba(168, 85, 247, 0.15)',
    '--dyvix-marquee-hover-bg': 'rgba(30, 15, 50, 0.9)',
    '--dyvix-marquee-hover-color': '#38bdf8',
    '--dyvix-marquee-hover-border-color': 'rgba(56, 189, 248, 0.6)',
    '--dyvix-marquee-hover-box-shadow': '0 0 20px rgba(56, 189, 248, 0.35)'
  }}
  items={[
    { label: 'Feature One', href: '/features' },
    { label: 'Documentation' }
  ]}
/>
```

## Available Overrides

- `--dyvix-marquee-padding`: `8px 16px || 10px 22px || 12px 24px || string`
- `--dyvix-marquee-gap`: `100px || 1rem || string`
- `--dyvix-marquee-color`: `color || string`
- `--dyvix-marquee-letter-spacing`: `-0.02em || -0.01em || 0em || string`
- `--dyvix-marquee-border-width`: `0px || 1px || 2px || string`
- `--dyvix-marquee-border-style`: `solid || dashed || dotted || double || none || string`
- `--dyvix-marquee-border-radius`: `0px || 4px || 6px || 8px || 9999px || string`
- `--dyvix-marquee-transition`: `string || none`
- `--dyvix-marquee-hover-color`: `color || string`
- `--dyvix-marquee-hover-transform`: `none || translateY(-1px) || scale(1.02) || string`
- `--dyvix-marquee-hover-border-width`: `0px || 1px || 2px || string`
- `--dyvix-marquee-hover-border-style`: `solid || dashed || string || none`
- `--dyvix-marquee-hover-border-radius`: `0px || 4px || 6px || 8px || 9999px || string`
- `--dyvix-marquee-bg`: `color || transparent || string`
- `--dyvix-marquee-font-family`: `Geist || system-ui || monospace || string`
- `--dyvix-marquee-font-size`: `0.875rem || 0.9rem || 1rem || 1.125rem || string`
- `--dyvix-marquee-font-weight`: `400 || 500 || 600 || 700 || string`
- `--dyvix-marquee-border-color`: `color || transparent`
- `--dyvix-marquee-box-shadow`: `none || inset 0 1px 0 0 rgba(255, 255, 255, 0.05) || string`
- `--dyvix-marquee-hover-bg`: `color || transparent || string`
- `--dyvix-marquee-hover-border-color`: `color || transparent`
- `--dyvix-marquee-hover-box-shadow`: `none || 0 4px 12px rgba(0, 0, 0, 0.5) || string`
- `--dyvix-marquee-width`: `fit-content || 100% || auto || string`
- `--dyvix-marquee-height`: `fit-content || 100% || auto || string`
- `--dyvix-marquee-mask-image`: `string || none`
- `--dyvix-marquee-display`: `inline-block || block || inline-flex || flex || inline || grid || none || string`
