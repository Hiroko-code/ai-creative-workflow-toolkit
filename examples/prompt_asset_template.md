# Prompt Asset Template

Use this template to describe reusable prompt assets without attaching private images, local paths, unpublished character settings, or generated outputs.

## Asset Summary

- Asset ID: `asset_placeholder_001`
- Asset type: `character / location / prop / style / panel layout / correction note`
- Public-safe name: `Character A / Location A / Prop A`
- Intended use: `prompt planning / storyboard planning / human review`
- Status: `draft / reviewed / approved`

## Description

Write a short public-safe description.

```text
Example: Character A is a traveler with a simple cloak, readable silhouette, and calm expression.
```

Do not include:

- Private character lore
- Real personal information
- Local file paths
- Reference image filenames
- Generated image filenames
- Hidden production notes

## Visual Attributes

| Field | Value |
| --- | --- |
| Silhouette | `simple / angular / rounded / tall / compact` |
| Clothing | `generic outfit description` |
| Palette | `optional public-safe color notes` |
| Expression range | `calm, surprised, determined` |
| Pose constraints | `clear hands, readable face, stable proportions` |
| Style constraints | `manga line art, clean tones, no over-rendering` |

## Prompt Use

```text
Use this asset as a public-safe prompt description.
Preserve the listed visual attributes.
Do not infer private lore or add unlisted personal details.
```

## Negative Constraints

- Do not add private story details.
- Do not use real personal data.
- Do not include logos, copyrighted characters, or private reference filenames.
- Do not include local paths or hidden production metadata.
- Do not use this template as proof that a private image is publishable.

## Review Checklist

- [ ] No API keys or secret-like strings
- [ ] No local paths
- [ ] No private project names
- [ ] No private character names
- [ ] No reference image filenames
- [ ] No generated image filenames
- [ ] No imported chat excerpts
- [ ] No database or log references
- [ ] Safe to copy into a public repository

## Change Log

| Date | Change | Reviewer |
| --- | --- | --- |
| YYYY-MM-DD | Initial public-safe draft | Reviewer Name |
