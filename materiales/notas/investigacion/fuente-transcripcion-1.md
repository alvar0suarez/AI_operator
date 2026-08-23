# Fuente 1 — Webinar Damian Naprawa / Ola Zajączkowska · Tramo 00:00:00 – 00:40:00

**Vídeo:** «LIVE: Jak zbudować system AI, który zna Twoją pracę i przejmuje jej powtarzalną część»
(«Cómo construir un sistema de IA que conoce tu trabajo y se hace cargo de su parte repetitiva»)
**Fuente:** https://www.youtube.com/watch?v=xRd75ejF-5I · uploader: Damian Naprawa · idioma: polaco
**Duración real:** 01:56:59 (7019 s) — **prometen 90 minutos en el minuto 00:00:38**
**Ponentes:** Aleksandra («Ola») Zajączkowska (AI Engineer, hace ~90 % del contenido técnico) y Damian Naprawa (apertura, cierre, venta)
**Embudo:** el webinar es el gancho de `aioperators.pl` → programa de pago «AI Operators», 5 semanas, 995 zł netos (1223,85 zł brutos), preventa hasta el 2 de septiembre, arranque el 26 de octubre.
**Archivos usados:** `transcripcion.md` (líneas 1–1000 ≈ 00:00:00–00:40:57), `informe.md` (OCR de pantalla, líneas 61–800), frames `0019`, `0024`, `0027`, `0032`, `0034`, `0035`.

> **Aviso de lectura obligatorio.** La transcripción es ASR y destroza sistemáticamente los nombres propios. Ver §10 antes de citar nada literal.

---

## 0. Mapa del tramo (qué pasa y cuándo)

| Tramo | Bloque | Quién | Naturaleza |
|---|---|---|---|
| 00:00:25 – 00:03:22 | Apertura, público objetivo, anti-hype («no habrá 50 prompts») | Damian | **Venta** (encuadre) |
| 00:03:39 – 00:04:56 | «LLM Second Brain» + acuñación de «AI Operator» | Damian | **Venta** (naming del producto) |
| 00:05:04 – 00:07:31 | Bios, prueba social, marca wKontenerach | Ambos | **Venta** |
| 00:07:32 – 00:07:47 | Las 3 preguntas de gobernanza del sistema | Damian | **Docencia real** (10 s, la joya escondida) |
| 00:07:48 – 00:08:50 | Regalo por asistencia en directo (web en 4 tardes + cómo vender) | Damian | **Venta** (retención) |
| 00:09:06 – 00:13:35 | Los 5 pasos + «esto es lo que busca el mercado» | Ola | **Venta con envoltorio docente** |
| 00:13:38 – 00:14:10 | «Todo esto sin programar» | Ola | **Venta** (claim frágil) |
| 00:14:27 – 00:19:50 | **PASO 01** — Modelo / automatización / agente. Árbol de decisión | Ola | **Docencia real** (el mejor bloque) |
| 00:19:54 – 00:22:20 | Ejemplo elegido (análisis de competencia) + 4 usos alternativos | Ola | Docencia real |
| 00:22:21 – 00:24:10 | **PASO 02** — Especificación de la tarea (entradas/herramientas/decisiones/resultado) | Ola | **Docencia real** |
| 00:24:19 – 00:27:28 | Por qué el modelo necesita memoria externa · LLM Brain | Ola | Docencia real + claim de accesibilidad |
| 00:27:33 – 00:29:29 | **PASO 03** — Pipeline: fuentes → Obsidian → skill | Ola | Docencia real **pero sin el «cómo»** |
| 00:29:30 – 00:34:59 | Demo en Obsidian: grafo, clústeres, conceptos | Ola | Demo (docencia por observación) |
| 00:35:00 – 00:40:00 | Dashboard de resultados «Rentgen rynku agencji» + trabajo ejecutor→supervisor | Ola | Docencia real (el mejor insight del tramo) |

**Dato estructural:** en el minuto 00:09:42 anuncian 5 pasos. Al minuto 40:00 solo se han tocado 01, 02 y 03 (este último a medias). **Los pasos 04 (acceso a herramientas) y 05 (evaluación de calidad) no existen todavía en este tramo** — y son precisamente los dos que la web vende como semanas 3-4 del programa de pago.

---

## 1. Inventario de afirmaciones enseñables

### 1.1 Encuadre (00:01:10 – 00:04:00)

- **[00:01:10]** Hay dos públicos para este tipo de sistema: quien empieza y quiere entender los fundamentos, y quien ya usa IA y quiere aprender a construir un sistema que entienda su trabajo. El objetivo en ambos casos es el mismo (según diapositiva OCR): *«przejść od dorywczego używania AI do systemu pracy»* = **«pasar del uso ocasional de la IA a un sistema de trabajo»**. Ese es el eje pedagógico de todo el material.
- **[00:01:51]** Diagnóstico del nivel base del público: mucha gente usa la IA solo como buscador mejor que Google — escribe al chat, copia, obtiene una respuesta. Es la línea de partida que el curso asume.
- **[00:03:07]** **Tesis central del webinar:** la ventaja no está en un prompt, sino en un contexto bien configurado, alimentado por conocimiento, herramientas y reglas adecuadas. Eso es lo que compone un «sistema».
- **[00:03:39]** Nombre que le dan al artefacto: **LLM Second Brain** — «donde la IA entiende tu contexto: empresas, documentos, decisiones, procesos».
- **[00:03:55]** Definición del rol: **AI Operator** = «la persona capaz de diseñar ese sistema». Es una competencia, no una herramienta.

### 1.2 Gobernanza (00:07:32) — el bloque más denso y más corto

**[00:07:38]** Tres preguntas obligatorias antes de construir cualquier sistema de este tipo:
1. ¿Qué tiene que saber la IA sobre tu empresa / tu trabajo?
2. ¿De dónde sabe **en qué fuentes confiar**?
3. ¿Dónde conserva el control el humano? ¿Dónde debe aprobar cosas el humano?

> Estas tres preguntas son, comprimidas, el temario entero: (1) contexto, (2) jerarquía de fuentes de verdad, (3) puntos de aprobación humana. Duran 10 segundos y **no se responden en las 33 minutos siguientes**. La pregunta 2 se roza en el minuto 35 (fuentes de verdad como concepto) y la 3 **no se toca en absoluto** en este tramo.

### 1.3 PASO 01 — Fluidez en herramientas de IA (00:14:27 – 00:19:50)

