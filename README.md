# AI Creative Workflow Toolkit

AI Creative Workflow Toolkit is a public, project-neutral collection of templates and workflow notes for AI-assisted manga, illustration, prompt, and storyboard production.

This repository is intended to start small. It does not include private project files, character lore, reference images, generated outputs, imported chats, databases, local paths, API keys, or agent configuration. The initial release focuses on safe documentation and reusable creative planning templates.

## What This Toolkit Helps With

- Planning manga pages and short visual sequences
- Describing characters, props, locations, and style constraints in a reusable way
- Preparing prompts for human review before using image or text generation tools
- Keeping storyboard decisions separate from private assets and production logs
- Documenting a safe public-release process for AI creative tools

## Initial Contents

```text
LICENSE
docs/
  roadmap.md
  public_release_policy.md
examples/
  storyboard_template.md
  prompt_asset_template.md
```

## Design Principles

- Keep private assets out of the public repository.
- Prefer templates over project-specific data.
- Make prompts reviewable before generation.
- Separate reusable workflow structure from unpublished story material.
- Avoid storing generated images, reference images, raw logs, imported chats, databases, or local machine configuration.

## Non-Goals For The Initial Release

- No application source code copied from private projects
- No provider-specific API integration
- No bundled model outputs
- No character universe, story bible, or unpublished creative setting
- No storage layer, database, import pipeline, or local agent setup

## Suggested Use

1. Copy this public starter set into a new repository.
2. Review `docs/public_release_policy.md` before adding any new file.
3. Use `examples/storyboard_template.md` for page or sequence planning.
4. Use `examples/prompt_asset_template.md` to describe prompt assets without attaching private references.
5. Add code only after a separate review confirms it contains no secrets, local paths, private data, or generated assets.

## Repository Name

Recommended public repository name:

```text
ai-creative-workflow-toolkit
```

## License

This starter set is released under the MIT License. See `LICENSE` for details.
