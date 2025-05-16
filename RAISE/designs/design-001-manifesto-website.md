# Design 001: RAISE Manifesto Website

This document outlines the design considerations for the RAISE Manifesto website, focusing on making the manifesto itself prominent while providing context about its origins and future.

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

## Visual Hierarchy & Style:

*   **Typography:**
    *   **Manifesto Body:** Lora (serif), base size 18-22px. Chosen for its elegant readability, suitable for extended reading.
    *   **Headings within Manifesto:** Open Sans (sans-serif), Bold or Semi-Bold weight. Sized appropriately larger than the body text (e.g., 1.5-2x base font size for main headings, smaller for subheadings). This provides clear contrast and modern scannability against the serif body.
    *   **Supporting Text ("Who," "Next," Discussion Links, Version Info):** Open Sans (sans-serif), regular weight, size 14-16px. This ensures a clean, neutral presentation for secondary information.
*   **Color Palette:**
    *   **Background:** An off-white (e.g., `#F8F8F8` or `#FAF9F6`) or very light warm gray for the main background. This provides a softer reading experience than stark white and subtly nods to the preference for less harsh screens, without implementing a full dark mode.
    *   **Text:** Dark gray (e.g., `#333333`) or near-black for primary text to ensure high contrast and readability.
    *   **Accents:** A muted, trustworthy color (e.g., a desaturated blue or green) for links and an occasional highlight, used sparingly. The color should align with simplicity and transparency values.
*   **Spacing:** Generous leading (line-height) for manifesto text (e.g., 1.6-1.8). Ample margins around the main content block and paragraph spacing to prevent a cramped feel.
*   **Simplicity:** No unnecessary images, animations, or complex UI elements. The design should be "invisible" and let the content shine. Decorative elements, if any, should be extremely subtle and purposeful.

## Navigation:

*   **Primary Navigation:** Essentially, none beyond scrolling. If the manifesto becomes very long, consider subtle in-page anchor links for major sections, perhaps presented as a simple table of contents at the beginning or as sticky section headers that appear on scroll.
*   **Secondary Navigation (to "Who," "Next," "Discuss"):** Achieved by scrolling to these sections on the same page. Clear headings for these sections will be crucial.

## Responsiveness:

*   The design must be fully responsive. A single-column layout will be enforced for mobile and tablet views, ensuring readability and ease of scrolling. Text will reflow, and font sizes may adjust slightly for smaller screens.

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

