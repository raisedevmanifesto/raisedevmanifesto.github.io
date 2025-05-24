# RAISE Manifesto Website Sitemap

**Last Updated**: May 23, 2025

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
├── /projects/ (Projects Directory)
│   │
│   ├── /index.html (Projects Overview/Listing)
│   │   ├── Breadcrumb Navigation
│   │   ├── Introduction/Description of Projects
│   │   └── Project Entries (Title, Description, Summary, Link to full project)
│   │
│   └── /project-folders/ (Individual Project Implementations)
│        ├── /project-name-1/
│        │   ├── index.html (Project Overview)
│        │   ├── /vision/ (Vision Document)
│        │   ├── /values/ (Values Document)
│        │   ├── /stories/ (User Stories)
│        │   ├── /designs/ (Design Decisions)
│        │   ├── /sitemap/ (Site Map)
│        │   └── /architecture/ (Architecture Decisions)
│        └── /project-name-2/
│            ├── index.html (Project Overview)
│            └── [Similar RAISE artifact structure]
│
└── /blog/ (Blog Directory)
    │
    ├── /index.html (Blog Overview/Listing)
    │   ├── Breadcrumb Navigation
    │   ├── Introduction/Description of Blog
    │   └── Blog Post Entries (Title, Date, Summary, Link to full post)
    │
    └── /posts/ (Individual Blog Posts)
        ├── /YYYY-MM-DD/post-slug-1/
        │   └── index.html (Full Blog Post Content)
        └── /YYYY-MM-DD/post-slug-2/
            └── index.html (Full Blog Post Content)
```

## Navigation Patterns

### Primary Navigation
- **Top Navigation Bar**: Links to Homepage (Manifesto), Projects, Blog
  - Present on all pages except homepage (maintains manifesto focus)
  - Consistent placement and styling across sections
- **Homepage**: Manifesto-first approach with section CTAs and footer links
- **Inter-Page Navigation**: Consistent breadcrumb trails showing location

### Secondary Navigation
- **Breadcrumb Navigation**: Present on all non-homepage pages
- **Within Project Pages**: Sidebar navigation to different artifacts
- **Back to Top**: Links at the bottom of long pages
- **Return Navigation**: Clear paths back to parent sections

For comprehensive navigation design details, see [Navigation System Design](designs/design-004-navigation-system.md).

## Content Hierarchy

1. **Manifesto Content**: Primary focus of the site, presented first on the homepage
2. **Blog Content**: News, updates, and articles.
3. **Example Projects**: Secondary content that demonstrates the methodology in practice
4. **Supporting Information**: Open Questions as supplemental content

## Future Considerations

- **Additional Example Projects**: More projects will be added to the /projects/ directory as they are developed
- **Resources Section**: Potential future expansion for templates and tools
- **Community Section**: Possible addition for contribution guidelines and community engagement

This site map reflects the story-first approach of the RAISE methodology, with a clear progression from core principles (the manifesto) to practical examples (the projects section) that demonstrate implementation, and timely updates via the blog.