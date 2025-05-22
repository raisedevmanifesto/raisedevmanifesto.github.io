# Blog Section: Design Overview

- The blog section uses and extends site-wide style from `style.css` for consistency and visual integration.
- Blog navigation should be discoverable from the main site; consider a blog index page and links from the homepage or navbar.
- Only reviewed, published content is visible; markdown sources are never published directly.
- The AI conversion process should be:
  - Repeatable and auditable
  - Extensible: future support for custom components, rich media, and accessibility improvements
  - Capable of handling metadata extraction (title, date, author, tags) from markdown frontmatter
- Posts should have consistent layout, date and author display, and optional summary/preview.
- Future: Consider automated RSS feed generation, integration with comments (external platforms), and archive support.