- **[00:14:32]** Antes de resolver nada hay que saber **con qué** se resuelve: modelo, automatización o agente. Esa elección es el primer paso, no un detalle de implementación.
- **[00:14:48]** Lo presentan como un *«esquema mental»* (schemat myślowy) para pensar en alto nivel antes de arrancar.
- **[00:15:12]** **La pregunta bisagra del árbol:** «¿Tiene la tarea pasos definidos y repetibles?» (*«Ma określone, powtarzalne kroki?»*).
- **[00:15:17]** **Si SÍ → probablemente la solución no es IA en absoluto, es automatización.** Enseñanza contraintuitiva y la más valiosa del bloque.
- **[00:15:40]** Criterio operativo de «pasos definidos»: *no hay ninguna dosis de pensamiento crítico*; es un algoritmo simple, se puede escribir en pasos siempre idénticos.
- **[00:15:54]** **Si NO → posiblemente un modelo de lenguaje sea la buena solución.** Ojo al «posiblemente».
- **[00:16:17]** Dentro de los modelos de lenguaje hay **dos opciones**: (A) usarlo en la ventana de chat; (B) usar un agente.
- **[00:16:40]** El chat es «el primer nivel» de uso de LLM: preguntas y lluvia de ideas.
- **[00:16:46]** **«Y la mayoría de la gente se detiene en ese nivel.»** — el diagnóstico que justifica todo el producto.
- **[00:17:00]** El agente es «el nivel superior»: se le deja entrar a un proceso complejo, multietapa y que a menudo exige pensamiento crítico — no solo preguntas/respuestas o escribir un correo rápido.
- **[00:17:20]** **Definición operativa de «fluidez»:** saber *cuándo* usar un modelo de lenguaje y *en qué forma*, porque el agente no es bueno para todo. A veces basta una consulta normal al LLM; a veces no hace falta IA y hay que usar automatización.
- **[00:18:21]** Modo de operación del chat: *«zadawanie pytań i odpowiadanie jednokierunkowe»* = **preguntas y respuestas unidireccionales**: pregunta → respuesta → pregunta → respuesta. Se le llevan temas simples.
- **[00:18:32]** Modo de operación de la automatización: pasos definidos, **la misma ruta cada vez** (en diapositiva: *«Ta sama ścieżka»*).
- **[00:19:04]** **Definición de «proceso complejo»:** tenemos un objetivo, hay que llegar a un estado determinado, hay que elegir herramientas concretas o conectar con herramientas externas, y luego hace falta evaluación crítica. **Los pasos se van ordenando sobre la marcha y no se pueden fijar al principio.** Eso es territorio de agente.
- **[00:23:57]** Etiqueta técnica que le ponen: es un **proceso no determinista** («proces niedeterministyczny»); los pasos se establecen durante la ejecución → el agente es la solución.

### 1.4 PASO 02 — Descripción/especificación de la tarea que delegas (00:20:09 – 00:24:10)

- **[00:22:07]** **Qué significa «pensar en sistemas»:** describir la tarea que delegas al modelo de lenguaje **de forma que quede mapeado todo lo que hay por el camino** (*«żeby zmapować wszystko po drodze»*).
- **[00:22:21]** Primer movimiento del mapeo: preguntarse **qué necesitamos** (en el ejemplo: información de webs, listas de precios, N competidores y sus datos) → **sobre qué datos vamos a trabajar**.
- **[00:22:43]** Segundo movimiento: **de dónde sacamos esos datos y qué herramientas necesitamos**.
- **[00:23:38]** Tercer movimiento: **¿este proceso necesita decisiones?** Ejemplo dado: si los datos son viejos habrá que actualizarlos; hay que iterar sobre ellos; hace falta pensamiento crítico al hacer research y sacar conclusiones.
- **[00:23:16]** El propio mapeo **te dice qué solución usar**: si aparecen muchas herramientas + proceso multietapa + conexión a fuentes internas + descarga de internet → agente. **El PASO 02 retroalimenta al PASO 01.** Este bucle es lo más aprovechable didácticamente de todo el tramo.
- **Diapositiva (frame 0027, `#slide=13`, 00:26:15)** — la plantilla completa de especificación, con numeración desordenada tal cual aparece en pantalla:

```
01 / WEJŚCIA          03 / NARZĘDZIA              02 / DECYZJE
Strony i cenniki  →   Claude + skill          →   Dane starsze
8 konkurentów         Notion · Airtable ·          niż 30 dni?
                      Firecrawl
                             ↑___ TAK → POBIERZ ŚWIEŻE ___|

04 / REZULTAT · LLM BRAIN                    NA TEJ PODSTAWIE
Baza danych / pamięć dla modelu          →   Analiza z wnioskami
tabela konkurentów, zmiany w czasie,
format karty
```

**Traducción:** `01 / ENTRADAS`: webs y listas de precios, 8 competidores. `03 / HERRAMIENTAS`: Claude + skill; Notion · Airtable · Firecrawl. `02 / DECISIONES`: ¿datos con más de 30 días? → SÍ → **descarga frescos** (bucle de retorno a Entradas). `04 / RESULTADO · LLM BRAIN`: base de datos / memoria para el modelo; tabla de competidores, cambios en el tiempo, formato de ficha. `SOBRE ESTA BASE`: análisis con conclusiones.

> **Esto es plantilla reutilizable de curso.** Cuatro casillas + una regla de frescura + un bucle. Es lo único con forma de «formato de entregable» en todo el tramo.

### 1.5 Memoria y contexto (00:24:19 – 00:27:28)

- **[00:24:19]** **«En la práctica, cuando trabajas de verdad con modelos de lenguaje, no existe tal cosa como trabajar con modelos sin memoria.»**
- **[00:24:27]** **Justificación empírica de por qué:** en ChatGPT en el navegador, llega un punto en que la ventana de chat es tan larga que **el contexto se pierde** y el modelo **empieza a responder peor** con el tiempo.
- **[00:24:39]** Conclusión de diseño: para construir un sistema de trabajo realmente útil hay que **diseñarle la memoria** al modelo.
- **[00:24:50]** Hay **varias maneras** de hacerlo (lo dice explícitamente dirigiéndose a los técnicos). Enseñan **una**: la que llaman **LLM Brain**.
- **[00:25:03]** **Definición de LLM Brain:** una base de datos — **para los técnicos: una base de datos en grafo** — que **cumple el papel de memoria para el modelo**.
- **[00:25:24]** Argumento del volumen: 60 agencias no caben en una ventana de chat; se convierte en un caos y **se acaba la ventana de contexto**.
- **[00:25:36]** Función esperada de esa base: crear **un cerebro dinámico que se mejora a sí mismo** y **ve conexiones** entre datos dispares.
- **[00:26:00]** La base de conocimiento **es parte del traspaso de contexto** (no un almacén aparte): es el fundamento sobre el que el agente saca conclusiones.
- **[00:26:22]** Promesa de valor: análisis apoyado en una cantidad enorme de datos y conexiones «que nosotros haríamos en días u horas, o que directamente sería imposible de percibir».

