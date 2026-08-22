# Análisis de la referencia: AI Operators (Polonia)

Fecha del análisis: 2026-08-22
Fuentes: `materiales/fuentes/web-aioperators/` y `materiales/fuentes/webinar-damian-naprawa/`

---

## 0. Advertencia metodológica

Lo que tenemos son **dos piezas de un embudo de venta**, no el curso:

- La **web** (`aioperators.pl`) es la *promesa*: dice qué vas a saber hacer al
  terminar, semana a semana. Está redactada como argumentario comercial, así que
  describe resultados, no contenidos.
- El **webinar** de 1 h 57 min es el *gancho*: enseña el método a alto nivel y una
  demo, y deliberadamente se queda corto para que compres el programa.

El contenido real de las 20 lecciones está detrás del pago. Todo lo que sigue es
una reconstrucción desde fuera. Es suficiente para saber **qué enseñan y con qué
lógica**, pero no para copiar su temario — y, como argumento más abajo, tampoco
querríamos copiarlo.

Todo el material está en polaco. Las citas van traducidas.

---

## 1. Qué es el programa de referencia

**AI Operators**, primera edición.

| | |
|---|---|
| Formato | 5 semanas, cohorte con fecha fija |
| Inicio | 26 de octubre de 2026; primer LIVE el martes 27 |
| Ritmo | 4 lecciones por semana (vídeo + texto) + 1 sesión LIVE semanal |
| LIVEs | 27.10 · 05.11 · 12.11 · 19.11 · 26.11 (jueves a partir de la 2.ª semana) |
| Precio | 995 zł netos en preventa (orden de magnitud: ~230 €), 1 223,85 zł con IVA |
| Preventa | hasta el 2 de septiembre |
| Extras | feedback de mentores, comunidad, 12 meses de acceso, certificado al entregar el proyecto, 7 días de garantía |

**Mentores.** Aleksandra Zajączkowska (AI Engineer, 7+ años, formadora de la
"Eskadra" del modelo polaco Bielik) y Damian Naprawa (arquitecto de sistemas,
marca *wKontenerach*, dice haber formado a 5 000+ alumnos de pago y 20-30 000 en
formaciones gratuitas).

**Posicionamiento.** Se dirigen a la vez a dos públicos —no técnicos y
ingenieros IT— con el mismo tronco durante 4 semanas y bifurcación en la 5.ª. Es
una decisión comercial (duplica el mercado direccionable) que tiene un coste
pedagógico evidente: el tronco tiene que ser lo bastante genérico para no perder
a ninguno de los dos.

**Definición que dan del rol:**

> "Una persona que sabe diseñar un sistema así es un AI Operator."

Y, con honestidad, en el propio webinar:

> "No os apeguéis al nombre, porque el mercado cambia muy rápido y cada empresa
> lo llama distinto: a veces AI Product Builder, a veces Solution Engineer."

---

## 2. El método: los cinco pasos

Es el esqueleto del webinar y, por lo que se ve, del programa entero.

### Paso 1 — Modelo, automatización o agente

La competencia que hay detrás: **fluidez en herramientas de IA**, entendida no
como saber usar muchas, sino como **saber cuál toca**.

El árbol de decisión que dan, y que es lo más aprovechable de todo el webinar:

```
                       TAREA
                         │
        ¿tiene pasos definidos y repetibles?
                 │                    │
                SÍ                    NO
                 │                    │
          AUTOMATIZACIÓN         MODELO DE LENGUAJE
          (n8n, Make)                  │
       "el mismo camino          ┌─────┴─────┐
        siempre"               CHAT        AGENTE
                            pregunta/    proceso complejo,
                            respuesta,   multietapa, precisa
                            brainstorm   juicio y herramientas
                                         (Claude Code, Codex)
```

El ejemplo con el que lo explican: escanear una factura, pasar los datos a Excel
y calcular algo, siempre igual → **eso no necesita IA**, necesita una
automatización. Y al revés: un research de mercado donde los pasos se van
decidiendo sobre la marcha → agente.

