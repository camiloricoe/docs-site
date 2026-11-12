# Pocket Timer docs

The user documentation of Pocket Timer, a small command-line focus timer, as Markdown pages in `docs/`.

## Commands
- Check: the TEST_CMD in factory.conf checks every relative link and #anchor (must pass before any PR).

## Conventions
- One `# Title` per page, then `##` sections. Short paragraphs, second person ("you"), present tense.
- Commands in backticks: `pocket start`. Config keys as `key = value`.
- Every page is linked from `docs/index.md`. Link to sections with `page.md#section-slug`.

## Factory rules
- Phase state lives in `.factory/` as markdown files.
- Only the paths in SCOPE (factory.conf) may change. Do not touch factory.sh, lib/, gates/, .claude/, tools/ or this file.

## Exact commands (copy them exactly)
- Check: `python3 tools/check_links.py` (the TEST_CMD). Gates: run each file in gates/ before finishing.
- Run them exactly as written: no `cd`, no env vars, no pipes or `&&`, no other spelling.
  Anything else is blocked by the factory and the run is rejected.

## Review scope
- Security findings are about the diff (`git diff main`). Files the change did not touch,
  such as factory.conf, are out of scope for the review.
- Prefer the smallest change that fully meets the ticket; every gate in gates/ must pass.

