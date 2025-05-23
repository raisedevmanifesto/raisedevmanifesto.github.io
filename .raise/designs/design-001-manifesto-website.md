# Design 001: RAISE Manifesto Website

**Last Updated**: May 16, 2025

## Overview

This document outlines the design considerations for the RAISE Manifesto website, focusing on making the manifesto itself prominent while providing context about its origins and future. It builds upon the foundational design system defined in [Design 000: Design System](./design-000-design-system.md) and applies those principles to the specific needs of the manifesto presentation.

## Core Principles from User Story 001:

*   The RAISE Manifesto is published in a clear, readable format.
*   The site is simple, fast, and works on any device.
*   Prominent links to external discussion threads.
*   No login required.
*   Date-based versioning for the manifesto.
*   Reflect RAISE values: simplicity, transparency, humility, and bravery.
*   Include "Who We Are" (author bio) and "What's Next" (future plans).

## Design Directives:

*   **Manifesto First:** The manifesto text is the hero content.
*   **De-emphasize "Who":** The author information should be present but not overshadow the manifesto.
*   **Clarity for "What's Next":** Future plans should be easy to understand.

## Layout Strategy:

1.  **Main View - Manifesto:**
    *   The primary landing experience will be the manifesto text itself. It should occupy the main content area of the page.
    *   Minimal distraction around the manifesto text.
    *   Clear display of the manifesto version (last updated date), subtly placed near the main title or at the very end of the manifesto content.

2.  **Secondary Information - "Who We Are" & "What's Next":**
    *   These sections will be positioned below the main manifesto content on the same page, separated by a clear but unobtrusive visual element (e.g., a light horizontal rule or a subtle change in background shade for these sections).
    *   The "Who We Are" section will be brief, text-only, and styled modestly to maintain its de-emphasized nature.
    *   The "What's Next" section will follow, also presented concisely.

3.  **Discussion Links:**
    *   These will be placed at the very end of the page, after the "Who We Are" and "What's Next" sections. They should be clearly labeled and easy to interact with.

## Visual Hierarchy & Style

### Typography Implementation

Following the design system's font choices and type scale:

* **Manifesto Body:** Lora (serif) at `--font-size-md` (1.2rem/~19px), providing elegant readability for extended content
* **Headings within Manifesto:** 
  * Main heading (h1): Open Sans at `--font-size-2xl` (2.074rem/~33px)
  * Section headings (h2): Open Sans at `--font-size-xl` (1.728rem/~28px)
  * Subsection headings (h3): Open Sans at `--font-size-lg` (1.44rem/~23px)
* **Supporting Text:** Open Sans at `--font-size-sm` (1rem/16px) for secondary information

### Color Application

Implementing the design system's color palette:

