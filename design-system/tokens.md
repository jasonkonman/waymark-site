# Waymark Design System Tokens

Quick reference for all Waymark design tokens. Copy the CSS variable names to use in your projects.

---

## Color Tokens

### Brand Colors

| Token | Light | Dark | CSS Variable | Usage |
|-------|-------|------|--------------|-------|
| Brand | `#2B7A5F` | `#3EBF8A` | `--wm-brand` | Primary color for headlines, CTAs, links, active states |
| Brand Soft | `#E8F5EE` | `#1A2E25` | `--wm-brand-soft` | Tinted backgrounds, light accents |

### Accent Colors (Saffron)

| Token | Light | Dark | CSS Variable | Usage |
|-------|-------|------|--------------|-------|
| Accent | `#E88639` | `#F0A05A` | `--wm-accent` | Secondary CTAs, highlights, badges |
| Accent Soft | `#FFF3E8` | `#2A2014` | `--wm-accent-soft` | Tinted backgrounds for accent elements |

### Surface Colors

| Token | Light | Dark | CSS Variable | Usage |
|-------|-------|------|--------------|-------|
| Surface | `#FAFCFD` | `#161818` | `--wm-surface` | Page background, default surface |
| Surface Elevated | `#FFFFFF` | `#1E2022` | `--wm-surface-elevated` | Cards, modals, elevated containers |
| Surface Grouped | `#F0F2F5` | `#111315` | `--wm-surface-grouped` | Section backgrounds, grouped content |

### Text Colors

| Token | Light | Dark | CSS Variable | Usage |
|-------|-------|------|--------------|-------|
| Text Primary | `#1A1D21` | `#F0F2F5` | `--wm-text-primary` | Body text, headlines, primary content |
| Text Secondary | `#6B7280` | `#9CA3AF` | `--wm-text-secondary` | Subtext, muted labels, descriptions |

### Borders & Dividers

| Token | Light | Dark | CSS Variable | Usage |
|-------|-------|------|--------------|-------|
| Border Subtle | `#E5E8EB` | `#374151` | `--wm-border-subtle` | Dividers, borders, subtle strokes |

### Semantic Colors

| Token | Light | Dark | CSS Variable | Usage |
|-------|-------|------|--------------|-------|
| Success | `#16A34A` | `#4ADE80` | `--wm-success` | Positive states, confirmations, "on track" |
| Warning | `#D97706` | `#FBBF24` | `--wm-warning` | Cautionary states, alerts, "off pace" |
| Danger | `#DC2626` | `#F87171` | `--wm-danger` | Errors, destructive actions, "failed" |
| Info | `#2563EB` | `#60A5FA` | `--wm-info` | Informational messages, "in progress" |

### Opacity Utilities

| Token | Value | CSS Variable | Usage |
|-------|-------|--------------|-------|
| Brand 12% | `rgba(43, 122, 95, 0.12)` | `--wm-brand-opacity-12` | Subtle tint backgrounds |
| Brand 18% | `rgba(43, 122, 95, 0.18)` | `--wm-brand-opacity-18` | Stronger tint backgrounds |
| Accent 12% | `rgba(232, 134, 57, 0.12)` | `--wm-accent-opacity-12` | Subtle accent tints |
| Accent 16% | `rgba(232, 134, 57, 0.16)` | `--wm-accent-opacity-16` | Stronger accent tints |

---

## Spacing Scale

All spacing is built on a 4px base grid.

| Token | Value | CSS Variable | Usage |
|-------|-------|--------------|-------|
| XS | 4px | `--wm-spacing-xs` | Tight spacing, gaps between related items |
| SM | 8px | `--wm-spacing-sm` | Small padding, icon spacing |
| MD | 12px | `--wm-spacing-md` | Standard component padding |
| LG | 16px | `--wm-spacing-lg` | Section padding, card padding |
| XL | 24px | `--wm-spacing-xl` | Section margins, major spacing |
| 2XL | 32px | `--wm-spacing-2xl` | Large section breaks, main layout gaps |

