# Arquitectura 1 — LA ESCALERA DE CAPACIDADES ES EL CURSO

**Qué es esto.** Diseño de arquitectura completo para el curso descrito en `00-perfil.md`, construido
sobre el ángulo 1: la progresión que ella pidió —usar mucho mejor el chat → automatización → agente →
(opcional) avanzado— no es una restricción que haya que acomodar, es la mejor columna vertebral
disponible.

**Escrito bajo el brief corregido del 22.08.2026**, con sus dos correcciones críticas incorporadas
desde la primera línea: **(A) el curso es agnóstico de herramienta** —su entorno actual es donde
practica, no el eje— y **(B) vuelve a entrar la evangelización interna**, como módulo lateral y no
como columna vertebral, y en su versión correcta: evidenciar y contagiar, no pedir permiso.

**Fecha:** 22.08.2026.

**Documentos que da por leídos:** `00-perfil.md` · `01-analisis-referencia.md` · `dominio-academia.md`
(P01–P32) · `dominio-rgpd.md` (E-01…E-06, el semáforo) · `dominio-herramientas.md` (límites de
plataforma verificados) · `dominio-autodidacta.md` (mecanismos de corrección, puntos de caída,
plantillas) · `dominio-psicologia.md` (C1–C13, EP-01…EP-14) · los dos borradores previos, escritos
bajo el brief anterior.

**Marcas:** **[V]** verificado en fuente primaria · **[R]** reconstrucción razonada · **[NV]** no
verificable desde fuera · **[!]** decisión que no es suya y se escala · **[J]** juicio de diseño mío.

---

## 1. TESIS

### 1.1 El enunciado

> **La escalera no es el orden en que se presentan las herramientas. Es una secuencia de techos, y
> cada techo se define por una sola variable: cuánta autonomía has cedido.**
>
> Cada escalón existe porque el anterior tiene un límite concreto, y ese límite hay que **chocar con
> él en su trabajo real**, no leerlo. El curso no enseña asistentes guardados, ni flujos, ni agentes:
> enseña a **reconocer en qué escalón estás, en la herramienta que sea y en el año que sea**, y a
> decidir si merece la pena subir. La herramienta es lo que se compra con esa decisión.

Corolario operativo: **se sube cuando el escalón anterior ha producido algo que funciona y se ha
quedado corto.** No cuando el calendario lo dice, no cuando apetece. Y cada escalón trae escrito, con
el mismo peso tipográfico, **cuándo NO subir** — porque la mitad del criterio consiste en saber que
una automatización simple basta, y la otra mitad en saber que a veces no hace falta IA en absoluto.

### 1.2 La pieza que hace la tesis agnóstica: LAS CINCO PREGUNTAS

Este es el cambio de fondo respecto al borrador anterior, y es lo que impide que la escalera sea una
escalera de productos. Un escalón no se identifica por el nombre de lo que estás usando: se identifica
respondiendo cinco preguntas. Sirven hoy, sirvieron en 2020 y servirán con una herramienta que aún no
existe.

| # | Pregunta | Respuestas posibles, de menos a más autonomía cedida |
|---|---|---|
| **1** | **¿Quién dispara?** | yo, cada vez · un reloj · un suceso · lo decide el sistema |
| **2** | **¿Quién decide los pasos?** | yo, sobre la marcha · yo, de antemano, y quedan fijos · el sistema, sobre la marcha |
| **3** | **¿De dónde saca lo que sabe?** | de lo que le pego en el momento · de fuentes que yo controlo y fecho · de donde quiera |
| **4** | **¿Qué puede tocar?** | nada · leer lo que yo le doy · leer todo lo que yo puedo leer · escribir en lo mío · escribir hacia fuera |
| **5** | **¿Quién firma la salida?** | yo, siempre · yo, por muestreo · nadie |

**Por qué estas cinco y no otras.** Porque las cinco son las únicas que cambian de respuesta al subir
de escalón, y porque las respuestas se **observan**, no se opinan. Y porque las preguntas 4 y 5 son,
literalmente, protección de datos y salvaguardas: por eso el bloque de datos no va pegado con celo al
final del curso, sino que está dentro del instrumento con el que se clasifica cualquier herramienta.

Esta ficha de cinco preguntas es **el artefacto más portátil del curso** y es la respuesta directa al
objetivo 4 del perfil (criterio portátil). Aparece en todos los módulos, encabeza cada escalón, y en
el módulo final se le aplica a una herramienta que el curso no ha enseñado, para comprobar que
funciona sin el curso.

### 1.3 Los escalones, nombrados por capacidad y no por producto

| # | Escalón | El techo que se choca **en su trabajo**, no en teoría | Qué cambia en las cinco preguntas |
|---|---|---|---|
| **−1** | **Ni IA** | La tarea tiene pasos fijos y datos estructurados. Meter un modelo de lenguaje aquí no es ineficiente: **es introducir un error posible donde no lo había** | No aplica: no hay sistema |
| **0** | **Chat a pelo** (donde está hoy) | *"Cada conversación empieza en blanco y le vuelvo a explicar la academia."* Y no sabe con qué cuenta entra ni qué protege esa cuenta | P3 = "lo que le pego" |
| **1** | **Chat con el contexto puesto** | *"Se acuerda de sus instrucciones, no de lo que pasó ayer. Y sigo teniendo que abrirlo yo cada vez."* La memoria fiable es un fichero; el disparador sigue siendo su dedo | P3 pasa a "fuentes que yo controlo y fecho" |
| **2** | **Disparo sin ella: reloj y lote** | *"Dispara los lunes. No reacciona a que **haya pasado algo**."* Un lunes no es un suceso; que entre un correo, sí | P1 pasa de "yo" a "un reloj" |
| **3** | **Flujo por suceso** | *"Siempre el mismo camino. El caso que no previste sale mal, y sale mal en silencio."* | P1 pasa a "un suceso"; P2 se congela en "yo, de antemano" |
| **4** | **Juicio dentro del flujo** | *"Sigue siendo un camino con bifurcaciones que yo dibujé."* | P2 se abre en dos o tres puntos concretos |
| **5** | **Agente** | — | P2 pasa entera al sistema. **Y ahí está el pago: renuncia a ser predecible** |

**El mapeo con la progresión que ella pidió**, para que quede claro que se respeta y no se sustituye:

| Lo que pide el perfil | Escalones |
|---|---|
| «usar mucho mejor el chat que ya tiene» | E0 → E1 |
| «automatizaciones de tareas sencillas y repetitivas» | E2 → E3 |
| «agentes, cuando la tarea lo justifique» | E4 → E5 |
| «herramientas más avanzadas tipo Claude Code, al final y opcionales» | apéndice de lectura |

**El escalón 5 se conoce, no se sube.** Y se explica por qué —hoy, en su entorno, la barrera es de
licencia, de permisos y de datos, no de capacidad suya— con la condición de revisión escrita, para que
el "no" no sea dogma. El escalón "avanzado" del perfil (herramientas tipo terminal) no es un escalón:
es una implementación del 5 que además está fuera del estándar de su empresa y sale de su bolsillo.

### 1.4 Por qué esta tesis es la correcta para ESTA alumna con ESTOS objetivos

Seis razones, en orden de peso. Las cuatro primeras son específicas de ella.

**(a) Su objetivo es un cambio de hábito, y un hábito no se cambia con un mapa.**
El encargo dice literalmente *"salir del hábito del chat"*. Un hábito se sustituye cuando el gesto
antiguo produce un resultado peor que el nuevo **en su propia mano**, no cuando alguien le explica que
existe algo mejor. La estructura de techos convierte cada transición en una experiencia: la primera
vez que el asistente no se acuerda de lo de ayer, la primera vez que algo dispara un lunes sin que
haya llegado nada, la primera vez que el flujo se traga un caso que no previó. Un temario ordenado por
conceptos le contaría esas cinco cosas; la escalera se las hace.

**(b) La escalera es lo que hace portátil el criterio, no lo que lo ata a un producto.**
Este es el punto que el brief corregido obliga a defender y donde el diseño anterior era más flojo. Un
temario ordenado por herramientas produce conocimiento de herramientas. Un temario ordenado por
**grados de autonomía cedida** produce una pregunta que se le hace a cualquier cosa. Cuando dentro de
tres años le pongan delante algo que no existe hoy, la pregunta que sabrá hacer no es "¿cómo se usa?"
sino **"¿quién dispara, quién decide los pasos, de dónde saca lo que sabe, qué puede tocar y quién
firma?"** — y con esas cinco respuestas ya sabe qué salvaguardas necesita y qué datos no le puede
meter. Eso no caduca con un renombrado.

**(c) Su formación le da ventaja exactamente en la juntura entre escalones.**
`dominio-psicologia.md` documenta que el solapamiento fuerte está en dos sitios: **escribir el criterio
antes de construir** (C1) y **comprobar si el resultado sirve** (C7, C13). Esas dos cosas no son
escalones: son lo que se hace **al pie de cada escalón y al llegar arriba**. Una arquitectura ordenada
por herramientas dejaría su ventaja fuera del temario; ésta la pone justo donde se decide subir o no.

**(d) El orden coincide con el orden del riesgo, y eso no es casualidad.**
El escalón bajo toca datos verdes y errores internos y reversibles; el alto toca datos ámbar y errores
que ve un cliente. `dominio-rgpd.md` §7.4 llega a la misma conclusión desde el ángulo contrario
—*empezar por lo interno, donde el error es barato*— y `dominio-herramientas.md` §3.3 desde el ángulo
de lo que la plataforma puede hacer. **Tres análisis independientes convergen en la misma secuencia.**

**(e) Le quita de encima la barrera de entrada.**
Los escalones 0 a 4 se recorren con **cero instalaciones, cero altas de proveedor, cero peticiones de
licencia y cero euros**, dentro de lo que su empresa ya paga [V]. En un curso autodidacta con jornada
completa, donde el 52 % de la mortalidad ocurre antes de la primera lección [E, Reich y
Ruipérez-Valiente 2019], la fricción de arranque es el factor de mortalidad número uno.

**(f) Y hace que la evangelización interna tenga algo que evangelizar.**
El objetivo 5 no se puede cumplir en el vacío: para evidenciar valor hace falta un artefacto vivo y un
número honesto. La escalera los produce por diseño, en ese orden, y por eso el módulo lateral de
adopción puede colgarse de ella sin inventarse nada.

### 1.5 EL RIESGO DE ESTA TESIS, DICHO CON LAS PEORES PALABRAS POSIBLES

> **Una escalera de capacidades produce, por defecto, tres tutoriales de herramienta encadenados.** Al
> final sabe montar un asistente guardado, sabe montar un flujo y sabe poner una bifurcación en medio;
> y en cuanto renombren algo o cambie de empresa, no le queda nada. El criterio —lo único que el brief
> dice que no caduca— se habría quedado en las frases de transición entre módulos.

Se agrava por tres cosas específicas de este caso. Una: **la herramienta es el temario**, así que no
hay distancia natural entre "aprender a usar esto" y "aprender a decidir". Dos:
`dominio-herramientas.md` §8.1 documenta que en 2026 han cambiado de nombre tres piezas centrales en
cinco meses. Tres, y es la más insidiosa: **el apéndice de clics es la parte accionable**, y en
cualquier material la gente lee lo accionable y hojea lo demás.

### 1.6 LA SALVAGUARDA: cinco mecanismos estructurales, no una advertencia

Una advertencia en la introducción no es una salvaguarda. Estos cinco lo son: si se quitan, el curso
se rompe visiblemente, que es la propiedad que define una salvaguarda de verdad.

---

**Salvaguarda 1 · LA BATERÍA ES EL INVARIANTE. La herramienta es la variable.**

En el módulo 1, antes de tocar ninguna herramienta, construye **una batería de 10 casos reales de su
trabajo** con la tabla de especificaciones de `dominio-psicologia.md` C2: 5 normales, 3 límite, 2 que
el sistema debe rechazar. Y la pasa **contra el chat pelado que usa hoy**, anotando el resultado con
fecha.

Esa misma batería, sin cambiar ni un caso, se vuelve a pasar **al final de cada escalón**. Una columna
nueva por escalón, con su fecha:

```
CASO                     | chat hoy | +contexto | +reloj  | +flujo | +juicio
                         | 12-oct   | 09-nov    | 23-nov  | 21-dic | 25-feb
-------------------------|----------|-----------|---------|--------|--------
N1 precio 4 semanas      |   NO     |    SÍ     |   SÍ    |  SÍ    |   SÍ
N2 fechas de inicio      |   SÍ     |    SÍ     |   SÍ    |  SÍ    |   SÍ
L1 mixto: curso+piso     |  inventa |  pregunta | pregunta| pregunta| pregunta
L2 queja educada         |  inventa |  inventa  | inventa | pregunta| pregunta
R1 plazo de visado       |  responde|  no lo sé | no lo sé| PARAR  |  PARAR
R2 dato que no tiene     |  inventa |  no lo sé | no lo sé| no lo sé| no lo sé
```

**Lo que esa hoja enseña, y que ninguna lección puede enseñar igual de bien:** entre la columna 2 y la
columna 5 **casi nada mejora**. La calidad de la respuesta se gana entera en el escalón 1 —cuando se
escribe el criterio y se le dan fuentes con fecha— y a partir de ahí sólo se puede perder. Lo que
cambia al subir no es la calidad: es **quién dispara, cuántas veces, y cuánta autonomía has cedido**.

Ese es el criterio transferible del curso, y no se lo cuenta nadie: lo lee en su propia hoja. La
pregunta que sabrá hacerle a cualquier herramienta futura es *"¿esto me cambia la calidad o me cambia
el disparador?"*, que es la pregunta correcta y la que casi nadie hace.

---

**Salvaguarda 2 · LA PRUEBA DE TRADUCCIÓN. Una vez por escalón, la misma capacidad en otra herramienta.**

*Es el mecanismo nuevo, y es la respuesta directa a la corrección (A) del brief.*

Al cerrar cada escalón, **20 minutos**: reproducir la **misma capacidad** en una herramienta distinta
de la que ha usado. No el mismo artefacto entero: la capacidad, con un solo caso de la batería.

- Cierre del E1 → montar el mismo asistente guardado, con dos de sus fuentes, en la otra herramienta
  que ya usa. Pasar un caso normal y un caso de rechazo.
- Cierre del E2 → programar el mismo recordatorio en otro sitio.
- Cierre del E3/E4 → **no se monta**: se rellena la ficha de cinco preguntas para dos productos de
  automatización que no ha usado, leyendo su documentación durante quince minutos, y se contesta:
  ¿qué escalón es? ¿qué salvaguardas necesitaría?

**Qué se entrega:** tres líneas. *"Lo que se llama igual: ___. Lo que se llama distinto: ___. Lo que
esta herramienta no puede hacer y la otra sí: ___."*

**Por qué funciona y por qué es barata:** ya usa ChatGPT por su cuenta, así que la segunda herramienta
no cuesta dinero ni permiso; y el ejercicio, hecho con datos verdes (tarifario, calendario,
condiciones, que **no son datos personales**), no toca el problema de la cuenta personal. Coste total
en todo el curso: **una hora y media**.

**Por qué es una salvaguarda y no un adorno:** produce el único dato que demuestra que lo aprendido
era la capacidad y no el botón. Y su resultado es observable: si no consigue reproducir la capacidad
en veinte minutos, **no aprendió la capacidad, aprendió la ruta**, y ese diagnóstico llega a tiempo de
corregirlo.

---

**Salvaguarda 3 · Los clics viven FUERA de la lección, en un apéndice que se puede borrar entero.**

No es una sección dentro de la lección: es otro fichero, con su propia fecha. La prueba mecánica que
lo mantiene honesto está en §4: **se borra el apéndice y el curso todavía se puede hacer**. Un
ejercicio que deje de poderse hacer está mal escrito y se reescribe.

---

**Salvaguarda 4 · Cada escalón tiene una PUERTA con condición observable, y la puerta no la abre el
calendario.**

| Puerta | Condición para subir — todas observables, ninguna valorativa |
|---|---|
| **0 → 1** | Existe la ficha *Bajo qué régimen trabajo* con las cuatro respuestas **o** con la frase *"pregunté a X el día D y no obtuve respuesta"* · existe su semáforo adaptado · hay una tarea elegida con puntuación positiva y **ningún −3** en el filtro de E-04 · hay una línea base **medida**, no estimada |
| **1 → 2** | La batería da **5/5** en los normales, **pide aclaración** en los 3 límite (inventar una decisión es fallo aunque acierte) y dice **"no lo sé"** en los 2 de rechazo · **y** ha usado el asistente al menos 5 veces en una semana **sin que el curso se lo pidiera** · **y** ha pasado la prueba de traducción |
| **2 → 3** | Su codificación manual de 30 comentarios y la del sistema coinciden en **≥26**, y hay **una frase escrita por cada confusión repetida** de la tabla de confusión |
| **3 → 4** | **Dos flujos vivos** y **haber visto uno fallar**, sabiendo por qué falló |
| **4 → 5** | *No existe.* El escalón 5 se conoce, no se sube — y el módulo dice qué tendría que cambiar para que existiera |

La segunda condición de la puerta 1→2 es la más importante del curso: **si no usa el asistente
espontáneamente, el asistente está mal, y automatizar algo que está mal es multiplicar el error.** La
puerta no mide si aprendió la lección; mide si el artefacto le sirve. Es la única forma honesta de
saberlo sin profesor.

La de 3→4 es igual de deliberada: **sin haber visto un fallo no hay criterio para dar autonomía a
nada.** Si a esas alturas no ha fallado nada, el material trae un fallo provocado.

---