### 1.6 PASO 03 — Contexto y conocimiento de la empresa (00:27:33 – 00:29:29)

- **[00:27:42]** Lo que «busca el mercado»: gente capaz de **extraer el conocimiento de las herramientas internas, reunir los datos de la empresa y componer un “sistema de verdad” (system prawdy) adaptado al trabajo con un modelo de lenguaje**.
- **[00:28:00]** **Pipeline de construcción, en 4 tiempos:**
  1. **[00:28:00]** Descargar información de internet (webs de las agencias) — vía **Claude Code + Firecrawl**.
  2. **[00:28:16]** Descargar información interna de CRM / Airtable — vía **conectores de Claude Code** con esas herramientas.
  3. **[00:28:28]** Eso constituye **«nuestras fuentes de verdad»** (*źródła prawdy*).
  4. **[00:28:31]** Elegir la herramienta contenedora — aquí **Obsidian**, que permite crear una base de datos en grafo.
- **[00:28:41]** **Por qué grafo:** los grafos van muy bien con modelos de lenguaje porque **permiten que el propio modelo cree la base de datos y vea por sí mismo las conexiones entre fuentes distintas**. «Y esa es la clave».
- **[00:29:07]** **Qué es el skill, funcionalmente:** una vez metidas las fuentes en Obsidian, «escribimos el modo en que Claude Code debe ordenar esos datos para nosotros» y **de eso hacemos un skill, una habilidad**: se le describe **de qué van los datos, nuestro modo de trabajar, qué información debe extraer y cómo debe ordenarla** para que construya la base por sí mismo.

### 1.7 Demo del grafo (00:29:30 – 00:34:59)

- **[00:30:05]** Efecto visual buscado: «efectivamente parece un cerebro». Se ven **clústeres** y **centros** que significan algo.
- **[00:30:20]** **Lo que se le entrega al modelo son «archivos desnudos» (gołe pliki)** — no una estructura previa.
- **[00:31:00]** **Lo que hace Claude Code:** extrae segmentos por sí mismo y agrupa las empresas; crea la base de datos con los clústeres.
- **[00:31:50]** **«El modelo de lenguaje se crea él solo esos clústeres y los agrupa él solo; no es algo que tengamos que hacer nosotros.»**
- **[00:32:05]** Además de clústeres, extrae **conceptos** (*koncepty*) por sí mismo: patrones transversales.
- **[00:32:10]** Detalle honesto: los conceptos le salieron en inglés «por la forma en que trabajé»; podrían estar en polaco. → **el idioma del artefacto depende del idioma de instrucción**.
- **[00:33:18]** **La distinción más importante del tramo:** el grafo **no es para el humano**. Está adaptado al agente, para que pueda recorrer la información, encontrar rápido las conexiones y sacar conclusiones. *«To, co widzicie tutaj, jest dla agenta»*.
- **[00:34:02]** Descripción del objeto: es «un sistema de notas muy complejo». Se puede entrar en una agencia concreta y ver etiquetas, información, su posicionamiento, qué dicen de sí mismos.
- **[00:34:29]** Generalización: el mismo esquema serviría para estudiar (tema → nota sobre bases de datos en grafo → todo dentro del sistema), con conceptos y análisis concretos.

**Estructura real del vault (frame 0032, verificada visualmente — NO se explica en voz, pero es el mapa completo del sistema):**

```
artefakty/            ← salidas para humanos (aquí vive prezentacja5.html)
raw/                  ← material bruto, inmutable
  agencies/
  assets/
wiki/                 ← conocimiento derivado por el agente
  analyses/           ← conclusiones (8 notas)
  concepts/           ← patrones transversales (20 notas)
  entities/
  segments/           ← los 4 clústeres
    duzi-marka
    duzi-performance
    msp-marka
    msp-performance
  sources/
  index               ← índice
  log                 ← registro
  overview            ← vista general
CLAUDE                ← CLAUDE.md, archivo de contexto del agente
```

> Separación `raw/` (crudo) ↔ `wiki/` (derivado) ↔ `artefakty/` (entregable), más `index` + `log` + `overview` como capa de navegación para el agente, más `CLAUDE.md` como contexto raíz. **Esto es arquitectura enseñable y está gratis en pantalla; nunca la verbalizan.**

### 1.8 El resultado y el cambio de rol (00:35:00 – 00:40:00)

- **[00:35:05]** Lo que ve el humano no es el grafo: son **las conclusiones que entrega el agente**. «Ese era su cerebro; esto es lo que él me entrega».
- **[00:35:35]** **Tesis del cambio de trabajo:** cuando empiezas a trabajar con un agente y a pasarle contexto y tu conocimiento, **tu trabajo pasa de ejecutor a supervisor** (*«z tej wykonawczej pracy na bardziej nadzorującą»*).
- **[00:36:14]** **Definición del nuevo deber:** «mi obligación ahora es comprobarlo, supervisarlo, ver qué me ha traído **e iterarlo**: ¿vamos en la buena dirección o sigue trabajando en ello?». El pensamiento crítico es la aportación humana.
- **[00:36:37]** Estructura del entregable: **6 clústeres, 4 sobre empresas y 2 sobre conclusiones y análisis**.
- **[00:36:50]** Clúster 1 — *Leads para pequeñas empresas* (25 agencias): hablan directamente al dueño de la pequeña empresa; producen llamadas, consultas, pedidos; **precios públicos y garantías**.
- **[00:37:35]** Clúster 2 — *Resultados para grandes marcas*: procesos descritos, **herramientas propias**, se facturan por **ROAS**, y les importa mucho el **coste de adquisición de cliente**.
- **[00:37:56]** Clúster 3 — *Marca de pequeñas empresas*: pymes que quieren parecer y sonar como una marca mayor; reciben **estética y portfolio** (p. ej. gestión de contenido).
- **[00:38:15]** Clúster 4 — *Campañas de grandes marcas* (12 agencias): viene el director de marketing y compra creatividad e imagen; **a menudo no publican precios**, pero exhiben una lista de clientes grandes y conocidos.
- **[00:38:52]** **Conceptos** que el agente devolvió por su cuenta: **arquetipos** (cómo operan), **mecanismos** (cómo entregan valor), si el precio es público, si dan garantía, **métodos nombrados**, cómo hacen educación, y su forma de captar clientes.
- **[00:39:24]** **Análisis**: conclusiones derivadas de las conexiones. Producen respuestas listas, notas, comparativas, **a veces matrices de servicios, precios y condiciones**, y sobre eso un **mapa de posicionamiento** y la detección de **huecos y oportunidades de mercado**.
- **[00:40:01]** **Generalización del patrón (clave para el diseño de curso):** si usaras el sistema para otra cosa que no fuera análisis de competencia, tendrías igualmente: **datos agrupados en clústeres + conceptos extraídos + análisis**. Es decir: *segmentos / conceptos / análisis* es la **forma canónica del output**, independiente del dominio.
- **[00:40:30]** **Mantenimiento:** el sistema se puede configurar para que al añadir un análisis nuevo, un concepto nuevo o una empresa nueva, **Claude recorra toda la base, compruebe si se conecta con el resto y actualice él solo todas las conexiones**.