---

## Border Radius

| Token | Value | CSS Variable | Usage |
|-------|-------|--------------|-------|
| Small | 8px | `--wm-radius-sm` | Small components, icons |
| Medium | 12px | `--wm-radius-md` | Buttons, inputs, badges |
| Large | 16px | `--wm-radius-lg` | Cards, modals, large components |

---

## Shadows

| Token | Value | CSS Variable | Usage |
|-------|-------|--------------|-------|
| Card | `0 1px 3px rgba(0, 0, 0, 0.04)` | `--wm-shadow-card` | Subtle elevation for cards |

---

## Typography Scale

### Font Stack

```css
font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
```

### Font Sizes & Weights

| Role | Size | Weight | Line Height | CSS Variable | Usage |
|------|------|--------|-------------|--------------|-------|
| Headline | 28px | 700 | 1.3 | `--wm-font-headline` | Main page headings |
| Subheading | 15px | 600 | 1.4 | `--wm-font-subheading` | Section headings |
| Body | 16px | 500 | 1.5 | `--wm-font-body-semibold` | Body copy, standard text |
| Caption | 12px | 400 | 1.4 | `--wm-font-caption` | Labels, small text |
| Footnote | 13px | 400 | 1.4 | `--wm-font-footnote` | Fine print, metadata |

---

## Component Recipes

### Card / Container

```css
background: var(--wm-surface-elevated);
border-radius: var(--wm-radius-lg);
border: 1px solid var(--wm-border-subtle);
padding: var(--wm-spacing-lg);
box-shadow: var(--wm-shadow-card);
```

### Primary Button

```css
background: var(--wm-brand);
color: white;
padding: 12px var(--wm-spacing-xl);
border-radius: var(--wm-radius-md);
font-weight: 600;
```

### Badge / Pill

```css
background: var(--wm-accent-16%);
color: var(--wm-accent);
padding: 4px 8px;
border-radius: 12px;
font-weight: 600;
font-size: 12px;
```

### Progress Bar

```css
background: var(--wm-border-subtle);
height: 6px;
border-radius: 3px;
overflow: hidden;

/* Fill */
background: var(--wm-brand);
height: 100%;
```

### Empty State

```css
text-align: center;
padding: var(--wm-spacing-2xl) var(--wm-spacing-xl);
background: var(--wm-surface-grouped);
border-radius: var(--wm-radius-lg);
border: 1px dashed var(--wm-border-subtle);
```

### Text Link

```css
color: var(--wm-brand);
text-decoration: none;
transition: opacity 0.15s;
```

```css
/* Hover */
opacity: 0.8;
```

---

## Dark Mode

All tokens include dark mode variants. They automatically adapt via CSS media query:

```css
@media (prefers-color-scheme: dark) {
  :root {
    --wm-brand: #3EBF8A;
    --wm-text-primary: #F0F2F5;
    /* ... etc */
  }
}
```

No additional work needed — just use the CSS variable names.

---

## Implementation

### Web

```html
<link rel="stylesheet" href="path/to/_tokens.css">
```

Then reference in your CSS:

```css
.my-button {
  background: var(--wm-brand);
  color: white;
  padding: var(--wm-spacing-md);
  border-radius: var(--wm-radius-md);
}
```

### Light/Dark Mode Toggle

Use the theme toggle in the visual style guide (`design-system/index.html`). Or manually set:

```html
<html data-theme="dark">
```

---

## Notes

- All colors meet WCAG AA contrast requirements in light and dark modes
- Spacing values are multiples of 4px for consistency
- Use CSS variables for all color and spacing — never hardcode values
- Test component designs in both light and dark modes
- For new collateral projects, start by importing `_tokens.css` and referencing these variables

---

## Questions?

Refer to the visual style guide at `design-system/index.html` for rendered examples and usage patterns.
