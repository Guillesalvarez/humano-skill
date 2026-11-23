# humano

Skill para Claude Code y OpenAI Codex que escribe o reescribe textos en español con una voz natural, evitando patrones habituales de la escritura con IA. Se basa en el catálogo de Wikipedia [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).

## Instalación

En macOS o Linux, abre la Terminal y copia el bloque completo de la herramienta que uses. Cada bloque descarga la skill desde este repositorio; no necesitas clonar el proyecto. Para actualizarla, ejecuta nuevamente el mismo bloque: reemplazará el archivo `SKILL.md` instalado.

### Claude Code

```bash
mkdir -p ~/.claude/skills/humano && curl -fL https://raw.githubusercontent.com/Guillesalvarez/humano-skill/main/humano/SKILL.md -o ~/.claude/skills/humano/SKILL.md
```

### Codex

Para usarla en todos tus proyectos:

```bash
mkdir -p ~/.agents/skills/humano && curl -fL https://raw.githubusercontent.com/Guillesalvarez/humano-skill/main/humano/SKILL.md -o ~/.agents/skills/humano/SKILL.md
```

Para instalarla solo en el proyecto actual, ejecuta este comando desde la carpeta del proyecto:

```bash
mkdir -p .agents/skills/humano && curl -fL https://raw.githubusercontent.com/Guillesalvarez/humano-skill/main/humano/SKILL.md -o .agents/skills/humano/SKILL.md
```

## ¡Reinicia!

Después de instalar la skill, cierra y vuelve a abrir Codex o Claude Code para que la detecte. Luego inicia una conversación nueva y escribe `$humano` en Codex o `/humano` en Claude Code.

## Uso

- En Claude Code, escribe `/humano` seguido de un tema para redactar un texto, o de un texto para reescribirlo sin cambiar los hechos.
- En Codex, escribe `$humano` seguido de tus instrucciones o del texto que quieres reescribir. También puedes pedir que use la skill humano.

La misma skill funciona en ambos; no es necesario mantener dos versiones de sus instrucciones.


### ¿Por qué `/humano` en Claude Code y `$humano` en Codex?

Cada herramienta usa una forma distinta de invocar sus skills. Claude Code utiliza `/humano`, mientras que Codex permite mencionar la skill con `$humano`. En Codex, la barra `/` se usa para comandos de la aplicación.

Es la misma skill y conserva las mismas instrucciones en ambas herramientas; solo cambia la forma de llamarla. En Codex también puedes escribir, por ejemplo: «usa la skill humano para reescribir este texto». Para que la encuentre, primero debes instalarla en el entorno donde la vas a usar.
