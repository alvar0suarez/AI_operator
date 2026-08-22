# Fuente: transcripción webinar Damian Naprawa + Ola Zajączkowska — tramo 00:40:00 → 01:20:00

**Archivo base:** `/home/user/AI_operator/materiales/fuentes/webinar-damian-naprawa/transcripcion.md` (líneas 960–2512)
**Apoyo visual/OCR:** `/home/user/AI_operator/materiales/fuentes/webinar-damian-naprawa/informe.md` (líneas 800–2260; frames 0036–0100)
**Contraste comercial:** `/home/user/AI_operator/materiales/fuentes/web-aioperators/index.txt`
**Cobertura leída:** 00:39:56 → 01:24:39 (se leyó algo más allá del corte para no partir el argumento de precio y el arranque del Q&A).
**Idioma original:** polaco. Traducciones al español mías, literales salvo indicación.

Nota de estructura: este tramo tiene **cuatro bloques nítidos**:
1. **00:40–00:52** — cierre docente de la demo: mantenimiento de la base de datos, generalización a otros casos de uso, y el bloque de **evaluación** (el más denso técnicamente de todo el webinar).
2. **00:52–00:56** — recapitulación de los "5 elementos" + **matar el hype** ("detrás hay varias decenas de intentos").
3. **00:56–01:03** — traspaso a Damian: "el prompt ya no basta", "el problema no está en el modelo", **enunciación del hueco de mercado** + vídeo de venta.
4. **01:03–01:24** — **pitch completo**: programa AI Operators, dos itinerarios, semanas 1–5, garantía, umbral de 100 personas, precio, bono, primer Q&A.

La frontera docencia/venta cae con precisión en **[00:56:35]** ("y eso será todo por mi parte") — y de forma explícita y confesada en **[00:57:07]** ("todavía tengo unas palabras que añadir por mi parte").

---

## 1. Afirmaciones enseñables (con marca de tiempo)

### 1.1 Mantenimiento y crecimiento de la base de conocimiento

- **[00:40:07–00:40:18]** El mismo esquema sirve fuera del caso "análisis de competencia": siempre se obtienen (a) datos agrupados en **clústeres** por tema del que se recogen informaciones, (b) **conceptos** extraídos, y (c) **análisis**. Es decir: la arquitectura clúster→concepto→análisis se presenta como plantilla reutilizable.
- **[00:40:30–00:40:53]** *Afirmación central del bloque*: si se trabaja eficazmente con los modelos de lenguaje, el sistema puede configurarse de modo que **al añadir un análisis nuevo, un concepto nuevo o una empresa nueva, Claude recorre toda la base de datos**, comprueba si eso se conecta con el resto y **actualiza él solo todas las conexiones**.
- **[00:41:02–00:41:20]** Concreción visual en Obsidian: al añadir una empresa nueva, el agente **no la deja como un circulito suelto colgando**; recorre todos los ficheros, mira con qué enlaza y **crea aristas nuevas que aparecen en el grafo como flechas nuevas**.
- **[00:41:26–00:42:00]** *Matiz honesto dirigido a los técnicos del público*: el grafo es **solo una** de las formas de construir una base de datos para modelos de lenguaje. "Es muy eficaz. Hay también otras formas... no es que sea la única por la que haya que ir hoy". Se justifica como (a) universal, (b) útil en muchos casos, (c) **"algo bonito de mostrar"** — nótese la mezcla de criterio técnico con criterio de escaparate.

### 1.2 Por qué una base estructurada supera al "tirar ficheros al chat"

- **[00:42:25–00:42:45]** Diagnóstico del método ingenuo: si le sueltas a Claude 5 o 10 ficheros sin estructura, **"lo hará muy por encima, te devolverá algo genérico, no verá los detalles, tendrás que romper la tarea en etapas pequeñas... y así se trabaja iterativamente y sale con suerte variable"**.
- **[00:42:46–00:42:59]** Con base de datos: el contexto **ya viene descrito de antemano**, hay **formas de trabajo** declaradas, y además se le puede meter dentro de la propia base **la instrucción de cómo debe usar esa base**. (Idea clave: el manual de uso del conocimiento vive dentro del conocimiento.)
- **[00:42:59–00:43:06]** Generalización explícita: si se hiciera la base de un **proceso interno de empresa**, también se configura para que el agente opere de ese modo.
- **[00:43:20–00:43:33]** Valor prometido: conclusiones que **"permiten ver algo que normalmente no veríamos sin un análisis tan profundo"**, porque el sistema **conecta puntos** ("to są takie kropki" — "son como puntitos").
- **[00:43:33–00:43:53]** *Problema del usuario nombrado con precisión*: "muchísima gente se topa con esto: trabaja con modelos de lenguaje y piensa 'joder, pero él no sabe que ahora que escribo este informe necesito conclusiones de un informe de hace tres meses'". Respuesta: crear un análisis/dashboard que vea esas conexiones, **porque el grafo lo garantiza y se ocupa de ello**.

### 1.3 El resultado como artefacto de decisión

- **[00:44:02–00:44:45]** Del grafo sale un **panel/artefacto** por empresa: en qué se diferencia, en qué es **mejor que el mercado**, en qué es **peor**, y **qué hacer para diferenciarse** — todo ya redactado por el sistema.
- **[00:45:10–00:45:36]** El artefacto responde a: cómo se posiciona la empresa frente al mercado en su **oferta**, cuál es su posición según datos, información sobre sus **clientes** y sobre **qué hay en su web** y cómo se posicionan a sí mismos.
- **[00:45:37–00:45:57]** Argumento de autoridad de Ola: "de mi propia experiencia trabajando con datos, que tengo muchísimos años, en muy distintos sectores, sé que a veces ese proceso de extraer conclusiones es **muy penoso/laborioso** (mozolny), y los modelos de lenguaje nos lo facilitan".

### 1.4 El sistema mostrado es un prototipo, y prototipar es la competencia

- **[00:46:47–00:46:56]** **"El sistema que os he enseñado es en realidad un prototipo de sistema"**, o interno para una empresa, o para tu propio trabajo concreto.
- **[00:47:01–00:47:30]** Enumeración de la competencia demostrable (cinco verbos en primera persona, casi un guion de entrevista de trabajo): *sé qué solución elegir · sé diseñar tal sistema · sé descargar/obtener los datos · sé diseñar esos datos para el modelo de lenguaje · sé proponer una solución de la que sacar conclusiones valiosas para el negocio* (p. ej. fabricando el artefacto que ordena esas conclusiones).
- **[00:47:36–00:48:03]** **Regla de higiene de accesos**: "es muy importante controlar el acceso a las herramientas, y que Claude alcance solo allí donde realmente tenemos que sacar esa información". Receta explícita: elegir Claude → **conectarlo solo con las herramientas necesarias vía conectores** → **asignarle una carpeta concreta**.
- **[00:48:09–00:48:33]** *Núcleo doctrinal*: "**lo más importante somos nosotros**, lo más importante es nuestro conocimiento experto y nuestra actuación crítica: nosotros somos quien **comprueba** su resultado, **aprueba** su resultado, y en su caso **itera** sobre ese resultado y lo dirige en la buena dirección. **Y eso es la verdadera transmisión de contexto.**"
- **[00:48:34–00:49:00]** Metáfora que usan: "**antes se decía que los datos son como el petróleo; ahora se dice que el contexto es como el petróleo**" — el conocimiento experto traducido a un proceso de trabajo legible para el modelo, para que descargue al humano de una tarea concreta.