---

## 2. Distinciones conceptuales, con la definición exacta que dan

### 2.1 Modelo vs Automatización vs Agente (PASO 01)

| | Cuándo | Definición literal dada | Herramienta que asignan |
|---|---|---|---|
| **Automatización** | La tarea **tiene** pasos definidos y repetibles | *«Ta sama ścieżka za każdym razem»* = «la misma ruta cada vez». «Un algoritmo simple, se puede escribir en pasos siempre idénticos», **cero pensamiento crítico** [00:15:40] | n8n, Make [00:18:41] |
| **Modelo (chat)** | La tarea **no** tiene pasos definidos, y es simple | *«Zadawanie pytań i odpowiadanie jednokierunkowe»* = «hacer preguntas y responder de forma unidireccional»: pregunta → respuesta → pregunta → respuesta [00:18:21]. «Preguntas y lluvia de ideas» [00:16:44] | ChatGPT, Claude (web) [00:16:24] |
| **Agente** | Proceso complejo | «Tenemos un objetivo, hay que llegar a un estado determinado, elegir herramientas concretas o conectar el proceso con herramientas externas, y después hace falta evaluación crítica. **Los pasos se van ordenando sobre la marcha y no somos capaces de fijarlos al principio**» [00:19:04–00:19:30] | Claude Code, OpenAI Codex [00:16:52 / 00:19:30] |

**Regla de decisión, tal como se dibuja en la diapositiva (frame 0024, `#slide=8`):**
`ZADANIE → ¿Ma określone, powtarzalne kroki? → TAK → B / AUTOMATYZACJA (Ta sama ścieżka)`; la rama NIE lleva a modelo → (A) chat / (B) agente.

**Matiz explícito del ponente [00:16:04 y 00:16:13]:** *«mówię tutaj możliwe, bo oczywiście ten schemat jest pomocniczy… czasami to nie jest takie zero-jedynkowe»* = «digo *posible* porque este esquema es auxiliar… a veces no es tan binario». **El árbol es heurístico, no normativo.**

### 2.2 Fuentes de verdad vs Memoria vs Skill (PASO 03) — la tríada central

**Diapositiva `#slide=15` (frame 0034, visible en 00:35:02), verbatim y traducida:**

| Concepto (PL) | Definición literal (PL) | Traducción | Artefacto que le asignan |
|---|---|---|---|
| **Źródła prawdy** | *Fakty z jednego adresu.* | **Fuentes de verdad: hechos desde una única dirección.** (una sola ubicación canónica por hecho) | `tabela konkurentów` — tabla de competidores |
| **Pamięć** | *Ustalenia, które zostają.* | **Memoria: los acuerdos/hallazgos que permanecen.** | **Obsidian** · `graf notatek` — grafo de notas |
| **Skill** | *Sposób pracy: kroki i format.* | **Skill: el modo de trabajar: pasos y formato.** | `analiza konkurencji` — análisis de competencia |

> Las tres definiciones caben en una línea cada una y son excelentes como andamiaje de curso. **Ojo: se muestran en pantalla y no se leen en voz alta.** El audio pasa por encima de la diapositiva más importante del tramo. Quien solo escuche el webinar, no se lleva la tríada.
>
> **Confirmación de embudo:** la web (`index.txt`, líneas 284-286) vende exactamente esto como *«Tydzień 03 — Kontekst, pamięć i własne skille»* («Semana 03 — Contexto, memoria y skills propios»). La diapositiva 15/22 del webinar **es el índice de la semana 3 del curso de pago**.

### 2.3 Otras distinciones operativas

- **[00:33:18] Para el agente vs para el humano.** El grafo/vault está diseñado para el agente («jest dla agenta»); el humano consume otra cosa (el dashboard de conclusiones). **Dos interfaces sobre el mismo sistema.** Es la distinción de arquitectura más útil del tramo entero.
- **[00:30:20] `gołe pliki` (archivos desnudos) vs estructura.** El humano aporta archivos crudos; la estructura (segmentos, conceptos) la produce el agente.
- **[00:23:57] Determinista vs no determinista.** Determinista → automatización. No determinista (pasos fijados durante la ejecución) → agente. Reetiquetado técnico del árbol del PASO 01.
- **[00:35:45] Trabajo ejecutor vs trabajo supervisor.** El sistema no elimina al humano: le cambia la función a verificar, supervisar e iterar.
- **[00:40:01] Segmentos / Conceptos / Análisis.** Tres capas de salida del sistema, invariantes respecto al dominio: agrupaciones de entidades, patrones transversales, conclusiones.
- **[00:12:58] AI Product Builder ≈ AI Operator ≈ Solution Engineer.** Lo declaran explícitamente intercambiable: *«nie chcę, żebyście się przywiązywali do nazwy»* = «no quiero que os apeguéis al nombre».

---

## 3. Herramientas nombradas y papel exacto asignado

| Herramienta | Marca de tiempo | Papel exacto que le dan |
|---|---|---|
| **Claude Code** (ASR: «kod kod», «klockod», «krotkot», «KlotKot», «Cloud Code»; en diapositiva: `Claude + skill`) | 00:16:52, 00:19:30, 00:23:32, 00:28:12, 00:31:03, 00:35:39 | **El agente.** Ejecuta el proceso multietapa, se conecta a las herramientas, crea y mantiene el grafo, extrae segmentos y conceptos, produce el análisis y **actualiza las conexiones al añadir datos nuevos**. Es el motor del sistema. |
| **OpenAI Codex** (ASR: «kodeks») | 00:16:52, 00:19:30, 00:33:36 | **Alternativa intercambiable a Claude Code.** *«nieważne, co sobie wybierzecie do pracy»* = «da igual lo que elijáis». Se nombra siempre en pareja con Claude Code, nunca se demuestra. |
| **Obsidian** | 00:28:31, 00:29:30, 00:40:57 | **El contenedor de la memoria.** Elegida porque «permite crear una base de datos en grafo». Es donde vive el LLM Brain. Única herramienta realmente mostrada en pantalla. |
| **Firecrawl** | 00:23:03, 00:28:12 | **Ingesta desde internet.** Descargar webs y listas de precios de los competidores. Se cita como conexión de Claude Code. |
| **Airtable** | 00:22:57, 00:28:16 | **CRM / fuente interna estructurada.** Se accede vía «conectores» de Claude Code. |
| **Notion** | 00:22:48, diapositiva 00:26:15 | **Base interna de conocimiento previo** («ahí hay información de agencias que ya habíamos investigado»). ⚠️ Aparece en la diapositiva de herramientas pero **nunca se usa en la demo**. |
| **n8n** (ASR: «AnyTen») | 00:18:41, 00:18:59 | **Automatización determinista.** «Las herramientas de automatización más populares». Explícitamente **fuera** del territorio del agente. |
| **Make** | 00:18:41, 00:18:59 | Igual que n8n. |
| **ChatGPT** | 00:16:24, 00:24:27 | **Ejemplo de uso de nivel 1** (chat como buscador) y **caso de estudio del problema**: la ventana larga pierde contexto y responde peor. Se usa como el «antes» de la narrativa. |
| **Claude (web/chat)** | 00:16:24, 00:17:43 | Nivel 1 de uso: «a veces basta con resolver el problema con una consulta normal al LLM». |
| **Gemini** | 00:01:51 | Mención de pasada, agrupado en «chat como buscador». |
| **Excel** | 00:15:32 | Destino del ejemplo de automatización (facturas). |
| **Google** | 00:01:51 | Referencia comparativa («mejor buscador que Google»). |

