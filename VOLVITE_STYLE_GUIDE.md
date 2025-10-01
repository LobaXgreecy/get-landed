# Volvite.ai - Comprehensive Style Guide

## 1. Color System

### Primary Colors
```css
--primary-black: #000000
--accent-orange: #fc5a35
--link-blue: #09f (bright blue)
```

### Background Colors
```css
--background-primary: #000000
--background-gradient-start: #01010100 (transparent black)
--background-gradient-end: #000000ab (semi-transparent black)
```

### Text Colors
```css
--text-primary: #ffffff (white)
--text-link: #09f
--text-muted: rgba(255, 255, 255, 0.7)
```

### Opacity Variants
- Full opacity backgrounds for solid sections
- Gradient overlays for depth and visual interest
- Semi-transparent borders and dividers

---

## 2. Typography

### Font Families
```css
--font-primary: 'DM Sans', 'Inter', -apple-system, BlinkMacSystemFont, sans-serif
```

### Font Weights
- 400 (Regular) - Body text
- 500 (Medium) - Sub-headings, emphasized text
- 600 (Semi-Bold) - Important labels
- 700 (Bold) - Section headings
- 900 (Black) - Hero headlines

### Font Sizes
```css
--font-size-base: 16px

/* Headings (Desktop) */
--h1-size: 56-72px
--h2-size: 40-48px
--h3-size: 32-36px
--h4-size: 24-28px
--h5-size: 20-22px
--h6-size: 18px

/* Body Text */
--body-large: 18px
--body-regular: 16px
--body-small: 14px
--caption: 12px
```

### Line Heights
```css
--line-height-tight: 1.2em (headings)
--line-height-normal: 1.5em (body text)
--line-height-relaxed: 1.8em (large paragraphs)
```

### Letter Spacing
```css
--letter-spacing-tight: -0.02em (large headings)
--letter-spacing-normal: 0em (body text)
--letter-spacing-wide: 0.05em (uppercase labels)
```

### Responsive Typography
- Desktop: Full scale (base 16px)
- Tablet (810-1199px): 90% scale
- Mobile (<809px): 80-85% scale

---

## 3. Header Components

### Logo Style
```css
.logo {
  /* Logo appears to be text or SVG based */
  display: flex;
  align-items: center;
  font-weight: 700;
  color: #ffffff;
}
```

### Navigation Menu
```css
.navigation {
  display: flex;
  align-items: center;
  gap: 30px;
  font-size: 16px;
  font-weight: 500;
}

.nav-link {
  color: #ffffff;
  text-decoration: none;
  transition: opacity 0.2s ease;
  cursor: pointer;
}

.nav-link:hover {
  opacity: 0.7;
}

.nav-link:active {
  opacity: 0.5;
}
```

### Mobile Navigation
```css
@media (max-width: 809px) {
  .navigation {
    flex-direction: column;
    gap: 20px;
  }

  /* Hamburger menu implementation */
  .menu-toggle {
    display: block;
  }
}
```

---

## 4. Hero Section

### Layout
```css
.hero-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 200px 20px 100px;
  background: #000000;
  text-align: center;
  max-width: 1200px;
  margin: 0 auto;
}
```

### Headline Style
```css
.hero-headline {
  font-size: 72px;
  font-weight: 900;
  line-height: 1.2em;
  letter-spacing: -0.02em;
  color: #ffffff;
  max-width: 800px;
  margin-bottom: 24px;
}

@media (max-width: 1199px) {
  .hero-headline {
    font-size: 56px;
  }
}

@media (max-width: 809px) {
  .hero-headline {
    font-size: 40px;
  }
}
```

### Subtext Style
```css
.hero-subtext {
  font-size: 18px;
  font-weight: 400;
  line-height: 1.6em;
  color: rgba(255, 255, 255, 0.7);
  max-width: 500px;
  margin-bottom: 40px;
}
```