### 1.5 Los 5 elementos (recapitulación doctrinal completa) — [00:52:15–00:55:02]

El pantallazo (frame 0044, 00:52:12) fija los cinco bajo el rótulo **"TEGO SZUKA RYNEK"** ("esto es lo que busca el mercado"):

| # | Elemento (PL) | Traducción | Contenido según la voz |
|---|---|---|---|
| 1 | Płynność w narzędziach AI | Fluidez en herramientas de IA | Saber **cuándo el LLM sirve y cuándo no**, cuándo usar agente y **cuándo el agente es un "overkill"**: para un brainstorm simple no hace falta meter a Claude Code ni a Codex [00:52:26–00:52:48] |
| 2 | Myślenie systemami | Pensar en sistemas | Saber describir bien tu forma de trabajar = transmisión de contexto: mapear el conocimiento experto, **estructurarlo, aislar etapas, decir qué datos usas, cómo, en qué orden, cuánto necesitas, si hay que actualizarlo** [00:52:49–00:53:20] |
| 3 | Wewnętrzne narzędzia | Herramientas internas / acceso a datos | ¿Podemos acceder a esos datos?, ¿cómo ordenarlos?, ¿cuántos proyectos implicar? "Los modelos de lenguaje también trabajan sobre datos, **no pueden apoyarse solo en su propio conocimiento**" [00:53:21–00:53:38] |
| 4 | Zdolność prototypowania | Capacidad de prototipar | Dirigir bien a Claude Code para que **convierta tus ideas en un artefacto tangible, un prototipo que sea herramienta para extraer conclusiones** [00:53:39–00:53:59] |
| 5 | Wynik realnie rozwiązuje problem | Que el resultado resuelva de verdad el problema | Evaluar los resultados del sistema y ver si **resuelve realmente el problema** [00:54:34–00:55:02] |

- **[00:53:59–00:54:34]** *Definición del cambio de rol*: cuando tienes ese sistema "**dejamos de ejecutar la tarea** y podemos delegarla al agente; **nos convertimos en un especialista asistido por IA**, y lo que hacemos es la evaluación, el pensamiento crítico y una actuación más estratégica: hacia dónde ir, qué conclusiones sacar" — una vez entregadas al agente las tareas "repetitivas, aburridas o difíciles y tediosas" (*żmudne*).

### 1.6 Bloque de Damian: prompt, modelo y hueco de mercado

- **[00:57:18–00:57:41]** "Hoy **el prompteo ya no tiene sentido**... mejor dicho: **el prompt por sí solo no resuelve los problemas** de los que nos enseñaban hace un año, cuando nos decían que el prompt engineering era lo más importante. Hoy esa regla está un poco *passé*. **La ventaja está en construir un sistema.**" (Slide frame 0050: *"…nie jest lepszy prompt"* — "…no es un prompt mejor").
- **[00:57:50–00:58:19]** **"El problema no está en la elección del modelo de IA."** Mucha gente pregunta qué modelo usó; su respuesta habitual: "**no tiene mayor importancia qué modelo uses mientras no gastes de verdad cientos de miles o miles en tokens**".
- **[00:58:19–00:58:43]** El problema real: **"cada vez le explicas a la IA la empresa desde cero"** (slide frame 0051). Reconoce el motivo psicológico: "**la gente es perezosa, yo también soy perezoso** y no me apetece explicarlo todo cada vez; eso hace que tenga peores resultados si no tuviera un sistema donde el conocimiento esté recogido en un sitio y el contexto bien puesto".
- **[00:58:50–00:59:06]** Por qué falla el "una frase y ya": "si no lo describimos bien antes, **los resultados también son flojos, porque se sacan de la estadística**. Recuerdo que la IA es una tecnología basada un poco en la estadística. **Probabilidad, esa es mejor palabra.**"
- **[00:59:11]** Frase-bisagra de todo el webinar: **"I tu się właśnie pojawia luka, kto przygotuje firmę do realnej pracy z AI"** — "**Y aquí es donde aparece el hueco: ¿quién preparará a la empresa para el trabajo real con IA?**" (Slide frame 0052: "I TU POJAWIA SIĘ LUKA / Kto przygotuje firmę do realnej pracy z AI?").
- **[00:59:18–00:59:31]** "Ya sabemos que **no tienen por qué ser programadores**. Yo también sé programar, pero hoy ya no programo. Y hoy **mi mayor skill es que sé conectar los puntos y poner bien el contexto**."
- **[00:59:34–01:00:05]** Tesis provocadora fechada: "hoy los **humanistas** o las personas no técnicas a menudo tendrán **ventaja sobre los programadores**. Si hubiera dicho esto hace 5 o 3 años, todos se habrían reído de mí, me habrían linchado. **Hoy está pasando.** Los especialistas con conocimiento de dominio a menudo saben describir mejor un problema y metérselo a la IA que las personas técnicas."
- **[01:00:17–01:00:27]** Definición de la demanda: "hoy **necesitamos gente que sepa ordenar un conocimiento y convertirlo en procesos**. Y sobre todo **preparar el contexto para esa IA**."

---

## 2. Distinciones conceptuales, con definición exacta