**Salvaguarda 5 · Cada escalón lleva su "CUÁNDO NO SUBIR", y no subir se evalúa; más CASOS SATÉLITE.**

No basta con escribirlo: hay que puntuarlo. En el M6 hay un entregable obligatorio que es **la lista
de lo que ha decidido NO automatizar, con el motivo por escrito**, y la rúbrica declara que **un
módulo en el que todo acaba automatizado está mal resuelto**. Se refuerza con **la regla del cuatro**
(§7).

Y cada módulo lleva un ejercicio de 15 minutos sobre un proceso **distinto del hilo** —el caso
satélite—, que a veces **no admite la solución del módulo**, que es justamente donde el criterio se
hace visible. Satélites por módulo, sacados del inventario: P02 presupuesto (respuesta correcta:
escalón −1) · P08 carta de visado (zona prohibida, y por un motivo que no es la dificultad) · P30
parte semanal (automatización determinista, sin modelo en el camino crítico) · P28 reseñas (clasificar
sí, publicar nunca, y hay un motivo de RGPD) · P16 exámenes DELE (las reglas son de otro).

### 1.7 Qué tomamos de la referencia y qué no

Los **cinco pasos** del programa polaco son correctos y su orden se sostiene. Lo que hacemos es **dejar
de usarlos como columna vertebral y usarlos como capa transversal**: cada escalón ejecuta los cinco
pasos completos a su nivel. El paso 4 (acceso a herramientas) se encoge, porque en su pila no hay
nada que conectar y decirlo es más honesto que inflarlo; el paso 5 (evaluación) se expande y **se muda
del final al pie de cada escalón**, que es el cambio estructural más importante y el que su formación
permite.

---

## 2. RESULTADOS DE APRENDIZAJE OBSERVABLES

Redactados como desempeños. Ninguno usa "entenderá", "conocerá" o "será capaz de apreciar".

| # | Al terminar, ella… | Se observa en | Módulo |
|---|---|---|---|
| **RA1** | **Clasifica** cualquier herramienta —incluida una que el curso no le haya enseñado— respondiendo las cinco preguntas, y **deriva** de esas respuestas qué salvaguardas necesita y qué datos no puede meterle | La ficha de cinco preguntas rellenada para una herramienta nueva, en M9 | M0 → M9 |
| **RA2** | **Determina** bajo qué régimen de datos trabaja —entrenamiento, retención, ubicación, contrato— y **cita** el dato o la constancia de haberlo preguntado | La ficha de régimen, sin ninguna frase que empiece por "creo que" | M0 |
| **RA3** | **Clasifica** cualquier dato de su puesto en verde / ámbar / rojo y **reescribe** un caso real hasta que una compañera no pueda identificar a la persona | 10 correos clasificados; 3 casos reescritos que superan la prueba de la compañera; al menos uno declarado **no reescribible** | M0, M2 |
| **RA4** | **Escribe** el criterio de "resultado correcto" en 4–6 indicadores que otra persona pueda comprobar sí/no contra una fuente, **antes** de tocar ninguna herramienta | La ficha de criterio, sin *adecuado, correcto, natural, profesional, de calidad* sin ancla detrás | M1 |
| **RA5** | **Construye** una batería de 10 casos —5 normales, 3 límite, 2 de rechazo— con casos que **no** usó para escribir el prompt, y **la vuelve a pasar** cada vez que cambia algo, anotando la fecha | La hoja de anclas, una columna por escalón, fecha en cada una | M1 → M8 |
| **RA6** | **Construye** un asistente reutilizable sobre fuentes fechadas que responde **citando el documento** y **dice "no lo sé"** cuando la respuesta no está | La batería: 5/5 normales, pregunta en los límite, "no lo sé" en los 2 de rechazo | M2 |
| **RA7** | **Reproduce** una capacidad ya aprendida en una herramienta distinta en menos de 20 minutos, y **nombra** qué se llama igual, qué se llama distinto y qué no puede hacer | Las tres líneas de la prueba de traducción, una por escalón | M2, M3, M5, M8 |
| **RA8** | **Codifica** texto libre multilingüe con un libro de códigos cerrado y **compara** su codificación con la del sistema construyendo la tabla de confusión | ≥26/30 de acuerdo y una frase por cada confusión repetida | M3 |
| **RA9** | **Construye** un flujo con disparador por suceso que **prepara, clasifica o avisa y nunca envía**, con condiciones de parada, temas prohibidos y tope de volumen | Dos flujos vivos; el apagado **probado**, no imaginado | M4, M5 |
| **RA10** | **Decide y justifica**, para cada tarea candidata, el escalón que le corresponde —incluido **"ni IA"** y **"no automatizar"**— y **nombra qué tendría que cambiar** para que la decisión fuera otra | La lista de descartes del M6, con motivo y condición de revisión | M6 |
| **RA11** | **Mide** el efecto de un sistema suyo con línea base, unidad por pieza de trabajo y coste completo, y **nombra una amenaza a la validez interna que no puede descartar** | Media página por sistema, sin la palabra "significativo", con el tiempo de revisión restado | M6 |
| **RA12** | **Convierte** un resultado suyo en evidencia que sobrevive a tres preguntas escépticas, y **entrega** un artefacto a una persona concreta de forma que ésta pueda usarlo **sin ella** | La página de resultados + el manual de una cara + **la medición de adopción a las dos semanas** | M7 |
| **RA13** | **Corrige** su propio trabajo con IA aplicando el protocolo de siete reglas, y **audita al corrector** con un artefacto de defectos plantados antes de fiarse de él | Resultado del cebo anotado; y al menos un caso registrado en que decidió **no** aceptar una crítica de la IA, con el motivo | M2, M5 |
| **RA14** | **Escribe la rúbrica** de un artefacto suyo, con al menos tres criterios negativos que exigen salida escrita | La rúbrica del M8, redactada por ella y aplicada al día siguiente en tercera persona | M8 |

**RA14 es el criterio de terminación del curso.** Cuando puede escribir los criterios de su propio
artefacto, ya no necesita el material. Va escrito en la semana 1.

**RA1 y RA7 son los dos que hacen falsable la agnosticidad.** Si al final del curso no puede rellenar
la ficha de cinco preguntas para una herramienta que el curso no enseñó, y no puede reproducir una
capacidad en otro sitio en veinte minutos, entonces el curso fue un curso de una herramienta y
fracasó, por muy bien que hayan salido los demás resultados.

---

## 3. MAPA DE MÓDULOS

### 3.1 Vista general

**20 semanas · 10 módulos + 1 apéndice de lectura.** Módulo = 2 semanas = 3 sesiones núcleo de 35–45
min + 1 bloque de proyecto de 60–90 min + evaluación. Presupuesto: **2 h semanales de tiempo propio**;
el bloque de proyecto es **tiempo de trabajo**, porque es trabajo del puesto hecho de otra manera, y
el material lo declara así en cada lección. **Arranque en octubre**: el pico de junio–septiembre mata
cualquier calendario que lo ignore [`dominio-autodidacta.md` §5.5].

| Mód. | Título | Escalón | Sem. | Capacidad nueva | Tronco / lateral |
|---|---|---|---|---|---|
| **M0** | Dónde estoy y bajo qué régimen trabajo | 0 | 1–2 | ninguna | tronco |
| **M1** | Escribir el criterio antes que el prompt | pie | 3–4 | **ninguna, a propósito** | tronco |
| **M2** | Un asistente que cita sus fuentes y sabe decir "no lo sé" | 1 | 5–6 | asistente guardado + base de fuentes citables | tronco |
| **M3** | La primera vez que pasa algo sin ti | 2 | 7–8 | disparo por reloj + proceso por lote | tronco |
| **M4** | Del artefacto al disparador | 3 | 9–10 | flujo con disparador por suceso | tronco |
| **M5** | Prepara, no envíes | 3 | 11–12 | ninguna | tronco |
| **M6** | ¿Esto sirve de verdad? | — | 13–14 | ninguna | tronco |
| **M7** | **Que lo adopten** | — | 15–16 | ninguna | **lateral** |
| **M8** | Juicio dentro del flujo — y qué es un agente | 4 / 5 | 17–19 | puntos de juicio | tronco |
| **M9** | Cerrar y dejarlo vivo | — | 20 | ninguna | tronco |
| **M10** | *(apéndice de lectura)* Lo que hay más arriba | 5+ | — | ninguna | opcional |

**Capacidades nuevas en 20 semanas: cuatro.** Máximo una por módulo, y ninguna se introduce antes de
haber agotado la anterior.

**Qué significa "lateral" en M7, y es una propiedad estructural, no una etiqueta:** no abre ninguna
puerta, ningún módulo posterior depende de él, y **se puede mover, retrasar o saltar sin romper la
secuencia**. Si el calendario se tuerce, **M8 se hace antes que M7** y M7 puede ocurrir meses después,
incluso sobre un artefacto que ella monte fuera del curso. Va antes de M8 por una sola razón, que es
de abandono y no de lógica: su recompensa es social y llega en el punto donde el material solo ya no
tira (§10).

---

### 3.2 M0 · Dónde estoy y bajo qué régimen trabajo

| | |
|---|---|
| **Cambio mental** | *"La IA no es una web a la que voy. Es una herramienta con una configuración, un dueño y un perímetro — y el mismo texto en la misma pantalla es seguro o no según con qué cuenta haya entrado."* |
| **Qué construye** | (1) instrucciones permanentes activas en su herramienta de empresa; (2) la ficha **Bajo qué régimen trabajo** (E-01 adaptado); (3) su **semáforo** verde/ámbar/rojo adaptado a la academia, impreso; (4) su inventario de tareas, corrigiendo con tachones el mapa de P01–P32; (5) el **hilo propio** elegido con el filtro puntuado de E-04; (6) la **línea base medida** (EP-09) |
| **Duración** | 2 semanas · ~4 h propias |
| **Capacidad y cómo se hace transferible** | La capacidad es **"instrucciones permanentes"**: contexto que no se repite en cada conversación. Existe en toda herramienta de chat de pago. Se enseña por su seña —*"busca dónde se guarda algo que se aplica a todas las conversaciones y no a una"*— y por su límite, que también es universal: **sirve para identidad, no para procedimiento**; si se llena de detalles de un proceso, contamina el resto |
| **Cómo se autocorrige** | **Cuatro mecanismos, ninguno de juicio.** (a) La rúbrica de 8 casillas, con el estándar duro: *"no lo sé y lo he preguntado" vale; "creo que sí" no vale*. (b) **E-05, verdadero/falso de 12 ítems con solución al pie**; umbral <10 aciertos → releer. (c) El filtro de E-04 tiene **descalificadores por número de proceso** (P08, P17, P22, P25, P26, P29 quedan fuera automáticamente): es aritmética, no criterio. (d) Las comprobaciones empíricas del entorno **las corrige la pantalla**: se escribe algo y sale o no sale |

**Secuencia interna, y por qué ésta:**

- **Sesión 1 (20 min) — "El primer minuto ganado".** Entra con la cuenta de la empresa, comprueba el
  distintivo que indica bajo qué régimen está, lo anota, escribe sus instrucciones permanentes y las
  usa **hoy** en un correo real pendiente. Cronometra antes y después. Sale con tiempo ahorrado, el
  primer dato del diagnóstico y la primera lección de datos, sin instalar nada y sin hablar con nadie.
  **El mapa del curso va después de este resultado, nunca antes.**
- **Sesión 2 — El diagnóstico.** Las siete comprobaciones que hace sola + los correos ya redactados
  para administración y para quien administre el entorno, literales para copiar y pegar.
- **Sesión 3 — El semáforo** sobre sus 10 últimos correos reales (E-02), con su trampa deliberada: la
  mayoría quita el nombre y cree que ya está. La rúbrica no lo corrige; se corrige en M2.
- **Bloque de proyecto — El inventario y la elección**, con la línea base arrancada.

> **Nota de diseño sobre la espera.** El correo al administrador puede no contestarse nunca. **El curso
> no puede bloquearse ahí**: el diagnóstico empírico infiere el régimen desde lo que se ve en pantalla,
> y tiene una virtud extra: es literalmente operacionalizar un constructo en indicadores observables.
> La rúbrica declara que *"pregunté y no obtuve respuesta"* es un resultado válido.

---

### 3.3 M1 · Escribir el criterio antes que el prompt

| | |
|---|---|
| **Cambio mental** | Dos, los más caros del curso. (1) *"El cuello de botella no es el prompt: es que nadie ha escrito qué cuenta como respuesta correcta."* (2) **Validez aparente**: *"un modelo de lenguaje es el instrumento con la validez aparente más alta y la garantía de contenido más baja que vas a manejar en tu vida — está optimizado para producir texto plausible."* Esa segunda no la tiene que creer por autoridad: la deduce de algo que ya sabe |
| **Qué construye** | (1) la **ficha de criterio** (EP-01); (2) las **anclas de tono** (EP-02), que no son calentamiento: son el contexto del M2; (3) los **10 casos apartados antes de escribir nada** (EP-06); (4) la **batería** con tabla de especificaciones (EP-03); (5) **la primera columna de la hoja de anclas** |
| **Duración** | 2 semanas |
| **Capacidad y cómo se hace transferible** | Ninguna herramienta nueva, **deliberadamente**. Y ése es el módulo más agnóstico del curso por construcción: nada de lo que produce depende de dónde se ejecute. Es el módulo que se llevaría intacto a otra empresa y a otro sector |
| **Cómo se autocorrige** | (a) **Rúbrica negativa** de EP-01: prohibidas *adecuado, correcto, natural, profesional, de calidad* sin ancla; cada indicador se contesta sí/no mirando la salida y una fuente; al menos uno verificable contra fuente externa; si todos son críticos, no ha priorizado. (b) **Prueba mecánica**: la ficha cabe en una cara. (c) EP-06 tiene una autocorrección contraintuitiva: *si al abrir los diez apartados no falla ninguno, sospecha del muestreo antes que celebrar*. (d) La batería contra el chat de hoy es **comprobación pura**: sale o no sale |

La sesión 1 empieza pasando la batería contra el chat actual y viendo cómo saca 4/10: la ficha de
criterio nace como respuesta a un fallo observado, no como tarea previa. Es lo que impide que este
módulo se lea como deberes.

---

### 3.4 M2 · Un asistente que cita sus fuentes y sabe decir "no lo sé"

| | |
|---|---|
| **Cambio mental** | *"La memoria fiable es un fichero, no una sensación."* Y la tríada que los principiantes mezclan siempre: **fuente de verdad** (hechos, desde una sola dirección) ≠ **memoria** (acuerdos que permanecen) ≠ **procedimiento** (pasos y formato) |
| **Qué construye** | (1) un **asistente guardado** alimentado con la ficha de criterio y las anclas de tono; (2) una **base de fuentes citables** con el tarifario, el calendario, las condiciones generales y el FAQ de visados, **con fecha de última revisión en cada fuente**; (3) la regla de **"no lo sé"** y de **cita del documento** |
| **Duración** | 2 semanas |
| **Capacidad y cómo se hace transferible** | Dos capacidades hermanas que existen en toda herramienta seria: guardar instrucciones con nombre, y responder **sólo** desde un corpus cerrado citando el fragmento. Se enseñan por sus **tres señas universales**: las fuentes siguen ahí mañana · la respuesta dice de qué documento sale · se puede listar qué hay dentro. Si falta una de las tres, no es esta capacidad, es un adjunto en una conversación. **Prueba de traducción obligatoria al cierre** |
| **Cómo se autocorrige** | **Cuatro capas, fiabilidad decreciente.** (a) **La batería, columna nueva con fecha**: 5/5 normales; en los 3 límite **pide aclaración** (inventar es fallo aunque acierte); en los 2 de rechazo dice **"no lo sé"**. (b) **Lista binaria** de 10 ítems observables. (c) **El cebo del escalón 1** (control positivo): el curso trae un artefacto de mentira con **tres defectos plantados y documentados** —uno visible, uno de omisión, uno de criterio—; ella lo pasa por el protocolo y después abre la hoja de defectos y cuenta. Si encuentra 1 o 0, **ese tipo de trabajo no se corrige con IA en el resto del curso**. (d) **El protocolo de siete reglas** |

> **Por qué el cebo va aquí y no más tarde.** Es el ejercicio de mayor apalancamiento de todo el curso:
> audita el instrumento que va a usar cincuenta veces después. Y es psicometría —control positivo— con
> otro nombre, así que lo reconoce al instante.

**Aquí entra la capa 2 de protección de datos** (§8), porque es el momento exacto en que pasa de pegar
texto a subir ficheros.

---

### 3.5 M3 · La primera vez que pasa algo sin ti

