# ADR 001: Blog Post Format and Generation

**Status**: Proposed

**Context**:

The RAISE Manifesto website needs a blog section as per User Story 003. We need to decide on the format for blog posts and how they will be published on the site. The core constraint is to avoid a static site generator or CMS, aligning with the project's philosophy of simplicity and direct HTML/CSS/JS editing.

**Decision**:

Blog posts will be authored in Markdown (`.md`) files. These Markdown files will serve as the source of truth for blog content.
A script (or manual process initially, to be potentially automated by an AI assistant) will be responsible for converting these Markdown files into individual HTML pages.
The HTML pages will be structured to fit the existing website's design and navigation.
The process will be:
1. Create a new Markdown file in a designated `blog/posts_markdown/` directory (or similar).
2. The content will be plain Markdown. Metadata like title, date, and author can be included at the top of the Markdown file in a simple, parseable format (e.g., frontmatter-like, or specific comment convention).
3. A conversion step (manual or AI-assisted) will take this Markdown file, parse the metadata and content, and generate a corresponding HTML file in the `/blog/posts/YYYY/MM/DD/post-slug/index.html` structure.
4. The main blog listing page (`/blog/index.html`) will also be updated (manually or by AI assistance) to include a link and summary for the new post.

**Consequences**:

*   **Pros**:
    *   **Simplicity of Authoring**: Markdown is easy to write and widely understood.
    *   **Version Controllable**: Blog posts are plain text files, making them ideal for Git version control.
    *   **No Complex Dependencies**: Avoids introducing a static site generator or CMS, keeping the tech stack minimal.
    *   **AI-Friendly**: The conversion from Markdown to HTML is a task well-suited for AI assistance, fitting the "AI will do that for me" aspect mentioned.
    *   **Flexibility**: HTML structure can be precisely controlled during the conversion process.
*   **Cons**:
    *   **Manual/Semi-Manual Process**: Requires a distinct step to convert Markdown to HTML and update the blog index. This could be error-prone if entirely manual.
    *   **No Dynamic Features Out-of-the-Box**: Features like tags, categories, or search would need to be manually implemented or AI-generated into the HTML.
    *   **Build Step (Implicit)**: Even without a "generator," there's a transformation step.

This decision supports our values of transparency and community engagement by maintaining simple, accessible content creation while preserving quality through human oversight.

## Related Documents

- [Blog Design Document](../designs/design-0003-blog-design.md) - Visual design and user experience for blog section
- [Navigation System Design](../designs/design-004-navigation-system.md) - Navigation patterns for blog integration 