1. **Contexto ≠ prompt.** El prompt es una instrucción puntual; el contexto es conocimiento experto traducido a proceso legible por el modelo, persistente y versionable. "La verdadera transmisión de contexto" se define en [00:48:21–00:48:33] como **el ciclo comprobar → aprobar → iterar → dirigir**, no como escribir un texto largo.
2. **Trabajo ejecutivo vs. trabajo supervisor.** El sistema convierte al humano de ejecutor en supervisor/evaluador [00:53:59–00:54:22]; el rol resultante se nombra **"specjalista wspierany przez AI"** (especialista asistido por IA).
3. **Proceso determinista vs. no determinista.** Aparece como criterio de selección de proceso en la semana 1 del curso [01:07:41]: "cuándo elegir proceso determinista, no determinista; cuándo encaja una solución basada en Claude Code; cuándo hay que hacer prototipo; cuándo automatización".
4. **Agente vs. overkill.** Distinción operativa [00:52:37–00:52:48]: un brainstorm simple no justifica un agente de código.
5. **LLM brain (grafo) vs. sistemas RAG.** [01:10:22–01:11:08] "Crear una base de conocimiento para el agente **no son solo grafos** y no solo esos bonitos LLM brains de colores; **también hay sistemas RAG**, y también sistemas RAG muy simples que se pueden hacer sin construirlos uno mismo". Y el matiz honesto: "**no es que un LLM brain sea la solución para todo**... no siempre servirá el LLM brain, a veces será otra solución".
6. **Prototipo interno vs. producto para vender.** [01:13:58–01:14:35] Distinción tajante: construir algo para necesidades internas y publicarlo en internet "**son dos mundos distintos y dos caminos distintos**".
7. **Base de datos con procedencia vs. montón de ficheros.** La base grafo permite ver **fuente** y **fecha de creación de la nota**, entrar y verificar qué se le metió y cómo se conectó [00:50:54–00:51:11]. Es la condición de posibilidad de la evaluación.
8. **Ruta no técnica vs. ruta técnica** (ver §10.3): la primera ordena procesos y contexto; la segunda construye la capa segura entre agente y API/logs/documentación interna.
9. **Datos como petróleo vs. contexto como petróleo** [00:48:34–00:48:43]: reformulación explícita del tópico, para desplazar el valor del dato bruto al conocimiento operativo.

---

## 3. Herramientas nombradas y su papel exacto

| Herramienta | Papel en este tramo | Marca |
|---|---|---|
| **Claude** (modelo/app) | Motor que recorre la base y actualiza conexiones; se le conecta **solo** con las herramientas necesarias vía **conectores** y se le asigna **una carpeta concreta** | 00:40:41, 00:47:54–00:48:03 |
| **Claude Code** (en la transcripción aparece deformado como "kodkod"/"plot-code"/"KlotKot") | Agente que convierte ideas en artefacto/prototipo; también el ejemplo de "overkill" si la tarea es trivial | 00:52:48, 00:53:44, 01:07:44 |
| **Codex** ("kodeks") | Citado solo como alternativa equivalente en el mismo argumento de overkill | 00:52:48 |
| **Obsidian** | Visor del grafo; escenario donde se demuestra que una empresa nueva no queda como nodo suelto | 00:40:57–00:41:20, OCR frame 0036 |
| **Grafo de notas / LLM brain** | Base de conocimiento con procedencia y fechas; una opción entre varias | 00:41:26, 00:50:54, 01:10:13 |
| **MCP (servidores y conectores)** | Vendido, no enseñado, en este tramo: semana 2 usar servidores MCP existentes; semana 5 (ruta técnica) construir uno propio como capa segura hacia API/logs/documentación internos | 01:08:41–01:09:02, 01:11:25–01:12:14 |
| **Skills** | Igual: semana 2 "aprender a crear skills desde cero"; semana 3 skills que apoyan el montaje de contexto | 01:08:41, 01:09:55 |
| **Sistemas RAG** | Mencionados como alternativa a enseñar en semana 4; no se explican aquí | 01:10:29 |
| **Artefacto HTML** (`prezentacja5.html`, servido desde `C:/Users/Lenovo/Desktop/Self-firma/artefakty/`) | El "Rentgen rynku agencji" (radiografía del mercado de agencias): dashboard de conclusiones | OCR frames 0037–0040 |
| **Bash, Git, API** | Requisitos previos "simples" declarados **solo** para la ruta técnica | 01:16:35 |
| **PayU raty** | Financiación en 10 plazos al 0% | 01:19:03 |

---

## 4. Ejemplos concretos

1. **Radiografía de una agencia de marketing anonimizada** ("Kadrio – Wrocław", grupo "Leady dla małych firm"), con datos reales y nombre inventado [00:44:02–00:44:10]. El artefacto muestra: en qué destaca (hace **AI SEO/GEO**), qué la hace **mejor que el mercado** (habla de precio, lista larga de clientes), en qué es **peor** (oferta más estrecha: vende 2 de 12 categorías de servicios), su posición frente al mercado y qué hacer para diferenciarse ("ve más a fondo", "añade una cuarta prueba", "ocupa un sector sin dueño").
2. **Tip de búsqueda de empleo / captación** [00:44:46–00:45:09]: usar el mismo análisis para llamar a la puerta de una empresa — "oye, he detectado estos huecos en vosotros, podéis mejorar esto" — y para prepararse una candidatura a un puesto concreto.
3. **Catálogo de usos alternativos del mismo sistema** [00:49:26–00:50:17, corroborado por el slide del frame 0042]: aprendizaje de un tema (materiales de YouTube, cursos, artículos), conocimiento de un departamento (procedimientos y acuerdos), asesor personal (tus notas), **RR. HH./reclutamiento** (candidatos en un formato único), **tarifas y ofertas** (cambios del mercado, para ventas), **atención al cliente** (preguntas repetitivas respondidas a partir de casos ya resueltos).
4. **El informe de hace tres meses** [00:43:38–00:43:47] como ejemplo canónico del fallo de memoria del LLM.
5. **Caso de prueba de degradación** [00:51:35–00:51:42]: "si le añadimos 15 ficheros más, ¿no empieza a perderse y a responder peor?".
6. **Asistente de voz que atiende el teléfono** [01:20:11–01:21:55]: bono; ejemplo de desvío del número de iPhone al asistente; sectores citados como compradores naturales: **restaurantes y salones de belleza**.
7. **Testimonio de Katarzyna Kot**, auditora de calidad de producción alimentaria [01:18:00–01:18:19 + frame 0095]: "el conocimiento antes reservado a los programadores lo habéis traducido a un lenguaje comprensible para alguien de fuera del sector IT".
8. **La propia web de AI Operators** como ejemplo de landing hecha con IA a partir de "un contexto muy bueno, desarrollado ya durante más de un año" [01:14:37–01:14:56].

---

## 5. Cifras y datos

**Del caso demostrado (voz + OCR del artefacto):**
- **59 empresas** en el universo analizado; el rasgo diferencial (AI SEO/GEO) lo hacen "solo **8 de 59**" según la voz [00:44:18–00:44:22]; el artefacto en pantalla muestra contadores del tipo "igual **5 de 59**" y "igual **7 de 59**" (frames 0038 y 0040) — **la cifra dicha y la cifra en pantalla no coinciden exactamente**.
- **25 empresas** en el grupo "Leady dla małych firm"; **43 empresas** en otra celda; **17 marcas** mostradas en la web (mediana de mercado 10); **mediana de mercado 5** en otro indicador; **2 de 12 categorías** de servicios vendidas; **"AI SEO/GEO – nivel 4 de 4: tecnología propia"** (frames 0038–0040).
- **Ahorro declarado** (justo antes del tramo, [00:35:55]): lo que Claude hizo "yo lo habría hecho en unos **2 meses**".

