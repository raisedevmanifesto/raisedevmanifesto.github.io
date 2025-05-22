# Blog Section: Design Overview

## Directory Structure

- `.raise/blog_src/` — Source markdown files for all blog stories (drafts and published posts)
- `/blog/` — Published HTML blog posts, generated from markdown
- `.raise/architecture/` — Architectural decision records (see `adr-004-blog-content-flow.md` for rationale)

## Editorial & Publishing Process

1. Authors draft and edit blog posts as markdown files in `.raise/blog_src/`.
2. When a post is ready, an AI or automated process is triggered to:
   - Convert markdown to styled HTML
   - Insert site navigation, metadata, and consistent formatting
   - Apply syntax highlighting, image handling, and post metadata extraction
   - Place the generated HTML in `/blog/`
3. Drafts and unpublished posts remain in `.raise/blog_src/`.
4. The system allows for future enhancements, e.g., AI-powered summaries, automated tagging, cover images, or custom layouts.
5. The process supports clear separation of source (unpublished) and published (production) content.

## Design Notes

- The blog section uses and extends site-wide style from `style.css` for consistency and visual integration.
- Blog navigation should be discoverable from the main site; consider a blog index page and links from the homepage or navbar.
- Only reviewed, published content is visible; markdown sources are never published directly.
- The AI conversion process should be:
  - Repeatable and auditable
  - Extensible: future support for custom components, rich media, and accessibility improvements
  - Capable of handling metadata extraction (title, date, author, tags) from markdown frontmatter
- Posts should have consistent layout, date and author display, and optional summary/preview.
- Future: Consider automated RSS feed generation, integration with comments (external platforms), and archive support.