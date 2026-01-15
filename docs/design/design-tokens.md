# ShouldI Design Tokens

Design specifications from Tim's email for the ShouldI marketing website.

---

## Colors

Use these exact values:

| Token | Value | Usage |
|-------|-------|-------|
| Background | `#F7F8FA` | Page background |
| Surface | `#FFFFFF` | Cards, elevated elements |
| Text | `#111827` | Primary text |
| Text muted | `#6B7280` | Secondary/supporting text |
| Border | `#E5E7EB` | Dividers, borders |
| Accent teal | `#0E7490` | **CTAs only** |

---

## Typography

**Font Family:** Inter (single family throughout)

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Hero | 72px | 700 | 1.1 |
| H2 | 48px | 700 | 1.1 |
| H3 | 20px | 600 | 1.1 |
| Body | 16px | 400 | 1.6 |

---

## Spacing

| Property | Desktop | Mobile |
|----------|---------|--------|
| Section padding (vertical) | 160px | 80px |
| Container padding (horizontal) | 48px | — |
| Max content width | 1280px | — |

---

## Visual Direction

Reference sites (copy the level of **restraint**, not the templates):

### Stripe (5 screenshots)
- [Hero](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/stripe_1_hero.png)
- [Features](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/stripe_2_features.png)
- [Analytics](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/stripe_3_analytics.png)
- [More](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/stripe_4_more.png)
- [Footer](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/stripe_5_footer.png)

### Linear (3 screenshots)
- [Hero](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/linear_1_hero.png)
- [Features](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/linear_2_features.png)
- [More](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/linear_3_more.png)

### Basecamp (2 screenshots)
- [Hero](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/basecamp_1_hero.png)
- [Content](file:///Users/bintangputra/Downloads/websitebrief/docs/design/references/basecamp_2_content.png)

> "Build Should-I with Stripe's restraint, Linear's simplicity, and Basecamp's editorial calm — if anything feels flashy or clever, remove it."


---

## Visual Rules

- White/off-white background, dark text
- One teal accent only for primary CTAs + key emphasis
- Big readable typography, generous spacing
- Single-column scroll, minimal visuals, no gimmicks/animations
- **No dark mode**
- **No gradients**

---

## CSS Variables Reference

```css
:root {
  /* Colors */
  --bg: #F7F8FA;              /* Background */
  --surface: #FFFFFF;         /* Cards/frames */
  --text: #111827;            /* Body text */
  --text-muted: #6B7280;      /* Secondary text */
  --border: #E5E7EB;          /* Dividers */
  --accent: #0E7490;          /* CTAs only - use sparingly */
 
  /* Typography */
  /* Import Inter via Google Fonts or local asset */
  --font-family: 'Inter', system-ui, sans-serif;
  --fs-hero: clamp(40px, 6vw, 72px);     /* Hero headlines - responsive */
  --fs-h2: 48px;              /* Section headlines */
  --fs-h3: 20px;              /* Sub-headlines */
  --fs-body: 16px;            /* Body text */
 
  /* Spacing */
  --section-padding: 160px;   /* Vertical space between sections (desktop) */
  --section-padding-mobile: 80px;
  --container-max: 1280px;    /* Max content width */
  --container-padding: 48px;  /* Horizontal padding */
}
```