**Del pitch:**
- Programa de **5 semanas**; **dos itinerarios**; fundamento común en las **semanas 1–4**; el proyecto se elige **en la semana 5** (frame 0086).
- **7 días** de garantía desde el inicio; devolución del **100 %**; plazo hasta el **2 de noviembre** [01:18:33–01:18:43]; reembolso en **3 días hábiles** como colchón (transferencia = 1 día hábil) [01:23:50–01:24:02].
- **Mínimo 100 personas** en preventa o **se cancela el proyecto entero** y se devuelve todo el dinero [01:19:29–01:19:57].
- **Precio: 995 zł netto + 23 % IVA** [01:23:16–01:23:28]; la web añade **1223,85 zł brutto**. **10 plazos al 0 %** vía PayU [01:19:01–01:19:05].
- Inicio del programa: **octubre** [01:18:45–01:18:51] (la web precisa **26 de octubre**; preventa hasta el **2 de septiembre**, que es la fecha en pantalla del webinar, frame 0098).
- Bono por comprar **hoy hasta las 23:59 / medianoche**: curso online "construye un asistente de voz IA que contesta al teléfono", entregado **en septiembre** [01:20:01–01:20:13, frames 0100–0101].
- Precio de mercado de esos asistentes de voz: **500–1200 zł al mes** en suscripción, según volumen de llamadas [01:21:00–01:21:20, confirmado en el slide].
- Certeza declarada sobre Android: "**calculo que un 80 %** también se puede" [01:22:25].
- Inversión publicitaria del lanzamiento: "**literalmente unos céntimos** para nuestros estándares", deliberadamente, para que entren los clientes habituales [01:24:24–01:24:39].

---

## 6. Advertencias y matices (lo que sí acotan)

- **El grafo no es la única vía** ni obligatoria [00:41:26–00:41:47]; y parte de su atractivo es que **luce bien** [00:41:55].
- **El proceso es iterativo por naturaleza**: "no se trata de que montemos el sistema una vez y ya nos dé un buen resultado, sino de que **iteraremos sobre él**" [00:45:58–00:46:19].
- **El LLM no puede apoyarse solo en su conocimiento propio**; necesita datos [00:53:36].
- **El agente puede ser excesivo** para tareas triviales [00:52:37–00:52:48].
- **Hype**: "la IA es **solo una tecnología**" y una solución existe **para resolver un problema concreto** [00:54:45–00:55:02].
- **No siempre todo se resuelve con modelos de lenguaje** — dicho literalmente al describir la semana 1 [01:08:01–01:08:05].
- **El LLM brain no vale para todo** [01:10:51–01:11:08].
- **No enseñarán a construir y vender aplicaciones**: "no os echamos arena a los ojos diciendo que aprenderéis a construir aplicaciones y luego venderlas. **En absoluto.** Aunque sé que hay gente en internet que sí engaña así a la gente, **y no los respeto nada**" [01:13:58–01:14:19]. Considera ese terreno "**reservado hoy por hoy a ingenieros y programadores**".
- **Los servidores MCP no se construyen en la semana 2** por ser "un poco más complicados"; se dejan a la ruta técnica [01:08:56–01:09:04].
- **Requisitos previos declarados**: ninguno para la ruta no técnica ("basta con usar ChatGPT de forma esporádica", [01:04:03–01:04:21]); Bash, Git, API para la técnica [01:16:35].
- **Transparencia comercial parcial**: admite que la preventa se dirige a clientes fijos y que apenas han invertido en publicidad [01:24:21–01:24:39].

---

## 7. EVALUACIÓN DE RESULTADOS Y CASOS DE PRUEBA (bloque prioritario)

Es el "KROK 05" de la presentación, rotulado en pantalla **"TEGO SZUKA RYNEK / Ocena jakości wyniku / Wynik realnie rozwiązuje problem"** ("Esto busca el mercado / Evaluación de la calidad del resultado / Que el resultado resuelva realmente el problema"), frame 0043.

**7.1 Alcance universal de la evaluación — [00:50:27–00:50:42]**
"Esa evaluación de la calidad del resultado no se refiere solo al sistema que os he enseñado, ni solo a este caso concreto, sino en realidad **a todo aquello para lo que fuerais capaces de usar este sistema**."

**7.2 Es el punto crítico del oficio — [00:50:42–00:50:52]**
"**To jest taki krytyczny punkt pracy z modelami językowymi, że zawsze musimy oceniać, jak ten model językowy zwraca nam te odpowiedzi.**" → "Este es un punto crítico del trabajo con modelos de lenguaje: **siempre tenemos que evaluar cómo nos devuelve el modelo esas respuestas**."

**7.3 Precondición: trazabilidad — [00:50:52–00:51:11]**
La base de datos en grafo permite: ver **la fuente**, ver **cuándo se creó la nota**, poder **entrar y verificar siempre** qué información se le metió y **cómo quedó conectada**. Sin procedencia no hay evaluación posible.

**7.4 Definición operativa de "caso de prueba" (przypadek testowy) — [00:51:11–00:51:34]**
Un caso de prueba consta de dos piezas:
1. **Un fenómeno esperado**: "algún caso, por ejemplo **una conexión concreta, un concepto concreto que el sistema debería captar**".
2. **Una consulta fija**: "deberíamos tener **una pregunta concreta** con la que siempre podamos preguntar y ver si **sigue captando esas conexiones**".

**7.5 El caso de estrés canónico — [00:51:35–00:51:42]**
"czy jak na przykład dodamy mu 15 innych plików, czy on nie zacznie się gubić i nie zacznie nagle odpowiadać gorzej" → "**si, por ejemplo, le añadimos otros 15 ficheros, ¿no empieza a perderse y de golpe a responder peor?**" — es decir, **regresión por crecimiento del corpus**: el mismo test, ejecutado antes y después de ampliar la base.

**7.6 Qué mide la evaluación — [00:51:42–00:51:53]**
Tres preguntas explícitas, en este orden:
- ¿**se degrada** la base con el tiempo? (*czy ona nie degraduje z czasem*)
- ¿**mejora** realmente? (*czy ona faktycznie się ulepsza*)
- ¿**se conserva el contexto**? (*czy ten kontekst pozostaje zachowany*)

**7.7 Criterio final, no técnico — [00:54:34–00:55:02]**
Por encima de todo lo anterior: "tenemos que saber evaluar los resultados de un sistema así y **ver si resuelve realmente el problema**... porque hay muchísimo hype con la IA y pensamos que es capaz de resolverlo todo, **pero es solo una tecnología**, y al final, igual que cuando diseñamos cualquier solución, existe para resolver un problema dado; entonces, ¿lo resuelve de verdad, o quizá no nos aporta un valor concreto?"

