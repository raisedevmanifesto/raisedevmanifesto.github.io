# RAISE Projects Directory Design

**Last Updated**: May 16, 2025

## Overview

This document outlines the design and implementation strategy for the RAISE Manifesto Example Projects section. This area of the site showcases real-world implementations of the RAISE methodology, demonstrating how vision translates to values, which inform user stories, which guide architecture decisions and implementation.

## Purpose

The Projects Directory serves multiple purposes:

1. Demonstrates RAISE in action through tangible examples
2. Provides a learning resource for those new to the methodology
3. Showcases the progression from vision to implementation
4. Creates a platform for community contribution and growth
5. Reinforces that RAISE is not just theoretical but practical

## User Needs

Based on our user stories, visitors to the Projects section need:

- Clear examples showing how RAISE methodology works in practice
- Access to complete artifacts for each project (vision, stories, decisions)
- A way to understand the progression of a project from concept to implementation
- Easy navigation between different projects and their artifacts
- Accessible content regardless of device or assistive technology

## Design Focus

This design document focuses on the visual presentation, user experience, and implementation approach for the Projects Directory. The information architecture and URL structure are defined in the [Site Map](/RAISE/site_map.md) document.

## Layout Strategy

### Projects Index Page

- **Header**: Standard site header with proper title
- **Breadcrumb Navigation**: Home > Example Projects
- **Introduction**: Brief explanation of the purpose of the examples section
- **Project Cards**:
  - Grid layout with responsive adjustments
  - Each card contains project name, brief description, and technologies used
  - Cards link to individual project overview pages

### Individual Project Page

- **Header**: Project name and last updated date
- **Breadcrumb Navigation**: Home > Example Projects > [Project Name]
- **Two-Column Layout**:
  - Left sidebar: Navigation between project artifacts
  - Main content: Project overview and timeline
- **Project Overview**: Description, key features, screenshots
- **Development Timeline**: Visualization of the project's progression
- **Artifact Links**: Cards linking to each RAISE artifact
- **Repository Link**: Link to source code when applicable

### Artifact Pages

- **Header**: Artifact name and project name
- **Breadcrumb Navigation**: Home > Example Projects > [Project Name] > [Artifact]
- **Two-Column Layout**:
  - Left sidebar: Navigation between project artifacts
  - Main content: Artifact content
- **Consistent Content Structure**:
  - Introduction explaining the artifact's purpose
  - The artifact content itself
  - Implementation notes showing how it connects to other artifacts

## Visual Design

### Project Cards

- Clean, minimal design with subtle hover effects
- Consistent height but flexible width based on screen size
- Visual indicator for featured or new projects
- Small tag indicators showing technologies or methodologies used

### Navigation

- Sidebar navigation is sticky on larger screens for easy reference
- Active states clearly indicate current location
- Breadcrumbs show full path and allow quick navigation to parent sections

### Content Presentation

- Timeline visualization for project progression
- Card-based layout for artifact links
- Consistent typography and spacing following main design system
- Subtle use of color to differentiate artifact types

## Responsive Behavior

- **Mobile (< 600px)**:
  - Single column layout throughout
  - Stacked navigation above content
  - Full-width cards
  
- **Tablet (600px - 900px)**:
  - Two-column grid for project cards
  - Adaptive layout for project pages
  - Sidebar navigation collapses to top on smaller tablets
  
- **Desktop (> 900px)**:
  - Three-column or more grid for project cards
  - Full two-column layout for project pages
  - Sticky sidebar navigation

## Accessibility Considerations

- Semantic HTML structure for proper screen reader navigation
- Keyboard accessibility for all interactive elements
- Sufficient color contrast for all text elements
- Focus states visible for keyboard navigation
- Appropriate ARIA attributes where needed
- Alternative text for any visual elements

## Implementation Approach

Following the RAISE methodology itself, implementation will:

1. Start with this design document as the vision
2. Develop specific user stories for each component
3. Create a detailed implementation plan
4. Build the directory structure and base templates
5. Implement the first example project (the RAISE Manifesto site itself)
6. Test thoroughly across devices and with accessibility tools
7. Document the implementation for future maintainers

## Future Expansion

The projects directory is designed to grow organically as more examples are added:

- Each new project follows the same structure for consistency
- New project types can be added by following the established pattern
- The index page can be extended to include filtering or categorization as the number of examples grows

---

This design document will be updated as implementation progresses and as we gather feedback from users. It serves as both a guide for implementation and a reference for understanding the design decisions.
