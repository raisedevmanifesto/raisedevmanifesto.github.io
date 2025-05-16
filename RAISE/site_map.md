# RAISE Manifesto Website Sitemap

**Last Updated**: May 16, 2025

## Overview

The RAISE Manifesto website has evolved from a single-page site to a multi-page structure that includes example projects. This sitemap documents the organization and navigation flow of the entire site.

## Site Structure

```
RAISE Manifesto Website
│
├── / (Homepage)
│   ├── Header
│   │   └── Site title, version, last updated date
│   │
│   ├── Manifesto Content
│   │   ├── Introduction
│   │   ├── Core Principles
│   │   └── Methodology
│   │
│   ├── Example Projects Section
│   │   └── Link to Projects Directory
│   │
│   ├── Open Questions Section
│   │
│   └── Footer
│       └── Copyright, back to top link
│
└── /projects/ (Projects Directory)
    │
    ├── /index.html (Projects Overview)
    │   ├── Breadcrumb Navigation
    │   ├── Introduction
    │   └── Project Cards
    │       ├── RAISE Manifesto Website
    │       └── [Future Projects]
    │
    └── /manifesto-site/ (RAISE Manifesto Website Project)
        ├── /index.html (Project Overview)
        │   ├── Breadcrumb Navigation
        │   ├── Sidebar Navigation to Artifacts
        │   ├── Project Summary
        │   ├── Key Features
        │   ├── Development Timeline
        │   ├── Artifact Navigation Cards
        │   └── Repository Link
        │
        ├── /vision/ (Vision Document)
        │   └── index.html
        ├── /values/ (Values Document)
        │   └── index.html
        ├── /stories/ (User Stories)
        │   └── index.html
        ├── /sitemap/ (Site Map)
        │   └── index.html
        └── /architecture/ (Architecture Decisions)
            └── index.html
```

## Navigation Patterns

### Primary Navigation

- **Homepage**: Vertical scrolling with a focus on reading the manifesto
- **Project Links**: Direct links from homepage to projects section
- **Inter-Page Navigation**: Consistent breadcrumb trails showing location

### Secondary Navigation

- **Within Project Pages**: Sidebar navigation to different artifacts
- **Back to Top**: Links at the bottom of long pages
- **Return Navigation**: Clear paths back to parent sections

## Content Hierarchy

1. **Manifesto Content**: Primary focus of the site, presented first on the homepage
2. **Example Projects**: Secondary content that demonstrates the methodology in practice
3. **Supporting Information**: Open Questions as supplemental content

## Future Considerations

- **Additional Example Projects**: More projects will be added to the /projects/ directory as they are developed
- **Resources Section**: Potential future expansion for templates and tools
- **Community Section**: Possible addition for contribution guidelines and community engagement

This site map reflects the story-first approach of the RAISE methodology, with a clear progression from core principles (the manifesto) to practical examples (the projects section) that demonstrate implementation.