| | |
|---|---|
| **Cambio mental** | *"Automatizar no es una herramienta nueva. Es quitar el dedo del disparador."* Y el corolario que la escalera hace visible: **subir de escalón no mejora la respuesta; cambia quién la pide y cuántas veces** |
| **Qué construye** | (1) un **disparo por reloj**: un resumen semanal o un recordatorio; (2) el **proceso por lote** sobre la hoja de respuestas de la encuesta, con el **libro de códigos** de EP-10 dentro como instrucción. Aquí arranca de verdad el hilo guiado (P27) |
| **Duración** | 2 semanas |
| **Capacidad y cómo se hace transferible** | Dos capacidades: **disparo recurrente** y **aplicar la misma instrucción a muchas filas**. La segunda existe hoy dentro de las hojas de cálculo, pero la capacidad —*una instrucción, N unidades, resultado en columna*— es anterior a ese botón y le sobrevivirá. Se enseña con su límite universal: **un reloj no es un suceso**, y ése es el techo que motiva el escalón siguiente |
| **Contingencia obligatoria** | Si su entorno no incluye la función en la hoja, el material trae la ruta alternativa por delante: el mismo libro de códigos dentro del asistente guardado, procesando en bloques. **Aquí se cobra el diagnóstico del M0**, y se dice así: no es un fallo suyo ni del curso. El ejercicio y su corrección son idénticos |
| **Cómo se autocorrige** | **Doble codificación (EP-07), comprobación pura.** Clasifica ella 30 comentarios **antes** de ver la salida; compara; construye la **tabla de confusión**; escribe una frase por confusión repetida; y mira el acuerdo de la **categoría menos frecuente por separado** —si el 60 % son de alojamiento, un clasificador que dijera siempre "alojamiento" acertaría el 60 %. Y: al aplicar el libro cerrado a 40 comentarios nuevos, **menos del 15 % debe caer en "otros"**; si cae 0 %, sospechar de encajes forzados |
| **Satélite** | **P02, el presupuesto**, montado **con IA y con fórmula** sobre los mismos veinte casos, cronometrado y con los errores contados. Gana la fórmula por goleada. **Enseñar el "no" haciendo el "sí" y midiendo que pierde es infinitamente más fuerte que prohibirlo** |

---

### 3.6 M4 · Del artefacto al disparador

| | |
|---|---|
| **Cambio mental** | *"Un flujo no piensa: ejecuta el camino que tú decidiste. Su virtud es que es aburrido y predecible — y eso, en atención al cliente, es una virtud, no una limitación."* |
| **Qué construye** | El **flujo A** del hilo guiado: disparador *cuando llega una respuesta del formulario* → extraer idioma y tema → consultar **su propio asistente, el del M2** → bifurcar si es negativo y grave → añadir fila + avisar sólo si es grave |
| **Duración** | 2 semanas |
| **Capacidad y cómo se hace transferible** | **Flujo con disparador por suceso.** Los tres conceptos —disparador, paso, condición— son los mismos en todos los constructores de flujos que existen, y ése es el hecho que hace este módulo agnóstico: se enseñan como vocabulario del oficio, con el nombre del producto sólo en el apéndice. El criterio de elección también es portátil y se enseña como tal: **automatiza donde ya viven tus datos**, y **cuándo eso deja de ser la respuesta correcta** (cuando el flujo tenga que tocar algo fuera de tu suite: el software de gestión académica, la pasarela de pago, WhatsApp Business, el portal de una agencia) |
| **Los límites, por delante y no por sorpresa** | Va en la primera página del módulo: **los flujos de su entorno fallan con unidades y carpetas compartidas** [V], un solo disparador por flujo, y el administrador puede tener pasos restringidos sin que ella lo sepa. Como el centro de gravedad de su puesto **es un buzón compartido**, los primeros flujos se construyen sobre **su propio buzón y sus propias copias**. Descubrirlo en la lección 1 en vez de en el tercer intento fallido separa un material honesto de uno que la frustra |
| **Cómo se autocorrige** | (a) **Ejecución real**: se dispara o no. (b) **La batería, columna nueva** — y la lectura correcta es la contraintuitiva: *si la calidad ha mejorado respecto al M2, sospecha: probablemente reescribiste el criterio por el camino*. (c) **Lista de comprobación de plataforma** de 8 ítems binarios, que además sirve de diagnóstico cuando algo falla |

---

### 3.7 M5 · Prepara, no envíes

| | |
|---|---|
| **Cambio mental** | *"Automatiza la lectura y la preparación; la escritura hacia fuera la firma una persona."* Y la razón, que no es prudencia sino diseño de aprendizaje: **si el artefacto sólo prepara, todos sus errores son recuperables, y por eso puedes permitirte equivocarte mucho — que es lo que hace falta para aprender** |
| **Qué construye** | El **flujo B, del hilo propio**: triaje del correo entrante (clasificar y etiquetar, **no responder a nadie**) o borradores para P01 con bifurcación *si no encuentra fuente → "responder a mano"*. Más: **lista de temas prohibidos** (E-06), **condiciones de parada**, **tope de volumen** (*si la lista supera N, no redactes nada y avísame*) y **cómo se apaga, probado de verdad** |
| **Duración** | 2 semanas |
| **Capacidad y cómo se hace transferible** | Ninguna nueva. Lo que se enseña —parada, tope, apagado, revisión humana— es **la parte del oficio que no depende de ninguna herramienta y que ninguna herramienta trae puesta**. Se formula con las preguntas 4 y 5: *¿qué puede tocar? ¿quién firma?*. Prueba de traducción del escalón 3: rellenar la ficha de cinco preguntas para dos constructores de flujos que no ha usado |
| **Cómo se autocorrige** | (a) **Rúbrica con criterios negativos**, cada uno con salida escrita obligatoria y sin "no aplica". (b) **Prueba del apagado**: se apaga de verdad. Un sistema que no sabes apagar no está terminado. (c) **Prueba ciega (EP-08)**: 5 respuestas suyas de hace meses + 10 borradores del sistema, sin marcas de origen, **barajadas por otra persona**, puntuadas con la ficha del M1. Desactiva de golpe fluidez, halo y sesgo del experimentador |
| **Comprobación que decide el módulo** | *La respuesta a "¿quién revisa antes de que salga?" es **una persona con nombre**. Si no hay nombre, no hay revisión.* Y: *si tu diseño permite que algo llegue a un cliente sin que alguien le dé a enviar, vuelve al principio* |

---

### 3.8 M6 · ¿Esto sirve de verdad?

| | |
|---|---|
| **Cambio mental** | *"Que el flujo se ejecute cada lunes no es que funcione."* **Evaluación de proceso ≠ evaluación de resultado** |
| **Qué construye** | (1) **El vigilante de plantillas (P32)**: comprueba el tarifario maestro contra las plantillas de cada idioma y lista las discrepancias. Ataca el riesgo *"alto y silencioso"* del inventario. (2) La **media página de evaluación** por sistema (EP-09): línea base vs. después, **por unidad de trabajo**, con el coste completo restado. (3) La **cadena causal en cinco flechas** (EP-14) con el eslabón subrayado que no depende de ella. (4) **La lista de lo que ha decidido NO automatizar, con el motivo** |
| **Duración** | 2 semanas |
| **Capacidad y cómo se hace transferible** | Ninguna herramienta. Una hoja de cálculo, a propósito. Es, con M1, el módulo cien por cien portátil: la línea base, el coste completo y las amenazas a la validez interna se aplican igual a un proceso de una academia que a uno de una fábrica |
| **Por qué el vigilante va aquí** | Porque este módulo cae en la frontera de abandono (§10) y no puede ser un módulo sin producto visible. El vigilante produce **una lista de errores reales que nadie sabía que existían**. Es el artefacto de mayor retorno visible del curso — y es, además, la materia prima del M7 |
| **Cómo se autocorrige** | (a) La comparación con la línea base del M0 es **aritmética**. (b) Rúbrica con tres prohibiciones duras: **prohibida la palabra "significativo"**; **obligatorio restar** revisión y mantenimiento; **obligatorio nombrar una amenaza a la validez interna que no puede descartar**. (c) Cláusula explícita: **si el saldo es negativo y aun así quiere conservarlo por otra razón (menos errores, menos carga mental, respuesta más rápida), es legítimo — pero entonces mide esa otra razón**. (d) La rúbrica de la lista de descartes declara: **un módulo en el que todo acaba automatizado está mal resuelto** |

---

### 3.9 M7 · Que lo adopten — *módulo lateral* (desarrollado entero en §6)

| | |
|---|---|
| **Cambio mental** | *"El ahorro se nota en la oficina, en silencio; el fallo se nota en internet, en público. Lo que no se hace visible, organizativamente no existe — y no por vanidad: porque nadie puede adoptar lo que no ve."* Y el segundo: **la adopción se diseña antes, no se vende después** |
| **Qué construye** | (1) **La página de resultados**, una cara, escrita para quien no ha visto nunca el sistema. (2) **El manual de una cara** del artefacto: qué hace / qué **no** hace / cómo se apaga / quién lo mantiene / cuándo se revisa. (3) **Una entrega real a una persona con nombre**, en el sitio donde esa persona ya mira. (4) **La medición de adopción a las dos semanas** |
| **Duración** | 2 semanas · **~1–1,5 h propias por semana**, la mitad que los demás, porque escribir media página sobre tu propio resultado y enseñársela a una compañera **es tiempo de trabajo** |
| **Capacidad y cómo se hace transferible** | Cero dependencia de herramienta y cero dependencia de empresa: es el módulo que más limpiamente se lleva a otro empleo. Lo que enseña —jerarquía de evidencia, coste de adopción cero, dueño con nombre, deuda de mantenimiento— no tiene fecha de caducidad |
| **Cómo se autocorrige** | **La adopción se comprueba, no se valora.** A las dos semanas: *¿alguien lo ha usado sin que se lo pidieras? SÍ/NO*. Es mecanismo 1 —ejecución real— aplicado a personas. Y si es NO, la rúbrica no dice "vuelve a intentarlo": **obliga a elegir cuál de las cinco causas fue** (§6.5), que es donde está el aprendizaje |

---

### 3.10 M8 · Juicio dentro del flujo — y qué es un agente

| | |
|---|---|
| **Cambio mental** | Dos. (1) *"Un agente no es una automatización mejor: es una automatización que **ha renunciado a ser predecible** a cambio de poder afrontar casos que no previste. Esa renuncia se paga, y hay que pagarla a conciencia y sólo donde compensa."* (2) **El riesgo no es el del día 1, es el del día 60**: sesgo de automatización. *La confianza no es una salvaguarda* |
| **Qué construye** | (1) Un flujo que **se bifurca según un criterio que ella definió y sabe justificar**, con reglas de escalado. (2) El fichero **Mapa de lo que existe**, escrito por ella (§7). (3) **La rúbrica de su propio artefacto** — el desvanecimiento completo del andamiaje. (4) La **ficha de cinco preguntas aplicada a una herramienta que el curso no ha enseñado** |
| **Duración** | **3 semanas**, no 2. Es la frontera más dura y se le da aire |
| **Capacidad y cómo se hace transferible** | La capacidad es **meter juicio en un punto concreto de un camino fijo**, y su criterio de uso es el mismo en cualquier producto: *juicio sólo donde el camino se bifurca por una razón que no puedes escribir de antemano*. La conclusión honesta, dicha sin disculparse: **su escalón 4 real es "un flujo con juicio en dos o tres puntos", no "un agente autónomo"**, y la barrera no es técnica ni suya: es de **licencia**, de **permisos** y de **datos** |
| **Cómo se autocorrige** | (a) **La batería, última columna**, ahora con **casos límite nuevos escritos por ella**. (b) **La rúbrica la escribe ella**; el curso sólo trae la lista de comprobación *de la rúbrica*: ¿tiene 3 criterios negativos? ¿cada uno exige salida escrita, sin "no aplica"? ¿hay umbral de "listo" formulado como condiciones de fallo? (c) **Lectura de la hoja de anclas completa**: una frase por columna diciendo qué aportó ese escalón. Si no puede escribirla para alguna columna, ese escalón no le aportó nada y merece la pena saberlo |

---

### 3.11 M9 · Cerrar y dejarlo vivo · M10 · Lo que hay más arriba

