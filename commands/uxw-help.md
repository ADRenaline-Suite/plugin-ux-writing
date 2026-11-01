---
name: uxw-help
description: "ADRenaline. Help: catalog of plugin-ux-writing (skills, rules, commands)."
---

# Help — ADRenaline UX Writing

Print this catalog as the reply. Do not run any skill or command. Do not invent entries that are not listed. If a component was added to the plugin and is missing here, add one line from its frontmatter `description` and say the catalog was refreshed.

When this help command is the first command in the message, every command, skill, or rule named after it is the subject of the help. Do not run those names. Do not print the full catalog. For each name, in the order given, print its catalog line (the linked id and the sentence). When the README has a heading for that command, also print the paragraphs under that heading, up to the next heading. A skill name uses the skill's catalog line and the README group that names that skill, up to its first command heading. A name that is not in this catalog is one line: it is not in this plugin. Do not invent what it does, and do not write a file.

Write the sentences in the language of the request. Keep command names, file ids, and every URL unchanged. Every id is a markdown link to the GitHub URL on its line. Do not print a repository `name` as the visible label of a plugin.

Keep the section headings, in this order: Plugin, Commands, Skills, Rules, then Agents, Hooks, and MCP when the plugin has them, then Output, then Not in this plugin. The title and the Plugin line show `ADRenaline` plus the `displayName`, then one sentence on what the plugin does. Under Commands, group the lines by the skill named in the line. Each group opens with that skill name linked to its SKILL.md. One line per item: the linked id, then the sentence. Output links this plugin's GitHub repository under that same label. A plugin under Not in this plugin uses `ADRenaline` plus its short name, and links to `https://github.com/<owner>/<other-plugin>` only when that repository exists.

## Plugin

- [**ADRenaline UX Writing**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/README.md) — Writes the string the interface shows, in each language the product already named.

## Commands

- [**/uxw-help**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/README.md) — This help (one-line catalog of the plugin).
- [**write-ui-copy**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/write-ui-copy/SKILL.md) — Writes one interface string: a label, an error, or a short instruction.
- [**/uxw-microcopy**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/write-ui-copy/references/microcopy.md) — Microcopy: the label, the button, the hint, and the empty state, one key per string.
- [**/uxw-errors**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/write-ui-copy/references/errors.md) — Error copy: what happened and how to fix it, next to the field.
- [**define-voice**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/define-voice/SKILL.md) — Records the voice and the glossary the interface strings must share.
- [**/uxw-voice**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/define-voice/references/voice.md) — Voice: how the product speaks, in choices the person already made.
- [**/uxw-glossary**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/define-voice/references/glossary.md) — Glossary: one term for one concept, in each language the product named.
- [**review-copy**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/review-copy/SKILL.md) — Reviews copy for clarity or for one term per concept.
- [**/uxw-clarity**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/review-copy/references/clarity.md) — Clarity review: a quoted string, what blocks understanding, the replacement.
- [**/uxw-consistency**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/review-copy/references/consistency.md) — Consistency review: two strings for one concept, and the term that wins.
- [**write-brand**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/write-brand/SKILL.md) — Records a personal-brand statement the person already made. It is not interface copy.
- [**/uxw-purpose**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/write-brand/references/purpose.md) — Personal brand: the purpose the person stated, who it is for, and which channels they named.

## Skills

- [**write-ui-copy**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/write-ui-copy/SKILL.md) — Writes one interface string: a label, an error, or a short instruction.
- [**define-voice**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/define-voice/SKILL.md) — Records the voice and the glossary the interface strings must share.
- [**review-copy**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/review-copy/SKILL.md) — Reviews copy for clarity or for one term per concept.
- [**write-brand**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/skills/write-brand/SKILL.md) — Records a personal-brand statement the person already made. It is not interface copy.

## Rules

- [**output-folder**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/rules/output-folder.mdc) — Every file goes in `adrenaline/ux-writing/` (or in `outputDirs["plugin-ux-writing"]` of `.cursor/adrenaline.json`). The artifact follows the language of the request.
- [**no-invented-voice**](https://github.com/ADRenaline-Suite/plugin-ux-writing/blob/main/rules/no-invented-voice.mdc) — Copy follows the product's style guide and the languages it named. The layout and the audit stay in their plugins.

## Output

- Repository: [**ADRenaline UX Writing**](https://github.com/ADRenaline-Suite/plugin-ux-writing).
- Folder: `adrenaline/ux-writing/`. One named subject goes in `<subject>/`. `<NNN>` is monotonic across the whole folder.

## Not in this plugin

- Layout and handoff → [**ADRenaline plugin-ui-ux-design**](https://github.com/ADRenaline-Suite/plugin-ui-ux-design).
- WCAG audit → ADRenaline plugin-accessibility.
- Marketing pages → ADRenaline plugin-documentation.
