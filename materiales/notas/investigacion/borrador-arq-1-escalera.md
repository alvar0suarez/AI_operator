# Arquitectura 1 — LA ESCALERA ES EL CURSO

**Qué es esto.** Un diseño de arquitectura completo y defendible para el curso de la alumna descrita
en `00-perfil.md`, construido sobre el ángulo 1: la progresión que ella misma pidió —chat → automatización
→ agente → (opcional) avanzado— no es una restricción a acomodar, es la columna vertebral pedagógica.

**Fecha:** 22.08.2026.

**Documentos que da por leídos:** `00-perfil.md` (fuente de verdad del encargo, corregida),
`01-analisis-referencia.md`, `dominio-academia.md` (P01–P32), `dominio-rgpd.md` (E-01…E-06, el semáforo),
`dominio-herramientas.md` (escalera 0→4, límites de plataforma verificados), `dominio-autodidacta.md`
(mecanismos de corrección sin profesor, puntos de caída, plantillas), `dominio-psicologia.md`
(correspondencias C1–C13, ejercicios EP-01…EP-14).

**Convención de marcas** (heredada de los documentos de dominio):
**[V]** verificado en fuente primaria · **[R]** reconstrucción razonada · **[NV]** no verificable desde
fuera · **[!]** decisión que no es suya y se escala · **[J]** juicio de diseño mío, argumentado.

---

## 1. TESIS

### 1.1 El enunciado

> **La escalera no es el orden en que se presentan las herramientas. Es una secuencia de techos.**
>
> Cada escalón existe porque el anterior tiene un límite concreto, y ese límite hay que **chocar con
> él en su trabajo real**, no leerlo. El curso no enseña Gems, ni flujos, ni agentes: enseña a
> reconocer el techo en el que estás y a decidir si merece la pena romperlo. La herramienta es lo que
> se compra con esa decisión.

Corolario que hace el diseño operativo: **se sube cuando el escalón anterior ha producido algo que
funciona y se ha quedado corto**. No cuando el calendario lo dice, no cuando apetece. Y cada escalón
trae escrito, con el mismo peso, **cuándo NO subir** — porque la mitad del criterio consiste en saber
que una automatización simple basta, y la otra mitad en saber que a veces no hace falta IA en absoluto.

### 1.2 Los cinco techos, nombrados

Esta tabla es el curso. Todo lo demás es implementación.

| # | Escalón | El techo que se choca **en su trabajo**, no en teoría | Lo que lo rompe |
|---|---|---|---|
| **0** | Chat tal cual lo usa hoy | *"Cada conversación empieza en blanco y le vuelvo a explicar la academia."* Y: no sabe con qué cuenta está entrando ni qué protege esa cuenta | Diagnóstico + instrucciones personalizadas |
| **1** | Chat con contexto (instrucciones, Gem, cuaderno) | *"Se acuerda de sus instrucciones, no de lo que pasó ayer. Y sigo teniendo que abrirlo yo cada vez."* La memoria fiable es un fichero; el disparador sigue siendo su dedo | Automatización: el disparador deja de ser ella |
| **1,5** | Acción programada + `=AI()` en la hoja | *"Dispara por calendario. No reacciona a que **haya pasado algo**."* Un lunes no es un evento; que entre un correo, sí | Workspace Studio: disparadores por suceso |
| **2** | Flujo determinista | *"Siempre el mismo camino. El caso que no previste sale mal, y sale mal en silencio."* | Juicio en puntos concretos del flujo (`Decide`, `Extract`) |
| **3** | Flujo con juicio | *"Sigue siendo un camino con bifurcaciones que yo dibujé. No sirve para una tarea cuyos pasos hay que decidir sobre la marcha, ni para procesar cincuenta ficheros locales."* | Agentes de verdad — **y aquí se explica por qué hoy están fuera de su alcance por licencia y por permisos, no por capacidad suya** |

El escalón 4 (Claude Code, Cowork, Antigravity) **no se sube: se lee**. Su objetivo declarado no es que
lo use, sino que sepa qué es y por qué hoy no lo necesita. `dominio-herramientas.md` §5.2 lo argumenta
sin ambigüedad: no resuelve mejor ninguno de sus 32 procesos, está fuera del estándar de su empresa y
cuesta dinero de su bolsillo.

Y hay un escalón **por debajo del 0**, que es el que más rendimiento da y el que ningún curso pone:

| **−1** | **Ni IA.** La tarea tiene pasos fijos y datos estructurados: no necesita un modelo de lenguaje, necesita una fórmula, un filtro o un calendario de recursos. Ejemplo canónico de su casa: **P02, el presupuesto**, que es aritmética sobre una tabla de precios; y **P22, la hoja de camas**, que es un calendario de ocupación |

### 1.3 Por qué esta tesis es la correcta para ESTA alumna con ESTE objetivo

Cinco razones, en orden de peso. Las tres primeras son específicas de ella; ninguna sería igual de
fuerte con otro perfil.

**(a) Porque su objetivo es un cambio de hábito, y un hábito no se cambia con un mapa.**
El encargo dice literalmente *"salir del hábito del chat"*. Un hábito se sustituye cuando el gesto
antiguo produce un resultado peor que el nuevo **en su propia mano**, no cuando alguien le explica
que existe algo mejor. La estructura de techos convierte cada transición en una experiencia: la
primera vez que el Gem no se acuerda de lo que pasó ayer, la primera vez que la acción programada
dispara un lunes sin que haya llegado nada, la primera vez que el flujo se traga un caso que no
previó. Un temario ordenado por conceptos le contaría esas cinco cosas; la escalera se las hace.

**(b) Porque la continuidad de herramienta es literal, no metafórica** [V, `dominio-herramientas.md`
§1.2.h]. Workspace Studio tiene un paso `Ask a Gem` y un paso `Ask Gemini Notebook`. El Gem que
construye en la semana 5 **se convierte en un paso de un flujo en la semana 10 sin reescribir nada**.
Eso significa que el escalón no es un cambio de herramienta con coste de aprendizaje: es una
capitalización. En Make o n8n tendría que rehacerlo; aquí lo hereda. Ninguna otra estructura del
curso aprovecha ese hecho, y es el mejor argumento que tenemos, porque no es pedagógico: es del
producto.

**(c) Porque su formación le da ventaja exactamente en la juntura entre escalones.**
`dominio-psicologia.md` documenta que el solapamiento fuerte está en dos sitios: **escribir el
criterio antes de construir** (C1, operacionalizar) y **comprobar si el resultado sirve** (C7, C13,
evaluación). Esas dos cosas no son escalones: son lo que se hace **al pie de cada escalón y al llegar
arriba**. Una arquitectura ordenada por herramientas dejaría su ventaja fuera del temario; una
arquitectura ordenada por techos la pone en el sitio donde se decide subir o no. Ahí es donde el curso
tiene que gastar sus mejores páginas.

**(d) Porque el orden coincide con el orden del riesgo, y eso no es casualidad.**
El escalón bajo toca datos verdes y errores internos y reversibles; el alto toca datos ámbar y
errores que ve un cliente. `dominio-rgpd.md` §7.4 llega a la misma conclusión desde el ángulo
contrario —*empezar por lo interno, donde el error es barato*— y `dominio-herramientas.md` §9.6 desde
el ángulo del producto. **Tres análisis independientes convergen en la misma secuencia.** Eso es lo
más parecido a una validación que se puede tener antes de escribir el material.

**(e) Porque le quita de encima la barrera de entrada.**
Escalones 0, 1, 1,5, 2 y 3 se recorren **con cero instalaciones, cero altas de proveedor, cero
peticiones de licencia y cero euros**, dentro de lo que su empresa ya paga [V]. En un curso
autodidacta con jornada completa, donde el 52 % de la mortalidad ocurre antes de la primera lección
[E, Reich y Ruipérez-Valiente 2019], la fricción de arranque no es un detalle de comodidad: es el
factor de mortalidad número uno.

### 1.4 EL RIESGO DE ESTA TESIS, DICHO ANTES DE DEFENDERLA

El riesgo es real y hay que enunciarlo con las peores palabras posibles antes de contestarlo:

> **Una escalera de herramientas produce, por defecto, tres tutoriales encadenados.** Al final la
> alumna sabe hacer un Gem, sabe hacer un flujo y sabe poner un `Decide` en medio; y en cuanto Google
> renombre algo o cambie de empresa, no le queda nada. El criterio —lo único que el brief dice que no
> caduca— se habría quedado en las frases de transición entre módulos.

El riesgo se agrava por dos cosas específicas de este caso. Una: **la herramienta es el temario**, así
que no hay distancia natural entre "aprender a usar Studio" y "aprender a decidir". Dos:
`dominio-herramientas.md` §8.1 documenta que en 2026 han cambiado de nombre tres piezas centrales en
cinco meses (Flows→Studio, NotebookLM→Gemini Notebook, Gemini CLI→Antigravity CLI). Un curso
construido sobre nombres de menú nace con fecha de caducidad de meses.

### 1.5 LA SALVAGUARDA: cuatro mecanismos, no una advertencia

Una advertencia en la introducción no es una salvaguarda. Estos cuatro son estructurales: si se
quitan, el curso se rompe visiblemente, que es la propiedad que define una salvaguarda de verdad.

---

**Salvaguarda 1 · LA BATERÍA ES EL INVARIANTE. La herramienta es la variable.**

En el módulo 1, antes de tocar ninguna herramienta, ella construye **una batería de 10 casos reales de
su trabajo** con la tabla de especificaciones de `dominio-psicologia.md` C2: 5 normales, 3 límite, 2
que el sistema debe rechazar. Y la pasa **contra el chat pelado que usa hoy**, anotando el resultado
con fecha en una hoja.

Esa misma batería, sin cambiar ni un caso, se vuelve a pasar **al final de cada escalón**. Una columna
nueva por escalón, con su fecha. Al terminar el curso, la hoja tiene esta forma:

```
CASO                     | chat hoy | +Gem/cuad | +progr. | +flujo | +juicio
                         | 12-oct   | 09-nov    | 23-nov  | 21-dic | 25-ene
-------------------------|----------|-----------|---------|--------|--------
N1 precio 4 semanas      |   NO     |    SÍ     |   SÍ    |  SÍ    |   SÍ
N2 fechas de inicio      |   SÍ     |    SÍ     |   SÍ    |  SÍ    |   SÍ
...
L1 mixto: curso+piso     |  inventa |  pregunta | pregunta| pregunta| pregunta
L2 queja educada         |  inventa |  inventa  | inventa | pregunta| pregunta
...
R1 plazo de visado       |  responde|  no lo sé | no lo sé| PARAR  |  PARAR
R2 dato que no tiene     |  inventa |  no lo sé | no lo sé| no lo sé| no lo sé
```

**Lo que esa hoja enseña, y que ninguna lección puede enseñar igual de bien:** entre la columna 2 y la
columna 5 **casi nada mejora**. La calidad de la respuesta se gana entera en el escalón 1 —cuando se
escribe el criterio y se le dan fuentes con fecha— y a partir de ahí sólo se puede perder. Lo que
cambia al subir no es la calidad: es **quién dispara, cuántas veces, y cuánta autonomía has cedido**.

Ese es el criterio transferible del curso, y no se lo cuenta nadie: lo lee en su propia hoja. Si
dentro de tres años le ponen delante una herramienta que no existe hoy, la pregunta que sabrá hacer
es *"¿esto me cambia la calidad o me cambia el disparador?"*, que es la pregunta correcta.

**Y sirve además como red anti-caducidad:** la hoja de anclas es un artefacto suyo, en su Drive, que
sobrevive a cualquier renombrado de Google (`dominio-psicologia.md` C3, ítems ancla).

---

**Salvaguarda 2 · Cada escalón tiene una PUERTA con condición observable, y la puerta no la abre el
calendario.**

| Puerta | Condición para subir — todas observables, ninguna valorativa |
|---|---|
| **0 → 1** | Existe el fichero *Mi Workspace* con el plan **o** con la frase *"pregunté a X el día D y no obtuve respuesta"* · existe su semáforo verde/ámbar/rojo adaptado · hay una tarea elegida con puntuación positiva y **ningún −3** en el filtro de E-04 · hay una línea base **medida**, no estimada |
| **1 → 1,5** | La batería da **5/5** en los normales, **pide aclaración** en los 3 límite (inventar una decisión es fallo aunque acierte) y dice **"no lo sé"** en los 2 de rechazo · **y** ha usado el Gem al menos 5 veces en una semana **sin que el curso se lo pidiera** |
| **1,5 → 2** | Su codificación manual de 30 comentarios y la de la columna `=AI()` coinciden en **≥26**, y hay **una frase escrita por cada confusión repetida** de la tabla de confusión |
| **2 → 3** | **Dos flujos vivos** y **haber visto uno fallar**, sabiendo por qué falló |
| **3 → 4** | *No existe.* El escalón 4 no se sube: se lee |

