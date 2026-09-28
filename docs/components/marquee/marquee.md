---
title: Dyvix Marquee
---

# Dyvix Marquee

DyvixMarquee is an animated Marquee component that supports both themed and unstyled rendering modes. It supports two usage patterns:

- **Config-driven mode** for rendering marquee from structured data.
- **Composable mode** for building fully custom marquee layouts using sub-components.

## Attributes

- `items`
  - : `Array<{ label: string, href?: string }>`. Defines marquee links displayed in config-driven mode.
- `children`
  - : `ReactNode`. Used in composable mode to manually build the marquee using `DyvixMarquee.Item` / `DyvixMarqueeItem`.
- `repeat`
  - : `number`. Defaults to `-1`. Identifies how many times to repeat the marquee loop.
- `speed`
  - : `number`. Defaults to `1`. Identifies the speed of the marquee loop.
- `pauseOnHover`
  - : `boolean`. Defaults to `false`. Pauses on hover if true.
- `overrides`
  - : `Record<string, string | number>`. An object of typed CSS Variables allowing easy-customization of the component. See [marquee overrides](/components/marquee/overrides.md) for more information.
- `theme`
  - : `string`. Controls the design and feel of the marquee. See the [Themes list](/guide/themes) for a full list.
- `animation`
  - : `string`. Controls the entrance animation of the marquee. Defaults to `fade`. See the [Animation List](/guide/animations) for a full list.
- `className`
  - : `string`. Contains a custom class for your marquee, allowing more control for the developer.
- `timeline`
  - : `function`. A GSAP callback function that allows an external `gsap.timeline()` instance to control the component's internal animations.

## Sub-components

Used exclusively in composable mode. Can be accessed as `<DyvixMarquee.Item>` or imported directly as `<DyvixMarqueeItem>`:

- `DyvixMarquee.Item` / `DyvixMarqueeItem`
  - : Represents the item to duplicate and showcase in the marquee. Accepts `children`, `className`, `href`, `onClick`, and `style`.

## Example

### Config-driven mode

```jsx
import { DyvixMarquee } from 'dyvix-ui';

function MarqueeExample() {
  return (
    <DyvixMarquee
      theme={'Singularity'}
      timeline={tl}
      repeat={1}
      items={[
        { label: 'Feature One', href: '/features' },
        { label: 'Documentation', href: '/docs' }
      ]}
    />
  );
}
```

### Composable mode

```jsx
import { DyvixMarquee, DyvixMarqueeItem } from 'dyvix-ui';

function MarqueeExample() {
  return (
    <DyvixMarquee pauseOnHover repeat={1} speed={2} theme={'Singularity'}>
      <DyvixMarqueeItem>Feature One</DyvixMarqueeItem>
      <DyvixMarqueeItem>Documentation</DyvixMarqueeItem>
    </DyvixMarquee>
  );
}
```