**Artefactos de software propios visibles en pantalla (no mencionados en voz, pero verificables):**
- `C:/Users/Lenovo/Desktop/Instagram/prezentacja-system-ai-v21.html` — la presentación es **una web local hecha a mano, versión 21**, de **22 diapositivas**. Es en sí mismo un ejemplo de «vibe coding» del que no hablan.
- `C:/Users/Lenovo/Desktop/Self-firma/artefakty/prezentacja5.html` — **el dashboard de resultados «RENTGEN RYNKU AGENCJI» es un HTML generado**, guardado dentro de `artefakty/` del propio vault. El «entregable para humanos» del sistema es una página web autocontenida.
- **StreamYard** — plataforma de emisión (pestaña visible).

---

## 4. Ejemplos concretos, con su detalle

### 4.1 Ejemplo de automatización pura (contraejemplo de IA) — [00:15:32]
Factura → escanear los datos de la factura → pasarlos a un Excel → calcular algo. **Y cada vez es igual.** Sin pensamiento crítico. → **No necesitas IA; lo resuelve una automatización.**

### 4.2 Ejemplo maestro: análisis de competencia — [00:20:09 en adelante]
- **Encargo (según diapositiva):** «Reúnes una lista de empresas de marketing y SEO en el mercado polaco, compruebas cómo queda tu agencia frente a ellas, ordenas los datos y sacas conclusiones».
- **Corpus real:** **60 agencias de marketing de Polonia**, datos reales, **con los nombres anonimizados** («para no hacerle publicidad a nadie»; se ven nombres deformados, pero los datos son verdaderos) [00:20:32, 00:30:39].
- **Entradas:** webs, listas de precios, datos de los competidores.
- **Herramientas:** Claude Code + skill; Notion, Airtable, Firecrawl.
- **Regla de decisión:** ¿datos con más de 30 días? → sí → descargar frescos.
- **Salida:** el vault Obsidian (para el agente) + el dashboard `prezentacja5.html` (para el humano).
- **Resultado medido en pantalla (frame 0035):** 4 clústeres de empresas — *Leady dla małych firm* 25 agencias · *Wyniki dla dużych marek* 13 agencias · *Marka małych firm* 9 agencias · *Kampanie dużych marek* 12 agencias — más *Koncepty* 20 notas y *Analizy* 8 notas. El dashboard se titula **«Rentgen rynku agencji»** = «Radiografía del mercado de agencias», con subtítulo en pantalla: **«To jest baza wiedzy, z której wyszła cała analiza»** = «Esta es la base de conocimiento de la que salió todo el análisis».

### 4.3 Cuatro traslados del mismo esquema a otros dominios — [00:20:58 – 00:21:58]
1. **Aprender un tema nuevo**: todo lo que aprendes sobre IA, en un solo sitio, con el mismo método.
2. **Base de conocimiento de departamentos**: documentos, procedimientos, acuerdos — ventas, RR. HH., finanzas o cualquier otro.
3. **Asesor privado**: metes tus notas, tus reflexiones, tus documentos, y obtienes un asesor que recuerda, sugiere y con el que contrastas ideas.
4. **(Implícito, [00:34:29])** Sistema de estudio: tema → nota sobre bases de datos en grafo → todo contenido en el sistema.

### 4.4 Ejemplos concretos de conceptos que el agente extrajo solo — [00:32:18 – 00:32:41]
Metodologías que usan las agencias; qué CTA/SEO tienen en sus landing pages *(el ASR dice «CEO», casi con seguridad «CTA»)*; cómo cualifican a los posibles clientes; si tienen branding basado en el fundador; qué hacen en educación.

### 4.5 La «persona de caja» — [00:27:01]
*«Jest tak naprawdę w stanie złożyć nawet osoba pracująca na kasie»* — «esto lo puede montar incluso una persona que trabaja en la caja de un supermercado»; lo aclara: usa esa profesión solo por nombrar un oficio totalmente ajeno al nicho de negocio. **Es un claim de accesibilidad, no un ejemplo. No hay caso real detrás.**

---

## 5. Cifras, fechas y datos verificables

| Dato | Marca | Comentario |
|---|---|---|
| **90 minutos** prometidos | 00:00:38 | El vídeo dura **1:56:59**. Sobrepasan en ~27 min. |
| **7+ años** de experiencia (Ola) | 00:05:14 | Coincide con la web («AI Engineer z 7+ lat doświadczenia»). |
| **8 años** en el sector (Ola) | 00:13:55 | **Contradice** al minuto 5. Se usa la cifra mayor para justificar la autoridad («la barrera antes era altísima»). |
| **20–30 mil** participantes en formaciones gratuitas | 00:07:06 | Textual: *«grubo ponad 20-30 tysięcy»*. Rango vago, no auditable. |
| **~5 mil** participantes en formaciones de pago | 00:07:20 | Marca: **wKontenerach**. |
| **8 meses de 2026** observando el mercado | 00:10:31 | Sitúa el webinar en **agosto de 2026**. |
| **20.08.2026**, 20:09–20:34 | Barra de tareas en frames 0019–0035 | **Fecha y hora exactas de la emisión.** El tramo 00:09–00:35 del vídeo corresponde a 20:09–20:34 reales. |
| **60 agencias** de marketing polacas | 00:20:32 y 00:30:39 | El corpus. |
| **8 competidores** | Diapositiva 00:26:15 | ⚠️ **Contradice el «60» hablado.** La diapositiva es plantilla genérica sin actualizar. |
| **25 / 13 / 9 / 12** agencias por clúster | Frame 0035 (00:35:03) | Suma **59**, no 60. Discrepancia menor pero real. |
| **20 notas** de conceptos · **8 notas** de análisis | Frame 0035 | Volumen del conocimiento derivado. |
| **6 clústeres** (4 de empresas + 2 de conclusiones) | 00:36:43 | Estructura del entregable. |
| **30 días** — umbral de frescura de datos | Diapositiva 00:26:15 | Única regla numérica de diseño de todo el tramo. |
| **«2 meses»** de trabajo manual ahorrado | 00:35:55 | Estimación propia de Ola, sin desglose. |
| **5 pasos** del método | 00:09:42 | Solo se cubren 3 en 40 min. |
| **22 diapositivas**, versión **v21** | Frames 0027/0034 | El deck lleva 21 iteraciones. |
| **10 proyectos** (ejemplo de datos de empresa) | 00:11:34 y diapositiva 00:35:02 | Escala típica que sugieren. |
| **ROAS** y **coste de adquisición** | 00:37:44 | Métricas del clúster «resultados para grandes marcas». |
| **995 zł netos / 1223,85 zł brutos**, hasta 10 cuotas 0 %, preventa hasta el **2 de septiembre**, inicio **26 de octubre**, 5 semanas, garantía de **7 días**, IVA 23 % | Web `index.txt` | El precio no se menciona en este tramo del webinar; es el destino del embudo. |

