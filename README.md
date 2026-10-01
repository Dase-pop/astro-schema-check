# astro-schema-check

Paste a post. See exactly why Astro silently dropped it.

Live tool: https://astro-schema-check.pages.dev

## What it catches

- Missing or empty required fields
- Quoted dates (text, not a date)
- Numbers or booleans where text is expected
- Unquoted colons that break YAML
- Tags written as text instead of a list

Everything runs in your browser. Nothing is uploaded.
