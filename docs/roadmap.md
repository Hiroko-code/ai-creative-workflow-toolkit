# Roadmap

This roadmap describes a cautious public release path for AI Creative Workflow Toolkit. The goal is to publish reusable creative workflow materials without exposing private project data, unpublished story material, local configuration, or generated assets.

## Phase 0: Public Starter Files

Status: proposed initial release

Scope:

- Project README
- Public release policy
- Storyboard template
- Prompt asset template
- Documentation-only repository structure

Out of scope:

- Source code copied from private tools
- API clients
- Private prompt libraries
- Reference images
- Generated images
- Imported chats or raw logs
- Databases and indexes
- Local agent configuration

## Phase 1: Workflow Templates

Goal: expand the toolkit with safe, reusable creative planning templates.

Candidate additions:

- Character brief template using placeholder examples only
- Location brief template
- Shot list template
- Page review checklist
- Prompt review checklist
- Model-agnostic image generation request template

Acceptance criteria:

- No private names, unpublished lore, or project-specific story beats
- No local paths or machine-specific setup
- No API keys, tokens, credentials, or secret-like examples
- No generated or reference images

## Phase 2: Optional Lightweight Utilities

Goal: add small, generic helper scripts only after a separate safety review.

Candidate additions:

- Markdown template validator
- Checklist generator
- Plain-text storyboard parser
- Prompt asset schema examples

Acceptance criteria:

- No network calls by default
- No provider-specific credentials
- No storage of raw prompts, logs, images, or personal data
- Clear tests or dry-run examples
- Public release policy updated before code is added

## Phase 3: Optional UI Prototype

Goal: explore a small local-first UI for editing templates.

Candidate additions:

- Minimal form-based prompt asset editor
- Storyboard markdown preview
- Export to plain Markdown or JSON

Acceptance criteria:

- No private project code copied directly
- No automatic upload or generation
- No bundled private assets
- No database required for first run
- Config files are optional and safe by default

## Long-Term Ideas

- Model-neutral prompt quality checklists
- Human review gates for generated art workflows
- Accessibility notes for visual storytelling templates
- Collaboration guidelines for writers, artists, and AI tool operators
- Example workflows using fully fictional placeholder content

## Release Discipline

Before every public release:

- Run a secret scan.
- Search for local paths.
- Confirm no image, database, raw log, import, sandbox, or external agent directory is included.
- Review all examples for private names or unpublished worldbuilding.
- Keep the release small enough to audit manually.