Insisten en dos direcciones del error, no solo en una:

> "Saber cuándo un agente es *overkill*. Si solo quieres hacer una lluvia de
> ideas, no hace falta meter ahí un Claude Code."

Y sitúan honestamente dónde está el alumno medio:

> "El primer nivel es usar el chat como un buscador un poco más sofisticado. Y la
> mayoría de la gente se queda en ese nivel."

### Paso 2 — Describir la tarea que delegas

La competencia: **pensamiento sistémico**. Antes de tocar nada, mapear:

- **Entradas** — qué datos hacen falta (webs, tarifas, número de competidores…)
- **Herramientas** — de dónde salen esos datos (Notion, Airtable, Firecrawl…)
- **Decisiones** — dónde hay juicio, qué hay que actualizar, qué es no determinista
- **Resultado** — qué formato tiene que tener la salida

El mapa mismo es el que te dice qué solución toca: si aparecen varias
herramientas, varias etapas y juicio crítico, ya sabes que es un agente.

### Paso 3 — Contexto y conocimiento de la empresa

El paso central, y donde ponen la demo. Se apoya en una tríada:

| | Qué es |
|---|---|
| **Fuentes de verdad** | Hechos, desde una sola dirección |
| **Memoria** | Acuerdos que permanecen entre sesiones |
| **Skill** | La forma de trabajar: pasos y formato de salida |

La demo es un **"LLM Brain"**: una base de datos en grafo montada en **Obsidian**,
alimentada por **Claude Code** + **Firecrawl** (scraping) + conectores a Notion y
Airtable, y organizada por un *skill* que le dice al agente cómo ordenar lo que
recoge.

