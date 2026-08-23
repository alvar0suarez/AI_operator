# Arquitectura 2 — «El inventario de su semana manda»

**Ángulo:** el mapa de sus tareas reales dirige el temario, el orden y los ejemplos.
**Brief:** `00-perfil.md`, revisado por segunda vez el 22.08.2026. Manda sobre este documento.
**Fecha:** 22.08.2026.

**Documentos que da por leídos:** `00-perfil.md`, `01-analisis-referencia.md`, `dominio-academia.md`
(P01–P32), `dominio-rgpd.md` (E-01…E-06, semáforo), `dominio-herramientas.md` (escalones 0–4 y límites
de plataforma verificados), `dominio-autodidacta.md` (mecanismos de corrección, puntos de caída,
plantillas), `dominio-psicologia.md` (EP-01…EP-14, correspondencias y falsos amigos), y los borradores
`borrador-arq-1-escalera.md` y `borrador-arq-2-inventario.md`, escritos bajo el brief anterior.

**Qué corrige este documento respecto al borrador anterior de este mismo ángulo.** Dos errores, los dos
de primer orden:

1. **El borrador hacía de Gemini el eje** («herramienta troncal: Gemini dentro de Google Workspace»),
   con módulos titulados por producto. Aquí Gemini es **el entorno donde practica**, no el eje. Los
   módulos se titulan por **capacidad**, el criterio va separado físicamente de los clics, y el curso
   incorpora un mecanismo explícito de portabilidad entre herramientas.
2. **El borrador eliminaba la evangelización interna.** Vuelve, como **módulo adicional** —no como
   columna vertebral— y con el encuadre correcto: **evidenciar y contagiar, no pedir permiso.**

**Convención de marcas:** **[V]** verificado en fuente primaria · **[R]** reconstrucción razonada ·
**[NV]** no verificable desde fuera · **[!]** decisión que no es suya y se escala · **[J]** juicio de
diseño mío, sin respaldo externo.

---

## 0. Resumen en catorce líneas

1. El curso no empieza por la IA ni por un catálogo. Empieza por **su semana**, levantada con un
   instrumento y no de memoria.
2. Ese inventario —el **Semanario**— no es un preámbulo: es **el índice**. Cada módulo posterior existe
   porque una fila del Semanario lo pidió.
3. «Saber qué existe» se enseña asignando a cada tarea suya **uno de seis veredictos**. El catálogo se
   aprende porque hay que usarlo doce veces sobre su propio trabajo.
4. Dos de los seis veredictos son **«no metas IA aquí»**, y una regla obliga a que al menos cuatro de
   doce tareas acaben ahí. El «no» hay que encontrarlo, no evitarlo.
5. **El curso es agnóstico de herramienta y el material lo demuestra físicamente:** el criterio vive en
   un fichero y los clics en otro, reemplazable, fechado y por herramienta.
6. Cada módulo produce una **ficha de capacidad** escrita por ella: qué hace esa capacidad, para qué le
   sirve en su semana, cuál es su techo, cómo sabe que funciona — y una sola línea perecedera con cómo
   se llama hoy en su entorno. Nueve fichas = el curso entero, en su lenguaje, sin nombres de producto.
7. Tres veces en el curso hace una **prueba de portabilidad**: reconstruir lo mismo en otra herramienta
   y anotar qué viajó y qué hubo que rehacer. Es la agnosticidad demostrada, no prometida.
8. La escalera del perfil se respeta literalmente: chat mejor usado (M0–M2) → automatizaciones (M3–M5)
   → juicio dentro del flujo, que es lo que en su caso significa «agente» (M6) → avanzado, apéndice de
   lectura opcional.
9. La protección de datos no es un módulo: es **la columna 8 del Semanario**, rellenada doce veces, más
   tres capas pegadas al momento en que desbloquean algo.
10. **La evangelización interna es el módulo M8**, va después de medir, y produce cuatro artefactos:
    dossier de una página, demo de tres minutos, piloto con otra persona y ficha de traspaso.
11. Todo entregable se corrige **sin nadie**: ejecución real, batería con clave sellada, lista binaria
    observable o rúbrica con criterios negativos. La IA correctora es el puesto 6 de 9 y va con
    protocolo y con control positivo.
12. Seis puntos de consulta de diez minutos con su pareja, con ficha escrita antes y **alternativa
    degradada** en todos.
13. Nueve módulos, **19 semanas**, dos horas propias por semana, arranque en octubre. Y una frontera
    declarada: al acabar M6 ya hay curso; M7–M8 es donde se cobran los objetivos 4 y 5.
14. Fuera: pedir permiso, portfolio, landing, cambio de rol, catálogos de producto, comparativas de
    modelos y cualquier cosa vistosa.

---

# 1. TESIS

## 1.1 Enunciado

> **Un catálogo abstracto de «esto es un agente, esto una automatización» se olvida en una semana. El
> mismo catálogo colgado de sus veinte tareas reales se queda, porque deja de ser información y pasa a
> ser una decisión que ella ha tomado y firmado sobre su propio trabajo.**
>
> **Y lo que se lleva puesto no es el catálogo: es el juicio.** Por eso el curso no entrena el manejo de
> un producto, entrena la operación de mirar un proceso y decidir qué clase de solución le corresponde
> —incluida ninguna—. Esa operación se automatiza en su cabeza repitiéndola sobre decenas de casos
> propios, y viaja con ella a cualquier otra empresa y a cualquier herramienta que exista en 2029.

Dos corolarios que convierten la tesis en arquitectura:

> **(a) El inventario no es el módulo 1: es el índice.** El orden de los módulos es el orden de la cola
> de tareas que el Semanario produce, no el orden de un temario.
>
> **(b) Las unidades del curso son capacidades, no productos.** Un módulo se llama «Que pase algo sin
> que yo lo pida», no «Acciones programadas». La capacidad es lo que dura; el producto es la
> implementación de hoy, y vive en un apéndice fechado y reemplazable.

## 1.2 Por qué es la correcta para ESTA alumna con ESTOS objetivos

Seis argumentos, en orden de peso. Los cuatro primeros son específicos de ella: con otro perfil no
serían igual de fuertes.

**(a) Es la única forma de cumplir el objetivo 1 sin fabricar un catálogo muerto.**
El perfil pide «saber qué existe: que existen agentes, que existen automatizaciones, **qué se puede
automatizar de su trabajo y qué no**». Los tres términos van pegados a *su trabajo*. No pide un mapa
del sector: pide un mapa de su semana. Un curso que conteste con un recorrido de productos está
contestando a otra pregunta, y además contesta con la mitad que caduca.

**(b) Es la única forma de cumplir el objetivo 4 —criterio portátil— con un mecanismo y no con una
promesa.** El criterio no se transmite explicándolo: se entrena repitiendo el juicio. Doce veredictos
en el M1, más un caso satélite por módulo, más la segunda vuelta del Semanario en el M7, dan **más de
treinta juicios** sobre procesos reales en 19 semanas. Ese número es el mecanismo. Y como los
veredictos están formulados en capacidades y no en productos, el juicio entrenado sobrevive al cambio
de herramienta y al cambio de empresa, que es literalmente lo que ella pide.

**(c) Ataca el problema real, que no es la ignorancia de herramientas sino la ausencia de mapa.**
El diagnóstico del webinar de referencia es exacto y merece abrir el curso: *«el problema no está en el
modelo; el problema es que cada vez le explicas tu empresa desde cero»*. Pero hay un paso previo que la
referencia no da, porque su alumno tipo quiere entrar en el sector de la IA y la nuestra no: **antes de
explicarle la empresa a un sistema, hay que tenerla escrita en algún sitio**. Y en una academia de
treinta personas donde «una misma persona atiende el teléfono, contesta el buzón compartido, resuelve
una incidencia de alojamiento y emite una carta de visado en la misma hora» (`dominio-academia.md`
§0.2), eso no está escrito en ningún sitio. **El Semanario es el primer documento de contexto de empresa
que existe, y lo escribe la única persona que puede escribirlo.**

**(d) Es el uso más rentable de su formación, sin halagarla.**
Un inventario con conteo real, cronometraje por unidad y columnas observables **es un registro de
conducta con muestreo de eventos**, y una línea base. Eso es materia de licenciatura de Psicología y lo
hará mejor que un ingeniero (`dominio-psicologia.md` C7). Y hay que decirle en la misma página que **la
parte de montar un flujo no se la da su formación en absoluto** (§6 del mismo documento), porque sin esa
segunda mitad la primera es adulación.

**(e) Resuelve la corrección sin mentor, que es donde se juega el diseño.**
Un curso autodidacta no puede evaluar «¿tu asistente está bien?». Pero sí puede evaluar «¿la fila 7 de
tu Semanario tiene cero palotes?» o «¿hay alguna fila con la columna 9 en “dinero, plazo legal o
visado” sin el tachón de zona prohibida?». **El inventario convierte gran parte de la evaluación en
comprobación**, que es el mecanismo 1–3 de `dominio-autodidacta.md` §3.2, el que no necesita el juicio
de nadie. Un curso construido sobre un artefacto tabulado se autocorrige mucho mejor que uno construido
sobre prosa.

**(f) Elimina la competencia por el tiempo, que es la primera causa de abandono.**
Eriksson et al. lo titularon *«Time is the bottleneck»*: 21 de 34 abandonos mencionan el tiempo. La
contramedida no es motivacional, es estructural: **que el trabajo del curso sea trabajo del puesto**. El
Semanario es literalmente su semana; rellenarlo no compite con la jornada, la describe. Y el material
declara en cada sesión si es **tiempo propio** o **tiempo de trabajo**, porque sin esa distinción escrita
ella lo contabilizará todo como tiempo propio y el curso parecerá el doble de caro.

## 1.3 La corrección de brief que cambia la arquitectura: agnóstico de herramienta

Esto no es una capa de barniz sobre el diseño anterior. Cambia tres cosas estructurales:

| Qué cambia | Antes (borrador) | Ahora |
|---|---|---|
| **Título de los módulos** | Por producto: «la columna `=AI()`», «Workspace Studio» | Por capacidad: «que pase algo sin que yo lo pida», «disparador, paso, condición» |
| **Unidad de contenido** | La lección, con criterio y clics mezclados | **Dos ficheros**: `leccion.md` (criterio, sin fecha, sin nombres de producto) y `clics-<herramienta>.md` (fechado, reemplazable, uno por herramienta) |
| **Entregable de aprendizaje** | El artefacto | El artefacto **más su ficha de capacidad**, escrita por ella, sin nombres de producto salvo una línea |
| **Prueba de que es agnóstico** | Una declaración en la introducción | **Tres pruebas de portabilidad ejecutadas**, una por escalón, con entregable |

Y un listón de admisión, aplicado a cada párrafo del material:

> **¿Le seguirá sirviendo dentro de dos o tres años?** Si no, o va al apéndice de clics, o no entra.
> Nada por estar de moda. Y la prueba operativa que decide en qué mitad va una frase:
> **¿deja de ser cierta si mañana renombran un producto, o si mañana trabaja con otra herramienta?**
> Si la respuesta es sí, la frase está en la mitad equivocada.

**Lo único específico de su entorno que hay que resolver pronto** —y va en la semana 1— es qué plan de
Gemini tiene contratada la empresa y cómo está configurado, porque de eso depende qué puede meter ahí
dentro. Y hasta eso se enseña agnóstico: las **cuatro preguntas que definen cualquier plan de cualquier
proveedor** son criterio; la ruta para averiguarlas en la consola de Google es clic. Ver §5.4.

## 1.4 La corrección de brief que añade un módulo: evangelización interna

Su empresa empuja la IA con bastante desconocimiento de lo que se puede hacer. Ella **no necesita
permiso** —usar IA está bien visto y lo mal visto es no automatizar—. Lo que necesita es saber
**evidenciar el valor** de lo que monta y **arrancar un proyecto de forma que después la organización lo
adopte**. Demostrar y arrastrar.

Consecuencias de diseño, y las tres son restricciones, no adornos:

1. **Va después de medir, no antes.** No se evangeliza lo que no está medido; un número inventado quema
   los tres proyectos siguientes. M8 consume la salida de M7.
2. **Es un módulo, no una lente.** No se reescribe el resto del curso «pensando en el público interno».
   Si la evangelización fuera la columna vertebral, el curso dejaría de ser sobre su trabajo y pasaría a
   ser sobre su reputación, que es exactamente el error del itinerario no técnico de la referencia.
3. **Pero deja un hilo barato desde la semana 1:** el **Cuaderno de evidencias**, tres líneas por
   módulo. Sin ese hilo, M8 sería «fabricar pruebas al final», que es lo mismo que inventarlas.

## 1.5 Lo que esta tesis rechaza, y por qué

| Alternativa | Por qué se rechaza |
|---|---|
| **Empezar por un recorrido de lo que existe** (chat, asistentes, cuadernos, flujos, agentes, MCP) | Es el catálogo muerto. Se lee cómodo, produce sensación de aprendizaje —que es un mal indicador (Deslauriers)— y a los diez días no queda nada porque no cuelga de nada suyo. Además es la mitad del material que caduca |
| **Empezar por «elige un proyecto y móntalo»** (el atajo de la referencia) | Elegir bien exige el criterio que el curso todavía no ha dado. Sin inventario elegirá **lo que más duele**, que en su puesto es el matching de alojamiento (P17) o el calendario de camas (P22): categorías especiales del RGPD y riesgo crítico. Es la trampa perfecta |
| **Empezar por protección de datos** | Un bloque legal de apertura produce parálisis, y el objetivo es que use **más** IA, en el sitio correcto |
| **Ordenar el curso por la escalera de herramientas** (la arquitectura 1) | Es un buen diseño y produce tres tutoriales encadenados si se descuida. Su propia autocrítica lo dice: *«ordena el curso por autonomía de la herramienta, no por dificultad del criterio»*. Con el brief agnóstico corregido, ese riesgo sube, no baja |
| **Seguir los cinco pasos de la referencia como columna vertebral** | Son correctos y se usan —el Semanario *es* su paso 2 y M7 *es* su paso 5—, pero su orden asume cohorte, mentores, dos públicos y un alumno que quiere cambiar de sector |
| **Hacer el curso «multiherramienta» de verdad, montándolo todo dos veces** | Duplicaría la fricción y produciría competencia en ninguna. La agnosticidad se consigue con **vocabulario de capacidades + tres pruebas de portabilidad acotadas**, no practicando en dos sitios a la vez. Ver la autocrítica §14.1 |

---

# 2. RESULTADOS DE APRENDIZAJE OBSERVABLES

Verbos de desempeño. Cada uno con su evidencia observable y el módulo donde se cierra. Ninguno dice
«entenderá», «conocerá» ni «será capaz de valorar».

| # | Al terminar, ella… | Evidencia observable | Cierra en |
|---|---|---|---|
| **RA1** | **Levanta** el inventario de su semana con conteo real y cronometraje por unidad, no de memoria | Semanario con ≥18 filas, 5 días de palotes y 3 tareas cronometradas 3 veces cada una | M0 |
| **RA2** | **Determina** bajo qué régimen de datos trabaja: qué plan, qué licencia, qué retención, qué política escrita — **o documenta** a quién y cuándo lo preguntó | Ficha E-01 con las 8 casillas y **ninguna frase que empiece por «creo que»** | M0 |
| **RA3** | **Asigna** a cada una de sus doce tareas de más peso uno de seis veredictos y **justifica** cada uno citando una columna concreta del Semanario | Mapa de la semana firmado y fechado; doce filas; una frase de justificación por fila que menciona una columna | M1 |
| **RA4** | **Rechaza** por escrito al menos cuatro tareas —por no necesitar IA, por no tener fuente de verdad o por zona prohibida— y **nombra**, para cada una, qué sí se puede hacer alrededor | ≥4 filas con veredicto 1, 2 o ZP, cada una con su casilla «lo que sí» rellena con un artefacto nombrable | M1 |
| **RA5** | **Escribe** el criterio de «resultado correcto» de una tarea suya en 4–6 indicadores que otra persona pueda comprobar sí/no contra una fuente, **antes** de tocar ninguna herramienta | Ficha de criterio de una cara, sin *adecuado, correcto, natural, profesional, de calidad* sin ancla detrás | M2 |
| **RA6** | **Construye** una batería de 10 casos —5 típicos, 3 límite, 2 de rechazo— con casos apartados **antes** de escribir el prompt, y la **vuelve a pasar** con fecha cada vez que cambia algo | `casos.md` + `CLAVE.md` sellada + hoja de anclas con una columna por fecha | M2 → M7 |
| **RA7** | **Monta** un asistente reutilizable con fuentes propias que **cita el documento y su fecha** y que **responde «no lo sé»** a lo que está fuera de alcance | 5/5 en típicos, pide aclaración en los 3 límite, «no lo sé» en los 2 de rechazo | M2 |
| **RA8** | **Reconstruye** una capacidad suya en una herramienta distinta y **nombra** qué viajó y qué hubo que rehacer | Ficha de portabilidad: lo que viajó (criterio, fuentes, batería), lo que no (dónde está el botón, el nombre), y el techo que sí cambió | M2, M4, M6 |
| **RA9** | **Audita a su propio corrector**: detecta los defectos plantados de un artefacto-cebo y **decide con ese dato** si la IA sirve para corregir ese tipo de trabajo | Hoja de resultado del cebo + decisión escrita + al menos un caso registrado en que **no** aceptó una crítica de la IA, con el motivo | M2, M6 |
| **RA10** | **Codifica** texto libre multilingüe con un libro de códigos cerrado y **compara** su codificación con la del sistema construyendo la tabla de confusión | ≥26/30 de acuerdo, una frase escrita por confusión repetida, y el acuerdo de la categoría minoritaria mirado aparte | M3 |
| **RA11** | **Monta** algo con disparador que **prepara, clasifica o avisa y nunca envía**, con condición de parada y tope de volumen, y **lo apaga habiéndolo probado** | El flujo se dispara con 5 casos fabricados y produce las 5 salidas correctas; la prueba de apagado está hecha, no imaginada | M4, M6 |
| **RA12** | **Distingue** en un proceso propio qué parte tiene pasos fijos y qué parte necesita juicio, y **argumenta por qué un agente autónomo sería exceso** | Media página con la frontera trazada y los dos puntos de juicio nombrados | M6 |
| **RA13** | **Reconoce** cuál es el único proceso de su academia que caería en el Anexo III del Reglamento de IA y **a quién lo escala** | Una frase, un nombre, un puesto | M6 |
| **RA14** | **Mide** el efecto de un sistema suyo en minutos por unidad, **resta** revisión y mantenimiento y **nombra** una amenaza a la validez que no puede descartar | Media página de evaluación por sistema, sin la palabra «significativo» | M7 |
| **RA15** | **Produce** un dossier de una página por artefacto cuyo número **puede reproducir con su método**, que dice también **qué NO hace** el artefacto y quién lo mantiene | Dossier de una cara; la reproducción del cálculo, hecha delante de sí misma dos semanas después, da el mismo número ±10 % | M8 |
| **RA16** | **Entrega** un artefacto suyo a otra persona, que lo usa una semana **sin ella**, y **corrige** lo que ese piloto revele | Ficha de traspaso + resultado del piloto + lista de lo que hubo que arreglar | M8 |
| **RA17** | **Explica** en treinta segundos, sin nombrar ninguna herramienta, qué hace uno de sus sistemas y qué vale | La prueba del pasillo, superada con alguien que no ha visto el artefacto | M8 |
| **RA18** | **Escribe la rúbrica** de un artefacto suyo, con ≥3 criterios negativos, y **la valida** contra un cebo | Si el cebo pasa su rúbrica, la rúbrica es blanda y se rehace | M9 |
| **RA19** | **Revisa** el Semanario seis meses después y **marca** qué veredictos han cambiado y por qué | Segunda hoja, mismas columnas, diferencias marcadas y motivadas | M7, M9 |
| **RA20** | **Sitúa** cada tipo de dato de su puesto en verde/ámbar/rojo y **reescribe** un caso real que sobrevive a la prueba de la compañera — y declara al menos uno **no reescribible** | 3 casos reescritos que **siguen produciendo una respuesta útil** + 1 declarado imposible | M0, M3 |

**Criterio de «curso terminado», definido en la semana 1 y observable:**

> Tres artefactos vivos que usa sin que el curso se lo pida · un Mapa de la semana con doce veredictos
> firmados · un Cuaderno de capacidades con nueve fichas escritas por ella · una rúbrica propia · y un
> artefacto que **otra persona** usa.

No es «leer la última lección». Y RA18 es el indicador honesto de que ya no necesita el material.

---

# 3. LOS TRES INSTRUMENTOS PERMANENTES

Van antes del mapa de módulos porque todos los módulos cuelgan de ellos. Son tres ficheros que viven
los diecinueve meses siguientes, no diecinueve semanas.

## 3.1 El Semanario — el inventario que manda

Una hoja de cálculo. Una fila por **tarea en forma de verbo** («contestar a un lead que pregunta
precio», no «admisiones»). Once columnas. Y la decisión que la hace viable: **solo tres columnas se
rellenan en vivo**; las otras ocho se rellenan en una única sesión de 45 minutos y solo para las doce
filas que sobreviven al filtro de volumen.

| # | Columna | Cuándo | Para qué sirve después |
|---|---|---|---|
| 1 | **Tarea, en verbo** | Pase A, día 2 | Es la unidad de todo |
| 2 | **Palotes** (5 días laborables) | En vivo, 3 min/día | Frecuencia **real**, no percibida |
| 3 | **Minutos por unidad** (3 mediciones) | En vivo, solo 3 tareas | Línea base para M7 |
| 4 | **Disparador** — qué la inicia | Sesión de cierre | Es el disparador del futuro flujo |
| 5 | **Fuentes que consulto** — qué documento abro | Sesión de cierre | Es el conocimiento del futuro asistente |
| 6 | **Salida** — qué produzco y adónde va | Sesión de cierre | Es el último paso del flujo |
| 7 | **¿Sale a un cliente?** sí / indirecto / no | Sesión de cierre | Decide si se puede automatizar la escritura |
| 8 | **Semáforo de datos** VERDE / ÁMBAR / ROJO | Sesión de cierre | Protección de datos integrada, no anexada |
| 9 | **Consecuencia del PEOR error** interna / molesta a un cliente / dinero-plazo-visado | Sesión de cierre | Riesgo, y de ahí la zona prohibida |
| 10 | **¿Los pasos son siempre los mismos?** sí / parcial / no | Sesión de cierre | El eje del árbol de decisión |
| 11 | **¿Sé cómo se hace bien?** perfectamente / más o menos / depende de otra persona | Sesión de cierre | Detecta la dependencia externa y el veredicto 2 |