---

## 6. Advertencias, matices y «cuidado con»

- **[00:15:17] «Puede que la solución no sea IA.»** La advertencia más valiosa y la que más contradice al resto del embudo: si los pasos son fijos, usa automatización, no un LLM.
- **[00:16:04 / 00:16:13] El árbol es auxiliar, no binario.** «Vuestro caso puede tener un montón de matices; a veces no es tan de cero o uno». Reconoce el límite de su propio marco.
- **[00:17:20] «No para todo es bueno el agente.»** A veces basta una consulta simple al LLM.
- **[00:24:27] La ventana de chat larga degrada la calidad.** El contexto se pierde y el modelo responde peor. → No es un fallo del usuario; es una propiedad del medio.
- **[00:25:26] Se agota la ventana de contexto.** Meter 60 fichas en un chat = «un caos enorme» y luego un problema.
- **[00:23:43] Los datos envejecen.** Hay que actualizarlos e iterar sobre ellos (formalizado en la regla de los 30 días).
- **[00:23:51] El research exige una dosis de pensamiento crítico** — no es delegable del todo.
- **[00:36:14] Es tu obligación comprobar y supervisar el resultado.** La salida del agente no es final: hay que verificarla e iterarla.
- **[00:32:10] El idioma de salida depende de cómo trabajaste**, no del modelo — los conceptos salieron en inglés por su forma de instruir.
- **[00:33:04] El grafo intimida y no importa:** «no sé cómo moverme por esto» es una reacción legítima porque **el artefacto no está hecho para ti**.
- **[00:30:41] Anonimización de datos de terceros** antes de mostrarlos públicamente. Buena práctica ejercida, no enseñada.
- **[00:12:36] Advertencia de altitud:** «lo que os voy a enseñar es una solución técnica, pero al final construimos algo que debe dar valor de negocio y resolver un problema real; por eso se evalúan los resultados — es la parte más importante del proceso».
- **[00:13:13] No os apeguéis al nombre del puesto.** El mercado cambia y cada empresa lo llama distinto.

---

## 7. Citas literales más potentes (PL → ES)

1. **[00:03:07]** *«Przewaga nie leży w jednym promptcie, tylko tak naprawdę praca z AI zaczyna się od dobrze ustawionego kontekstu, który jest zasilony wiedzą, narzędziami i odpowiednimi zasadami.»*
   → «La ventaja no está en un prompt: el trabajo con IA empieza de verdad con un contexto bien configurado, alimentado con conocimiento, herramientas y las reglas adecuadas.»

2. **[00:07:38]** *«Co AI musi wiedzieć o waszej firmie, o waszej pracy? Skąd wie, którym źródłom ufać i gdzie człowiek zachowuje kontrolę?»*
   → «¿Qué tiene que saber la IA sobre vuestra empresa, sobre vuestro trabajo? ¿De dónde sabe en qué fuentes confiar, y dónde conserva el humano el control?»

3. **[00:15:17]** *«Jeśli tak, to bardzo możliwe, że rozwiązaniem tego problemu w ogóle nie będzie AI, tylko automatyzacja.»*
   → «Si es así, es muy posible que la solución a ese problema no sea IA en absoluto, sino automatización.»

4. **[00:16:46]** *«I większość osób się na tym poziomie zatrzymuje.»*
   → «Y la mayoría de la gente se queda en ese nivel.»

5. **[00:17:20]** *«Ta płynność w narzędziach AI… to jest ta umiejętność, że Ty jako użytkownik wspierany przez AI wiesz, kiedy użyć modelu językowego, w jakiej formie, bo też nie do wszystkiego agent jest dobry.»*
   → «Esa fluidez en herramientas de IA es la capacidad de que tú, como usuario asistido por IA, sepas cuándo usar un modelo de lenguaje y en qué forma, porque el agente tampoco es bueno para todo.»

6. **[00:19:24]** *«Kroki w zasadzie układają się w trakcie i nie jesteśmy ich w stanie ułożyć na samym początku.»*
   → «Los pasos se van ordenando sobre la marcha y no somos capaces de fijarlos al principio.» *(la definición operativa de cuándo hace falta un agente)*

7. **[00:24:19]** *«Nie ma czegoś takiego praktycznie, jak się faktycznie pracuje z modelami językowymi, jak praca z modelami bez pamięci.»*
   → «En la práctica, cuando trabajas de verdad con modelos de lenguaje, no existe eso de trabajar con modelos sin memoria.»

8. **[00:24:30]** *«To wasze okienko czatu już jest takie długie, kontekst się gubi i on zaczyna odpowiadać po jakimś czasie gorzej.»*
   → «Esa ventana de chat vuestra ya es tan larga que el contexto se pierde y, pasado un rato, empieza a responder peor.»

9. **[00:28:41]** *«Pozwalają na to, żeby model językowy sam stworzył bazę danych, w którym sam zobaczy połączenia pomiędzy różnymi źródłami i to jest właśnie ten klucz.»*
   → «Permiten que el propio modelo de lenguaje cree la base de datos en la que él mismo verá las conexiones entre distintas fuentes; y esa es precisamente la clave.»

10. **[00:31:50]** *«Model językowy sam sobie tworzy te klastry i sam to grupuje, to nie jest coś, co my musimy zrobić.»*
    → «El modelo de lenguaje se crea esos clústeres él solo y los agrupa él solo; no es algo que tengamos que hacer nosotros.»