El caso trabajado: análisis de competencia de agencias de marketing en Polonia.
Recopila un listado de 60 agencias y desarrolla el análisis sobre un grupo
reducido de competidores. Salida final: un artefacto HTML navegable ("radiografía
del mercado de agencias") con posicionamiento, precios, garantías, arquetipos de
claim y recomendaciones.

Dicen explícitamente —y es el argumento de venta clave— que **no hace falta
programar**:

> "Lo que os estoy enseñando lo puede montar hasta una persona que trabaja en una
> caja de supermercado. Aquí no hace falta programación; solo hace falta entender
> cómo funciona y saber transmitir el contexto, que es lo que tenéis vosotros como
> especialistas."

Y la frase que resume su tesis entera:

> "Antes se decía que los datos eran el petróleo. Ahora el petróleo es el contexto."

### Paso 4 — Acceso a herramientas

La competencia: **capacidad de prototipar**. Pero el contenido real del paso es
de seguridad y alcance:

- conectar el agente **solo** a las herramientas necesarias
- darle **una carpeta concreta**, no el disco entero
- el humano se queda como verificador: revisa, aprueba, itera

En la web esto está más desarrollado que en el webinar: rol definido, permisos
mínimos, criterios de éxito, y "el humano aprueba las acciones que escriben".

### Paso 5 — Evaluación de la calidad del resultado

El paso que casi ningún curso de IA incluye, y el que ellos ponen al final a
propósito:

- **casos de prueba** fijos: una conexión o un concepto que el sistema *debería*
  detectar, con su consulta asociada
- volver a lanzarlos cuando el sistema crece: *"si le metes 15 ficheros más,
  ¿empieza a perderse y a responder peor?"*
- medir **degradación en el tiempo**, no solo acierto puntual
- y por encima de todo: **¿esto resuelve de verdad el problema de negocio?**

> "Hay muchísimo hype con la IA y pensamos que puede resolverlo todo, pero es solo
> tecnología. Al final diseñas una solución para resolver un problema concreto."

En la web añaden dos cosas que no salen en el webinar y que son buenas: enseñar
al agente a **decir "no lo sé"** cuando faltan datos, y a **citar el fichero
concreto** del que sale cada respuesta.

### El cierre honesto

Lo mejor del webinar es el último minuto de la parte técnica:

> "Ves el resultado. Detrás hay varias decenas de intentos."
>
> "Trabajar con un modelo de lenguaje es siempre trabajo iterativo. Quiero cerrar
> matando el hype, porque me pone de los nervios que la gente piense que esto es
> una varita mágica."

Y el diagnóstico de Damian, que es la mejor frase para abrir *nuestro* curso:

> "El problema no está en el modelo. Da bastante igual qué modelo uses mientras no
> gastes miles en tokens. El problema es que cada vez le explicas tu empresa desde
> cero."

---

## 3. La estructura de las 5 semanas

Semanas 1-4 tronco común; en la 5.ª se elige itinerario (y se conservan los dos).

**Semana 1 — De la tarea al proyecto de IA.** Dejar de elegir herramienta a ojo:
evaluar la tarea por valor, riesgo y resultado esperado. Elegir entre GPT, Claude
y Gemini según calidad/riesgo/presupuesto. Convertir una petición vaga en una
especificación con objetivo, contexto, restricciones y formato. Salir de la
ventana de chat hacia un "proyecto" que conoce ficheros y reglas.
→ *Entregable: auditoría de un proceso propio con veredicto chat / workflow / agente.*

**Semana 2 — Agente, herramientas y acceso seguro.** Elegir la tarea repetitiva
cuya cesión libera tiempo de verdad y escribir un criterio medible de "trabajo
bien hecho". Conectar por MCP a una fuente real sin darle acceso a toda la
empresa. Diseñar rol, límites y **condiciones de parada** (cuándo actúa y cuándo
te pregunta). Probar con al menos 5 casos: correctos, límite y erróneos.
→ *Entregable: agente funcionando contra una fuente, con acceso limitado y escenarios de prueba.*

**Semana 3 — Contexto, memoria y skills propios.** Fichero de contexto que hace
que el agente conozca la empresa desde el primer mensaje. **Jerarquía de fuentes
de verdad** para que las instrucciones contradictorias no acaben en una decisión
al azar. Memoria controlada: guarda decisiones y preferencias, no guarda datos
sensibles ni acuerdos caducados. Convertir un procedimiento en un *skill* con
condiciones de disparo, entrada requerida, límites y formato fijo.
→ *Entregable: paquete de contexto + un skill que reproduce un procedimiento.*

**Semana 4 — Base de conocimiento que conoce sus fuentes.** Mapear documentos,
decisiones y procedimientos y elegir arquitectura: RAG, búsqueda o grafo. Que el
agente cite el fichero. Que sepa decir "no lo sé". Distinguir documento caducado
de decisión vigente. Preguntas de control y reglas de actualización.
→ *Entregable: base de conocimiento con citas, regla de "no lo sé" y batería de preguntas de control.*

**Semana 5A — No técnicos.** Inteligencia competitiva: mapear mercado y 3-5
competidores, construir un operador que convierte evidencias, fechas y grado de
confianza en un informe con recomendaciones; empaquetarlo en un prototipo de app
y una landing.

**Semana 5B — Ingenieros.** Servidor MCP propio con acceso controlado a APIs,
logs y runbooks; operador con modos `/status`, `/debug` e `/incident`; validación,
permisos mínimos, auditoría y confirmación humana para toda escritura.

**Herramientas que declaran:** Claude Code, OpenAI Codex, ChatGPT, Gemini,
Obsidian, MCP, Lovable, API, Git, RAG.

---

## 4. Qué nos sirve

1. **Los cinco pasos como columna vertebral.** Son correctos y están bien
   ordenados: primero decidir el tipo de solución, luego especificar, luego
   contexto, luego acceso, luego evaluación. Ese orden se sostiene en cualquier
   dominio.
2. **El árbol de decisión del paso 1.** Es exactamente el modelo mental que le
   falta a alguien que usa el chat como buscador. Y el mérito está en que corta en
   los dos sentidos: hay tareas que no necesitan IA en absoluto.
3. **La tríada fuentes de verdad / memoria / skill.** Nombra bien tres cosas que
   los principiantes mezclan continuamente.
4. **La evaluación como paso de primera clase**, con casos correctos, límite y
   erróneos, y con la pregunta de si el sistema se degrada al crecer.
5. **"No lo sé" + cita de la fuente.** En atención al cliente esto no es un
   refinamiento, es el requisito que separa una herramienta usable de un
   generador de problemas.
6. **El tono anti-hype.** Reconocer que detrás de la demo hay decenas de intentos
   es lo que evita que la alumna abandone en el primer resultado mediocre.

---

## 5. Qué no transfiere

1. **La mitad del valor del programa es la cohorte.** LIVEs semanales, feedback
   de mentores, comunidad, ver los proyectos de otros, entregar para que te
   corrijan. Nuestro curso es autodidacta y personal: **nada de eso existe**. Si
   copiamos su estructura sin más, copiamos un esqueleto al que le falta el
   músculo. Todo lo que allí resolvía un mentor aquí tiene que resolverlo el
   material: rúbricas, soluciones comentadas, autodiagnóstico y criterios
   explícitos de "esto está bien / esto está mal".

2. **La demo es el dominio equivocado.** Análisis de competencia de agencias de
   marketing. Nuestra alumna hace atención al cliente en una academia de idiomas.
   El caso hay que sustituirlo entero, no adaptarlo: si el ejemplo no es su
   trabajo, vuelve al modo "leo el curso" en lugar de "monto lo mío".

3. **El grafo de Obsidian es atrezzo de webinar.** Es visualmente espectacular —
   por eso está ahí. Para un puesto de atención al cliente, el artefacto útil es
   mucho más aburrido: una base de respuestas con fuente y fecha, un triador de
   incidencias, un redactor de respuestas con reglas de tono. El grafo es una
   opción de implementación, no un objetivo de aprendizaje.

4. **El doble público diluye.** Nosotros tenemos *una* alumna y sabemos su puesto.
   Podemos ser mucho más específicos que ellos, y ahí está nuestra ventaja real.

5. **Dan por supuesto Claude Code.** Para alguien que hoy solo abre chatgpt.com,
   una terminal es una barrera seria y temprana. Hay que decidir conscientemente
   la escalera de herramientas en lugar de heredar la suya.

---

## 6. Huecos del programa de referencia

Cosas que, con el material disponible, no aparecen en ningún sitio y que en
nuestro caso son obligatorias:

- **Protección de datos.** Ni una mención. Nuestra alumna maneja datos de
  estudiantes extranjeros: pasaportes, cartas para visado, alojamiento, pagos,
  posiblemente menores. Meter eso en una herramienta de IA sin criterio es el
  riesgo más real de todo el proyecto, y va antes que cualquier prototipo.
- **Vender la idea dentro de la empresa.** Su itinerario no técnico acaba en
  landing y portfolio, es decir, orientado a *cambiar de trabajo*. El objetivo de
  nuestra alumna es el contrario: que en su empresa le digan que sí. Eso es un
  módulo entero que allí no existe: alcance de piloto, riesgos, coste, a quién se
  lo cuentas y cómo mides que funcionó.
- **Coste y licencias reales.** Firecrawl, conectores, Airtable, planes de pago.
  En una pyme de 30 personas eso es una conversación con quien firma.
- **Qué hacer cuando el agente se equivoca delante de un cliente.** Plan de
  degradación, revisión humana previa al envío, trazabilidad.
- **Multilingüe.** Su alumnado es polaco trabajando en polaco. La nuestra atiende
  a estudiantes extranjeros, previsiblemente en varios idiomas. Cambia el diseño
  de la base de conocimiento y de las pruebas.
