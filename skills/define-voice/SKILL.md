---
name: define-voice
description: Records the voice and the glossary the interface strings must share.
---

<p align="right">Language:&emsp;<img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-on.svg" align="middle" style="vertical-align:middle"> <a href="SKILL.es.md" style="vertical-align:middle"><img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-off.svg" align="middle" style="vertical-align:middle"></a></p>

[🏠 UX Writing](../../README.md)

# Records the voice and the glossary the interface strings must share

One term for one concept. The voice is a choice the person made, written down.

Source: ISO 24495-1:2023. The product style guide when one was given.

## Before writing

1. Read only [voice](references/voice.md) or [glossary](references/glossary.md).

References: [voice](references/voice.md), [glossary](references/glossary.md).

## Delivery

Every file this skill writes goes in `adrenaline/ux-writing/`, or in `outputDirs["plugin-ux-writing"]` when `.cursor/adrenaline.json` gives a valid relative path. If `adrenaline/ux-writing/` does not exist yet and `ux-writing/` at the project root already has this plugin's `ORIGIN.json` or `STATUS.md`, keep writing there and say so.

When the person names one project, app, service, or domain, put that subject's file in `<subject>/`. A file about the whole product stays at the output root. `<NNN>` is the next free number in the whole output folder. The `archivo` cell is `<subject>/<file>` when there is a subject (`doc/arch/adr-008-asunto-subcarpeta.md`).

Write `ORIGIN.json` beside `STATUS.md` when the folder is created, and again only if it is missing or a field differs. Fields: `suite` `ADRenaline-Suite`, `plugin` `plugin-ux-writing`, `repository` `https://github.com/ADRenaline-Suite/plugin-ux-writing`, `convention` `adr-001`. It is not an `<NNN>` file and it has no row in `STATUS.md`.

Do not invent a fact the person did not give. A required heading with no fact stays a gap and the file stays `proposed`. "None." fills a heading.

## Done

- [ ] Only the reference for this command was applied.
- [ ] The output folder, the subject subfolder, `ORIGIN.json`, and `STATUS.md` match the delivery rules.
- [ ] A missing required fact is a gap. The file stays `proposed`.

## Example

A request that names the piece and its source writes one file. A request missing that source writes nothing and names the gap.