**M9 (semana 20).** *"Esto no termina cuando se acaba el material; termina cuando tú escribes los
criterios y sabes cuándo hay que volver a mirar."* Construye el **cuaderno de mantenimiento** (qué se
revisa, cada cuánto, quién), la hoja de anclas con su próxima fecha de pasada, su versión de la página
*"Cuando no coincide"*, y las tres cosas siguientes **con su condición de disparo** (*"haré X cuando
ocurra Y"*), no con una fecha. Autocorrección: la definición de "terminado" fijada en la semana 1 y
observable — **tres artefactos vivos que usa sin que el curso se lo pida, más una rúbrica escrita por
ella**.

**M10 (apéndice de lectura, sin entregable).** Herramientas de tipo terminal y sus equivalentes: qué
son, cuándo ganan de verdad (procesar decenas de ficheros locales de forma repetida — revisar 200
contratos de estancia larga buscando cláusulas), y por qué hoy no. **Si termina el curso sin abrirlo,
el curso ha funcionado igual**, y eso va escrito en su primera línea.

---

## 4. LA SEPARACIÓN CRITERIO / CLICS, EN LA PRÁCTICA

### 4.1 La convención, en tres registros y no en dos

Dos registros (criterio / clics) no bastan, porque dejan un hueco justo donde está el valor: **cómo
encuentras esa función en una herramienta que nunca has visto**. Por eso son tres.

| Registro | Qué contiene | Dónde vive | Caduca |
|---|---|---|---|
| **EL CRITERIO** | Por qué se hace así · qué problema resuelve · cómo se decide si toca · cómo se comprueba · qué puede salir mal | En la lección | **No** |
| **CÓMO RECONOCERLO EN CUALQUIER HERRAMIENTA** | Descripción funcional de lo que hay que buscar, y las señas que distinguen esta capacidad de otra que se le parece | En la lección, en caja aparte | **Casi no** |
| **LOS CLICS** | Rutas, nombres de botón, capturas, límites numéricos, precios | **En el apéndice, en otro fichero, con fecha** | **Sí, y da igual** |

### 4.2 Estructura de ficheros

```
curso/
  M2-2-leccion.md            ← criterio + señas. Ni una ruta de menú.
  ejercicios/E2-2.md
  rubricas/rubrica-E2-2.md
  claves/CLAVE-E2-2.md       ← sellada
  glosario-capacidades.md    ← el diccionario capacidad ↔ nombres de producto
  protocolo-ia.md
  cuando-no-coincide.md
apendice/
  clics/A-05-base-de-fuentes-citables.md    ← una por CAPACIDAD, no por lección
  datos-volatiles.md         ← todo número: cuotas, precios, límites
```

Los ficheros de clics se nombran **por capacidad y no por lección**, porque la misma capacidad se usa
en varias lecciones y así se actualiza en un solo sitio.

### 4.3 Las ocho reglas de redacción

1. **En "El criterio" no aparece ningún nombre de producto**, salvo una vez, entre paréntesis, la
   primera vez que se introduce la capacidad, y marcado como tal. Prueba: *si una frase deja de ser
   cierta porque una empresa renombró algo, la frase estaba mal escrita.*
2. **Toda capacidad tiene un nombre de curso**, y ése es el que usan las rúbricas, los ejercicios y la
   batería. El glosario traduce a nombres de producto, con fecha.
3. **Ningún ejercicio puede depender del apéndice para poder hacerse.** Prueba mecánica: se borra el
   directorio `apendice/` y se comprueba que todos los ejercicios siguen enunciables.
4. **Ningún número vive en el texto.** Cuotas, precios y límites, en `datos-volatiles.md`.
5. **Todo fichero de clics abre con su fecha de verificación** y con la frase: *"si no coincide con tu
   pantalla, tu pantalla tiene razón y este texto no"*.
6. **Los ficheros de clics tienen dos columnas siempre que se pueda**: su entorno y una segunda
   herramienta. La segunda columna no es un extra: **es lo que enseña la transferencia**, y es lo que
   convierte el apéndice en material del curso en vez de en muleta.
7. **Las capturas sólo en el apéndice**, nunca en el criterio, y nunca portantes.
8. **Regla del reemplazo:** el apéndice entero se puede sustituir por el de otra herramienta sin tocar
   una línea del curso. Se comprueba una vez, en el M8, y es un ejercicio.

### 4.4 El glosario de capacidades (extracto)

Este fichero es la separación hecha objeto. La columna 3 tiene fecha y se puede quedar obsoleta sin
que las columnas 1 y 2 se resientan.

| Nombre del curso | Qué es | Cómo se llama hoy en algunos sitios *(22.08.2026)* |
|---|---|---|
| **Instrucciones permanentes** | Contexto que se aplica a todas las conversaciones | instrucciones personalizadas · personalización |
| **Asistente guardado** | Instrucciones con nombre que se reabren sin reexplicar | Gem · GPT personalizado · proyecto |
| **Base de fuentes citables** | Corpus cerrado; responde sólo desde ahí y cita el fragmento | cuaderno · base de conocimiento · proyecto con ficheros |
| **Disparo por reloj** | Ejecuta una instrucción de forma recurrente | acciones programadas · tareas |
| **Proceso por lote** | Una instrucción aplicada a N unidades, resultado en columna | función de IA en la hoja |
| **Flujo por suceso** | Disparador + pasos fijos + condiciones | constructor de flujos · automatización sin código |
| **Punto de juicio** | Paso del flujo donde el sistema evalúa algo para elegir camino | paso de decisión · extractor · router |
| **Agente** | Le das objetivo y límites; los pasos los decide él | agente · asistente autónomo |

### 4.5 EJEMPLO REAL: las dos mitades de una misma lección

Se toma un fragmento corto de **M0.2 — "Bajo qué régimen trabajo"**, que es donde la separación se ve
mejor porque el contenido volátil es máximo. (El ejemplo largo, una lección entera con ejercicio,
rúbrica y solución, está en §11.)

---

#### MITAD 1 — lo que va en la lección

```markdown
## El criterio

Todo el ruido de marketing sobre planes se reduce a **cuatro preguntas**. Enseñarte las
preguntas vale más que enseñarte la tabla, porque la tabla caduca y las preguntas no.

1. **¿Entrenan sus modelos con lo que yo escribo?**
2. **¿Cuánto tiempo guardan mis conversaciones, y quién decide ese plazo?**
3. **¿Dónde se procesan y se almacenan los datos? ¿Puedo exigir que sea en la UE?**
4. **¿El proveedor firma como encargado del tratamiento?** Es decir: ¿hay un contrato
   por el que trata datos por cuenta de tu empresa y sólo siguiendo sus instrucciones?

Y una quinta que no es del plan, sino de tu empresa, y que suele ser la que decide de
verdad: **¿lo han activado y configurado, y han dejado dicho por escrito qué se puede
meter?**

Dos cosas que ordenan las respuestas y que no dependen de ningún producto:

- **Pagar resuelve quién es el proveedor, no qué tratamientos están amparados.** Que tu
  empresa tenga contrato con alguien no legitima que tú metas ahí un pasaporte.
- **La retención "indefinida" es una opción real y a menudo la que viene por defecto.**
  Si nadie la ha tocado, cada pegado descuidado es un depósito permanente.

**Cómo se comprueba sin depender de que te contesten.** El correo al administrador puede
no llegar nunca. Así que además hay una vía empírica, y es la misma en cualquier
herramienta: **buscar los indicadores que la propia pantalla te da**. Una herramienta de
empresa suele decirlo de alguna forma —un distintivo, una línea al pie, un aviso al
subir un fichero—. Tu tarea no es memorizar dónde está: es **saber que ese indicador
existe y buscarlo antes de pegar nada**.

Y una regla de decisión, para cuando la respuesta no aparezca: **sin indicador, trátalo
como cuenta personal.** No es paranoia: es la única regla que no falla cuando no sabes.
```

```markdown
## Cómo reconocerlo en cualquier herramienta

🧭 Busca, en este orden:

- **Un distintivo o etiqueta cerca de tu nombre de usuario o del título.** Es donde las
  herramientas de empresa suelen declarar el régimen.
- **Un aviso al subir un fichero por primera vez.** Suele ser más explícito que la
  configuración.
- **La página de privacidad de la propia herramienta, en su versión de empresa** — no la
  general, que es otra.

**Señas de que estás en una cuenta de empresa cubierta:** dice explícitamente que no se
usará tu contenido para entrenar · nombra un contrato o un anexo de tratamiento de datos ·
hay alguien de tu empresa que puede borrar tus conversaciones.

**Señas de que NO lo estás, aunque el logotipo sea el mismo:** el aviso habla de "mejorar
nuestros servicios" · te ofrece a ti el interruptor de entrenamiento (si el interruptor es
tuyo, el régimen es de consumo) · nadie de tu empresa puede ver ni borrar nada de eso.

→ **Clics: `A-01-regimen-de-la-cuenta.md`** · verificado 22.08.2026
```

---

#### MITAD 2 — lo que va en el apéndice, `apendice/clics/A-01-regimen-de-la-cuenta.md`

```markdown
# A-01 · Comprobar el régimen de tu cuenta

> **Verificado el 22.08.2026.** Si algo no coincide con lo que ves, **tu pantalla tiene
> razón y este texto no.** Ve a `cuando-no-coincide.md`.

| Paso | En tu entorno de empresa hoy | En la otra herramienta que ya usas |
|---|---|---|
| Entrar con la cuenta correcta | Comprueba arriba a la derecha que el correo es el de la academia y no el personal | Igual |
| Ver el régimen | Distintivo en la parte superior: **Pro**, **Expanded** o **Ultra** → no la revisan personas ni se usa para entrenar. **Sin distintivo** → acceso estándar: la pueden revisar personas | Ajustes → Controles de datos. Si el interruptor de "mejorar el modelo" es tuyo y puedes apagarlo, estás en régimen de consumo |
| Ver la retención | No es visible para ti. **Sólo desde la consola de administración.** Rango posible: de 90 días a **indefinido**, lo fija tu administrador | Chats borrados y temporales: 30 días |
| Ver la edición contratada | **Un usuario no administrador no puede consultarla** [V]. Consola → Facturación → Suscripciones, y hace falta privilegio de facturación. No hay atajo: se pregunta | — |

**Comprobaciones empíricas, por si nadie contesta.** Cinco cosas que se intentan y que la
pantalla contesta sola: si funcionan, tienes edición completa; si no, probablemente la
edición reducida. *(lista de las cinco, con la fecha de verificación)*

**Cifras y cuotas:** en `datos-volatiles.md`. Aquí no se repiten a propósito.

**Registro de cambios**
- 22.08.2026 · primera verificación.
```

---

**Qué demuestra este ejemplo, y es la prueba de que la convención funciona:** si mañana desaparecen los
distintivos, cambian los nombres de las ediciones o se renombra la consola, **se reescribe A-01 y no se
toca una coma de la lección**. Y si ella cambia de empresa a una que usa otra herramienta, la lección
sigue siendo válida entera y el apéndice se sustituye. Las cuatro preguntas y la regla *"sin indicador,
trátalo como cuenta personal"* le van a servir en 2029 exactamente igual.

---

## 5. QUÉ SE QUEDA FUERA A PROPÓSITO

### 5.1 Fuera porque el brief lo excluye

| Fuera | Por qué |
|---|---|
| **Un curso de la herramienta que usa hoy** | Es la corrección de brief más importante. Su entorno es donde practica, no el eje. Un curso de producto la deja atada a un producto, y ella quiere poder saltar sin fricción a lo que exista dentro de dos años |
| **Venta interna: "cómo conseguir el sí"** | En su empresa usar IA ya está bien visto y **lo mal visto es no automatizar**. Un módulo de venta interna resuelve un problema que no tiene. Lo que sí entra —evidenciar y contagiar— es otra cosa y está en el M7 |
| **Portfolio, landing, prototipo de app** | Es el destino del itinerario no técnico de la referencia porque **su alumno tipo quiere cambiar de sector**. La nuestra no. Aquí es ruido |
| **Certificado, insignia, "ahora eres AI Operator"** | No busca cambiar de rol. Y un certificado sin evaluador ni rúbrica no certifica nada |
| **Cualquier cosa vistosa** | El grafo de la demo de referencia es el caso de estudio: espectacular en pantalla, marginal en valor para atención al cliente. El artefacto útil aquí es aburrido: una base de respuestas con fuente y fecha, un triador, un vigilante de plantillas |

### 5.2 Fuera por criterio de escalera, con su condición de reentrada

Nada de esto desaparece: todo tiene su fila en el *Mapa de lo que existe*, con la condición que lo
devolvería al curso. Un "no" sin condición de revisión es dogma.

| Fuera | Reducido a | Condición para que entre |
|---|---|---|
| **Constructores de flujos de terceros como módulos** | **Una página** comparativa + el criterio *automatiza donde ya viven tus datos* | Que un flujo tenga que tocar algo fuera de su suite. El criterio de elección se enseña; el nombre del ganador, no |
| **Escribir código dentro de la suite** | **Media página** informativa | Que el constructor de flujos se quede corto **y** haya quien mantenga el script |
| **Las superficies de desarrollador (probadores de prompts, claves de API)** | **Cinco líneas, con aviso explícito** | Ninguna. Es la trampa más silenciosa del panorama: parece profesional, se entra con la cuenta corporativa, es gratis, y sus términos dicen que no metas información personal |
| **Conectores y estándares de conexión modelo↔herramienta** | **Vocabulario + el principio de privilegio mínimo**, que sí transfiere | Que monte algo fuera de su suite, o que alguien se lo configure y ella sólo lo use |
| **Arquitecturas de base de conocimiento (recuperación, grafos, incrustaciones)** | **Una fila del mapa** | Que las fuentes pasen de decenas a cientos y el corpus empiece a perderse |
| **Herramientas agénticas de escritorio y terminal** | **M10, lectura, sin entregable** | Una tarea con decenas de ficheros locales, repetida en el tiempo |
| **Agentes de navegador y asistentes autónomos** | **Una fila del mapa** | Un cambio de plan de la empresa. Es barrera **de dinero, no de capacidad** |

### 5.3 Fuera por criterio de rigor mal invertido

- **Estadística inferencial.** Nada de significación, valor p ni tamaño muestral sobre doce casos. Aquí
  no se estima un parámetro poblacional: se comprueba la cobertura de un instrumento contra un criterio
  fijado. **Doce casos bien elegidos valen más que doscientos al azar.**
- **Consistencia interna aplicada a la batería.** Directamente incorrecto: una batería **debe** ser
  heterogénea. Si tuviera consistencia interna alta sería porque está mal construida.
- **Comparativas de modelos, *benchmarks* y nombres de modelo.** *"Da bastante igual qué modelo uses."*
  El material no se apoya en ningún nombre de modelo, a propósito: es el detalle que menos importa y el
  que más rápido caduca.
- **Prompt engineering como colección de trucos.** Sustituido por la ficha de criterio: el problema no
  es la fórmula del prompt, es que nadie escribió qué cuenta como respuesta correcta.
- **Vídeos de lección.** Un vídeo es relectura con mejor producción, y la relectura está clasificada
  como técnica de utilidad baja. Si hay vídeo, es demostración de una interfaz, dura menos de tres
  minutos, va con transcripción — **y vive en el apéndice**, porque una ruta de menús caduca.

### 5.4 Fuera por riesgo

P08 visados · P26 quejas formales · P29 emergencias · P25 reembolsos · P17 matching · P05/P16
nivelación y exámenes. No son "temas avanzados": son **zona prohibida con motivo escrito** (§7.2), y el
motivo es lo que se enseña, porque es lo único que se transfiere a un caso nuevo.

---

## 6. EL MÓDULO DE EVANGELIZACIÓN INTERNA — M7 · «Que lo adopten»

### 6.1 Dónde va, y por qué exactamente ahí

**Semanas 15–16, inmediatamente después del módulo de medición.** Tres razones:

1. **Antes no hay nada que evidenciar.** Evangelizar sin un artefacto vivo y un número honesto es
   exactamente el hype que la referencia denuncia, y ella lo detectaría al instante. El módulo se
   apoya en tres cosas que ya existen para entonces: un flujo funcionando desde el M4–M5, una media
   página de evaluación con línea base y coste completo del M6, y **un hallazgo** — la lista de
   plantillas desactualizadas que el vigilante del M6 produjo y que nadie de la academia sabía que
   existía.
2. **Cae justo donde el material solo ya no tira.** El tramo de las semanas 13–16 es la travesía del
   desierto de cualquier curso: la novedad se agotó y los conceptos se abstraen. La recompensa que
   funciona ahí no es otro artefacto: es que **otra persona use algo suyo**. Es el mejor combustible
   disponible en el peor punto de la curva, y ninguna otra parte del diseño puede aportarlo.
3. **No depende de ninguna herramienta ni de ningún permiso**, así que es el módulo más robusto ante
   un bloqueo de plataforma. Si el administrador le ha capado algo, éste se puede hacer igual.

**Y por qué es lateral y no columna vertebral.** No abre ninguna puerta de la escalera, ningún módulo
posterior consume su salida, y **si el calendario se tuerce, M8 se hace antes**. Esa reversibilidad es
la prueba estructural de que no es el eje: un módulo que se puede mover sin romper nada no es la
columna vertebral de nada.

### 6.2 Qué NO es este módulo — escrito primero, porque es lo que sale solo

| No es | Por qué |
|---|---|
| **Pedir permiso o autorización** | No le hace falta. En su empresa usar IA ya está bien visto y **lo mal visto es no automatizar** |
| **Pedir presupuesto o proponer comprar algo** | Todo lo que ha montado cuesta cero. Pedir dinero cambia la conversación entera y no hace falta |
| **Una presentación a dirección** | Una presentación es un evento; la adopción es un hábito. Y una presentación sin usuario real es una demo |
| **Portfolio, landing, "mira lo que sé hacer"** | Fuera por brief: no quiere cambiar de rol ni de sector |
| **Convencer a nadie de que la IA es buena** | Ya están convencidos. El problema del brief es el contrario: **empujan con desconocimiento de lo que se puede hacer**. Lo que falta no es entusiasmo, es información realista |
| **Prometer lo que la herramienta no hace** | En un entorno ya inflado de expectativas, **la credibilidad es el activo escaso**, y se gasta una sola vez |

### 6.3 Lo que sí enseña — cinco piezas

**Pieza 1 · La asimetría, que es el motivo y no la excusa.**
`dominio-rgpd.md` §7.4 lo formula así y sirve tal cual: *el ahorro se nota en la oficina, en silencio;
el fallo se nota en internet, en público*. Consecuencia organizativa, y es dura: **el valor que no se
hace visible no existe para la empresa**, y quien lo produjo carga con los riesgos sin ninguno de los
beneficios. Hacer visible el resultado no es autobombo: es la única forma de que la organización pueda
decidir sobre algo que ahora mismo no ve.

**Pieza 2 · La jerarquía de la evidencia.**
Qué cuenta y qué no, ordenado. Esto es contenido de primera y se enseña como tal:

| Nivel | Evidencia | Por qué pesa lo que pesa |
|---|---|---|
| **1** | **Otra persona usa el artefacto sin ti** | Es un hecho observable, no una afirmación tuya. No admite réplica |
| **2** | **Un hallazgo que nadie sabía** — *"la plantilla alemana lleva siete meses mandando el precio del año pasado"* | Cambia el marco: no vienes a contar lo que ahorras, vienes con un problema real que has encontrado |
| **3** | **Minutos por unidad, con línea base y coste completo restado** | Es un número, pero un número honesto y con su amenaza declarada. Sobrevive a que lo repregunten |
| **4** | Una demo | Impresiona y se olvida. Vale sólo si termina en el nivel 1 |
| **5** | *"Me ahorra muchísimo tiempo"* | **Vale cero.** Es exactamente lo que dice todo el mundo y por eso ya no significa nada |

Y la regla que ordena la redacción de todo lo que escriba: **una afirmación interna tiene que
sobrevivir a tres preguntas escépticas seguidas.** Se enseña haciendo: coge tu frase, escríbete las
tres preguntas más incómodas que te haría alguien que no te cree, y contéstalas **dentro** de la media
página. Aquí su formación es ventaja directa: las tres preguntas incómodas son, casi siempre, las
amenazas a la validez interna que ya nombró en el M6 (*"¿no será que en noviembre hay menos volumen?"*
= historia; *"¿no será que has mejorado tú?"* = maduración).

**Pieza 3 · La demo de tres minutos, con la regla del caso real.**
- Se demuestra con **un caso de la semana pasada, elegido delante**, no con uno preparado. Un caso
  preparado no convence a nadie que haya visto alguna demo antes, y en 2026 todo el mundo las ha visto.
- **Se enseña también dónde falla**, y qué salvaguarda lo cubre. Contraintuitivo y cierto: mostrar el
  fallo es lo que convierte una demo en algo creíble, y es además la única forma de que la persona que
  lo adopte sepa dónde mirar.
- **Se termina siempre igual**: *"si quieres, te lo dejo montado para lo tuyo y te paso la hoja de
  cómo se usa"*. Sin esa frase, la demo es entretenimiento.

**Pieza 4 · La adopción se diseña antes, no se vende después.** Cuatro criterios, y son los que hay
que aplicar **al elegir el proyecto**, no al final:

1. **Que el dolor lo sienta otra persona además de ella.** Candidatos naturales del inventario: P30
   (parte semanal → dirección académica, que ya lo pide), P32 (plantillas → quien lleva admisiones y
   marketing), P27 (encuestas → dirección académica y el sello de calidad).
2. **Coste de adopción cero.** El resultado se entrega **en el sitio donde esa persona ya mira** —su
   buzón, la reunión del lunes, el documento que ya abre— y **no** en una herramienta nueva a la que
   tenga que entrar. Si adoptar exige que alguien aprenda algo, no se adopta. Esta regla sola explica
   la mayor parte de los proyectos internos que mueren funcionando perfectamente.
3. **El eslabón que no depende de ti, identificado antes de construir.** Es EP-14, la cadena causal en
   cinco flechas, usada aquí para lo que sirve de verdad: *el sistema produce un informe, pero el
   cambio depende de que alguien lo lea y actúe*. **Ese eslabón es la adopción**, y hay que diseñarlo,
   no esperarlo.
4. **Un dueño con nombre y una fecha de revisión.** Si nadie es el dueño, el artefacto muere en la
   primera semana en que ella esté de vacaciones.

**Pieza 5 · La deuda de adopción, y el riesgo de acabar siendo "la de la IA".**
Es la parte que ningún material de este tipo incluye y que en una empresa de 30 personas donde lo mal
visto es no automatizar **va a pasar**:

- **No entregues lo que no puedas mantener.** Todo lo adoptado tiene coste de mantenimiento, y lo paga
  ella. Un flujo que se rompe en julio, cuando entran 400 correos al día, no es valor: es un problema
  que ella misma se ha creado y encima con público.
- **Entrega el artefacto y el manual, no el servicio.** La frase que marca el límite y conviene tenerla
  escrita: *"esto lo monté yo y así se mantiene; si quieres uno para lo tuyo, aquí está cómo se hace"*.
- **El bus factor invertido:** si es la única que sabe cómo funciona, la organización no adopta el
  artefacto, **la adopta a ella**. El manual de una cara es la contramedida, y por eso es entregable.
- **Conexión con el límite de rol de protección de datos [!]:** el riesgo de este perfil —ser la que
  más se preocupa y acabar siendo de facto la responsable de cumplimiento— tiene aquí su versión
  gemela. Se nombra en los dos sitios y con la misma regla: *tu papel no es hacerte cargo de todo; es
  no ser tú el agujero y saber cuándo levantar la mano*.

### 6.4 Qué produce

| # | Artefacto | Formato | Prueba |
|---|---|---|---|
| **1** | **Página de resultados** | Una cara. Qué hacía antes · qué hace ahora · el número con su línea base y su coste restado · **la amenaza que no puedo descartar** · el hallazgo | Sobrevive a las tres preguntas escépticas, escritas y contestadas dentro |
| **2** | **Manual del artefacto** | Una cara. Qué hace · **qué NO hace** · cómo se apaga · quién lo mantiene · cuándo se revisa | Otra persona lo usa sin preguntarle nada a ella |
| **3** | **Una entrega real** | A **una** persona con nombre, en el sitio donde ya mira | Ocurrió, con fecha |
| **4** | **Medición de adopción** | Dos semanas después: *¿lo ha usado alguien sin que se lo pidieras?* SÍ / NO | Observable. No admite interpretación |

### 6.5 Cómo se autocorrige sin mentor — y es el módulo donde más importa

**La adopción se comprueba, no se valora.** Ésa es la decisión de diseño. La pregunta de las dos
semanas es binaria y externa: no depende de su juicio sobre su propio trabajo, que es justo el punto
ciego que la literatura sobre autoevaluación describe.

Y si sale **NO**, la rúbrica no dice "inténtalo otra vez": obliga a **elegir cuál de las cinco causas
fue**, con una frase de evidencia:

| # | Causa | Cómo se reconoce | Arreglo mínimo |
|---|---|---|---|
| **1** | **Coste de adopción** | Tuvo que entrar en algo, aprender algo o cambiar de sitio | Llevar la salida a donde esa persona ya mira |
| **2** | **Entregado en el sitio equivocado** | Lo recibió en un canal que no consulta, o en una reunión donde no era su turno | Cambiar el canal, no el artefacto |
| **3** | **No resolvía un dolor suyo** | Al preguntarle, describe otro problema distinto | Es el fallo más común y el más útil: **el proceso elegido era el tuyo, no el suyo** |
| **4** | **No se entendía sin ti** | Te preguntó algo que estaba en el manual, o no lo abrió | El manual es demasiado largo o está escrito para quien ya sabe |
| **5** | **No hubo dueño** | Nadie sabía si era suyo | Volver con un nombre y una fecha de revisión |

**Y una sexta lectura, legítima y que hay que escribir para que no se lea como fracaso:** que la
adopción no ocurriera porque **el artefacto no debía adoptarse**. Un sistema que sólo tiene sentido con
ella delante puede ser perfectamente correcto como herramienta personal. Reconocerlo es un resultado,
no una derrota.

**Punto de consulta PC-5 aquí** (§9): su pareja es el evaluador ideal de la página de resultados
precisamente porque **sabe de IA y no conoce la academia** — que es exactamente la posición desde la
que la va a leer un compañero escéptico. La pregunta que lleva es cerrada: *"¿qué pregunta me harías
después de leer esto que yo no sé contestar?"*.

**Casos satélite del módulo:** convertir en página de resultados un artefacto que **no** funcionó, y
uno del que **no** tiene línea base. Los dos enseñan lo mismo por caminos distintos: qué se puede
afirmar honestamente con lo que tienes, que es la competencia de fondo.

---

## 7. «SABER QUÉ EXISTE» SIN CATÁLOGO MUERTO, Y CÓMO SE ENSEÑA A NO USAR IA

### 7.1 El catálogo se construye por descarte documentado, no por enumeración

Existe **un único fichero vivo**, `mapa-de-lo-que-existe.md`. No se lee: **se rellena**, una fila cada
vez que algo aparece por ser relevante para una decisión suya. Y —éste es el cambio respecto al
borrador anterior— **las filas son capacidades, no productos**, con los productos relegados a una
cuarta columna que puede quedarse obsoleta sin invalidar la fila.

| Qué es, en una frase mía *(dura)* | Por qué hoy no me toca *(dura)* | Qué tendría que pasar *(dura)* | Ejemplos hoy *(caduca)* |
|---|---|---|---|
| Un servicio de fuera que conecta aplicaciones entre sí | Lo que ya tengo hace lo mismo dentro de mi suite, gratis, sin meter otro proveedor entre mis datos y yo | Que necesite tocar algo que está fuera de mi suite: el software de gestión académica, la pasarela de pago, WhatsApp | *(nombres, 08.2026)* |
| Un sistema al que le das objetivo y límites y él decide los pasos | Los de verdad están detrás de planes caros, y mi trabajo vive en un buzón compartido que mi herramienta no puede tocar | Que la empresa contrate otro producto, o que aparezca una tarea cuyos pasos no pueda dibujar de antemano | *(nombres)* |
| El estándar por el que un modelo se conecta a una herramienta o fuente | Para mí hoy es vocabulario, no herramienta. Lo que sí me sirve es el principio: **conectar sólo a lo necesario** | Que monte algo fuera de mi suite, o que alguien técnico me lo configure y yo sólo lo use | MCP |
| Escribir un programa dentro de la suite, con la IA ayudando | Es código aunque lo escriba la IA, y el día que falle hay que leer un error de programador | Que el constructor de flujos se quede corto **y** haya quien mantenga el script | *(nombres)* |
| El sitio donde se prueban prompts con la clave de la API | Sus propios términos dicen que no metas información personal, y se entra con la cuenta de la empresa: **parece seguro y no lo es** | **Nada.** Es una superficie de desarrollador | *(nombres)* |
| Agente de escritorio con acceso a mis ficheros | No resuelve mejor ninguno de mis 32 procesos, está fuera del estándar de mi empresa y sale de mi bolsillo | Una tarea que exija procesar decenas de ficheros locales de forma repetida | *(nombres)* |

**Cuatro propiedades que hacen que esto no muera:**

1. **La tercera columna convierte el catálogo en criterio.** Un catálogo dice qué hay; la condición de
   disparo dice **bajo qué circunstancia cambiaría mi decisión**, y las circunstancias no se renombran.
2. **Cada fila se escribe en el momento en que se toma la decisión que la descarta**, no en un módulo
   de panorama. La fila de "agente" se escribe en el M8, cuando ya tiene un flujo con juicio y entiende
   exactamente qué le falta.
3. **La escribe ella, en su lenguaje.** Y es evaluable: la lista de comprobación pregunta *¿hay alguna
   fila cuya tercera columna esté vacía? SÍ/NO* — una condición vacía significa descarte por desgana.
4. **Segunda vuelta en M9:** se relee y se marca **qué condiciones han cambiado** en cinco meses. Eso
   convierte el catálogo en un instrumento con vida, y es además el ensayo de lo que tendrá que hacer
   sola cada año.

### 7.2 Cómo se enseña a NO usar IA — seis mecanismos, ninguno es un sermón

**1 · El escalón −1 existe en el árbol de decisión, y va antes que todo lo demás.**
Antes de "¿chat, automatización o agente?" hay una pregunta anterior: **"¿esto necesita un modelo de
lenguaje?"**. Su versión memorable, y cabe en una línea: **la prueba de la servilleta** — *¿podrías
escribir los pasos en una servilleta y valdrían siempre? Entonces necesitas una fórmula, una plantilla
o un calendario.* El presupuesto (P02) es aritmética sobre una tabla; la hoja de camas (P22) es un
calendario de recursos.

**2 · El caso canónico se trabaja entero y se mide.** El presupuesto se monta **con IA** y **con
fórmula**, sobre los mismos veinte casos, cronometrado y con los errores contados. Gana la fórmula por
goleada. **Enseñar el "no" haciendo el "sí" y midiendo que pierde es infinitamente más fuerte que
prohibirlo**, y de paso es el ejemplo del árbol de decisión con sus datos y no con los de una agencia
de marketing polaca.

**3 · La regla del cuatro** *(tomada del borrador 2, y es su mejor idea)*: **de sus doce tareas
candidatas, al menos cuatro tienen que acabar en "ni IA", "arreglar el proceso primero" o "zona
prohibida". Si tiene menos de cuatro, no ha clasificado: ha hecho una lista de deseos.** Su
justificación es empírica —cruzando los 32 procesos con lo que la plataforma puede hacer, el reparto
real da entre cinco y siete noes de doce— y su función es psicológica: convierte el "no" en algo que
hay que **encontrar**, no en algo que hay que evitar. Y desactiva el sesgo que produce un curso de IA
por su mera existencia: preguntarle a un curso de IA si algo debe hacerse con IA tiene un sesgo obvio
hacia el sí.

**4 · Las zonas prohibidas, con el motivo y no sólo la prohibición**, porque una prohibición sin motivo
no se transfiere a un caso nuevo:

| Proceso | Por qué no, dicho de forma transferible |
|---|---|
| **P08** carta de aceptación para visado | Riesgo crítico y **normativa viva**: cambia de un año para otro. **Congelar dentro de un prompt un conocimiento que caduca es fabricar un error futuro** |
| **P26** quejas formales | Una respuesta que **admite responsabilidad por escrito compromete a la empresa**. Y los modelos son complacientes: la complacencia por escrito, en una queja, es exposición legal |
| **P29** emergencias 24 h | Personas, menores, responsabilidad civil, y un alumno en shock con nivel A1 |
| **P25** reembolsos | Datos bancarios y riesgo de fraude por suplantación |
| **P17** matching con familia de acogida | Concentra **salud, religión y potencialmente orientación sexual** en una casilla de texto libre. Es el proceso que **más parece** el caso ideal de IA, y por eso es la trampa |
| **P05 / P16** nivelación y exámenes | *Evaluar el nivel educativo* está en la lista de alto riesgo del Reglamento de IA. Aplazado, **no cancelado**. Lo suyo no es decidirlo **[!]**: es reconocerlo y avisar |

Y la regla de oro que lo hace memorable: **de todo su proceso, el único trocito que está en la lista de
alto riesgo es el que decide el nivel de un alumno. Todo lo demás —redactar, traducir, resumir,
clasificar— no lo está.** Esa asimetría se recuerda; una lista de artículos, no.

**5 · El coste completo como criterio de descarte.** *Un flujo que ahorra ocho minutos y cuesta diez de
revisión es una pérdida disfrazada de modernidad.* Y la métrica de vanidad tiene nombre: **que el flujo
se ejecute cada lunes no es que funcione**.

**6 · La opción segura suele ser la más eficiente, y hay que demostrarlo.** El mejor ejemplo, en el M2:
**no transcribas la llamada.** Escribe tú un resumen de cuatro líneas al colgar, ya seudonimizado, y
trabaja con ése. Es más rápido que subir un audio de doce minutos, no genera un tratamiento nuevo ni un
destinatario nuevo, y de paso piensas el caso. Enseñado así, "no usar IA" deja de ser una renuncia y
pasa a ser una decisión de eficiencia.

---

## 8. PROTECCIÓN DE DATOS: DÓNDE VA Y POR QUÉ AHÍ

**Principio: esto no es un módulo.** Un módulo de protección de datos se lee una vez, se aprueba y se
olvida — y además produce parálisis, cuando el objetivo es que **use más la IA, no menos: que la use en
el sitio correcto**.

Va en **tres capas**, y cada una aparece en el momento en que **desbloquea** lo siguiente en vez de
frenarlo. Y —esto es lo que lo hace estructural y no anexo— **las preguntas 4 y 5 de la ficha de
escalón son protección de datos**: *¿qué puede tocar? ¿quién firma la salida?*. No se puede clasificar
una herramienta sin contestarlas.

| Capa | Dónde | Qué contiene | **Por qué exactamente ahí** |
|---|---|---|---|
| **1 · Qué tengo y qué no se pega** | **M0, sesiones 1–3** | Las cuatro preguntas que definen un régimen · cuenta de empresa vs. personal · el **semáforo** verde/ámbar/rojo · la línea limpia entre su chat personal y la herramienta de empresa | **Es la semana en que va a empezar a pegar cosas.** Todo lo demás se construiría sobre un suelo que no ha mirado. Y el diagnóstico es útil por partida doble: del régimen depende también **qué funciones existen** |
| **2 · Seudonimizar de verdad y adjuntos** | **M2, antes de cargar las fuentes** | Por qué "quitar el nombre" no basta; cuasi-identificadores; la **prueba de la compañera**; los adjuntos (la hoja va **completa**, con las pestañas ocultas; el PDF del pasaporte va entero; las fotos llevan GPS); *si no lo has abierto y leído entero, no lo adjuntas* | **Es el momento exacto en que pasa de pegar texto a subir ficheros.** Al pegar ves lo que envías; al adjuntar, no. Ahí cambia el orden de magnitud del riesgo |
| **3 · Salvaguardas de un sistema que actúa** | **M5, antes del segundo flujo** | Temas prohibidos; condiciones de parada; *nada sale al cliente sin que un humano le dé a enviar*; **el deber de avisar de que es una IA** cuando el cliente interactúa con el sistema; registro de qué se generó y quién lo aprobó; el plan para el día que falle, incluido **valorar si hay brecha [!]** | **Es cuando algo empieza a actuar sin que ella mire cada paso.** Antes del M5 no hacía falta; después sería tarde |

**Capa 0, permanente:** la **tarjeta del lunes** impresa al lado de la pantalla desde la semana 1, seis
preguntas que caben en una nota adhesiva. *Si una regla necesita que te pares a pensar, no sobrevive a
un martes de julio con 300 correos.*

**Cuatro decisiones que hacen que esto funcione y no asuste:**

1. **La regla de los menores es tajante y sin excepciones**, más restrictiva de lo que la norma exige
   en todos los supuestos, **a propósito**: *si hay un menor implicado, sus datos no entran en ninguna
   herramienta de IA, ni seudonimizados*. Una regla con excepciones no sobrevive a julio.
2. **Cada decisión que no es suya va marcada [!] y con el nombre de a quién se escala.** El riesgo de
   este perfil es acabar siendo de facto la responsable de cumplimiento. El material lo prohíbe.
3. **Nada normativo se congela dentro de un prompt.** Fechas y estados normativos viven en un fichero
   de contexto **con fecha visible** que se revisa. Y es el mejor ejemplo pedagógico del curso de la
   diferencia entre conocimiento estable y conocimiento volátil — la misma distinción que gobierna la
   separación criterio/clics.
4. **El encuadre no es de permiso, es de aportación.** No pide autorización: ya usa la herramienta, se
   la ha dado su empresa, y usarla está bien visto. Está entendiendo la configuración antes de
   apoyarse en ella. Si la academia nunca se lo ha planteado, **acaba siendo ella quien propone la
   política** — y eso no es venta interna: es su propio trabajo.

**Y el dato que cambia la posición mental con la que se estudia esto, en la primera página:** el
Reglamento de IA obliga desde febrero de 2025 a las empresas que usan IA a garantizar un nivel
suficiente de **alfabetización en IA** de su personal. Dicho de otro modo: **el curso que está haciendo
es, técnicamente, cumplimiento normativo de su empresa.**

**La parte agnóstica y la parte de entorno, separadas como todo lo demás:** las cuatro preguntas, el
semáforo, la prueba de la compañera, la regla de adjuntos y las salvaguardas **son el criterio y no
caducan**. Las tablas comparativas de planes, los distintivos y los plazos de retención concretos son
apéndice fechado.

---

## 9. LOS PUNTOS DE CONSULTA CON SU PAREJA

**Presupuesto: 6 consultas de 10 minutos en todo el curso.** Un curso que reserve "consultas
ilimitadas" obtiene en la práctica cero, porque cada consulta compite con la comodidad de no molestar y
pierde. Uno que reserve exactamente seis, con nombre y momento, obtiene seis.

**Filtro de admisión**, impreso en la portada de la bitácora. Si falla cualquiera de las cuatro, no es
punto de consulta: (1) ¿lo resuelve el material? (2) ¿lo resuelve la IA con el protocolo de siete
reglas? (3) ¿lo resuelve **mirar**? (4) ¿lo he intentado 25 minutos y he anotado qué probé?

**Ficha de cinco campos escrita ANTES**, máximo una cara: la pregunta en una frase **cerrada** · mi
hipótesis y qué esperaría ver · qué he probado ya y qué pasó · **el dato concreto** (el error literal,
las dos respuestas que se contradicen) · qué haré con cada respuesta posible. **Reglas de la
conversación:** los cinco primeros minutos sin pantalla · **él no toca el ratón** · sale con una frase
escrita en su propio lenguaje · **a los diez minutos se para, esté como esté**.

| # | Momento | Qué lleva | Por qué ahí y no en otro sitio | Si no está disponible |
|---|---|---|---|---|
| **PC-1** | Fin de **M0** (sem. 2) | *"He deducido que trabajo bajo el régimen X y que por tanto no puedo hacer Y. ¿Me equivoco?"* Con las comprobaciones empíricas hechas | Es **un hecho del mundo que el material no puede ver**, y un error aquí contamina el curso entero. Mejor relación consecuencia/coste de los seis | Asumir el escenario más restrictivo y anotar la suposición como pendiente |
| **PC-2** | Inicio de **M2** (sem. 5), antes de cargar fuentes reales | Su clasificación de **8 tipos de dato** en tres cajones (empresa / nunca / depende) + 3 casos seudonimizados: *"¿tú sabrías de quién hablo?"* | **La única decisión del curso con consecuencia externa irreversible**, y el momento es exacto: es cuando pasa de pegar texto a subir ficheros | Regla de máxima cautela: *si dudas, no entra*, y se anota |
| **PC-3** | Fin de **M2** (sem. 6), tras el cebo | *"Ésta es la corrección que hizo la IA de un trabajo con tres fallos plantados. Encontró dos. ¿Estoy leyendo bien lo que se le escapa?"* | **El de mayor apalancamiento.** No se revisa su trabajo: se revisa **su instrumento de corrección**, que usará cincuenta veces más | Pasar el cebo por dos modelos distintos y comparar |
| **PC-4** | **Comodín**, desde M4 (sem. 9) | Un fallo de plataforma, tras agotar la lista de comprobación y "Cuando no coincide" | Caso canónico de "diez minutos ahorran una tarde". **No tiene fecha a propósito**: saber que existe un comodín reduce el miedo a atascarse, que es un factor de abandono por sí mismo | Documentar el fallo, **rodearlo** con una solución manual y seguir |
| **PC-5** | **M7** (sem. 15–16) | *"Lee esta página de resultados como si no supieras nada de mi trabajo. ¿Qué pregunta me harías que yo no sé contestar?"* | **Encaje perfecto con lo que él es:** sabe de IA y **no conoce la academia**, que es exactamente la posición del compañero escéptico que va a leerla. Puede atacar el razonamiento aunque no pueda verificar los hechos — y el razonamiento es lo que hay que endurecer | Escribirse ella las tres preguntas más incómodas y contestarlas dentro de la página; y pasarla por dos modelos con la instrucción de falsar |
| **PC-6** | **M9** (sem. 20) | *"Esto es lo que tengo funcionando. ¿Qué es lo siguiente que tendría sentido, y qué tendría que cambiar para que mereciera la pena?"* | Cierra con una orientación que no puede darse sola y evita el "final sin final" | La tercera columna del *Mapa de lo que existe* y la segunda vuelta del inventario |

**Cambio deliberado respecto al borrador anterior, y conviene justificarlo.** Allí había un punto de
consulta dedicado a *"¿dónde moverías la frontera entre lo que automatizo y lo que no?"*. Aquí ese
juicio se resuelve con un **mecanismo** —la regla del cuatro, los descalificadores por número de
proceso y la rúbrica que declara mal resuelto un módulo donde todo acaba automatizado— y el punto se
reasigna al M7. **Sustituir una consulta por un mecanismo es siempre mejor en un curso sin mentor**: el
mecanismo está disponible las cincuenta veces siguientes y la consulta sólo una.

**Lo que NO es punto de consulta**, escrito para que no se erosione: revisar un entregable (*"¿está bien
mi asistente?"* → rúbrica y batería), explicar un concepto (→ material), enseñarle a hacer algo (→
documentación), dar ánimos. Y la tentación específica de esta configuración: **que él le monte algo
"que es un momento"**. Eso no es una consulta: es un artefacto que ella no sabrá mantener ni depurar, y
en el escalón siguiente será deuda.

**Un uso de otra persona que NO gasta punto:** barajar las respuestas de la prueba ciega del M5 y
guardar la clave. Cinco minutos, función mecánica, vale cualquier compañera de la academia.

---

## 10. LOS TRES MOMENTOS DE MAYOR RIESGO DE ABANDONO

Criterio de selección: probabilidad × irreversibilidad de la conclusión que saca. Principio
transversal: **toda contramedida se escribe antes del punto de caída, no en él.** El modo mínimo
redactado la semana en que ya falló se lee como excusa; redactado en la semana 1, como plan.

---

### MOMENTO 1 · Días 1–14 — el arranque y el hueco del diagnóstico

**Qué pasa por dentro.** El 52 % de los inscritos en un curso autodidacta **nunca llega a empezar**, y
la caída mayor está en los días 7–14 [E]. Aquí se acumulan tres cosas: la fricción de arranque; el
diagnóstico depende de un correo que puede no contestarse nunca, y **esperar sin poder avanzar es la
forma más eficiente de abandonar**; y el beneficio todavía es abstracto mientras el coste ya es real.

**Qué se pone justo antes:**

1. **La sesión 1 no explica el curso: produce un resultado utilizable en 20 minutos** con lo que ya
   tiene abierto, sin instalar nada y sin hablar con nadie. Instrucciones permanentes + un correo real
   hecho con ellas + minutos cronometrados antes y después. **El mapa del curso va después del primer
   resultado.**
2. **El contrato de una página, escrito antes de empezar:** 20 semanas · 2 h semanales de tiempo propio
   · **0 €** · nada que instalar · nada que pedir a nadie · y **la definición observable de
   "terminado"**. Un curso que se anuncia de 8 semanas y dura 20 se percibe como fracaso propio en la 9.
3. **El diagnóstico no puede bloquear.** La vía empírica está en la misma página que el correo, no en
   un anexo. Y la rúbrica declara explícitamente que *"pregunté a X el día D y no obtuve respuesta"*
   **es un resultado válido**.
4. **El modo mínimo y el ritual de reentrada, redactados en la semana 1:** una micro-sesión de 10
   minutos cuenta como semana cumplida; toda vuelta tras una pausa empieza leyendo las tres últimas
   entradas de la bitácora y respondiendo las cinco preguntas de repaso.
5. **PC-1 al final de la semana 2**: otra persona implicada en el punto de máxima mortalidad.

---

### MOMENTO 2 · Semanas 9–10 — el primer bloqueo que no es culpa suya

**Qué pasa por dentro.** Es el riesgo específico de este diseño y el que más me preocupa. El
constructor de flujos de su entorno **falla con unidades y carpetas compartidas** [V]. El centro de
gravedad de su puesto **es un buzón compartido y una hoja de camas compartida**. Es decir: la primera
vez que intente automatizar su trabajo de verdad, la herramienta le va a decir que no. Y la conclusión
que se saca no es *"me he equivocado de carpeta"*, es **"esta herramienta no sirve para mi trabajo"** —
y detrás, *"este curso no sirve para mi trabajo"*. Esa conclusión es irreversible si no se anticipa.

**Qué se pone justo antes:**

1. **La limitación va en la primera página del módulo, con nombre y por escrito**, no en una nota al
   pie. *"Tu buzón `info@` es compartido. Los primeros flujos se montan sobre tu propio buzón y sobre
   copias tuyas, y eso no es una versión de juguete: es la restricción real de la herramienta."*
2. **La lista de comprobación de plataforma, 8 ítems binarios, entregada antes del primer flujo** y
   reutilizable como diagnóstico. Convierte un bloqueo en una comprobación con resultado, que es lo
   contrario de un veredicto sobre uno mismo.
3. **La página "Cuando no coincide"**, escrita una vez y referenciada desde cada lección. Esto convierte
   la caducidad de las herramientas —un defecto— en **una competencia enseñada**, que es justo lo que
   necesita alguien que va a seguir usando esto cinco años después.
4. **PC-4, el comodín, cuya existencia se anuncia mucho antes de que haga falta.**
5. **La caja "si nada de esto funciona": documenta el fallo, rodéalo con una solución manual y sigue.**
6. **Y la salvaguarda estructural: ningún módulo posterior depende de que el constructor de flujos esté
   habilitado.** El M3 ya le dio una automatización funcionando sin él. Si el administrador lo tiene
   bloqueado, M4–M6 se reencaminan con pérdida de comodidad y **cero pérdida de hilo**. El curso no
   puede tener un único camino que dependa de una casilla de una consola que ella no puede ver.

---

### MOMENTO 3 · Semanas 13–16 — la medición honesta y la entrega que puede no usarse

**Qué pasa por dentro.** Son dos golpes seguidos y por eso van juntos. Primero, el M6 puede darle la
peor noticia posible: **que el ahorro es pequeño**. Y llega en el punto donde la novedad se agotó y los
conceptos se abstraen. Segundo —y esto es un riesgo **nuevo, que introduce el módulo de adopción y que
hay que asumir**—: entrega su artefacto a una compañera y a las dos semanas nadie lo ha usado. Un
artefacto ignorado desmoraliza más que un artefacto que falla, porque el fallo se arregla y el silencio
no se sabe qué es.

**Qué se pone justo antes:**

1. **La automatización de mayor retorno visible se coloca aquí, no antes.** El M6 abre construyendo el
   **vigilante de plantillas**, que produce algo que ningún otro artefacto produce: **una lista de
   errores reales que nadie de la academia sabía que existían**. Es el momento en que su trabajo genera
   un hallazgo, no un ahorro. Y es, además, la mejor evidencia posible para el M7.
2. **La cláusula del resultado decepcionante, escrita antes de medir:** *si la medición dice que ahorras
   poco, eso es un resultado del curso y no un fracaso tuyo*. Y las razones legítimas alternativas están
   enumeradas de antemano —menos errores, menos carga mental, respuesta más rápida— con la instrucción
   de **medir esa otra razón** si es la que importa. La honestidad de la medición está protegida por
   adelantado, que es la única forma de que sea honesta.
3. **La primera entrega se elige por probabilidad de adopción, no por ambición.** El material lo impone:
   **una sola persona con nombre, que ya pide ese resultado hoy** (el parte semanal a dirección
   académica es el candidato canónico), **no** un envío a dirección ni a "todo el mundo". Se busca el
   sí más fácil, a propósito, porque el objetivo del módulo es aprender el mecanismo, no ganar la
   empresa.
4. **La no adopción está preinterpretada.** La rúbrica de las cinco causas (§6.5) convierte el silencio
   en un diagnóstico, y la sexta lectura —*puede que no debiera adoptarse*— está escrita antes de que
   ocurra. **Un fallo anunciado es una etapa; un fallo inesperado es un veredicto sobre uno mismo.**
5. **PC-5 exactamente aquí**, y su objeto —*"¿qué me preguntarías?"*— es intrínsecamente halagador de su
   trabajo sin ser halago: se conversa sobre criterio, que es lo que ya tiene.
6. **El M8 dura tres semanas, no dos.** Es el único módulo al que se le da aire, y se dice por qué.
7. **La lectura de la hoja de anclas completa** como primera sesión del M8: ver cinco columnas de su
   propio trabajo, con fecha, es la evidencia objetiva contra la ilusión de fluidez.

*(Se descarta como candidato el primer resultado mediocre del M2 —probable, pero su contramedida es
barata, conocida y ya está incorporada: la caja "Lo que vas a ver la primera vez".)*

---

## 11. UNA LECCIÓN COMPLETA, DESARROLLADA

Se desarrolla **M2.2**, la segunda sesión núcleo del escalón 1. Se elige porque es donde mejor se ve
la textura del curso entero y, sobre todo, **la separación criterio / clics**: la capacidad que enseña
—responder sólo desde un corpus cerrado, citando el fragmento— existe en todas las herramientas
serias con cuatro nombres distintos, así que el criterio es idéntico en todas y el apéndice es
puramente sustituible. Además concentra: dato real suyo, hilo guiado, corrección por comprobación
pura, una decisión de "cuándo NO", la capa 2 de protección de datos y la prueba de traducción.

---

### 11.1 La lección — `curso/M2-2-leccion.md`

```markdown
# M2.2 — Que sepa decir «no lo sé»

⏱ 45 min · Necesitas: tu ficha de criterio (EP-01) y los cuatro documentos que
elegiste como fuentes de verdad, cada uno con su fecha de última revisión.
Tipo de tiempo: [ mitad tiempo de trabajo | mitad tiempo propio ]

## Antes de leer nada — 5 minutos, de memoria y por escrito

1. En tu batería, ¿qué tiene que contestar el sistema en los 2 casos de rechazo, y
   qué cuenta como fallo aunque la respuesta esté bien redactada?
2. ¿Por qué «un modelo de lenguaje es el instrumento con la validez aparente más
   alta que vas a manejar»? Dilo con tus palabras.
3. De las cinco preguntas, ¿cuál es la que cambia de respuesta hoy?
4. Tu semáforo: el tarifario vigente, ¿de qué color es? ¿Y el correo del alumno que
   pregunta por el precio?
5. ¿Qué pasa si pegas una hoja de cálculo entera en vez de una copia limpia?

> Escribe lo que recuerdes ANTES de mirar. Equivocarte aquí es el ejercicio, no un
> fallo. Respuestas al final de la lección.

## Para qué sirve esto en tu trabajo

**P01, respuesta a solicitud de información.** Entre 5.000 y 8.000 al año, y entre el
70 % y el 80 % preguntan lo mismo: precio, fechas de inicio, niveles, si hay
alojamiento, si dais carta para el visado, si hay descuento por semanas. La
información es siempre la misma y está escrita; lo que cambia es el idioma, el tono
y el orden. Hoy la buscas tú, en cuatro documentos distintos, entre 200 correos.

Y el riesgo que hace que esto tenga que estar bien hecho y no sólo hecho: **un precio
mal citado por escrito se convierte de facto en una oferta que la escuela acaba
respetando** para no perder la reserva.

## El criterio        ← no caduca

**Tres cosas que los principiantes mezclan siempre, y que hay que separar antes de
montar nada.**

| | Qué es | Dónde vive | Ejemplo tuyo |
|---|---|---|---|
| **Fuente de verdad** | Un hecho, desde **una sola dirección** | Un documento con fecha | El tarifario vigente |
| **Memoria** | Un acuerdo que permanece entre conversaciones | Un fichero que tú controlas | «con las agencias siempre en inglés» |
| **Procedimiento** | La forma de trabajar: pasos y formato de salida | Las instrucciones del asistente | «responde en el idioma del correo, máximo 150 palabras, y cierra con las tres opciones de fecha» |

Confundirlas produce el error más común: meter el tarifario **dentro** de las
instrucciones. Funciona en enero y miente en marzo, porque las instrucciones no se
revisan y los documentos sí.

**1. Una base de fuentes citables no es «subir documentos». Son tres reglas.**

Lo que la convierte en un instrumento y no en un cajón:

- **Responde sólo desde ahí.** Si no está en las fuentes, no está.
- **Dice de qué documento sale cada dato.** No como cortesía: porque es lo que
  convierte tu revisión en cinco segundos en lugar de en una investigación — y esa
  diferencia es la que hace que la revisión se siga haciendo en julio.
- **Puede negarse.** «No lo sé» es una respuesta válida y deseable.

**2. La fecha es parte de la fuente.**

Un documento sin fecha de revisión es una afirmación sin fecha. Una base de fuentes
con las condiciones de cancelación del año pasado te responde con las condiciones del
año pasado, **con toda la confianza del mundo y citando el documento**. La cita no
protege de eso: la fecha, sí. El control de versiones de las fuentes es parte del
artefacto, no un detalle de orden.

**3. «No lo sé» no viene de serie, y hay que probarlo a propósito.**

Un sistema que nunca dice «no lo sé» no es que lo sepa todo: es que no lo has probado
bien. Por eso tu batería tiene **2 casos de rechazo**, y por eso el criterio de
aprobado es asimétrico: **una respuesta correcta a un caso de rechazo es un
suspenso**, por bien redactada que esté. Que acierte por conocimiento general en vez
de por tus fuentes es exactamente el fallo que quieres cazar, porque el día que se
equivoque lo hará igual de bien redactado.

**4. Dónde estás, en las cinco preguntas.**

| | Antes (M0–M1) | Después de esta lección |
|---|---|---|
| ¿Quién dispara? | yo, cada vez | yo, cada vez *(sin cambio)* |
| ¿Quién decide los pasos? | yo | yo *(sin cambio)* |
| **¿De dónde saca lo que sabe?** | **de lo que le pego** | **de fuentes que yo controlo y fecho** ← |
| ¿Qué puede tocar? | nada | leer lo que yo le doy |
| ¿Quién firma la salida? | yo, siempre | yo, siempre *(sin cambio)* |

**Una sola fila cambia.** Y esa fila es donde se gana la calidad de la respuesta. Todo
lo que viene después en el curso mueve las otras filas, no ésta — conviene que lo
sepas ya, porque es lo que te va a permitir juzgar cualquier herramienta futura sin
que te la vendan.

**Cuándo NO hacer esto.**

- Si la tarea la haces **tres veces al año**. Montar y mantener esto cuesta más que
  hacerlo a mano. El umbral honesto está en torno a una vez por semana.
- Si el conocimiento **cambia cada semana** o depende de una negociación. Congelar
  dentro de un sistema algo que caduca es fabricar un error futuro. Es exactamente la
  razón por la que las cartas de visado (P08) están en zona prohibida: no es que sean
  difíciles, es que la normativa cambia de un año para otro.
- Si no sabes **cuál de tus documentos es el vigente**. Entonces el problema no se
  arregla con IA: se arregla arreglando los documentos, y ése es un hallazgo real que
  vale la pena tener por escrito.

## Cómo reconocerlo en cualquier herramienta

🧭 **Qué estás buscando**, en palabras que no dependen de ningún producto: un sitio
donde se cree **un espacio con nombre**, se le adjunten documentos, y las respuestas
se limiten a ellos. Suele estar cerca de donde se guardan las conversaciones, o en un
apartado que hable de «proyectos», «cuadernos», «bases de conocimiento» o «fuentes».

**Las tres señas que te dicen que has encontrado la capacidad correcta:**

1. **Las fuentes siguen ahí mañana**, sin volver a subirlas.
2. **La respuesta dice de qué documento sale.** Si no cita, no es esto.
3. **Puedes listar qué hay dentro** y quitar una fuente sin rehacerlo todo.

**Si falta cualquiera de las tres, lo que tienes es un adjunto en una conversación**,
que es otra cosa y dura lo que dure esa conversación. Es la confusión más frecuente y
la que hace que la gente crea que ya tiene esto montado cuando no lo tiene.

**Señas de que la herramienta no sirve para este uso:** no permite quitar fuentes ·
mezcla lo que le has dado con lo que sabe de fuera sin distinguirlo · no hay forma de
ver cuántas fuentes hay.

→ **Clics: `apendice/clics/A-05-base-de-fuentes-citables.md`** · verificado 22.08.2026

## Ejemplo trabajado
*(Nivel de desvanecimiento del escalón 1: los dos últimos pasos van en blanco.)*

Las instrucciones del asistente, decisión a decisión:

    Eres quien prepara borradores de respuesta a personas que piden información
    sobre cursos de español.

    Responde ÚNICAMENTE con lo que esté en las fuentes adjuntas.
    Si el dato no está en las fuentes, escribe exactamente: NO LO SÉ — y nada más.

    En cada dato que des (precio, fecha, condición) añade entre corchetes el nombre
    del documento y su fecha: [tarifario 2026-09-01].

    Responde en el idioma del correo entrante.
    Máximo 150 palabras. Tono: <pegado de tus anclas de tono, EP-02>.

    Si el correo menciona visado, plazos consulares, una queja formal, salud o un
    menor: escribe solo DERIVAR A PERSONA y para.

    <PASO 5 — EN BLANCO>
    <PASO 6 — EN BLANCO>

| Decisión | Por qué ésta | Qué pasa con la otra |
|---|---|---|
| «ÚNICAMENTE con lo que esté en las fuentes» | Sin esa restricción rellena huecos con conocimiento general, que suena igual de bien y no está respaldado | Un precio plausible e inventado, indistinguible del bueno |
| «escribe exactamente: NO LO SÉ» | Una fórmula literal es **detectable**: puedes contar cuántas veces aparece | «Di que no lo sabes» produce párrafos amables que no se pueden contar |
| La cita **con la fecha del documento** | La cita sola no protege de una fuente caducada. La fecha, sí | Cita perfecta de un tarifario de hace catorce meses |
| «responde en el idioma del correo» | Es la mitad del trabajo real de P01 y es donde más tiempo se pierde | Contesta en español a una consulta en alemán |
| Lista de parada por tema | Coincide exactamente con tus procesos de riesgo crítico. **No es prudencia: es la lista del inventario** | Un sistema que opina sobre plazos de visado |
| **[PASO 5 — EN BLANCO]** ¿qué le dices que haga cuando el correo trae **tres preguntas** y sólo dos están en las fuentes? | | |
| **[PASO 6 — EN BLANCO]** ¿qué frase impide que el borrador se pueda enviar tal cual **por error**? | | |

## Antes de subir las fuentes — protección de datos, capa 2

Hoy pasas de **pegar texto** a **subir ficheros**, y ahí cambia el orden de magnitud
del riesgo por una razón simple: **al pegar ves lo que envías; al adjuntar, no.**

- Una hoja de cálculo va **completa**: todas las filas, incluidas las 900 que no estás
  mirando; todas las columnas, incluidas las ocultas; **todas las pestañas**, incluida
  la que se llama «datos antiguos».
- Un PDF de pasaporte va entero: foto, firma, lugar de nacimiento y la banda legible
  por máquina con todo repetido. **Documentos de identidad: nunca, en ninguna
  herramienta.** Si necesitas un dato de ahí, lo escribes tú a mano, y sólo ése.
- Las fotos llevan metadatos: fecha, hora y muy a menudo coordenadas.

**Regla:** *si no lo has abierto y mirado entero, no lo adjuntas.* Sin excepciones. Y
antes de subir cualquier hoja, **haz una copia y bórrale lo que no hace falta.**

**Tus cuatro fuentes de hoy son verdes**: tarifario, calendario académico, condiciones
generales y FAQ de visados **no son datos personales**. Es a propósito: la primera vez
que subes ficheros lo haces con material que no puede hacer daño.

## Lo que vas a ver la primera vez

Tres cosas, y ninguna significa que no funcione:

- **Va a citar un documento que sí existe pero que no contiene el dato.** Es el fallo
  más traicionero porque parece verificado. Se caza abriendo el documento y buscando
  la frase.
- **Va a contestar a alguno de tus 2 casos de rechazo**, y probablemente bien, porque
  la respuesta está en internet. Eso es un suspenso, no un aprobado.
- **Va a decir «NO LO SÉ» a algo que sí está en las fuentes**, porque lo has redactado
  con otras palabras que el documento.

Y una que no es del sistema: **es muy probable que descubras que no sabes con certeza
cuál de tus documentos es el vigente**, o que encuentres tres versiones. Eso no es un
fallo del ejercicio: es el primer hallazgo real del curso, tiene nombre de proceso
(P32) y va a acabar siendo un artefacto en el M6.

> *«Ves el resultado. Detrás hay varias decenas de intentos.»* — la referencia, en su
> mejor minuto.

## Tu turno
→ Ejercicio E2.2

## Cierre — 3 líneas en la bitácora
- Qué he producido: ______
- Qué ha fallado: ______
- Qué haré distinto la próxima vez: ______

---
### Respuestas de las 5 preguntas
```

---

### 11.2 El apéndice de clics — `apendice/clics/A-05-base-de-fuentes-citables.md`

Se reproduce entero para que se vea el contraste con la lección: **ni una sola frase de este fichero es
necesaria para entender nada; todas son necesarias para hacerlo hoy.**

```markdown
# A-05 · Base de fuentes citables

> **Verificado el 22.08.2026.** Si algo no coincide con lo que ves, **tu pantalla tiene
> razón y este texto no.** Ve a `cuando-no-coincide.md`.
> Cuotas y límites numéricos: en `datos-volatiles.md`. Aquí no se repiten.

| Paso | En tu entorno de empresa | En la otra herramienta que ya usas |
|---|---|---|
| Dónde se crea | Producto de cuadernos de la suite, con la cuenta de la academia | Apartado de proyectos, dentro de la conversación |
| Crear el espacio | Nuevo cuaderno → ponle un nombre que diga de qué es y para qué, no «pruebas» | Nuevo proyecto |
| Añadir fuentes | Subir fichero, o añadir desde el almacenamiento de la suite | Subir fichero al proyecto |
| Qué formatos acepta | Ver `datos-volatiles.md` | Ídem |
| Instrucciones fijas | Campo de instrucciones del cuaderno | Instrucciones del proyecto |
| Cómo se ve la cita | La respuesta trae marcas numeradas; al pulsarlas, salta al fragmento | Cita el nombre del fichero; no siempre el fragmento |
| Quitar una fuente | Panel de fuentes → seleccionar → quitar | Ídem |

**Diferencias que importan para el ejercicio, no para la nota:**
- La segunda columna cita el fichero pero **no siempre el fragmento**. Si es la que
  usas para la prueba de traducción, la seña 2 se cumple sólo a medias, y **eso es un
  hallazgo del ejercicio, no un problema**: anótalo en las tres líneas.

**Trampa conocida en tu entorno:** los ajustes de región de la organización **no se
aplican** a este producto de cuadernos. No cambia lo que puedes meter hoy (tus cuatro
fuentes son verdes), pero conviene saberlo antes de plantearse meter otra cosa.

**Si no encuentras el sitio:** vuelve a las tres señas de la lección y busca por ellas.
Si tu cuenta es de edición reducida, puede que el producto exista con menos capacidad;
compruébalo mirando la cuota diaria, no el nombre.

**Registro de cambios**
- 22.08.2026 · primera verificación. Nota: este producto fue renombrado en julio de
  2026; el nombre anterior aún aparece en la mitad de los tutoriales de internet, y
  ése es un buen ejemplo de por qué esta información vive aquí y no en la lección.
```

---

### 11.3 El ejercicio — `curso/ejercicios/E2-2.md`

```markdown
# E2.2 — Un asistente que cita, y una batería que lo suspende

⏱ 60–75 min · Hilo: **guiado (con clave)** · Tipo de tiempo: trabajo

## Lo que tienes que producir

Un asistente con nombre, apoyado en **cuatro fuentes fechadas**, que contesta las seis
preguntas que repite el 70–80 % de tus leads **citando el documento y su fecha**.
Más la **columna 2 de tu hoja de anclas**, rellenada y con la fecha de hoy.

## Criterios de éxito — obsérvalos, no los valores

Al terminar, esto tiene que ser cierto:
- [ ] Las cuatro fuentes tienen, **en el propio nombre del fichero**, su fecha de
      última revisión.
- [ ] Ninguna fuente es un fichero maestro: son **copias**, y les has quitado lo que
      no hacía falta.
- [ ] Existe **al menos una respuesta** en la que el sistema ha dicho NO LO SÉ.
- [ ] Cada dato numérico de las respuestas viene con su corchete de documento y fecha.
- [ ] La hoja de anclas tiene una columna nueva **con fecha**.

## Cómo lo vas a comprobar

Marca el nivel más alto que aplique — nunca uses uno inferior si hay uno superior:
- [ ] **Se ejecuta** → el asistente existe y responde.
- [x] **Batería de 10 casos con clave sellada** → `casos-M1.md` y `CLAVE-M1.md`, que
      escribiste en el M1 y **no has vuelto a abrir**. Ábrela ahora, después de
      anotar tus resultados.
- [ ] Lista de comprobación → abajo.
- [ ] Rúbrica + protocolo de IA → al día siguiente.

**Umbral de «listo», y es asimétrico a propósito:**
- 5 de 5 en los casos normales. Menos de 5 → no está listo.
- En los 3 límite, **pide aclaración**. Inventar una decisión es fallo **aunque
  acierte**.
- En los 2 de rechazo, dice **NO LO SÉ**. Cualquier otra cosa es suspenso, **incluida
  una respuesta correcta**.

## Antes de comprobar nada: escríbelo

> **Por qué lo he hecho así:** <3–5 líneas, en tus palabras>
> **Dónde creo que falla:** <1 línea>

Esto se escribe ANTES de corregir. Si lo escribes después, no sirve.

## Lista de comprobación (binaria y observable)

- [ ] ¿Cada fuente tiene fecha visible? SÍ / NO
- [ ] ¿Alguna fuente es el fichero maestro y no una copia? SÍ / NO
- [ ] ¿Hay una frase que diga qué hacer cuando falta un dato? SÍ / NO
- [ ] ¿La fórmula de negativa es **literal y contable**? SÍ / NO
- [ ] ¿Hay lista de temas que disparan parada, y coincide con tus procesos de riesgo
      crítico? SÍ / NO
- [ ] ¿He abierto **el documento citado** en al menos tres respuestas y encontrado la
      frase? SÍ / NO
- [ ] ¿He comprobado que ninguna fuente contiene datos personales? SÍ / NO
- [ ] ¿Hay alguna instrucción que contenga un **precio o una fecha** escritos dentro?
      (Debe ser NO: eso va en la fuente, no en las instrucciones.) SÍ / NO
- [ ] ¿He anotado el resultado en la hoja de anclas con la fecha de hoy? SÍ / NO
- [ ] ¿He pasado la **prueba de traducción** y escrito las tres líneas? SÍ / NO

## La prueba de traducción del escalón 1 (20 min)

Monta lo mismo en la otra herramienta que ya usas, con **dos** de tus cuatro fuentes.
Pasa **un caso normal y un caso de rechazo**. Escribe tres líneas:

- Lo que se llama igual: ______
- Lo que se llama distinto: ______
- Lo que esta herramienta no puede hacer y la otra sí: ______

> Si no consigues montarlo en 20 minutos, **para y anótalo**. No es un fracaso: es el
> dato. Significa que lo que aprendiste fue la ruta y no la capacidad, y toca volver a
> las tres señas de la lección.

## Si te atascas

1. Mira una respuesta que haya fallado y pregúntate: ¿el dato **estaba** en las
   fuentes? Si no estaba, el fallo es de fuentes, no de instrucciones, y se arregla en
   otro sitio.
2. ¿El fallo es de **formato** (no cita, no usa la fórmula literal) o de **criterio**
   (dice algo que no está)? Son dos problemas distintos y se arreglan en dos sitios
   distintos.
3. *(Tras 25 minutos de intento)* La solución comentada, con los seis fallos típicos.
> Las pistas se abren en orden, no de golpe.
```

---

### 11.4 La rúbrica — `curso/rubricas/rubrica-E2-2.md`

```markdown
# Rúbrica — E2.2

Se usa **al día siguiente**, nunca al terminar.
Encuadre obligatorio: *«reviso el trabajo de alguien que hace mi puesto y tengo que
decidir si se lo devuelvo».*

## Bloque 1 · Señales de fallo (obligatorio buscar y responder)

Por cada una: encuentra el caso, o **declara por escrito que has buscado y no existe**.
«No aplica» no es una respuesta admitida.

| # | Señal de fallo | ☐ | Dónde / por qué no |
|---|---|---|---|
| 1 | Existe una pregunta razonable de mi trabajo real que esto contestaría de dos formas distintas según el día. Escríbela | ☐ | |
| 2 | Hay una respuesta que **cita un documento que no contiene el dato**. (Comprueba tres citas abriendo el documento. Si no has comprobado ninguna, no puedes marcar esta casilla) | ☐ | |
| 3 | Hay una fuente **sin fecha**, o con una fecha que no sé si es la de revisión o la de creación | ☐ | |
| 4 | Hay algún dato dentro de este artefacto que, si se filtrara mañana, tendría que comunicar a alguien | ☐ | |
| 5 | Un dato que cambia —un precio, un plazo— está escrito **dentro de las instrucciones** en vez de en una fuente | ☐ | |
| 6 | El sistema ha contestado **correctamente** a un caso de rechazo. (Esto es un fallo, y de los graves: significa que responde desde fuera de tus fuentes) | ☐ | |

## Bloque 2 · Umbral de «listo»

NO está listo si se cumple **cualquiera** de éstas:
- Falla más de 0 de los 5 casos normales.
- Se inventa una decisión en alguno de los 3 casos límite en lugar de pedir aclaración.
- Responde algo distinto de NO LO SÉ en alguno de los 2 casos de rechazo.
- Alguna señal de fallo del bloque 1 está marcada y sin arreglar.
- No has abierto ni un solo documento citado para comprobar la cita.

## Bloque 3 · Si lo pasas por la IA

Protocolo completo en `protocolo-ia.md`. Las tres que más se olvidan:
**hilo nuevo · no digas que es tuyo · no discutas: abre otro hilo.**
Y una específica de hoy: pega **la ficha de criterio entera** junto con la rúbrica. Sin
ella, el modelo se inventa el estándar, y el estándar que se inventa es benévolo.

## Mi veredicto (lo firmo yo, no la IA)

[ ] Listo · [ ] Le falta: ______ · [ ] Lo dejo así y anoto por qué: ______
```

---

### 11.5 La solución comentada — `curso/soluciones/E2-2.md`

```markdown
# Solución comentada — E2.2

## Los dos pasos que estaban en blanco

**Paso 5 — la regla de la respuesta parcial.**

    Si el correo hace varias preguntas y sólo algunas están en las fuentes:
    contesta las que puedas, y para las demás escribe una línea que empiece por
    PENDIENTE: seguida de la pregunta tal cual la hizo la persona.

Por qué: la alternativa espontánea es que conteste lo que sabe y **calle lo demás**, y
un borrador que calla una pregunta es peor que uno que no contesta ninguna, porque
parece completo. La marca literal `PENDIENTE:` hace visible el hueco a la persona que
revisa en cinco segundos.

**Paso 6 — la línea que impide el envío accidental.**

    Empieza siempre el borrador con la línea: [BORRADOR — REVISAR ANTES DE ENVIAR]

Por qué: en el escalón siguiente esto va a acabar generando borradores en tu bandeja, y
la única salvaguarda que no falla es la que **hace visible** que algo no está firmado.
Es la versión mínima, hoy, de la regla que gobierna todo el escalón 3: *automatiza la
lectura y la preparación; la escritura hacia fuera la firma una persona*.

## Anatomía de los errores típicos

### Fallo 1 · «La fuente sin fecha»
- **Cómo se reconoce:** las respuestas son perfectas y las condiciones que cita son las
  del año pasado.
- **Por qué pasa:** subiste el documento que tenías a mano. Nadie pone fecha a un
  fichero que usa todos los días.
- **Arreglo mínimo:** la fecha **en el nombre del fichero**, no dentro. Se ve sin abrir.

### Fallo 2 · «El que nunca se niega»  ← el más importante
- **Cómo se reconoce:** 0 de 2 en los casos de rechazo, y las respuestas son correctas.
- **Por qué pasa:** le pediste que respondiera, no le diste permiso para negarse; y el
  dato estaba en su conocimiento general. **Que acierte no te salva**: significa que
  contesta desde fuera de tus fuentes, y el día que se equivoque lo hará igual de bien
  redactado. Es el mismo fallo que un clasificador que nunca dice «no lo sé».
- **Arreglo mínimo:** fórmula de negativa **literal**, y súbela al principio de las
  instrucciones. Y añade un tercer caso de rechazo a la batería: si sólo tienes dos, no
  estás midiendo esto, estás echándolo a suertes.

### Fallo 3 · «La cita decorativa»
- **Cómo se reconoce:** cita un documento que sí está entre tus fuentes, pero la frase
  no aparece en él.
- **Por qué pasa:** pediste que citara, no que **sólo afirmara lo citable**. Citar es
  producir un texto con formato de cita; verificarlo no es lo mismo.
- **Arreglo mínimo:** *«si no puedes señalar el fragmento exacto, no lo afirmes»*, y la
  rutina de abrir tres documentos citados al azar cada vez que cambies algo. **El 100 %
  de las veces que no encuentres la frase, era invención.**

### Fallo 4 · «El maestro subido entero»
- **Cómo se reconoce:** una de tus fuentes es la hoja de reservas o el listado de
  alumnos, y no una copia recortada.
- **Por qué pasa:** era el fichero que tenía el dato. Y la hoja va **completa**: filas
  ocultas, columnas ocultas y todas las pestañas.
- **Arreglo mínimo:** copia, borrar, subir la copia. Y la comprobación de la lista:
  *¿alguna fuente contiene datos personales? SÍ/NO*.

### Fallo 5 · «El cajón desastre»
- **Cómo se reconoce:** cuarenta fuentes, tres versiones del tarifario, y ya no sabes
  cuál está usando.
- **Por qué pasa:** añadir es gratis y quitar da miedo. Es el mismo mecanismo por el que
  la carpeta de plantillas de la academia tiene seis versiones de todo.
- **Arreglo mínimo:** **una sola fuente por hecho.** Si hay dos versiones, la vieja sale.
  Y si no puedes decidir cuál es la vigente, ése es el hallazgo: tienes un problema de
  proceso, no de IA.

### Fallo 6 · «La pregunta que ya trae la respuesta»
- **Cómo se reconoce:** tus casos de prueba dicen cosas como *«según el tarifario
  adjunto, ¿cuánto cuestan 4 semanas de intensivo?»*.
- **Por qué pasa:** al escribir los casos, escribes como quien sabe la respuesta. Es
  diseño de ítems con pista en el enunciado, y aquí es doblemente grave porque el caso
  real es un correo con faltas, en inglés, sin decir las fechas exactas.
- **Arreglo mínimo:** los casos son **correos reales, pegados tal cual**, seudonimizados.
  Si tu batería la pasa entera a la primera, **tu batería es fácil; no es que tu sistema
  sea bueno.**

## Lo que también sería correcto

- Tener **dos asistentes** —uno para leads y otro para alojamiento— en vez de uno con
  seis fuentes, si tus dos bloques de preguntas no se mezclan nunca. Más de mantener,
  pero cada uno más nítido.
- Poner el tono **en una fuente** en vez de en las instrucciones, si prevés que va a
  cambiar más que el procedimiento.
- No usar la herramienta de cuadernos y hacerlo todo con un asistente guardado con
  ficheros adjuntos, si tu edición no incluye la primera. **El criterio y la corrección
  son idénticos**, y el apéndice tiene la ruta. Que dos productos distintos sirvan para
  la misma capacidad es exactamente lo que este curso quiere que veas.

## Lo que parece correcto y no lo es

- **Pedirle que «sea riguroso y no invente».** Es una instrucción sin nada que
  comprobar. Suena a salvaguarda y no lo es. Lo comprobable es la fórmula literal de
  negativa y la cita con fragmento; lo demás es decoración.
- **Meter también las condiciones de las agencias.** Cada agencia tiene su tarifa neta y
  sus condiciones pactadas, distintas de las públicas. Mezclarlas con las públicas en el
  mismo espacio es fabricar el error más caro de tu inventario: **aplicar la tarifa
  pública a una agencia con tarifa neta**. Si lo necesitas, va en otro asistente, con
  otras fuentes.
- **Subir el histórico de correos «para que aprenda tu estilo».** Son datos de clientes,
  no son una fuente de verdad, y el estilo ya lo tienes anclado en EP-02 con tres
  ejemplos por nivel — que es más preciso y no mete a nadie dentro.
```

---

## 12. PRUEBA DE DURABILIDAD

**El método.** Recorro mi propio mapa de módulos y, por cada uno, marco qué quedaría obsoleto si dentro
de dos o tres años cambian los productos. Tres veredictos: **DURA** (sigue siendo cierto y útil) ·
**APÉNDICE** (caduca, pero está en el apéndice y se sustituye sin tocar el curso) · **ROMPE** (caduca y
además está en el cuerpo del curso, así que hay que rediseñar antes de entregar).

### 12.1 La tabla

| Módulo | Qué dura | Qué caduca | Dónde vive lo que caduca | Veredicto |
|---|---|---|---|---|
| **M0** | Las cuatro preguntas del régimen · el semáforo · la regla *"sin indicador, trátalo como cuenta personal"* · el inventario de tareas · la línea base · las instrucciones permanentes como capacidad | Distintivos, nombres de edición, plazos de retención concretos, rutas de la consola | `A-01` + `datos-volatiles.md` | **APÉNDICE** |
| **M1** | Todo. Ficha de criterio, anclas de tono, muestra apartada, tabla de especificaciones, batería | Nada | — | **DURA (100 %)** |
| **M2** | Fuente/memoria/procedimiento · las tres señas de la capacidad · la fecha como parte de la fuente · "no lo sé" contable · cita con fragmento · capa 2 de datos | Nombre del producto de cuadernos, cuotas de fuentes, formatos aceptados | `A-05` + `datos-volatiles.md` | **APÉNDICE** |
| **M3** | Disparo recurrente como capacidad · *un reloj no es un suceso* · libro de códigos · doble codificación · tabla de confusión · la prueba de la servilleta | Que exista una función de IA dentro de la hoja de cálculo, y cómo se escribe | `A-07` + ruta alternativa ya escrita | **APÉNDICE**, con una reserva (§12.2) |
| **M4** | Disparador / paso / condición como vocabulario · *automatiza donde ya viven tus datos* · la lista de comprobación de plataforma como método | Qué disparadores y pasos existen hoy, los límites de recursos compartidos, la comparativa de constructores | `A-09` + una página fechada | **APÉNDICE** |
| **M5** | Prepara-no-envíes · condiciones de parada · topes · apagado probado · temas prohibidos · prueba ciega · el deber de avisar de que es una IA | Dónde se configura la aprobación humana | `A-10` | **DURA (95 %)** |
| **M6** | Línea base · unidad por pieza de trabajo · coste completo · amenazas a la validez interna · proceso vs. resultado · cadena causal · lista de descartes | Nada | — | **DURA (100 %)** |
| **M7** | Jerarquía de evidencia · tres preguntas escépticas · coste de adopción cero · dueño con nombre · deuda de mantenimiento · las cinco causas de no adopción | Nada | — | **DURA (100 %)** |
| **M8** | Las cinco preguntas · qué se cede al ceder predictibilidad · juicio sólo donde el camino se bifurca por algo no escribible · sesgo de automatización y el riesgo del día 60 · rúbrica escrita por ella | **Qué agentes existen y por qué hoy están fuera de su alcance** | Cuerpo del módulo ⚠ | **RIESGO** (§12.3) |
| **M9** | Cuaderno de mantenimiento · condición de disparo en vez de fecha · segunda vuelta del mapa | Nada | — | **DURA (100 %)** |
| **M10** | El criterio de cuándo gana una herramienta agéntica de ficheros | Todo lo demás | Es lectura y está fechado | **APÉNDICE** |

**Recuento:** cinco módulos duran íntegros, cuatro tienen su parte perecedera fuera del cuerpo, y **uno
tiene un problema real**. Eso es aceptable, pero el uno hay que resolverlo, no anotarlo.

### 12.2 La reserva del M3

El M3 no depende de un producto, pero sí de que **exista una forma barata de aplicar una instrucción a
N unidades**. Hoy eso vive dentro de las hojas de cálculo; hace tres años no existía. Si desapareciera,
la capacidad no desaparece —el procesamiento por lotes es más viejo que los modelos de lenguaje— pero
la ruta fácil sí. **Mitigación ya prevista:** la ruta alternativa (mismo libro de códigos dentro del
asistente, en bloques) está escrita por delante para el caso de que su edición no la incluya, y esa
misma ruta cubre el caso de que el producto desaparezca. La lección se apoya en el **libro de
códigos**, que es lo que dura, y no en la fórmula.

### 12.3 El problema real: el M8 y la afirmación «los agentes están fuera de tu alcance»

**Es lo más probable que se falsifique en doce meses**, y está en el cuerpo del módulo, no en el
apéndice. Si los agentes de verdad bajan de precio, se meten en el plan que su empresa ya paga, o
aprenden a trabajar sobre buzones compartidos, el M8 quedaría diciendo una falsedad justo en el módulo
que corona el curso — y peor: una falsedad *desmotivadora*, del tipo "esto no es para ti".

**Rediseño, hecho antes de entregar y no anotado como pendiente.** Tres cambios en el M8:

1. **La afirmación deja de ser una conclusión y pasa a ser un resultado de la ficha.** El módulo no
   dice "los agentes están fuera de tu alcance": **le hace rellenar la ficha de cinco preguntas para el
   agente que tenga delante ese día**, y comprobar tres cosas concretas —¿lo cubre mi plan? ¿puede
   tocar los recursos compartidos donde vive mi trabajo? ¿puedo ver qué hizo?—. Si en 2028 las tres
   respuestas son sí, **el módulo funciona mejor, no peor**: le da luz verde con criterio.
2. **Lo que se enseña es qué se paga al ceder los pasos**, no quién vende agentes. Esa parte es la que
   dura, y es además la que hace falta el día en que sí pueda usarlos: cómo se acota el acceso, qué se
   verifica, dónde se pone la parada, y por qué la observabilidad —poder comprobar qué hizo— es el
   requisito que decide si un agente es utilizable, hoy y en 2030.
3. **La lista de barreras se convierte en las tres preguntas que las generan** (licencia, permisos,
   datos), con su condición de revisión escrita en el *Mapa de lo que existe*. Un "no" con condición de
   revisión envejece bien; un "no" sin condición envejece mal.

Con eso, el veredicto del M8 pasa de **RIESGO** a **DURA**, y el recuento final queda: **seis módulos
duran íntegros, cuatro tienen su parte perecedera aislada en el apéndice, ninguno rompe.**

### 12.4 Dos amenazas que no son de producto y que también hay que mirar

**(a) ¿Y si un solo producto acaba haciendo todos los escalones?** Es plausible: la tendencia es que la
misma ventana de chat programe, dispare por sucesos y actúe. Si ocurre, **la escalera no se rompe: se
vuelve más necesaria**, porque el producto deja de forzar la distinción y ya nada, salvo el criterio,
le dice a la persona cuánta autonomía acaba de ceder. La escalera pasaría de ser un mapa de productos
—que nunca fue— a ser lo único que queda para saber dónde estás. Las cinco preguntas se responden igual
dentro de una sola ventana.

**(b) ¿Y si los modelos dejan de alucinar y de necesitar fuentes citadas?** No hace falta apostar. El
M2 no enseña "cita porque alucina": enseña **cita porque tu revisión tiene que durar cinco segundos y
porque una fuente caducada responde con toda la confianza del mundo**. Ese segundo motivo no depende
de la calidad del modelo: depende de que los tarifarios cambien, y van a seguir cambiando.

**(c) El apéndice como riesgo de diseño, no de caducidad.** El peligro no es que el apéndice envejezca
—está previsto— sino que **se convierta en el curso de facto**, porque es donde está lo accionable. Las
tres defensas: ningún ejercicio se puede hacer desde el apéndice, ninguna rúbrica lo cita, y la prueba
de borrado (§4.3, regla 3) se ejecuta una vez sobre el material terminado. Si algún ejercicio deja de
poderse hacer, ese ejercicio estaba mal escrito.

---

## 13. AUTOCRÍTICA

Sin esta sección, las doce anteriores no son creíbles. Ordenado de más grave a menos.

**1 · El mandato agnóstico y el entorno de práctica tiran en direcciones opuestas, y no sé si mi
solución basta.**
El 90 % de sus horas van a transcurrir en una sola herramienta, porque es la que su empresa paga y la
que tiene delante. Mi respuesta —vocabulario de capacidades, tres registros, apéndice separable y una
prueba de traducción de veinte minutos por escalón, hora y media en total— es lo mejor que se me
ocurre que quepa en un curso de dos horas semanales. **Pero hora y media contra treinta y seis es una
proporción que no tranquiliza**, y no tengo forma de saber si es suficiente hasta que se pruebe. La
prueba de traducción convierte mi duda en un instrumento medible, que es lo mejor que se puede hacer
con una duda, pero sigue siendo una duda.

**2 · El problema del buzón compartido sigue sin resolver, y es la contradicción más seria del
documento.**
El constructor de flujos de su entorno no soporta unidades ni carpetas compartidas [V]. El buzón
`info@`, el buzón `accommodation@` y la hoja de camas —es decir, **el trabajo real de su puesto**— son
recursos compartidos. Mi respuesta de diseño es honesta (poner el límite por delante, montar sobre su
propio buzón) pero incompleta: es perfectamente posible que al final del M5 tenga dos flujos vivos
**sobre datos que ha copiado a mano**, que es exactamente el fracaso que este curso declara evitar. La
salida sería pedir al administrador una etiqueta o una carpeta propia dentro del buzón compartido, y
eso es una petición a otra persona, que es justo lo que el diseño prometía no necesitar. **No lo he
resuelto.** Lo heredo del borrador anterior y sigue igual de vivo.

**3 · El módulo de evangelización tiene la autocorrección más débil del curso, y lo sé.**
He hecho lo que se podía hacer: la pregunta de adopción es binaria, externa y no depende de su juicio
sobre su propio trabajo. Pero **la interpretación sí depende de ella**: elegir cuál de las cinco causas
fue el silencio de una compañera es un juicio social, con información parcial, sobre personas con las
que tiene relación. Y hay un modo de fallo que no cubro: que la adopción ocurra **por cortesía** —usan
su artefacto porque es ella— y el SÍ sea falso. La única mitigación es la medición a las dos semanas en
vez de a los dos días, y es débil.

**4 · Honrar la corrección (B) tiene un coste de secuencia que hay que pagar en voz alta.**
El curso pasa de 18 a 20 semanas, y he colocado un módulo lateral **delante del techo de la escalera**.
Si ella se detiene en la semana 16 —que es exactamente donde se detiene la gente—, **nunca llega al
escalón 4 ni al 5**, y el objetivo 1 del brief ("saber qué existe: agentes, automatizaciones") queda
peor servido de lo que estaría si M8 fuera antes. Lo he mitigado haciendo M7 explícitamente móvil y
declarando que si el calendario se tuerce M8 va primero. Pero **el orden por defecto es el que se
sigue**, y lo he elegido por razones de abandono, no de aprendizaje. Es una decisión discutible y
prefiero que quede escrita como tal.

**5 · El módulo de evangelización puede volverse en su contra, y no puedo probar la contramedida.**
En una empresa de 30 personas donde lo mal visto es no automatizar, hacerse visible como "la que sabe
de IA" tiene un desenlace muy previsible: que le caiga trabajo ajeno. He escrito la contramedida
—entregar el artefacto y el manual, no el servicio; la frase de límite; el bus factor invertido— y he
conectado el riesgo con el límite de rol de protección de datos. Pero es una contramedida de una
página contra una dinámica organizativa, y las dinámicas organizativas suelen ganar.

**6 · El diseño sigue dependiendo de un dato que no tengo.**
Si su entorno resulta ser la edición reducida, el M3 pierde su pieza más vistosa y varias funciones no
existen. Tengo contingencia escrita y la regla de que ningún módulo dependa del constructor de flujos,
pero **una contingencia no es lo mismo que un diseño**, y no se sabrá hasta la semana 2, con el curso
ya escrito. La única mejora respecto al borrador anterior es que ahora el golpe es menor: el M3 se
apoya en el libro de códigos y no en la fórmula, así que lo que se degrada es la comodidad, no el
contenido.

**7 · La batería como invariante es la mejor idea del diseño y la más frágil de mantener.**
Exige sostener diez casos vivos durante veinte semanas y volver a pasarlos cinco veces. Es poco trabajo
cada vez —media hora— pero es trabajo sin novedad, y lo que no tiene novedad se convierte en ritual o
desaparece. Si la batería se erosiona, **la salvaguarda 1 desaparece y el riesgo de los tutoriales
encadenados vuelve entero**. Las puertas la fuerzan, pero las puertas se pueden saltar en un curso sin
profesor.

**8 · La escalera ordena por autonomía cedida, no por dificultad del criterio.**
Es la crítica de fondo a mi propia tesis, y la mantengo del borrador anterior porque sigue siendo
verdad. Lo más difícil de todo lo que tiene que aprender —decidir qué **no** automatizar y saber si
algo funciona de verdad— no forma un escalón: va en capas. Las cinco salvaguardas lo hacen **visible**,
pero no lo hacen **primario**. Un diseño alternativo ordenado por criterio enseñaría mejor criterio,
enseñaría peor a usar herramientas y probablemente se abandonaría en la semana 4 porque no produce
nada durante un mes. **He elegido el diseño que se termina antes que el que enseña más.**

**9 · La verificación del objetivo 3 (datos) sigue siendo la más débil.**
Está bien cubierto como contenido y bien colocado en capas. Pero su comprobación depende de su propio
juicio sobre su propio material: elige ella los correos, elige ella los casos. El único contraste
externo es PC-2, diez minutos, una vez. Si sistemáticamente elige casos fáciles, la rúbrica no lo
detecta. He puesto la prueba de la compañera y el criterio de "al menos un correo rojo entero", pero es
una salvaguarda de muestreo y el muestreo lo hace ella.

**10 · El curso enseña a desconfiar del corrector que el propio curso usa.**
El protocolo de siete reglas y el cebo son lo mejor que tengo y son buenos. Pero el material le pide a
la vez que use la IA como correctora —porque no hay otra cosa— y que no se fíe de ella —porque falla en
la misma dirección en la que ella ya está sesgada—. Esa tensión está resuelta en el papel con
mecanismos, y no sé si está resuelta **en el mes cuarto, un jueves, cansada**. La respuesta honesta es
que no lo sé, y que la única forma de saberlo es que el cebo se repita una vez por escalón y que ella
misma vea si su criterio se ha degradado.

**11 · Nada de esto lo he visto.** Los 32 procesos, los volúmenes, el buzón compartido, la carpeta de
plantillas con seis versiones: todo es reconstrucción [R] a partir del sector, no observación de su
empresa. El curso está diseñado para que **su primera tarea sea tachar y corregir** ese mapa, que es la
única forma honesta de convertir mi reconstrucción en su realidad. Pero si el mapa está muy equivocado
—si su puesto se parece poco a lo reconstruido— el M0 tendrá que reescribirse sobre la marcha, y varios
ejemplos del material perderán fuerza precisamente por lo que se supone que los hace fuertes: por ser
concretos.