* **Background:** `--color-background` (#FAF9F6) for the main background, providing a softer reading experience
* **Text:** `--color-text` (#333333) for primary text, ensuring readability
* **Headings:** `--color-headings` (#222222) for strong visual hierarchy
* **Accents & Links:** `--color-accent` (#546A7B) used sparingly for links and highlights
* **Secondary Content:** Supporting sections use `--color-supporting-bg` (#F8F8F8) to differentiate from main content

### Spacing System

Utilizing the design system's spacing scale:

* **Line Height:** 1.6 for body text (1.8 for manifesto content) to enhance readability
* **Content Margins:** `--space-md` (1rem) on mobile, increasing to `--space-xl` (2rem) on larger screens
* **Paragraph Spacing:** `--space-lg` (1.5rem) between paragraphs
* **Section Spacing:** `--space-2xl` (3rem) between major sections

### Simplicity & Focus

Aligning with RAISE values:

* No unnecessary decorative elements or complex UI components
* Clean, minimal design letting content take center stage
* Subtle visual separation between content sections
* Responsive adjustments that maintain content integrity at all sizes

## Navigation:

**Homepage Strategy:** The manifesto page maintains a focused reading experience with minimal navigation to preserve content prominence. As the site evolved to include multiple sections, navigation was redesigned:

*   **Primary Navigation:** None on the homepage to maintain reading focus. Cross-section access provided via section CTAs and footer links.
*   **Secondary Navigation:** Scrolling to sections on the same page ("Who We Are," "Example Projects," "Open Questions"). Clear headings for these sections are crucial.
*   **Multi-Section Site:** For comprehensive navigation patterns across the full site (Projects, Blog), see [Navigation System Design](design-004-navigation-system.md).

## Responsive Implementation

Applying the design system's responsive approach:

### Desktop and Larger Tablets

* Maximum content width of `--content-max-width` (800px) for optimal readability
* Centered content with white space on either side
* Full type scale as defined in the design system
* Comfortable spacing between elements
* Two-column layout for supplemental sections where appropriate

### Mobile and Smaller Tablets

* Single column layout with comfortable side margins (`--space-md`)
* Slightly reduced font sizes, following the responsive adjustments in the design system
* Preserved spacing hierarchy, scaled appropriately for smaller screens
* Consistent content availability across all devices
* Touch-friendly sizing for interactive elements (minimum 44×44px)

### Breakpoints

Following the design system's defined breakpoints:

* Adjustments at 600px for mobile to tablet transition
* Adjustments at 900px for tablet to desktop transition

## Accessibility (A11y)

The RAISE Manifesto website will be designed and developed to meet high accessibility standards, aiming for compliance with Web Content Accessibility Guidelines (WCAG) 2.1 Level AA, and aspiring to Level AAA where feasible. Ensuring a "world-class" experience for screen reader users is a primary objective.

Key considerations include:

*   **Semantic HTML:**
    *   Utilize proper HTML5 semantic elements (`<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<aside>`, `<footer>`) to define page structure and landmarks, providing clear navigation paths for screen readers.
    *   Ensure a logical and hierarchical heading structure (`<h1>` for the main manifesto title, `<h2>` for major sections like "Who We Are," "What's Next," etc., and `<h3>-<h6>` as needed within content).
*   **ARIA (Accessible Rich Internet Applications):**
    *   Use ARIA attributes judiciously only when semantic HTML alone is insufficient to convey roles, states, and properties of UI components. The focus will be on correct native HTML first.
*   **Keyboard Navigation & Focus Management:**
    *   All interactive elements (links, buttons, future form fields if any) will be fully operable via keyboard.
    *   Visible focus indicators will be clear and prominent.
    *   Logical tab order will be maintained.
*   **Text Alternatives:**
    *   Since the site aims for minimal imagery, any essential images used will have descriptive `alt` text. Decorative images will have null `alt` attributes (`alt=""`).
*   **Content Readability & Structure:**
    *   The chosen fonts (Lora, Open Sans) and generous spacing support readability.
    *   Content will be organized clearly with ample white space.
    *   Links will have descriptive text that makes sense out of context (e.g., "Read more about the RAISE values" instead of "Click here").
*   **Color Contrast:**
    *   The chosen color palette (off-white background, dark gray text) already aims for high contrast, which will be verified against WCAG AA/AAA requirements.
*   **Language Declaration:**
    *   The HTML document will have a `lang` attribute correctly set (e.g., `lang="en"`).
*   **Simplicity:**
    *   The overall minimalist design approach will inherently reduce accessibility barriers by avoiding complex interactions or animations that can be problematic.

## Specifics for "Who We Are" Presentation:

*   A single, brief paragraph of 2-4 sentences.
*   Text-only, using the supporting text typography.
*   Located after the main manifesto and any discussion links, before "What's Next".

## Specifics for "What's Next" Presentation:

*   A short introductory sentence followed by 2-4 bullet points.
*   Clearly outlines the intent to build more applications and tools using RAISE.
*   Located after "Who We Are".

---

*This design document outlines the core decisions for the RAISE Manifesto website and will be updated as needed during development.*

