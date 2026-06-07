# Public Release Policy

This policy defines what may be included in AI Creative Workflow Toolkit and what must stay out of the public repository.

## Core Rule

Only publish reusable, project-neutral workflow materials. Do not publish private project data, unpublished story content, generated assets, reference assets, logs, databases, local machine paths, credentials, or external agent configuration.

## Allowed

The following file types are acceptable when they contain only generic placeholder content:

- Markdown documentation
- Public roadmap notes
- Workflow checklists
- Storyboard templates
- Prompt asset templates
- Example schemas with fictional placeholder values
- Small utility code after a separate safety review

## Not Allowed

Do not include:

- API keys, tokens, passwords, access keys, secret keys, or credential files
- `.env` files
- Local absolute paths
- Generated images or videos
- Reference images
- Private character art
- Story bibles or unpublished lore
- Chat exports, imported conversations, MHTML files, raw logs, or transcripts
- Databases, SQLite files, search indexes, or cache files
- Backup archives, zip files, trash folders, or deleted project material
- Sandbox experiments
- External agent configuration
- Private prompt libraries
- Private project code copied without a separate public-safety review

## Required Pre-Release Checks

Run these checks before copying files into the public repository:

```bash
find . -type f \( -name ".env" -o -name "*.sqlite3" -o -name "*.db" -o -name "*.mhtml" -o -name "*.html" -o -name "*.zip" -o -name "*.png" -o -name "*.jpg" -o -name "*.jpeg" -o -name "*.webp" \)
```

```bash
rg -n "API_KEY|SECRET|TOKEN|PASSWORD|ACCESS_KEY|PRIVATE_KEY"
```

```bash
rg -n "/Users/|/home/|/private/|localhost|127\.0\.0\.1|\.venv|venv/"
```

```bash
rg -n "[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}"
```

Every match must be reviewed. A match is acceptable only when it is a generic policy example and not a real credential, path, email address, or private value.

## Template Safety Rules

Templates must:

- Use placeholder names such as `Character A`, `Location A`, or `Project Title`.
- Avoid unpublished story details.
- Avoid real-world personal data.
- Avoid references to private images, local files, or generated outputs.
- Include fields for human review before generation.

Templates must not:

- Embed base64 images.
- Link to private files.
- Include production logs.
- Include provider credentials.
- Mention private project names or character names.

## Adding Code Later

Code may be added only after a separate review confirms:

- It is generic and not copied from a private application without cleanup.
- It does not require secrets to start.
- It has safe fallbacks when optional config files are missing.
- It does not write raw logs, images, or databases by default.
- It does not upload files automatically.
- It has a clear README section explaining what data is stored, if any.

## Manual Copy Guidance

For the initial public repository, copy only:

- `README.md`
- `docs/roadmap.md`
- `docs/public_release_policy.md`
- `examples/storyboard_template.md`
- `examples/prompt_asset_template.md`

Do not copy the parent private repository, git history, generated files, reference assets, imports, raw logs, databases, sandbox folders, or external agent files.