**7.8 El humano como juez — [00:48:09–00:48:33]**
El bucle de evaluación es humano: **sprawdzać (comprobar) → zatwierdzać (aprobar) → iterować (iterar) → kierować (dirigir)**. La web lo formula igual: "el humano aprueba las acciones que requieren escritura" (index.txt, línea 114) y "escenarios de prueba" como entregable de la semana 2 (línea 177).

**Lo que NO dicen sobre evaluación (hueco real):** ninguna métrica, ninguna rúbrica, ningún umbral de aceptación, ningún LLM-as-judge, ninguna frecuencia de reejecución, ningún tamaño mínimo de suite, ninguna herramienta de evals. La evaluación queda como **disciplina artesanal descrita en 80 segundos**.

---

## 8. LÍMITES DE LA IA, ITERACIÓN Y MUERTE DEL HYPE (bloque prioritario)

Es el "DOMKNIĘCIE" (cierre) de la presentación de Ola, slides 21 y 22 de 22.

**8.1 El aviso honesto, enunciado como tal — [00:55:04–00:55:14]**
Slide (frame 0045): "**Teraz powiem wam coś zupełnie szczerze**" → "Ahora os voy a decir algo completamente sincero". Es un movimiento retórico deliberado y anunciado.

**8.2 La lista de lo que acaban de ver — [00:55:16–00:55:41]**
"Acabáis de ver un sistema que funciona realmente bien: tenéis una base de datos preciosa, **parece de verdad un cerebro**, hay conexiones, los datos están descargados, **se actualiza sola, se mejora sola**, tenemos conclusiones concretas, tenemos el artefacto construido... y ahora podéis pensar que **esto va a ser como una varita mágica**."

**8.3 La demolición — [00:55:41–00:56:05]**
"**ja zawsze bardzo lubię obalać hype**" → "**a mí siempre me gusta mucho derribar el hype**". Y: "**praca z modelem językowym to jest zawsze praca iteracyjna**; siempre pasará que habrá que promptearlo un poco, dirigirlo e iterar... y tras esas, ya sabéis, **olas de iteración**, al final tendremos un sistema que funciona de verdad".

**8.4 La cifra escondida en el slide — frame 0046 (00:56:12), slide 22/22**
Texto en pantalla: "**Widzisz wynik. Za nim stoi kilkadziesiąt podejść.**" → "**Ves el resultado. Detrás de él hay varias decenas de intentos.**" (junto a la etiqueta WYNIK / LLM brain). Es la cifra más honesta del webinar y **solo aparece escrita, no se pronuncia**: la voz dice "olas de iteración", la pantalla dice "decenas de intentos".

**8.5 Cierre — [00:56:11–00:56:35]**
"Es verdad que **cada vez es más fácil trabajar con ellos**, pero quiero terminar esta presentación precisamente con esa **muerte del hype (zabiciem tego hype'u)**, porque **me pone muy nerviosa** que la gente piense que esto es no sé qué y que solo con una varita mágica vamos a tener un resultado increíble, **olvidándose de la naturaleza de cómo funcionan los modelos de lenguaje y de que requieren iteración**."

**8.6 Límites adicionales dispersos en el tramo**
- El LLM es **probabilístico/estadístico**, y por eso la calidad depende de lo bien descrito que esté todo antes [00:58:56–00:59:06].
- El LLM **no conoce tu empresa**: no sabe cómo trabajan los equipos, dónde está el conocimiento ni a qué fuentes se puede confiar [01:02:09–01:02:20, vídeo de venta].
- Sin base estructurada, el LLM es **superficial y genérico** ante 5–10 ficheros [00:42:29–00:42:37].
- **No todo se resuelve con LLM** [01:08:01].
- Construir para dentro ≠ publicar fuera; **vender aplicaciones no es para no técnicos hoy** [01:14:02–01:14:35].

**Tensión interna que conviene registrar:** el mismo tramo que "mata el hype" contiene "**se actualiza sola, se mejora sola**" [00:55:29] y "**Claude recorrerá toda la base de datos y actualizará él solo todas las conexiones**" [00:40:41–00:40:53], afirmaciones fuertes que no se acompañan de ninguna demostración de fiabilidad. El antídoto (evaluación, casos de prueba) se enuncia, pero la promesa de autonomía se mantiene intacta.

---

## 9. ARGUMENTO DE VENTA COMPLETO: el hueco y el posicionamiento

**9.1 La cadena lógica exacta (00:57:18 → 01:03:20)**
1. El prompt ya no es la ventaja → **el sistema lo es** [00:57:18–00:57:45].
2. El modelo tampoco es el problema; da igual cuál uses salvo gasto masivo en tokens [00:57:50–00:58:19].
3. El problema real es humano y repetido: **le explicas la empresa a la IA desde cero cada vez** — y no lo arreglas porque **eres perezoso** [00:58:19–00:58:33].
4. Consecuencia: resultados flojos, porque el modelo es estadístico [00:58:50–00:59:06].
5. **Luego existe un hueco: nadie prepara a la empresa para el trabajo real con IA** [00:59:11].
6. Ese hueco **no lo tapan los programadores**; lo tapa quien sabe **ordenar conocimiento, convertirlo en procesos y preparar contexto** [00:59:18–01:00:27].
7. **Y ese es el AI Operator, y nosotros lo formamos en 5 semanas** [01:03:20–01:03:40].

**9.2 El vídeo de venta, transcrito íntegro (01:02:09–01:03:17)** — la definición canónica del rol:
> "La IA puede hacer muchísimo, solo hay un problema: **no conoce tu empresa**. No sabe cómo trabajan los equipos, dónde está el conocimiento, ni a qué fuentes se puede confiar. **El AI Operator habla con los equipos, ordena el conocimiento de la empresa, prepara el contexto y muestra qué tareas merece la pena entregarle de verdad a la IA.** No tienes que ser programador para entrar en este rol, porque hoy los humanistas y las personas con conocimiento de dominio pueden ser más útiles que los programadores, porque sabrán describirle bien a la IA el contexto de la empresa. Y si trabajas en IT, puedes ir más lejos: puedes crear tus propios MCP y conectar la IA con los sistemas de la empresa. **El AI Operator es capaz de coger un problema del equipo y, con ayuda de la IA, entregar por sí solo un resultado concreto: un análisis, un informe, una web, un prototipo o una mejora del prototipo.** Sabe preparar el contexto, elegir las herramientas y llevar el tema hasta algo que el equipo pueda usar. En la formación AI Operators, durante 5 semanas no solo aprenderás a usar la IA eficazmente, sino que **construirás un proyecto para tu portfolio**, y cada semana nos vemos en directo para comentar tus preguntas y avances."

