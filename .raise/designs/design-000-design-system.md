# RAISE Manifesto Design System

**Last Updated**: May 16, 2025

## Overview

This document outlines the shared design language for the RAISE Manifesto website. The design system is built around the core principles of the RAISE methodology: clarity, purpose, and human-centered design. It ensures consistency across the site while remaining flexible enough to adapt to different contexts.

## Typography

### Font Families

- **Headings**: Open Sans (sans-serif)
- **Body Text**: Lora (serif)
- **UI Elements**: Open Sans (sans-serif)

### Type Scale

We use a modular scale with a ratio of 1.2 (minor third) to create a harmonious hierarchy:

```css
--font-size-xs: 0.833rem;  /* ~13px */
--font-size-sm: 1rem;       /* 16px */
--font-size-md: 1.2rem;     /* ~19px */
--font-size-lg: 1.44rem;    /* ~23px */
--font-size-xl: 1.728rem;   /* ~28px */
--font-size-2xl: 2.074rem;  /* ~33px */
--font-size-3xl: 2.488rem;  /* ~40px */
```

### Line Heights

- Headings: 1.2-1.3 (tighter)
- Body text: 1.6-1.8 (more spacious)

## Color System

### Primary Colors

```css
--color-background: #FAF9F6;  /* Off-white background */
--color-text: #333333;        /* Dark gray for main text */
--color-headings: #222222;    /* Darker gray for headings */
--color-accent: #546A7B;      /* Blue-gray accent color */
```

### Supporting Colors

```css
--color-supporting-bg: #F8F8F8;  /* Light gray for cards, asides */
--color-border: #E0E0E0;         /* Light gray for borders */
--color-text-secondary: #555555; /* Medium gray for secondary text */
--color-text-tertiary: #777777;  /* Lighter gray for tertiary text */
--color-link: #546A7B;           /* Same as accent color for links */
--color-focus: #4A90E2;          /* Blue for focus states */
```

### UI Colors

```css
--color-footer-bg: #333333;     /* Dark gray for footer */
--color-footer-text: #FFFFFF;   /* White text in footer */
```

## Spacing

We use a consistent spacing scale to create rhythm across the interface:

```css
--space-xs: 0.25rem;  /* 4px */
--space-sm: 0.5rem;   /* 8px */
--space-md: 1rem;     /* 16px */
--space-lg: 1.5rem;   /* 24px */
--space-xl: 2rem;     /* 32px */
--space-2xl: 3rem;    /* 48px */
--space-3xl: 4rem;    /* 64px */
```

## Layout

### Content Width

```css
--content-max-width: 800px;  /* Maximum width for content readability */
```

### Breakpoints

- Mobile: Up to 600px
- Tablet: 601px to 900px
- Desktop: 901px and above

## Components

### Header

- Dark background (#333333)
- White text
- Centered title
- Bottom border for visual separation

### Main Content

- White background
- Maximum width of 800px
- Centered on the page
- Light shadow for subtle depth

### Sections

- Clear headings
- Consistent spacing (margin-top: 2-3rem)
- Optional background colors for separation

### Footer

- Dark background matching header
- Simple centered text
- Links to key pages

### Cards

- Light background
- Subtle border (1px solid #E0E0E0)
- Border radius: 4px
- Subtle shadow on hover
- Padding: 1.5rem

### Buttons

- Primary: Accent color background, white text
- Border radius: 4px
- Padding: 0.5rem 1.5rem
- Font weight: 600 (semi-bold)
- Hover effect: Slightly darker background

### Navigation

**Top Navigation Bar**:
- Horizontal layout with consistent spacing
- Text-based links using primary font family
- Background: Transparent or subtle supporting background
- Hover effect: Underline
- Active state: Bold text or subtle background highlight

**Breadcrumb Navigation**:
- Small font size (var(--font-size-sm))
- Separator: "/" with muted color
- Links use standard link color
- Current page indicated without link

**Sidebar Navigation** (for project pages):
- Vertical list layout
- Active item highlighted with background color
- Hover effects consistent with other navigation

## Animation & Transitions

```css
--transition-fast: 150ms;      /* For small UI elements */
--transition-medium: 300ms;    /* For larger components */
--transition-slow: 500ms;      /* For major transitions */
```

## Accessibility

- Color contrast meets Web Content Accessibility Guidelines (WCAG) 2.1 AA standards
- Focus states are clearly visible
- Semantic HTML structure
- Text is resizable without breaking layouts
- Elements have appropriate spacing for touch targets

## Implementation Notes

The design system is implemented as CSS custom properties (variables) at the root level. This allows for consistent usage across the site while maintaining the flexibility to override values in specific contexts.

Implementors should refer to this document when making style decisions to ensure consistency with the overall design vision.

---

This design system is a living document and will evolve as the RAISE Manifesto site grows. Updates will be documented with version numbers and dates.
