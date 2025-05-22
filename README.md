# RAISE Manifesto Website

## Rules and AI for Intention-driven Software Engineering

This repository contains the RAISE Manifesto website, which documents and demonstrates the RAISE methodology for building better software with AI assistance.

## About RAISE

RAISE is a bold methodology designed to empower visionaries—technical or not—to shape, refine, and ship meaningful software through structured storytelling and artifact-driven engineering.

The methodology emphasizes:
- Vision comes first, before code
- Stories are the atomic unit of progress
- Narrative clarity fuels technical clarity
- Living artifacts form the backbone of high-integrity engineering

## Project Structure & Sitemap

This site is organized according to RAISE principles, with the following key sections:

- `/` - Root contains the main manifesto document
- `/projects/` - Example projects demonstrating RAISE methodology
- `/blog/` - Published blog stories, generated as HTML from markdown sources
- `/.raise/` - Source artifacts that drive site development and publishing workflows
    - `.raise/blog_src/` - Blog/story drafts and posts written in markdown (not published directly)
    - `.raise/designs/` - Design documents (see `design-003-blog-section.md` for blog design)
    - `.raise/architecture/` - Architectural Decision Records (see `adr-004-blog-content-flow.md` for blog publishing ADR)

**Blog Story Flow:**
- Blog posts are created and edited as markdown files in `.raise/blog_src/`.
- When ready for publication, an AI (or automated) process converts the markdown files into styled HTML pages, which are published in `/blog/`.
- Design and rationale for this flow can be found in:
    - `.raise/designs/design-003-blog-section.md` (design)
    - `.raise/architecture/adr-004-blog-content-flow.md` (ADR)

## Implementation Details

The site is intentionally built as a static HTML/CSS website without JavaScript dependencies, demonstrating simplicity, accessibility, and longevity principles core to the RAISE methodology.

## Contributing

We welcome contributions that align with the RAISE vision and values. If you're using the RAISE methodology for your own projects, we'd love to showcase them as examples.

Contact us: raisedevmanifesto@gmail.com

## License

© 2025 RAISE Initiative. All rights reserved.