### Hero CTA Button
```css
.hero-cta {
  padding: 16px 32px;
  font-size: 16px;
  font-weight: 600;
  background: #fc5a35;
  color: #ffffff;
  border: none;
  border-radius: 30px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.hero-cta:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(252, 90, 53, 0.4);
}
```

### Background Style
```css
.hero-background {
  background: linear-gradient(180deg, #01010100 0%, #000000ab 100%);
  /* Potential overlay effects */
}
```

---

## 5. Button Styles

### Primary Button
```css
.button-primary {
  padding: 10px 18px;
  font-size: 16px;
  font-weight: 600;
  background: #fc5a35;
  color: #ffffff;
  border: none;
  border-radius: 20px;
  cursor: pointer;
  transition: all 0.2s ease;
}

.button-primary:hover {
  transform: scale(1.05);
  opacity: 0.9;
}

.button-primary:active {
  transform: scale(0.98);
}
```

### Secondary Button
```css
.button-secondary {
  padding: 10px 18px;
  font-size: 16px;
  font-weight: 600;
  background: transparent;
  color: #ffffff;
  border: 1px solid rgba(255, 255, 255, 0.3);
  border-radius: 20px;
  cursor: pointer;
  transition: all 0.2s ease;
}

.button-secondary:hover {
  background: rgba(255, 255, 255, 0.1);
  border-color: rgba(255, 255, 255, 0.5);
}
```

### Button Sizes
```css
.button-small {
  padding: 8px 16px;
  font-size: 14px;
}

.button-large {
  padding: 16px 32px;
  font-size: 18px;
}
```

---

## 6. Spacing System

### Spacing Scale (8px base)
```css
--space-xs: 10px
--space-sm: 24px
--space-md: 30px
--space-lg: 50px
--space-xl: 80px
--space-xxl: 100px
```

### Section Spacing
```css
.section {
  padding: 100px 20px;
  max-width: 1200px;
  margin: 0 auto;
}

@media (max-width: 809px) {
  .section {
    padding: 60px 16px;
  }
}
```

### Component Gaps
```css
--gap-tight: 10px
--gap-normal: 24px
--gap-loose: 50px
```

---

## 7. Layout System

### Container Widths
```css
--container-small: 800px
--container-medium: 1200px
--container-large: 1440px
--container-xlarge: 1480px
```

### Grid System
```css
.grid-2col {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 50px;
}

@media (max-width: 809px) {
  .grid-2col {
    grid-template-columns: 1fr;
    gap: 30px;
  }
}
```

### Flexbox Patterns
```css
.flex-center {
  display: flex;
  align-items: center;
  justify-content: center;
}

.flex-between {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.flex-column {
  display: flex;
  flex-direction: column;
}
```

---

## 8. Card Components

### Basic Card
```css
.card {
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 20px;
  padding: 30px;
  transition: all 0.3s ease;
}

.card:hover {
  background: rgba(255, 255, 255, 0.08);
  border-color: rgba(255, 255, 255, 0.2);
  transform: translateY(-4px);
}
```

### Card Content
```css
.card-title {
  font-size: 24px;
  font-weight: 700;
  margin-bottom: 16px;
  color: #ffffff;
}

.card-description {
  font-size: 16px;
  line-height: 1.6em;
  color: rgba(255, 255, 255, 0.7);
}
```

---

## 9. Iconography

### Icon Sizes
```css
--icon-small: 16px
--icon-medium: 24px
--icon-large: 32px
--icon-xlarge: 110px (social media)
```

### Icon Colors
```css
--icon-primary: #ffffff
--icon-accent: #fc5a35
--icon-muted: rgba(255, 255, 255, 0.5)
```

### Icon Style
- Outlined or line icons preferred
- Consistent stroke width
- Minimal, modern aesthetic

---

## 10. Form Elements