**Columna 12, transversal y de una letra:** `V` si el volumen se multiplica en verano. Es la corrección
mínima a la estacionalidad brutal de su negocio —de 150 a 400 correos/día entre febrero y julio— y
cuesta una tecla.

**Se levanta en dos pases, y ninguno es un muro.**

**Pase A — cosecha retrospectiva. 25 minutos, día 2. No se escribe de memoria.**
La psicología dice por qué: *la gente describe sus procedimientos como cree que deberían ser, no como
los ejecuta* (`dominio-psicologia.md` C9), y los atajos y excepciones —que son justo lo que rompe una
automatización— no se verbalizan. Así que no se pregunta: se cosecha. Enviados de los últimos diez días
laborables (**solo asuntos y destinatarios, nunca cuerpos**); registro de llamadas del móvil de trabajo;
los diez últimos hilos de WhatsApp Business, solo el motivo; y el calendario, para lo que se repite.

> La restricción de «solo asuntos, nunca cuerpos» no es prudencia decorativa: es **la primera lección de
> minimización, enseñada haciendo**. Para saber qué tareas tiene no le hace falta ni un dato de un
> alumno. Ese descubrimiento vale más que tres páginas sobre el artículo 5.1.c.

**Pase B — muestreo prospectivo. Cinco días, tres minutos al día.** Un folio al lado de la pantalla. Un
palote por tarea ejecutada; una línea nueva cuando aparece una que no estaba. Corrige lo que el Pase A
no puede ver: las llamadas, el mostrador, el pasillo, el lunes de check-in. **Corre en paralelo mientras
se usa la victoria del día 1, y no bloquea nada.**

**Y viene medio hecho.** Los 32 procesos de `dominio-academia.md` no son material de referencia del
diseñador: **son la primera versión de su Semanario**, y así se le entregan. Su primera operación no es
escribir, es **tachar**: *«de estos 32, tacha los que en tu academia no ocurren o no llevas tú; corrige
los volúmenes; añade lo que falte»*. Reconocer es mucho más barato que recordar: una hoja en blanco
delante de alguien cansado un martes produce ocho filas y abandono; una lista de 32 para corregir
produce veinticinco filas en veinte minutos. Y cada tachadura es información de dominio que ningún curso
genérico podría darle hecha.

## 3.2 El Cuaderno de capacidades — el instrumento que hace el curso portátil

**Es la pieza nueva de esta arquitectura y la que ejecuta la corrección de brief.**

Cada módulo cierra con **una ficha de capacidad de una cara, escrita por ella**, con seis campos fijos:

```
FICHA DE CAPACIDAD nº __ · <nombre de la capacidad, en mis palabras>

1. QUÉ HACE            (dos frases. Sin nombres de producto.)
2. PARA QUÉ SIRVE       (qué filas de mi Semanario la piden, con su número de proceso)
   EN MI SEMANA
3. CUÁL ES SU TECHO     (qué es lo que NO puede hacer, y cómo se nota que has llegado)
4. CÓMO SÉ QUE          (la comprobación concreta: qué miro y qué tiene que salir)
   FUNCIONA
5. CUÁNDO NO USARLA     (la situación en la que es exceso, y qué usar en su lugar)
6. CÓMO SE LLAMA HOY    ← ÚNICA LÍNEA PERECEDERA. Con fecha. Se tacha y se reescribe.
   DONDE YO TRABAJO
```

Cuatro razones por las que este instrumento es el que resuelve el objetivo 4:

1. **Es el curso entero en su lenguaje y sin nombres de producto.** Nueve fichas, nueve caras. Si dentro
   de tres años cambia de empresa y de herramientas, el Cuaderno sigue siendo verdad **salvo nueve
   líneas**, y esas nueve líneas se reescriben en una tarde.
2. **El campo 3 —el techo— es lo que de verdad transfiere.** Las funciones cambian cada seis meses; los
   techos casi no. «Un asistente guardado recuerda sus instrucciones, no recuerda lo que pasó ayer» va a
   seguir siendo el modelo mental correcto cuando el producto se llame otra cosa, y es lo que le permite
   diagnosticar un problema en una herramienta que no ha visto nunca.
3. **El campo 6 enseña la convención del curso practicándola.** Ella misma aísla lo perecedero en una
   línea marcada. Es la separación criterio/clics aplicada a sus propias notas, y se aprende haciéndola,
   no leyéndola.
4. **Es autocorregible mecánicamente.** La lista de comprobación de cada ficha es binaria: *¿aparece
   algún nombre de producto fuera del campo 6? SÍ/NO* · *¿el campo 2 cita un número de proceso? SÍ/NO* ·
   *¿el campo 3 dice algo que la capacidad no puede hacer, no algo que ella todavía no sabe hacer?
   SÍ/NO* · *¿el campo 4 se puede contestar mirando? SÍ/NO*.

**Las nueve capacidades del curso** (y nótese que ninguna es un producto):

| # | Capacidad | Módulo |
|---|---|---|
| 1 | Contexto permanente: lo que no hay que volver a explicar nunca | M0 |
| 2 | Inventariar un proceso y clasificarlo | M1 |
| 3 | Criterio explícito de resultado correcto, escrito antes | M2 |
| 4 | Asistente reutilizable con fuentes propias, cita y «no lo sé» | M2 |
| 5 | Clasificación en lote con un libro de códigos cerrado | M3 |
| 6 | Disparador: que algo ocurra sin que tú lo pidas | M3 |
| 7 | Flujo: disparador, pasos y condiciones | M4–M5 |
| 8 | Juicio dentro del flujo, y sus límites de parada | M6 |
| 9 | Medir si sirve, y traspasarlo a otra persona | M7–M8 |

## 3.3 El Cuaderno de evidencias — el hilo barato de la evangelización

Tres líneas por módulo, escritas el día que el artefacto empieza a funcionar. Coste: dos minutos.

```
ARTEFACTO: ______        fecha: ______
- Qué hacía yo antes, y cuántos minutos por unidad:
- Qué hace ahora, y cuántos minutos por unidad:
- Qué NO hace, y qué sigo haciendo yo:
```

Existe desde la semana 2 por una razón operativa, no ceremonial: **si el M8 tuviera que fabricar las
pruebas al final, las inventaría.** Un número reconstruido de memoria en la semana 17 no es un número, y
el módulo de evangelización se apoya entero en que sus números sean reproducibles. La tercera línea
—*qué NO hace*— es la que después hace creíble a todo el dossier: quien enumera los límites de su propio
sistema se gana el derecho a que le crean el resto.

## 3.4 Los seis veredictos — el catálogo, colgado de sus tareas

Cada fila del top 12 recibe **uno** de estos seis. Es el árbol de decisión de la referencia, corregido en
dos sitios donde su versión se queda corta, y reescrito en capacidades para que no caduque.

| # | Veredicto | Prueba que lo decide | Capacidad que le corresponde | Ejemplos suyos |
|---|---|---|---|---|
| **1** | **NI IA** | **La servilleta:** ¿podrías escribir los pasos en una servilleta y valdrían siempre? | Fórmula, plantilla o calendario. Ninguna capacidad de IA | **P02** presupuestos (aritmética sobre una tabla) · **P22** calendario de camas (calendario de recursos) · **P16** exámenes DELE (un plazo con alarma) |
| **2** | **ARREGLAR EL PROCESO PRIMERO** | La columna 5 dice «pregunto a alguien», «el de siempre», o hay dos versiones y no sabes cuál manda | Ninguna todavía. Falta fuente de verdad | **P32** plantillas en seis idiomas sin control de versiones · cualquier tarea cuyo tarifario vigente ella no pueda nombrar |
| **3** | **CHAT, MEJOR USADO** | Poca frecuencia + mucho juicio + conocimiento que no se repite | Contexto permanente (cap. 1) | **P13** cambios de grupo · **P31** redactar el comentario del informe mensual |
| **4** | **ASISTENTE GUARDADO CON FUENTES** | Se repite, el conocimiento está escrito y es estable, el juicio sigue siendo suyo | Asistente reutilizable con cita (cap. 4) | **P01** las seis preguntas que repite el 70–80 % de los leads · **P10** certificados |
| **5** | **DISPARADOR Y PASOS FIJOS** | Hay un disparador identificable **y** los pasos son siempre los mismos | Flujo (cap. 7) | **P27** encuestas · **P30** parte semanal · **P06** recordatorio de pagos |
| **6** | **FLUJO CON JUICIO** | Hay disparador, pero en dos o tres puntos hay que **evaluar** algo para saber por dónde seguir | Juicio dentro del flujo (cap. 8) | **P28** triaje de reseñas · **P20** clasificar y enrutar incidencias (nunca responderlas) |
| **ZP** | **ZONA PROHIBIDA** — no es un veredicto, es un tachón encima del que hubiera | Columna 9 = «dinero, plazo legal o visado», o columna 8 = ROJO irreducible | — | **P08** visados · **P26** quejas formales · **P29** emergencias · **P25** reembolsos · **P17** matching con familias · **P22** overbooking |

**Y una séptima categoría que deliberadamente NO es un veredicto: el agente autónomo.** Se define, se
explica y se le pone su condición de activación, pero **no está en la lista de destinos posibles para una
tarea suya**, y eso se dice con todas las letras. El motivo es pedagógico y verificable: el error número
uno al clasificar es poner «agente» a todo, porque es la palabra que suena a solución completa y es lo
que promete internet. Sacarlo de la lista de opciones obliga a decidir entre las seis que sí existen para
ella, y luego el M6 explica exactamente qué es lo que se ha quedado fuera y qué tendría que cambiar.

**Las dos correcciones a la referencia, y por qué importan:**

- **El veredicto 1 existe con nombre propio y va el primero.** La referencia lo menciona de pasada
  («escanear una factura y pasarla a Excel no necesita IA»). Aquí es el primer destino de la lista y el
  ejemplo canónico es suyo: el presupuesto (P02) es riesgo Alto, 2.500–3.500 al año, y es aritmética
  pura. Meter un modelo de lenguaje ahí no es ineficiente: **es introducir un error posible donde no lo
  había.**
- **El veredicto 2 no existe en ningún curso de IA y es el que más le va a salir.** «Arreglar el proceso
  primero» es el diagnóstico correcto de P32 y de media docena de filas más. Y tiene una virtud
  pedagógica enorme: **es un hallazgo que aportar, no un fracaso.** En una empresa donde lo mal visto es
  no automatizar, llegar diciendo *«esto no se puede automatizar todavía porque no sabemos cuál es el
  tarifario vigente en alemán»* es trabajo de valor. De hecho es la primera entrada de su Cuaderno de
  evidencias y el germen del artefacto de M9.

## 3.5 La regla del cuatro

> **De tus doce filas, al menos cuatro tienen que acabar en veredicto 1, veredicto 2 o zona prohibida.
> Si tienes menos de cuatro, no has clasificado: has hecho una lista de deseos. Vuelve.**

Es un forzador deliberado y su justificación es empírica: cruzando los 32 procesos de
`dominio-academia.md` con lo que la plataforma puede hacer de verdad (`dominio-herramientas.md` §3.3),
**el reparto real de una academia como la suya da entre cinco y siete noes de doce**. Cuatro es un suelo
prudente, no una cuota inventada.

Su función psicológica es la importante: convierte el «no» en algo que hay que **encontrar**. Y desactiva
de raíz el sesgo que produce un curso de IA por su mera existencia — preguntarle a un curso de IA si algo
debe hacerse con IA tiene un sesgo obvio hacia el sí. *(Sobre el riesgo de que una cuota fabrique noes de
conveniencia, ver §14.6.)*

---

# 4. MAPA DE MÓDULOS

Nueve módulos, **19 semanas**, **2 h propias/semana** más el trabajo que es trabajo del puesto. Arranque
en **octubre**: el pico de junio–septiembre de la academia (250–400 correos/día) mata cualquier
calendario que lo ignore, y noviembre–febrero es su temporada baja.

**Una frontera declarada desde la semana 1, y esto es diseño anti-abandono, no una rebaja:**

> **Al final de M6 (semana 14) ya hay curso**: tres artefactos vivos, un mapa de doce veredictos y ocho
> fichas de capacidad. **M7 y M8 son donde se cobran los objetivos 4 y 5** —criterio portátil y
> evangelización— y son la parte que más rinde a doce meses vista. Decirlo así, y no fingir que las
> diecinueve semanas son un bloque indivisible, es lo que evita que la semana 15 se lea como fracaso.

Formato de cada ficha: **título · cambio mental · qué construye · duración realista · qué capacidad
entrena y cómo se enseña de forma transferible · cómo se autocorrige sin mentor**.

---

## M0 · El primer atajo, y el suelo que piso (semanas 1–2)

**Cambio mental.** *«La IA no es una ventana donde se pregunta. Es algo que se deja montado y que sigue
ahí mañana.»* Y el segundo, que llega el día 2: *«lo primero que hay que mapear no es la IA: es tu
semana.»* Y el tercero, incómodo y necesario: *«el mismo texto en la misma pantalla es seguro o no según
con qué cuenta hayas entrado.»*

**Qué construye.**
1. **Día 1, 25 minutos: un asistente de consulta con tres fuentes verdes.** Instrucciones guardadas +
   tarifario vigente, calendario académico y condiciones generales como conocimiento adjunto, que
   contesta las seis preguntas que repite el 70–80 % de los leads **citando de qué documento sale cada
   dato**. Cero datos personales: tarifas, calendario y condiciones **no son datos personales**. Se usa
   esa misma tarde, y se cronometra antes y después.
2. **Día 2: el Pase A del Semanario**, tachando sobre la lista de 32 procesos que trae el curso.
3. **Días 3–10: el Pase B**, tres minutos diarios de palotes + tres tareas cronometradas.
4. **La ficha del plan (E-01)**: qué edición, si su cuenta tiene licencia, qué retención, si hay política
   escrita. Con los cuatro mensajes literales para copiar y pegar y las cinco comprobaciones empíricas
   por si nadie contesta.
5. **La tarjeta del lunes**: el semáforo VERDE/ÁMBAR/ROJO impreso al lado de la pantalla.
6. **Ficha de capacidad nº 1** — contexto permanente.

**Duración realista.** 2 semanas. **~2 h de tiempo propio en total** (25 min el día 1 + 45 min el día 2 +
25 min de E-01 + una sesión de 35 min), más 3 min/día de palotes y el cronometraje, que **son tiempo de
trabajo**. El material lo declara así, línea a línea.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad 1: **contexto permanente** — la idea de que hay conocimiento que no se vuelve a explicar nunca
porque vive en un sitio que tú controlas. Se enseña transferible con tres piezas:
- **El techo, declarado el primer día:** un asistente guardado recuerda sus instrucciones, **no recuerda
  lo que pasó ayer**. La memoria fiable es un fichero, no una sensación. Eso será verdad en cualquier
  herramienta durante años.
- **La tabla de tres nombres** (§5.3): la misma capacidad, con su nombre de hoy en las tres herramientas
  que ella ya conoce. Aparece una vez, en el apéndice, y no vuelve al cuerpo.
- **Las cuatro preguntas que definen cualquier plan** (§5.4) en lugar de la tabla de planes de Google. Es
  el ejemplo más limpio del curso de criterio frente a clic, y va el primero a propósito.

**Cómo se autocorrige.**
- **Ejecución real (mecanismo 1).** El asistente existe y responde, o no. Binario.
- **Batería sellada de 10 preguntas escritas ANTES de montarlo.** 5 con respuesta en las fuentes, 3
  ambiguas a propósito, 2 fuera de alcance. La clave la escribe ella el mismo día, en un fichero aparte
  que no reabre hasta el final. **Umbral:** falla >0 de las 5 → no está listo; se inventa una decisión en
  alguna de las 3 → no está listo; contesta algo distinto de «no lo sé» en alguna de las 2 → no está
  listo.
- **La pantalla corrige el plan.** Las cinco comprobaciones empíricas se corrigen solas: la pantalla
  contesta. Y enseñan de paso que **la documentación dice una cosa y la instancia dice otra, y manda la
  instancia** — que es exactamente lo que necesitará saber cuando el material envejezca.
- **Rúbrica de E-01, ocho casillas,** con un estándar de suspenso brutal y muy útil: **si en algún punto
  has escrito «creo que», «supongo que» o «me suena que», está mal resuelto.** «No lo sé y lo pregunté el
  día 14» sí vale. Distinguir lo que sabes de lo que supones es el mismo estándar que necesitará para
  evaluar respuestas de una IA, y por eso va el primero.
- **Cronómetro.** Minutos por unidad, tres mediciones. No admite interpretación.

**Caja obligatoria «lo que vas a ver la primera vez».** *«Vas a descubrir que no sabes con certeza cuál
es el tarifario vigente, o vas a encontrar tres versiones. Eso no es un fallo del ejercicio: es el primer
hallazgo del curso, es una fila del Semanario con veredicto 2, y es la primera entrada de tu Cuaderno de
evidencias.»*

---

## M1 · El veredicto: seis destinos para una tarea (semanas 3–4)

**Cambio mental.** *«No hay una respuesta “usar IA”. Hay seis destinos posibles para una tarea, y dos de
ellos son no usarla. Saber cuál toca es la competencia; las herramientas son el detalle.»*

**Qué construye.** **El Mapa de la semana:** doce filas, cada una con su veredicto, una frase de
justificación que cita una columna concreta, y —para los noes— la casilla **«lo que sí se puede hacer
alrededor»**. Firmado y fechado. Más **la cola de ataque**: las doce filas reordenadas por
`palotes × minutos ÷ riesgo`, que es el orden en que se abordan de M2 a M6. Más la **ficha de capacidad
nº 2**.

**Duración realista.** 2 semanas. Una sesión de 45 min para cerrar las ocho columnas del top 12, dos
sesiones núcleo de 40 min para los veredictos, una para el cebo.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad 2: **inventariar un proceso y clasificarlo**. Es la capacidad más portátil del curso entero y
la que ella pide con el nombre de «criterio portátil». Se enseña transferible por construcción:
- **Los seis veredictos están formulados como capacidades, no como productos.** El veredicto 4 no es «un
  Gem»: es «un asistente guardado con fuentes propias». Esa formulación es la que sigue siendo cierta
  cuando cambie de empresa y de herramienta.
- **Las pruebas que deciden cada veredicto son preguntas sobre la tarea, no sobre la herramienta.** «¿Cabe
  en una servilleta?», «¿puedes nombrar el documento y su fecha?», «¿los pasos son siempre los mismos?».
  Ninguna se puede contestar mirando un menú, y ninguna caduca.
- **Casos satélite desde aquí:** cada módulo posterior lleva un ejercicio de 15 minutos que aplica el
  mismo juicio a un proceso **que no es el suyo del hilo**. Es la contramedida a que el criterio se pegue
  al caso (`dominio-autodidacta.md` §7.3).

**Herramienta y por qué: ninguna nueva. Una hoja de cálculo y un lápiz.** Es deliberado y hay que
decirlo en el material: *el instrumento que decide qué se automatiza no puede vivir dentro de la
herramienta que va a automatizar.* Si el Mapa vive dentro de Gemini, Gemini opina sobre su propio
alcance.

**Cómo se autocorrige.**
- **Lista de comprobación binaria, doce ítems observables.** Dos personas distintas darían la misma
  respuesta sin discutir: *¿hay alguna fila del top 12 con cero palotes?* · *¿hay alguna fila cuya
  columna «fuentes que consulto» esté vacía?* · *¿hay al menos cuatro veredictos 1, 2 o ZP?* · *¿cada
  veredicto menciona una columna concreta?* · *¿alguna fila describe un departamento en vez de un verbo?*
  · *¿hay más de tres veredictos 6?* · *¿alguna fila con la columna 9 en «dinero, plazo legal o visado»
  no lleva el tachón?*
- **La comprobación más barata y la que más caza:** coger tres filas al azar y preguntarse *«¿la hice
  esta semana?»*. Si la respuesta es no en alguna, el inventario es aspiracional y hay que volver a los
  palotes.
- **El cebo del Mapa (control positivo).** El curso trae un Mapa de mentira, de una academia inventada,
  con **tres errores de clasificación plantados y documentados** en un fichero sellado: uno visible (una
  tarea determinista clasificada como flujo con juicio), uno de omisión (una tarea de riesgo crítico sin
  marcar como zona prohibida) y uno de criterio (una tarea sin fuente de verdad clasificada como
  automatizable). Ella lo corrige, anota, y **después** abre la hoja de defectos. Doble función: calibra
  su criterio **y** calibra su corrector.
- **Protocolo de corrección con IA**, siete reglas, primera aplicación: hilo nuevo · no digas que es tuyo
  · nunca «¿está bien?» sino «enumera los incumplimientos de esta rúbrica y cita textualmente el
  fragmento que los incumple» · pega la rúbrica entera · **prohibido discutir en el mismo hilo** · dos
  modelos, y el desacuerdo es la señal · su veredicto no cierra nada.
- **PC-2 aquí** (§7).

---

## M2 · El criterio antes del prompt, y el asistente que cita (semanas 5–6)

**Cambio mental.** *«La calidad no se pide: se define antes.»* Y la frase que abre el módulo y que es la
más rentable de todo el curso para este perfil:

> **Un modelo de lenguaje es el instrumento con la validez aparente más alta y la garantía de validez de
> contenido más baja que vas a manejar en tu vida. Está optimizado para producir texto plausible: la
> plausibilidad es su función objetivo, no un efecto secundario.**

No tiene que creerla por autoridad. La deduce de algo que sabe desde tercero de carrera.

**Qué construye.** Sobre la tarea nº 1 de su cola de ataque:
1. **La ficha de criterio** (EP-01): definición en una frase, 4–6 dimensiones, un indicador observable por
   dimensión, críticos marcados y punto de corte. Una cara.
2. **Las anclas de tono** (EP-02): tres frases completas —bajo, medio, alto— para dos dimensiones, sacadas
   de correos que envió de verdad. **Ese fichero es el contexto de tono del asistente**, no un
   calentamiento.