**9.3 Diagnóstico del problema en dos versiones (slide frames 0083–0084, 01:04:33–01:05:00)**
- **Para no técnicos**: "En la empresa hay conocimiento y procesos, **pero falta la persona que los prepare para la IA**."
- **Para técnicos**: "Tienes sistemas y API, pero **el agente necesita herramientas seguras** para poder usarlos."
- Cierre del slide (frame 0085): "**Puedes convertirte en la persona de IA que prepara la empresa para trabajar con IA.**"

**9.4 La transformación prometida (frame 0082, 01:04:03)**
"HOY: usas la IA esporádicamente (p. ej. ChatGPT) → **DESPUÉS DE 5 SEMANAS: diseñas un sistema de IA que conoce tu trabajo.**"

**9.5 Palancas de conversión utilizadas, en orden**
1. **Prueba social pedida en directo** ("¿estáis de acuerdo en que estos 50 minutos han sido tiempo bien empleado? decidlo en el chat") — y los comentarios se muestran en pantalla [01:00:28–01:01:33].
2. **Permiso fingido**: "tengo una propuesta corta para vosotros y os pregunto si queréis oírla. Bueno, **me respondo yo solo y sigo**" [01:01:40–01:01:47].
3. **Acotación del tiempo**: "esta propuesta durará **15 minutos como máximo**" [01:01:55].
4. **Regalo pendiente como ancla de permanencia**: el curso "web en cuatro tardes" se entrega **después** del pitch [01:01:57, 01:24:09].
5. **Sin riesgo**: 7 días de garantía, 100 % del dinero [01:15:23–01:15:46, 01:18:31–01:18:43].
6. **Escasez de precio**: "hoy es el mejor momento, **esta precio no volverá nunca**, siempre será más caro después. **Es como comprar entrada de concierto: antes, más barato**" [01:18:51–01:19:19].
7. **Escasez inversa / prueba de honestidad**: el umbral de **100 personas** o se cancela y se devuelve todo [01:19:29–01:19:57]. Funciona a la vez como garantía moral y como llamada a la urgencia colectiva.
8. **Bono con caducidad de horas**: solo quien compre **hoy hasta las 23:59** [01:19:59–01:20:13, frame 0101].
9. **Argumento de ROI del bono**: las empresas pagan 500–1200 zł/mes por asistentes de voz; es "el proyecto con mayor retorno" para portfolio [01:21:00–01:21:55].
10. **Testimonio** de una participante no técnica de un programa anterior [01:17:57].
11. **Diferenciación moral frente a la competencia**: "no os echamos arena a los ojos... a esa gente no la respeto nada" [01:14:07–01:14:19].
12. **Insider framing**: "esta preventa, no lo oculto, la dirigimos a los clientes fijos; en publicidad hemos metido literalmente unos céntimos" [01:24:21–01:24:39].

**9.6 Objeciones que anticipan y cómo las desarman**
| Objeción | Respuesta en el webinar | Marca |
|---|---|---|
| "Soy lego, no me voy a aclarar" | 7 días de prueba + 100 % de devolución + material pensado para no técnicos | 01:15:19–01:15:58 |
| "No tengo conocimiento experto" | "Si tu trabajo actual es repetitivo, **nosotros te propondremos un proyecto**" | 01:15:58–01:16:25 |
| "No tengo ideas para el proyecto" | "No tienes que venir con uno hecho; te ayudaremos a encontrar un proceso y te enseñaremos un ejemplo completo" | 01:16:57 (slide) + 01:16:57–01:17:07 |
| "¿Me servirá en mi trabajo?" | "Si en tu trabajo hay información, decisiones y tareas repetitivas, **tienes qué mejorar**" (slide con MARKETING/VENTAS/OPERACIONES/RR.HH./IT/ANÁLISIS) | 01:16:33 (slide) + 01:16:41–01:16:55 |
| "No tengo tiempo, trabajo por cuenta ajena" | Programa diseñado para gente con empleo; sesiones en directo por la tarde; **todo se graba** | 01:17:12 (slide) + 01:17:15–01:17:33 |
| "Lo dejaré a medias" | Se avanza **con el grupo**: "no lo dejarás en el estante seguro" + foro + soporte | 01:17:35–01:17:51 |
| "Requisitos técnicos" | Solo para la ruta técnica: Bash, Git, API | 01:16:29–01:16:38 |

---

## 10. PERFIL PROFESIONAL: cómo describen al AI Operator

**10.1 Nombres que usan como sinónimos o vecinos — [01:12:45–01:13:17]**
Ola: "sé que hay muchísimos especialistas que tienen ese conocimiento experto y saben que si le añaden ese **skill de IA** pueden, desde su puesto de **project manager, product manager, comercial** o profesiones de negocio similares, **pasar a un rol que es como un operador de IA. Un solution engineer. O un product builder. Hay muchísima gente que tiene competencias afines.**"
→ Traducción de los tres nombres tal cual salen: **"operator AI" · "solution inżynier" · "product builder"**. No se define ninguno de los tres por separado; se presentan como etiquetas intercambiables de un mismo movimiento lateral de carrera.

**10.2 Definición funcional (del vídeo, §9.2)**
Cinco verbos: **hablar con los equipos · ordenar el conocimiento · preparar el contexto · señalar qué tareas delegar · entregar un resultado concreto** (análisis, informe, web, prototipo o mejora de prototipo). Más tres competencias: **preparar contexto, elegir herramientas, llevar el tema hasta algo usable por el equipo**.

**10.3 Perfil según la doctrina de Ola**
Es el "**specjalista wspierany przez AI**" (especialista asistido por IA) [00:54:08]: alguien que ha dejado de ejecutar y ahora **evalúa, piensa críticamente y decide estrategia**. Su valor es el conocimiento de dominio traducido a contexto.

**10.4 Perfil según la doctrina de Damian**
"Mi mayor skill hoy es que **sé conectar los puntos y poner bien el contexto**" [00:59:23]. Y la inversión jerárquica: **los humanistas y no técnicos tendrán ventaja sobre los programadores** porque describen mejor los problemas de dominio [00:59:34–01:00:05].

