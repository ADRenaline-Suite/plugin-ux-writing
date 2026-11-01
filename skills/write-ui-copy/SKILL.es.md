---
name: write-ui-copy
description: Escribe una cadena de interfaz: una etiqueta, un error o una instrucción corta.
---

<p align="right">Idioma:&emsp;<a href="SKILL.md" style="vertical-align:middle"><img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-off.svg" align="middle" style="vertical-align:middle"></a> <img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-on.svg" align="middle" style="vertical-align:middle"></p>

[🏠 UX Writing](../../README.md)

# Escribe una cadena de interfaz: una etiqueta, un error o una instrucción corta

Un botón es un verbo. Un error dice cómo corregirlo y conserva lo que la persona escribió.

Source: ISO 24495-1:2023. GOV.UK Design System, componente de mensaje de error.

## Antes de escribir

1. Lee solo [microcopy](references/microcopy.md) o [errors](references/errors.md).

References: [microcopy](references/microcopy.md), [errors](references/errors.md).

## Entrega

Cada archivo de este skill va en `adrenaline/ux-writing/`, o en `outputDirs["plugin-ux-writing"]` si `.cursor/adrenaline.json` da una ruta relativa válida. Si `adrenaline/ux-writing/` aún no existe y `ux-writing/` en la raíz del proyecto ya tiene el `ORIGIN.json` o el `STATUS.md` de este plugin, sigue escribiendo ahí y dilo.

Si la persona nombra un proyecto, una app, un servicio o un dominio, el archivo de ese asunto va en `<subject>/`. Un archivo de todo el producto se queda en la raíz de la salida. `<NNN>` es el siguiente número libre en toda la carpeta. La celda `archivo` es `<subject>/<file>` cuando hay asunto (`doc/arch/adr-008-asunto-subcarpeta.md`).

Escribe `ORIGIN.json` junto a `STATUS.md` al crear la carpeta, y otra vez solo si falta o un campo difiere. Campos: `suite` `ADRenaline-Suite`, `plugin` `plugin-ux-writing`, `repository` `https://github.com/ADRenaline-Suite/plugin-ux-writing`, `convention` `adr-001`. No es un archivo `<NNN>` y no tiene fila en `STATUS.md`.

No inventes un dato que la persona no dio. Un título obligatorio sin dato queda como hueco y el archivo sigue `proposed`. "None." llena un título.

## Done

- [ ] Solo se aplicó la referencia de este command.
- [ ] La carpeta de salida, la subcarpeta del asunto, `ORIGIN.json` y `STATUS.md` coinciden con las reglas de entrega.
- [ ] Un dato obligatorio que falta es un hueco. El archivo sigue `proposed`.

## Example

Un pedido que nombra la pieza y su fuente escribe un archivo. Un pedido sin esa fuente no escribe nada y nombra el hueco.