3. **Los diez apartados** (EP-06): diez casos reales sacados por orden cronológico —no elegidos— y
   cerrados antes de escribir una línea de prompt.
4. **La batería con tabla de especificaciones** (EP-03): matriz categoría × dificultad, con cupo fijo para
   los límite.
5. **El asistente v2 y su base de fuentes**, con **fecha de revisión en cada fuente**, cita del documento
   y regla de «no lo sé».
6. **La prueba de portabilidad nº 1** (ver abajo).
7. **Fichas de capacidad nº 3 y nº 4.**

**Duración realista.** 2 semanas. Es el módulo más denso en trabajo mental y el más ligero en clics.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidades 3 y 4: **criterio explícito** y **asistente reutilizable con fuentes, cita y «no lo sé»**.
Y aquí va el mecanismo central de la agnosticidad del curso:

> **PRUEBA DE PORTABILIDAD Nº 1 — 25 minutos, tiempo propio.**
> Reconstruye el mismo asistente en **otra herramienta** —ella ya usa ChatGPT por su cuenta— usando
> **solo material verde**: tarifario, calendario y condiciones generales, que no son datos personales.
> Pásale las mismas diez preguntas de la batería. Y rellena la ficha:
>
> | Qué viajó tal cual | Qué hubo que rehacer | Qué techo cambió |
> |---|---|---|
> | La ficha de criterio · las fuentes con su fecha · la batería de 10 casos · la regla de «no lo sé» | Dónde se guarda, cómo se llama, cuántos ficheros admite, dónde se pega la instrucción | Cuántas fuentes acepta · si cita el fragmento o solo el fichero · si conserva la instrucción entre sesiones |
>
> **Lo que se aprende no es «ChatGPT también sirve». Es que el 80 % de tu trabajo era el criterio y las
> fuentes, y eso no estaba dentro de ninguna herramienta.** Es la lección del curso que más falta hace
> dentro de dos años, y es la única forma de enseñarla que no es un sermón.
>
> **Restricción de datos, y es contenido:** la prueba se hace **con material verde exclusivamente**. Su
> cuenta personal de ChatGPT no tiene contrato de encargado del tratamiento, y por ahí no pasa ni un dato
> de un alumno. Que la prueba de portabilidad sea también un ejercicio de semáforo no es casualidad: es
> el diseño.

**Cómo se autocorrige.**
- **Ctrl+F sobre la ficha de criterio.** Si aparecen «adecuado», «correcto», «natural», «profesional» o
  «de calidad» sin un ancla detrás, no ha operacionalizado: ha renombrado el constructo. Autocorrección
  mecánica perfecta, cinco segundos.
- **Los diez apartados se abren al final y tiene que fallar al menos uno.** Si no falla ninguno, sospecha
  del muestreo antes que celebrar: *si tu batería la pasa entera a la primera, tu batería es fácil; no es
  que tu sistema sea bueno.*
- **Y el criterio no se toca.** Si al abrirlos le dan ganas de cambiar la ficha para que aprueben, **lo
  anota y no lo cambia**. Ese impulso es el dato más interesante del ejercicio y tiene nombre: sesgo del
  experimentador.
- **Lectura por columnas** (EP-05): comprobar el indicador 1 en las cinco salidas, luego el 2 en las
  cinco, y comparar con la lectura normal del tirón. Si por columnas encuentra más fallos —lo habitual—,
  el procedimiento se queda como rutina.
- **Segundo cebo, ahora sobre un asistente**, y **PC-3** justo después (§7): no se revisa su trabajo, se
  revisa **su instrumento de corrección**.
- **La prueba de portabilidad se corrige sola:** o las tres columnas de la ficha están rellenas con cosas
  concretas, o no lo están. Y hay un criterio negativo: *si la columna «qué viajó tal cual» está vacía,
  no construiste criterio: construiste un prompt.*
- **Checkpoint de divorcio.** Al final de M2, cambiar de tarea hilo es un movimiento **legítimo y
  preautorizado**, escrito desde la semana 1. No es un fracaso.

---

## M3 · Que pase algo sin que yo lo pida (semanas 7–8)

**Cambio mental.** *«Algo puede ocurrir sin que yo abra nada.»* Es el momento psicológico del curso, y
por eso llega en la semana 7 y no en la 14.

**Qué construye.**
1. **El libro de códigos** (EP-10): 5–8 categorías con definición operativa, criterios de inclusión y
   exclusión, dos ejemplos prototípicos y **dos ejemplos frontera con la decisión ya tomada y
   justificada**. Ese documento no es preparación para el prompt: **es el prompt.**
2. **Una clasificación en lote real**: los comentarios de la última encuesta de satisfacción (P27) con
   taxonomía cerrada, categoría de rechazo y regla de parada.
3. **Un disparador por horario**: un resumen semanal que le llega sin pedirlo.
4. **Capa 2 de protección de datos**: seudonimizar de verdad (cuasi-identificadores, no solo el nombre) y
   la regla de adjuntos.
5. **Fichas de capacidad nº 5 y nº 6.**

**Duración realista.** 2 semanas. La clasificación en lote es media hora; **el libro de códigos es lo que
cuesta, y es el trabajo que más rinde.**

**Por qué P27 y no otra cosa.** Cuatro análisis independientes convergen: es riesgo **bajo** (no hay
dinero, no hay plazo legal, no lo ve ningún cliente), es volumen **alto** (600–800 respuestas al año), es
el proceso **más multilingüe** de su lista (10+ idiomas), **hoy no se hace** porque nadie tiene tiempo —
así que no compite con un procedimiento establecido— y es el que **más solapa con su formación** (análisis
de contenido, libro de códigos, estilos de respuesta culturales). Que el proyecto más útil sea también el
más seguro es un regalo para el diseño, no una coincidencia buscada.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidades 5 y 6: **clasificación en lote** y **disparador**. Transferibilidad:
- **El libro de códigos es el artefacto portátil, no la implementación.** Se puede aplicar desde una
  fórmula de hoja de cálculo, desde un asistente pegando lotes de cuarenta, o desde un flujo. **La misma
  taxonomía funciona en las tres**, y el ejercicio obliga a decirlo: *«nombra dos formas distintas de
  aplicar tu libro de códigos a 600 filas y di qué cambia entre ellas»*. Lo que cambia es la comodidad y
  el volumen; lo que no cambia es la calidad de la clasificación.
- **El techo del disparador por horario, declarado:** dispara por calendario, **no reacciona a que haya
  pasado algo**. Un lunes no es un suceso; que entre un correo, sí. Ese techo es el que motiva el M4, y
  es una propiedad de la categoría, no de un producto.
- **Contingencia declarada por delante:** si su plan no incluye la función de hoja de cálculo, la ruta es
  el mismo libro de códigos aplicado en lotes de cuarenta desde el asistente. **Se pierde comodidad, no
  aprendizaje**, y se dice así. Aquí se cobra el diagnóstico del M0, y no es un fallo suyo ni del curso.

**Cómo se autocorrige.**
- **Doble codificación** (EP-07): clasifica **ella** 30 comentarios **antes** de ver la salida del
  sistema; después compara y construye la tabla de confusión. El oráculo es ella misma, preregistrada. Y
  la comprobación fina: mirar el acuerdo de la categoría **menos frecuente** por separado, porque un 95 %
  global con un 30 % en «administración» es una mentira útil para nadie.
- **El test del libro de códigos, con umbral por los dos lados:** aplicado cerrado a 40 comentarios
  nuevos, **menos del 15 % debe caer en «sin clasificar»**; si cae más, la taxonomía no cubre el dominio;
  **si cae 0 %, está forzando encajes**. Dos umbrales lo convierten en comprobación y no en opinión.
- **La clasificación se ejecuta o devuelve error**, cuarenta veces seguidas. Binario.
- **Lista de adjuntos, cinco ítems binarios:** *¿he abierto entero el fichero que voy a subir? ¿he hecho
  una copia y borrado filas, columnas y hojas que no hacen falta? ¿estoy subiendo el maestro? ¿hay algún
  documento de identidad? ¿hay una captura con la bandeja de fondo?*
- **PC-4 aquí** (§7): la prueba de la compañera sobre tres casos seudonimizados.

**Caso satélite (15 min).** P02, el presupuesto: se monta **con IA** y **con fórmula** sobre los mismos
veinte casos, se cronometra y se cuentan los errores. Gana la fórmula, y por goleada. Ver §8.2.

---

## M4 · Disparador, paso, condición (semanas 9–10)

**Cambio mental.** *«Un flujo no es un prompt largo. Es un disparador, unos pasos y unas condiciones — y
el paso 3 no ve lo que produjo el paso 1 salvo que se lo pases.»* Esto no se lo da su formación en
absoluto, y hay que decírselo con esas palabras: es nuevo, se aprende haciendo, y le va a costar los dos
primeros intentos (`dominio-psicologia.md` §6).

**Qué construye.** **El triaje del correo entrante:** clasifica lo que llega —lead, incidencia, visado,
pago, otro—, etiqueta, destaca lo urgente y le avisa si menciona visado, denegación o un menor. **Y no
contesta a nadie.** Regla escrita en el material: *este flujo solo ordena. Etiquetar es reversible;
enviar no.* Más la **ficha de capacidad nº 7** y la **prueba de portabilidad nº 2**.

**Duración realista.** 2 semanas, y es el módulo con más probabilidad de desbordarse. Presupuesto
honesto: dos sesiones de 45 min de tiempo propio más un bloque de proyecto de 90 min **en horario de
trabajo**.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad 7: **flujo**. La transferencia aquí es especialmente limpia porque **la anatomía de un flujo es
la misma en todas las herramientas de automatización que existen**: un disparador, una secuencia de
pasos, condiciones que bifurcan y un tope. Cambia el inventario de pasos disponibles y cambia dónde se
hace clic; no cambia la anatomía.

> **PRUEBA DE PORTABILIDAD Nº 2 — 20 minutos, sobre papel y documentación, sin dar de alta nada.**
> Escribe tu flujo en notación neutra —`DISPARADOR → PASO → PASO → CONDICIÓN → SALIDA`— y después busca,
> en la documentación de **otra** herramienta de automatización, dónde estaría cada pieza. Entregable de
> tres líneas: **las cinco piezas y su nombre allí**, **la pieza que allí no existe**, y **la pieza que
> allí es más fácil**.
>
> No se construye nada y no se da de alta ninguna cuenta: el objetivo es que compruebe que su flujo es
> describible sin nombrar un producto, y que localice el catálogo de pasos de una herramienta que no ha
> visto nunca. Esa segunda habilidad es la que usará dentro de tres años.

**Los límites, por delante y no al tercer intento fallido.** Va en la primera página del módulo, no en una
fe de erratas: **la automatización nativa de su entorno falla con unidades compartidas, carpetas
compartidas y hojas enlazadas** [V]; un solo disparador por flujo; tope de etiquetas visibles. Y el
centro de gravedad de su puesto **es un buzón compartido** (`info@`, `accommodation@`) y una hoja de camas
compartida. **Los primeros flujos se construyen sobre su propio buzón de empresa y sobre copias suyas, y
eso no es una versión de juguete: es la restricción real de la herramienta.** Decirlo en la lección 1 del
módulo, y no dejar que lo descubra, es lo que separa un material honesto de uno que la frustra.

**Cómo se autocorrige.**
- **El flujo se dispara o no se dispara.** El mecanismo más fiable que existe, y aquí está entero.
- **La prueba de los cinco correos fabricados.** Se manda a sí misma cinco correos inventados, uno por
  categoría, y mira las etiquetas. **Cinco etiquetas correctas o no las hay.** Comprobación pura, cero
  rúbrica. Y un sexto correo **que NO debe disparar**, que es el que casi nadie prueba.
- **Lista de comprobación de plataforma, seis ítems binarios**, escrita como síntomas y reutilizable como
  diagnóstico: *¿el fichero que toca el flujo está en una unidad compartida? ¿la hoja usa enlaces
  externos? ¿el flujo tiene más de un disparador? ¿hay algún paso que escriba fuera? ¿hay etiquetas que
  la interfaz no muestre por el tope? ¿lo he probado con un caso que debe NO disparar?*
- **La regla dura:** si algún paso envía algo a alguien que no sea ella, no está listo. Se comprueba
  mirando, no valorando.
- **PC-5, el comodín**, disponible desde aquí.

**Caso satélite (15 min).** P30, el parte semanal a dirección académica: determinista puro, sin modelo de
lenguaje en el camino crítico. La respuesta correcta es veredicto 5 con la mínima IA posible, y sirve para
ver que «automatizar» no siempre significa «meter un modelo».

---

## M5 · El flujo que reutiliza lo tuyo (semanas 11–12)

**Cambio mental.** *«Lo que construí en la semana 5 no era un ejercicio: es una pieza, y se enchufa.»*
Este es el momento en que la escalera deja de ser una metáfora: el flujo **consume el asistente y la base
de fuentes de M2** sin reescribir nada.

**Qué construye.** **Borradores para las preguntas repetidas (P01)** con cita de la fuente y bifurcación
honesta: si la base de fuentes encuentra la respuesta, redacta un borrador **en la bandeja**; si no la
encuentra, etiqueta «responder a mano» y para. **Lo importante del ejercicio es la rama del «no»:** es el
«saber decir no lo sé» de la referencia convertido en una bifurcación. Nunca envía.

**Duración realista.** 2 semanas.

**Qué capacidad entrena y cómo se enseña transferible.**
Sigue la capacidad 7, ahora con **composición**: un artefacto se convierte en pieza de otro. El principio
transferible, y merece ir en negrita en la ficha:

> **Automatiza donde ya viven tus datos, y construye cada escalón sobre el artefacto del anterior.** Es
> el criterio que decide entre herramientas de automatización en cualquier año: la que reutiliza lo que
> ya tienes gana a la que te obliga a rehacerlo, aunque la segunda sea más potente. Y la que mete a un
> proveedor nuevo entre tus datos y tú tiene que ganar por mucho para compensarlo.

**Cómo se autocorrige.**
- **La misma batería de 10 casos de M2, ahora contra el flujo**, con la clave sellada ya escrita. Atención
  puesta en **los dos casos de rechazo**: si el flujo redacta un borrador para alguno, no está listo, por
  bien redactado que esté.
- **Comprobación de cita, binaria:** cada borrador lleva el nombre del documento y su fecha, o no lo
  lleva. Se mira.
- **Ítems ancla y deriva** (EP-04): cinco casos fijos en una hoja con **una columna por fecha**. Se vuelven
  a pasar cuando cambie el prompt, cuando añada fuentes y el primer día que note que «responde raro». Y
  la distinción que se entrena aquí: **variación de forma** (dice lo mismo con otras palabras:
  irrelevante) frente a **variación de calidad** (una vez cita el precio y otra no: grave). Confundirlas
  hace descartar sistemas buenos y aprobar sistemas malos.
- **El riesgo de la base de fuentes, dicho en voz alta:** un cuaderno con las condiciones de cancelación
  del año pasado responde con las del año pasado, con toda la confianza del mundo. El control de versiones
  de las fuentes es parte del ejercicio, no un detalle.

**Caso satélite (15 min).** P28, respuesta a reseñas online: clasificar y preparar sí, publicar nunca — y
el motivo no es de calidad, es de RGPD: confirmar públicamente que alguien fue alumno y tuvo un problema
ya es una cesión de datos.

---

## M6 · Juicio dentro del flujo: esto es un agente y esto no (semanas 13–14)

**Cambio mental.** *«Un agente no es una automatización mejor. Es una automatización que **ha renunciado
a ser predecible** a cambio de poder afrontar casos que no previste. En atención al cliente esa renuncia
se paga a conciencia y solo donde compensa.»* Y la dirección del error que casi nadie enseña: **un agente
puede ser exceso.**

**Qué construye.**
1. Un flujo que **bifurca según un criterio que ella ha definido y sabe justificar**, con el juicio
   confinado a dos o tres puntos concretos.
2. **La lista de temas prohibidos de su propio sistema** (E-06), en negativo y sin matices: *nunca
   respondas sobre requisitos o plazos de visado; nunca cites importes; nunca confirmes disponibilidad de
   alojamiento; nunca respondas a una queja formal; nunca menciones salud. Si el tema aparece, escribe
   SOLO: DERIVAR A PERSONA, y para.*
3. **Condiciones de parada y topes.** Cliente enfadado, mención de abogado o de hoja de reclamaciones,
   salud, menor, importe por encima de X, o simplemente no encontrar la respuesta. Y el tope: *si la lista
   supera N, no redactes nada y avisa.* Un flujo que genera cuarenta borradores un lunes de julio no
   ayuda, entorpece.
4. **El plan para cuando falle**, en cinco pasos: detectar, parar, reparar con la persona (llamada, no
   correo), corregir el sistema añadiendo ese caso a la batería, y valorar si hay brecha de datos — esto
   último **no lo decide ella [!]**, lo escala el mismo día.
5. **La caja del fondo** (§8.1): qué existe, qué tarea suya lo pediría y qué tendría que cambiar.
6. **Capa 3 de protección de datos**: art. 50 y Anexo III.
7. **Ficha de capacidad nº 8** y **prueba de portabilidad nº 3**.

**Duración realista.** 2 semanas.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad 8: **juicio dentro del flujo y sus límites**. Y aquí va la honestidad incómoda, dicha sin
disculparse porque es cierta y porque lo alcanzable es lo que se sostiene:

> **Su escalón 3 realista es «un flujo con juicio en dos o tres puntos», no «un agente autónomo que
> gestiona el buzón».** La barrera número uno no es técnica ni de capacidad suya: es **de licencia** —los
> agentes de verdad están detrás de planes que su empresa casi con seguridad no tiene [V]—, de
> **permisos** —un agente útil necesitaría el buzón compartido y la hoja de camas— y de **datos** —sus
> procesos de más volumen mezclan salud, religión, menores y documentación de identidad—.

> **PRUEBA DE PORTABILIDAD Nº 3 — el catálogo de límites, 20 minutos.**
> Para las tres cosas que hoy no puede hacer (agente autónomo, tocar un sistema fuera de su suite,
> conectar una fuente con permisos acotados), escribe **la condición exacta que tendría que cambiar** —no
> el producto que la haría posible—. *«Que la empresa contrate un plan con X», «que el sistema tenga una
> interfaz de acceso y alguien la configure», «que aparezca una tarea con decenas de ficheros locales».*
> **Las condiciones no caducan; los productos sí.** Esta ficha es lo que le permitirá, dentro de dos años,
> mirar una herramienta nueva y saber en dos minutos si desbloquea algo suyo.

**Cómo se autocorrige.**
- **Cinco casos de parada fabricados que DEBEN parar.** Si alguno no para, no está listo. Comprobación
  pura.
- **La prueba del tope:** meterle un lote de cuarenta y comprobar que se detiene.
- **La prueba de apagado:** apagarlo de verdad y volver a encenderlo. *Un sistema que no sabes apagar no
  está terminado.* La rúbrica exige que la respuesta a «cómo se apaga» esté **probada**, no imaginada.
- **Rúbrica de E-06 con criterios negativos:** la lista de temas prohibidos incluye importes, plazos de
  visado, disponibilidad y salud **aunque su proceso no los toque hoy** —los sistemas se expanden solos, y
  la lista se escribe para el sistema de dentro de seis meses—; la respuesta a «quién revisa» es **una
  persona con nombre**, no «se revisa»; y ninguna salida llega a un cliente sin que alguien le dé a
  enviar.
- **Verdadero/falso de doce ítems** sobre el marco (E-05), autocorrección instantánea. Menos de 10
  aciertos → releer.
- **Tercer cebo**, cerrando el ciclo de control positivo: si su corrector se ha degradado, se detecta aquí.

**Caso satélite (15 min).** P08, la carta de aceptación para visado: zona prohibida, y el motivo que hay
que saber decir no es «es difícil» sino **«la normativa cambia de un año para otro, y congelar dentro de
un prompt un conocimiento que caduca es fabricar un error futuro»**. Es el satélite que mejor entrena el
juicio transferible, porque el criterio —no metas conocimiento volátil dentro de un artefacto— vale para
cualquier dominio.

---

## M7 · ¿Esto sirve? Medirlo sin engañarme (semanas 15–16)

**Cambio mental.** *«Que el flujo se ejecute no es que sirva. Un flujo puede ejecutarse impecablemente
cada lunes y no cambiar nada, porque el informe que produce no lo lee nadie.»* **Evaluación de proceso ≠
evaluación de resultado.**

**Qué construye.**
1. **Media página de evaluación por sistema**, con fecha: el número antes, el número después, el coste
   completo (montaje + revisión + mantenimiento), **cuál de las seis amenazas a la validez interna podría
   explicar el resultado** y qué mediría para descartarla.
2. **La prueba ciega** (EP-08): cinco respuestas suyas de hace meses y diez borradores del sistema, sobre
   casos comparables, sin marcas de origen, **barajadas por otra persona** y puntuadas con la ficha de
   criterio de M2.
3. **La cadena causal en cinco flechas** (EP-14), con el eslabón que no depende de ella subrayado.
4. **La segunda vuelta del Semanario.** Mismas columnas, seis meses después: qué veredictos han cambiado y
   por qué. **Aquí el ángulo cierra el círculo, y aquí se demuestra que el criterio se ha movido.**
5. **Ficha de capacidad nº 9**, primera mitad.

**Duración realista.** 2 semanas. La prueba ciega es una tarde.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad 9: **medir si sirve**. Es la más portátil de todas y la que ningún curso de IA da: es
metodología, no producto. Se enseña con su vocabulario, declarando el préstamo: *«en el mundo de la IA a
la batería la llaman evals o tests de regresión; el nombre psicométrico —ítems ancla— dice mejor para qué
sirven, que es hacer comparables dos momentos distintos»*.

**Herramienta y por qué: una hoja de cálculo, un cronómetro y una persona que baraje.** Deliberado: **la
evaluación no se hace con la herramienta evaluada.** Pedirle a un modelo que juzgue lo que él mismo
produjo acumula dos sesgos documentados —preferencia por lo verboso y auto-preferencia— que apuntan al
mismo desastre: aprobar por construcción.

