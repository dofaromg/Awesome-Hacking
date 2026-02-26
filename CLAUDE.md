# CLAUDE.md

## Repository Overview

**Awesome-Hacking** is a curated list of awesome lists for hackers, pentesters, and security researchers. It is a content-only repository — there is no application code, build system, or test suite. The entire project is a single `README.md` linking to external GitHub repositories and resources.

Original upstream: `Hack-with-Github/Awesome-Hacking`

## Repository Structure

```
.
├── README.md              # Main content — the curated list of resources
├── contributing.md        # Contribution guidelines
├── LICENSE                # CC0 1.0 Universal (public domain)
├── awesome_hacking.jpg    # Banner image used in README
└── .github/
    └── workflows/
        └── lock-threads.yml  # Auto-locks inactive issues/PRs after 7 days
```

## Content Format

`README.md` contains two markdown tables:

1. **Awesome Repositories** — Primary curated security/hacking awesome lists
2. **Other Useful Repositories** — Supplementary security tools, references, and resources

Each table row follows this format:

```markdown
[Repository Name](https://github.com/owner/repo) | Short description of the resource
```

## Key Conventions

### Ordering
- Entries within each table section **must be in alphabetical order** by repository name.

### Descriptions
- Descriptions are concise, single-line summaries.
- Use sentence case (capitalize first word only, unless proper nouns).

### Table Alignment
- Column separator uses ` | ` (space-pipe-space) between the link and description.
- The header separator row is `---- | ----`.

### Adding Entries
- Add new entries to the appropriate section (`Awesome Repositories` or `Other Useful Repositories`).
- Maintain alphabetical order within the section.
- Ensure the linked repository actually exists and is relevant to hacking/security.
- Submit changes via pull request.

### Removing Entries
- Remove entries only if the linked resource returns a 404 or is no longer maintained/relevant.

## CI/Automation

- **Lock Threads** (`.github/workflows/lock-threads.yml`): Runs hourly, auto-locks issues and PRs that have been inactive for 7 days. Uses `dessant/lock-threads@v5`.

## License

CC0 1.0 Universal — public domain dedication. See `LICENSE` for full text.

## Development Notes

- There is no build step, linter, or test suite. Changes are purely content edits to `README.md`.
- The only file that should be edited for content changes is `README.md`.
- Do not modify `awesome_hacking.jpg` or `LICENSE` unless specifically requested.
- When validating changes, check that links are well-formed URLs and entries are alphabetically sorted within their section.