### Input Fields
```css
.input {
  padding: 12px 16px;
  font-size: 16px;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.2);
  border-radius: 12px;
  color: #ffffff;
  transition: all 0.2s ease;
}

.input:focus {
  outline: none;
  border-color: #fc5a35;
  background: rgba(255, 255, 255, 0.08);
}

.input::placeholder {
  color: rgba(255, 255, 255, 0.4);
}
```

### Dropdown/Select
```css
.select {
  padding: 12px 16px;
  font-size: 16px;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.2);
  border-radius: 12px;
  color: #ffffff;
  cursor: pointer;
}
```

### Checkbox
```css
.checkbox {
  width: 20px;
  height: 20px;
  border: 2px solid rgba(255, 255, 255, 0.3);
  border-radius: 4px;
  cursor: pointer;
}

.checkbox:checked {
  background: #fc5a35;
  border-color: #fc5a35;
}
```

---

## 11. Footer Design

### Footer Container
```css
.footer {
  background: #000000;
  padding: 120px 20px 60px;
  max-width: 1480px;
  margin: 0 auto;
}
```

### Footer Layout
```css
.footer-content {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 50px;
  margin-bottom: 60px;
}

@media (max-width: 809px) {
  .footer-content {
    flex-direction: column;
    gap: 40px;
  }
}
```

### Footer Links
```css
.footer-link {
  color: #09f;
  text-decoration: underline;
  font-size: 16px;
  transition: opacity 0.2s ease;
}

.footer-link:hover {
  opacity: 0.7;
}
```

### Social Icons
```css
.social-icon-container {
  width: 110px;
  height: 110px;
  display: flex;
  align-items: center;
  justify-content: center;
}
```

### Copyright Text
```css
.copyright {
  font-size: 14px;
  color: rgba(255, 255, 255, 0.5);
  text-align: center;
}
```

---

## 12. Animations & Transitions

### Standard Transitions
```css
--transition-fast: 0.2s ease
--transition-normal: 0.3s ease
--transition-slow: 0.5s ease
```

### Hover Effects
```css
.hover-lift {
  transition: transform 0.3s ease;
}

.hover-lift:hover {
  transform: translateY(-4px);
}

.hover-scale {
  transition: transform 0.2s ease;
}

.hover-scale:hover {
  transform: scale(1.05);
}
```

### Fade Animations
```css
.fade-in {
  animation: fadeIn 0.5s ease forwards;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
```

---

## 13. Shadows & Elevation

### Shadow Scale
```css
--shadow-sm: 0 2px 8px rgba(0, 0, 0, 0.1)
--shadow-md: 0 4px 16px rgba(0, 0, 0, 0.15)
--shadow-lg: 0 8px 24px rgba(0, 0, 0, 0.2)
--shadow-xl: 0 16px 48px rgba(0, 0, 0, 0.3)
```

### Accent Shadows
```css
--shadow-accent: 0 8px 20px rgba(252, 90, 53, 0.4)
```

### Card Elevation
```css
.card-elevated {
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.2);
}

.card-elevated:hover {
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.3);
}
```

---

## 14. Responsive Breakpoints

### Breakpoint System
```css
/* Desktop First Approach */
--breakpoint-desktop: 1200px
--breakpoint-tablet: 810px to 1199px
--breakpoint-mobile: max 809px

/* Media Queries */
@media (max-width: 1199px) {
  /* Tablet styles */
}

@media (max-width: 809px) {
  /* Mobile styles */
}
```

### Responsive Patterns
- Desktop: Multi-column layouts, full navigation
- Tablet: 2-column grids, condensed spacing
- Mobile: Single column, hamburger menu, stacked elements

---

## 15. Imagery & Graphics

### Image Treatment
- High contrast images
- Subtle overlays for readability
- Responsive image sizing
- Modern, tech-oriented visuals

### Background Patterns
```css
.gradient-overlay {
  background: linear-gradient(180deg, #01010100 0%, #000000ab 100%);
}
```

