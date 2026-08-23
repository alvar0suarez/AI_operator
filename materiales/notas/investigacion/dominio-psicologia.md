# Dominio — La formación en Psicología como ventaja operativa para especificar y evaluar sistemas de IA

**Para qué sirve este documento.** La licenciatura en Psicología de la alumna suele tratarse, en un
curso de IA, como un dato biográfico irrelevante o —peor— como material para un cumplido ("¡qué bien,
tú entiendes a las personas!"). Las dos cosas son un error. Hay un solapamiento **técnico, no
metafórico**, entre la metodología que se enseña en una licenciatura de Psicología y lo que hace falta
para especificar, probar y evaluar un sistema de IA. Este documento delimita ese solapamiento con
precisión: dónde es real, dónde es parcial, dónde no existe, y qué contenido de curso sale de cada
caso.

**Fecha:** 22.08.2026.

**Documentos con los que se acopla:**
`00-perfil.md` (encargo), `dominio-academia.md` (los 32 procesos, P01–P32), `dominio-rgpd.md`
(ejercicios E-01 a E-06 y el semáforo de datos), `dominio-herramientas.md` (la escalera 0→4 y las cinco
automatizaciones), `01-analisis-referencia.md` (los cinco pasos del programa polaco).

---

## Advertencia de método — la regla que gobierna todo el documento

Un curso que halaga con analogías falsas se cae en la primera contradicción. El día que la alumna
descubra que el alfa de Cronbach no tiene nada que decir sobre una batería de casos de prueba, dejará
de creerse también lo que sí era cierto. Por eso aquí **cada correspondencia va calificada**, y las que
no se sostienen se descartan por escrito en lugar de estirarse.

| Marca | Significado |
|---|---|
| **[FUERTE]** | Es la **misma operación** con otro nombre. Se puede enseñar diciendo literalmente "esto ya lo sabes hacer". La transferencia es directa y las técnicas concretas se aplican tal cual. |
| **[PARCIAL]** | El **problema** es análogo pero el **objeto** o el **mecanismo** son distintos. Transfiere el método, no la explicación. Hay que enunciar el límite en el mismo párrafo en que se enuncia el parecido. |
| **[FALSA]** | Suena bien y no es. Va en la sección 7 (falsos amigos) y **el material debe decir explícitamente que no aplica**, porque es analogía que alguien va a hacer sola si no se le corta antes. |
| **[!]** | Punto donde la decisión **no es suya**: se escala. Misma convención que `dominio-rgpd.md`. |
| **[NV]** | Afirmación no verificada en esta sesión. Ver sección 12. |

Y la segunda regla, que va dirigida al material y no a ella:

> **El curso no debe decirle "ya sabes de IA porque eres psicóloga". Debe decirle: "en estas siete
> cosas partes por delante de un ingeniero; en estas otras cinco empiezas de cero como todo el mundo,
> y una de ellas te va a costar más precisamente por venir de donde vienes".**

Sin la segunda mitad, la primera es adulación.

---

## 1. La tesis, en diez líneas

La mayoría de los proyectos de IA en atención al cliente no fracasan por la tecnología. Fracasan
porque **nadie escribió qué es una respuesta correcta antes de empezar**, porque **la prueba se hizo
con los mismos tres ejemplos que se usaron para escribir el prompt**, y porque **se aceptó una salida
mediocre que estaba bien redactada**. Los tres son problemas de medida, no de ingeniería.

Una licenciatura en Psicología es, en buena parte, un entrenamiento de cinco años en medir cosas que
no se dejan medir: definir un constructo difuso en indicadores observables, construir un instrumento,
comprobar que mide lo que dice medir, detectar los sesgos que introduce el propio procedimiento y
distinguir un cambio real de un artefacto de la medición.

Ese entrenamiento es exactamente el **paso 5 del método de referencia** ("evaluación de la calidad del
resultado"), que el propio webinar reconoce que casi ningún curso de IA incluye. Y buena parte del
paso 2 ("describir la tarea que delegas"), que es operacionalización pura.

Dicho de forma operativa: **el paso 5 no hay que enseñárselo, hay que traducírselo.**

---

## 2. Tabla maestra de correspondencias

| # | Psicología | Sistemas de IA | Grado | Escalón | Ejercicio |
|---|---|---|---|---|---|
| C1 | Operacionalizar un constructo | Escribir el criterio de "respuesta correcta" | **FUERTE** | 0–1 | EP-01, EP-02 |
| C2 | Validez de contenido · tabla de especificaciones | Que la batería de pruebas cubra el trabajo real | **FUERTE** | 1–2 | EP-03 |
| C2b | Validez de constructo · deficiencia y contaminación del criterio | Que la métrica mida lo que importa y no un correlato | **FUERTE** | 2–3 | EP-09 |
| C2c | Validez aparente | Trampa: el modelo la maximiza por construcción | **FUERTE** (como advertencia) | 1 | EP-05 |
| C3 | Fiabilidad test-retest e ítems ancla | Misma entrada / misma calidad; degradación al crecer o al cambiar de versión | **PARCIAL** | 1–2 | EP-04 |
| C3b | Acuerdo entre jueces (kappa) | Que la clasificación automática coincida con la suya | **FUERTE** | 2 | EP-07 |
| C3c | Consistencia interna (alfa) | — | **FALSA** | — | §7.2 |
| C4 | Diseño de ítems sin pistas · dificultad del ítem | Casos de prueba que no regalen la respuesta | **FUERTE** | 1–2 | EP-03, EP-06 |
| C5 | Sesgo de confirmación, halo, anclaje, fluidez | Por qué aceptamos una salida mediocre bien redactada | **FUERTE** | 1–3 | EP-05, EP-08 |
| C6 | Análisis de contenido · libro de códigos | Procesar texto libre de encuestas (P27) | **FUERTE** | 1,5–2 | EP-07, EP-10 |
| C7 | Línea base y diseño pre-post · amenazas a la validez interna | Demostrar que algo ahorra tiempo de verdad | **FUERTE** | 0 y 3 | EP-09 |
| C8 | Confidencialidad, disociación, minimización | Protección de datos | **PARCIAL** (con falsos amigos graves) | 0 | E-02/E-03 del doc RGPD |
| C8b | Consentimiento informado | Base jurídica del RGPD | **FALSA** | — | §7.4 |
| C9 | Entrevista semiestructurada · entrevista cognitiva | Levantar el contexto de la empresa preguntando a compañeros | **FUERTE** | 0–1 | EP-11 |
| C10 | Diseño de cuestionarios · sesgo de no respuesta | Que la encuesta de satisfacción no mienta | **FUERTE** | 2 | EP-12 |
| C11 | Estilos de respuesta culturales | Por qué un clasificador de sentimiento falla con alumnado asiático | **FUERTE** | 2 | EP-10 |
| C12 | Justicia organizacional (procedimental e interaccional) | Rúbrica de una respuesta difícil | **FUERTE** | 1–2 | EP-13 |
| C13 | Evaluación de programas · proceso vs resultado | "¿Esto resuelve de verdad el problema?" | **FUERTE** | 3 | EP-09, EP-14 |

Numeración de ejercicios: **EP-xx**, deliberadamente distinta de los **E-01…E-06** de
`dominio-rgpd.md` para que no colisionen cuando se monte el temario.

---

## 3. Las correspondencias, una por una

### C1 · Operacionalizar un constructo ↔ escribir un criterio medible de "respuesta correcta" — [FUERTE]

**Lo que es en Psicología.** Un constructo —ansiedad, motivación, satisfacción— no se observa. Se
define conceptualmente, se descompone en dimensiones, cada dimensión se traduce en indicadores
observables, cada indicador en ítems o conductas registrables, y se fija una regla de puntuación y un
punto de corte. Sin esa cadena no hay medida: hay opinión.

**Lo que es aquí.** "Una buena respuesta a un lead" (P01) es un constructo exactamente igual de
difuso. Y el prompt más elaborado del mundo no sirve de nada si nadie ha escrito qué cuenta como
buena. La cadena es la misma:

| Psicometría | Sistema de IA |
|---|---|
| Definición conceptual | "Una respuesta que permite al alumno decidir sin volver a escribir" |
| Dimensiones | exactitud del dato · completitud · idioma · tono · longitud · trazabilidad |
| Indicadores observables | "el precio coincide con el tarifario vigente"; "responde a las 3 preguntas del correo" |
| Regla de puntuación | sí/no por indicador |
| Punto de corte | "se envía si cumple los 4 críticos y al menos 2 de los 3 deseables" |

**Dónde la analogía se afina.** El primo hermano exacto **no es el test psicométrico de rasgo latente,
es la escala de anclajes conductuales (BARS) y la evaluación criterial**. En un test de rasgo, el
indicador es señal de algo que existe ahí fuera y que intentas estimar. Aquí no estimas nada: **decides**
qué va a contar como correcto. Es una norma, no un descubrimiento. Esa diferencia importa porque
elimina una pregunta que ella se va a hacer ("¿y cómo sé si mi criterio es el verdadero?"): no hay
criterio verdadero, hay criterio explícito y defendible, o no hay nada.

**Uso en el curso.** Es el primer artefacto de todo el curso y precede a cualquier herramienta.
Ninguna Gem, ningún flujo, ninguna automatización se monta antes de tener su ficha de criterio. Va en
el escalón 0–1 de la escalera de `dominio-herramientas.md`, pegado a la construcción de la primera Gem.

> **EP-01 · La ficha de criterio**
> Coge la tarea que hayas elegido en E-04 y escribe su ficha: definición en una frase, entre 4 y 6
> dimensiones, y para cada dimensión **un indicador que otra persona pueda comprobar sin saber qué
> tenías tú en la cabeza**. Añade la regla de decisión: qué es imprescindible y qué es deseable.
>
> *Autocorrección — está bien si:*
> - [ ] Ninguna dimensión usa las palabras **adecuado, correcto, natural, profesional o de calidad**
>       sin un ancla detrás. Si aparecen sueltas, no has operacionalizado: has renombrado el constructo.
> - [ ] Cada indicador se puede contestar **sí o no** mirando la salida y una fuente. Si necesitas
>       "depende", divídelo en dos indicadores.
> - [ ] Al menos un indicador es **verificable contra una fuente externa** (tarifario, calendario,
>       condiciones), no contra tu impresión.
> - [ ] Has marcado cuáles son **críticos** (un fallo tumba la respuesta entera) y cuáles no. Si todos
>       son críticos, no has priorizado; si ninguno lo es, el precio equivocado pesa lo mismo que una
>       coma.
> - [ ] La ficha cabe en una cara. Una rúbrica de dos páginas no se usa nunca.

> **EP-02 · Anclas conductuales para el tono**
> El tono es el constructo más difuso de su trabajo y el que peor se transmite a un modelo. Para dos
> dimensiones de tono (p. ej. *cercanía* y *firmeza*), escribe **tres anclas**: un ejemplo real de
> nivel bajo, uno de nivel medio y uno de nivel alto, tomados de correos que hayas enviado de verdad.
>
> *Autocorrección — está bien si:*
> - [ ] Las anclas son **frases completas**, no adjetivos.
> - [ ] La de nivel alto de *firmeza* sigue siendo una respuesta que enviarías a un cliente. Si no,
>       has anclado el extremo fuera de la escala útil.
> - [ ] Un compañero podría clasificar tres correos tuyos con tus anclas y coincidir contigo.
>
> *Producto reutilizable:* estas anclas **son** el fichero de contexto de tono del escalón 1. No es un
> ejercicio de calentamiento: es el entregable con el que se alimenta la Gem.

---

### C2 · Validez de contenido ↔ que la batería de pruebas cubra el trabajo real — [FUERTE]

**Lo que es en Psicología.** Validez de contenido = el conjunto de ítems representa el dominio
completo del constructo, en la proporción adecuada. El instrumento canónico es la **tabla de
especificaciones**: una matriz de áreas de contenido × niveles, con el número de ítems que toca a cada
celda. Y el procedimiento de control es el juicio de expertos (CVR de Lawshe, V de Aiken).

**Lo que es aquí.** Una batería de casos de prueba **es** un instrumento, y la enfermedad universal de
las baterías de prueba de IA es que se construyen con los casos que uno recuerda, que son los típicos
y los que ya funcionan. Resultado: un sistema que aprueba el examen y suspende el lunes.

**La tabla de especificaciones para su primer proyecto (P27, clasificación de comentarios de
encuesta)**, que es el ejemplo que hay que usar en el material porque es el proyecto real:

| | Típico | Límite | Debe rechazar / escalar |
|---|---|---|---|
| Académico | 3 | 2 | 1 |
| Alojamiento | 3 | 2 | 1 |
| Instalaciones | 2 | 1 | — |
| Actividades | 2 | 1 | — |
| Administración | 2 | 1 | — |

Con dos reglas que son las que hacen el trabajo:

1. **Los casos típicos van en la proporción real** de su buzón (el alojamiento y lo académico pesan
   más que las actividades). Eso es representatividad del dominio.
2. **Los casos límite NO van en proporción real: van por cupo fijo.** Son raros por definición y si se
   muestrean proporcionalmente desaparecen. Es la misma decisión que sobremuestrear un subgrupo
   pequeño para poder decir algo de él.

Casos límite concretos que deben estar en esa batería, salidos del dominio:

- comentario **mixto** con dos categorías y valencias opuestas ("el profesor genial, el piso sucio");
- **queja educada indirecta** ("quizá el desayuno podría mejorar un poquito") — ver C11;
- comentario **irónico**;
- comentario en un **idioma minoritario** de su mezcla real (coreano, turco, neerlandés);
- comentario **vacío de contenido** ("bien", "todo ok") que no debe inventar categoría;
- comentario que menciona un **dato de salud** → no se clasifica, se para (enlaza con E-06);
- comentario que **nombra a un profesor concreto** → dato personal de un empleado, no puede acabar en
  un informe con nombre;
- comentario sobre el **precio** que en realidad habla de expectativas creadas por la web, no del
  precio (ver C13 y el modelo de desconfirmación de expectativas).

**Uso en el curso.** Sustituye a la instrucción vaga de la referencia ("probar con al menos 5 casos:
correctos, límite y erróneos"). La referencia dice cuántos; la psicometría dice **de qué celdas**.

> **EP-03 · La tabla de especificaciones de tu batería**
> Antes de probar nada, dibuja la matriz categoría × dificultad de tu proceso y rellénala con casos
> **reales de tu buzón**, seudonimizados según E-03.
>
> *Autocorrección — está bien si:*
> - [ ] Hay al menos una celda con un caso que **el sistema debe rechazar** o derivar. Si tu batería
>       solo tiene casos que debe acertar, no estás midiendo: estás haciéndote una demo.
> - [ ] Los casos típicos respetan la proporción de tu trabajo real y los límite no.
> - [ ] **Ningún caso de la batería se usó para escribir el prompt.** Si lo hiciste, cámbialo (ver C4).
> - [ ] Puedes decir, para cada caso, cuál es la respuesta correcta **antes** de lanzarlo. Si no
>       puedes, ese caso no es una prueba, es una pregunta.

---

### C2b · Validez de constructo ↔ que la métrica mida lo que importa — [FUERTE]

Aquí la transferencia útil no es "validez convergente y discriminante" —eso pide correlaciones que
ella no va a calcular— sino un par de conceptos de psicología del trabajo que son exactamente el
problema y que casi nadie en el mundo de la IA sabe nombrar:

- **Deficiencia del criterio:** la medida deja fuera parte de lo que importa. Ejemplo suyo: mides
  "minutos por correo" y no mides que la respuesta rápida generó una segunda consulta. El ahorro es
  contable y falso.
- **Contaminación del criterio:** la medida recoge cosas ajenas al constructo. Ejemplo suyo: "el 90 %
  de los borradores se envían sin editar" no mide calidad; mide calidad **más** cansancio de las siete
  de la tarde de un lunes de julio. Un indicador que sube cuando ella está agotada no es un indicador
  de calidad.
- **Relevancia del criterio:** la parte que sí solapa. Es lo único que estás midiendo de verdad.

**Uso en el curso.** Es la vacuna contra la métrica de vanidad, y va en el escalón 2–3, cuando ya
tenga flujos vivos y empiece a querer contar lo que hacen. Es también la respuesta rigurosa a la
pregunta del webinar de referencia ("¿esto resuelve de verdad el problema de negocio?"), que allí se
formula sin método detrás.

---

### C2c · Validez aparente ↔ la trampa central de todo el curso — [FUERTE, como advertencia]

En psicometría, la **validez aparente** —que un instrumento *parezca* que mide lo que dice— es
explícitamente **la que no es evidencia de nada**. Sirve para que el evaluado acepte el test, no para
que el test funcione. Un psicólogo aprende pronto a desconfiar de ella.

Pues bien:

> **Un modelo de lenguaje es el instrumento con la validez aparente más alta y la garantía de validez
> de contenido más baja que va a manejar en su vida.** Está literalmente optimizado para producir
> texto plausible. La plausibilidad de la superficie es su función objetivo, no un efecto secundario.

Esta frase debe estar en el material, y probablemente en la primera lección. Es el puente más limpio
entre lo que ella ya sabe y el error número uno de todo el mundo. Y a diferencia de casi cualquier
otra advertencia anti-hype, esta no la tiene que creer por autoridad: la deduce de algo que ya sabe.

---

### C3 · Fiabilidad ↔ misma entrada, misma calidad; degradación al crecer — [PARCIAL]

**Lo que transfiere bien.**

- **La idea de error de medida.** Que dos pasadas del mismo instrumento sobre el mismo objeto no den
  lo mismo es esperable, y la magnitud de esa variación es un dato, no una anécdota.
- **El principio de que la fiabilidad acota la validez.** Si la misma entrada le da respuestas de
  calidad muy dispar, no hay prompt que arreglar: cualquier conclusión sacada de una sola pasada
  buena es ruido. Practicamente: **nunca se evalúa con n=1**, ni siquiera para descartar. Tres
  pasadas del mismo caso es el mínimo decente, y son treinta segundos.
- **Los ítems ancla.** En psicometría, cuando se cambia de forma de un test, se conserva un conjunto
  de ítems comunes para poder equiparar las puntuaciones. Traducción directa: **un subconjunto fijo
  de casos que se vuelve a pasar cada vez que cambia algo** —el prompt, las fuentes, la versión del
  modelo— y cuyos resultados se apuntan con fecha. En el mundo de la IA a esto lo llaman *tests de
  regresión* o *evals*; el nombre psicométrico describe mejor **para qué sirven**, que es hacer
  comparables dos momentos distintos.

**Dónde la analogía se rompe, y hay que decirlo.**

1. En test-retest, la inestabilidad se atribuye a error de medida **más cambio real en la persona**.
   Aquí el sujeto (el caso de prueba) no cambia: **el que cambia es el instrumento**. La variación
   viene del muestreo estocástico del propio modelo y, sobre todo, de que el proveedor actualiza el
   modelo sin avisar. El análogo correcto no es la inestabilidad del sujeto, es **la deriva del
   instrumento y la caducidad de los baremos**: un test recalibrado en silencio.
2. Consecuencia práctica que no existe en psicología: **la fecha de la última pasada de la batería es
   parte del sistema.** Un cuaderno de resultados con fechas no es burocracia; es lo único que
   distingue "esto ha empeorado" de "esto siempre fue así y no me había dado cuenta".
3. La "degradación al crecer" del programa de referencia —meterle quince ficheros más y ver si
   empieza a perderse— **no tiene análogo psicométrico limpio**. Se parece más a un problema de
   señal/ruido en recuperación de información. Se enseña por su cuenta, sin forzar el paralelismo.

> **EP-04 · Ancla, ruido y deriva**
> (a) Coge tres casos de tu batería y pásalos **tres veces cada uno**, sin cambiar nada. Anota si la
> respuesta cambia y si cambia *de calidad* según tu ficha de EP-01.
> (b) Marca cinco casos como **ancla**. Guárdalos en una hoja con una columna por fecha.
> (c) Vuelve a pasarlos cuando cambies el prompt, cuando añadas fuentes y el primer día que notes que
> "responde raro".
>
> *Autocorrección — está bien si:*
> - [ ] Distingues **variación de forma** (dice lo mismo con otras palabras: irrelevante) de
>       **variación de calidad** (una vez cita el precio y otra no: grave). Confundirlas es el error
>       típico y hace descartar sistemas buenos y aprobar sistemas malos.
> - [ ] La hoja de anclas tiene **fecha en cada columna**. Sin fecha no sirve para nada.
> - [ ] Has resistido la tentación de arreglar el prompt en mitad de la tanda. Si lo arreglas a mitad,
>       las tres pasadas no son comparables.

---

### C3b · Acuerdo entre jueces ↔ ¿clasifica el sistema como clasificarías tú? — [FUERTE]

Cuando el sistema **clasifica** (comentarios de encuesta en P27, correos entrantes en el triaje,
reseñas en P28), la pregunta de calidad no es "¿está bien redactado?" sino **"¿coincide con el juicio
de la experta?"**. Eso es acuerdo entre codificadores, y ella lo ha hecho en clase.

Lo que hay que enseñar entero, porque es donde está el valor:

- **El acuerdo bruto engaña cuando una categoría domina.** Si el 60 % de los comentarios son de
  alojamiento, un clasificador que dijera "alojamiento" siempre acertaría el 60 %. Por eso existe la
  kappa: κ = (P₀ − Pₑ) / (1 − Pₑ), donde P₀ es el acuerdo observado y Pₑ el esperado por azar dadas
  las frecuencias marginales. Dos líneas de aritmética en una hoja de cálculo.
- **La versión barata y suficiente**, para no montar un aparato estadístico sobre 20 casos: mirar el
  acuerdo **dentro de cada categoría minoritaria por separado**. Si el sistema acierta el 95 % global
  y el 30 % de la categoría "administración", el 95 % es una mentira útil para nadie.
- **Con n pequeño, la kappa es inestable.** No se reporta con dos decimales ni se usa para decidir
  nada fino. Sirve para ver un orden de magnitud y sobre todo para **obligar a mirar la tabla de
  confusión**, que es donde de verdad se aprende: qué se confunde con qué. "Confunde
  *administración* con *alojamiento* cuando el comentario habla de la factura del piso" es un
  hallazgo accionable; "kappa = 0,62" no lo es.

> **EP-07 · Doble codificación**
> Coge 30 comentarios reales de la última encuesta. Clasifícalos **tú primero**, sin ver la salida del
> sistema. Después compara.
>
> *Autocorrección — está bien si:*
> - [ ] Clasificaste tú **antes** de ver la respuesta del sistema. Al revés no vale y es lo que sale
>       solo (ver C5, anclaje).
> - [ ] Has construido la **tabla de confusión** y has escrito una frase por cada confusión repetida.
> - [ ] Has revisado tus propios desacuerdos: en al menos uno de ellos, el que estaba mal eras tú, y
>       eso es información sobre tu **libro de códigos**, no sobre el sistema.
> - [ ] Has mirado el acuerdo de la categoría **menos frecuente** por separado.

---

### C4 · Diseño de ítems no sesgados ↔ casos de prueba que no regalen la respuesta — [FUERTE]

Esta es, junto con C1, la transferencia con más valor práctico del documento, porque ataca el error
que **todo el mundo comete de forma natural** y que un curso normal ni siquiera nombra.

**El error, descrito con precisión.** El procedimiento espontáneo de cualquiera es: cojo tres
ejemplos, escribo el prompt, lo ajusto hasta que esos tres salen bien, y digo que está probado. En
lenguaje de medida eso tiene nombre y es doble delito: **contaminación de la muestra** (evalúas con el
material con el que construiste) y **capitalización del azar** (ajustas a las particularidades de tu
muestra). La regla que lo resuelve también tiene nombre y es la misma de siempre: **muestra de
validación independiente**, apartada antes de empezar y no tocada.

Regla operativa para el material, en una línea:

> **Los casos con los que escribes el prompt y los casos con los que lo pruebas no pueden ser los
> mismos. Se apartan diez casos ANTES de escribir nada y no se miran hasta el final.**

**Lo que transfiere de la redacción de ítems:**

- **Pistas en el enunciado.** Un caso de prueba que ya trae dentro la respuesta ("adjunto el
  tarifario, dime el precio de 4 semanas") no prueba el sistema, prueba la aritmética. El caso real es
  el correo del alumno tal cual llegó, con faltas, en inglés, sin decir las fechas exactas.
- **Índice de dificultad.** Un ítem que aprueba el 100 % de la gente no discrimina. Traducción: **si
  tu batería la pasa entera a la primera, tu batería es fácil, no tu sistema es bueno.** Es la única
  interpretación honesta de un 10/10 y hay que enseñarla porque el 10/10 produce euforia y la euforia
  produce el despliegue prematuro.
- **Distractores plausibles.** El caso límite bueno es el que está *cerca* de la categoría correcta,
  no el absurdo. "Un comentario en klingon" no prueba nada; "un comentario que se queja del wifi del
  piso —¿instalaciones o alojamiento?—" prueba el libro de códigos.
- **Preguntas dirigidas.** Preguntarle al propio modelo "¿está bien esta respuesta?" es una pregunta
  sugestiva de manual. Si se le pregunta, se le pregunta en forma de tarea de falsación: *"busca el
  dato de esta respuesta que no está respaldado por las fuentes y cítalo"*. Ver el matiz de C5 y §7.3:
  transfiere la **contramedida**, no la explicación psicológica.

> **EP-06 · Los diez apartados**
> Antes de escribir una sola línea de prompt para tu proceso, aparta diez casos reales en un documento
> aparte. Ciérralo. No vuelvas hasta tener el sistema montado.
>
> *Autocorrección — está bien si:*
> - [ ] Los diez salieron de tu buzón **por orden cronológico o al azar**, no elegidos por ti. Si los
>       elegiste, elegiste los que sabes contestar.
> - [ ] Al abrirlos al final, **falla al menos uno**. Si no falla ninguno, sospecha del muestreo antes
>       que celebrar.
> - [ ] Si al abrirlos te dan ganas de cambiar el criterio de EP-01 para que aprueben, **anótalo y no
>       lo cambies**. Ese impulso es el dato más interesante del ejercicio y se llama sesgo del
>       experimentador (C5).

---

### C5 · Sesgo de confirmación ↔ por qué aceptamos una salida mediocre que suena bien — [FUERTE]

El brief lo llama "sesgo de confirmación", pero ahí dentro hay cinco mecanismos distintos, cada uno
con su contramedida. Separarlos es precisamente lo que aporta el perfil, porque la contramedida
depende del mecanismo. Todos están documentados en la literatura psicológica estándar y **todos
describen a la evaluadora humana, no al modelo** (esa distinción es §7.1).

| Mecanismo | Qué hace exactamente | Cómo se manifiesta en su trabajo | Contramedida |
|---|---|---|---|
| **Fluidez de procesamiento** | Lo que se lee con facilidad se juzga más verdadero y más probable | Un correo bien construido en un español impecable pasa el filtro con el precio equivocado dentro | Leer **contra la ficha de criterio**, indicador por indicador, nunca de un vistazo |
| **Efecto halo** | Una dimensión saliente contamina el juicio de las demás | El tono es perfecto → asumes que los datos también | **Evaluar por columnas, no por filas**: comprobar la misma dimensión en los diez casos antes de pasar a la siguiente |
| **Anclaje** | El primer borrador fija el resultado final; editas alrededor en vez de rehacer | Aceptas una estructura peor porque ya está escrita | Antes de leer el borrador, escribir en dos líneas **qué tiene que decir**. Comparar contra eso |
| **Sesgo de confirmación** | Buscas evidencia de que está bien, no de que está mal | Relees para confirmar, no para falsar | Convertir la lectura en **tarea de falsación**: "encuentra el error", no "¿está bien?" |
| **Sesgo del experimentador** | Lo has montado tú y quieres que funcione | Ajustas el criterio hasta que apruebe | **Evaluación ciega** (EP-08) y criterio congelado antes de probar |
| **Sesgo de automatización** | Complacencia con la máquina: errores de omisión (no ves lo que se dejó) y de comisión (sigues una recomendación errónea) | A la tercera semana dejas de revisar los borradores | Revisión **muestreada y programada**, no "cuando me parezca". Y el dato de C7: la revisión decae con el tiempo, no con la calidad |

El sesgo de automatización viene de factores humanos y ergonomía, no de psicología cognitiva básica,
pero está en el mismo currículo y es el más relevante a medio plazo: **el riesgo del sistema no es el
del día 1, es el del día 60**, cuando ya se confía. Eso conecta con la regla de
`dominio-herramientas.md` §3.5 ("automatiza la lectura y la preparación; la escritura hacia fuera la
firma una persona") y le da la razón por la que esa regla no se puede relajar por costumbre, solo con
datos.

> **EP-05 · Lectura por columnas**
> Coge cinco salidas del sistema. Prohibido leerlas enteras. Comprueba **el indicador 1 en las cinco**,
> luego el 2 en las cinco, y así. Anota cuántos fallos encuentras. Después léelas enteras del tirón,
> como habrías hecho normalmente, y cuenta cuántos habrías detectado.
>
> *Autocorrección:* si la lectura por columnas encuentra **más fallos** que la lectura normal —lo
> habitual es que encuentre bastantes más— el ejercicio ha demostrado su tesis y el procedimiento se
> queda como rutina. Si encuentra los mismos, tu ficha de criterio probablemente tiene indicadores
> redundantes: vuelve a EP-01.

> **EP-08 · La prueba ciega** — el ejercicio con mejor relación valor/esfuerzo de todo el curso
> Coge 5 respuestas que escribiste tú a mano hace meses y 10 borradores del sistema, sobre casos
> comparables. Quita cualquier marca que delate el origen (formato, firma, fecha). Mézclalas,
> numéralas y **pide a alguien que te las presente en orden aleatorio** sin decirte cuál es cuál.
> Puntúalas con la ficha de EP-01.
>
> *Autocorrección — está bien si:*
> - [ ] Has puntuado **todas** antes de mirar la clave. Mirar a mitad invalida la tanda entera.
> - [ ] Puedes contestar a: ¿acierto identificando cuáles eran mías? ¿Ganan las mías? ¿Por qué
>       dimensión concreta ganan o pierden?
> - [ ] Si las del sistema puntúan igual o mejor **en las dimensiones no críticas** y peor **en la
>       exactitud del dato**, has encontrado el patrón real de estos sistemas y ya sabes dónde poner
>       la revisión humana.
>
> *Por qué esto vale tanto:* es un diseño experimental elemental que ella sabe montar y que casi nadie
> en el mundo de la IA aplicada monta nunca. Es, literalmente, la diferencia entre "me parece que
> funciona" y "he comprobado que funciona". Y desactiva de golpe la fluidez, el halo y el sesgo del
> experimentador, que son tres de los seis mecanismos de la tabla.

---

### C6 · Análisis de contenido de respuesta abierta ↔ procesar el texto libre de las encuestas — [FUERTE]

Esta correspondencia cae **exactamente encima del primer proyecto recomendado** (P27, 600–800
respuestas al año con comentarios libres en más de diez idiomas, que hoy nadie analiza). No es una
coincidencia afortunada: es la razón por la que ese proyecto es el correcto para ella y no para otra
persona.

**Lo que hace un no-psicólogo:** pedirle al modelo "clasifica estos comentarios por temas". El modelo
inventa catorce categorías solapadas, distintas en cada pasada, y el informe no es comparable ni
consigo mismo.

**Lo que ella sabe hacer y aquí es la solución técnica:**

1. **Libro de códigos.** Cada categoría con nombre, **definición operativa**, criterios de inclusión y
   de exclusión, dos ejemplos prototípicos y —lo que de verdad marca la diferencia— **dos ejemplos
   frontera con la decisión ya tomada y justificada**. Ese documento es, sin cambiarle una coma, el
   fichero de contexto del clasificador. No es preparación para el prompt: **es el prompt**.
2. **Categorías exhaustivas y mutuamente excluyentes**, con su categoría "otros" y su regla de qué
   hacer cuando algo no encaja. La regla de "no lo sé" del programa de referencia es, en este
   dominio, la casilla "sin clasificar" de un libro de códigos bien hecho.
3. **Unidad de análisis.** ¿La unidad es la respuesta o la frase? "El profesor genial, el piso sucio"
   es **una** respuesta y **dos** unidades con valencias opuestas. Si el flujo obliga a una etiqueta
   por respuesta, se pierde la mitad de la información y las medias mienten. Es una decisión
   metodológica que ella está entrenada para tomar y que determina el diseño de la hoja de cálculo
   (una fila por comentario frente a una fila por unidad codificada).
4. **Fase inductiva y fase deductiva.** Primera pasada abierta sobre una submuestra para construir la
   taxonomía; después se **congela** el libro de códigos y se aplica cerrado al resto. Y se mantiene
   congelado entre oleadas: si las categorías cambian cada mes, no hay serie temporal, hay anécdotas
   mensuales. Esto es lo que convierte el proyecto de "un informe bonito" en "un indicador".
5. **Saturación.** Cuándo dejar de añadir categorías: cuando veinte comentarios nuevos no obligan a
   crear ninguna.
6. **El idioma.** Traducir antes de codificar mete un paso que altera intensidad y cortesía, que es
   justo lo que se quiere medir. Regla práctica: **codificar sobre el original cuando el modelo lo
   permita, y conservar el original al lado de la traducción en todo lo que se escale a una persona.**
   Es la versión práctica de la retrotraducción y de la equivalencia de instrumentos entre culturas.

> **EP-10 · El libro de códigos**
> Coge 40 comentarios reales de la última encuesta. Primera pasada abierta: apunta temas sin
> categorías previas. Construye entre 5 y 8 categorías con definición, inclusión, exclusión, dos
> ejemplos prototípicos y dos frontera. Congélalo. Aplícalo a 40 comentarios nuevos.
>
> *Autocorrección — está bien si:*
> - [ ] Al aplicar el libro cerrado a los 40 nuevos, **menos del 15 % cae en "otros"**. Si cae más, la
>       taxonomía no cubre el dominio: vuelve a la fase inductiva. Si cae 0 %, sospecha: probablemente
>       estás forzando encajes.
> - [ ] Cada categoría tiene su **ejemplo frontera con la decisión justificada**. Sin eso, ni tú ni el
>       modelo clasificaréis igual dentro de dos meses.
> - [ ] Has decidido y escrito cuál es tu **unidad de análisis**, y tu hoja de cálculo la respeta.
> - [ ] Hay una regla explícita para el comentario que menciona **salud, un menor o a un empleado con
>       nombre**: no se clasifica, se para. (Enlaza con E-06 del bloque de datos.)

---

### C7 · Línea base y medida pre/post ↔ demostrar que algo ahorra tiempo de verdad — [FUERTE]

El programa de referencia pregunta "¿esto resuelve de verdad el problema?" y no da ningún método para
contestarlo. La psicología lo da entero, y encima con el catálogo de formas de engañarse.

**Lo que hay que hacer, en orden:**

1. **Medir antes de construir.** Una semana de registro del proceso candidato, apuntando en el
   momento, no reconstruyendo el viernes de memoria. Si la línea base se estima después de tener el
   sistema, está contaminada por las ganas de que funcione.
2. **Definir la unidad.** No "horas a la semana" sino **minutos por unidad de trabajo**: minutos por
   comentario procesado, por lead contestado, por confirmación enviada. Es lo único que sobrevive a la
   estacionalidad brutal de su negocio (el volumen se multiplica por tres entre febrero y julio).
3. **Contar el coste completo,** no solo el tiempo de ejecución: montaje, revisión de las salidas,
   corrección de los fallos y mantenimiento cuando cambia el tarifario. Un flujo que ahorra ocho
   minutos y cuesta diez de revisión es una pérdida disfrazada de modernidad.
4. **Volver a medir con la misma regla.** Instrumentación idéntica o la comparación no vale.

**Las amenazas a la validez interna, traducidas una a una a su caso.** Esto es contenido de curso
directo, no ilustración:

| Amenaza | Cómo la muerde a ella |
|---|---|
| **Historia** | Septiembre no es julio. Cualquier pre-post que cruce temporada mide la temporada, no el sistema |
| **Maduración** | Ella misma mejora en la tarea por repetirla. Parte de la mejora es suya, no del flujo |
| **Regresión a la media** | Elegirá el proceso que **más duele**, y lo que más duele suele medirse en su peor semana. Mejorará algo solo, sin hacer nada |
| **Instrumentación** | Si al principio calculó "a ojo" y luego con cronómetro, la diferencia puede ser de método |
| **Reactividad de la medida** | La semana que se cronometra, se trabaja más rápido. La línea base sale optimista → **el ahorro real es mayor que el medido**. Es el sesgo que juega a favor y conviene decirlo, porque hace creíble el resto |
| **Mortalidad / atrición** | Si deja de usar el flujo los días de agobio, la muestra final son los días tranquilos: justo aquellos en los que menos falta hacía |

**Y la distinción que salva el proyecto entero**, tomada de evaluación de programas (C13):
**evaluación de proceso ≠ evaluación de resultado.** Un flujo puede ejecutarse impecablemente cada
lunes (proceso perfecto) y no cambiar nada (resultado cero) porque el informe que produce no lo lee
nadie o porque los borradores se reescriben siempre. Medir solo que el flujo se ejecuta es la métrica
de vanidad canónica.

> **EP-09 · La línea base honesta**
> Antes de montar tu primer flujo: una semana de registro en el momento, con unidad definida. Después
> de montarlo y usarlo dos semanas: mismo registro. Escribe media página con (a) el número antes, (b)
> el número después, (c) el coste de montaje y de revisión, (d) **cuál de las seis amenazas de la
> tabla podría explicar tu resultado**, y (e) qué medirías para descartarla.
>
> *Autocorrección — está bien si:*
> - [ ] La medida es **por unidad**, no por semana.
> - [ ] Has restado el tiempo de revisión y el de mantenimiento. Si el saldo es negativo y aun así
>       quieres conservarlo por otra razón (menos errores, menos carga mental, respuesta más rápida al
>       cliente), **dilo y mide esa otra razón**: es legítimo, pero entonces el ahorro de tiempo no era
>       el objetivo.
> - [ ] Has nombrado al menos **una amenaza que no puedes descartar**. Un pre-post de un solo grupo
>       nunca las descarta todas, y decirlo es lo que separa un dato de un argumento comercial.
> - [ ] No has usado la palabra "significativo" (ver §7.6).

---

### C8 · Confidencialidad y consentimiento ↔ protección de datos — [PARCIAL, con falsos amigos graves]

`dominio-rgpd.md` es la autoridad de este bloque y aquí solo se marca **qué parte de su formación le
da ventaja y qué parte le va a jugar una mala pasada**.

**Lo que transfiere bien y es ventaja real:**

- **Minimización.** En investigación se recoge lo que la pregunta necesita y nada más. Es literalmente
  el principio del art. 5.1.c. Ya lo tiene interiorizado y aplicado al ejercicio E-02 funciona solo.
- **Codificado no es anónimo.** Un psicólogo sabe que un fichero con código y una clave guardada
  aparte **no es anónimo**: es disociado de forma reversible. Esa es exactamente la distinción
  seudonimización/anonimización del RGPD, y es la que más gente confunde. Parte por delante.
- **Reidentificación por cuasi-identificadores.** La intuición del caso clínico ("varón de 34 años,
  único caso de la unidad") es la misma que hace fallar el E-03: quitar el nombre no basta cuando
  queda "coreana de 19 años que llegó el 3 de julio al piso de Lavapiés". Le va a costar cero.
- **Deber de secreto.** Tiene un código deontológico profesional con confidencialidad dentro. La
  disposición está; lo que cambia es el marco jurídico.

**Lo que NO transfiere está en §7.4 y §7.5, y es importante:** el consentimiento informado, el
anonimato de investigación y el comité de ética son tres falsos amigos con consecuencias prácticas.

**[!] Y el límite de rol, que hay que escribir en el material:** su formación le da **sensibilidad**,
no **competencia jurídica ni autoridad**. El riesgo específico de este perfil es que, por ser la que
más se preocupa, acabe siendo de facto la responsable de cumplimiento de la academia. `dominio-rgpd.md`
§8.5 ya lo prohíbe explícitamente y este documento lo refuerza: cada vez que aparezca una decisión que
no es suya, va marcada y con el nombre de a quién se escala.

---

### C9 · Entrevista y escucha activa ↔ extraer de sus compañeros cómo funciona un proceso — [FUERTE]

El paso 3 del programa de referencia dice que "el contexto es el nuevo petróleo" y que el alumno tiene
que transmitir su conocimiento de la empresa al sistema. Lo que no dice —y es el hueco— es **cómo se
extrae ese conocimiento cuando vive en la cabeza de otras personas**. Eso es una entrevista, y hay
literatura entera al respecto.

**Lo que transfiere entero:**

- **Entrevista semiestructurada.** Guion de temas fijo, orden libre, repreguntas según lo que salga.
  Es exactamente el formato adecuado para levantar un procedimiento.
- **Estructura de embudo.** De lo general a lo específico. Primero "cuéntame cómo va esto", después
  las preguntas cerradas de detalle. Al revés, las cerradas contaminan el relato.
- **Preguntas no sugestivas.** La literatura de memoria de testigos existe para demostrar que la
  redacción de la pregunta cambia la respuesta recuperada. Aquí sirve tres veces a la vez: para
  entrevistar a compañeros, para redactar la encuesta (C10) y para escribir prompts, porque un prompt
  dirigido devuelve la respuesta que sugiere.
- **Pedir el último caso concreto, no la regla general.** La técnica clave, y la que hay que enseñar
  con nombre y todo: *"no me cuentes cómo se hace normalmente; cuéntame el último, el del jueves
  pasado, y ábrelo en la pantalla"*. Motivo: **la gente describe sus procedimientos como cree que
  deberían ser, no como los ejecuta**. El acceso introspectivo al propio procedimiento es limitado, y
  los atajos, apaños y excepciones —que son justo lo que rompe una automatización— no se verbalizan
  espontáneamente. [NV en su formulación fuerte: la tesis general sobre acceso introspectivo está
  discutida; la consecuencia práctica —preguntar por el caso concreto y mirar el artefacto real— es
  técnica estándar de entrevista con independencia de esa discusión.]
- **Reformulación y devolución.** Escribir el procedimiento tal y como lo has entendido y devolverlo
  para que lo corrijan. Corrigiendo se saca más que preguntando: es más fácil detectar un error ajeno
  que producir una descripción completa.
- **Deseabilidad social.** El compañero describirá el proceso oficial, no el real. Contramedidas
  concretas: preguntar por **excepciones** ("¿cuándo fue la última vez que esto no funcionó?"),
  preguntar por **la última vez que hubo que rehacer algo**, y pedir ver el fichero en lugar de que se
  lo cuenten.

**El matiz social, que sí importa aquí.** En su empresa automatizar está bien visto (no hay que vender
nada, el brief es taxativo). Pero eso no elimina que a nadie le gusta que le auditen el
procedimiento. El encuadre que funciona no es "quiero automatizar tu tarea" sino **"quiero aprender a
hacerlo yo bien para no molestarte cada vez"**. Es verdad, además, que es la mejor manera de
conseguirlo.

> **EP-11 · Una entrevista de veinte minutos**
> Elige el proceso propio que más dependa de otra persona (candidatos naturales: P02 presupuestos con
> administración, P22 hoja de camas con alojamiento, P24 condiciones de cancelación con dirección).
> Guion de seis preguntas abiertas. Veinte minutos. Después escribe el procedimiento en una página y
> **devuélvelo para que lo corrijan**.
>
> *Autocorrección — está bien si:*
> - [ ] Las seis preguntas son abiertas y ninguna contiene la respuesta. Prueba: ¿se puede contestar
>       "sí"? Entonces reescríbela.
> - [ ] Al menos dos preguntan por **el último caso concreto**, no por la norma.
> - [ ] Al menos una pregunta por **la excepción**.
> - [ ] La devolución produjo **al menos dos correcciones**. Si no produjo ninguna, o el proceso es
>       trivial o la persona no lo ha leído. Ninguna de las dos cosas es un éxito.
> - [ ] En tu página aparece al menos un paso que **no estaba en tu idea previa del proceso**. Ese
>       paso es el que habría roto tu automatización.

---

## 4. Ampliaciones — correspondencias que el encargo no listaba y que se sostienen

### C10 · Diseño de cuestionarios ↔ que la encuesta de satisfacción no mienta — [FUERTE]

El proceso P27 es el primer proyecto del curso. Pero automatizar el análisis de una encuesta mal
construida es industrializar un error. Ella es la única persona de la academia que puede ver que el
instrumento está mal, y eso es contenido de curso de pleno derecho, no un extra.

**El catálogo, aplicado a una encuesta de satisfacción de academia de idiomas:**

- **Preguntas dobles.** "¿Estás satisfecho con el profesor y con el material?" no se puede contestar y
  no se puede interpretar.
- **Preguntas dirigidas.** "¿Cómo de útil te ha resultado el curso?" presupone la utilidad. La versión
  neutra deja sitio al cero.
- **Etiquetado de la escala.** Etiquetar solo los extremos y numerar el medio produce interpretaciones
  distintas por cultura y por nivel de español. Con alumnado de nivel A2 en un cuestionario en su
  cuarto idioma, **cada punto etiquetado con palabras**, y palabras cortas.
- **Punto medio.** Quitarlo fuerza una posición y sube artificialmente la polarización; ponerlo invita
  al refugio. Es una decisión, y hay que tomarla a conciencia, no por defecto de la herramienta.
- **Ítems invertidos.** La contramedida clásica contra la aquiescencia **aquí es mala idea**: en una
  población que responde en un idioma que está aprendiendo, un ítem en negativo produce errores de
  comprensión que se confunden con respuestas. Es un ejemplo perfecto de "la técnica correcta en el
  contexto equivocado", y merece salir en el material precisamente por eso.
- **Efectos de orden y de contexto.** Preguntar por el alojamiento justo antes de la pregunta global
  arrastra la global. Si la valoración global importa, va primero.
- **Momento de la medición.** La encuesta del último día, después de la fiesta de despedida y las
  fotos, no mide la estancia: mide el final de la estancia. El juicio retrospectivo de una experiencia
  pesa desproporcionadamente el pico y el final. Consecuencia concreta: **la encuesta de fin de curso
  y la de mitad de curso no miden lo mismo y no se pueden promediar juntas**, y una caída de la nota
  puede venir de haber cambiado el día en que se pasa.
- **Sesgo de no respuesta y autoselección.** Con 600–800 respuestas de ~1.400 envíos, **quien contesta
  no es una muestra aleatoria**. Responden más los muy contentos y los muy enfadados. Corolarios
  operativos: (a) la media no es la media de los alumnos; (b) **comparar meses con tasas de respuesta
  distintas no es comparar satisfacción**; (c) la tasa de respuesta hay que apuntarla siempre al lado
  del resultado, y si nadie la apunta hoy, empezar a apuntarla ya es una mejora medible.
- **NPS.** Un solo ítem, puntos de corte arbitrarios y una métrica que tira información. Si en la
  academia se usa, ella puede decir por qué la variación mes a mes con n pequeño es en buena parte
  ruido. No hace falta pelearse con la métrica: basta con reportar al lado la distribución completa.

> **EP-12 · Autopsia del cuestionario actual**
> Consigue el cuestionario de satisfacción que se usa hoy. Marca sobre él: preguntas dobles,
> preguntas dirigidas, escalas mal etiquetadas, problemas de orden, y anota la tasa de respuesta y el
> momento en que se pasa. Escribe una versión corregida y **una nota de media página** para quien sea
> dueño del cuestionario, con los tres cambios que más impacto tienen y por qué.
>
> *Autocorrección — está bien si:*
> - [ ] Has encontrado **al menos un problema de redacción y uno de procedimiento** (momento, canal,
>       tasa de respuesta). Casi ninguna encuesta interna se libra de los dos.
> - [ ] Tu versión corregida **no es más larga** que la original. Alargar una encuesta baja la tasa de
>       respuesta y empeora el sesgo que intentas corregir.
> - [ ] La nota propone **tres cambios, no doce**, y cada uno dice qué problema concreto resuelve.
>
> *Nota de encaje con el brief:* esto **no es un módulo de venta interna** —que el brief prohíbe—.
> Es su propio trabajo: la satisfacción del cliente está en su puesto. La diferencia está en que no
> propone una herramienta ni pide presupuesto: mejora un instrumento del que ya es responsable.

---

### C11 · Estilos de respuesta culturales ↔ por qué un clasificador de sentimiento falla con su alumnado — [FUERTE]

Este es, probablemente, el aporte técnico más valioso y menos evidente de todo el perfil, y es
específico de su empresa: **80,3 % europeos, 9,3 % asiáticos, y comentarios en más de diez idiomas**.

Dos fenómenos documentados en psicología transcultural:

1. **Estilo de respuesta extremo frente a estilo moderado.** Hay diferencias sistemáticas por cultura
   en el uso de los extremos de una escala: los encuestados de varias culturas del este asiático
   tienden a evitar los extremos y los de culturas latinoamericanas a usarlos más. Efecto directo:
   **un 3/5 japonés y un 3/5 italiano no significan lo mismo**, y comparar la satisfacción media por
   nacionalidad sin tenerlo en cuenta produce un ranking de estilos de respuesta disfrazado de ranking
   de calidad. Si en el informe mensual a gerencia (P31) aparece "los alumnos coreanos están menos
   satisfechos", puede que solo estén siendo coreanos.
2. **Normas de cortesía e indirección.** "Quizá el desayuno podría mejorar un poquito" puede ser una
   queja seria; "the flat was dirty" puede ser un informe factual neutro. Un clasificador de
   sentimiento, entrenado sobre todo con texto en inglés y con quejas explícitas, **subestima
   sistemáticamente la queja educada indirecta**.

**En qué se convierte esto, que es lo que importa:**

- Casos de la batería (C2) que **solo se le ocurren a ella**: la queja indirecta, el elogio tibio que
  en realidad es una crítica, el silencio en un campo que en otro alumno estaría lleno.
- Una **regla de calibración** en el libro de códigos: la intensidad se codifica **con la lengua de
  origen a la vista**, y los umbrales de escalado se revisan por grupo lingüístico.
- Una **advertencia fija en el informe**: no se comparan medias entre nacionalidades sin nota al pie.
- Y una consecuencia de diseño de la encuesta: preferir **preguntas de conducta** ("¿recomendarías el
  alojamiento a un amigo?", "¿volverías?") a preguntas de valoración pura, porque las conductuales
  son menos sensibles al estilo de respuesta.

[NV] El detalle de qué culturas concretas puntúan cómo no se ha verificado en fuente en esta sesión y
**no debe entrar al material como tabla de nacionalidades**: entra como principio, con la instrucción
de comprobarlo con sus propios datos, que ella tiene y las publicaciones no. Convertir esto en una
lista de "los alemanes puntúan así" sería estereotipo con barniz metodológico y es justo lo que hay
que evitar.

---

### C12 · Justicia organizacional ↔ la rúbrica de una respuesta difícil — [FUERTE]

Cuando la respuesta al cliente es "no" —no hay reembolso, no se cambia de familia, la política es la
que es—, lo que determina si esa persona escribe una reseña de una estrella no es el resultado. La
investigación sobre justicia organizacional distingue tres componentes, y los tres son operacionalizables
como dimensiones de rúbrica:

| Componente | Qué es | Cómo se ve en un correo | Indicador comprobable |
|---|---|---|---|
| **Distributiva** | El resultado es proporcionado | El importe devuelto | ¿Coincide con la política? |
| **Procedimental** | El procedimiento es consistente y se explica | "Estas son las condiciones que aceptaste el 3 de marzo, y se aplican igual a todos" | ¿Se cita la regla y su origen? ¿Se dice quién decide y en qué plazo? |
| **Interaccional** | Trato respetuoso y explicación sincera | Reconocer el perjuicio sin negarlo | ¿Hay reconocimiento explícito? ¿Hay una explicación, no solo una decisión? |

**Por qué esto es contenido y no filosofía:** convierte "escribe con empatía" —que es una instrucción
inútil para un modelo y para una persona— en **tres indicadores comprobables** que caben en la ficha
de criterio de EP-01 y en el fichero de contexto del redactor. Un perfil técnico no tiene de dónde
sacar esas tres dimensiones; ella sí.

**La tensión que hay que enseñar, porque es real y es peligrosa [!]:** el reflejo entrenado de la
psicóloga es validar, empatizar y hacerse cargo. En P26 (quejas formales, riesgo **crítico**), hacerse
cargo por escrito **es una admisión de responsabilidad que compromete a la empresa**. Hay formulaciones
que reconocen el malestar sin admitir el hecho ni la culpa, y hay que enseñarlas explícitamente:

- Reconocer la experiencia, no calificar el hecho: *"entiendo que llegar y encontrarte la habitación
  así fue una mala llegada"* frente a *"tienes razón, la habitación estaba en malas condiciones"*.
- Describir lo que se ha hecho, no juzgar lo que pasó: *"hemos hablado con la familia y hemos
  revisado el registro de la llegada"*.
- Evitar el **"lamentamos que te sientas así"**, que es la fórmula que suena a disculpa y funciona
  como invalidación. Es el peor de los dos mundos.
- Y la frontera: **importes, plazos legales, responsabilidad y compensaciones no las decide ella ni el
  sistema.** Se escala.

> **EP-13 · Rúbrica de respuesta difícil y su batería**
> Construye la ficha de criterio de "respuesta a una queja" con seis dimensiones: exactitud del hecho ·
> justicia procedimental · justicia interaccional · ausencia de admisión de responsabilidad · idioma y
> registro · siguiente paso concreto (qué, quién, cuándo). Prepara ocho casos reales seudonimizados de
> P20, P24, P26, P09 y P28. Genera borradores y **evalúalos en ciego** (EP-08).
>
> *Autocorrección — está bien si:*
> - [ ] La dimensión "siguiente paso" exige **persona y fecha**. "Lo revisaremos" no cumple.
> - [ ] Al menos dos de tus ocho casos son de los que **el sistema no debe redactar**, sino marcar y
>       pasar a una persona. Si los ocho son redactables, tu muestra evita lo difícil.
> - [ ] Has encontrado al menos un borrador que **suena estupendo y admite responsabilidad**. Aparece
>       casi siempre: los modelos son complacientes y la complacencia por escrito, en una queja, es
>       exposición legal. Cuando aparezca, es el mejor ejemplo del curso entero de por qué la
>       validez aparente no basta.

---

### C13 · Evaluación de programas ↔ "¿esto resuelve de verdad el problema?" — [FUERTE]

La pregunta con la que el programa de referencia cierra su método es, sin cambiarle nada, una pregunta
de **evaluación de programas**, que es una asignatura de la carrera. El armazón entero transfiere:

| Evaluación de programas | Su versión aquí |
|---|---|
| Evaluación de necesidades | El inventario de tareas y la elección del proceso de partida (E-04) |
| Teoría del programa | "Si el sistema clasifica los comentarios, entonces X pasará" — escrito **antes** |
| Evaluación de implantación / proceso | ¿El flujo se ejecuta? ¿Se usa? ¿Se usa como se diseñó? |
| Evaluación de resultado | ¿Cambió lo que queríamos que cambiara? |
| Evaluación económica | Coste de montaje + revisión + mantenimiento frente al ahorro |

**La pieza que más rinde es la teoría del programa**, porque obliga a escribir la cadena causal
completa antes de construir: *"hoy nadie lee los 700 comentarios → si se clasifican y se resumen cada
semana → dirección académica verá los problemas recurrentes de alojamiento en semanas en vez de en
meses → se podrá actuar antes de que se acumulen"*. Escrita así, salta a la vista el eslabón débil:
**el sistema produce un informe, pero el cambio depende de que alguien lo lea y actúe.** Si ese
eslabón no existe, el proyecto puede estar técnicamente perfecto y no servir para nada, y conviene
saberlo antes de dedicarle tres semanas.

> **EP-14 · La cadena causal en cinco flechas**
> Antes de montar el flujo, escribe la cadena desde lo que haces hoy hasta el cambio que esperas, con
> un máximo de cinco flechas. Subraya **el eslabón que no depende de ti**.
>
> *Autocorrección:* si ningún eslabón depende de otra persona, probablemente has elegido una tarea
> puramente tuya, y eso es **bueno para empezar**. Si hay dos o más eslabones fuera de tu control,
> el proyecto es más frágil de lo que parece: no lo descartes, pero mide el proceso además del
> resultado, y ten prevista la versión que te sirve a ti aunque nadie más la use.

---

## 5. Vocabulario: qué usar deliberadamente y qué sonaría falso

### 5.1 Vocabulario que conviene usar, y por qué

La regla para decidir: **se usa el término de psicología cuando nombra mejor que el término de IA una
cosa que hay que hacer**. No como guiño.

| Término | Por qué se usa |
|---|---|
| **Operacionalizar / definición operativa** | No hay equivalente en el vocabulario de IA no técnico. "Escribir un buen prompt" no dice lo mismo |
| **Indicador observable · ancla conductual** | Convierte "buen tono" en algo comprobable |
| **Validez de contenido · tabla de especificaciones** | Nombra por qué una batería de casos puede estar mal aunque sea grande |
| **Validez aparente** | Es la advertencia central del curso y ella ya sabe desconfiar de ella |
| **Deficiencia y contaminación del criterio** | El vocabulario de IA no tiene nada tan preciso para "estás midiendo lo que no es" |
| **Fiabilidad entre jueces · tabla de confusión** | Nombra exactamente la pregunta "¿clasifica como yo?" |
| **Ítem ancla** | Se usa **declarando el préstamo**: "en IA a esto lo llaman tests de regresión o *evals*; el nombre psicométrico dice mejor para qué sirven" |
| **Libro de códigos · unidad de análisis · categorías exhaustivas y excluyentes** | Es literalmente el artefacto que hay que construir en P27 |
| **Línea base · amenazas a la validez interna · regresión a la media · reactividad de la medida** | Es el método que falta en el paso 5 de la referencia |
| **Sesgo de no respuesta · autoselección** | Sin esto, el informe de satisfacción miente y nadie sabe por qué |
| **Efecto halo · anclaje · fluidez de procesamiento · sesgo del experimentador** | Nombran mecanismos distintos con contramedidas distintas |
| **Evaluación ciega** | Es una técnica, no una metáfora, y la puede montar en una tarde |
| **Seudonimización · cuasi-identificador · minimización** | Coinciden con el vocabulario del RGPD, así que además es el término correcto |
| **Entrevista semiestructurada · embudo · pregunta sugestiva · reformulación** | Es el método para levantar contexto, que es el paso 3 del método |
| **Justicia procedimental e interaccional** | Convierte "empatía" en rúbrica |
| **Evaluación de proceso frente a evaluación de resultado** | La distinción que evita la métrica de vanidad |

### 5.2 Vocabulario que sonaría forzado, falso o condescendiente

| No usar | Por qué |
|---|---|
| "El prompt es como establecer *rapport* con el modelo" | No hay relación, no hay alianza, no hay nadie enfrente. Es la analogía que más rápido destruye la credibilidad del material |
| "Escucha activa con la IA" | La escucha activa atiende al estado de un interlocutor. Aquí no hay estado que atender |
| "Empatía con el modelo", "el modelo se frustra / se cansa / hoy está vago" | Categoría equivocada. Y además produce diagnósticos falsos: si crees que "está cansado", vuelves a preguntarle en vez de arreglar la fuente |
| Vocabulario clínico o psicodinámico (resistencia, transferencia, proyección, inconsciente del modelo) | Es el registro que convierte un documento técnico en un texto ridículo |
| **Alfa de Cronbach** aplicado a una batería de casos | Directamente incorrecto. Ver §7.2 |
| **Significación estadística, valor p, potencia** sobre 12 casos | Ritual sin función. Ver §7.6 |
| "Análisis factorial de las respuestas del modelo" | Ni el objeto ni el n lo permiten |
| "Perfil psicométrico del modelo", "personalidad del modelo" | Los modelos tienen configuraciones y sesgos estadísticos, no rasgos |
| "Como psicóloga, esto ya lo sabes" dicho a secas y en general | Es el halago que el brief prohíbe. Se dice **de qué** parte concreta, y se dice también qué parte no |
| "Terapia" o "diagnóstico" aplicados a un cliente enfadado | Es un cliente, no un paciente. El encuadre clínico con un cliente es intrusivo y suena condescendiente |

### 5.3 Registro: cómo se dirige el material a ella

- Se le habla como a alguien con formación metodológica, **sin explicarle qué es una variable**.
- Cuando algo lo sabe, se dice en una línea y se pasa: *"esto es una tabla de especificaciones; ya
  sabes cómo se hace, aquí las celdas son categorías de comentario"*. Nada de reintroducir la
  psicometría desde cero: es lo que la haría abandonar por aburrimiento.
- Cuando algo **no** lo sabe —que un disparador dispara, que un paso de un flujo consume el resultado
  del anterior— se explica entero y sin dar por supuesto nada, **y se dice que es nuevo**. La mezcla
  de los dos registros sin avisar es lo que hace que un material se sienta condescendiente en unos
  párrafos e incomprensible en otros.

---

## 6. Qué NO le da la psicología — la mitad honesta

Esta sección existe para que el resto sea creíble, y debería estar también en el material, no solo en
esta nota.

1. **Entender cómo funciona una automatización.** Qué es un disparador, qué es un paso, por qué el
   paso 3 no ve lo que produjo el paso 1, qué es una condición. No hay nada en su formación que ayude.
   Se aprende como todo el mundo, haciendo, y le va a costar los primeros dos intentos.
2. **Tolerancia al trasteo.** Buena parte del trabajo real es probar, fallar por un motivo tonto,
   volver a probar. La formación en método enseña a diseñar bien antes de ejecutar; aquí se ejecuta
   mal muchas veces a propósito. Es un cambio de hábito, no de conocimiento.
3. **Pensar en datos estructurados.** Que una hoja de cálculo tenga una fila por unidad y una columna
   por variable **sí** le suena; que haya que decidir formatos, identificadores estables y qué pasa
   cuando falta un campo, no.
4. **Diagnosticar por qué falla algo.** Cuando el flujo no arranca, el razonamiento útil es de
   sistemas, no de personas. Aquí es donde rinden los **puntos de consulta** con su pareja.
5. **Criterio de coste y de límites de plataforma.** Cuotas, planes, qué está incluido. Es información,
   no habilidad, y está en `dominio-herramientas.md`.

Y el riesgo propio del perfil, que hay que decir con todas las letras:

> **El riesgo de este perfil no es quedarse corta de rigor: es pasarse.** Una psicóloga puede dedicar
> tres semanas a construir el instrumento perfecto para una tarea que se resuelve probando una tarde.
> La asignación correcta es: **el montaje se hace rápido y sucio; el rigor se gasta entero en la
> evaluación.** Un prototipo mediocre bien evaluado enseña más que un diseño impecable sin probar.
> Si un ejercicio de este documento le está llevando más de lo que le llevaría hacer la tarea a mano
> durante un mes, el ejercicio está mal calibrado y hay que recortarlo.

---

## 7. Falsos amigos — en qué se parece pero no es igual

Los ocho de esta sección son analogías que **se le van a ocurrir sola** si el material no las corta
antes. Están ordenados de más a menos peligroso.

### 7.1 El modelo no es un sujeto, y el fallo del modelo no es un sesgo cognitivo — [FALSA]

La trampa más probable de este perfil concreto, y la que más daño hace porque produce diagnósticos
falsos y, por tanto, arreglos falsos.

Un sesgo cognitivo es una desviación sistemática del juicio humano con un mecanismo detrás:
heurísticos, motivación, capacidad limitada, historia de aprendizaje del individuo. Lo que hace un
modelo de lenguaje tiene otras causas: distribución del texto de entrenamiento, función objetivo,
ajuste posterior por preferencias humanas. **Que el resultado se parezca no implica que el mecanismo
sea el mismo, y las contramedidas psicológicas no se pueden importar por analogía.**

Consecuencias prácticas de confundirlo:

- "Se ha confundido porque el correo era ambiguo, como me habría pasado a mí" → explicación cómoda
  que impide ver que el problema era que **el tarifario no estaba entre sus fuentes**.
- "Está teniendo un mal día" → se vuelve a preguntar en vez de arreglar el contexto.
- "Se lo he explicado con más cariño y ahora lo hace bien" → probablemente lo que ha cambiado es que
  al reescribir has puesto el dato que faltaba, no el tono.

**La regla para el material:** los fallos se describen en términos de **entrada → salida**, nunca de
intenciones o estados. "Cuando el correo no dice las fechas, inventa una" es un diagnóstico.
"No entiende bien a los alumnos que escriben con prisa" es una historia.

**El matiz que salva la parte útil, y hay que darlo:** algunos efectos **funcionalmente** parecidos sí
se reproducen —el orden de la información cambia la respuesta, la formulación de la pregunta arrastra
la contestación, el sistema tiende a darte la razón—. Lo que transfiere es **el método experimental
para detectarlos** (variar el orden, contrabalancear, formular en neutro y en dirigido y comparar), no
la explicación psicológica ni el repertorio de técnicas de *debiasing* humano.

### 7.2 Consistencia interna ≠ fiabilidad de una batería de casos — [FALSA]

El alfa de Cronbach mide en qué grado los ítems de una escala comparten un factor común. Una batería
de casos de prueba **debe ser deliberadamente heterogénea**: cubre categorías distintas, dificultades
distintas y modos de fallo distintos. Si tuviera consistencia interna alta, sería porque todos los
casos miden lo mismo, es decir, porque la batería está mal.

**En un banco de pruebas, la heterogeneidad es una virtud, al revés que en una escala.** Se dice así,
en una línea, y se cierra el tema.

### 7.3 Preguntarle al modelo si lo ha hecho bien ≠ una segunda opinión — [PARCIAL, muy engañosa]

Un modelo tiende a asentir a la formulación que se le da. El parecido funcional con la aquiescencia es
evidente, pero el mecanismo no es el mismo (§7.1), y de ahí sale el falso amigo: se cree que basta con
"pedirle que sea crítico". No basta, porque no hay un juicio independiente detrás; hay otra generación
condicionada por el mismo texto.

Lo que sí funciona, y es transferencia de diseño de ítems:

- Pedir **falsación concreta**, no valoración: *"señala las tres afirmaciones de este texto que no
  estén respaldadas por las fuentes adjuntas, y cita el fichero"*.
- Pedir el **contraargumento** por separado, no el veredicto.
- **No preguntarle nunca en la misma conversación** en la que produjo la respuesta, porque arrastra
  todo el contexto que la generó.
- Y sobre todo: **la evaluación que decide es la de la ficha de criterio, hecha por una persona.** El
  modelo puede pre-filtrar, no puede aprobar.

### 7.4 Consentimiento informado ≠ base jurídica del RGPD — [FALSA, y con consecuencias]

En investigación, el consentimiento informado es la vía por defecto para legitimar el tratamiento. En
el RGPD es **una de seis bases jurídicas, y en su empresa casi nunca es la que aplica**: los datos de
un alumno se tratan para ejecutar el contrato de matrícula y para cumplir obligaciones legales, no
porque el alumno haya consentido. Y el consentimiento tiene requisitos que en una relación comercial
rara vez se cumplen: libre —no puede ser condición para recibir el servicio—, específico, informado y
**revocable en cualquier momento**, lo que obligaría a deshacer el tratamiento.

Riesgo concreto si se confunde: proponer "pedimos consentimiento para usar IA con los datos de los
alumnos" como solución. Suena responsable, es incorrecto, es más frágil que la base que ya tienen y la
deja en mal lugar ante quien sí lleva el cumplimiento. **[!] La base jurídica no la elige ella.**
Ver `dominio-rgpd.md` §1.2.

### 7.5 Anonimato de investigación ≠ anonimización del RGPD · Comité de ética ≠ EIPD — [FALSA]

- "Anónimo" en un estudio suele significar "no publicaremos tu nombre". Anonimizado en el RGPD
  significa **irreversiblemente no reidentificable**, y entonces el RGPD deja de aplicarse. El listón
  es muchísimo más alto y casi nada de lo que ella maneja lo cumple. Lo que hará en la práctica es
  **seudonimizar**, que sigue siendo dato personal.
- Un comité de ética de investigación y una evaluación de impacto en protección de datos comparten
  espíritu y no son la misma cosa: distinto disparador, distinto contenido, distinto responsable.
  Saber que existe la figura está bien; **[!] decidir si hace falta una EIPD no es su decisión**.

### 7.6 Inferencia estadística ≠ evaluación de un sistema propio — [FALSA]

Tentación natural del perfil: querer significación, tamaño muestral, contraste. Aquí **no se está
estimando un parámetro de una población** ni contrastando hipótesis: se está comprobando la cobertura
de un instrumento contra un criterio fijado. Es evaluación criterial, no inferencial.

Traducción operativa: **doce casos bien elegidos valen más que doscientos al azar**, y la pregunta no
es "¿es significativa la diferencia?" sino "¿en qué celda de mi tabla falla y por qué?". El día que
haga falta comparar dos versiones con datos de verdad, ya lo hablará con alguien; hasta entonces,
importar el ritual inferencial solo añade trabajo y falsa autoridad.

### 7.7 "Satisfacción" en psicología ≠ satisfacción del cliente — [PARCIAL]

La satisfacción del cliente no es un rasgo estable ni un estado de bienestar: es un **juicio
transaccional que compara la experiencia con la expectativa previa**. Consecuencias que le tocan de
lleno:

- La expectativa **la fabrica la propia academia** con su web, sus fotos del piso y lo que ella misma
  promete por correo. Una caída en la satisfacción puede venir de un marketing mejor, no de un
  servicio peor. Es una hipótesis que hay que poder poner encima de la mesa en P31.
- Por eso las **descripciones realistas del alojamiento** son intervención de satisfacción, no
  honestidad decorativa.
- Y por eso las quejas de alojamiento (P20) mezclan siempre hechos y expectativas, como ya recoge
  `dominio-academia.md`. Separar las dos cosas antes de responder es media respuesta.

### 7.8 Entrevista clínica ≠ entrevista de proceso · empatía ≠ admisión — [PARCIAL]

- Con un compañero, el encuadre es profesional y no confidencial de la manera en que lo es el clínico.
  Las técnicas de exploración transfieren; el contrato relacional, no. Ir de terapeuta con un
  compañero es intrusivo y se nota.
- Con un cliente enfadado por escrito, el registro de acompañamiento emocional puede leerse como
  condescendencia, y en una queja formal puede convertirse en admisión de responsabilidad (C12). La
  frontera está en **reconocer la experiencia sin calificar el hecho**.

### 7.9 Un apunte final sobre "el sistema aprende" — [FALSA]

Un modelo no aprende de las correcciones dentro de una conversación de la manera en que aprende una
persona: no consolida nada más allá del contexto disponible, y la memoria entre sesiones es una
función del producto, limitada y explícita, no un proceso de aprendizaje. `dominio-herramientas.md`
§2.2 marca ese límite con detalle. Aquí solo se registra que el vocabulario del aprendizaje humano es
el que produce la expectativa equivocada: **si algo tiene que estar disponible mañana, se escribe en
un fichero de contexto; no se le "enseña".**

---

## 8. El aporte diferencial en atención al cliente asistida por IA, convertido en contenido

Requisito 5 del encargo. Aquí está lo que un perfil de psicología aporta y un perfil técnico no, ya en
forma de módulos. Ninguno de estos módulos es "blando": todos terminan en un artefacto reutilizable.

### 8.1 El argumento, sin adornos

Un perfil técnico monta el flujo, entiende por qué falla la integración, controla el coste y sabe
dónde poner los permisos. Lo que **no** puede aportar es el contenido de la especificación: qué es una
respuesta correcta en este negocio, qué se puede decir y qué no, qué significa realmente el comentario
de una alumna coreana, y por qué la métrica que todo el mundo mira no mide lo que dice medir.

En atención al cliente, **el cuello de botella no es la ingeniería, es la especificación y la
evaluación**. Ahí es donde está su ventaja, y es donde el curso tiene que gastar sus mejores páginas.

### 8.2 Módulo T · Tono como especificación, no como adjetivo

- Anclas conductuales por dimensión y por canal (correo, WhatsApp, respuesta pública a reseña), que
  no son el mismo registro.
- Reglas positivas y negativas con ejemplos reales suyos.
- Variación por idioma: la cortesía no se traduce, se sustituye. Un correo en alemán correcto no es un
  correo en español traducido.
- **Artefacto:** el fichero de contexto de tono del escalón 1, que después se reutiliza como fuente en
  la Gem y como paso en el flujo. *Ejercicio: EP-02.*

### 8.3 Módulo Q · Respuestas difíciles

- Separar hecho / interpretación / emoción en la queja entrante, antes de redactar nada.
- Estructura de respuesta: acuse → reformulación de lo ocurrido → qué se ha comprobado → qué se ofrece
  o por qué no → siguiente paso con persona y fecha.
- Las tres justicias como dimensiones de rúbrica (C12).
- La frontera legal: empatía sin admisión; qué no se pone nunca por escrito; qué se escala **[!]**.
- Catálogo de fórmulas que suenan a disculpa y funcionan como invalidación.
- **Artefacto:** ficha de criterio de respuesta a queja + banco de ocho casos + prueba ciega.
  *Ejercicios: EP-13, EP-08.*
- **Nota de alcance:** P26 (quejas formales) es riesgo crítico y **zona de no automatización**. Este
  módulo entrena a *ella* a redactar mejor y a evaluar borradores, no a delegar la queja formal.

### 8.4 Módulo D · Detección de insatisfacción en texto libre

- Libro de códigos con categorías, valencia e **intensidad** como dimensiones separadas.
- La queja educada indirecta y el estilo de respuesta cultural (C11) como casos de prueba obligatorios.
- Regla de escalado: qué comentario deja de ser un dato de encuesta y se convierte en una incidencia
  que hay que atender **hoy** (mención de salud, de un menor, de dinero, de abogado o de reclamación).
- Qué hacer con el comentario que nombra a un empleado.
- **Artefacto:** el clasificador de P27, con su libro de códigos y su batería. *Ejercicios: EP-10,
  EP-07, EP-03.*

### 8.5 Módulo E · Encuestas que no sesgan

- Autopsia del cuestionario actual y versión corregida (C10).
- Tasa de respuesta y sesgo de autoselección como parte obligatoria de cualquier informe.
- Momento de la medición y por qué la nota del último día no es la nota de la estancia.
- Preguntas de conducta frente a preguntas de valoración en población multilingüe.
- **Artefacto:** cuestionario revisado + nota de media página. *Ejercicio: EP-12.*

### 8.6 Módulo M · Medir si esto sirve

- Línea base, unidad de medida, coste completo (C7).
- Las seis amenazas a la validez interna aplicadas a su caso.
- Proceso frente a resultado, y la cadena causal en cinco flechas (C13).
- **Artefacto:** media página de evaluación por cada sistema que monte, con fecha. *Ejercicios: EP-09,
  EP-14.*

### 8.7 Dónde encaja cada cosa en la escalera de `dominio-herramientas.md`

| Escalón | Qué entra de este documento |
|---|---|
| **0 · Diagnóstico** | C1 (ficha de criterio como hábito), C7 (línea base **antes** de construir), C9 (entrevista para levantar contexto), C8 junto al bloque de datos |
| **1 · Salir del chat** | C1/EP-01 y EP-02 (tono anclado, que alimenta la Gem), C2c (validez aparente como advertencia de apertura), C4/EP-06 (apartar diez casos antes de escribir el prompt), C2/EP-03 (la batería de la Gem) |
| **1,5 · Primera automatización** | C6 (libro de códigos para la columna `=AI()` de la encuesta) |
| **2 · Automatización con Studio** | C6 completo, C3b/EP-07 (doble codificación), C11 (calibración cultural), C10/EP-12, C12/EP-13, C5/EP-08 (prueba ciega) |
| **3 · Juicio dentro del flujo** | C3/EP-04 (anclas y deriva), C2b (deficiencia y contaminación del criterio), C13/EP-14, C5 (sesgo de automatización: el riesgo del día 60) |
| **4 · Opcional** | Nada. Es lectura |

### 8.8 Los puntos de consulta con su pareja que salen de este documento

El brief obliga a racionar este recurso. De todo lo anterior, **solo dos lo merecen**, y ninguno de
los dos se solapa con los dos que ya reserva `dominio-rgpd.md` §8.4:

1. **Presentar las respuestas barajadas en EP-08 (prueba ciega).** No es una consulta, es una función
   que ella no puede hacer sola: alguien tiene que barajar y guardar la clave. Cinco minutos, y sin
   esa persona el ejercicio pierde su propiedad esencial. Vale también cualquier compañero.
2. **La primera vez que un flujo falle y no se sepa si el fallo es de diseño o de plataforma.** Es el
   punto que ya marca `dominio-herramientas.md` en el escalón 2, y este documento solo lo confirma
   desde otro ángulo: distinguir "mi criterio estaba mal" de "la herramienta no puede hacer esto" es
   justo lo que su formación **no** le da (§6, punto 4).

Todo lo demás se autocorrige con las rúbricas de los EP.

---

## 9. Cómo debe entrar todo esto en el material — reglas de redacción

1. **Nunca un módulo llamado "tu ventaja como psicóloga".** Sería exactamente el halago que el brief
   rechaza y además rompería el orden de la escalera. Va **repartido y pegado a la acción**: el
   vocabulario aparece cuando hace falta hacer la cosa.
2. **La primera vez que se usa un término de psicología, se dice explícitamente por qué se usa ese y
   no el de IA**, y se da el equivalente de IA entre paréntesis para que sepa buscarlo por su cuenta.
3. **Cada correspondencia se enuncia con su límite en el mismo párrafo.** Nunca "esto es igual que";
   siempre "esto es la misma operación, con esta diferencia".
4. **Los falsos amigos de la sección 7 aparecen antes de que ella pueda cometer el error**, no
   después. El de "el modelo no es un sujeto" va en la primera semana.
5. **Ningún ejercicio EP se presenta como práctica metodológica.** Todos producen un artefacto que se
   usa en el escalón siguiente: la ficha de criterio alimenta la Gem, el libro de códigos alimenta el
   clasificador, las anclas de tono alimentan el fichero de contexto.
6. **Se dice también lo que no le sirve** (§6), y se dice pronto. Es lo que hace creíble el resto.

---

## 10. Riesgos de este enfoque

- **Sobreintelectualizar el curso.** Es un curso para automatizar tareas, no un máster de
  metodología. Salvaguarda: ningún ejercicio EP sin artefacto reutilizable; el que no lo tenga, fuera.
- **Convertir el rigor en freno.** Una alumna que no monta nada hasta tener la batería perfecta no
  monta nada. Salvaguarda: la regla de §6 —montaje rápido, rigor en la evaluación— repetida en el
  material, no solo aquí.
- **Que el material suene a que la evalúan a ella.** Todo el vocabulario de este documento viene de
  contextos donde alguien evalúa a personas. Aquí el objeto evaluado es **un sistema que ella
  construye**, y conviene que eso quede claro desde la primera línea o el registro se vuelve incómodo.
- **Que la sección de vocabulario se lea como permiso para lucirse.** Los términos se usan para hacer
  cosas; en un correo interno a un compañero no se dice "he calculado el acuerdo intercodificador",
  se dice "he comprobado 30 comentarios a mano y coincide en 26".

---

## 11. Resumen ejecutivo

1. El solapamiento es real y está concentrado en **dos de los cinco pasos** del método de referencia:
   describir la tarea (paso 2) y evaluar el resultado (paso 5). En esos dos, el curso puede ir mucho
   más rápido y mucho más hondo que un curso genérico.
2. Las transferencias **fuertes** son doce, y las tres que más rinden son: la **ficha de criterio**
   (C1), la **muestra apartada** de casos de prueba (C4) y la **prueba ciega** (C5/EP-08).
3. La advertencia que organiza el curso entero se deduce de algo que ya sabe: **un modelo de lenguaje
   maximiza la validez aparente**, que es precisamente la que en psicometría no es evidencia de nada.
4. El primer proyecto recomendado por los otros documentos —análisis de las encuestas de satisfacción,
   P27— es también el que más solapa con su formación (análisis de contenido, libro de códigos,
   diseño de cuestionario, estilos de respuesta culturales). La convergencia por tres caminos
   independientes es la mejor confirmación de que es el proyecto correcto.
5. Hay **nueve falsos amigos**, y dos son peligrosos de verdad: tratar los fallos del modelo como
   sesgos cognitivos, y confundir el consentimiento informado de investigación con la base jurídica
   del RGPD.
6. El riesgo del perfil no es la falta de rigor, es el exceso. **El montaje se hace rápido; el rigor
   se gasta entero en la evaluación.**

---

## 12. Estado de verificación de las fuentes

Este documento no se apoya en fuentes recuperadas en esta sesión: se apoya en el cuerpo estándar de la
metodología de la Psicología, que es materia de licenciatura, y su valor no depende de la cita
concreta sino de que la transferencia funcione. Se señalan aquí las referencias de apoyo y su estado,
por si el material final quiere citarlas.

| Idea | Referencia habitual | Estado |
|---|---|---|
| Amenazas a la validez interna del diseño pre-post | Campbell y Stanley | Canónica, no verificada en sesión |
| Deficiencia, contaminación y relevancia del criterio | Tradición de psicología del trabajo (problema del criterio) | Canónica |
| Escalas con anclas conductuales (BARS) | Smith y Kendall | Canónica |
| Validez de contenido y juicio de expertos | Lawshe (CVR), Aiken (V) | Canónica |
| Acuerdo entre jueces corregido por azar | Cohen (kappa) | Canónica |
| Análisis de contenido y libro de códigos | Krippendorff | Canónica |
| Fluidez de procesamiento y juicio de verdad | Reber y Schwarz; Alter y Oppenheimer | Canónica |
| Efecto halo en evaluación del desempeño | Tradición de psicología del trabajo | Canónica |
| Sesgo de automatización, errores de omisión y comisión | Factores humanos (Mosier y Skitka; Parasuraman y Riley) | Canónica |
| Preguntas sugestivas y memoria | Loftus | Canónica |
| Límites del acceso introspectivo al propio procedimiento | Nisbett y Wilson (1977) | **Discutida en su versión fuerte.** La consecuencia práctica no depende de ella |
| Regla del pico y el final en el juicio retrospectivo | Kahneman y colaboradores | Canónica, con límites de generalización |
| Estilos de respuesta extremo/moderado por cultura | Literatura transcultural de encuesta (p. ej. Harzing) | Canónica en el principio; **[NV]** en cualquier detalle por nacionalidad |
| Satisfacción como desconfirmación de expectativas | Oliver | Canónica |
| Justicia organizacional en tres componentes | Tradición de justicia organizacional (p. ej. Colquitt) | Canónica |
| Paradoja de la recuperación del servicio | Literatura de *service recovery* | **Discutida y no replicable de forma consistente. No construir nada sobre ella** |

Lo que sí está verificado y es de esta casa: los procesos P01–P32 y sus riesgos vienen de
`dominio-academia.md`; el marco de datos, de `dominio-rgpd.md`; la escalera y los límites de
plataforma, de `dominio-herramientas.md`; el método de los cinco pasos y sus citas, de
`01-analisis-referencia.md`.
