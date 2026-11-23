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