### Image Positioning
```css
.image-container {
  border-radius: 20px;
  overflow: hidden;
}

.image-full-width {
  width: 100%;
  height: auto;
  display: block;
}
```

---

## 16. Accessibility Considerations

### Color Contrast
- White text on black background: 21:1 ratio (AAA)
- Muted text (70% opacity): Still meets AA standards
- Link blue (#09f) on black: High contrast

### Focus States
```css
.focusable:focus {
  outline: 2px solid #fc5a35;
  outline-offset: 2px;
}
```

### Interactive Elements
- Minimum touch target: 44x44px
- Clear hover and active states
- Keyboard navigable

---

## 17. Design Principles

### Core Aesthetics
1. **Minimalism**: Clean, uncluttered interfaces
2. **Dark Mode First**: Black backgrounds with white text
3. **High Contrast**: Clear visual hierarchy
4. **Modern**: Contemporary tech aesthetic
5. **Functional**: Purpose-driven design

### Visual Hierarchy
1. Large, bold headlines
2. Clear section separation
3. Consistent spacing system
4. Strategic use of accent colors
5. Typography-driven hierarchy

### Interaction Design
1. Smooth transitions (0.2-0.3s)
2. Subtle hover effects
3. Clear active states
4. Responsive feedback
5. Progressive disclosure

---

## 18. Component Reusability Guidelines

### Naming Convention
```css
/* Block-Element-Modifier (BEM) Style */
.component {}
.component__element {}
.component--modifier {}
```

### Component Structure
```jsx
// Example React component following Volvite style
const Card = ({ title, description, variant = 'default' }) => (
  <div className={`card card--${variant}`}>
    <h3 className="card__title">{title}</h3>
    <p className="card__description">{description}</p>
  </div>
);
```

### CSS Variables Usage
```css
:root {
  /* Always define reusable tokens */
  --primary-color: #fc5a35;
  --spacing-unit: 10px;
}

.component {
  color: var(--primary-color);
  margin: calc(var(--spacing-unit) * 2);
}
```

---

## 19. Implementation Checklist

### Setting Up the Design System
- [ ] Import DM Sans and Inter fonts
- [ ] Set up CSS variables for colors, spacing, typography
- [ ] Create base reset/normalize styles
- [ ] Implement responsive breakpoints
- [ ] Set up dark mode as default

### Component Development
- [ ] Build button variants
- [ ] Create card components
- [ ] Develop form elements
- [ ] Implement navigation patterns
- [ ] Design footer structure

### Polish & Details
- [ ] Add hover states to interactive elements
- [ ] Implement smooth transitions
- [ ] Test responsive behavior
- [ ] Verify color contrast ratios
- [ ] Optimize for performance

---

## 20. Quick Reference

### Most Used Values
```css
/* Colors */
background: #000000;
color: #ffffff;
accent: #fc5a35;
link: #09f;

/* Spacing */
gap: 24px, 50px, 100px;
padding: 10px 18px (buttons), 100px 20px (sections);

/* Typography */
font-family: 'DM Sans', 'Inter';
font-size: 16px (base), 72px (hero), 24px (h3);
font-weight: 400, 600, 700, 900;

/* Borders */
border-radius: 20px (cards/buttons), 12px (inputs);

/* Transitions */
transition: all 0.2s ease;

/* Shadows */
box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
```

---

## Conclusion

This style guide captures the minimalist, modern, and high-contrast design aesthetic of Volvite.ai. The design system emphasizes:

- **Dark mode first** approach with black backgrounds
- **Bold typography** with DM Sans font family
- **Strategic accent colors** (orange and blue)
- **Generous spacing** for breathing room
- **Subtle interactions** with smooth transitions
- **Mobile-first responsive** design patterns

Use this guide as a foundation for building consistent, accessible, and visually cohesive interfaces that match the Volvite aesthetic.
