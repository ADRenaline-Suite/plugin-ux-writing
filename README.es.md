<p align="right">Idioma:&emsp;<a href="README.md" style="vertical-align:middle"><img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-off.svg" align="middle" style="vertical-align:middle"></a> <img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-on.svg" align="middle" style="vertical-align:middle"></p>

# UX Writing (`plugin-ux-writing`)

Escribe la cadena que la interfaz muestra, en cada idioma que el producto ya nombró, más la voz y el glosario que esas cadenas comparten.

Las instrucciones están en inglés. El archivo que guarda el plugin sigue el idioma del pedido. Los archivos van en `adrenaline/ux-writing/`.

## /uxw-microcopy

Una clave. El botón es un verbo. Una entrada por idioma que el producto nombró.

## /uxw-errors

Qué está mal y cómo corregirlo. El valor escrito se conserva.

## /uxw-voice

Persona, tiempo verbal y las palabras a usar o evitar. Una elección que falta queda en hueco.

## /uxw-glossary

Un término para un concepto.

## /uxw-clarity

Una cadena citada, qué la estorba y un reemplazo.

## /uxw-consistency

Dos cadenas para un concepto, y el término que gana.

## /uxw-purpose

El propósito personal, la audiencia y los canales que la persona nombró. No es texto de interfaz.

## Ayuda

## /uxw-help

El catálogo de este plugin. No escribe un archivo.

## Para quién es

Quien necesita las palabras de una pantalla. El layout queda en `plugin-ui-ux-design`. La auditoría WCAG queda en `plugin-accessibility`. Una página de marketing no es este plugin. Este plugin no copia sus skills.

## Qué incluye

Portable, para cualquier agente que siga [Agent Skills](https://agentskills.io/specification):

- `write-ui-copy` escribe una etiqueta, un botón o un error.
- `define-voice` registra la voz y el glosario.
- `review-copy` revisa una cadena por claridad o por un término por concepto.
- `write-brand` registra un enunciado de marca personal que la persona ya dijo.

Cursor y Claude Code: los commands de arriba. En Cursor, `/uxw-microcopy`. En Claude Code, `/plugin-ux-writing:uxw-microcopy`.

Solo Cursor: las rules `output-folder`, `no-invented-voice`. Claude Code no carga rules. Las mismas restricciones están en los skills.

## Instalar

En Cursor, instala el plugin desde este repositorio en Customize.

En Claude Code:

```text
claude plugin marketplace add ADRenaline-Suite/plugin-ux-writing
claude plugin install plugin-ux-writing@plugin-ux-writing
```

Para probar una copia local, arranca Claude Code con `claude --plugin-dir <ruta de este repositorio>`.

## Ejemplo

Pide `/uxw-errors` y nombra el campo. El archivo dice qué está mal y cómo corregirlo, en cada idioma que el producto ya nombró.

## Configuración

Los archivos van en `adrenaline/ux-writing/`. Una pantalla nombrada va en `<subject>/`. Los idiomas son los que el producto ya nombró.

## Licencia

MIT. Copyright (c) 2026 Ricardo Plascencia.