**10.5 Las dos rutas del programa como dos versiones del rol**
- **No técnica** (responsable: Ola) — [01:05:13–01:05:53]: ordenar el contexto y los procesos de la empresa; mejorar el trabajo propio y el de otros; iniciar proyectos internos y construir prototipos para necesidades de la empresa; construirse un **portfolio** para entrar al sector IA.
- **Técnica** (responsable: Damian) — [01:11:17–01:12:14]: construir una **capa segura entre el agente de IA y la API interna, los logs o la documentación de la empresa**; usarla, por ejemplo, para comprobar el estado de los sistemas ("buen conocimiento para gente de DevOps"). Problema que resuelve: "**las integraciones ya hechas se acaban justo donde empiezan los sistemas internos de la empresa**"; para un sistema interno propio es difícil que exista un conector MCP listo, así que hay que construírselo.
- **Acceso cruzado** [01:09:04–01:09:22]: "las personas no técnicas **también tienen acceso a la ruta técnica**. No lo separamos. Recibís acceso a todo. Vosotros decidís por qué ruta ir."

**10.6 El proyecto de portfolio como prueba de identidad — [01:13:17–01:13:33]**
"De lo que se trata es de que seáis capaces de hacer algo que sea vuestro proyecto para el portfolio: **'oye, cogí mi conocimiento experto, hice una solución de IA, y mira lo que tengo ahora en mi CV'**. Y de verdad sé usar esa IA junto con mi conocimiento experto."

---

## 11. Citas literales potentes (polaco → español)

1. **[00:48:09]** "…najważniejszy jesteśmy my, najważniejsza jest ta nasza tutaj wiedza ekspercka i to nasze działanie krytyczne…"
 → "…lo más importante somos nosotros, lo más importante es nuestro conocimiento experto y nuestra actuación crítica…"
2. **[00:48:38]** "Kiedyś się mówiło, że dane są jak ropa, teraz mówi się o tym, że kontekst jest jak ropa."
 → "Antes se decía que los datos son como el petróleo; ahora se dice que **el contexto es como el petróleo**."
3. **[00:50:42]** "To jest taki krytyczny punkt pracy z modelami językowymi, że zawsze musimy oceniać, jak ten model językowy zwraca nam te odpowiedzi."
 → "Es un punto crítico del trabajo con modelos de lenguaje: **siempre tenemos que evaluar cómo nos devuelve las respuestas**."
4. **[00:51:35]** "…czy jak na przykład dodamy mu 15 innych plików, czy on nie zacznie się gubić i nie zacznie nagle odpowiadać gorzej…"
 → "…si le añadimos otros 15 ficheros, ¿no empezará a perderse y de pronto a responder peor?…"
5. **[00:51:49]** "…czy ona nie degraduje z czasem, czy ona faktycznie się ulepsza i czy ten kontekst pozostaje zachowany."
 → "…si no se degrada con el tiempo, si de verdad mejora, y **si el contexto se mantiene**."
6. **[00:54:47]** "…jest bardzo duży hype teraz na AI i myślimy, że ono jest w stanie rozwiązać wszystko, ale to jest tylko technologia."
 → "…hay muchísimo hype con la IA y pensamos que puede resolverlo todo, **pero es solo una tecnología**."
7. **Slide 22/22 [00:56:12]** "Widzisz wynik. Za nim stoi kilkadziesiąt podejść."
 → "**Ves el resultado. Detrás hay varias decenas de intentos.**"
8. **[00:55:47]** "…ja zawsze bardzo lubię obalać hype…"
 → "…a mí siempre me gusta mucho **derribar el hype**…"
9. **[00:56:16]** "…chcę zakończyć tę prezentację takim zabiciem tego hype'u, bo strasznie mnie on denerwuje."
 → "…quiero terminar esta presentación **matando ese hype**, porque me pone terriblemente nerviosa."
10. **[00:57:18]** "…dzisiaj promptowanie już nie ma sensu… sam prompt nie rozwiązuje takich problemów… Przewagą jest zbudowanie systemu."
 → "…hoy el prompteo ya no tiene sentido… el prompt por sí solo no resuelve esos problemas… **La ventaja está en construir un sistema**."
11. **[00:58:04]** "…to nie ma większego znaczenia, którego modelu używasz, dopóki naprawdę nie wydajesz setek tysięcy albo tysięcy na te tokeny."
 → "…**no importa demasiado qué modelo uses**, mientras no gastes de verdad cientos de miles o miles en tokens."
12. **[00:58:27]** "…ludzie są leniwi, ja też jestem leniwy i nie chce mi się za każdym razem tłumaczyć wszystkiego…"
 → "…la gente es perezosa, **yo también soy perezoso** y no me apetece explicarlo todo cada vez…"
13. **[00:59:11]** "I tu się właśnie pojawia luka, kto przygotuje firmę do realnej pracy z AI."
 → "**Y aquí aparece el hueco: ¿quién preparará a la empresa para el trabajo real con IA?**"
14. **[00:59:34]** "…dzisiaj to humaniści, czy też ludzie nietechniczni często będą mieli przewagę nad programistami. Gdybym powiedział to 5 lat temu… to by mnie wszyscy wyśmiali, zlinczowali."
 → "…hoy los humanistas o los no técnicos a menudo tendrán **ventaja sobre los programadores**. Si lo hubiera dicho hace 5 años, todos se habrían reído de mí, me habrían linchado."
15. **[01:02:14]** "AI potrafi zrobić bardzo dużo, tylko jest jeden problem. Nie zna Twojej firmy."
 → "La IA puede hacer muchísimo, solo hay un problema: **no conoce tu empresa**."
16. **[01:14:07]** "…nie mydlimy wam tu oczu, że nauczycie się budować aplikacje i potem je sprzedawać. Absolutnie nie… wiem, że są w internecie ludzie, którzy w ten sposób mydlą oczy ludziom. I bardzo ich nie szanuję."
 → "…**no os echamos arena a los ojos** diciendo que aprenderéis a construir aplicaciones y luego venderlas. **En absoluto**… sé que en internet hay gente que engaña así, y **no los respeto nada**."
17. **[01:14:25]** "…zbudowanie czegoś na potrzeby wewnętrzne, a udostępnienie tego do internetu, to są w ogóle dwa różne światy i dwie różne ścieżki."
 → "…construir algo para uso interno y publicarlo en internet **son dos mundos distintos y dos caminos distintos**."
18. **[01:15:00]** "…jak tworzyć strony, które nie wyglądają jak AI generated, tylko wyglądają jakby wyszły od designera."
 → "…cómo hacer webs **que no parezcan generadas por IA**, sino que parezcan salidas de un diseñador."
19. **[01:19:31]** "…musi do nas dołączyć minimum 100 osób… Jeśli nie uzbieramy tych 100 osób, to anulujemy projekt całkowicie."
 → "…tienen que apuntarse **mínimo 100 personas**… Si no reunimos esas 100, **cancelamos el proyecto por completo**."
20. **[01:19:15]** "Przedsprzedaż jak kupujecie bilet na koncert. Wcześniej to macie taniej."
 → "La preventa es como comprar entrada de concierto: **antes, más barato**."