La segunda condición de la puerta 1→1,5 es la más importante del curso y merece explicarse: **si no
usa el Gem espontáneamente, el Gem está mal, y automatizar algo que está mal es multiplicar el error**
[`dominio-herramientas.md` §7.3]. La puerta no mide si aprendió la lección; mide si el artefacto le
sirve. Es la única forma honesta de saberlo sin profesor.

La condición de la puerta 2→3 es igual de deliberada: **sin haber visto un fallo no hay criterio para
dar autonomía a nada.** Si en el módulo 5 no ha fallado nada, el material trae un fallo provocado.

---

**Salvaguarda 3 · Cada escalón lleva su "CUÁNDO NO SUBIR", y no subir se evalúa.**

No basta con escribirlo: hay que puntuarlo. En el módulo 6 hay un entregable obligatorio que es **la
lista de lo que ha decidido NO automatizar, con el motivo por escrito**. La rúbrica declara
explícitamente que **un módulo en el que todo acaba automatizado está mal resuelto**, y da los tres
motivos legítimos de descarte: riesgo (el error lo paga un cliente o una administración), coste
completo negativo (ahorra ocho minutos y cuesta diez de revisión), y escalón equivocado (la tarea es
determinista y no necesita un modelo, necesita una fórmula).

---

**Salvaguarda 4 · CASOS SATÉLITE: cada módulo lleva un ejercicio de 15 minutos sobre un proceso
distinto del hilo.**