**Cómo se autocorrige.**
- **La prueba ciega es autocorrección en estado puro.** No hay rúbrica que discutir: o acierta
  identificando cuáles eran suyas, o no; o ganan las suyas, o no. Y el patrón que aparece casi siempre —el
  sistema empata o gana en las dimensiones no críticas y pierde en la exactitud del dato— **le dice
  exactamente dónde poner la revisión humana**, que es la decisión que el curso entero perseguía.
- **Prohibiciones de vocabulario como comprobación mecánica:** si aparece «significativo», está mal —aquí
  no se estima un parámetro poblacional, se comprueba la cobertura de un instrumento contra un criterio
  fijado—. Si la medida es «horas a la semana» en vez de «minutos por unidad», está mal: es lo único que
  sobrevive a que el volumen se multiplique por tres entre febrero y julio.
- **La resta obligatoria.** Si no ha restado revisión y mantenimiento, está mal. Y si el saldo es negativo
  y aun así quiere conservarlo por otra razón —menos errores, menos carga mental, respuesta más rápida—,
  **que lo diga y mida esa otra razón**: es legítimo, pero entonces el ahorro de tiempo no era el objetivo.
- **Una amenaza que no puede descartar,** nombrada obligatoriamente. Un pre-post de un solo grupo nunca
  las descarta todas, y decirlo es lo que separa un dato de un argumento comercial.
- El único favor humano del módulo —**barajar**— son cinco minutos y **no consume punto de consulta**:
  vale cualquier compañera.

---

## M8 · Que lo adopten: evidenciar y contagiar (semanas 17–19)

**El módulo adicional que el brief reincorpora.** Desarrollado entero en §6.

**Cambio mental.** *«Un artefacto que solo funciona conmigo delante no es un sistema de la academia: es
una manía mía. Y lo que hace que otros lo adopten no es convencerles: es que puedan usarlo sin mí y que
yo pueda enseñar el número.»*

**Qué construye.** El **dossier de una página** por artefacto · la **demo de tres minutos** guionizada ·
el **piloto con una segunda persona**, una semana, sin ella · la **ficha de traspaso y mantenimiento** ·
y la **lista de lo que decidió no automatizar**, que es la pieza que le da credibilidad al resto.

**Duración realista.** **3 semanas**, y es el único módulo al que se le da una semana extra, porque
contiene una espera que no depende de ella: el piloto dura una semana natural.

**Cómo se autocorrige.** El piloto **es** la corrección: otra persona lo usa una semana o no lo usa. Ver
§6.4 para el detalle completo, que es donde este módulo se juega su credibilidad como diseño.

---

## M9 · Cerrar, dejarlo vivo, y qué hay más arriba (semana 19)

**Cambio mental.** *«Esto no termina cuando se acaba el material: termina cuando tú escribes los criterios
y sabes cuándo hay que volver a mirar.»*

**Qué construye.**
1. **La rúbrica escrita por ella**, con ≥3 criterios negativos, sin usar la del curso — y **validada
   contra un cebo**: si el cebo pasa su rúbrica, su rúbrica es blanda y se rehace.
2. **El vigilante de plantillas (P32)** como último artefacto: una comprobación programada que avisa
   cuando el tarifario maestro cambia y las versiones en otros idiomas no. Ataca el riesgo «alto y
   silencioso» del inventario, que hoy no vigila nadie, y produce algo que ningún otro artefacto produce:
   **una lista de errores reales que nadie sabía que existían**.
3. **El calendario de revisión** del Cuaderno de capacidades y de la hoja de anclas, con su próxima fecha.
4. **El apéndice del escalón 4**, marcado como opcional y como lectura: herramientas agénticas de
   escritorio y de terminal. **Objetivo declarado: que sepa qué son y por qué hoy no las necesita. Si
   termina el curso sin abrirlo, el curso ha funcionado igual**, y eso va en la primera línea.

**Duración realista.** 1 semana, con aire.

**Cómo se autocorrige.** La validación de su rúbrica contra el cebo es un control positivo aplicado al
instrumento que ella misma acaba de fabricar, y es **el criterio honesto de que ha terminado el curso**:
cuando escribe las rúbricas, ya no lo necesita.

---

## 4.1 Vista de conjunto

| M | Semanas | Escalón del perfil | Artefacto que sale | Capacidad | Corrección dominante |
|---|---|---|---|---|---|
| M0 | 1–2 | 1 · chat | Asistente v1 + Semanario + ficha del plan | 1 | Ejecución + batería sellada + la pantalla |
| M1 | 3–4 | — (el índice) | **Mapa de la semana** + cola de ataque | 2 | Lista binaria + cebo |
| M2 | 5–6 | 1 · chat | Ficha de criterio + anclas + batería + asistente v2 con fuentes | 3, 4 | Muestra apartada + Ctrl+F + cebo + portabilidad 1 |
| M3 | 7–8 | 2 · automatización | Libro de códigos + clasificación en lote + disparador por horario | 5, 6 | Doble codificación + umbral por los dos lados |
| M4 | 9–10 | 2 · automatización | Flujo de triaje | 7 | Se dispara o no + cinco correos + el que no debe disparar |
| M5 | 11–12 | 2 · automatización | Flujo de borradores con cita y rama de «no lo sé» | 7 | Batería reutilizada + ítems ancla con fecha |
| M6 | 13–14 | 3 · agentes | Flujo con juicio + temas prohibidos + plan de fallo + caja del fondo | 8 | Casos de parada + prueba de apagado + tercer cebo |
| M7 | 15–16 | transversal | Evaluación + prueba ciega + 2.ª vuelta del Semanario | 9a | Prueba ciega |
| M8 | 17–19 | **adicional** | Dossier + demo + piloto + ficha de traspaso | 9b | **El piloto** |
| M9 | 19 | 4 · opcional | Rúbrica propia + vigilante + lectura | — | Su rúbrica contra un cebo |

**Herramientas nuevas en 19 semanas: tres** —asistente con fuentes, clasificación en lote, flujo— y
ninguna se introduce antes de haber agotado la anterior. **Coste: cero euros.** Si el curso acaba
costando dinero, el diagnóstico estaba mal.

---

# 5. LA SEPARACIÓN CRITERIO / CLICS, EN LA PRÁCTICA

Esto no es una recomendación de estilo. Es la convención de producción del material, y si se relaja el
curso deja de ser agnóstico en tres módulos.

## 5.1 La convención de maquetación: dos ficheros, no dos apartados

El borrador anterior —y el borrador de la arquitectura 1— proponían **dos apartados dentro de la misma
lección**. Es insuficiente por tres motivos: los apartados se mezclan al escribir, no se pueden sustituir
en bloque cuando el producto cambia, y no se pueden duplicar por herramienta. La convención correcta es
**separación física**:

```
curso/
  M2/
    M2.3-leccion.md          ← EL CRITERIO. Sin fecha. Sin nombres de producto.
    M2.3-ejercicio.md        ← EL EJERCICIO. Tampoco nombra productos.
    M2.3-rubrica.md
    M2.3-solucion.md
    clics/
      M2.3-clics-gemini.md   ← fechado, reemplazable, el que ella usa hoy
      M2.3-clics-chatgpt.md  ← fechado, para la prueba de portabilidad
      M2.3-clics-claude.md   ← opcional
  comun/
    datos-volatiles.md       ← TODO número: cupos, límites, precios, planes
    tres-nombres.md          ← la tabla de equivalencias de nombres
    cuando-no-coincide.md    ← el procedimiento para cuando el manual y la pantalla discrepan
    protocolo-ia.md
```

**Cuatro reglas de producción, todas mecánicamente comprobables:**

1. **Ningún nombre de producto en el fichero de criterio.** Comprobación real, no aspiracional:
   `grep -iE "gem|notebook|studio|gemini|chatgpt|claude|workspace|sheets|gmail" M2.3-leccion.md` tiene que
   devolver **cero líneas**. Si devuelve alguna, esa frase va al fichero de clics o se reescribe en
   capacidades.
2. **Ningún número volátil en ningún fichero de criterio.** Cupos, límites, precios y qué edición incluye
   qué viven en `datos-volatiles.md` y se referencian. Actualizar el curso es actualizar un fichero, no
   veinte.
3. **Ningún ejercicio puede depender de una captura de pantalla ni de una ruta de menú.** El enunciado
   describe qué se busca («el sitio donde se guardan las instrucciones de este asistente»), la captura
   solo ilustra. Si la captura envejece, el ejercicio sigue haciéndose.
4. **Todo fichero de clics abre con la misma cabecera, sin excepción:**

   > *Verificado el 22 de agosto de 2026 en `<herramienta>`. **Si algo no coincide con lo que ves, tu
   > pantalla tiene razón y este texto no.** Ve a `cuando-no-coincide.md`.*

**Y `cuando-no-coincide.md`, media página escrita una vez y referenciada desde los treinta ficheros de
clics**, convierte la caducidad del material de defecto en **competencia enseñada**: buscar el nombre
nuevo en las novedades del proveedor, comprobar si es restricción de plan o de administrador, preguntarle
a la propia IA cómo se llama ahora eso y dónde está, y —solo si nada de eso funciona— el comodín PC-5. Eso
es exactamente lo que va a necesitar alguien que seguirá usando estas herramientas cinco años después de
terminar el curso.

## 5.2 La regla de redacción: se nombra la capacidad, no el producto

| No se escribe | Se escribe |
|---|---|
| «Crea un Gem» | «Guarda este asistente con nombre, para poder reabrirlo sin volver a explicar el contexto» |
| «Sube el tarifario al Notebook» | «Dale como fuentes los documentos sobre los que quieres que responda, y exige que cite de cuál sale cada dato» |
| «Añade un paso Ask a Gem» | «Haz que el flujo llame a tu asistente en lugar de repetir sus instrucciones dentro del flujo» |
| «Workspace Studio no admite unidades compartidas» | «Comprueba, antes de diseñar, sobre qué ficheros puede actuar tu herramienta de automatización: casi todas tienen restricciones con recursos compartidos» *(y el límite concreto, en el fichero de clics)* |
| «Usa la función =AI() de Sheets» | «Aplica tu libro de códigos a las 600 filas de golpe, sin copiar y pegar» |

**La prueba que decide en qué mitad va una frase, y cabe en una línea:**

> **¿Esta frase deja de ser cierta si mañana renombran un producto, o si mañana ella trabaja con otra
> herramienta?** Si sí → clics. Si no → criterio.
>
> Y el listón de admisión al curso, aplicado antes que nada: **¿le seguirá sirviendo dentro de dos o tres
> años?** Si no, o va a clics, o no entra.

## 5.3 La tabla de tres nombres

Vive en `comun/tres-nombres.md`, es la única página del curso donde conviven nombres de producto, y su
función no es enseñar productos: es **desactivar el miedo del principiante a quedarse casado con una
herramienta**, que es el freno mejor documentado del Q&A de la referencia (*«¿me estás obligando a
casarme con un programa que no conozco?»*, preguntado tres veces con distintas palabras).

| Capacidad (lo que dura) | Nombre hoy, herramienta A | Nombre hoy, herramienta B | Nombre hoy, herramienta C |
|---|---|---|---|
| Contexto que se aplica a todas las conversaciones | Instrucciones personalizadas | Instrucciones personalizadas | Preferencias |
| Asistente guardado con instrucciones propias | Gem | GPT personalizado | Proyecto |
| Fuentes propias con cita del fragmento | Cuaderno de fuentes | Ficheros de conocimiento | Ficheros del proyecto |
| Algo que ocurre por horario sin que lo pidas | Acción programada | Tarea programada | Tarea recurrente |
| Flujo con disparador por suceso | Automatización nativa de la suite | Plataforma de automatización externa | Plataforma de automatización externa |
| Acceso acotado a una fuente o herramienta | Conector | Conector | Conector / MCP |

> **Nota fija al pie de la tabla, y es la que hace el trabajo:** *«Esta tabla es la única página del
> curso que caduca por completo. Está fechada. Cuando algún nombre no coincida con tu pantalla,
> corrígelo tú: es tuya. Lo que no cambia es la columna de la izquierda.»*

## 5.4 Ejemplo real de las dos mitades de una misma lección

Se elige **M0.2, «¿Qué tengo yo exactamente?»**, porque es la lección donde la tentación de escribir un
manual de Google es máxima —es literalmente una tarea de la consola de otra empresa— y porque el brief
señala ese diagnóstico como lo único específico de su entorno que hay que resolver pronto.

---

### `M0/M0.2-leccion.md` — **el criterio** *(sin fecha, sin nombres de producto)*

> ## Por qué esto va antes que nada
>
> Vas a empezar a pegar cosas en una herramienta. Antes de eso hay que saber **bajo qué reglas** estás
> pegándolas, porque de eso depende qué puedes meter ahí dentro. Montar automatizaciones sobre un suelo
> que no has mirado es construir sobre algo que no sabes si aguanta.
>
> Y ojo al encuadre, porque es lo que hace que esta conversación te deje mejor y no peor: **no estás
> pidiendo permiso para nada.** Ya usas la herramienta, te la ha dado tu empresa, y usarla está bien
> visto. Estás haciendo lo que hace alguien que se toma en serio su herramienta: entender la
> configuración antes de apoyarse en ella.
>
> ## Las cuatro preguntas que definen cualquier plan, de cualquier proveedor, en cualquier año
>
> Aprenderte una tabla de planes no sirve de nada: las tablas cambian cada seis meses. **Aprenderte las
> preguntas sí sirve, porque las preguntas no cambian.** Son cuatro, y valen para tu herramienta actual,
> para la que uses en 2029 y para cualquiera que te pongan delante en otra empresa:
>
> 1. **¿Entrenan sus modelos con lo que yo escribo?**
> 2. **¿Cuánto tiempo guardan mis conversaciones, y quién decide ese plazo?**
> 3. **¿Dónde se procesan y se almacenan los datos? ¿Puedo exigir que sea en la Unión Europea?**
> 4. **¿El proveedor firma como encargado del tratamiento, con contrato?** Esta es la que de verdad
>    separa una cuenta de empresa de una cuenta personal: sin contrato no hay encargado, hay una cesión
>    de datos a un tercero sin amparo.
>
> Y una quinta que no es del plan sino de tu empresa, y que suele ser la que decide de verdad:
> **¿alguien ha configurado esto y ha dejado dicho por escrito qué se puede meter?**
>
> ## El principio que hay detrás, y que no caduca
>
> **La misma frase escrita en la misma pantalla es segura o insegura según con qué cuenta hayas
> entrado.** No depende del texto, ni del modelo, ni de lo cuidadosa que seas: depende del régimen
> jurídico de la cuenta. Por eso el primer dato que anotas es con qué correo has entrado.
>
> Segundo principio: **pagar resuelve quién es el proveedor, no qué tratamientos están amparados.** Que
> tu empresa pague la herramienta no legitima que pasen por ahí pasaportes o datos de salud si nadie lo
> ha contemplado por escrito.
>
> ## Cómo se responden estas preguntas cuando nadie te contesta
>
> Hay dos vías, y las dos son parte del ejercicio.
>
> **Vía A — preguntar bien.** Un mensaje corto a quien lleva las licencias, que **abre con trabajo hecho**
> y pregunta dos cosas concretas de una sola respuesta. La formulación que funciona descansa siempre en
> el mismo movimiento: **tú aportas algo, no pides algo.** Y si no existe una política escrita sobre qué
> se puede meter, ofreces la tuya como borrador: acabas siendo quien la propone, que es el mejor
> resultado posible.
>
> **Vía B — deducirlo de lo que ves.** Si nadie contesta, se infiere el plan desde la pantalla: se
> intentan cinco cosas concretas y se anota cuáles funcionan y cuáles no. Esto es operacionalizar un
> constructo en indicadores observables, que es tu casa. Y enseña algo que vas a necesitar durante todo
> el curso: **la documentación dice una cosa y la instancia concreta dice otra, y manda la instancia.**
>
> ## El estándar de esta lección
>
> **«No lo sé y lo he preguntado el día 14» es un resultado válido. «Creo que sí» no lo es.** Distinguir
> lo que sabes de lo que supones es el mismo estándar que vas a necesitar para evaluar respuestas de una
> IA, y por eso este ejercicio va el primero.
>
> ## Los clics
>
> → `clics/M0.2-clics-gemini.md` *(y `M0.2-clics-chatgpt.md` si algún día cambias de entorno)*

---

### `M0/clics/M0.2-clics-gemini.md` — **los clics** *(fechado y reemplazable)*

> *Verificado el 22 de agosto de 2026 en Gemini dentro de Google Workspace. **Si algo no coincide con lo
> que ves, tu pantalla tiene razón y este texto no.** Ve a `cuando-no-coincide.md`.*
>
> **Pregunta 1 y 2, en treinta segundos:**
> 1. Entra en `gemini.google.com` **con la cuenta de la academia**. Comprueba arriba a la derecha que no
>    es la personal. Anota el correo exacto.
> 2. Mira el **distintivo** de la parte superior. Si pone **Pro**, **Expanded** o **Ultra**, tus
>    conversaciones no las examinan revisores humanos ni se usan para mejorar modelos. **Si no hay
>    distintivo, no asumas que estás protegida: pregunta.**
>
> **Las cinco comprobaciones de la Vía B** — se hacen en diez minutos y se anota qué funciona:
>
> | Comprobación | Si funciona | Si no funciona |
> |---|---|---|
> | Escribir `=AI("di hola")` en una celda de una hoja de cálculo | Plan intermedio o superior | Probablemente el plan básico |
> | Abrir el panel lateral de la IA dentro de un documento | Plan intermedio o superior | Plan básico |
> | Entrar en la web de automatización de la suite | La automatización nativa está habilitada | El administrador no la ha activado |
> | Mirar cuántos resúmenes en audio diarios permite el cuaderno de fuentes | Ver `datos-volatiles.md` | — |
> | Intentar entrar en la consola de administración | (Casi seguro que no) | **Te dice quién manda: anótalo** |
>
> **Dato duro:** un usuario que no es administrador **no puede consultar la edición contratada** de su
> organización. Está en Consola de administración → Facturación → Suscripciones. No hay atajo, y por eso
> existe la Vía A.
>
> **Los cuatro mensajes literales para copiar y pegar** → `M0.2-mensajes.md`.
>
> **Cifras y planes** → `comun/datos-volatiles.md`. *No las copies aquí.*

---

**Qué demuestra este ejemplo, y por qué lo he elegido:** la mitad de criterio ocupa el doble que la de
clics, no menciona ni una vez el nombre del producto, **y seguiría siendo válida palabra por palabra si
mañana su empresa se pasara a otro proveedor**. La mitad de clics es sustituible en veinte minutos por
alguien que no haya escrito el curso. Ese es el criterio de calidad de toda la maquetación.

## 5.5 Qué se pierde con esta convención, dicho aquí

Dos cosas, y conviene no fingir que salen gratis:

- **La lección se lee peor de corrido.** Saltar entre dos ficheros tiene un coste de atención real. La
  mitigación es que el fichero de clics sea corto, numerado y siempre en el mismo sitio, y que la lección
  termine con un enlace único. No la elimina.
- **Redactar en capacidades es más lento y más abstracto.** Escribir «guarda este asistente con nombre»
  es menos inmediato que «pulsa Nuevo Gem». La compensación es que el ejercicio y la rúbrica viven en la
  mitad que no caduca, así que **el trabajo de mantenimiento del curso baja de treinta ficheros a diez**.
  Es una decisión de coste, y está tomada a favor de los dos o tres años que el brief pide.

---

# 6. EL MÓDULO DE EVANGELIZACIÓN INTERNA (M8)

## 6.1 Qué NO es, dicho primero porque es donde se estropea

- **No es conseguir el sí.** No hay autorización que pedir. Usar IA en su empresa ya está bien visto y lo
  mal visto es no automatizar. Un módulo de venta interna resolvería un problema que ella no tiene.
- **No es marketing personal.** Nada de portfolio, nada de landing, nada de «mira lo que tengo ahora en
  mi CV». Ese es el destino del itinerario no técnico de la referencia porque su alumno tipo quiere
  cambiar de sector. La nuestra no.
- **No es la columna vertebral.** Es un módulo de tres semanas al final, alimentado por un hilo de tres
  líneas por módulo. Si fuera la lente del curso entero, el curso dejaría de ser sobre su trabajo.
- **No es evangelizar hacia arriba en abstracto.** El objeto de la adopción no es una idea («deberíamos
  usar IA»): son **artefactos concretos que ya funcionan y que otra persona puede usar**.

## 6.2 Qué es: el enunciado del módulo

> **Demostrar y arrastrar.** Su empresa empuja la IA sin saber bien qué se puede hacer. Lo que cambia esa
> situación no es un argumento: es **una cosa que funciona, un número que se puede reproducir, y una
> segunda persona que la usa sin ella delante.** Este módulo produce esas tres cosas.

Y el principio que ordena todo el módulo, que es el mismo que atraviesa el curso:

> **La credibilidad se compra con los noes.** Quien llega diciendo «estas cuatro cosas NO deberían
> automatizarse, y aquí está por qué» consigue que le crean sobre la quinta. Quien llega diciendo que
> todo se puede automatizar consigue que no le crean sobre nada — y esa es, exactamente, la posición en
> la que su empresa está hoy respecto a la IA.

## 6.3 Qué enseña — siete piezas, todas con artefacto

**(1) El número y su método.** Del M7 sale un ahorro medido en minutos por unidad, con el coste de
revisión restado y con una amenaza a la validez que no se puede descartar. **Las tres cosas van juntas o
no va ninguna.** Un número sin método es una promesa, y una promesa que no se cumple quema los tres
proyectos siguientes. Aquí su formación es una ventaja competitiva directa: casi nadie que presenta
resultados de IA en una empresa sabe decir *«esto podría explicarse también porque septiembre no es
julio»*, y decirlo es lo que hace que el resto se crea.

**(2) Lo que el artefacto NO hace.** Es la tercera línea del Cuaderno de evidencias, y en el dossier va
en su propio apartado, no en letra pequeña. Doble función: es honestidad, y es **gestión de expectativas
operativa** — si el dossier dice «no responde nada sobre visados y para en cuanto aparece la palabra», la
primera pregunta incómoda ya está contestada antes de que la hagan.