11. **[00:33:21]** *«To wygląda w ten sposób, ale to nie jest dla nas… ona jest dostosowana do naszego agenta. To, co widzicie tutaj, jest dla agenta.»*
    → «Tiene esta pinta, pero no es para nosotros… está adaptada a nuestro agente. Lo que veis aquí es para el agente.»

12. **[00:35:45]** *«Nasza praca się zmienia z tej wykonawczej pracy na bardziej nadzorującą.»*
    → «Nuestro trabajo cambia de un trabajo ejecutor a uno más de supervisión.»

13. **[00:36:20]** *«Moim obowiązkiem jest teraz to sprawdzić, nadzorować, zobaczyć, co on mi tutaj przyniósł i poiterować go, czy idziemy w dobrym kierunku.»*
    → «Mi obligación ahora es comprobarlo, supervisarlo, ver qué me ha traído aquí e iterarlo: si vamos en la buena dirección.»

14. **[00:27:01]** *«Jest tak naprawdę w stanie złożyć nawet osoba pracująca na kasie.»*
    → «Esto lo puede montar de verdad hasta una persona que trabaja en la caja.» *(claim de accesibilidad — ver §8)*

15. **Diapositiva 00:35:02** — *«Źródła prawdy: Fakty z jednego adresu. · Pamięć: Ustalenia, które zostają. · Skill: Sposób pracy: kroki i format.»*
    → «Fuentes de verdad: hechos desde una única dirección. · Memoria: los acuerdos que permanecen. · Skill: el modo de trabajar: pasos y formato.»

16. **Diapositiva 00:02:57** — *«NIE BĘDZIE: 50 promptów, 20 aplikacji, jednego magicznego triku. BĘDZIE: System AI, który zna Twoją firmę.»*
    → «NO HABRÁ: 50 prompts, 20 aplicaciones, un truco mágico. HABRÁ: un sistema de IA que conoce tu empresa.»

17. **Diapositiva 00:26:45** — *«Wygląda na skomplikowane, a złoży go też osoba pracująca na kasie, z zawodem zupełnie spoza biznesu. Programowanie nie jest tu potrzebne.»*
    → «Parece complicado, pero también lo montará una persona que trabaja en caja, con un oficio totalmente ajeno al negocio. Aquí no hace falta programar.»

---

## 8. Dónde es VENTA disfrazada de docencia y dónde es DOCENCIA real

### 8.1 Docencia real (transferible sin comprar nada)

| Bloque | Por qué cuenta como docencia |
|---|---|
| **Árbol de decisión modelo/automatización/agente** [00:14:32–00:19:50] | Marco reutilizable, con criterio operativo («pasos idénticos, cero pensamiento crítico»), con **contraejemplo** (facturas → Excel), y con **autolímite declarado** («es auxiliar, no es binario»). Además va **contra su propio interés comercial**: le dice al público que a veces no necesita IA. |
| **Plantilla de especificación de tarea** [00:22:21–00:24:10 + diapositiva 00:26:15] | Cuatro casillas (entradas / herramientas / decisiones / resultado) + regla de frescura de 30 días + bucle de refresco. Es un formato copiable tal cual. |
| **Diagnóstico del colapso de la ventana de chat** [00:24:19–00:25:36] | Afirmación falsable, verificable por el propio alumno, que motiva la necesidad de memoria externa sin recurrir a autoridad. |
| **Tríada Źródła prawdy / Pamięć / Skill** [diapositiva 00:35:02] | Tres definiciones de una línea, precisas y accionables. |
| **«El grafo es para el agente, no para ti»** [00:33:18–00:34:00] | Reencuadre arquitectónico genuino: dos interfaces sobre un mismo sistema. Desactiva la ansiedad del alumno y a la vez enseña un principio de diseño. |
| **Ejecutor → supervisor, con la obligación de verificar e iterar** [00:35:35–00:36:31] | Define el trabajo humano residual. Honesto: no promete autonomía total. |
| **Forma canónica de salida: segmentos / conceptos / análisis** [00:40:01] | Generalización explícita y comprobable contra la demo. |
| **Las 3 preguntas de gobernanza** [00:07:38] | Contenido de altísimo valor… en 10 segundos. |
| **Estructura del vault visible en pantalla** [frame 0032] | `raw/` vs `wiki/` vs `artefakty/` + index/log/overview + CLAUDE.md. Docencia involuntaria: se ve, no se explica. |

### 8.2 Venta disfrazada de docencia

