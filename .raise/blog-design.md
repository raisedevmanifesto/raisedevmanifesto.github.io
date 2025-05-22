# Blog Section: Design Overview

## Directory Structure

- `.raise/blog_src/` — Source markdown files for all blog stories (drafts and published posts)
- `/blog/` — Published HTML blog posts, generated from markdown
- `.raise/adr/` — Architectural decision records, including the blog content flow ADR

## Editorial & Publishing Process

1. Write and edit blog posts as markdown files in `.raise/blog_src/`.
2. When a post is ready, trigger the AI or automated process to:
   - Convert markdown to styled HTML
   - Apply site navigation, metadata, and consistent formatting
   - Place the generated HTML in `/blog/`
3. Drafts remain unpublished in `.raise/blog_src/`.
4. Design can evolve; future enhancements could include AI-powered summaries, images, or custom layouts.

## Design Notes

- The blog inherits site-wide style from `style.css` and navigation from the root.
- Source markdown is never published directly, ensuring only reviewed content is visible.
- The AI conversion process should be repeatable and extensible.