**(3) El artefacto que se enseña en tres minutos.** No una presentación: **un antes y un después con un
caso real**, y un número. Aquí la lección de la referencia se aplica invertida: su grafo de Obsidian era
espectacular en pantalla y marginal en valor, y era *para el agente, no para el humano*. Lo que se enseña
aquí es aburrido y sirve: la pantalla de antes (una bandeja con doscientos comentarios sin leer) y la de
después (una tabla con las categorías y tres hallazgos). **Guion de tres minutos, escrito, cronometrado.**

**(4) La prueba del pasillo.** Explicar qué hace y qué vale **en treinta segundos y sin nombrar ninguna
herramienta**. Regla de vocabulario dura: se nombra el resultado, no la tecnología. No *«monté un flujo
con un paso de extracción que llama a mi cuaderno de fuentes»*, sino *«las setecientas encuestas del año
se leen solas, y en enero supimos que el problema del piso de Chamberí llevaba tres meses»*. Esta regla es
además la vacuna contra el efecto que más daño hace a un evangelizador interno: **sonar a que ha
descubierto una religión**.

**(5) El piloto con una segunda persona.** Una semana, una compañera, sin ella delante. Es el único test
real de adopción y produce siempre el mismo hallazgo, que es lo que lo hace valioso: **una parte del
artefacto era ella**. Instrucciones implícitas, decisiones que tomaba sin darse cuenta, un fichero que
solo ella sabe dónde está. Lo que el piloto revela es lo que hay que arreglar para que la cosa sobreviva
a sus vacaciones, y sobrevivir a sus vacaciones es literalmente la definición de que la organización lo
ha adoptado.

**(6) La ficha de traspaso y mantenimiento.** Qué fuente caduca y cada cuánto · quién la revisa, **con
nombre** · qué batería se vuelve a pasar cuando se toque algo · **cómo se apaga**, probado. Es lo que
convierte «una cosa que hizo Marta» en «una cosa que tiene la academia». Y es también protección propia:
un artefacto sin dueño y sin fecha se degrada, y cuando se degrada el recuerdo que queda no es «faltaba
mantenimiento», es «aquello de la IA no funcionaba».

**(7) Cómo se arranca un proyecto para que lo adopten, y no al revés.** Cuatro reglas, todas derivadas de
lo que el curso ya ha hecho:
- **Empieza por un proceso que no sea de nadie.** P27 no se lo quitas a nadie: hoy no lo hace nadie. Un
  proyecto que mejora la tarea de una compañera empieza con una persona a la defensiva; uno que hace lo
  que nadie hacía empieza con cero resistencia. **La elección del primer proyecto es el 80 % de su
  adopción.**
- **Enseña el resultado, no el proceso.** La primera vez se enseña el informe de encuestas, no cómo se
  hizo. El «cómo» se cuenta cuando alguien lo pide, que es la señal de que ya hay adopción.
- **Ofrece el trabajo, no la herramienta.** «Te paso el resumen de las quejas de alojamiento de este mes»
  gana siempre a «te enseño a montar un clasificador».
- **Deja que lo pidan.** La segunda persona no se recluta: aparece cuando ve el primer informe. Si a las
  tres semanas nadie ha pedido nada, el artefacto no era tan útil como parecía — **y eso también es un
  resultado del curso**, no un fracaso personal.

## 6.4 Cómo se autocorrige sin mentor — el punto donde este módulo se juega su credibilidad

Es el módulo más difícil de autocorregir de los nueve, porque su criterio de éxito es **la conducta de
otras personas**, que ella no controla. Decirlo es obligatorio. Y aun así hay cinco mecanismos, cuatro de
ellos comprobaciones y no juicios:

1. **El piloto es el corrector, y es binario.** Otra persona lo usó cinco días laborables sin ella, o no
   lo usó. Se cuenta. Y el entregable no es «salió bien»: es **la lista de lo que hubo que arreglar**,
   que tiene que tener al menos dos entradas. *Si el piloto no reveló nada que arreglar, no fue un
   piloto: estuviste mirando por encima del hombro.* Ese es el criterio negativo del módulo.
2. **La reproducción del número.** Dos semanas después, con la ficha de método delante, vuelve a calcular
   el ahorro. **Si no sale el mismo número ±10 %, el número no era reproducible y el dossier se
   reescribe.** Es un test-retest de su propio instrumento y no necesita a nadie.
3. **La prueba del pasillo, cronometrada.** Treinta segundos, sin nombres de herramienta, a alguien que
   no ha visto el artefacto. Comprobaciones binarias: *¿nombré alguna herramienta? SÍ/NO* · *¿la otra
   persona pudo repetirme qué hace? SÍ/NO* · *¿dije un número? SÍ/NO* · *¿dije qué NO hace? SÍ/NO*.
4. **Rúbrica del dossier, con criterios negativos y salida escrita obligatoria:**
   - *Hay en el dossier un número cuyo método no puedo reproducir delante de alguien.* ☐
   - *Hay una afirmación que no podría defender si alguien la comprobara la semana que viene.* ☐
   - *El apartado «qué NO hace» está vacío o dice generalidades.* ☐
   - *La respuesta a «quién lo mantiene» no es una persona con nombre.* ☐
   - *No hay ninguna forma de apagarlo, o la hay pero no la he probado.* ☐
   - *Presento como resultado del sistema algo que en realidad hago yo a mano después.* ☐
5. **PC-6** (§7): la prueba del pasillo con alguien que sabe de IA y **no conoce la academia** es el
   evaluador ideal para detectar dos cosas que ella no puede ver desde dentro: **jerga** y
   **sobreafirmación**.

## 6.5 Dónde va y por qué exactamente ahí

| Alternativa | Por qué no |
|---|---|
| Al principio, como encuadre motivador | No hay nada que enseñar todavía. Y arranca el curso con la mirada puesta en lo que piensen los demás, que es exactamente el desvío que el brief prohíbe |
| Repartido por todos los módulos | Convertiría cada artefacto en una pieza de comunicación y contaminaría el criterio: se elegiría lo vistoso sobre lo útil, que es el error del grafo de la referencia |
| **Al final, después de medir** ← **la elegida** | Consume la salida de M7. **No se evangeliza lo que no está medido.** Y llega en el momento en que el material solo ya no tira: el único incentivo disponible en la semana 17 es que **alguien de fuera use lo que has hecho**, y ese es precisamente el contenido del módulo |
| Al final, pero sin hilo previo | El Cuaderno de evidencias existe desde la semana 2 justamente porque, sin él, M8 tendría que reconstruir números de memoria — es decir, inventarlos |

## 6.6 Qué produce, en una lista

1. **Un dossier de una cara por artefacto vivo** (tres): qué hace · qué ahorra y con qué método se midió
   · **qué no hace** · quién lo mantiene · cómo se apaga.
2. **Un guion de demo de tres minutos**, cronometrado, con un antes y un después reales.
3. **Un piloto ejecutado** con una segunda persona, y su lista de arreglos.
4. **Una ficha de traspaso y mantenimiento** por artefacto.
5. **La lista de lo que decidió no automatizar**, con el motivo — heredada del M1 y actualizada.
6. **Una nota de media página** para quien lleve la política de uso de IA, si en el M0 resultó que no
   existe ninguna. No es venta: es cerrar el hueco que ella misma detectó en la semana 1, y es el hallazgo
   con mejor relación valor/esfuerzo de todo el curso.

---

# 7. LOS PUNTOS DE CONSULTA CON SU PAREJA

## 7.1 El principio, antes de la lista

El recurso es **escaso, no renovable y con coste relacional**. Un mentor pagado se gasta sin culpa; una
pareja, no. Y un curso que convierta a la pareja en el soporte técnico de la alumna daña dos cosas a la
vez: la relación y la autonomía que el curso persigue.

**Presupuesto: seis consultas de diez minutos en todo el curso.** Una hora repartida en cuatro meses y
medio. Un curso que reserve «consultas ilimitadas» obtiene en la práctica **cero**, porque cada consulta
individual compite con la comodidad de no molestar y pierde. Uno que reserve exactamente seis, con nombre
y momento, obtiene seis.

**Filtro de admisión, impreso en la portada de la bitácora. Si falla cualquiera de las cuatro, no es un
punto de consulta:** (1) ¿lo resuelve el material? (2) ¿lo resuelve la IA con el protocolo de siete
reglas? (3) ¿lo resuelve **mirar** —su pantalla, su consola, preguntar a su administrador—? (4) ¿lo he
intentado veinticinco minutos y he anotado qué he probado?

**Ficha de cinco campos escrita ANTES**, máximo una cara: la pregunta **en una frase y cerrada** · mi
hipótesis y qué esperaría ver si tengo razón · qué he probado ya y qué pasó · **el dato concreto**
(mensaje de error literal, captura, las dos respuestas que se contradicen) · qué haré con cada respuesta
posible.

**Cuatro reglas de la conversación:** los cinco primeros minutos **sin pantalla**, explicándolo en voz
alta con la ficha delante —muchas veces se resuelve ahí, y eso es autoexplicación con oyente— · **él no
toca el ratón**, puede decir dónde mirar pero no mira él · sale con **una frase escrita en su propio
lenguaje** dentro de la hora siguiente · **a los diez minutos se para, esté como esté**; lo que no cabe en
diez minutos no es una consulta, es un problema de diseño del curso y se anota como tal.

## 7.2 Dónde caen, y por qué exactamente ahí

Los cuatro tipos de trabajo que la IA **no puede** corregir (`dominio-autodidacta.md` §3.5.4) son la
materia prima legítima: hechos de su empresa que el modelo no tiene · el estado real de su entorno ·
decisiones de riesgo con consecuencia externa irreversible · juicios de escala y oportunidad. Los seis
puntos son uno de cada, más un comodín y un cierre.

| # | Momento | Qué se lleva | Por qué ahí y no en otro sitio | Si no está disponible |
|---|---|---|---|---|
| **PC-1** | **Fin de M0** (sem. 2) | *«He deducido que tenemos el plan X y que por tanto no puedo hacer Y. ¿Me equivoco?»* Con las cinco comprobaciones hechas y las capturas | Es un **hecho del mundo que el material no puede ver**, y un error aquí contamina el curso entero: cambia qué módulos son posibles. Mejor relación consecuencia/coste de los seis | Asumir el escenario **más restrictivo** y anotarlo como pendiente de confirmar |
| **PC-2** | **Mitad de M1** (sem. 4) | *«Estas son mis doce filas con su veredicto. Estas tres no las tengo claras. ¿Moverías alguna?»* | **El de mayor apalancamiento de esta arquitectura.** Es un juicio de escala y oportunidad que ni el material ni la IA pueden dar: preguntarle a un modelo si algo debe hacerse con IA tiene un sesgo obvio hacia el sí. Y un error aquí no cuesta un ejercicio: **cuesta el orden de los seis módulos siguientes** | Aplicar los descalificadores por número de proceso y **bajar un escalón** el veredicto de las tres dudosas |
| **PC-3** | **Fin de M2** (sem. 6) | *«Esta es la corrección que hizo la IA de un artefacto con tres fallos plantados. Encontró dos. ¿Estoy leyendo bien lo que se le escapa?»* | **No se revisa su trabajo: se revisa su corrector**, que va a usar cincuenta veces más. Diez minutos aquí valen por todas las correcciones posteriores | Pasar el cebo por **dos modelos distintos** y comparar: el desacuerdo es un sustituto pobre pero real del juicio externo |
| **PC-4** | **Inicio de M3** (sem. 7), antes del primer lote de datos reales | Su clasificación de **ocho tipos de dato reales** en tres cajones (cuenta de empresa / nunca / depende), más tres casos seudonimizados: *«¿tú sabrías de quién hablo?»* | **La única decisión del curso con consecuencia externa irreversible.** Y la prueba de la compañera necesita por definición una mirada de fuera que ella no puede tener sobre su propio material. El momento es exacto: es cuando se pasa de casos sueltos a lotes | Regla de máxima cautela: **si dudas, no entra**, y se anota |
| **PC-5** | **Comodín**, desde M4 (sem. 9) | Un fallo de plataforma tras agotar la lista de seis comprobaciones y `cuando-no-coincide.md` | Caso canónico de «diez minutos ahorran una tarde». **No tiene fecha a propósito:** saber que existe un comodín reduce el miedo a atascarse, que es un factor de abandono por sí mismo, aunque no se use | Documentar el fallo, **rodearlo** con una solución manual y seguir. Un curso no puede parar por un botón que movieron |
| **PC-6** | **M8** (sem. 18–19) | La **prueba del pasillo** —treinta segundos, sin nombrar herramientas— y después: *«esto es lo que tengo funcionando; ¿qué es lo siguiente que tendría sentido, y qué tendría que cambiar para que mereciera la pena?»* | Dos cosas que ella no puede ver desde dentro: si su explicación tiene jerga y si sobreafirma. Alguien que **sabe de IA y no conoce la academia** es el evaluador ideal para las dos. Y cierra el curso con una orientación que no puede darse sola, evitando el «final sin final» | Grabarse treinta segundos, escucharse al día siguiente y contar los nombres de herramienta. Para el «qué sigue», la tercera columna de la caja del fondo |

## 7.3 Lo que deliberadamente NO es punto de consulta

Escrito para que no se erosione: revisar un entregable (*«¿está bien mi asistente?»* → rúbrica y batería)
· explicar un concepto (*«¿qué es MCP?»* → material) · enseñarle a hacer algo (*«¿cómo se hace un
flujo?»* → documentación) · dar ánimos genéricos.

Y la tentación específica de esta configuración: **que él le monte algo «que es un momento»**. Eso no es
una consulta: es un artefacto que ella no sabrá mantener ni depurar, y en el módulo siguiente será deuda.
Además contradice el objetivo entero: lo que el curso persigue es criterio propio, y el criterio no se
adquiere viendo trabajar a otro.

**Un uso de otra persona que NO gasta punto:** barajar las respuestas de la prueba ciega del M7 y guardar
la clave. Es una función mecánica de cinco minutos y vale cualquier compañera de la academia.

**Nota de riesgo sobre este diseño [NV]:** todo esto asume que la pareja sabe de plataformas y no solo de
modelos. Si su conocimiento es de modelos, **PC-5 pierde casi todo su valor** y ese punto se reasigna a
PC-2 o a PC-6.

---

# 8. «SABER QUÉ EXISTE» SIN CATÁLOGO MUERTO, Y CÓMO SE ENSEÑA A NO USAR IA

## 8.1 El objetivo 1, resuelto con tres mecanismos y ningún listado de productos

**(1) Los seis veredictos son el catálogo, y solo se aprenden asignándolos.** Cada categoría se ancla en
dos o tres tareas **suyas, con nombre y número de proceso**. La diferencia entre *«un agente decide sus
propios pasos»* y *«el triaje de reseñas es lo único de mi lista donde hay que evaluar algo para saber
por dónde seguir»* es la diferencia entre una definición y un conocimiento. Doce asignaciones en M1, más
un caso satélite por módulo, más la segunda vuelta del Semanario: **más de treinta juicios**.

**(2) La caja del fondo, con tres campos fijos.** Lo que existe pero hoy no le toca entra en media página
por pieza, siempre con la misma estructura:

> **Qué es** (dos frases, sin marketing) · **Qué tarea tuya lo pediría** (una fila de tu Semanario, con su
> número) · **Qué tendría que cambiar para que te tocara** (la condición de activación).

El tercer campo es lo que impide que sea catálogo muerto: **cada cosa lleva escrita su propia condición de
disparo, y las condiciones no caducan aunque el producto se renombre.**

| Pieza | Qué tarea tuya lo pediría | Qué tendría que cambiar |
|---|---|---|
| **Plataformas de automatización externas** | Cualquier flujo que tenga que tocar el software de gestión académica, la pasarela de pago, WhatsApp Business o el portal de una agencia | Que el flujo necesite **salir de tu suite**. Criterio de elección: la más barata a tu volumen que no exija que alguien la mantenga. La que exige servidor propio solo si aparece alguien técnico |
| **Acceso acotado a una fuente (conectores, MCP)** | Un asistente que consulte la hoja de camas sin que tú se la pegues | Que la fuente tenga interfaz de acceso **y** que alguien configure el permiso. Hoy es **vocabulario, no herramienta** — pero el principio que hay detrás sí lo usas ya: **conectar solo a lo necesario, y a una carpeta, no al disco** |
| **Agentes que manejan el navegador por ti** | Rellenar los formularios de las agencias intermediarias (P03) | Un plan superior. Es barrera **de dinero, no de capacidad** |
| **Plataformas de agentes de empresa** | Un buscador sobre todo el conocimiento de la academia | Que la empresa contrate un producto distinto. **[!]** Decisión de empresa, no suya |
| **Programar dentro de la suite** (scripts asistidos) | Nada que la automatización nativa no cubra | Que hagas algo que la automatización nativa no puede **y** que haya quien mantenga el script. Ojo: **es código aunque lo escriba una IA, y cuando falla hay que leer un error de programador** |
| **Entornos de desarrollo de modelos** | **Ninguna.** Y hay que decirlo con contundencia | Nada. Es una superficie de desarrollador cuyos propios términos advierten de no enviar información personal, tiene aspecto profesional y se entra con la cuenta de siempre: **es la trampa más silenciosa del panorama** |
| **Agentes de escritorio y de terminal** | Procesar decenas de ficheros locales de forma repetida — revisar doscientos contratos de estancia larga buscando una cláusula | Que aparezca esa tarea. Escalón 4, apéndice de lectura, opcional |
| **Bases de conocimiento grandes (recuperación, grafos)** | Que tus fuentes pasen de decenas a cientos y el cuaderno empiece a perderse | Ese salto de volumen, y no antes. Un cuaderno con veinte fuentes bien fechadas te da lo mismo con mucho menos aparato |

**(3) La segunda vuelta, en M7 y M9.** Se relee la caja del fondo y se marca **qué condiciones han
cambiado** en cuatro meses. Es lo que convierte un catálogo en un instrumento con vida — y es, además, el
ensayo de lo que tendrá que hacer sola cada año.

**El vocabulario mínimo**, para que no se quede fuera de una conversación en la oficina: agente, flujo,
disparador, paso, contexto, alucinación, batería de casos (que en el mundo de la IA llaman *evals*),
conector, MCP. Regla de redacción: la primera vez que se usa un término se da su equivalente al uso entre
paréntesis, para que sepa buscarlo por su cuenta.

**Lo que este bloque NO hace:** comparar modelos, dar nombres de modelo ni recomendar por *benchmark*.
*«Da bastante igual qué modelo uses mientras no gastes miles en tokens»*, y apoyar el material en el
nombre del modelo es garantizar que nazca viejo.

## 8.2 Cómo se enseña a NO usar IA cuando no toca

Siete mecanismos, todos estructurales. Ninguno es un sermón, y **todos se evalúan**.

**1 · Dos de los seis veredictos son «no», y van los primeros de la lista.** No al final como advertencia:
al principio como destino.

**2 · La regla del cuatro.** Al menos cuatro de doce. El «no» hay que **encontrarlo**, no evitarlo. Y la
rúbrica declara explícitamente que **un mapa en el que todo acaba automatizado está mal resuelto**.

**3 · La prueba de la servilleta.** *¿Podrías escribir los pasos de esta tarea en una servilleta y
valdrían siempre?* Si sí, no necesitas un modelo de lenguaje: necesitas una fórmula, una plantilla o un
calendario. Cabe en una línea y sobrevive a cualquier renombrado.

**4 · El caso canónico, trabajado entero y medido — el mecanismo más fuerte de los siete.**
El presupuesto (P02) se monta **con IA** —asistente con el tarifario adjunto— **y con fórmula**, sobre los
mismos veinte casos. Se cronometra y se cuentan los errores. **Gana la fórmula, y gana por goleada.**
Enseñar el «no» haciendo el «sí» y midiendo que pierde es infinitamente más fuerte que prohibirlo. Y es
el ejemplo canónico del árbol de decisión de la referencia contado con sus datos y no con los de una
agencia de marketing polaca.

**5 · Las zonas prohibidas, con el motivo y no solo la prohibición** — porque una prohibición sin motivo
no se transfiere a un caso nuevo:

| Proceso | Por qué no, dicho de forma transferible |
|---|---|
| **P08** carta de aceptación para visado | Riesgo crítico y **normativa viva**: cambia de un año para otro. **Congelar dentro de un artefacto un conocimiento que caduca es fabricar un error futuro** |
| **P26** quejas formales | Una respuesta que **admite responsabilidad por escrito compromete a la empresa**. Y los modelos son complacientes: la complacencia por escrito, en una queja, es exposición legal |
| **P29** emergencias 24 h | Personas, menores, responsabilidad civil, y un alumno en shock con nivel A1 |
| **P25** reembolsos | Datos bancarios y riesgo de fraude por suplantación en el cambio de cuenta |
| **P17** matching con familia de acogida | Concentra **salud, religión y potencialmente orientación sexual** en una casilla de texto libre. Es el proceso que **más parece** el caso ideal de IA, y por eso es la trampa |
| **P05 / P16** nivelación y exámenes | Anexo III del Reglamento de IA: *evaluar el nivel educativo* es alto riesgo. Aplazado a diciembre de 2027, **no cancelado**. Lo suyo no es decidirlo **[!]**: es reconocerlo y avisar |

Y la regla de oro que hace todo esto memorable: **de todo su proceso, el único trocito que está en la
lista de alto riesgo es el que decide el nivel de un alumno. Todo lo demás —redactar, traducir, resumir,
clasificar, preparar borradores— no lo está.** Esa asimetría se recuerda; una lista de artículos, no.

**6 · La regla del coste completo, descubierta y no dictada.** *Un flujo que ahorra ocho minutos y cuesta
diez de revisión es una pérdida disfrazada de modernidad.* Se descubre en M7, con su propia hoja. Y la
métrica de vanidad tiene nombre: **que el flujo se ejecute cada lunes no es que funcione.**

**7 · El «no» del día 60.** El riesgo del sistema no es el del día 1: es el del día 60, cuando ya se
confía y se deja de revisar. Se llama sesgo de automatización, tiene errores de omisión y de comisión, y
su contramedida es de diseño y no de disciplina: **revisión muestreada y programada, no «cuando me
parezca»**. La frase que ordena el bloque:

> **La confianza no es una salvaguarda. Si la seguridad de un sistema depende de que alguien se acuerde
> de revisar, el sistema es seguro hasta el primer día de mucho trabajo. Y en una academia, el día de
> mucho trabajo es predecible: se llama julio.**