21. **[01:24:33]** "…w reklamę wrzuciliśmy dosłownie parę groszy… specjalnie po to, żeby dołączyli nasi stali klienci."
 → "…en publicidad hemos metido **literalmente unos céntimos**… precisamente para que se apunten nuestros clientes habituales."
22. **[01:01:44]** "I mam tutaj pytanie, czy chcecie ją usłyszeć. Ale w sumie odpowiem sobie sam i pójdę dalej."
 → "Y os pregunto si queréis oírla. Pero en el fondo **me respondo yo solo y sigo**."

---

## 12. Venta vs. docencia — dónde cae la línea

**Docencia real (contenido transferible, sin coste):**
- 00:40:07–00:41:24 — mantenimiento incremental de una base de conocimiento; el agente reindexa relaciones al añadir un nodo.
- 00:42:25–00:43:06 — por qué el "sube 10 ficheros al chat" degrada; el manual de uso dentro de la propia base.
- 00:47:36–00:48:03 — principio de mínimo privilegio: solo los conectores necesarios, una carpeta.
- 00:48:09–00:48:33 — el bucle humano comprobar/aprobar/iterar/dirigir.
- 00:50:27–00:51:53 — **evaluación y casos de prueba** (el mejor material del tramo).
- 00:52:15–00:55:02 — los 5 elementos como checklist.
- 00:55:04–00:56:35 — la iteración como naturaleza del medio; "decenas de intentos".
- 00:57:50–00:59:06 — el modelo no es el cuello de botella; el LLM es probabilístico.

**Venta pura (promesa, no método):**
- 00:41:55 — "es algo bonito de mostrar" y "sirve para muchísimas empresas" (argumento de escaparate, no técnico).
- 00:44:46–00:45:09 — el tip de usar el análisis para conseguir trabajo/clientes: aspiracional.
- 00:49:26–00:50:17 — el catálogo de 6 casos de uso, todos enunciados, ninguno demostrado.
- 01:01:40–01:03:20 — permiso fingido + vídeo publicitario.
- 01:03:20–01:24:07 — programa, semanas, garantía, precio, umbral, bono.

**Zona híbrida (docencia usada como prueba de capacidad de los formadores):**
- 00:46:47–00:47:33 — "esto es un prototipo" + la lista de cinco competencias, que es a la vez pedagogía y guion del producto que venden.
- 01:06:54–01:11:08 — el temario semanal contiene **conceptos reales enunciados** (mapa del proceso propio; agente con rol, herramientas, **límites de actuación y forma de evaluar el resultado**; contexto versionado + skill propio; grafos vs. RAG), pero **sin ninguna explicación**: son títulos de lo que hay tras el pago.

**Lo que explícitamente queda tras el pago (según ellos mismos):**
construir servidores MCP propios (semana 5, ruta técnica); crear skills desde cero (semana 2); versionado de contexto (semana 3); panorama de bases de conocimiento incluidos RAG (semana 4); criterios de decisión determinista/no determinista (semana 1); prototipos de aplicación para product managers; cómo hacer webs que no parezcan de IA; y el curso-bono del asistente de voz telefónico.

---

## 13. Contradicciones, huecos y señales a vigilar

1. **Lapsus del guion en [01:05:54]**: dice "**W ścieżce nietechnicznej** nauczymy Was jak łączyć agentów z systemami firmy… zbudujemy własny serwer MCP" ("en la ruta **no técnica** os enseñaremos a conectar agentes con los sistemas de la empresa… construiremos un servidor MCP propio"). Contradice todo lo demás [01:08:56, 01:11:17]: construir MCP es de la **ruta técnica**. Es un desliz oral, pero si alguien compra por esa frase, la expectativa queda mal fijada.
2. **8 de 59 dicho vs. 5 de 59 / 7 de 59 en pantalla** [00:44:18 vs. frames 0038/0040]: la cifra que sostiene el "gran hallazgo" del demo no coincide con el artefacto que se está mostrando.
3. **"Se actualiza sola, se mejora sola"** [00:55:29] convive en el mismo minuto con "detrás hay decenas de intentos" [frame 0046]. La autonomía se afirma; el coste se admite solo en el slide.
4. **La evaluación se declara "punto crítico" y se despacha en ~80 segundos**, sin métricas ni herramientas — justo el bloque que separaría a un profesional de un entusiasta.
5. **Autoridad asimétrica**: Ola aporta el contenido técnico y la honestidad epistémica; Damian aporta el marco de mercado y toda la maquinaria de conversión. La frase "yo también sé programar, pero hoy ya no programo" [00:59:20] sostiene su autoridad sin evidencia mostrada en el tramo.
6. **El "hueco de mercado" no se apoya en ningún dato**: ni ofertas de empleo, ni salarios, ni encuestas. La única cifra de mercado del tramo (500–1200 zł/mes por asistentes de voz) pertenece al **bono**, no al rol de AI Operator.
7. **Escasez con doble filo**: "esta precio no volverá nunca" + "mínimo 100 personas o cancelamos" + "bono solo hasta las 23:59" en menos de 5 minutos, todo ello después de haber declarado que no harían un webinar de trucos.
8. **Fechas que conviene fijar**: webinar y cierre de preventa = **2 de septiembre** (slide frame 0098); inicio = **octubre** (web: 26 de octubre); garantía hasta el **2 de noviembre**; bono entregado en **septiembre**. Coherentes entre sí, pero el bono llega antes que el curso comprado.
9. **Incertidumbre admitida en directo** [01:22:11–01:22:31]: sobre si el desvío de llamadas funciona en Android — "no estoy seguro… calculo un 80 %… seguridad al 100 % no la tengo". Es el momento más honesto del Q&A y también el único dato duro que ofrece del bono.
10. **Doble tratamiento del "no engañamos"**: se marca distancia moral frente a los vendedores de "construye y vende apps" [01:14:07] mientras se usa la batería completa de técnicas de urgencia. La honestidad se ejerce sobre el **alcance del contenido**, no sobre el **método de venta**.

---

## 14. Qué me llevo de este tramo para el proyecto

- El **único bloque metodológico verdaderamente escaso en el mercado hispanohablante** que aparece aquí es §7 (evaluación con casos de prueba y detección de degradación por crecimiento del corpus). Está bien planteado y mal desarrollado: es el hueco a llenar.
- La frase del slide "**Ves el resultado. Detrás hay varias decenas de intentos**" es el mejor resumen honesto de todo el webinar y merece ser un principio propio, no una nota al pie.
- El **argumento del hueco** ("¿quién prepara a la empresa para trabajar de verdad con IA?") es sólido como diagnóstico y **completamente indocumentado** como afirmación de mercado. Reutilizable, pero exige datos propios.
- La distinción **prototipo interno vs. producto publicado** es la línea de honestidad más útil que trazan, y la trazan bien.
