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
   - Place the generated HTML in `/blog/`
3. Drafts and unpublished posts remain in `.raise/blog_src/`.
4. The system allows for future enhancements, e.g., AI-powered summaries, tagging, images, or custom layouts.

## Design Notes

- The blog section uses site-wide style from `style.css` and integrates into main navigation.
- Only reviewed, published content is visible; markdown sources are never published directly.
- The AI conversion process is designed to be repeatable, auditable, and extensible for future needs.