**Y un octavo, incómodo: el «no» a la propia arquitectura.** El checkpoint de divorcio de M2 autoriza por
escrito, desde la semana 1, a cambiar de tarea hilo. Un curso que no permite abandonar una decisión suya
no puede pedirle a ella que abandone las suyas.

---

# 9. PROTECCIÓN DE DATOS, INTEGRADA

**Decisión de diseño, y es la más específica de esta arquitectura:**

> **La protección de datos no es un módulo. Es la columna 8 del Semanario, rellenada doce veces sobre
> tareas suyas.**

Un módulo de RGPD se lee una vez, se aprueba y se olvida. Una columna del inventario se rellena doce
veces, y la decimotercera sale sola. Y colocarla como columna la convierte en **criterio de selección** en
vez de en **freno posterior**: no se elige un proyecto y luego se comprueba si es legal; **el semáforo
participa en el veredicto**, y una fila con ROJO irreducible se lleva el tachón de zona prohibida antes de
que a nadie se le ocurra automatizarla.

Sobre esa columna, **tres capas, cada una pegada al momento en que desbloquea lo siguiente**:

| Capa | Dónde | Qué entra | Por qué exactamente ahí |
|---|---|---|---|
| **1 · Antes de pegar nada** | **M0**, días 1–2 | El semáforo VERDE/ÁMBAR/ROJO · la tarjeta del lunes (seis preguntas) · **las cuatro preguntas que definen cualquier plan** y su respuesta para el suyo (E-01) · la línea limpia entre la cuenta personal y la de empresa | **Es la semana en que va a empezar a pegar cosas.** Y el Pase A del Semanario ya enseña minimización **haciendo**: para inventariar tus tareas no necesitas ni un dato de un alumno, solo asuntos |
| **2 · Antes de automatizar** | **M3** | Seudonimizar de verdad (cuasi-identificadores, no solo el nombre) · la regla de adjuntos · el caso de las grabaciones de llamadas | **Automatizar multiplica el volumen de datos** que pasa por la herramienta: se pasa de un caso suelto a cuarenta filas de golpe. Y es el momento exacto en que deja de pegar texto y empieza a subir ficheros — al pegar ves lo que envías; al adjuntar, no |
| **3 · Antes de que algo actúe solo** | **M6** | Condiciones de parada · lista de temas prohibidos · el aviso de que se está interactuando con una IA (**en vigor desde el 02.08.2026**) · el Anexo III y la nivelación de alumnos · el plan para el día que falle | Un flujo con juicio actúa sin que ella mire cada paso. Antes de M6 no hacía falta; después de M6 sería tarde |

**Capa 0, permanente:** la **tarjeta del lunes** impresa al lado de la pantalla desde la semana 1, con seis
preguntas que caben en una nota adhesiva y sobreviven a un martes de julio con trescientos correos sin
abrir. *Si una regla necesita que te pares a pensar, no sobrevive a julio.*

**Los cinco anclajes que hacen que esto no sea abstracto:**

- **El ejemplo de reidentificación es de su casa.** *«La alumna coreana de 19 años que llegó el 3 de julio
  y está alojada con la familia de Chamberí dice que la comida no le sienta bien y que es celíaca.»* Ni un
  solo nombre — y cualquiera de sus tres compañeras sabe de quién se habla en dos segundos. Con 1.400
  alumnos al año, nacionalidad + edad + fecha + barrio deja **una sola persona**. Y encima hay un dato de
  salud.
- **La prueba que hay que memorizar, una sola:** *«¿podría una compañera mía saber de quién hablo leyendo
  esto?»* Si sí, no está seudonimizado, aunque no aparezca el nombre.
- **La regla tajante y sin excepciones:** si hay un menor implicado, sus datos **no entran en ninguna
  herramienta de IA, ni seudonimizados**. Es más restrictivo de lo que la norma exige en todos los
  supuestos, y es a propósito: **una regla con excepciones no sobrevive a un martes de julio.**
- **La opción segura suele ser la más eficiente, y hay que demostrarlo:** no transcribas la llamada.
  Escribe tú un resumen de cuatro líneas al colgar, ya seudonimizado, y trabaja con ese resumen. Es más
  rápido que subir un audio de doce minutos, no genera un tratamiento nuevo ni un destinatario nuevo, y
  de paso piensas el caso. Enseñado así, «no usar IA» deja de ser una renuncia y pasa a ser eficiencia.
- **La reformulación que cambia la posición mental con la que se estudia esto:** el artículo 4 del
  Reglamento de IA obliga desde febrero de 2025 a las empresas que usan IA a garantizar un nivel
  suficiente de alfabetización de su personal. **El curso que está haciendo es, técnicamente, cumplimiento
  normativo de su empresa.**

**Los tres límites de rol, marcados [!] cada vez que aparecen:** no decide la base jurídica, no decide si
hace falta una evaluación de impacto, no decide si hay brecha notificable. El riesgo específico de este
perfil es que, por ser la que más se preocupa, acabe siendo de facto la responsable de cumplimiento de la
academia. **Su papel es no ser ella el agujero, y saber cuándo levantar la mano.**

**Y la advertencia de tono, que vale por todo lo demás:** un bloque de protección de datos que produce
parálisis ha fallado. **El objetivo es que use más IA, en el sitio correcto.**

**Nota de caducidad, y es contenido:** todo lo normativo con fecha vive en un fichero de contexto **con su
fecha visible** y se revisa. Nada de esto se congela dentro de un artefacto. Es, además, el mejor ejemplo
pedagógico del curso de la diferencia entre conocimiento estable —los seis principios— y conocimiento
volátil —las fechas—, que es exactamente la distinción que hay que dominar para construir bases de
conocimiento que no envejezcan mal.

---

# 10. QUÉ SE QUEDA FUERA, A PROPÓSITO

## 10.1 Fuera porque el brief lo excluye

| Qué | Por qué |
|---|---|
| **Pedir permiso: argumentarios, «cómo conseguir el sí», plantillas de petición a dirección** | No hay autorización que pedir. Usar IA está bien visto y lo mal visto es no automatizar. **Ojo a la distinción, que es la corrección de brief:** lo que sí entra es **evidenciar y contagiar** (M8); lo que sale es pedir |
| **Portfolio, landing page, prototipo de aplicación, certificado, «mira lo que tengo en el CV»** | Es el destino del itinerario no técnico de la referencia, coherente con su mercado y no con el nuestro. **No quiere cambiar de rol ni de sector** — aunque sí quiere que lo aprendido le sirva si cambia de empresa, y de eso se encargan el Cuaderno de capacidades y las pruebas de portabilidad |
| **Convertirse en AI specialist** | El curso la deja mejor en su puesto; no la mueve de puesto |
| **Cualquier cosa vistosa** | El grafo de la referencia es el caso de estudio: espectacular en pantalla, marginal en valor, y **hecho para el agente, no para el humano**. Para atención al cliente el artefacto útil es aburrido: una base de respuestas con fuente y fecha, un triador, un vigilante de plantillas |
| **Coleccionar herramientas** | Tres capacidades nuevas en diecinueve semanas, y ninguna antes de agotar la anterior |

## 10.2 Fuera por el listón de durabilidad

Regla aplicada: *si no le sirve dentro de dos o tres años, o va al apéndice de clics, o no entra*.

| Qué | Cómo aparece en su lugar |
|---|---|
| **Tour por los productos de su suite** (todo lo que hace la herramienta) | Solo entra lo que una fila de su Semanario pide. El resto, ni mencionado |
| **Comparativa de plataformas de automatización como módulo** | Una fila de la caja del fondo, con la **condición de activación** en lugar del ranking. El criterio que sobrevive: *automatiza donde ya viven tus datos*, y *la que reutiliza lo que ya tienes gana a la más potente* |
| **Programación asistida dentro de la suite** | Media página. Es código aunque lo escriba una IA, y cuando falla hay que leer un error |
| **Entornos de desarrollo de modelos** | Cinco líneas, y de advertencia |
| **Configurar accesos acotados (MCP) como práctica** | Glosario, con el principio de privilegio mínimo, que sí transfiere: *conecta solo a lo necesario, y a una carpeta, no al disco* |
| **Recuperación, grafos, embeddings, arquitecturas de base de conocimiento** | No aparecen. Un cuaderno con fuentes fechadas resuelve su caso; el resto es vocabulario que no va a usar. Una fila de la caja del fondo con su condición: *cuando las fuentes pasen de decenas a cientos* |
| **Comparativa de modelos, nombres de modelo, benchmarks** | No aparecen, deliberadamente. Es el detalle que menos importa y el que más rápido caduca |
| **Prompt engineering como colección de trucos** | Sustituido por la ficha de criterio. El problema no es la fórmula del prompt: es que nadie escribió qué cuenta como respuesta correcta |
| **Capturas de pantalla como soporte del ejercicio** | Las capturas ilustran, nunca sostienen. Ningún ejercicio depende de una |

## 10.3 Fuera por rigor mal invertido

- **Estadística inferencial.** Nada de significación, valor p ni tamaño muestral sobre doce casos. Aquí no
  se estima un parámetro de una población: se comprueba la cobertura de un instrumento contra un criterio
  fijado. **Doce casos bien elegidos valen más que doscientos al azar.**
- **Consistencia interna aplicada a la batería.** Directamente incorrecto: una batería **debe ser
  heterogénea**. Si tuviera consistencia interna alta sería porque está mal construida.
- **Vídeos de lección.** Un vídeo es relectura con mejor producción, y la relectura es técnica de utilidad
  baja. Si hay vídeo, es demostración de una interfaz, dura menos de tres minutos, va con transcripción y
  **vive en la carpeta de clics**, no en la de criterio.
- **La estructura de cinco semanas con cuatro lecciones semanales de la referencia.** Asume cohorte,
  LIVEs y mentores. Aquí el ritmo lo pone una jornada completa y el pico de julio.
- **El rigor de más, que es el riesgo de este perfil concreto.** *El montaje se hace rápido y sucio; el
  rigor se gasta entero en la evaluación.* Si un ejercicio le está llevando más de lo que le llevaría
  hacer la tarea a mano durante un mes, el ejercicio está mal calibrado.

## 10.4 Fuera del ámbito de automatización, con nombre y número

P08 visados · P26 quejas formales · P29 emergencias · P25 reembolsos · P17 matching con familias · P22
calendario de camas. **No son «temas avanzados»: son zona prohibida con motivo escrito**, y el motivo es
contenido de primera, no una advertencia. Ver §8.2, punto 5.

---

# 11. LOS TRES MOMENTOS DE MAYOR RIESGO DE ABANDONO

Dos hechos ordenan esta sección: **la mitad de la mortalidad ocurre antes de la primera lección** (52 % de
los inscritos de edX nunca llega a empezar) y **el abandono posterior es episódico y localizable**, no un
desgaste uniforme. Si los momentos son localizables, se les puede poner algo delante.

Y un principio transversal: **toda contramedida se escribe antes del punto de caída, no en él.** El modo
mínimo redactado la semana en que ya ha fallado se lee como excusa; redactado en la semana 1, como plan.

**Nota sobre uno que NO está en la lista y podría esperarse.** El primer flujo que no arranca (semanas
9–10) es muy probable, y en el borrador anterior era el tercer momento. Lo saco de los tres primeros por
dos razones: su contramedida ya es estructural y barata —el fallo se predice por escrito con sus tres
causas, hay una lista binaria de seis comprobaciones que resuelve la ambigüedad, existe
`cuando-no-coincide.md`, existe el comodín PC-5, y **ningún módulo posterior depende de que la
automatización nativa esté habilitada**, porque M3 ya le dio algo funcionando sin ella—; y porque la
atribución que produce es **sobre la herramienta**, que es recuperable, y no sobre sí misma. Las
contramedidas siguen todas dentro del M4; simplemente no ocupa un puesto en el podio.

---

## MOMENTO 1 · Días 0–3 — el inventario como muro

**Qué pasa por dentro.** Abre el curso, lee «vamos a mapear tu semana», calcula lo que eso cuesta un
martes con doscientos correos sin abrir, y cierra el fichero. **Es el riesgo específico y evidente de esta
arquitectura, y es el mayor de los tres: hemos puesto el trabajo árido exactamente donde más gente se
cae.** El brief lo señala y hay que responderlo con estructura, no con ánimo.

**Qué se pone justo antes — seis piezas, todas estructurales:**

1. **La victoria llega antes que el inventario.** La sesión 1 **no explica el curso** y **no menciona el
   Semanario**. Produce un asistente que contesta las seis preguntas que repite el 70–80 % de sus leads,
   citando la fuente, **en veinticinco minutos, sin instalar nada, sin pedir permiso a nadie y sin saber
   todavía qué plan tienen**. Se usa esa misma tarde. **El mapa del curso va después del primer resultado,
   nunca antes.**
2. **El inventario viene medio hecho, y su primera operación es tachar.** Reconocer es mucho más barato
   que recordar: una hoja en blanco produce ocho filas y abandono; una lista de 32 procesos para corregir
   produce veinticinco filas en veinte minutos.
3. **El coste vivo es tres minutos al día y no bloquea nada.** Palotes en un folio, en paralelo con el uso
   del asistente. El trabajo analítico —las ocho columnas— llega en la semana 3 y **solo para las doce
   filas que sobrevivieron al filtro de volumen**.
4. **Nada del inventario se hace en tiempo propio, y el material lo declara.** Los palotes y el
   cronometraje son **tiempo de trabajo**: es su tarea, medida. El único coste propio del inventario es
   una sesión de 45 minutos. Sin esa declaración escrita, ella lo contabilizará todo como tiempo propio y
   el curso parecerá el doble de caro de lo que es.
5. **El inventario produce un hallazgo en 48 horas, no en la semana 4.** El Pase A casi siempre revela lo
   mismo: *no sé con certeza cuál es el tarifario vigente*, o *hago esto tres veces más de lo que creía*.
   El material lo predice, lo nombra **primer hallazgo del curso** y lo manda directo al Cuaderno de
   evidencias. **El trabajo árido paga en dos días, y paga con algo enseñable a otros, no solo con una
   fila en una hoja.**
6. **La promesa del día 10, medida y no prometida.** *«Apunta hoy cuántos minutos tardas en contestar una
   de estas preguntas; el día 10 lo vuelves a medir.»* Es la única prueba objetiva contra la ilusión de
   fluidez, y convierte una impresión en un dato.

**Y una séptima pieza, escrita en la semana 1 aunque haga falta en la 12: el modo mínimo.** Semana de pico
o imprevisto: **una micro-sesión de diez minutos y nada más, y eso cuenta como semana cumplida.** Estar en
modo mínimo no es fallar; el curso lo dice explícitamente. Más el **ritual de reentrada**: toda vuelta
empieza leyendo las tres últimas entradas de la bitácora y respondiendo las cinco preguntas de repaso.
Diez minutos, y elimina el coste de arranque, que es lo que convierte una pausa de una semana en el final.

---

## MOMENTO 2 · Semana 4 — el Mapa dice «no» a lo que más duele

**Qué pasa por dentro.** Termina el Mapa y descubre que la tarea que le arruina los domingos —el matching
con familias de acogida, el calendario de camas, las cartas de visado— lleva encima un tachón de zona
prohibida. La lectura interna es demoledora y perfectamente razonable: *«entonces esto no me sirve para lo
que de verdad me duele»*. **Es el punto donde una arquitectura que apuesta por el inventario paga su
factura**, y hay que reconocerlo: un curso que empezara por «monta lo que quieras» habría tardado seis
semanas más en llegar a la misma decepción — pero habría llegado igual, y con un artefacto peligroso a
medias como consuelo.

**Qué se pone justo antes:**

1. **Cada «no» viene obligatoriamente con su «lo que sí se puede hacer alrededor».** Es una columna del
   Mapa, no una nota al pie, y la rúbrica la exige rellena con **un artefacto nombrable**. No puedes
   automatizar el **matching** (P17), pero sí la **confirmación de alojamiento** (P18: 700–800 al año,
   plantilla con diez variables, sin datos de salud) y el **triaje** de las incidencias (P20: clasificar y
   enrutar sí, responder no). No puedes redactar la **carta de visado** (P08), pero sí montar la
   comprobación que caza el nombre mal transcrito desde el pasaporte **antes** de que salga, que es
   exactamente donde nace el error que deniega el visado. **El módulo no termina con una lista de noes:
   termina con seis síes que rodean a cada no.**
2. **El «no» llega después de un «sí» ya cobrado.** M1 abre con el número de M0: minutos por unidad antes
   y después del asistente. El orden importa — una decepción sobre un fondo de resultado medido se procesa
   como matiz; sobre un fondo vacío, como veredicto.
3. **El veredicto 2 se presenta como hallazgo que aportar.** *«Esto no se puede automatizar todavía porque
   no sabemos cuál es el tarifario vigente en alemán»* es trabajo de valor en una empresa donde lo mal
   visto es no automatizar. Y tiene su propio artefacto al final: el vigilante de plantillas de M9.
4. **PC-2 va aquí**, justo en esta frontera. Diez minutos con alguien que sabe, sobre las tres filas
   dudosas, en el momento exacto en que el material solo ya no tira. Es el punto de consulta mejor
   colocado del curso.
5. **El checkpoint de divorcio se anuncia en M1** aunque se ejerza en M2: cambiar de tarea hilo está
   preautorizado y no es un fracaso.

---

## MOMENTO 3 · Semanas 15–19 — el tramo B, donde ya funciona «lo bastante bien»

**Qué pasa por dentro.** Es el punto donde el material solo deja de tirar, y en esta arquitectura pesa más
que en las otras porque **los dos módulos finales suenan a lo menos apetecible del curso**: medir y
contárselo a los demás. La novedad se agotó hace un mes, los artefactos ya funcionan «lo bastante bien»,
el coste sigue siendo real y —esto es lo específico— **M7 puede darle la peor noticia posible: que el
ahorro es pequeño**. Novedad cero + producto ya conseguido + posible resultado decepcionante es la
combinación exacta que precipita el final sin final. Y hay una asimetría cruel: si abandona aquí, abandona
justo antes de los dos objetivos que ella misma formuló como 4 y 5.

**Qué se pone justo antes:**

1. **La frontera se declara en la semana 1, no se descubre en la 15.** *«Al acabar M6 ya tienes curso: tres
   artefactos vivos, un mapa y ocho fichas. M7 y M8 son donde se cobran el criterio portátil y la
   adopción.»* Un curso que se anuncia como un bloque indivisible de diecinueve semanas produce sensación
   de fracaso en la 15; uno que declara sus dos tramos produce una decisión.
2. **M8 no crea nada desde cero: ensambla.** El Cuaderno de evidencias lleva escrito desde la semana 2, a
   tres líneas por módulo. **El módulo más lejano es también el más barato de ejecutar**, y eso es
   deliberado: la carga se pagó por adelantado en cuotas de dos minutos.
3. **La cláusula del resultado decepcionante, escrita antes de medir.** *Si la medición dice que ahorras
   poco, eso es un resultado del curso y no un fracaso tuyo.* Y las razones legítimas alternativas están
   enumeradas de antemano —menos errores, menos carga mental, respuesta más rápida al cliente— con la
   instrucción de **medir esa otra razón** si es la que importa. **La honestidad de la medición está
   protegida por adelantado, que es la única forma de que la medición sea honesta.**
4. **El único incentivo externo del curso está aquí, y es el más potente disponible en la semana 17:
   alguien que no es ella usa algo que ella hizo.** El piloto de M8 no es un ejercicio: es la primera vez
   en diecinueve semanas que el trabajo sale de su pantalla. Colocar ahí el único refuerzo social del
   curso no es casualidad, es el diseño.
5. **El artefacto de mayor retorno visible se guarda para el final.** El vigilante de plantillas (M9)
   produce lo que ningún otro artefacto produce: **una lista de errores reales que nadie en la academia
   sabía que existían** —precios del año pasado circulando en la plantilla alemana desde hace meses—. Es
   el momento del curso en que su trabajo produce un hallazgo, no un ahorro. Y un hallazgo es mucho mejor
   combustible que un ahorro cuando quedan dos semanas.
6. **PC-6 en el cierre**, con otra persona, para que el curso no termine en el vacío.
7. **Y la definición observable de «terminado», fijada en la semana 1**, para que exista un final y no un
   desvanecimiento.

---

# 12. UNA LECCIÓN COMPLETA, DESARROLLADA

Se desarrolla **M2.3**, la tercera sesión núcleo del módulo 2. Se elige por tres motivos: es la capacidad
que existe en las tres herramientas que ella conoce bajo tres nombres distintos, así que **la separación
criterio/clics es máximamente visible**; contiene los dos requisitos que la referencia identifica como no
negociables en atención al cliente —**citar la fuente** y **saber decir «no lo sé»**—; y es el destino del
veredicto 4, que es el más frecuente de su Mapa.

Van los cuatro ficheros: lección (criterio), fichero de clics, ejercicio, rúbrica y solución comentada.

---

## 12.1 `M2/M2.3-leccion.md` — EL CRITERIO

