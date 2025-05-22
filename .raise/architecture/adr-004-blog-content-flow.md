# ADR-004: Blog Content Flow with Markdown and AI Conversion

## Status

Proposed

## Context

We want to add a blog/story section to the RAISE Manifesto website. Blog posts should be authored as markdown files for easy drafting and versioning, but not published directly. Instead, an AI process will convert markdown posts into styled HTML pages for publishing, ensuring consistency and enabling editorial review and transformation.

## Decision

- Create a directory (`blog_src/`) containing markdown files for each story/post.
- These markdown files are source artifacts and are not published as-is.
- An AI or automated process will convert these markdown files into HTML pages with site styling and navigation, placing them in a `blog/` directory for publication.
- Drafts and unpublished posts remain only in `blog_src/` until promoted.
- This supports editorial workflows and provides a clear separation between source and published content.

## Consequences

- Authors can focus on writing in markdown, with AI handling formatting and publication.
- The publishing process is auditable and repeatable.
- Future improvements may include automated summarization, tagging, or design enhancements during conversion.