Es la contramedida a la trampa documentada en `dominio-autodidacta.md` §7.3 ("el proyecto se come el
temario"). Si todo lo que hace es su proyecto, aprende una solución, no un criterio. El caso satélite
la obliga a aplicar el mismo criterio a un proceso que no es el suyo y que a veces **no admite la
solución del módulo** — que es justamente donde el criterio se hace visible.

Ejemplos de satélites, uno por módulo, sacados del inventario: P02 presupuesto (respuesta correcta:
escalón −1, ni IA) · P08 carta de visado (respuesta correcta: zona prohibida, y por un motivo que no
es la dificultad sino que la normativa cambia de un año a otro) · P30 parte semanal (respuesta
correcta: automatización determinista pura, sin modelo de lenguaje en el camino crítico) · P28 reseñas
(respuesta correcta: clasificar y preparar sí, publicar nunca, y hay un motivo de RGPD) · P16 exámenes
DELE (respuesta correcta: las reglas son de otro, el sistema no puede saberlas).

---

### 1.6 Qué tomamos de la referencia y qué no, en una frase

Los **cinco pasos** del programa polaco son correctos y su orden se sostiene. Lo que hacemos es
**dejar de usarlos como columna vertebral y usarlos como capa transversal**: cada escalón de nuestra
escalera ejecuta los cinco pasos completos a su nivel. El paso 4 (acceso a herramientas) se encoge a
una página, porque en su pila no hay nada que conectar por MCP y decirlo es más honesto que inflarlo;
el paso 5 (evaluación) se expande y **se muda del final al pie de cada escalón**, que es el cambio
estructural más importante respecto a la referencia y el que su formación permite.

---

## 2. RESULTADOS DE APRENDIZAJE OBSERVABLES

Redactados como desempeños. Cada uno lleva **cómo se ve que ha ocurrido** y el módulo donde se
verifica. Ninguno usa "entenderá", "conocerá" o "será capaz de apreciar".

| # | Al terminar, ella… | Se observa en | Módulo |
|---|---|---|---|
| **RA1** | **Determina** con qué cuenta y bajo qué régimen de datos está trabajando, y **cita** el distintivo, la edición y el plazo de retención, o la constancia documentada de haberlos preguntado | El fichero *Mi Workspace*, sin ninguna frase que empiece por "creo que" | M0 |
| **RA2** | **Clasifica** cualquier dato de su puesto en verde / ámbar / rojo y **reescribe** un caso real hasta que una compañera no pueda identificar a la persona | 10 correos clasificados; 3 casos reescritos que superan la prueba de la compañera; y al menos uno declarado **no reescribible** | M0, M2 |
| **RA3** | **Escribe** el criterio de "resultado correcto" de una tarea suya en 4–6 indicadores que otra persona pueda comprobar sí/no contra una fuente, **antes** de tocar ninguna herramienta | La ficha de criterio, sin las palabras *adecuado, correcto, natural, profesional, de calidad* sin ancla detrás | M1 |
| **RA4** | **Construye** una batería de 10 casos —5 normales, 3 límite, 2 de rechazo— con casos que **no** usó para escribir el prompt, y **la vuelve a pasar** cada vez que cambia algo, anotando la fecha | La hoja de anclas con una columna por escalón y fecha en cada una | M1 → M7 |
| **RA5** | **Construye** un asistente reutilizable y una base de fuentes que responde **citando el documento y su fecha** y que **dice "no lo sé"** cuando la respuesta no está | La batería: 5/5 normales, pregunta en los límite, "no lo sé" en los 2 de rechazo | M2 |
| **RA6** | **Codifica** texto libre multilingüe aplicando un libro de códigos cerrado y **compara** su codificación con la del sistema construyendo la tabla de confusión | ≥26/30 de acuerdo y una frase escrita por cada confusión repetida | M3 |
| **RA7** | **Construye** un flujo con disparador por suceso que **prepara, clasifica o avisa, y nunca envía**, con condiciones de parada, lista de temas prohibidos y tope de volumen | Dos flujos vivos; el apagado **probado**, no imaginado; ningún paso que salga a un cliente sin aprobación | M4, M5 |
| **RA8** | **Decide y justifica**, para cada tarea candidata, el escalón que le corresponde —incluido **"ni IA"** y **"no automatizar"**— y **nombra qué tendría que cambiar** para que la decisión fuera otra | La lista de descartes del M6, con motivo y condición de revisión por cada uno | M6 |
| **RA9** | **Mide** el efecto de un sistema suyo con línea base, unidad por pieza de trabajo y coste completo, y **nombra una amenaza a la validez interna que no puede descartar** | Media página por sistema, sin la palabra "significativo", con el tiempo de revisión restado | M6 |
| **RA10** | **Distingue**, mirando su hoja de anclas, qué aportó cada escalón: dónde cambió la calidad y dónde sólo cambió el disparador | Una frase escrita por columna de la hoja | M7 |
| **RA11** | **Explica** qué son agente, MCP, conector, agente de navegador y base de conocimiento con fuentes, **y por qué hoy no los usa y qué tendría que pasar para usarlos** | El fichero *Mapa de lo que existe*, escrito por ella, con la columna de condición de disparo rellena | M7 |
| **RA12** | **Corrige** su propio trabajo con la IA aplicando el protocolo de siete reglas, y **audita al corrector** con un artefacto de defectos plantados antes de fiarse de él | Resultado del cebo anotado; y al menos un caso registrado en el que decidió **no** aceptar una crítica de la IA, con el motivo | M2, M5 |
| **RA13** | **Escribe la rúbrica** de un artefacto suyo, con al menos tres criterios negativos que exigen salida escrita | La rúbrica del M7, redactada por ella y aplicada al día siguiente en tercera persona | M7 |

**RA13 es el criterio de terminación del curso.** Cuando puede escribir los criterios de su propio
artefacto, ya no necesita el material. Es el único indicador honesto de fin, y va escrito en la
semana 1.

---

## 3. MAPA DE MÓDULOS

### 3.1 Vista general

Duración total **18 semanas**, 9 módulos + 1 opcional. Módulo = 2 semanas = **3 sesiones núcleo de
35–45 min + 1 bloque de proyecto de 60–90 min + evaluación**. Presupuesto: **2 h semanales de tiempo
propio**; el bloque de proyecto es **tiempo de trabajo**, porque es trabajo del puesto hecho de otra
manera, y el material lo declara así explícitamente en cada lección. **Arranque en octubre**: el pico
de junio–septiembre de la academia mata cualquier calendario que lo ignore [`dominio-autodidacta.md`
§5.5].

| Mód. | Título | Escalón | Semanas | Herramienta nueva |
|---|---|---|---|---|
| **M0** | Dónde estoy parada | 0 | 1–2 | ninguna (Gemini con la cuenta correcta) |
| **M1** | Escribir el criterio antes que el prompt | 1a | 3–4 | **ninguna, a propósito** |
| **M2** | Un asistente que ya sabe dónde trabajas | 1b | 5–6 | Gems + Gemini Notebook |
| **M3** | La primera vez que pasa algo sin ti | 1,5 | 7–8 | Acciones programadas + `=AI()` |
| **M4** | Del artefacto al disparador | 2a | 9–10 | Google Workspace Studio |
| **M5** | Prepara, no envíes | 2b | 11–12 | (Studio + Notebook, sin nada nuevo) |
| **M6** | ¿Esto sirve de verdad? | 2c | 13–14 | ninguna |
| **M7** | Juicio dentro del flujo — y por qué no un agente | 3 | 15–17 | pasos de IA de Studio |
| **M8** | Cerrar y dejarlo vivo | — | 18 | ninguna |
| **M9** | *(opcional)* Lo que hay más arriba | 4 | — | ninguna. Es lectura |

**Herramientas nuevas en 18 semanas: tres.** Máximo una por módulo, y ninguna se introduce antes de
haber agotado la anterior [`dominio-herramientas.md` §7.1].

---

### 3.2 M0 · Dónde estoy parada

| | |
|---|---|
| **Cambio mental** | *"La IA no es una web a la que voy. Es una herramienta con una configuración, un dueño y un perímetro — y el mismo texto en la misma pantalla es seguro o no según con qué cuenta haya entrado."* |
| **Qué construye** | (1) instrucciones personalizadas activas en Gemini de empresa; (2) el fichero **Mi Workspace** (E-01); (3) su **semáforo** verde/ámbar/rojo adaptado a la academia, impreso; (4) su inventario de tareas, corrigiendo con tachones el mapa de P01–P32; (5) el **hilo propio** elegido con el filtro puntuado de E-04; (6) la **línea base medida** del proceso elegido (EP-09) |
| **Duración** | 2 semanas · ~4 h propias |
| **Herramienta y por qué** | Gemini con la cuenta de la academia y un documento de texto. Nada más. **Porque la sesión 1 no puede exigir instalar, registrarse ni pedir nada a nadie**: el 52 % de la mortalidad de un curso autodidacta ocurre antes de la primera lección [E] |
| **Cómo se autocorrige** | **Cuatro mecanismos, ninguno de juicio.** (a) La rúbrica de 8 casillas de E-01, con el estándar duro: *"no lo sé y lo he preguntado" vale; "creo que sí" no vale*. (b) **E-05, verdadero/falso de 12 ítems con solución al pie**: corrección instantánea, umbral <10 aciertos → releer. (c) El filtro de E-04 tiene **descalificadores por número de proceso** (P08, P17, P22, P25, P26, P29 quedan fuera automáticamente): es aritmética, no criterio. (d) La línea base es una medición: no se evalúa, se compara en el M6 |

**Secuencia interna, y por qué esta y no otra:**

- **Sesión 1 (20 min) — "El primer minuto ganado".** Abre `gemini.google.com` **con la cuenta de la
  academia**, mira el distintivo de arriba (Pro / Expanded / Ultra / ninguno) y lo anota, escribe sus
  instrucciones personalizadas, y las usa **hoy** en un correo real que tiene pendiente. Cronometra
  antes y después. Sale de la sesión con tiempo ahorrado, con el primer dato del diagnóstico y con la
  primera lección de datos, todo a la vez, sin instalar nada y sin hablar con nadie. **El mapa del
  curso va después de este resultado, nunca antes.**
- **Sesión 2 — El diagnóstico** (Fase 1 de E-01: las siete comprobaciones que hace sola) **+ los
  correos ya redactados** para administración y para quien administre Workspace. El material se los
  da literales para copiar y pegar: redactarlos desde cero es una barrera absurda.
- **Sesión 3 — El semáforo** sobre sus 10 últimos correos reales (E-02), con su trampa deliberada:
  la mayoría quita el nombre y cree que ya está. La rúbrica no lo corrige; se corrige en el M2.
- **Bloque de proyecto — El inventario y la elección**, con la línea base arrancada.

> **Nota de diseño sobre la espera.** El correo al administrador puede no contestarse nunca. El curso
> **no puede bloquearse ahí**: la Vía B es el diagnóstico empírico de cinco comprobaciones
> (`dominio-herramientas.md` §1.6) que infiere el plan desde lo que ve en pantalla. Y tiene una virtud
> extra: es literalmente operacionalizar un constructo en indicadores observables, que es su casa.

---

### 3.3 M1 · Escribir el criterio antes que el prompt

| | |
|---|---|
| **Cambio mental** | Dos, y son los dos más caros del curso. (1) *"El cuello de botella no es el prompt: es que nadie ha escrito qué cuenta como respuesta correcta."* (2) **Validez aparente**: *"un modelo de lenguaje es el instrumento con la validez aparente más alta y la garantía de contenido más baja que vas a manejar en tu vida — está literalmente optimizado para producir texto plausible"*. Esa segunda no la tiene que creer por autoridad: la deduce de algo que ya sabe |
| **Qué construye** | (1) la **ficha de criterio** (EP-01) de su tarea; (2) las **anclas de tono** (EP-02), que no son un calentamiento: son el fichero de contexto del M2; (3) los **10 casos apartados antes de escribir nada** (EP-06); (4) la **batería** con tabla de especificaciones (EP-03); (5) **la primera columna de la hoja de anclas**: la batería pasada contra su chat de hoy, con fecha |
| **Duración** | 2 semanas |
| **Herramienta y por qué** | **Ninguna nueva, deliberadamente.** Un documento. Es el módulo que más se parece a "deberes" y por eso su sesión 1 empieza pasando la batería contra el chat actual y viendo cómo saca 4/10: la ficha de criterio nace como respuesta a un fallo observado, no como tarea previa |
| **Cómo se autocorrige** | (a) **Rúbrica negativa** de EP-01: prohibidas las palabras *adecuado, correcto, natural, profesional, de calidad* sin ancla; cada indicador tiene que contestarse sí/no mirando la salida y una fuente; al menos uno verificable contra fuente externa; si todos son críticos, no ha priorizado. (b) **Prueba mecánica**: la ficha cabe en una cara — una rúbrica de dos páginas no se usa nunca. (c) EP-06 tiene una autocorrección contraintuitiva y valiosa: *si al abrir los diez apartados no falla ninguno, sospecha del muestreo antes que celebrar*. (d) La batería contra el chat de hoy es **comprobación pura**: sale o no sale |

---

### 3.4 M2 · Un asistente que ya sabe dónde trabajas

| | |
|---|---|
| **Cambio mental** | *"La memoria fiable es un fichero, no una sensación."* Y la tríada que los principiantes mezclan siempre: **fuente de verdad** (hechos, desde una sola dirección) ≠ **memoria** (acuerdos que permanecen) ≠ **procedimiento** (pasos y formato). Un Gem recuerda sus instrucciones; **no recuerda lo que pasó ayer** |
| **Qué construye** | (1) un **Gem** con instrucciones y hasta 10 ficheros de conocimiento [V], alimentado con la ficha de criterio y las anclas de tono del M1; (2) un **cuaderno de Gemini Notebook** con las fuentes de verdad de su puesto —tarifario, calendario académico, condiciones generales, FAQ de visados— **con fecha de última revisión en cada fuente**; (3) la regla de **"no lo sé"** y de **cita del documento** |
| **Duración** | 2 semanas |
| **Herramienta y por qué** | Gems + Gemini Notebook. Incluidos en el plan de su empresa desde Business Standard [V], cero coste, cero instalación. Y el motivo decisivo, que no es pedagógico sino de producto: **Workspace Studio los consume literalmente como pasos** (`Ask a Gem`, `Ask Gemini Notebook`), así que lo que construye aquí se reutiliza tal cual en el M4 |
| **Cómo se autocorrige** | **Cuatro capas, en orden de fiabilidad decreciente.** (a) **La batería del M1, otra vez, columna nueva con fecha** — comprobación, no juicio. Umbral: 5/5 normales; en los 3 límite **pide aclaración** (inventar una decisión es fallo aunque acierte); en los 2 de rechazo dice **"no lo sé"**. (b) **Lista de comprobación binaria** de 10 ítems observables: *¿cada fuente del cuaderno tiene fecha? SÍ/NO · ¿hay una frase que diga qué hacer cuando falta un dato? SÍ/NO · ¿alguna respuesta cita un documento que no está en las fuentes? SÍ/NO*. (c) **El cebo del escalón 1** (control positivo): el curso trae un Gem de mentira con **tres defectos plantados y documentados** —uno visible, uno de omisión, uno de criterio—; ella lo pasa por el protocolo de corrección con IA y después abre la hoja de defectos y cuenta. Si encuentra 1 o 0, **ese tipo de trabajo no se corrige con IA en el resto del curso**. (d) **El protocolo de siete reglas** para corregir con IA: hilo nuevo · no digas que es tuyo · nunca "¿está bien?" sino "cita el fragmento que incumple" · pega la rúbrica · **no discutas en el mismo hilo** · dos modelos para detectar desacuerdo, no para dirimirlo · su veredicto no cierra nada |

> **Por qué el cebo va aquí y no más tarde.** Es el ejercicio de mayor apalancamiento de todo el curso
> [`dominio-autodidacta.md` §3.5.3]: audita el instrumento que va a usar cincuenta veces después. Y es
> psicometría —control positivo— con otro nombre, así que lo reconoce al instante.

---

### 3.5 M3 · La primera vez que pasa algo sin ti

| | |
|---|---|
| **Cambio mental** | *"Automatizar no es una herramienta nueva. Es quitar el dedo del disparador."* Y el corolario que la escalera hace visible: **subir de escalón no mejora la respuesta; cambia quién la pide y cuántas veces** |
| **Qué construye** | (1) una **acción programada** en Gemini —un resumen semanal, un recordatorio—; (2) la **columna `=AI()`** en la hoja de respuestas de la encuesta, con el **libro de códigos** de EP-10 pegado dentro como instrucción. Aquí arranca de verdad el hilo guiado (P27) |
| **Duración** | 2 semanas |
| **Herramienta y por qué** | Acciones programadas + `=AI()` en Sheets. Es automatización real **sin salir de lo que ya tiene**, sin instalar, sin permisos y sin cuenta nueva. Y ataca el proceso que `dominio-academia.md`, `dominio-rgpd.md`, `dominio-herramientas.md` y `dominio-psicologia.md` señalan por caminos independientes como el mejor primer proyecto: **P27, riesgo bajo, volumen alto, multilingüe, y hoy no se hace** |
| **Contingencia obligatoria** | Si su plan es **Business Starter**, `=AI()` no existe [V]. El material trae la ruta alternativa por delante (el mismo libro de códigos dentro de un Gem, pegando la columna en bloques). **Aquí se cobra el diagnóstico del M0**, y se dice así: no es un fallo suyo ni del curso |
| **Cómo se autocorrige** | **Doble codificación (EP-07), que es comprobación pura.** Clasifica ella 30 comentarios **antes** de ver la salida del sistema; después compara; construye la **tabla de confusión**; escribe una frase por cada confusión repetida; y mira el acuerdo de la **categoría menos frecuente por separado** —porque si el 60 % son de alojamiento, un clasificador que dijera "alojamiento" siempre acertaría el 60 %. Autocorrección adicional del libro de códigos: al aplicarlo cerrado a 40 comentarios nuevos, **menos del 15 % debe caer en "otros"**; si cae 0 %, sospechar de encajes forzados |
| **Satélite** | **P02, el presupuesto.** Es aritmética sobre una tabla de precios. Respuesta correcta: **escalón −1**. Es el ejemplo canónico del árbol de decisión y hay que usarlo tal cual |

---

### 3.6 M4 · Del artefacto al disparador

| | |
|---|---|
| **Cambio mental** | *"Un flujo no piensa: ejecuta el camino que tú decidiste. Su virtud es que es aburrido y predecible — y eso, en atención al cliente, es una virtud, no una limitación."* |
| **Qué construye** | El **flujo A** del hilo guiado: disparador *cuando llega una respuesta de Forms* → `Extract` (idioma y tema) → `Ask a Gem` (**el suyo, del M2**) → `Check if` (¿negativo y grave?) → `Add a row` + `Notify me in Chat` sólo si es grave |
| **Duración** | 2 semanas |
| **Herramienta y por qué** | **Google Workspace Studio.** Cuatro razones en orden de peso [`dominio-herramientas.md` §3.2]: coste marginal cero y fricción de alta cero · continuidad literal con el escalón 1 · **los datos no salen del tenant de la empresa**, mientras que conectar Make o Zapier al buzón de una academia mete un proveedor más en la cadena de pasaportes y alojamientos de menores · su empresa vive en Google. Y **una sola página** —no un módulo— sobre Make, n8n, Zapier y Power Automate, con el criterio que sobrevive al producto: *automatiza donde ya viven tus datos*, y **cuándo Studio deja de ser la respuesta correcta**: cuando el flujo tenga que tocar algo que no está en Workspace (el software de gestión académica, la pasarela de pago, WhatsApp Business, el portal de una agencia) |
| **Los límites, por delante y no por sorpresa** | Va en la primera página del módulo, no en la de erratas: **los flujos fallan con unidades compartidas, carpetas compartidas y hojas con `IMPORTRANGE`** [V]; un solo disparador por flujo; sólo se muestran 50 etiquetas de Gmail. Como el centro de gravedad de su puesto **es un buzón compartido** (`info@`, `accommodation@`) y una hoja de camas compartida, los primeros flujos se construyen sobre **su propio buzón y sus propias copias**. Descubrir esto en la lección 1 en vez de en el tercer intento fallido es lo que separa un material honesto de uno que la frustra |
| **Cómo se autocorrige** | (a) **Ejecución real**: se dispara o no se dispara. Es el corrector más fiable que existe y es gratis. (b) **La batería, otra vez, columna nueva con fecha** — y aquí la lectura correcta es la contraintuitiva: *si la calidad ha mejorado respecto al M2, sospecha: probablemente reescribiste el criterio por el camino, y eso no es mérito del flujo*. (c) **Lista de comprobación de plataforma** de 8 ítems binarios, que además sirve de diagnóstico cuando algo falla: *¿el fichero es mío y no está en una unidad compartida? SÍ/NO*… |

---

### 3.7 M5 · Prepara, no envíes

| | |
|---|---|
| **Cambio mental** | *"Automatiza la lectura y la preparación; la escritura hacia fuera la firma una persona."* Y la razón, que no es prudencia sino diseño de aprendizaje: **si el artefacto sólo prepara, todos sus errores son recuperables, y por eso puedes permitirte equivocarte mucho — que es lo que hace falta para aprender.** Un curso construido sobre artefactos que envían no puede |
| **Qué construye** | El **flujo B, del hilo propio**: triaje del correo entrante (clasificar y etiquetar, **no responder a nadie**) o borradores para P01 con `Ask Gemini Notebook` y bifurcación *si no encuentra fuente → etiqueta "responder a mano"*. Más: la **lista de temas prohibidos** (E-06), las **condiciones de parada**, el **tope de volumen** (*si la lista supera N, no redactes nada y avísame*) y **cómo se apaga, probado de verdad** |
| **Duración** | 2 semanas |
| **Herramienta** | Ninguna nueva. Es el módulo donde el escalón 2 se profundiza en vez de ensancharse |
| **Cómo se autocorrige** | (a) **Rúbrica con criterios negativos**, cada uno con salida escrita obligatoria y sin "no aplica": *¿existe un caso en el que el flujo siga adelante sin un dato que necesita? Nómbralo o declara que has buscado y no existe* · *¿hay algún paso que salga hacia fuera sin que yo apruebe?* · *¿hay algún dato aquí dentro que, si se filtrara mañana, tendría que comunicar a alguien?*. (b) **Prueba del apagado**: se apaga de verdad, no se imagina. Un sistema que no sabes apagar no está terminado. (c) **Prueba ciega (EP-08)**, el ejercicio con mejor relación valor/esfuerzo del curso: 5 respuestas suyas de hace meses + 10 borradores del sistema, sin marcas de origen, **barajadas por otra persona**, puntuadas con la ficha del M1. Desactiva de golpe fluidez, halo y sesgo del experimentador |
| **Comprobación de rúbrica que decide el módulo** | *La respuesta a "¿quién revisa antes de que salga?" es **una persona con nombre**. Si no hay nombre, no hay revisión.* Y: *si tu diseño permite que algo llegue a un cliente sin que alguien le dé a enviar, vuelve al principio* |

---

### 3.8 M6 · ¿Esto sirve de verdad?

| | |
|---|---|
| **Cambio mental** | *"Que el flujo se ejecute cada lunes no es que funcione."* **Evaluación de proceso ≠ evaluación de resultado.** Un flujo puede ejecutarse impecablemente y no cambiar nada, porque el informe que produce no lo lee nadie o porque los borradores se reescriben siempre |
| **Qué construye** | (1) **El vigilante de plantillas (P32)**: un flujo programado que compara el tarifario maestro con las plantillas de cada idioma y crea una tarea con las discrepancias. Ataca el riesgo *"alto y silencioso"* del inventario —la versión alemana lleva meses mandando el precio del año pasado y nadie se entera hasta que un cliente lo reclama—. (2) La **media página de evaluación** por sistema (EP-09): línea base vs. después, **por unidad de trabajo** y no por semana, con el coste completo restado (montaje + revisión + mantenimiento). (3) La **cadena causal en cinco flechas** (EP-14) con el eslabón subrayado que no depende de ella. (4) **La lista de lo que ha decidido NO automatizar, con el motivo** |
| **Duración** | 2 semanas |
| **Herramienta** | Ninguna nueva. Una hoja de cálculo. A propósito |
| **Por qué el vigilante va aquí** | Porque este módulo cae exactamente en la frontera de abandono 2→3 (§9) y no puede ser un módulo sin producto visible. El vigilante produce **una lista de errores reales que nadie sabía que existían**: es el artefacto de mayor retorno visible de todo el curso y por eso se coloca en el punto donde el material solo ya no tira |
| **Cómo se autocorrige** | (a) La comparación con la línea base del M0 es **aritmética**, no juicio. (b) Rúbrica con tres prohibiciones duras: **prohibida la palabra "significativo"** (no se está estimando un parámetro de una población: es evaluación criterial, no inferencial); **obligatorio restar** el tiempo de revisión y mantenimiento; **obligatorio nombrar una amenaza a la validez interna que no puede descartar** —historia (septiembre no es julio), maduración, regresión a la media (eligió el proceso que más duele, y lo que más duele suele medirse en su peor semana), instrumentación, reactividad de la medida, atrición—. (c) Cláusula explícita: **si el saldo es negativo y aun así quiere conservarlo por otra razón (menos errores, menos carga mental, respuesta más rápida al cliente), es legítimo — pero entonces mide esa otra razón y di que el ahorro de tiempo no era el objetivo**. (d) La rúbrica de la lista de descartes declara: **un módulo en el que todo acaba automatizado está mal resuelto** |

---

### 3.9 M7 · Juicio dentro del flujo — y por qué no un agente

| | |
|---|---|
| **Cambio mental** | Dos. (1) *"Un agente no es una automatización mejor: es una automatización que **ha renunciado a ser predecible** a cambio de poder afrontar casos que no previste. Esa renuncia se paga, y en atención al cliente hay que pagarla a conciencia y sólo donde compensa."* (2) **El riesgo no es el del día 1, es el del día 60**: sesgo de automatización. A la tercera semana se deja de revisar. *La confianza no es una salvaguarda* |
| **Qué construye** | (1) Un flujo que **se bifurca según un criterio que ella ha definido y sabe justificar** (`Decide`, `Extract`), con reglas de escalado. (2) El fichero **Mapa de lo que existe**, escrito por ella (ver §5). (3) **La rúbrica de su propio artefacto**, redactada por ella — el desvanecimiento completo del andamiaje |
| **Duración** | **3 semanas**, no 2. Es la frontera de abandono y se le da aire |
| **Herramienta y por qué** | Los pasos de IA de Workspace Studio. Nada nuevo instalado. Y la conclusión honesta que hay que decir sin disculparse: **el escalón 3 en su caso es "un flujo con juicio en dos o tres puntos concretos", no "un agente autónomo que gestiona el buzón"**. La barrera no es técnica ni de capacidad: es de **licencia** (Spark, Mariner y auto-browse están detrás de AI Ultra o de Gemini Enterprise [V]), de **permisos** (un agente útil necesitaría el buzón compartido y la hoja de camas, que es justo lo que Studio no soporta) y de **datos** (sus procesos de más volumen mezclan salud, religión, menores y documentación de identidad) |
| **Cómo se autocorrige** | (a) **La batería, última columna**, ahora con **casos límite nuevos escritos por ella**. (b) **La rúbrica la escribe ella**; el curso sólo trae la lista de comprobación *de la rúbrica*: ¿tiene al menos 3 criterios negativos? ¿cada uno exige una salida escrita, sin "no aplica"? ¿hay un umbral de "listo" formulado como condiciones de fallo? (c) **Lectura de la hoja de anclas completa**: una frase escrita por columna diciendo qué aportó ese escalón. Si no puede escribir esa frase para alguna columna, ese escalón no le aportó nada y merece la pena saberlo |

---

### 3.10 M8 · Cerrar y dejarlo vivo · M9 · (opcional) Lo que hay más arriba

**M8 (semana 18).** Cambio mental: *"esto no termina cuando se acaba el material; termina cuando tú
escribes los criterios y sabes cuándo hay que volver a mirar."* Construye el **cuaderno de
mantenimiento**: qué se revisa, cada cuánto y quién; la hoja de anclas con su próxima fecha de pasada;
su versión de la página *"Cuando no coincide"*; y las tres cosas siguientes **con su condición de
disparo** (*"haré X cuando ocurra Y"*), no con una fecha. Autocorrección: la definición de "terminado"
fijada en la semana 1 y observable — **tres artefactos vivos que usa sin que el curso se lo pida, más
una rúbrica escrita por ella**.

**M9 (opcional, una lección, sin entregable).** Claude Code, Claude Cowork, Antigravity: qué son,
cuándo ganan de verdad (procesar decenas de ficheros locales de forma repetida — revisar 200 contratos
de estancia larga buscando cláusulas), y por qué hoy no. **Si termina el curso sin abrirlo, el curso ha
funcionado igual**, y eso va escrito en la primera línea del módulo.

---

## 4. LOS PUNTOS DE CONSULTA CON SU PAREJA

### 4.1 El principio, antes de la lista

El recurso es **escaso, no renovable y con coste relacional**. Un mentor pagado se gasta sin culpa;
una pareja, no. **Presupuesto: 6 consultas de 10 minutos en todo el curso** — una hora repartida en
cuatro meses. Un curso que reserve "consultas ilimitadas" obtiene en la práctica cero, porque cada
consulta compite con la comodidad de no molestar y pierde. Un curso que reserve exactamente seis, con
nombre y momento, obtiene seis.

**Filtro de admisión, impreso en la portada de la bitácora.** Si falla cualquiera de las cuatro, no es
punto de consulta: (1) ¿lo resuelve el material? (2) ¿lo resuelve la IA con el protocolo de siete
reglas? (3) ¿lo resuelve **mirar** —su pantalla, su consola, preguntar a su administrador—? (4) ¿lo he
intentado 25 minutos y he anotado lo que he probado?

**Ficha de cinco campos escrita ANTES**, máximo una cara: la pregunta en una frase **cerrada** · mi
hipótesis y qué esperaría ver si tengo razón · qué he probado ya y qué pasó · **el dato concreto**
(mensaje de error literal, las dos respuestas que se contradicen) · qué haré con cada respuesta
posible. Reglas de la conversación: **los cinco primeros minutos sin pantalla** · **él no toca el
ratón** · sale con una frase escrita en su propio lenguaje · **a los diez minutos se para, esté como
esté**.

### 4.2 Dónde caen, y por qué exactamente ahí

| # | Momento | Qué lleva | Por qué ahí y no en otro sitio |
|---|---|---|---|
| **PC-1** | **Fin del M0** (sem. 2) | *"He deducido que tenemos X y que por tanto no puedo hacer Y. ¿Me equivoco?"* Con las cinco comprobaciones empíricas hechas y las capturas | Es **un hecho del mundo que el material no puede ver**, y un error aquí contamina el curso entero: si el plan es Starter, media escalera cambia. Mejor relación consecuencia/coste de los seis |
| **PC-2** | **Inicio del M2** (sem. 5), justo antes de cargar fuentes reales en el cuaderno | Su clasificación de **8 tipos de dato reales** de su puesto en tres cajones: cuenta de empresa / nunca / depende. Él sólo dice de acuerdo o no, y por qué | **Es la única decisión del curso con consecuencia externa irreversible.** Y el momento es exacto: es cuando pasa de *pegar texto* a *subir ficheros*, que es donde cambia el orden de magnitud del riesgo |
| **PC-3** | **Fin del M2** (sem. 6), tras el cebo | *"Esta es la corrección que me hizo la IA de un trabajo con tres fallos plantados. Encontró dos. ¿Estoy leyendo bien lo que se le escapa?"* | **El de mayor apalancamiento.** No se revisa su trabajo: se revisa **su instrumento de corrección**, que va a usar cincuenta veces más. Diez minutos aquí valen por todas las correcciones posteriores |
| **PC-4** | **Comodín**, disponible desde el M4 | Un fallo de plataforma tras agotar la lista de comprobación y la página *"Cuando no coincide"* | Caso canónico de "diez minutos ahorran una tarde". **No tiene fecha a propósito**: saber que existe un comodín reduce el miedo a atascarse, que es un factor de abandono por sí mismo, aunque no se use |
| **PC-5** | **Frontera M6→M7** (sem. 14) | *"Esta es la frontera que he trazado entre lo que automatizo y lo que no. Aquí están los tres casos donde he dudado. ¿Dónde la moverías?"* | Juicio de escala y oportunidad: el modelo, preguntado, dirá que sí a automatizar, porque preguntar a un sistema si hay que hacer algo tiene un sesgo obvio hacia el sí. Y requiere que ya tenga dos flujos vivos: antes no hay sustancia sobre la que conversar |
| **PC-6** | **M8** (sem. 18) | *"Esto es lo que tengo funcionando. ¿Qué es lo siguiente que tendría sentido, y qué tendría que cambiar para que mereciera la pena?"* | Cierra con una orientación que no puede darse sola, y evita el "final sin final" |

**Sobre la concentración de PC-1, PC-2 y PC-3 en las seis primeras semanas** —tres de seis en un
tercio del curso—: es deliberado y tiene dos justificaciones independientes. La primera es de
consecuencia: los tres cubren un hecho del mundo que contamina todo, la única decisión irreversible, y
la calibración del instrumento que se usará después. La segunda es de abandono: **las dos primeras
semanas valen más que las diez siguientes juntas** [E], y que otra persona esté implicada temprano es
en sí mismo un mecanismo de permanencia.

**No es punto de consulta, y se escribe para que no se erosione:** revisar un entregable (*"¿está bien
mi Gem?"* → rúbrica + batería), explicar un concepto (*"¿qué es MCP?"* → material), enseñarle a hacer
algo (→ documentación), ni dar ánimos. Y la tentación específica de esta configuración: **que él le
monte algo "que es un momento"**. Eso no es una consulta: es un artefacto que ella no sabrá mantener
ni depurar, y en el escalón siguiente será deuda.

**Cada punto lleva su alternativa degradada escrita justo debajo**, porque el material no puede tener
un paso bloqueante que dependa de otra persona: PC-1 → asumir el escenario más restrictivo (Starter) y
anotar la suposición · PC-2 → regla de máxima cautela, *si dudas, no lo metes* · PC-3 → hacer el cebo
con dos modelos y comparar · PC-4 → documentar el fallo, **rodearlo** con una solución manual y seguir
· PC-5 → la lista de descalificadores por número de proceso · PC-6 → la tabla de escalones.

**Un uso de otra persona que NO gasta punto:** barajar las respuestas de la prueba ciega del M5 y
guardar la clave. Es una función mecánica de cinco minutos, no una consulta, y vale cualquier
compañera de la academia.

---

## 5. CÓMO SE CUBRE "SABER QUÉ EXISTE" SIN CONVERTIRLO EN CATÁLOGO MUERTO

Es el objetivo 1 del brief y el más fácil de resolver mal: un módulo llamado "panorama de la IA" que
se lee una vez, se olvida en dos semanas y caduca en seis meses.

**El principio: el catálogo se construye por descarte documentado, no por enumeración.**

Existe **un único fichero vivo**, `mapa-de-lo-que-existe.md`, con tres columnas. No se lee: **se
rellena**, una fila cada vez que una tecnología aparece por ser relevante para una decisión suya.

| Qué es, en una frase mía | Por qué hoy no me toca | Qué tendría que pasar para que me tocara |
|---|---|---|
| *Automatización tipo Make / Zapier: un servicio de fuera que conecta aplicaciones entre sí* | Studio hace lo mismo dentro de mi Workspace, gratis, y sin meter otro proveedor entre mis datos y yo | Que necesite tocar el software de gestión académica, la pasarela de pago o WhatsApp Business, que están fuera de Workspace |
| *Agente: le das el objetivo y los límites, y él decide los pasos sobre la marcha* | Los de verdad están detrás de AI Ultra o Gemini Enterprise, y mi trabajo vive en un buzón compartido que Studio no puede tocar | Que la empresa contrate Gemini Enterprise, o que aparezca una tarea cuyos pasos no pueda dibujar de antemano |
| *MCP: el estándar por el que un modelo se conecta a una herramienta o una fuente* | Para mí hoy es vocabulario, no herramienta. Lo que sí me sirve es el principio que hay detrás: conectar sólo a lo necesario | Que monte algo fuera de Workspace, o que alguien técnico lo configure y yo sólo lo use |
| *Apps Script: escribir un programa dentro de Google, con Gemini ayudando* | Es código JavaScript aunque lo escriba Gemini, y el día que falle hay que leer un error de programador. Studio me lo ahorra | Que Studio se quede corto en algo concreto **y** haya alguien que pueda mantener el script |
| *Google AI Studio: el sitio donde se prueban prompts con la API* | Sus propios términos dicen literalmente que no metas información personal, y se entra con la cuenta de Google, así que **parece** seguro y no lo es | Nada de mi trabajo. Es una superficie de desarrollador |
| *Claude Code / Cowork / Antigravity* | No resuelve mejor ninguno de mis 32 procesos, está fuera del estándar de mi empresa y sale de mi bolsillo | Una tarea que exija procesar decenas de ficheros locales de forma repetida |
| *Bases de conocimiento con RAG y grafos* | Un cuaderno con 20 fuentes bien fechadas me da lo mismo con mucho menos aparato | Que las fuentes pasen de decenas a cientos y el cuaderno empiece a perderse |

**Cuatro propiedades que hacen que esto no muera:**

1. **La tercera columna es la que convierte el catálogo en criterio.** Un catálogo dice qué hay; esta
   columna dice **bajo qué condición cambiaría mi decisión**. Es lo que sobrevive a que cambien los
   nombres, porque las condiciones no cambian: *"tocar algo fuera de Workspace"* seguirá siendo verdad
   cuando Studio se llame otra cosa.
2. **Cada fila se escribe en el momento en que se toma la decisión que la descarta**, no en un módulo
   de panorama. La fila de "agente" se escribe en el M7, cuando ya tiene un flujo con juicio y
   entiende exactamente qué le falta.
3. **La escribe ella, en su lenguaje.** Un fichero copiado no se relee; uno escrito, sí. Y es un
   entregable evaluable: la lista de comprobación pregunta *¿hay alguna fila cuya tercera columna esté
   vacía? SÍ/NO* — una condición vacía significa que el descarte fue por desgana y no por criterio.
4. **Los casos satélite fuerzan encuentros con opciones que no son las suyas**, así que el mapa no se
   queda en las cuatro cosas que su hilo necesitó.

**Lo que además evita:** el miedo documentado del principiante —*"¿me estás obligando a casarme con un
programa que no conozco?"* [fuente-qa, P2, P16, P19]—. Un mapa donde cada herramienta tiene su
condición de entrada y de salida es exactamente la vacuna contra ese miedo.

---

## 6. CÓMO SE ENSEÑA A NO USAR IA CUANDO NO TOCA

Seis mecanismos, de más estructural a más operativo. Ninguno es una advertencia suelta.

**1 · El escalón −1 existe en el árbol de decisión, con su ejemplo canónico de su casa.**
Antes de preguntar "¿chat, automatización o agente?" hay una pregunta anterior: **"¿esto necesita un
modelo de lenguaje?"**. Si la tarea tiene pasos fijos y datos estructurados, la respuesta es no.
**P02, el presupuesto**, es aritmética sobre una tabla de precios: número de semanas × tipo de curso ×
alojamiento × suplemento de julio-agosto × descuento por volumen. Eso no es un prompt, es una fórmula.
Y **P22, la hoja de camas**, es un calendario de recursos. Es el satélite obligatorio del M3, y es el
ejemplo con el que el árbol de la referencia corta en la dirección que casi nadie enseña.

**2 · Cada escalón tiene su sección "cuándo NO subir", con el mismo peso tipográfico que el resto.**
No subir del chat al Gem si la tarea la hace tres veces al año. No subir del Gem al flujo si aún no
usa el Gem espontáneamente (**puerta 1→1,5**). No subir del flujo al juicio si el camino siempre es el
mismo: meterle juicio a un proceso determinista lo hace más caro, más lento y menos auditable.

**3 · Las zonas prohibidas, con el motivo y no sólo la prohibición.**
Porque una prohibición sin motivo no se transfiere a un caso nuevo:

| Proceso | Por qué no, dicho de forma transferible |
|---|---|
| **P08** carta de aceptación para visado | Riesgo crítico y **normativa viva**: el RD 1155/2024 y la Instrucción SEM 3/2025 reordenaron la estancia por estudios y esto cambia de un año para otro. **Congelar dentro de un prompt un conocimiento que caduca es fabricar un error futuro** |
| **P26** quejas formales | Una respuesta que **admite responsabilidad por escrito compromete a la empresa**. Y los modelos son complacientes: la complacencia por escrito, en una queja, es exposición legal |
| **P29** emergencias 24 h | Personas, menores, responsabilidad civil, y un alumno en shock con nivel A1 |
| **P25** reembolsos | Datos bancarios y riesgo de fraude por suplantación en el cambio de cuenta |
| **P17** matching con familia de acogida | Concentra **salud, religión y potencialmente orientación sexual** en una casilla de texto libre. Es el proceso que **más parece** el caso ideal de IA y por eso es la trampa |
| **P05 / P16** nivelación y exámenes | Anexo III del Reglamento de IA: *evaluar el nivel educativo* es alto riesgo. Aplazado al 02.12.2027, **no cancelado**. Lo suyo no es decidirlo **[!]**, es reconocerlo y avisar |

Y la regla de oro que hace todo esto memorable: **de todo su proceso, el único trocito que está en la
lista de alto riesgo es el que decide el nivel de un alumno. Todo lo demás —redactar, traducir,
resumir, clasificar— no lo está.** Esa asimetría se recuerda; una lista de artículos, no.

**4 · El coste completo como criterio de descarte, no como cálculo de justificación.**
En el M6: *un flujo que ahorra ocho minutos y cuesta diez de revisión es una pérdida disfrazada de
modernidad*. Y la métrica de vanidad tiene nombre: **que el flujo se ejecute cada lunes no es que
funcione**.

**5 · La opción segura suele ser también la más eficiente, y eso hay que demostrarlo.**
El mejor ejemplo, y va en el M2: **no transcribas la llamada.** Escribe tú un resumen de cuatro líneas
al colgar, ya seudonimizado, y trabaja con ese resumen. Es más rápido que subir un audio de doce
minutos, no genera un tratamiento nuevo ni un destinatario nuevo, y de paso piensas el caso. Enseñado
así, "no usar IA" deja de ser una renuncia y pasa a ser una decisión de eficiencia.

**6 · Se evalúa.** La lista de descartes del M6 es un entregable con rúbrica, y la rúbrica dice que un
módulo donde todo acaba automatizado está mal resuelto. Si no se puntúa, no se hace.

---

## 7. PROTECCIÓN DE DATOS: DÓNDE VA Y POR QUÉ AHÍ

**Principio de diseño: esto no es un módulo.** Un módulo de protección de datos se lee una vez, se
aprueba y se olvida — y además produce parálisis, cuando el objetivo es que **use más la IA, no menos:
que la use en el sitio correcto**. Va repartido en **tres capas**, y cada una aparece en el momento en
que **desbloquea** lo siguiente en vez de frenarlo.

| Capa | Dónde | Qué contiene | **Por qué exactamente ahí** |
|---|---|---|---|
| **Capa 1 — Qué tengo y qué no se pega** | **M0, sesiones 1–3** | Cuenta de empresa vs. personal; el distintivo de la pantalla; edición, licencia y retención; el **semáforo** verde/ámbar/rojo; el argumento de la cuenta personal | **Es la semana en la que va a empezar a pegar cosas.** Todo lo demás se construiría sobre un suelo que no ha mirado. Y el diagnóstico es útil por partida doble: de la edición depende también **qué funciones existen** |
| **Capa 2 — Seudonimizar de verdad y adjuntos** | **M2, antes de cargar las fuentes** | Por qué "quitar el nombre" no basta; cuasi-identificadores; la **prueba de la compañera**; los adjuntos (el Excel va **completo**, con las hojas ocultas; el PDF del pasaporte va entero; las fotos llevan GPS); *si no lo has abierto y leído entero, no lo adjuntas* | **Es el momento exacto en que pasa de pegar texto a subir ficheros.** Al pegar ves lo que envías; al adjuntar, no. Ese salto es donde cambia el orden de magnitud del riesgo, y por eso la capa va pegada a él y no dos módulos antes ni dos después |
| **Capa 3 — Salvaguardas de un sistema que actúa** | **M5, antes del segundo flujo** | Lista de temas prohibidos; condiciones de parada; *nada sale al cliente sin que un humano le dé a enviar*; el **art. 50** (avisar de que es una IA, en vigor desde el 02.08.2026); registro de qué se generó y quién lo aprobó; el plan para el día que falle, incluido **valorar si hay brecha [!]** | **Es cuando algo empieza a actuar sin que ella mire cada paso.** Antes del M5 no hacía falta; después del M5 sería tarde |

**Capa 0, permanente:** la **tarjeta del lunes** impresa al lado de la pantalla desde la semana 1, con
seis preguntas que caben en una nota adhesiva y que sobreviven a un martes de julio con 300 correos
sin abrir. Si una regla necesita que te pares a pensar, no sobrevive a julio.

**Cuatro decisiones de diseño que hacen que esto funcione y no asuste:**

1. **La regla de los menores es tajante y sin excepciones**, más restrictiva de lo que la norma exige
   en todos los supuestos, **a propósito**: *si hay un menor implicado, sus datos no entran en ninguna
   herramienta de IA, ni seudonimizados*. Una regla con excepciones no sobrevive a julio.
2. **Cada decisión que no es suya va marcada [!] y con el nombre de a quién se escala.** El riesgo
   específico de este perfil es que, por ser la que más se preocupa, acabe siendo de facto la
   responsable de cumplimiento de la academia. El material lo prohíbe explícitamente.
3. **Nada normativo se congela dentro de un prompt.** Las fechas del Reglamento de IA, el estado del
   DPF y la ley española viven en un fichero de contexto **con fecha visible** que se revisa. Y eso es
   además el mejor ejemplo pedagógico del curso de la diferencia entre conocimiento estable y
   conocimiento volátil.
4. **El encuadre no es de permiso, es de aportación.** No está pidiendo autorización para nada: ya usa
   Gemini, se lo ha dado su empresa, y usarlo está bien visto. Está entendiendo la configuración antes
   de apoyarse en ella. Si la academia nunca se lo ha planteado, **acaba siendo ella quien propone la
   política**, que es el mejor resultado posible — y no es venta interna: es su propio trabajo.

**Y el dato que cambia la posición mental con la que se estudia esto, y que merece salir en la primera
página:** el artículo 4 del Reglamento de IA, en vigor desde febrero de 2025, obliga a las empresas
que usan IA a garantizar un nivel suficiente de **alfabetización en IA** de su personal. Dicho de otro
modo: **el curso que está haciendo es, técnicamente, cumplimiento normativo de su empresa.**

---

## 8. QUÉ SE QUEDA FUERA A PROPÓSITO

### 8.1 Fuera porque el brief lo excluye

| Fuera | Por qué |
|---|---|
| **Venta interna: "cómo conseguir el sí"** | En su empresa usar IA ya está bien visto y **lo mal visto es no automatizar**. Un módulo de venta interna resuelve un problema que ella no tiene, y le roba semanas a los que sí tiene |
| **Portfolio y landing page** | Es el destino del itinerario no técnico de la referencia (5A.3, 5A.4) porque **su alumno tipo quiere cambiar de sector**. La nuestra no. Aquí es ruido |
| **Certificado, insignia, "ahora eres AI Operator"** | No busca cambiar de rol. Y un certificado sin evaluador ni rúbrica no certifica nada |
| **Cualquier cosa vistosa** | El **grafo de Obsidian** de la referencia es el caso de estudio: espectacular en pantalla, marginal en valor para un puesto de atención al cliente. El artefacto útil aquí es mucho más aburrido: una base de respuestas con fuente y fecha, un triador, un vigilante de plantillas |
| **Construir y vender aplicaciones** | Ni siquiera la referencia lo promete, y con razón |

### 8.2 Fuera por criterio de escalera, con su condición de reentrada

| Fuera | Reducido a | Condición para que entre |
|---|---|---|
| **n8n, Make, Zapier, Power Automate** como módulos | **Una página** comparativa + el criterio *automatiza donde ya viven tus datos* | Que un flujo tenga que tocar algo fuera de Workspace. Entonces **Make** es la siguiente parada; **n8n sólo si aparece alguien técnico que lo mantenga**; Power Automate nunca, es el ecosistema equivocado |
| **Apps Script** | **Media página** informativa | Que Studio se quede corto **y** haya quien mantenga el script |
| **Google AI Studio** | **Cinco líneas, con aviso explícito** | Ninguna. Es la trampa más silenciosa del panorama: es de Google, parece profesional, se entra con la cuenta de Google, es gratis, y sus términos dicen literalmente que no metas información personal |
| **MCP y conectores** como práctica | **Vocabulario + el principio de privilegio mínimo** | Que monte algo fuera de Workspace o que alguien se lo configure |
| **RAG, grafos, arquitecturas de base de conocimiento** | **Una fila del mapa** | Que las fuentes pasen de decenas a cientos |
| **Claude Code / Cowork / Antigravity** | **M9, una lección, opcional, sin entregable** | Una tarea con decenas de ficheros locales repetida en el tiempo |
| **Agentes de navegador, Spark, Mariner** | **Una fila del mapa** | Un cambio de plan de la empresa, no una decisión suya |

### 8.3 Fuera por criterio de rigor mal invertido

- **Estadística inferencial.** Nada de significación, valor p ni tamaño muestral sobre doce casos.
  Aquí no se estima un parámetro de una población: se comprueba la cobertura de un instrumento contra
  un criterio fijado. **Doce casos bien elegidos valen más que doscientos al azar.**
- **Alfa de Cronbach aplicado a la batería.** Directamente incorrecto: una batería de casos **debe ser
  heterogénea**. Si tuviera consistencia interna alta sería porque está mal construida.
- **Comparativas y benchmarks de modelos, y nombres de modelo.** *"Da bastante igual qué modelo uses
  mientras no gastes miles en tokens"*. El material no se apoya en ningún nombre de modelo, a
  propósito: es el detalle que menos importa y el que más rápido caduca.
- **Prompt engineering como colección de trucos.** El curso enseña **el criterio antes del prompt**.
  Un prompt bueno que se escribe una vez y se pierde no vale nada; el mismo guardado como Gem, con sus
  fuentes, es infraestructura.
- **Vídeos de lección.** Un vídeo es relectura con mejor producción, y la relectura está clasificada
  como técnica de utilidad baja. Si hay vídeo, es de demostración de una interfaz, dura menos de tres
  minutos y va con transcripción escrita — porque la ruta de menús caduca.

### 8.4 Fuera por riesgo, ya listado en §6

P08 visados · P26 quejas formales · P29 emergencias · P25 reembolsos · P17 matching · P05/P16
nivelación y exámenes. No son "temas avanzados": son **zona prohibida con motivo escrito**.

---

## 9. LOS TRES MOMENTOS DE MAYOR RIESGO DE ABANDONO

Criterio de selección: probabilidad × irreversibilidad de la conclusión que saca. Se descarta como
"tercero" el primer resultado mediocre del M2 (semanas 5–6) no porque sea improbable —lo es— sino
porque **su contramedida es barata, conocida y ya está incorporada**: la caja *"Lo que vas a ver la
primera vez"*, escrita antes del ejercicio, que describe el resultado mediocre concreto que va a
obtener. Un fallo anunciado es una etapa; un fallo inesperado es un veredicto sobre uno mismo.

---

### MOMENTO 1 · Días 1–14 — el arranque y el hueco del diagnóstico

**Qué pasa por dentro.** El 52 % de los inscritos en un curso autodidacta **nunca llega a empezar**, y
la caída mayor está en los días 7–14 [E]. Aquí se acumulan tres cosas: la fricción de arranque; el
diagnóstico depende de un correo que puede no contestarse nunca, y esperar sin poder avanzar es la
forma más eficiente de abandonar; y el beneficio del curso todavía es abstracto mientras el coste ya
es real.

**Qué se pone justo antes:**

1. **La sesión 1 no explica el curso: produce un resultado utilizable en 20 minutos** con lo que ya
   tiene abierto, sin instalar nada y sin hablar con nadie. Instrucciones personalizadas + un correo
   real hecho con ellas + minutos cronometrados antes y después. **El mapa del curso va después del
   primer resultado.**
2. **El contrato de una página, escrito antes de empezar:** 18 semanas · 2 h semanales de tiempo
   propio · **0 €** · nada que instalar · nada que pedir a nadie · y **la definición observable de
   "terminado"** (tres artefactos vivos que usa sin que el curso se lo pida + una rúbrica escrita por
   ella). Un curso que se anuncia de 8 semanas y dura 18 se percibe como fracaso propio en la 9.
3. **El diagnóstico no puede bloquear.** La Vía B —cinco comprobaciones empíricas que infieren el plan
   desde la pantalla— está en la misma página que el correo, no en un anexo. Y la rúbrica declara
   explícitamente que *"pregunté a X el día D y no obtuve respuesta"* **es un resultado válido**.
4. **El modo mínimo y el ritual de reentrada, redactados en la semana 1** y no cuando ya ha fallado:
   una micro-sesión de 10 minutos cuenta como semana cumplida; toda vuelta tras una pausa empieza
   leyendo las tres últimas entradas de la bitácora y respondiendo las cinco preguntas de repaso.
   Redactado en la semana 1 se lee como plan; redactado en la semana en que ya falló, como excusa.
5. **PC-1 al final de la semana 2**: otra persona implicada en el punto de máxima mortalidad.

---

### MOMENTO 2 · Semanas 9–10 — el primer bloqueo que no es culpa suya

**Qué pasa por dentro.** Es el riesgo específico de este diseño y el que más me preocupa. Workspace
Studio **falla con unidades compartidas, carpetas compartidas e `IMPORTRANGE`** [V]. El centro de
gravedad de su puesto **es un buzón compartido y una hoja de camas compartida**. Es decir: la primera
vez que intente automatizar su trabajo de verdad, la herramienta le va a decir que no. Y la conclusión
que se saca de ahí no es *"me he equivocado de carpeta"*, es **"esta herramienta no sirve para mi
trabajo"** — y detrás, *"este curso no sirve para mi trabajo"*. Esa conclusión es irreversible si no se
anticipa, y por eso este momento pesa más que el resultado mediocre del M2.

**Qué se pone justo antes:**

1. **La limitación va en la primera página del módulo, con nombre y por escrito**, no en una nota al
   pie ni en una fe de erratas. *"Studio no puede trabajar con unidades compartidas. Tu buzón `info@`
   es compartido. Los primeros flujos se montan sobre tu propio buzón y sobre copias tuyas, y eso no
   es una versión de juguete: es la restricción real de la herramienta."*
2. **La lista de comprobación de plataforma, de 8 ítems binarios, entregada antes del primer flujo** y
   reutilizable como diagnóstico: *¿el fichero es mío y no está en una unidad compartida? ¿la hoja usa
   `IMPORTRANGE`? ¿el flujo tiene un solo disparador? ¿el administrador tiene ese paso restringido?*
   Convierte un bloqueo en una comprobación con resultado, que es lo contrario de un veredicto.
3. **La página "Cuando no coincide"**, escrita una vez y referenciada desde cada lección: qué hacer
   cuando el manual y la pantalla discrepan. *Si algo no coincide con lo que ves, tu pantalla tiene
   razón y este texto no.* Esto convierte la caducidad de un defecto del material en **una competencia
   enseñada**.
4. **PC-4, el comodín, cuya existencia se anuncia mucho antes de que haga falta.** Saber que hay
   salida reduce la ansiedad aunque no se use.
5. **La caja "si nada de esto funciona": documenta el fallo, rodéalo con una solución manual y sigue.**
   Un curso no puede pararse por un botón que Google movió.

---

### MOMENTO 3 · Semanas 13–15 — la frontera del escalón 2 al 3

**Qué pasa por dentro.** Es el punto donde el material solo ya no tira. La novedad se agotó, los
conceptos se abstraen (juicio, autonomía, condiciones de escalado), el pago está más lejos — y
encima, en el diseño original, aquí caía un módulo **de medición sin herramienta nueva** que además
puede darle la peor noticia posible: *que el ahorro es pequeño*. Novedad cero + producto cero +
resultado decepcionante es la combinación exacta que precipita el abandono.

**Qué se pone justo antes:**

1. **La automatización de mayor retorno visible se coloca aquí, no antes.** El M6 abre construyendo
   **el vigilante de plantillas (P32)**, que produce algo que ningún otro artefacto del curso produce:
   **una lista de errores reales que nadie de la academia sabía que existían** — precios del año
   pasado circulando en la plantilla alemana desde hace meses. Es el momento del curso en que su
   trabajo produce un hallazgo, no un ahorro.
2. **La cláusula del resultado decepcionante, escrita antes de medir:** *si la medición dice que
   ahorras poco, eso es un resultado del curso y no un fracaso tuyo*. Y las razones legítimas
   alternativas están enumeradas de antemano —menos errores, menos carga mental, respuesta más rápida
   al cliente— con la instrucción de **medir esa otra razón** si es la que importa. La honestidad de
   la medición está protegida por adelantado, que es la única forma de que la medición sea honesta.
3. **PC-5 exactamente en la frontera.** Una conversación de diez minutos sobre su propio criterio es
   el mejor combustible disponible en el punto donde el material ya no basta. Y el objeto de la
   conversación —*"¿dónde moverías la frontera?"*— es intrínsecamente halagador de su trabajo sin ser
   halago: se conversa sobre criterio, que es lo que ya tiene.
4. **El M7 dura tres semanas, no dos.** Es el único módulo al que se le da aire, y se dice por qué.
5. **La lectura de la hoja de anclas completa** como primera sesión del M7: ver cinco columnas de su
   propio trabajo, con fecha, es la evidencia objetiva contra la ilusión de fluidez. A las catorce
   semanas puede leer lo que en la semana 3 le parecía imposible.

---

## 10. UNA LECCIÓN COMPLETA, DESARROLLADA

Se desarrolla **M3.2**, la segunda sesión núcleo del escalón 1,5. Se elige porque concentra la textura
del curso entero: herramienta concreta, dato real suyo, hilo guiado, corrección por comprobación pura,
una decisión de "cuándo NO", una capa de protección de datos y el momento de lectura de la escalera.

---

```markdown
# M3.2 — La columna que clasifica sola

⏱ 45 min · Necesitas: una copia de la hoja de respuestas de la última encuesta,
y tu libro de códigos de EP-10.
Tipo de tiempo: [ mitad tiempo de trabajo | mitad tiempo propio ]

## Antes de leer nada — 5 minutos, de memoria y por escrito

1. Fuentes de verdad, memoria y procedimiento son tres cosas distintas. ¿Cuál de
   las tres, en tu montaje, es un fichero con fecha?
2. En tu batería, ¿qué tiene que contestar el sistema en los 2 casos de rechazo, y
   qué cuenta como fallo aunque la respuesta esté bien redactada?
3. Tu Gem, ¿se acuerda de lo que le dijiste ayer? ¿Por qué?
4. ¿Qué distintivo ves arriba en Gemini con la cuenta de la academia, y qué
   significaría no ver ninguno?
5. En tu libro de códigos, ¿cuál es la unidad de análisis y por qué elegiste esa?

> Escribe lo que recuerdes ANTES de mirar. Equivocarte aquí es el ejercicio, no un
> fallo. Respuestas al final de la lección.

## Para qué sirve esto en tu trabajo

**P27, encuestas de satisfacción.** Entre 600 y 800 respuestas al año con
comentarios en texto libre en más de diez idiomas. Hoy no se analizan, porque nadie
tiene tiempo de leerlos. Es el proceso de tu lista con más volumen y menos riesgo:
no hay dinero, no hay plazo legal, no lo ve ningún cliente, y equivocarse no rompe
nada. Esta lección lo pone en marcha en una tarde, dentro de una hoja de cálculo.

## El criterio        ← no caduca

**Tres ideas, y ninguna depende de Google.**

**1. Clasificar es aplicar un libro de códigos, no pedir una opinión.**
Si le pides a un modelo "clasifica estos comentarios por temas", te devuelve catorce
categorías solapadas, distintas en cada pasada, y el informe no es comparable ni
consigo mismo. Lo que produce un instrumento en vez de una anécdota es la lista
cerrada de categorías, con su definición, sus criterios de inclusión y exclusión, y
sus ejemplos frontera **con la decisión ya tomada**. Ese documento no es preparación
para el prompt: **es el prompt**.

**2. La taxonomía se congela.**
Fase abierta primero, sobre una submuestra, para construir las categorías. Después se
cierra y se aplica igual al resto, y **se mantiene igual entre oleadas**. Si las
categorías cambian cada mes, no tienes una serie temporal: tienes anécdotas
mensuales. Esto es lo que convierte el proyecto de "un informe bonito" en "un
indicador".

**3. La comprobación es la doble codificación, y lo que se aprende está en la tabla
de confusión, no en el porcentaje.**
Clasificas tú 30 comentarios **antes** de ver la salida del sistema. Después
comparas. El porcentaje global engaña cuando una categoría domina: si el 60 % de los
comentarios son de alojamiento, un clasificador que dijera "alojamiento" siempre
acertaría el 60 %. Lo accionable es *"confunde administración con alojamiento cuando
el comentario habla de la factura del piso"*. Eso se arregla; un porcentaje no.

**Y la lectura de escalón, que es lo que estás haciendo hoy:**
meter esto en la hoja **no mejora la clasificación** respecto a pegar los comentarios
en el chat. Mejora otras tres cosas, y conviene saber cuáles son: desaparece el
copiar y pegar; se aplica igual a 600 filas que a 6; y **el libro de códigos queda
escrito en un sitio en vez de en tu cabeza**. Si al subir de escalón te parece que ha
mejorado la calidad, sospecha: lo más probable es que por el camino reescribieras el
criterio, y eso es mérito tuyo, no de la hoja.

**Cuándo NO hacer esto.**
- Si la pregunta es cerrada (una escala de 1 a 5), no necesitas un modelo de
  lenguaje: necesitas una tabla dinámica. Escalón −1.
- Si el comentario menciona **salud, un menor, dinero, abogado o reclamación**, no se
  clasifica: **se para**. Deja de ser un dato de encuesta y pasa a ser una incidencia
  que hay que atender hoy.
- Si tienes 20 respuestas al año, hacerlo a mano es más rápido que montar esto.

## Los clics de hoy   ← caduca

> Verificado el 22.08.2026. Si algo no coincide con tu pantalla, **tu pantalla tiene
> razón y este texto no**. Ve a «Cuando no coincide».

1. Abre la hoja de respuestas y haz **Archivo → Hacer una copia**. Trabajas sobre la
   copia. Nunca sobre el original, nunca sobre una hoja compartida.
2. **En la copia, borra las columnas de correo, nombre y cualquier identificador**
   antes de nada. Un adjunto o una hoja van **completos**: todas las filas, todas las
   columnas, incluidas las ocultas, y todas las pestañas.
3. En una columna vacía, fila 2, escribe `=AI("<instrucción>"; B2)`. También acepta
   `=Gemini(...)`. Está en español desde septiembre de 2025 y **sólo funciona en la
   web, no en el móvil**.
4. Arrastra hacia abajo **por bloques de 50 filas**, no de 600. Si algo va mal,
   quieres enterarte en la fila 50.

> **Si la celda devuelve error o no reconoce la función:** casi seguro que tu plan es
> Business Starter, donde `=AI()` no existe. No es culpa tuya ni un fallo del curso:
> es el dato del módulo 0 cobrándose. Ruta alternativa al final de la lección: el
> mismo libro de códigos dentro de un Gem, pegando la columna en bloques. El
> ejercicio y su corrección son idénticos.

## Ejemplo trabajado
*(Nivel de desvanecimiento del escalón 1,5: los dos últimos pasos van en blanco.)*

    =AI("Eres un codificador que aplica un libro de códigos cerrado.

    Categorías permitidas, y sólo estas:
    ACADEMICO · ALOJAMIENTO · INSTALACIONES · ACTIVIDADES · ADMINISTRACION ·
    SIN_CLASIFICAR

    Definiciones, inclusiones y exclusiones: <pegadas de tu libro de códigos>

    Reglas:
    - Si el comentario encaja en dos categorías, devuelve la de la primera frase y
      añade ' +2:' con la segunda.
    - Si no encaja en ninguna, devuelve SIN_CLASIFICAR. No inventes categorías.
    - Si menciona salud, un menor, dinero, abogado o reclamación, devuelve PARAR y
      nada más.

    Devuelve sólo la etiqueta, sin explicación."; B2)

**Por qué está así, decisión a decisión:**

| Decisión | Por qué esta | Qué pasa con la otra |
|---|---|---|
| Lista cerrada y "y sólo estas" | Sin lista cerrada inventa categorías y cambia entre pasadas | Catorce categorías solapadas, informe no comparable |
| `SIN_CLASIFICAR` existe y está en la lista | Es la regla de "no lo sé" del escalón anterior, convertida en una casilla | Fuerza un encaje y ensucia todas las categorías |
| `PARAR` antes que clasificar | Es la condición de parada. Un comentario con salud no es un dato de encuesta | Un dato de categoría especial acaba en un informe |
| "Devuelve sólo la etiqueta" | Una columna de etiquetas se cuenta; una de párrafos, no | Tienes que releer 600 celdas, que es lo que querías evitar |
| **[EN BLANCO — paso 5]** ¿qué haces con la **valencia**, y por qué no cabe en esta misma columna? | | |
| **[EN BLANCO — paso 6]** ¿qué columna añades para poder **auditar** esto dentro de tres meses? | | |

## Lo que vas a ver la primera vez

Entre el 10 % y el 25 % de las filas mal, y casi todo concentrado en dos sitios:

- Los comentarios de una palabra —"bien", "ok", "todo correcto"— se colarán en alguna
  categoría en vez de caer en `SIN_CLASIFICAR`.
- Los comentarios mixtos ("el profesor genial, el piso sucio") perderán la mitad.

Y en tres o cuatro filas te devolverá una frase en vez de una etiqueta, porque el
modelo "quiere explicarse". Nada de eso significa que no funcione. Significa que tu
libro de códigos todavía no tiene una regla para esos dos casos. **La primera versión
de esto siempre se parece más a un borrador que a un instrumento.**

## Tu turno
→ Ejercicio E3.2

## Cierre — 3 líneas en la bitácora
- Qué he producido: ______
- Qué ha fallado: ______
- Qué haré distinto la próxima vez: ______

---
### Respuestas de las 5 preguntas
```

---

### 10.1 El ejercicio

```markdown
# E3.2 — Una hoja de encuestas clasificada, y su tabla de confusión

⏱ 60–75 min · Hilo: **guiado (con clave)** · Tipo de tiempo: trabajo

## Lo que tienes que producir

Una hoja llamada `encuestas-clasificadas-<fecha>`, copia limpia de la última
encuesta, con **60 respuestas reales** y tres columnas nuevas: `etiqueta`,
`segunda_categoria`, `parar`. Más una **tabla de confusión** de 30 de ellas.
Queda guardada en tu carpeta del curso, no en la carpeta compartida.

## Criterios de éxito — obsérvalos, no los valores

Al terminar, esto tiene que ser cierto:
- [ ] La hoja es **una copia** y el original no se ha tocado.
- [ ] En la copia **no hay** columnas de correo, nombre ni ningún identificador.
- [ ] Ninguna celda de `etiqueta` contiene una categoría que no esté en tu lista.
- [ ] Existe **al menos una fila** con `SIN_CLASIFICAR`.
- [ ] Existe **al menos una fila** con `PARAR`. Si no existe ninguna, comprueba que
      tu muestra no ha evitado los comentarios difíciles: coge 20 más por orden
      cronológico.

## Cómo lo vas a comprobar

Marca el nivel más alto que aplique:
- [ ] **Se ejecuta** → la columna se rellena en las 60 filas sin errores de fórmula.
- [x] **Batería con respuesta conocida → doble codificación.** La clave la escribes
      **tú**, antes: clasifica 30 comentarios a mano en `codificacion-manual.md`,
      guárdalo, y **no lo vuelvas a abrir hasta haber lanzado la columna**.
- [ ] Lista de comprobación → abajo.

## Antes de comprobar nada: escríbelo

> **Por qué lo he hecho así:** <3–5 líneas, en tus palabras>
> **Dónde creo que falla:** <1 línea>

Esto se escribe ANTES de corregir. Si lo escribes después, no sirve.

## Lista de comprobación (binaria y observable)

- [ ] ¿La hoja es una copia y no el maestro? SÍ / NO
- [ ] ¿He borrado las columnas identificadoras antes de escribir nada? SÍ / NO
- [ ] ¿Mi libro de códigos tiene, en cada categoría, **dos ejemplos frontera con la
      decisión justificada**? SÍ / NO
- [ ] ¿Está `SIN_CLASIFICAR` dentro de la lista de categorías permitidas? SÍ / NO
- [ ] ¿Hay una regla explícita para el comentario que menciona salud, un menor o a
      un empleado con nombre? SÍ / NO
- [ ] ¿He decidido y escrito cuál es mi **unidad de análisis**, y la hoja la
      respeta? SÍ / NO
- [ ] ¿Clasifiqué yo los 30 **antes** de ver la salida del sistema? SÍ / NO
- [ ] ¿He mirado el acuerdo de la **categoría menos frecuente por separado**? SÍ / NO
- [ ] ¿He escrito **una frase por cada confusión repetida**? SÍ / NO
- [ ] ¿He anotado el resultado en la hoja de anclas, con la fecha de hoy? SÍ / NO

## Si te atascas

1. Mira una fila que haya fallado y pregúntate: ¿qué regla de mi libro de códigos
   habría evitado esto? Casi siempre falta una regla, no falta "mejor prompt".
2. Comprueba si el fallo es de **formato** (devuelve una frase en vez de una
   etiqueta) o de **criterio** (devuelve la categoría equivocada). Son dos
   problemas distintos y se arreglan en sitios distintos del prompt.
3. *(Tras 25 minutos de intento)* La solución comentada, con los seis fallos
   típicos.
> Las pistas se abren en orden, no de golpe.
```

---

### 10.2 La rúbrica

```markdown
# Rúbrica — E3.2

Se usa **al día siguiente**, nunca al terminar.
Encuadre obligatorio: *"reviso el trabajo de alguien que hace mi puesto y tengo que
decidir si se lo devuelvo".*

## Bloque 1 · Señales de fallo (obligatorio buscar y responder)

Por cada una: encuentra el caso, o **declara por escrito que has buscado y no
existe**. "No aplica" no es una respuesta admitida.

| # | Señal de fallo | ☐ | Dónde / por qué no |
|---|---|---|---|
| 1 | Hay un comentario que este sistema clasificaría de dos formas distintas según el día. Escríbelo | ☐ | |
| 2 | Hay un comentario que cae en una categoría **sin que ninguna regla escrita lo respalde**: encajó "porque se ve" | ☐ | |
| 3 | Menos del 2 % de las 60 filas ha caído en `SIN_CLASIFICAR`. Si es así, el sistema no puede negarse, y un clasificador que nunca se niega no está midiendo | ☐ | |
| 4 | Hay algún dato en esta hoja que, si se filtrara mañana, tendrías que comunicar a alguien | ☐ | |
| 5 | Los comentarios en japonés, coreano o turco casi nunca salen negativos. Si es así, no es que estén contentos: es que **la queja educada indirecta no la estás capturando** | ☐ | |

## Bloque 2 · Umbral de "listo"

NO está listo si se cumple **cualquiera** de estas:
- El acuerdo con tu codificación manual está por debajo de **26 de 30**.
- Aparece **alguna etiqueta que no está en tu lista cerrada**.
- Algún comentario con mención de salud, menor, dinero o abogado **fue clasificado
  en vez de marcado `PARAR`**.
- Al aplicar el libro cerrado, **más del 15 %** cae en `SIN_CLASIFICAR`. (La
  taxonomía no cubre el dominio: vuelve a la fase abierta.)
- Cae **el 0 %** en `SIN_CLASIFICAR`. (Estás forzando encajes; es el mismo problema
  por el otro lado.)
- Alguna señal de fallo del bloque 1 está marcada y sin arreglar.

## Bloque 3 · Si lo pasas por la IA

Protocolo completo en `protocolo-ia.md`. Las tres que más se olvidan:
**hilo nuevo · no digas que es tuyo · no discutas: abre otro hilo.**
Y aquí, una específica: pega **el libro de códigos entero** junto con la rúbrica. Sin
él, el modelo se inventa el estándar, y el estándar que se inventa es benévolo.

## Mi veredicto (lo firmo yo, no la IA)

[ ] Listo · [ ] Le falta: ______ · [ ] Lo dejo así y anoto por qué: ______
```

---

### 10.3 La solución comentada

```markdown
# Solución comentada — E3.2

## Los dos pasos que estaban en blanco

**Paso 5 — la valencia va en su propia columna, no dentro de la etiqueta.**
Porque categoría e intensidad son **dos dimensiones independientes**: "el piso está
lejísimos" y "el piso está un poco lejos" son la misma categoría con distinta
intensidad, y meterlas en una sola etiqueta te obliga a multiplicar categorías
(ALOJAMIENTO_MUY_MAL, ALOJAMIENTO_REGULAR…) hasta que ninguna tiene casos
suficientes. Dos columnas: `etiqueta` y `valencia` (POSITIVO / NEUTRO / NEGATIVO).

**Paso 6 — una columna `version_libro` con la fecha del libro de códigos usado.**
Sin ella, dentro de tres meses tendrás una hoja de resultados y no sabrás con qué
criterio se produjeron, y la comparación entre oleadas será falsa. Es el mismo
principio que la fecha en cada fuente del cuaderno del M2: **un resultado sin la
fecha de su criterio no es comparable con nada.**

## Anatomía de los errores típicos

### Fallo 1 · «El clasificador amable»
- **Cómo se reconoce:** menos del 2 % de las filas en `SIN_CLASIFICAR`, y "bien" u
  "ok" clasificados como ACADEMICO.
- **Por qué pasa:** le pediste que clasificara, no le diste permiso para negarse.
  Es el mismo fallo que un sistema que nunca dice "no lo sé": no es que lo sepa
  todo, es que no lo has probado bien.
- **Arreglo mínimo:** mover `SIN_CLASIFICAR` al **principio** de la lista y añadir
  al libro un ejemplo frontera resuelto: *"'todo bien' → SIN_CLASIFICAR, porque no
  identifica ningún aspecto del servicio"*.

### Fallo 2 · «La categoría fantasma»
- **Cómo se reconoce:** aparece COMIDA, o PROFESORES, o WIFI.
- **Por qué pasa:** la lista estaba enunciada pero no cerrada, o tu libro de códigos
  nombra de pasada un tema que el modelo interpretó como categoría.
- **Arreglo mínimo:** "y sólo estas" + "no inventes categorías" + repasar el libro
  buscando sustantivos que puedan leerse como etiquetas.

### Fallo 3 · «El resumen en vez de la etiqueta»
- **Cómo se reconoce:** celdas de más de tres palabras.
- **Por qué pasa:** el formato de salida no estaba especificado como restricción,
  sólo sugerido.
- **Arreglo mínimo:** "devuelve sólo la etiqueta, sin explicación", y una columna
  auxiliar `=LARGO(...)` para cazarlas de un vistazo.

### Fallo 4 · «El traductor que suaviza»  ← el más importante y el menos evidente
- **Cómo se reconoce:** los comentarios de alumnado asiático casi nunca salen
  NEGATIVO, y sin embargo esos mismos alumnos cambiaron de alojamiento.
- **Por qué pasa:** clasificaste sobre la traducción. **Traducir antes de codificar
  altera intensidad y cortesía, que es justo lo que quieres medir.** "Quizá el
  desayuno podría mejorar un poquito" puede ser una queja seria; "the flat was
  dirty" puede ser un informe factual neutro.
- **Arreglo mínimo:** codificar **sobre el original** y guardar la traducción en
  otra columna, para la persona que luego lo lea.

### Fallo 5 · «La media que miente»
- **Cómo se reconoce:** en tu resumen aparece "los alumnos coreanos están menos
  satisfechos".
- **Por qué pasa:** hay diferencias sistemáticas por cultura en el uso de los
  extremos de una escala. Un 3/5 japonés y un 3/5 italiano no significan lo mismo.
  Puede que no estén menos satisfechos: puede que sólo estén siendo coreanos.
- **Arreglo mínimo:** nota al pie fija en el informe —no se comparan medias entre
  nacionalidades sin ella— y **la tasa de respuesta apuntada al lado del
  resultado**, siempre. Si hoy nadie la apunta, empezar a apuntarla ya es una mejora
  medible.

### Fallo 6 · «La batería fácil»
- **Cómo se reconoce:** 30 de 30 de acuerdo, y euforia.
- **Por qué pasa:** elegiste tú los 30. **Si tu batería la pasa entera a la primera,
  tu batería es fácil; no es que tu sistema sea bueno.**
- **Arreglo mínimo:** coger 30 por orden cronológico estricto y volver a mirar.

## Lo que también sería correcto

- Dos columnas separadas (`etiqueta` + `valencia`) frente a tres (añadiendo
  `intensidad`), si has anclado la intensidad con ejemplos.
- **Una fila por unidad de análisis** en vez de por comentario, si decidiste que la
  unidad es la frase. Es más trabajo y más correcto para los comentarios mixtos.
- Hacerlo todo dentro de un **Gem** en vez de con `=AI()` si tu plan no la incluye:
  el libro de códigos es el mismo y la corrección es idéntica.

## Lo que parece correcto y no lo es

- **Pedirle además "la intensidad del 1 al 10".** Devuelve un número con una validez
  aparente altísima —queda precioso en el informe— y sin ninguna ancla detrás: el
  7 de una fila no es comparable con el 7 de otra. Si quieres intensidad, ánclala
  con tres ejemplos por nivel, como hiciste con el tono en el M1. Si no, usa tres
  niveles y no diez.
- **Añadir una columna "resumen del comentario".** Te ahorra leerlos, que es justo
  lo que no te conviene ahorrar el primer mes: los comentarios son la única fuente
  que tienes para saber si tu libro de códigos cubre el dominio.
```

---

## 11. AUTOCRÍTICA

Sin la sección 11, las diez anteriores no son creíbles. Ordenado de más grave a menos.

**1 · El diseño depende de un dato que no tengo, y si sale mal se cae el mejor tramo del curso.**
Si su empresa está en **Business Starter**, `=AI()` no existe, Gemini no está en Docs ni en Sheets, y
Gemini Notebook queda en acceso básico [V]. El escalón 1,5 —que es el momento psicológico del curso,
la primera vez que algo pasa sin que ella lo pida— se degrada a una ruta alternativa correcta pero
claramente peor. Tengo contingencia escrita, pero **una contingencia no es lo mismo que un diseño**, y
el 40 % del atractivo del M3 desaparece. No puedo saberlo hasta la semana 2, y el curso entero está
escrito antes.

**2 · El riesgo más profundo: que el escalón 2 sólo se pueda montar sobre copias de juguete.**
Workspace Studio no soporta unidades ni carpetas compartidas [V]. El buzón `info@`, el buzón
`accommodation@` y la hoja de camas —es decir, **el trabajo real de su puesto**— son recursos
compartidos. Mi respuesta de diseño es honesta (poner el límite por delante, montar sobre su propio
buzón) pero incompleta: es perfectamente posible que al final del M5 tenga dos flujos vivos que
funcionan **sobre datos que ella ha copiado a mano**, lo cual es exactamente el fracaso que este curso
declara evitar — un curso que no toca el trabajo real. No tengo solución dentro de la escalera. La
salida sería pedir al administrador que le delegue una etiqueta o una carpeta propia dentro del buzón
compartido, y eso es una petición a otra persona, que es justo lo que el diseño prometía no necesitar.
**Es la contradicción más seria del documento y no la he resuelto.**

**3 · El escalón 3 es más flojo de lo que la tesis promete, y hay que decirlo.**
La escalera vende "chat → automatización → agente". Lo que puede construir de verdad es "chat →
automatización → **flujo con juicio en dos puntos**". Es honesto, es alcanzable, y `dominio-herramientas.md`
lo argumenta bien. Pero **el objetivo 1 del brief —saber qué existe, en concreto qué son los agentes—
se acaba sirviendo en buena parte por lectura**, que es justo el formato que este mismo diseño
descalifica como técnica de utilidad baja. El fichero *Mapa de lo que existe* mitiga eso convirtiendo
la lectura en escritura, pero es una mitigación, no una solución. Si el diseño tuviera un escalón 3
con producto real, sería mejor curso.

**4 · Concentro tres de los seis puntos de consulta en las seis primeras semanas.**
Lo defiendo en §4.2 y sigo pensando que es correcto por consecuencia y por curva de abandono. Pero el
riesgo es real: si en la semana 6 ya ha gastado la mitad del presupuesto relacional, el comodín PC-4 y
el PC-5 de la frontera llegan a un recurso más desgastado justo cuando más falta hacen. El diseño
apuesta a que **seis conversaciones de diez minutos en cuatro meses no desgastan nada**, y esa apuesta
no está verificada. Además, `dominio-autodidacta.md` §11 avisa de algo que asumo sin comprobar: **si el
conocimiento de su pareja es de modelos y no de Workspace, PC-4 pierde casi todo su valor.**

**5 · La batería como invariante es la mejor idea del diseño y también la más frágil de mantener.**
Exige que sostenga diez casos vivos durante dieciocho semanas y que los vuelva a pasar cinco veces. Es
poco trabajo cada vez —treinta minutos— pero es trabajo sin novedad, y las cosas sin novedad se
convierten en ritual o desaparecen. Si la batería se erosiona, **la salvaguarda número 1 del curso
desaparece y el riesgo de los tres tutoriales encadenados vuelve entero**. No he diseñado ningún
mecanismo que fuerce su mantenimiento salvo las puertas, y las puertas se pueden saltar en un curso
sin profesor.

**6 · La escalera ordena el curso por autonomía de la herramienta, no por dificultad del criterio.**
Es la crítica de fondo a mi propia tesis. Lo más difícil de todo lo que tiene que aprender —decidir
qué **no** automatizar, y saber si algo funciona de verdad— no forma un escalón: va repartido en
capas. Mis cuatro salvaguardas lo hacen **visible**, pero no lo hacen **primario**. Un diseño
alternativo que ordenara el curso por criterio y usara las herramientas como material seguramente
enseñaría mejor criterio; enseñaría peor a usar las herramientas, y probablemente se abandonaría en la
semana 4, porque no produce nada durante un mes. **He elegido el diseño que se termina antes que el
que enseña más, y esa es una decisión discutible que conviene que quede escrita.**

**7 · El curso son 36 horas de tiempo propio y arranca en octubre.**
Dieciocho semanas a dos horas. Es mucho para alguien con jornada completa en un puesto donde una misma
persona atiende el teléfono, el buzón y una incidencia de alojamiento en la misma hora. Y el
calendario asume octubre: **si quiere empezar ahora, en agosto, todo el diseño de secuencia está mal**,
porque agosto es su peor mes. La alternativa —arrancar sólo el M0 en agosto y parar— tiene su propio
riesgo: un curso que empieza y se detiene tres semanas rara vez se retoma.

**8 · El hilo guiado puede no sentirse suyo.**
P27 es el proyecto correcto por tres caminos independientes (riesgo, herramienta, formación). Pero es
un proceso que **hoy no se hace**, y eso que lo hace seguro también lo hace poco urgente. Existe el
riesgo de que lo viva como ejercicio de libro mientras su hilo propio es lo que le importa, y que el
doble hilo acabe siendo trabajo doble en vez de andamiaje. Es el supuesto más frágil del diseño y sólo
se puede comprobar usándolo.

**9 · La verificación del objetivo 3 es la más débil de las tres.**
"Manejar datos sensibles con seguridad" está bien cubierto como contenido y bien colocado como capas.
Pero **su comprobación depende de su propio juicio sobre su propio material**: E-02 y E-03 se
autocorrigen con rúbricas que ella aplica a casos que ella elige. El único contraste externo es PC-2,
diez minutos, una vez. Si sistemáticamente elige casos fáciles, la rúbrica no lo detecta. He puesto la
prueba de la compañera y el criterio de "al menos un correo rojo entero", pero es una salvaguarda de
muestreo, y el muestreo lo hace ella.

**10 · Y una duda que no sé resolver: el curso enseña a desconfiar del corrector que el propio curso
usa.**
El protocolo de siete reglas y el cebo son lo mejor que tengo, y son buenos. Pero el material le pide
a la vez que use la IA como correctora (porque no hay otra cosa) y que no se fíe de ella (porque falla
en la misma dirección en la que ella ya está sesgada). Esa tensión está resuelta en el papel con
mecanismos, y no sé si está resuelta en la práctica **en el mes cuarto, un jueves, cansada**. La
respuesta honesta es que no lo sé, y que la única forma de saberlo es que el cebo se repita —una vez
por escalón, como está previsto— y que ella misma vea si su criterio se ha degradado. He convertido mi
duda en un instrumento, que es lo mejor que se puede hacer con una duda, pero sigue siendo una duda.