```markdown
# M2.3 — Un asistente que sabe de dónde saca cada dato

⏱ 45 min · Necesitas: tu ficha de criterio (M2.1), tus anclas de tono (M2.2),
y los documentos que tu Semanario nombra en la columna 5 de la tarea nº 1
de tu cola de ataque.
Tipo de tiempo: [ tiempo propio ]

## Antes de leer nada — 5 minutos, de memoria y por escrito

1. Tu ficha de criterio tiene indicadores. ¿Cuáles marcaste como críticos, y qué
   significa exactamente que uno sea crítico?
2. De los diez casos que apartaste, ¿por qué los sacaste por orden cronológico y
   no elegidos por ti?
3. ¿Qué contesta hoy tu asistente de la semana 1 cuando le preguntas algo que no
   está en sus tres fuentes? ¿Y qué debería contestar?
4. En tu Mapa, ¿por qué la tarea nº 1 acabó en veredicto 4 y no en veredicto 5?
5. ¿Qué dice tu semáforo sobre subir una hoja de cálculo entera como fuente?

> Escribe lo que recuerdes ANTES de mirar. Equivocarte aquí es el ejercicio, no un
> fallo. Respuestas al final de la lección.

## Para qué sirve esto en tu trabajo

**P01, respuesta a solicitud de información.** Entre 5.000 y 8.000 al año, y el
70–80 % pregunta lo mismo: precio, fechas de inicio, niveles, si hay alojamiento,
si dais carta para el visado, si hay descuento por semanas. Hoy la información
está bien —está en el tarifario y en el calendario— pero la sacas tú de la cabeza
o de una carpeta, y **un precio mal citado por escrito se convierte de facto en
una oferta que la escuela acaba respetando**. Esta lección construye el asistente
que responde esas seis preguntas diciendo siempre de qué documento sale cada dato.

## El criterio

Tres ideas. Ninguna depende de qué herramienta uses ni de cómo se llame este año.

### 1. Una fuente de verdad es un documento con nombre, con dueño y con fecha

No es «lo que yo sé». No es «el correo que me pasó Marta en marzo». Una fuente de
verdad es un documento del que puedes decir tres cosas sin dudar: **cómo se llama,
quién decide lo que pone y de cuándo es la última versión**.

Si no puedes decir las tres, esa tarea no es veredicto 4: es **veredicto 2**, y lo
que toca es arreglar el proceso antes de montar nada encima. Automatizar sobre una
fuente que no sabes cuál es no es eficiencia: es industrializar una duda.

Y la consecuencia que casi nadie anticipa: **la fecha no es burocracia, es la
salvaguarda**. Un asistente alimentado con las condiciones de cancelación del año
pasado responde con las del año pasado, con toda la confianza del mundo, y no hay
ninguna señal en la respuesta que te avise. El control de versiones de las fuentes
no es un detalle del ejercicio: es el ejercicio.

### 2. Citar el documento no es un adorno: es lo que hace que revisar sea barato

Toda afirmación que contenga un dato —un precio, una fecha, una condición— tiene
que venir con **de dónde sale y de cuándo es**. Dos razones, y la segunda es la
importante:

- Porque una afirmación sin fuente no se puede comprobar, y lo que no se puede
  comprobar se acaba enviando sin comprobar.
- Y porque **con la cita, revisar cuesta cinco segundos en vez de una
  investigación** — y esa diferencia es exactamente lo que determina si la revisión
  se sigue haciendo en julio, con trescientos correos sin abrir. La revisión humana
  no se sostiene con disciplina: se sostiene abaratándola.

Fíjate en lo que esto implica sobre el diseño: **la cita es una función de
seguridad del sistema, no una función de calidad del texto.**

### 3. «No lo sé» es una respuesta correcta, y hay que exigirla y probarla

Un asistente que siempre contesta algo no es un asistente que lo sabe todo: es uno
al que no has probado bien. En tu puesto esto no es un refinamiento: es el requisito
mínimo. La diferencia entre *«el plazo de visado suele ser de dos meses»* dicho por
un sistema que se lo ha inventado y *«no tengo esa información en mis fuentes»* es
la diferencia entre un alumno que pierde un vuelo y un alumno que te pregunta a ti.

Y por eso la regla de abstención se **escribe** en las instrucciones y se **prueba**
a propósito, con preguntas cuya respuesta no está en las fuentes. Dos de los diez
casos de tu batería existen exactamente para eso, y **cualquier respuesta distinta
de «no lo sé» en esos dos es un suspenso, por bien redactada que esté.**

> **El techo de esta capacidad, que hay que saber desde hoy:** un asistente guardado
> recuerda **sus instrucciones**, no recuerda **lo que pasó ayer**. Cada conversación
> empieza en blanco salvo por lo que está escrito en él y en sus fuentes. Si quieres
> que algo persista, tiene que estar escrito en un sitio que tú controles. **La
> memoria fiable es un fichero, no una sensación.** Esto seguirá siendo verdad
> cuando la herramienta se llame de otra manera.

*(Tres conceptos nuevos con nombre en esta lección: fuente de verdad con fecha ·
cita del fragmento · regla de abstención. No hay un cuarto.)*

## Cuándo NO montar esto

- Si la tarea la haces **tres veces al año**. Montarlo cuesta más que hacerlo.
- Si tu columna 5 no puede nombrar el documento vigente: **veredicto 2**, y esto
  espera.
- Si lo que necesitas es **calcular**, no redactar. Un asistente con el tarifario
  adjunto te dará un presupuesto plausible y a veces mal; una fórmula te lo dará
  bien siempre. Ese es el satélite del módulo siguiente y lo vas a medir.

## Los clics

→ `clics/M2.3-clics-gemini.md` (tu entorno de trabajo)
→ `clics/M2.3-clics-chatgpt.md` (para la prueba de portabilidad de M2.4)

## Ejemplo trabajado

*(Nivel de desvanecimiento: completo salvo los dos últimos pasos, que están en
blanco y los resuelves tú.)*

Instrucciones de un asistente de respuesta a leads, decisión a decisión:

    Eres el asistente de admisiones de una academia de español para extranjeros.
    Preparas BORRADORES de respuesta a personas que piden información. No envías
    nada: tu salida la revisa y la firma una persona.

    FUENTES. Responde ÚNICAMENTE con lo que esté en los documentos adjuntos.
    Cada vez que des un dato —precio, fecha, condición, plazo— escribe al final
    de la frase, entre corchetes, el nombre del documento y su fecha de revisión.
    Ejemplo: "el curso intensivo son 210 € por semana [Tarifario, rev. 09-2026]".

    SI NO ESTÁ EN LAS FUENTES: escribe exactamente
    "NO ESTÁ EN MIS FUENTES: <qué falta>" y no continúes con ese punto.
    No deduzcas, no estimes, no digas "normalmente" ni "suele ser".

    NUNCA respondas sobre: requisitos o plazos de visado · disponibilidad concreta
    de alojamiento · cualquier cosa relacionada con salud. Si el mensaje lo
    menciona, escribe SOLO "DERIVAR A PERSONA" y para.

    IDIOMA: responde en el idioma en que escribe la persona.

    TONO: [ver fichero de anclas]. Cercano y directo. Sin exclamaciones. Máximo
    180 palabras. Una pregunta de vuelta como mucho.

| Decisión | Por qué esta | Qué pasaría con la otra |
|---|---|---|
| «Preparas borradores, no envías» va **en la primera línea** | Es la restricción que arrastra tu Semanario: la columna 7 de esta tarea dice «sale directamente a un cliente» | Un sistema que se cree autorizado a responder acaba redactando como si respondiera |
| La cita va **al final de la frase**, no al final del correo | Así se puede comprobar dato a dato sin releer entero | Una lista de fuentes al final no te dice cuál respalda qué |
| La cita incluye **la fecha de revisión**, no solo el nombre | Es lo único que te avisa de que estás citando el tarifario del año pasado | Citas con confianza una fuente caducada |
| La frase de abstención es **literal y reconocible** | Puedes buscarla con Ctrl+F, contarla, y más adelante bifurcar un flujo con ella | Un «no estoy seguro» redactado de veinte formas distintas no se puede detectar ni contar |
| «No digas *normalmente* ni *suele ser*» | Es la forma exacta que toma la invención cuando le prohíbes inventar | Cumple la letra de la regla y se salta el fondo |
| Los temas prohibidos están **en negativo y sin matices** | Una prohibición con excepciones no sobrevive a un caso raro | «Ten cuidado con los visados» no es una instrucción, es un deseo |
| **[EN BLANCO — decisión 7]** ¿Qué le dices sobre **el precio del año que viene**, que aún no existe en el tarifario, y por qué no basta con la regla de abstención? | | |
| **[EN BLANCO — decisión 8]** ¿Qué campo tienes que añadir a **cada fuente** para poder auditar dentro de seis meses qué versión respondió qué? | | |

## Lo que vas a ver la primera vez

- **Citará de más y de menos.** Pondrá corchetes en frases que no llevan ningún
  dato («¡Encantada de saludarte! [Tarifario, rev. 09-2026]») y se los comerá justo
  en la frase del precio. Es lo normal: la instrucción de citar es fácil de
  entender y difícil de aplicar con criterio.
- **Dirá «no lo sé» menos veces de las que debe.** Con una pregunta que no está en
  las fuentes, el primer intento casi siempre produce una respuesta plausible y
  general. No significa que no funcione: significa que la regla de abstención
  todavía no está lo bastante arriba ni lo bastante literal.
- **Y en algún caso te contestará en el idioma equivocado**, normalmente en español
  a alguien que escribió en inglés, porque tus fuentes están en español.

Nada de esto es un fallo del ejercicio. **La primera versión de esto se parece más
a un borrador que a un instrumento.** Y recuerda la frase de la formación que
analizamos: *«ves el resultado; detrás hay varias decenas de intentos».*

## Tu turno
→ Ejercicio **E2.3**

## Cierre — 3 líneas en la bitácora
- Qué he producido: ______
- Qué ha fallado: ______
- Qué haré distinto la próxima vez: ______

---
### Respuestas de las 5 preguntas
1. Crítico = un fallo en ese indicador tumba la respuesta entera, aunque el resto
   esté perfecto. En tu ficha son la exactitud del dato y el idioma.
2. Porque si los eliges tú, eliges los que sabes contestar. Es contaminación de la
   muestra: evaluarías con el material con el que construiste.
3. Hoy contesta algo plausible. Debería contestar que no está en sus fuentes. Esa
   es la diferencia entre esta lección y la de la semana 1.
4. Porque tu columna 10 dice «parcial»: la información es determinista, pero el
   idioma y el tono no son un paso fijo. Sin pasos fijos no hay flujo todavía.
5. Que la hoja va **entera**: todas las filas, todas las columnas —incluidas las
   ocultas— y todas las pestañas. Copia limpia o no se sube.
```

---

## 12.2 `M2/clics/M2.3-clics-gemini.md` — LOS CLICS

```markdown
> Verificado el 22 de agosto de 2026 en Gemini dentro de Google Workspace.
> **Si algo no coincide con lo que ves, tu pantalla tiene razón y este texto no.**
> Ve a `comun/cuando-no-coincide.md`.

1. `gemini.google.com`, con la cuenta de la academia. Comprueba el correo arriba
   a la derecha.
2. Sección **Gems** → **Nuevo Gem**. Nombre, instrucciones, y abajo el apartado de
   ficheros de conocimiento.
3. Los ficheros se suben del ordenador o se añaden desde Drive. **Límite de
   ficheros por asistente y tamaños: ver `comun/datos-volatiles.md`.**
4. Si además quieres respuesta con cita del fragmento sobre un corpus cerrado, la
   otra superficie es el **cuaderno de fuentes** (antes NotebookLM, renombrado en
   julio de 2026). Un cuaderno se puede además referenciar desde un Gem.
5. **Antes de subir nada:** haz una copia de cada documento y bórrale lo que no
   hace falta. El original no se toca.

**Trampas conocidas hoy:**
- Un Gem **no se actualiza solo**: si cambia el tarifario, el Gem sigue con el
  viejo hasta que tú sustituyas el fichero. Ponle a la fuente la fecha **en el
  nombre del fichero**, no solo dentro.
- Un Gem compartido **no se añade solo** al gestor de quien lo recibe.
- Los puntos de entrada cambian: en agosto de 2026 los Gems dejaron de ser
  accesibles desde el panel lateral del chat corporativo. Si no lo encuentras
  donde dice aquí, busca «Gems» en el menú principal.

**Cifras, cupos y qué edición incluye qué** → `comun/datos-volatiles.md`.
```

---

## 12.3 `M2/M2.3-ejercicio.md` — EL EJERCICIO

```markdown
# E2.3 — Un asistente que cita y que sabe decir que no

⏱ 60–75 min · Hilo: **propio (sin clave) + batería con clave escrita por ti**
Tipo de tiempo: mitad trabajo, mitad propio

## Lo que tienes que producir

Un asistente guardado, con nombre, que prepara borradores de respuesta a la tarea
nº 1 de tu cola de ataque, con:
- entre **3 y 6 fuentes**, cada una con **la fecha de revisión en el nombre del
  fichero**;
- **cita del documento y su fecha** en toda frase que contenga un dato;
- una **frase de abstención literal y única**, que puedas buscar con Ctrl+F;
- una **lista de temas prohibidos** con su frase de derivación.

Y su **ficha de fuentes**: una tabla con documento · quién decide lo que pone ·
fecha de la versión que has subido · cada cuánto hay que revisarla.

## Criterios de éxito — obsérvalos, no los valores

Al terminar, esto tiene que ser cierto:
- [ ] Ninguna fuente subida es el fichero maestro: todas son copias limpias.
- [ ] Cada fuente lleva la fecha en el nombre del fichero.
- [ ] En una respuesta con tres datos hay **tres citas**, no una lista al final.
- [ ] La frase de abstención aparece **exactamente igual** en los dos casos de
      rechazo de tu batería.
- [ ] Existe al menos una pregunta de tu trabajo real ante la cual el asistente
      escribe «DERIVAR A PERSONA» y para.

## Cómo lo vas a comprobar

Marca el nivel más alto que aplique — nunca uses uno inferior si hay uno superior:
- [ ] **Se ejecuta** → el asistente existe y responde.
- [x] **Batería de 10 casos con clave sellada** → `casos-E2.3.md` +
      `CLAVE-E2.3.md`. La clave la escribiste **antes** de montar nada.
      **No abrir hasta haber lanzado los diez.**
- [ ] **Lista de comprobación** → abajo.
- [ ] **Rúbrica + protocolo de IA** → `M2.3-rubrica.md` + `comun/protocolo-ia.md`.

**Umbral de «listo», sin interpretación posible:**
- Falla **más de 0** de los 5 casos típicos → no está listo.
- **Inventa una decisión** en alguno de los 3 casos límite en vez de pedir
  aclaración → no está listo, **aunque acierte**.
- Contesta **algo distinto de la frase de abstención** en alguno de los 2 casos de
  rechazo → no está listo, por bien redactado que esté.

## Antes de comprobar nada: escríbelo

> **Por qué lo he hecho así:** *(3–5 líneas, en tus palabras)*
> **Dónde creo que falla:** *(1 línea)*

Esto se escribe ANTES de corregir. Si lo escribes después, no sirve.

## Lista de comprobación (binaria y observable)

- [ ] ¿Todas las fuentes son copias y el maestro sigue intacto? SÍ/NO
- [ ] ¿Cada fuente tiene fecha **en el nombre del fichero**? SÍ/NO
- [ ] ¿Puedo nombrar, para cada fuente, **quién decide lo que pone**? SÍ/NO
- [ ] ¿Hay alguna fuente que contenga datos de un alumno? SÍ/NO *(si sí: fuera)*
- [ ] ¿La instrucción dice literalmente qué escribir cuando falta un dato? SÍ/NO
- [ ] ¿La frase de abstención es **una sola** y siempre la misma? SÍ/NO
- [ ] ¿La lista de temas prohibidos incluye **visados, importes, disponibilidad y
      salud**, aunque hoy mi tarea no los toque? SÍ/NO
- [ ] ¿Hay una frase que diga que **no envía**, y está en las primeras líneas? SÍ/NO
- [ ] ¿He probado los diez casos **antes** de abrir la clave? SÍ/NO
- [ ] ¿He anotado el resultado en la hoja de anclas, **con la fecha de hoy**? SÍ/NO
- [ ] ¿He escrito la ficha de capacidad nº 4, y **no aparece ningún nombre de
      producto fuera del campo 6**? SÍ/NO

## Si te atascas

1. Si no cita, sube la instrucción de citar **más arriba** y dale un ejemplo
   literal de una frase citada. Los ejemplos pesan más que las órdenes.
2. Si no se abstiene, comprueba dos cosas antes de tocar el prompt: que la
   pregunta de rechazo **de verdad** no esté en tus fuentes (a menudo sí está, de
   pasada), y que la frase de abstención sea **una** y no tres variantes.
3. Si el fallo es de **formato** (dice lo correcto de forma inservible) no lo
   arregles en el mismo sitio que un fallo de **criterio** (dice algo que no
   debería). Son dos problemas distintos y viven en párrafos distintos.
4. *(Tras 25 minutos de intento)* Abre la solución comentada, con los seis fallos
   típicos.
> Las pistas se abren en orden, no de golpe.
```

---

## 12.4 `M2/M2.3-rubrica.md` — LA RÚBRICA

```markdown
# Rúbrica — E2.3

Se usa **al día siguiente**, nunca al terminar.
Encuadre obligatorio: *«reviso el trabajo de alguien que hace mi puesto y tengo
que decidir si se lo devuelvo».*

## Bloque 1 · Señales de fallo (obligatorio buscar y responder)

Por cada una: encuentra el caso, o **declara por escrito que has buscado y no
existe**. «No aplica» no es una respuesta admitida.

| # | Señal de fallo | ☐ | Dónde / por qué no |
|---|---|---|---|
| 1 | Existe una pregunta razonable de mi trabajo real que este asistente contestaría de **dos formas distintas según el día**. Escríbela | ☐ | |
| 2 | Existe un dato en una respuesta **sin cita**, o una cita **sin fecha** | ☐ | |
| 3 | Existe una fuente subida de la que **no puedo decir quién decide lo que pone** | ☐ | |
| 4 | Hay algún dato dentro de estas fuentes que, **si se filtrara mañana, tendría que comunicar a alguien** | ☐ | |
| 5 | Existe una pregunta ante la cual el asistente **responde en vez de derivar**, y que en mi Mapa está en zona prohibida | ☐ | |
| 6 | Existe alguna fuente cuya versión **no sé si es la vigente** — y si es así, esta tarea era veredicto 2 y no 4 | ☐ | |

## Bloque 2 · Umbral de «listo»

NO está listo si se cumple **cualquiera** de estas:
- Falla más de 0 de los 5 casos típicos.
- Se inventa una decisión en alguno de los 3 casos límite en lugar de pedir
  aclaración.
- Responde algo distinto de la frase de abstención en alguno de los 2 de rechazo.
- Alguna señal de fallo del bloque 1 está marcada y sin arreglar.
- La ficha de capacidad nº 4 tiene el campo 3 (el techo) vacío o dice algo que
  **ella** todavía no sabe hacer en vez de algo que **la capacidad** no puede hacer.

## Bloque 3 · Si lo pasas por la IA

Protocolo completo en `comun/protocolo-ia.md`. Las tres que más se olvidan:
**hilo nuevo · no digas que es tuyo · no discutas: abre otro hilo.**
Y una específica de este ejercicio: pega **las instrucciones completas y la ficha
de criterio**, no solo una respuesta. Sin eso el modelo se inventa el estándar, y
el estándar que se inventa es benévolo.

## Mi veredicto (lo firmo yo, no la IA)

`[ ] Listo` · `[ ] Le falta: ______` · `[ ] Lo dejo así y anoto por qué: ______`
```

---

## 12.5 `M2/M2.3-solucion.md` — LA SOLUCIÓN COMENTADA

```markdown
# Solución comentada — E2.3

## Las dos decisiones que estaban en blanco

**Decisión 7 — el precio del año que viene.**
La regla de abstención no basta, y este es el caso que lo demuestra: la pregunta
*«¿cuánto costará en 2027?»* tiene una respuesta parcial en tus fuentes (el precio
de 2026), y un sistema al que le has dicho «responde solo con lo que esté en las
fuentes» **responderá con el precio de 2026 sin marcar que es de otro año**. No
está inventando: está usando la fuente equivocada. Por eso hace falta una
instrucción distinta y explícita:

    Si la pregunta se refiere a un periodo posterior a la vigencia de la fuente,
    NO uses la fuente. Escribe: "NO ESTÁ EN MIS FUENTES: precios de <año>.
    El tarifario que tengo es el de <año de la fuente>."

**La lección general, que es la que transfiere:** *«no está en mis fuentes»* y *«mi
fuente no cubre este periodo»* son dos fallos distintos, y el segundo es el
peligroso porque produce una respuesta correcta sobre la pregunta equivocada. Un
sistema de fuentes fechadas necesita saber **hasta cuándo vale cada fuente**, no
solo de cuándo es.

**Decisión 8 — el campo que falta en cada fuente: la vigencia.**
La ficha de fuentes necesita cinco columnas, no cuatro: documento · quién decide ·
fecha de la versión subida · **hasta cuándo vale** · cada cuánto se revisa. Sin la
cuarta, dentro de seis meses tendrás respuestas guardadas y no sabrás con qué
versión se produjeron, y no podrás reconstruir qué le dijiste a quién. Es el mismo
principio que la fecha en la hoja de anclas: **un resultado sin la fecha de su
criterio no es comparable con nada.**

## Anatomía de los errores típicos

### Fallo 1 · «El citador decorativo»
- **Cómo se reconoce:** hay corchetes en frases sin datos («encantada de saludarte
  [Tarifario]») y no los hay en la frase del precio.
- **Por qué pasa:** le pediste que citara, no le dijiste **qué** hay que citar. Para
  el sistema, citar es un estilo.
- **Arreglo mínimo:** «cita **solo** las frases que contengan un precio, una fecha,
  un plazo o una condición», más un ejemplo literal de frase citada y otro de frase
  sin citar.

### Fallo 2 · «El que nunca dice que no» ← el más importante
- **Cómo se reconoce:** los dos casos de rechazo de tu batería producen respuestas
  plausibles y generales, con «normalmente», «suele ser» o «en general».
- **Por qué pasa:** la instrucción de abstención estaba al final, redactada como una
  sugerencia, y compitiendo contra toda la presión del texto por ser útil.
- **Arreglo mínimo:** subirla arriba, hacerla literal, y **prohibir expresamente los
  atenuantes**: nada de «normalmente», «suele», «aproximadamente», «en torno a».
  Esos adverbios son la firma de la invención.
- **Y la comprobación que no se salta:** si tu asistente nunca dice «no lo sé», no
  es que lo sepa todo: **es que no lo has probado bien.**

### Fallo 3 · «La fuente sin dueño»
- **Cómo se reconoce:** en tu ficha de fuentes hay una fila cuya columna «quién
  decide lo que pone» dice «no sé» o «lo hicimos entre varias».
- **Por qué pasa:** como tú sabes cuál es el bueno, no te parecía un problema. Para
  un sistema lo es, y para tu compañera de agosto también.
- **Arreglo mínimo:** esa fila no entra como fuente. Y esa tarea, en tu Mapa, baja a
  **veredicto 2**. Descubrirlo aquí es un acierto del ejercicio, no un retroceso.

### Fallo 4 · «El maestro subido»
- **Cómo se reconoce:** la fuente es el fichero que usa todo el mundo, no una copia.
- **Por qué pasa:** es un clic menos y parece más «actualizado».
- **Arreglo mínimo:** copia limpia siempre. Un fichero de hoja de cálculo va
  **entero**: todas las filas, incluidas las 900 que no estás mirando; todas las
  columnas, incluidas las ocultas; **todas las pestañas**, incluida la que se llama
  «datos antiguos».

### Fallo 5 · «El bilingüe que no lo es»
- **Cómo se reconoce:** contesta en español a quien escribió en inglés, o traduce
  bien la respuesta y deja el nombre del curso y las condiciones en español a
  medias.
- **Por qué pasa:** tus fuentes están en español y la instrucción de idioma competía
  con ellas.
- **Arreglo mínimo:** decir explícitamente que las fuentes están en español y que la
  respuesta va en el idioma de la persona; y añadir un caso límite a la batería con
  un correo en un idioma minoritario de tu mezcla real —neerlandés, turco, coreano—,
  no en inglés, que es el fácil.

### Fallo 6 · «La batería fácil»
- **Cómo se reconoce:** diez de diez a la primera, y euforia.
- **Por qué pasa:** los casos salieron de tu memoria, y tu memoria guarda los que
  sabes contestar.
- **Arreglo mínimo:** coger diez por orden cronológico estricto del buzón y volver a
  mirar. **Si tu batería la pasa entera a la primera, tu batería es fácil; no es que
  tu sistema sea bueno.**

## Lo que también sería correcto

- **Poner las fuentes en un cuaderno separado** y que el asistente lo consulte, en
  lugar de adjuntarlas dentro del asistente. Es más trabajo hoy y más cómodo dentro
  de tres meses, cuando haya que actualizar el tarifario en un solo sitio.
- **Una frase de abstención distinta de la del ejemplo**, siempre que sea literal,
  única y buscable. El criterio es que se pueda contar, no cómo suena.
- **Tres fuentes en vez de seis.** Menos fuentes bien fechadas es mejor que más
  fuentes de procedencia dudosa. El número no es el objetivo.

## Lo que parece correcto y no lo es

- **Añadir «si no estás seguro, indícalo».** Suena prudente y no funciona: «seguro»
  no es un estado que el sistema pueda consultar, y lo que produce es una capa de
  matices verbales sobre respuestas igual de inventadas. Lo que funciona es
  condicionar la abstención a **un hecho comprobable**: si el dato no está en las
  fuentes, esta frase; si el periodo no está cubierto, esta otra.
- **Pedirle que puntúe su propia confianza del 1 al 10.** Devuelve un número con
  una validez aparente altísima —queda precioso— y sin ninguna ancla detrás: el 7 de
  una respuesta no es comparable con el 7 de otra. Si quieres una señal de confianza,
  que salga de **cuántas fuentes independientes concuerdan**, no del modelo.
- **Meter las condiciones de cancelación como fuente «por si acaso».** Cada fuente
  que añades es una superficie más que mantener y una respuesta más que puede
  caducar sin avisar. Las cancelaciones tienen consecuencia económica y en tu Mapa
  están cerca de la zona prohibida: si entran, entran con su propia regla de
  derivación.
```

