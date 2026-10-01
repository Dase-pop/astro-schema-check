# astro-schema-check

Paste a post. See exactly why Astro silently dropped it.

**Live tool:** https://astro-schema-check.pages.dev

## How to use it

1. Paste your schema into box 1 (one field per line, like `pubDate: date`).
2. Paste your whole post, or just its frontmatter, into box 2.
3. Tap Check and read the list of problems.

Add a question mark for optional fields, like `draft?: boolean`.

## What it catches

- Missing or empty required fields
- Quoted dates (text, not a date)
- Numbers or booleans where text is expected
- Unquoted colons that break YAML
- Tags written as text instead of a list
- Tabs in frontmatter

## Limits

- Field types supported: string, number, boolean, date, array
- No nested objects yet
- You type your schema in; it does not read content.config.ts yet

## Privacy

Everything runs in your browser. Nothing is uploaded or stored.

## Why this exists

Astro can drop a post from a collection without an error. I hit this while building my blog and wrote up the traps: https://codex-blog-6v6.pages.dev/blog/astro-content-collections-traps/

Found a case it misses? Open an issue with the frontmatter that fooled it.