| Movimiento | Marca | Cómo funciona |
|---|---|---|
| **El anti-hype como hype** | 00:02:45–00:03:07 | «No os vamos a dar 50 prompts mágicos ni tres secretos mágicos… habrá concreto». Se posiciona por encima de la competencia sin aportar contenido; es una promesa de calidad, no una enseñanza. |
| **Acuñar el puesto que luego venden** | 00:03:55 | *«nową kompetencję… którą nazwaliśmy AI Operatorem»* = «una nueva competencia **que nosotros hemos llamado** AI Operator». Se inventa la categoría, y el producto de pago certifica esa categoría (la web ofrece «certyfikat AI Operators»). Circularidad perfecta. |
| **«Esto es lo que busca el mercado»** | 00:10:22–00:13:35 | Repetido como estribillo y presente como marca de agua en cada diapositiva (`TEGO SZUKA RYNEK`). La única evidencia ofrecida es *«miałam masę konsultacji»* («tuve un montón de consultorías») y «8 meses observando». **Cero ofertas de empleo, cero fuentes, cero datos.** Es la premisa que justifica la compra y es la menos sostenida del webinar. |
| **Prueba social difusa** | 00:07:06 | «Grubo ponad 20-30 tysięcy» — un rango, no una cifra; «jakieś 5 tysięcy» en las de pago. Además la propia web admite: *«AI Operators startuje po raz pierwszy. Te opinie pochodzą z wcześniejszych programów»* («AI Operators arranca por primera vez; estas opiniones vienen de programas anteriores»). |
| **El regalo fuera de tema** | 00:07:48–00:08:40 | El bonus es «cómo construir una web con IA en 4 tardes» + «cómo encontrar el primer cliente y vender la web». **No tiene ninguna relación con el sistema de conocimiento del webinar.** Es un mecanismo de retención en directo y un gancho de side hustle («bez naciągania i bez hype'u», dice, mientras lo hace). |
| **«Sin programar»** | 00:13:38, 00:14:03, 00:26:45 | «Todo esto se puede hacer solo con lenguaje natural». En pantalla, mientras tanto: un vault Obsidian con jerarquía de carpetas, un `CLAUDE.md`, Firecrawl, conectores a Airtable, un agente de terminal y un HTML generado. **Es cierto que no se escribe código; es falso que no haya complejidad técnica.** La propia web contradice el claim: la ruta técnica exige *«podstawy Bash i Gita oraz rozumieć HTTP i API»* y 8–16 GB de RAM. |
| **La «persona de caja»** | 00:27:01 | Máxima ampliación del mercado direccionable con un ejemplo hipotético. No hay ningún caso, ni testimonio, ni demostración. |
| **El salto justo donde está el valor** | 00:29:07 | *«napiszemy odpowiednio sposób, w jaki Claude Code ma uporządkować te dane… i wtedy tworzymy z tego skill»* — «escribimos adecuadamente cómo debe ordenar los datos… y de eso hacemos un skill». **El «adecuadamente» es el curso entero.** No se muestra ni una línea del skill, ni del CLAUDE.md, ni del prompt. Se enseña el *qué* y se retiene el *cómo*. |
| **El grafo como espectáculo** | 00:30:05–00:32:49 | «Parece un cerebro», «puede parecer magia negra». La densidad visual funciona como prueba de sofisticación. Nótese que ella misma admite que **el objeto no es legible para humanos** — es decir, el público está admirando algo que, por diseño, no puede evaluar. |
| **La diapositiva 15/22 = semana 3 del curso** | 00:35:02 | La tríada `Źródła prawdy / Pamięć / Skill` es literalmente el índice de *«Tydzień 03 — Kontekst, pamięć i własne skille»* del programa de pago. El webinar entrega el mapa; el curso vende el terreno. |
| **«2 meses de trabajo»** | 00:35:55 | Cifra de ahorro sin desglose, sin comparación y sin coste (no dicen cuánto tardó el agente, ni cuántas iteraciones, ni cuánto costó en tokens). |

### 8.3 La costura del embudo, en una frase
El webinar es honesto en el **diagnóstico** (qué problema tienes, por qué el chat no basta, cómo decidir la herramienta) y opaco en la **ejecución** (cómo se escribe el skill, cómo se estructura el contexto, cómo se valida el resultado). Enseña **arquitectura sin implementación**. Los pasos 04 y 05 anunciados —acceso a herramientas y evaluación de calidad, es decir, permisos y control de calidad— ni siquiera se abordan en estos 40 minutos, y son exactamente los que la web vende como el diferencial del programa («minimalne uprawnienia», «człowiek zatwierdza działania wymagające zapisu»).

---

## 9. Huecos: lo prometido y no entregado en este tramo (= temario del curso a diseñar)

1. **El contenido del skill.** Nunca se muestra. ¿Qué secciones tiene? ¿Condiciones de disparo? ¿Formato de salida? *(La web lo detalla: «skill z warunkami uruchomienia, wymaganym wejściem, granicami działania i stałym formatem wyniku» — condiciones de activación, entrada requerida, límites de actuación y formato fijo del resultado. Eso es lo que falta aquí.)*
2. **El `CLAUDE.md`.** Visible en el árbol de archivos, jamás abierto.
3. **Cómo se conecta Firecrawl** y cómo se configuran los conectores a Airtable/Notion.
4. **La jerarquía de fuentes de verdad ante conflictos.** Se enuncia «saber en qué fuentes confiar» [00:07:38] y no se resuelve.
5. **Dónde aprueba el humano.** Pregunta 3 de gobernanza: cero cobertura en 40 minutos.
6. **Cómo se valida un clúster.** ¿Y si el agente agrupa mal? No hay criterio de aceptación, ni control de alucinación, ni verificación de que las 25 agencias del clúster 1 estén bien clasificadas.
7. **Coste y tiempo reales** de construir el LLM Brain de 60 agencias.
8. **Qué hacer cuando el grafo crece.** Se menciona el auto-update [00:40:30] pero no el límite: ¿a partir de cuántas notas deja de funcionar recorrer «toda la base»?
9. **Anonimización / privacidad de datos.** Se practica [00:30:41] y no se enseña.
10. **Evaluación (paso 05).** Declarada «la parte más importante del proceso» [00:12:54] y ausente.

---

## 10. Notas de transcripción — errores sistemáticos del ASR (leer antes de citar)

El reconocimiento automático destruye los nombres propios. Equivalencias confirmadas por diapositivas y contexto:

| Lo que dice la transcripción | Lo que realmente es |
|---|---|
| «kod, kod», «klockod», «krotkot», «KlotKot», «Cloud Code», «Klot» | **Claude Code** / Claude |
| «kloda», «klodzie» | Claude (declinado en polaco) |
| «kodeks» | **OpenAI Codex** |
| «AnyTen» | **n8n** |
| «okienko czasu» [00:16:21] | *okienko czatu* = **ventana de chat** |
| «od marketingu i od CEO» [00:20:23] | *marketingu i SEO* — **confirmado por la diapositiva** |
| «jakiego CEO, jakie mają CEO na landing page'ach» [00:32:21] | casi con seguridad **CTA** (o SEO) — ambiguo, no citar literalmente |
| «nie wiecie jak się zaniknąć» [00:19:47] | prob. *jak się za to zabrać* = «cómo meterle mano» |
| «LLM Brain» / «LLM Second Brain» | Se usan indistintamente (Damian dice «Second Brain» 00:03:39; Ola dice «LLM Brain» 00:24:57) |

**Regla para el diseño del curso:** contrastar SIEMPRE la transcripción con `informe.md` (OCR) y con el frame correspondiente antes de dar por buena cualquier cifra o nombre. Las diapositivas y las capturas son la fuente fiable; la transcripción es la fuente narrativa.

---

## 11. Qué me llevo para diseñar el curso (síntesis operativa)

- **Hay exactamente cuatro artefactos enseñables en 40 minutos:** (1) el árbol de decisión herramienta, (2) la plantilla de 4 casillas de especificación de tarea, (3) la tríada fuentes de verdad / memoria / skill, (4) la estructura de vault `raw` / `wiki` / `artefakty`. Todo lo demás es motivación, demo o venta.
- **El mejor material está en la diapositiva, no en el audio.** Un curso derivado debe *verbalizar* lo que ellos solo enseñaron de pasada: las tres definiciones de la tríada y el layout del vault.
- **El movimiento pedagógico más potente que hacen es negativo:** «puede que no necesites IA». Un curso honesto debe abrir por ahí.
- **El movimiento más deshonesto es la elipsis del skill.** Cualquier curso que quiera superar a este debe empezar exactamente donde este se detiene: mostrando el archivo.
- **La forma canónica del output (segmentos / conceptos / análisis) es reutilizable** y es el mejor candidato a «entregable de alumno»: mismo esqueleto, dominio propio.
- **Falta toda la capa de control:** permisos, aprobación humana, validación de clústeres, evaluación. Es a la vez el hueco del webinar y el argumento de venta del programa — y por tanto el sitio donde un curso propio aporta más valor diferencial.