---

## 12.6 Qué demuestra esta lección sobre la textura del material

Cuatro cosas, y son las que hay que auditar en cada lección que se escriba:

1. **La mitad de criterio no nombra un solo producto y sigue siendo accionable.** Se puede ejecutar en
   cualquier herramienta que permita guardar instrucciones y adjuntar documentos, que es todo lo que hay
   hoy y previsiblemente todo lo que habrá.
2. **El fichero de clics ocupa una quinta parte y es sustituible en veinte minutos.** Contiene además una
   caja de «trampas conocidas hoy» que es la parte que más envejece y la que más ayuda mientras dure.
3. **La corrección no necesita a nadie en ningún punto.** Umbral binario sobre una batería con clave que
   ella misma escribió antes; once ítems observables; seis señales de fallo con salida escrita
   obligatoria. El único mecanismo con juicio —la IA correctora— va en el bloque 3, el último, y con
   protocolo.
4. **La solución comentada enseña lo que la solución modelo no puede:** «lo que también sería correcto»
   impide leer *distinto* como *mal*, y «lo que parece correcto y no lo es» ataca los tres errores que
   una persona con criterio metodológico va a cometer precisamente por tenerlo —querer un índice de
   confianza, querer más fuentes, querer que el sistema module su seguridad—.

---

# 13. PRUEBA DE DURABILIDAD

**Procedimiento.** Recorrer el mapa de módulos suponiendo que en agosto de 2028 (a) los productos se han
renombrado al menos una vez —cosa que ya pasó tres veces en cinco meses de 2026: la automatización nativa
de la suite, el cuaderno de fuentes y la herramienta de terminal, las tres cambiaron de nombre—, (b)
algunas funciones se han movido de edición, (c) su empresa ha cambiado de proveedor o ella ha cambiado de
empresa. Y marcar, módulo a módulo, qué se rompe.

## 13.1 Recorrido, módulo a módulo

| Módulo | Qué es criterio (sigue válido en 2028) | Qué es clic (se rompe) | Coste de reparación |
|---|---|---|---|
| **M0** | Las cuatro preguntas que definen un plan · «la misma frase es segura o no según con qué cuenta entres» · «pagar resuelve quién es el proveedor, no qué tratamientos están amparados» · el semáforo · el estándar «no lo sé y lo pregunté» vale, «creo que sí» no · el Pase A y el Pase B · la lista de 32 procesos | El distintivo concreto de la pantalla · las cinco comprobaciones empíricas · la ruta de la consola · los cuatro mensajes literales | **1 fichero de clics.** El criterio no se toca |
| **M1** | Los seis veredictos · las pruebas que los deciden · la regla del cuatro · la zona prohibida y sus seis procesos · la cola de ataque | **Nada.** Este módulo no tiene fichero de clics | **Cero** |
| **M2** | Ficha de criterio · anclas de tono · muestra apartada · batería con tabla de especificaciones · fuente de verdad con fecha y con dueño · cita · regla de abstención · el techo de la memoria | Dónde se guarda un asistente, cuántos ficheros admite, cómo se llama la superficie de fuentes | **1 fichero de clics + 1 línea de `tres-nombres.md`** |
| **M3** | El libro de códigos entero · categorías exhaustivas y excluyentes · unidad de análisis · fase inductiva y deductiva · saturación · doble codificación y tabla de confusión · umbral por los dos lados · el techo del disparador por horario | Cómo se escribe una clasificación en lote en su hoja de cálculo · dónde se crea una tarea recurrente | **1 fichero de clics.** Y si esa función desaparece, la ruta alternativa (lotes desde el asistente) ya está escrita |
| **M4** | Anatomía de un flujo: disparador, pasos, condiciones, tope · «etiquetar es reversible, enviar no» · la prueba del caso que NO debe disparar · «comprueba antes sobre qué ficheros puede actuar tu herramienta» | Los límites concretos de su plataforma (recursos compartidos, un disparador por flujo, tope de etiquetas) · el catálogo de pasos disponibles | **1 fichero de clics + la lista de seis comprobaciones**, que hay que reescribir con los límites de la plataforma nueva. **Es la reparación más cara del curso** |
| **M5** | Composición: un artefacto se convierte en pieza de otro · «automatiza donde ya viven tus datos» · «la que reutiliza lo que tienes gana a la más potente» · ítems ancla y deriva · variación de forma frente a variación de calidad | Los nombres de los pasos que llaman al asistente y al cuaderno | **1 fichero de clics** |
| **M6** | Agente = objetivo y límites, pasos decididos sobre la marcha · «un agente puede ser exceso» · temas prohibidos · condiciones de parada · topes · plan de fallo · prueba de apagado · privilegio mínimo | Qué producto concreto está detrás de qué plan · qué pasos de juicio ofrece hoy la plataforma | **1 fichero de clics + la caja del fondo**, que se revisa entera. Está diseñada para eso: su tercera columna son condiciones, no productos |
| **M7** | Línea base · minutos por unidad · coste completo · las seis amenazas a la validez interna · proceso frente a resultado · cadena causal · prueba ciega | **Nada.** Es metodología y una hoja de cálculo | **Cero** |
| **M8** | El número y su método · qué NO hace · demo de tres minutos · prueba del pasillo · piloto con otra persona · ficha de traspaso · las cuatro reglas de arranque | **Nada** | **Cero** |
| **M9** | Escribir la propia rúbrica y validarla contra un cebo · calendario de revisión · condiciones de activación del escalón 4 | Los nombres de las herramientas del apéndice opcional | **1 párrafo** |

## 13.2 Recuento

| | Módulos | Proporción |
|---|---|---|
| **Sin nada que reparar** (M1, M7, M8) | 3 | 33 % |
| **Reparación de un fichero de clics** (M0, M2, M3, M5, M6, M9) | 6 | 60 % |
| **Reparación cara** (M4: clics + lista de comprobación de plataforma) | 1 | 11 % |
| **Módulos que habría que rediseñar** | **0** | **0 %** |

Y por instrumento: el **Semanario** no caduca (una academia de idiomas en 2030 seguirá emitiendo cartas
de visado y contestando leads); el **Cuaderno de capacidades** caduca **en nueve líneas** —el campo 6 de
cada ficha— por diseño; el **Cuaderno de evidencias** no caduca; la **batería** y la **hoja de anclas** no
caducan; la **tabla de tres nombres** caduca **entera**, y por eso está aislada en una sola página fechada.

**Veredicto: no hay que rediseñar.** Lo que sí ha habido que cambiar respecto al borrador anterior, y está
ya aplicado en este documento, es lo siguiente.

## 13.3 Cinco rediseños que esta prueba obligó a hacer, y que ya están incorporados

1. **Los títulos de los módulos ya no nombran productos.** El borrador tenía módulos que se llamaban por
   la herramienta. Con eso, el 60 % del índice del curso nacía caducado y —peor— **el índice enseñaba lo
   contrario que el contenido**. Ahora se titulan por capacidad.
2. **La clasificación en lote dejó de ser la pieza central de M3 y pasó a ser una implementación.** En el
   borrador, la función de hoja de cálculo era el artefacto del módulo, con lo cual el módulo entero
   dependía de que su plan la incluyera y de que la función siguiera existiendo. Ahora el artefacto del
   módulo es **el libro de códigos**, que se puede aplicar de tres maneras distintas, y el ejercicio
   obliga a nombrar dos. La contingencia dejó de ser un parche y pasó a ser contenido.
3. **La caja del fondo cambió de eje.** Antes listaba productos con una columna de «cuándo te tocaría».
   Ahora la fila **es la condición** y el producto es el ejemplo de hoy. Con el eje anterior, la tabla
   había que rehacerla entera cada año; con este, se revisa.
4. **Apareció la ficha de capacidad, y con ella el campo del techo.** Es la pieza que convierte el curso
   en un objeto portátil de nueve caras. El borrador no tenía ningún artefacto que sobreviviera al cambio
   de herramienta; ahora el artefacto principal del curso **es** ese.
5. **Las pruebas de portabilidad pasaron de no existir a ser entregables con rúbrica.** Sin ellas, la
   agnosticidad era una declaración en la introducción — es decir, exactamente lo que hace la referencia,
   que se declara agnóstica y luego demuestra todo con una sola herramienta. Con ellas, es un desempeño
   observable (RA8).

## 13.4 Lo que sigue siendo frágil aunque el diseño esté bien

Honestidad obligatoria, porque una prueba de durabilidad que sale limpia del todo es sospechosa:

- **M4 es el punto débil y no tiene arreglo estructural.** La anatomía de un flujo es durable, pero **los
  límites concretos de una plataforma no son un adorno del módulo: son la mitad del módulo**, porque son
  lo que determina si su buzón compartido se puede tocar o no. Si cambia la plataforma, hay que volver a
  averiguar los límites, y eso no se hereda.
- **La lista de 32 procesos envejece despacio pero envejece.** Si el sector cambia —una normativa de
  extranjería nueva, un canal de captación que desaparece— hay filas que dejan de existir. Sigue siendo
  el activo más duradero del curso, pero conviene fecharla como cualquier otra fuente.
- **Y una asimetría incómoda:** lo que menos caduca es lo que menos se parece a «un curso de IA»
  —inventariar, escribir criterios, medir, traspasar— y lo que más caduca es lo que más se parece.
  Es la mejor prueba de que el listón está bien puesto, y también el motivo por el que el material tiene
  que trabajarse el enganche de M1, M7 y M8 mucho más que el de M4.

---

# 14. AUTOCRÍTICA

Ordenada de más grave a menos. Sin esta sección, las trece anteriores no son creíbles.

**1 · El módulo de evangelización es el menos autocorregible del curso, y lo es por naturaleza.**
Su criterio de éxito es la conducta de otras personas. Puedo hacer binario el piloto —lo usó o no lo
usó—, puedo hacer mecánica la reproducción del número y la prueba del pasillo, y lo he hecho. Pero **no
puedo darle una rúbrica a «la organización lo adoptó»**, y esa es la palabra que usa el brief. Si su
compañera no usa el artefacto, hay al menos cuatro explicaciones —el artefacto es malo, la compañera está
desbordada, la tarea no era suya, no hubo tiempo— y el material no le da forma de distinguirlas. Es el
único módulo del curso donde una alumna diligente puede hacerlo todo bien y salir sin saber si lo hizo
bien.

**2 · La agnosticidad tiene un coste que he minimizado, no eliminado.**
Redactar en capacidades es más abstracto, y la abstracción es exactamente lo que peor le sienta a alguien
sin base técnica en las primeras semanas. He compensado con los ficheros de clics, que son concretísimos,
pero el riesgo real es una lección que se lee «bonita» y no se sabe ejecutar hasta abrir el segundo
fichero. La prueba de si esto funciona no está en el diseño: está en si la primera semana produce el
asistente. **Si el material resultara demasiado abstracto, la reparación correcta no es volver a mezclar:
es engordar los ficheros de clics y adelgazar el criterio.**

**3 · Diecinueve semanas, y los dos objetivos que ella formuló como 4 y 5 están al final.**
El criterio portátil se consolida en M7 y la evangelización es M8. Es la colocación correcta por
dependencia —no se evangeliza lo que no está medido— y es la peor por riesgo de abandono. He puesto seis
contramedidas (§11, momento 3) y la más importante es declarar la frontera de M6 en la semana 1. Aun así,
**he colocado la mitad del valor del curso en el tramo que menos gente termina**, y esa es una decisión
discutible que conviene que quede escrita. La alternativa —adelantar la evangelización— rompe la
dependencia y produce dossieres con números inventados, que es peor.

**4 · El inventario está sesgado hacia lo que deja rastro escrito.**
Los correos y WhatsApp se cosechan bien; las llamadas, el mostrador y el pasillo, mal. Y resulta que la
parte más cara y más humana de su puesto —el lunes de check-in con sesenta alumnos de nivel A0 en la
misma sala, la llamada de emergencia de un domingo— es justo la que peor se captura **y** la que menos se
automatiza. Consecuencia: **el Mapa va a parecer más automatizable de lo que es su semana real.** El Pase
B lo corrige a medias, y la señal de fallo nº 5 de la rúbrica de M1 lo busca explícitamente, pero no lo
resuelve.

**5 · Cinco días de palotes en octubre no son su año.**
El volumen se multiplica por tres entre febrero y julio. La columna `V` es un parche de una tecla, y sé
que es un parche. Un inventario de temporada baja miente sobre julio en frecuencias, en mezcla de tareas
y —sobre todo— en **tiempo disponible**, que es la variable que decide si un artefacto se usa o se
abandona.

**6 · La regla del cuatro es una cuota, y las cuotas producen cumplimiento de cuota.**
No hay evidencia de que cuatro sea el número: sale de cruzar los 32 procesos con lo que la plataforma
puede hacer, y eso da entre cinco y siete, así que cuatro es un suelo prudente. Pero puede fabricar noes
de conveniencia. La señal de fallo nº 3 de la rúbrica de M1 —*«existe un veredicto 1 o 2 que puse para
llegar a cuatro, no porque lo crea»*— lo busca de frente, y aun así **depende de su honestidad en el peor
sitio posible: consigo misma, sin nadie que compruebe.**

**7 · La arquitectura compite consigo misma en la primera semana.**
«El inventario manda» y «victoria temprana» tiran en direcciones opuestas: la victoria del día 1 se
construye **antes** de tener el Mapa, y por tanto sin el criterio que el Mapa da. El asistente de M0
podría resultar, en la semana 4, ser una tarea que merecía veredicto 2. Lo he convertido en material —*«el
primer artefacto del curso puede ser el primero que revises con criterio»*— y es un parche elegante, pero
sigue siendo un parche: **he sacrificado coherencia por supervivencia, a sabiendas.** Creo que es la
decisión correcta y es una incoherencia real.

**8 · Todo el arranque descansa en que el asistente del día 1 salga medianamente bien.**
Y lo más probable es que descubra que sus documentos están desordenados o desactualizados: es literalmente
el proceso P32 y su «riesgo alto y silencioso». La contención entera es una caja de texto que lo predice y
lo renombra como primer hallazgo. Si esa caja no funciona, **la primera experiencia del curso es un
fracaso y no hay red debajo.** Es el supuesto más frágil del diseño.

**9 · Las pruebas de portabilidad nunca tocan la parte difícil.**
La nº 1 se hace con material verde, porque no puede ser de otro modo: por su cuenta personal no puede
pasar un dato de un alumno. La nº 2 y la nº 3 son sobre papel. Es decir: **demuestro que el criterio viaja,
no demuestro que ella sabría trabajar de verdad en otra herramienta con datos reales.** Es honesto y es
suficiente para el objetivo declarado —saltar sin fricción, no ser experta en dos entornos— pero la prueba
es más débil de lo que su nombre sugiere, y hay que llamarla por lo que es: una prueba de portabilidad
**del criterio**, no de la competencia.

**10 · Depende de un dato que no tenemos.**
Si su empresa está en el plan básico, media docena de funciones no existen para ella y M3 pierde su
implementación más cómoda. He escrito las rutas alternativas y he puesto la regla estructural de que
**ningún módulo dependa de una sola función**, pero un curso con vía degradada en varios módulos es un
curso más flojo, y no sabremos cuál tenemos hasta la semana 2, con el curso ya escrito.

**11 · La corrección con IA es el eslabón blando de todo el andamiaje.**
Hay rúbricas, baterías con clave sellada y listas binarias, que es lo mejor que se puede hacer sin
profesor. Pero parte del feedback lo va a dar un modelo que se pliega a la opinión del usuario, que
prefiere lo verboso y que favorece el texto que él mismo generó. Tenemos tres controles positivos (los
cebos de M1, M2 y M6) y **no existen datos publicados sobre cómo se comporta un modelo de 2026 corrigiendo
un entregable contra una rúbrica dada** — que es exactamente nuestro caso. El cebo no es un adorno: es lo
único que tenemos, y puede resultar que la respuesta sea «para este tipo de trabajo, la IA no corrige».

**12 · Nadie va a decirle que el Mapa está mal.**
PC-2 lo mitiga con diez minutos de alguien que sabe de IA pero **no conoce la academia** — y el Mapa
depende precisamente del conocimiento de la academia. El punto de mayor apalancamiento del curso está
apoyado en alguien que puede auditar el razonamiento pero no los hechos. En última instancia el Mapa
descansa en su juicio sobre su propio trabajo, que es exactamente el punto ciego que la literatura sobre
autoevaluación describe.

**13 · Y una duda de fondo sobre el ángulo entero.**
Esta arquitectura asume que ella quiere un mapa. Puede que lo que quiera sea que le arreglen el martes. El
perfil dice que «prefiere lo útil y eficaz a lo bonito», y hay una lectura de esa frase que también
condena a los inventarios: **un Semanario es un documento, y los documentos no contestan correos.** Toda
la defensa descansa en que las cuatro semanas de mapa se pagan con creces en las quince siguientes. Lo
creo —y por eso he puesto la victoria antes que el inventario, y he hecho que el inventario pague un
hallazgo a las 48 horas— pero es una apuesta, y si falla, falla al principio, que es donde peor duele.

---

# 15. DÓNDE ACABA LO INVESTIGADO Y DÓNDE EMPIEZA LO APOSTADO

**Procede de los informes de dominio ya producidos y no se ha vuelto a verificar en esta sesión:** los
procesos P01–P32 con sus volúmenes y riesgos (`dominio-academia.md`); el marco de datos, el semáforo, los
ejercicios E-01…E-06, los planes y el Anexo III (`dominio-rgpd.md`); los escalones, las capacidades reales
de la plataforma y sus límites verificados (`dominio-herramientas.md`); los mecanismos de corrección, los
puntos de caída, las plantillas y el protocolo de siete reglas (`dominio-autodidacta.md`); las
correspondencias EP-01…EP-14 y los nueve falsos amigos (`dominio-psicologia.md`); los cinco pasos, sus
citas y sus huecos (`01-analisis-referencia.md`, `fuente-*.md`).

**Son decisiones de diseño mías, sin respaldo externo, y quien evalúe este documento debe saberlo:**

- Los **seis veredictos** y la decisión de dejar el agente autónomo fuera de la lista.
- La **regla del cuatro** y su número.
- Los **dos pases** del Semanario y las once columnas.
- La **columna 8 como forma de integrar la protección de datos** en el criterio de selección.
- **El Cuaderno de capacidades y la ficha de seis campos**, incluido el aislamiento del campo perecedero.
- **Las tres pruebas de portabilidad** y su formato.
- **La separación física criterio/clics en dos ficheros** y las cuatro reglas de producción.
- **El diseño entero del módulo M8** y sus cinco mecanismos de autocorrección.
- La **colocación de los tres momentos de riesgo** y la exclusión argumentada del cuarto.
- El **calendario de 19 semanas** y la frontera declarada en M6.

**Y una restricción que hereda de las fuentes y conviene repetir:** el dato más importante de todo el
diseño —qué plan tiene contratada su empresa y cómo está configurado— **[NV]** no es verificable desde
fuera. Es la primera tarea del curso, no de esta investigación, y de su respuesta depende qué versión de
M3 y de M4 se ejecuta.
