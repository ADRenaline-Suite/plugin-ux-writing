<p align="right">Language:&emsp;<img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-on.svg" align="middle" style="vertical-align:middle"> <a href="README.es.md" style="vertical-align:middle"><img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-off.svg" align="middle" style="vertical-align:middle"></a></p>

# UX Writing (`plugin-ux-writing`)

Writes the string the interface shows, in each language the product already named, plus the voice and the glossary those strings share.

The instructions are in English. The file the plugin saves follows the language of the request. Files go in `adrenaline/ux-writing/`.

## /uxw-microcopy

One key. The button is a verb. One entry per language the product named.

## /uxw-errors

What is wrong and how to fix it. The typed value stays.

## /uxw-voice

Person, tense, and the words to use or avoid. A missing choice stays a gap.

## /uxw-glossary

One term for one concept.

## /uxw-clarity

A quoted string, what blocks it, and one replacement.

## /uxw-consistency

Two strings for one concept, and the term that wins.

## /uxw-purpose

The personal purpose, the audience, and the channels the person named. It is not interface copy.

## Help

## /uxw-help

The catalog of this plugin. It does not write a file.

## Who it is for

Someone who needs the words on a screen. The layout stays with `plugin-ui-ux-design`. The WCAG audit stays with `plugin-accessibility`. A marketing page is not this plugin. This plugin does not copy their skills.

## What it includes

Portable, for any agent that follows [Agent Skills](https://agentskills.io/specification):

- `write-ui-copy` writes a label, a button, or an error.
- `define-voice` records the voice and the glossary.
- `review-copy` reviews a string for clarity or for one term per concept.
- `write-brand` records a personal-brand statement the person already made.

Cursor and Claude Code: the commands above. In Cursor, `/uxw-microcopy`. In Claude Code, `/plugin-ux-writing:uxw-microcopy`.

Cursor only: rules `output-folder`, `no-invented-voice`. Claude Code does not load rules. The same restrictions are in the skills.

## Install

In Cursor, install the plugin from this repository in Customize.

In Claude Code:

```text
claude plugin marketplace add ADRenaline-Suite/plugin-ux-writing
claude plugin install plugin-ux-writing@plugin-ux-writing
```

To try a local copy, start Claude Code with `claude --plugin-dir <path to this repository>`.

## Example

Ask `/uxw-errors` and name the field. The file says what is wrong and how to fix it, in each language the product already named.

## Configuration

Files go in `adrenaline/ux-writing/`. One named screen goes in `<subject>/`. Languages are the ones the product already named.

## License

MIT. Copyright (c) 2026 Ricardo Plascencia.

