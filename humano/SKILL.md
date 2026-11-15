---
name: humano
description: Escribe o reescribe texto para que suene humano y no a IA, evitando los patrones de "Signs of AI writing" de Wikipedia. Úsala cuando el usuario invoque /humano, pida "humanizar" un texto, o pida redactar algo (correos, posts, artículos, README, mensajes, descripciones de PR) que no deba sonar a IA.
---

# /humano

Escribe (o reescribe) texto que suene a una persona concreta con algo que decir, no a un modelo de lenguaje. Basado en el catálogo de Wikipedia "Signs of AI writing".

## Cómo usarla

- `/humano <tema o instrucciones>`: redacta el texto desde cero.
- `/humano` + texto pegado: reescríbelo quitando los vicios de IA, sin cambiar los hechos.
- Responde en el idioma del usuario y entrega solo el texto final. No expliques qué cambiaste a menos que te lo pidan.

## Principio de fondo

La IA se va hacia lo estadísticamente común: hechos concretos se vuelven prosa genérica, positiva e inflada. La cura no es quitar palabras sueltas, es **ser específico**: nombres, cifras, fechas, ejemplos reales, una opinión clara. Si no tienes un dato concreto, di menos, no rellenes. No inventes datos ni fuentes.

## Lo que NO debes hacer

### 1. Contenido
- **Inflar importancia**: "es un testimonio de", "juega un papel crucial/clave/fundamental", "marca un hito", "subraya la importancia de", "refleja tendencias más amplias", "deja una huella imborrable", "panorama en constante evolución", "sentó las bases para". Di qué pasó y ya.
- **Análisis superficial con gerundio al final**: "...destacando su relevancia", "...fomentando la innovación", "...contribuyendo a". Corta la frase antes o pon un hecho.
- **Atribución vaga**: "los expertos coinciden", "algunos críticos señalan", "diversos medios". Nombra la fuente o quítalo.
- **Asociación vaga**: "vinculado a", "asociado con", "en relación con" sin decir cuál es el vínculo.
- **Notoriedad y cobertura mediática**: no justifiques que algo importa listando medios que lo mencionan. Tampoco "mantiene una fuerte presencia en redes".
- **Cierre de "desafíos y perspectivas"**: "A pesar de estos desafíos…", "De cara al futuro…", secciones tipo "Desafíos y legado". Termina cuando termines.
- **Resúmenes y conclusiones que repiten lo dicho**: "En resumen", "En conclusión", "En definitiva", párrafo final que reformula el principio.
- **Lenguaje promocional**: "vibrante", "rico", "enclavado en el corazón de", "innovador", "reconocido", "impresionante", "amplia gama de".
- **Muletillas de relleno y avisos**: "es importante señalar/recordar que", "cabe destacar", "vale la pena mencionar", "no hay mucha información disponible", "mantiene un perfil bajo".
- **Marcos correctivos** (modelos recientes): "debe tratarse como X y no como Y", "no establece por sí mismo que", "no debe confundirse con".
- **Declaraciones de límite de conocimiento o rechazos**: "hasta mi última actualización", "como modelo de lenguaje".

### 2. Lenguaje y gramática
- **Vocabulario de IA en densidad**: crucial, fundamental, clave (como adjetivo comodín), pivotal, robusto, vibrante, intrincado, tapiz (metafórico), panorama (abstracto), sumergirse/adentrarse ("delve"), destacar/resaltar (verbo), subrayar, potenciar, fomentar/cultivar, aprovechar ("leverage"), multifacético, atractivo, "no solo… sino también", además (al inicio de frase), "valioso". Una palabra suelta no delata; varias juntas sí. Los modelos nuevos añaden: desafío, priorizar, discretamente, constante, práctico, "importa".
- **Evitar "es/son/tiene"**: "sirve como", "se erige como", "representa", "cuenta con", "ofrece", "funciona como", "se presenta como". Usa **ser, estar, tener** cuando eso es lo que quieres decir.
- **Paralelismos negativos**: "No es solo X, es Y", "No se trata de X, sino de Y", "sin X, sin Y, solo Z", "en lugar de X" como muletilla. Afirma lo que es.
- **Regla de tres automática**: tríadas de adjetivos o frases para sonar completo. Usa dos o cuatro, o uno solo, según lo que haya.
- **Variación elegante**: no cambies el nombre del sujeto en cada frase ("el artista", "el creador", "el maestro"). Repite el nombre o usa un pronombre.
- **Primera frase de definición a un título genérico**: "X se refiere a…", "X es una lista/recopilación curada de…". Entra directo.

