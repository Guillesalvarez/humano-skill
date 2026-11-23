# humano

Skill para Claude Code y OpenAI Codex que escribe o reescribe textos en español con una voz natural, evitando patrones habituales de la escritura con IA. Se basa en el catálogo de Wikipedia [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).

## Instalación

Clona el repositorio y entra en su carpeta:

```bash
git clone https://github.com/Guillesalvarez/humano-skill.git
cd humano-skill
```

### Claude Code

```bash
mkdir -p ~/.claude/skills
cp -R humano ~/.claude/skills/
```

### Codex

Para usar la skill en todos tus proyectos:

```bash
mkdir -p ~/.agents/skills
cp -R humano ~/.agents/skills/
```

Para instalarla solo en el proyecto actual, copia la carpeta en `.agents/skills/` dentro de ese proyecto. Inicia una sesión nueva para que Codex detecte la skill.

## Uso

- En Claude Code, escribe `/humano` seguido de un tema para redactar un texto, o de un texto para reescribirlo sin cambiar los hechos.
- En Codex, escribe `$humano` seguido de tus instrucciones o del texto que quieres reescribir. También puedes pedir que use la skill humano.

La misma skill funciona en ambos; no es necesario mantener dos versiones de sus instrucciones.


### ¿Por qué `/humano` en Claude Code y `$humano` en Codex?

Cada herramienta usa una forma distinta de invocar sus skills. Claude Code utiliza `/humano`, mientras que Codex permite mencionar la skill con `$humano`. En Codex, la barra `/` se usa para comandos de la aplicación.

Es la misma skill y conserva las mismas instrucciones en ambas herramientas; solo cambia la forma de llamarla. En Codex también puedes escribir, por ejemplo: «usa la skill humano para reescribir este texto». Para que la encuentre, primero debes instalarla en el entorno donde la vas a usar.
