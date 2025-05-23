# RAISE Website Navigation System Design

**Last Updated**: May 23, 2025

## Overview

This document defines the comprehensive navigation system for the RAISE Manifesto website, ensuring users can move intuitively between the manifesto, projects, and blog sections. The navigation system evolved from a single-page site to a multi-section experience requiring clear wayfinding.

## Purpose

The navigation system serves to:

1. Provide clear, consistent access to all major site sections
2. Help users understand their current location within the site
3. Enable smooth transitions between manifesto content, project examples, and blog updates
4. Maintain the site's focus on the manifesto while making other content discoverable
5. Support both linear reading and exploratory browsing patterns

## User Navigation Needs

Based on our user stories and site evolution, visitors need:

- Clear entry points to manifesto, projects, and blog from anywhere on the site
- Understanding of where they are and how sections relate to each other
- Easy return paths to the main manifesto content
- Breadcrumb trails for deeper navigation within projects
- Consistent navigation patterns across all sections

## Primary Navigation Design

### Breadcrumb-Only Navigation Strategy

To maintain content focus and minimal visual overhead, the site uses breadcrumb navigation as the primary wayfinding mechanism:

**All non-homepage pages include breadcrumb navigation**:
- **Format**: Home > Section > Subsection
- **Placement**: Below header, above main content
- **Styling**: Follows design system breadcrumb component
- **Behavior**: Each level is clickable for quick navigation

This approach:
- Maintains clean, uncluttered layouts
- Provides clear navigation context without competing with content
- Takes up minimal vertical space
- Follows the "clarity over complexity" principle central to RAISE

### Homepage Navigation Strategy

The homepage maintains its manifesto-first approach with:
- **No top navigation bar** (preserves focus on reading experience)
- **Section-based CTAs** within content (e.g., "Browse Example Projects")
- **Footer links** for secondary navigation
- **Skip links** for accessibility

This preserves the homepage as a focused reading experience while providing clear paths to other sections.

## Secondary Navigation Patterns

### Breadcrumb Navigation

Used on all non-homepage pages:
- **Format**: Home > Section > Subsection
- **Placement**: Below header, above main content
- **Styling**: Follows design system breadcrumb component
- **Behavior**: Each level is clickable for quick navigation

### Project Section Navigation

**Project Index Page**:
- Breadcrumb: Home > Projects
- Project cards linking to individual projects

**Individual Project Pages**:
- Breadcrumb: Home > Projects > [Project Name]
- Sidebar navigation between project artifacts
- Return links to project overview

**Project Artifact Pages**:
- Breadcrumb: Home > Projects > [Project Name] > [Artifact]
- Sidebar navigation between artifacts
- Return links to project overview

### Blog Section Navigation

**Blog Index Page**:
- Breadcrumb: Home > Blog
- Article cards linking to individual posts

**Individual Blog Posts**:
- Breadcrumb: Home > Blog > [Post Title]
- Return link to blog index

## Navigation States and Indicators

### Active States
- **Current page**: Indicated in breadcrumbs (non-linked final item)
- **Sidebar navigation**: Active artifact highlighted

### Hover States
- Subtle underline for text links
- Background change for button-style links
- Consistent with design system interaction patterns

### Focus States
- Visible focus indicators for keyboard navigation
- High contrast focus rings
- Logical tab order throughout navigation

## Responsive Navigation Behavior

Follows the design system breakpoints:

### Mobile
- Breadcrumbs remain visible but may abbreviate on very small screens
- Sidebar navigation converts to top-of-page navigation on project pages

### Tablet and Desktop
- Complete breadcrumb trails
- Sidebar navigation remains in sidebar for projects

## Implementation Guidelines

### HTML Structure
- Semantic `<nav>` elements with appropriate ARIA labels
- Consistent class naming following BEM methodology
- Proper heading hierarchy integration

### CSS Classes
- `.breadcrumb` for breadcrumb navigation
- `.sidebar-nav` for project artifact navigation

### Accessibility Requirements
- Skip links on all pages
- ARIA attributes for navigation landmarks
- Keyboard navigation support
- Screen reader friendly structure

## Integration with Existing Design

### Design System Integration
- Uses existing color variables and typography
- Follows established spacing and transition patterns
- Maintains consistent visual hierarchy

### Content Strategy
- Navigation supports but doesn't compete with content
- Clear information architecture reflected in navigation structure
- Progressive disclosure of complexity (manifesto → projects → detailed artifacts)

## Future Considerations

### Potential Enhancements
- Search functionality (could be added to header area)
- "Recently viewed" or "Related" navigation aids
- Tag-based navigation for blog posts
- Quick-access menu for frequent artifact types

### Scalability
- Navigation structure supports additional top-level sections
- Breadcrumb system scales to deeper hierarchies
- Sidebar navigation pattern can accommodate more artifact types

---

This navigation design ensures users can explore the full RAISE ecosystem while maintaining the manifesto's central position as the primary content experience.