### 3. Estilo y formato
- **Negritas** dispersas en la prosa, listas con etiqueta en negrita ("**Concepto:** explicación"), **encabezados en Title Case**, emojis al inicio de títulos o viñetas, encabezado de nivel 1 que repite el título. Si el texto es prosa, escribe prosa.
- **Estructura de esquema**: secciones y viñetas donde bastarían dos párrafos.
- **Comillas y apóstrofos tipográficos** (“ ” ’) cuando el contexto usa rectos.
- **Guiones largos (—)** en exceso o donde van comas, paréntesis o dos puntos. Úsalos poco o nada. Ojo: los modelos nuevos compensan abusando de comas y frases cortas de 8 a 20 palabras todas parecidas; varía el ritmo.
- **Títulos de sección enlatados**: "Premios y reconocimientos", "Desafíos y legado", "Perspectivas futuras", "Sobre mí / Mis intereses".

### 4. Comunicación con el usuario (nunca en el texto entregado)
- "¡Claro!", "¡Por supuesto!", "Espero que esto ayude", "¿Quieres que…?", "Avísame si…", "Aquí tienes…", "¡Excelente pregunta!", "Tienes toda la razón".
- Texto de relleno entre corchetes sin completar: `[Tu nombre]`, `[Insertar URL]`, `2025-XX-XX`.
- Tono de atención al cliente: disculpas innecesarias, "he revisado cuidadosamente", "agradezco tu comprensión".

### 5. Citas y referencias
- No inventes DOI, ISBN, URLs, páginas, autores ni citas. Si no tienes la fuente, no la cites.
- Elimina parámetros de rastreo como `utm_source=openai` o `utm_source=chatgpt.com` de cualquier enlace.
- Referencias a libros sin página, enlaces sospechosos o genéricos (example.com) son señal de alucinación.

### 6. Mensajes de commit, PR y resúmenes de cambios
- Evita las fórmulas: "garantiza el cumplimiento de", "mejora la claridad y el flujo", "refinado, mejorado, optimizado", "preservando el significado original", "se evitó…", "se añadieron fuentes verificadas".
- Di qué cambió y por qué en una frase concreta. Sin listar parámetros o nombres de plantillas uno por uno.

## Qué SÍ hace una persona

- Dice cosas concretas: quién, cuándo, cuánto, dónde.
- Usa palabras simples: "escribió" y no "fue autor de", "murió" y no "falleció", "usar" y no "utilizar/aprovechar".
- Acepta afirmaciones directas ("es el mejor", "fue el primero") cuando son ciertas y está sustentado, y usa matices solo cuando de verdad hay duda ("quizá", "suele", "bastante").
- Varía la longitud de las frases. Alguna corta. Alguna larga que se permite un par de subordinadas.
- Se queda en el tema y se calla cuando ya lo dijo. Sin párrafo de cierre.
- Tiene voz: una opinión, una objeción, un detalle raro, un ejemplo que solo conoce quien lo vivió.
- Respeta el registro de quien lo firma. Si el usuario escribe informal, el texto sale informal.

## Señales que NO son prueba de IA (no las "arregles")

Gramática perfecta, registro formal, un "además" o "sin embargo" suelto, prosa académica, o texto sin fuentes. No empeores un texto bueno para que parezca torpe. No metas errores a propósito.

## Proceso

1. **Entiende el propósito, el lector y la voz.** Si el usuario dio muestras de su escritura, imítalas.
2. **Reúne los hechos concretos.** Si faltan, pregunta o escribe menos; no rellenes.
3. **Redacta en prosa**, directo, sin introducción ni cierre de cortesía.
4. **Revisa contra las listas de arriba.** Busca: vocabulario de IA, "sirve como", "no solo… sino", tríadas, gerundios de cierre, guiones largos, negritas, resumen final, frases de la misma longitud. Reescribe lo que salte.
5. **Lee en voz alta mentalmente.** ¿Lo diría alguien así? Si suena a folleto o a ensayo escolar, bájalo a tierra.
6. **Entrega solo el texto.** Una nota breve solo si hubo que suponer un dato o falta información.

## Ejemplo

IA: "El café Aurora se erige como un testimonio vibrante de la rica tradición cafetera de la ciudad, ofreciendo a sus visitantes una experiencia única y contribuyendo a fortalecer la identidad cultural del barrio."

Humano: "El café Aurora abrió en 1987 en la calle Mercaderes. Tiene doce mesas, tuesta el grano en el local y casi todo el mundo pide el cortado."
