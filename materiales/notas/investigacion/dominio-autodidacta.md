# Dominio — Cómo funciona un curso sin profesor (y con una pareja para consultas puntuales)

**Para qué sirve este documento.** El brief quita el profesor y deja un recurso muy concreto en su
lugar: una pareja con conocimientos de IA, disponible para consultas puntuales, que **no corrige
entregas ni sigue el progreso**. Eso no es un mentor con menos horas: es una categoría distinta de
recurso, y diseñar como si fuera un mentor barato garantiza que se gaste mal.

Este documento resuelve cuatro cosas y produce una quinta:

1. Qué mata a los cursos autodidactas y **cuándo** los mata (sección 1).
2. Qué mecanismos pedagógicos siguen funcionando sin nadie delante (sección 2).
3. **El problema central: cómo se autocorrige quien por definición no sabe si lo ha hecho bien**
   (sección 3). Es la sección larga y es el núcleo del encargo.
4. Cómo se gasta el recurso escaso de la pareja (sección 4).
5. Y produce las **plantillas** que hacen que todo lo anterior se pueda aplicar mecánicamente a cada
   módulo, sin volver a pensarlo (sección 8).

**Fecha:** 22.08.2026.

**Documentos hermanos que este da por leídos:** `00-perfil.md` (fuente de verdad),
`01-analisis-referencia.md`, `dominio-academia.md` (los 32 procesos del puesto),
`dominio-herramientas.md` (la escalera Gemini → Workspace Studio → juicio en el flujo).

---

## 0. Marcas de fiabilidad y una advertencia

| Marca | Significado |
|---|---|
| **[E]** | **Evidencia publicada.** Metaanálisis, ensayo o estudio citado con enlace en la sección 10. |
| **[D]** | **Derivado.** Consecuencia razonada de [E] aplicada a este caso concreto. No está en la fuente. |
| **[J]** | **Juicio de diseño.** Decisión mía, argumentada, sin respaldo empírico directo. |

**Advertencia sobre el traslado.** Casi toda la evidencia buena sobre abandono viene de MOOCs, y un
MOOC no es esto: allí hay miles de inscritos con coste de entrada cero y ninguna relación con quien
lo hizo. Aquí hay una persona, un curso hecho a medida para ella, y una pareja implicada. El
**coste psicológico de abandonar es mucho mayor**, así que las tasas no se trasladan. Lo que **sí**
se traslada, y es lo que uso, son los **mecanismos y la forma de la curva**: en qué semana se cae,
qué la precipita y qué se puede poner justo antes. [J]

Segunda advertencia: hay un factor de riesgo específico de este caso que no aparece en ninguna
literatura y que domina sobre todos los demás. **Su empresa tiene el pico de trabajo en junio–
septiembre** (`dominio-academia.md` §0.3: de 150 a 400 correos/día, de 40 a 100 llamadas/día). Un
curso que exija dos horas semanales en agosto no fracasa por diseño instruccional: fracasa por
calendario. La sección 5 lo trata como restricción de primer orden.

---

## 1. Por qué fracasan los cursos autodidactas

### 1.1 La magnitud, con números reales

- Jordan (2015) siguió **221 cursos** y encontró tasas de finalización de **0,7 % a 52,1 %**, con
  **mediana del 12,6 %**. [E]
- Reich y Ruipérez-Valiente (*Science*, 2019), sobre **cinco años de datos de MIT y Harvard en edX**:
  la finalización **no mejoró con el tiempo, empeoró** — del ~6 % en 2014-15 al **3,13 % en
  2017-18** — y **el 52 % de los inscritos nunca llega a empezar**. [E]

Ese segundo dato es el más importante de los dos y casi nunca se cita. **La mitad de la mortalidad
ocurre antes de la primera lección.** No es un problema de contenido: es un problema de fricción de
arranque y de coste de entrada. Traducción directa para este curso: la lección 1 no puede empezar
con una instalación, un registro, una consulta al administrador ni una teoría. Tiene que empezar con
algo que ella haga en veinte minutos y que le sirva ese mismo día. [D]

### 1.2 Cuándo se abandona

La forma de la curva es consistente en toda la literatura de MOOCs: **la caída es fuertísima al
principio y luego se aplana**. Los modelos de predicción de abandono alcanzan ~80 % de acierto
usando solo datos de la **semana 2**, y se identifican hasta el 60 % de los futuros abandonos con la
interacción de la **primera semana** (Chen et al.; Alamri et al., 2019). [E]

Eso significa que la información sobre si alguien va a terminar **ya está escrita en los primeros
siete días**, y que **el diseño de las dos primeras semanas vale más que el de las diez siguientes
juntas**. [D]

Después del arranque, el abandono no desaparece: se vuelve episódico. Se cae en momentos
identificables —un bloqueo técnico, una semana mala, un resultado decepcionante— no por desgaste
uniforme. Eso es una buena noticia de diseño: **si los momentos son identificables, se les puede
poner algo delante** (sección 6). [D]

### 1.3 Por qué se abandona

Eriksson, Adawi y Ståhr (2017) entrevistaron en profundidad a **34 aprendices** con distintos grados
de finalización y encontraron cuatro factores: percepción del contenido, percepción del diseño del
curso, situación social, y **capacidad de encontrar y gestionar el tiempo**. **21 de los 34**
mencionaron la falta de tiempo; el título del artículo es *"Time is the bottleneck"*. Trabajo,
familia y otros estudios compiten directamente. [E]

Pero conviene leer ese hallazgo con cuidado, porque "no tuve tiempo" es la explicación socialmente
aceptable de casi cualquier abandono. Lo que hay debajo, y que sí se puede diseñar, es que **el
curso perdió la competencia por un hueco de tiempo contra otra cosa**. Un curso pierde esa
competencia cuando su beneficio es lejano y difuso y el de la alternativa es inmediato y concreto.
La contramedida no es motivacional, es estructural: **que el trabajo del curso sea trabajo del
puesto**, de modo que no compita con la jornada sino que la sustituya. Ese es el argumento más
fuerte a favor del proyecto hilo (sección 7). [D]

### 1.4 Los dos mecanismos psicológicos que hacen esto peor sin profesor

Estos dos son los que de verdad explican por qué un autodidacta se estanca, y los dos son
directamente relevantes para el diseño del feedback.

**(a) La ilusión de fluidez: sentir que aprendes es un mal indicador de aprender.**
Deslauriers et al. (*PNAS*, 2019) asignaron aleatoriamente a estudiantes de física a clase pasiva o
a aprendizaje activo, con el mismo contenido y los mismos materiales. Los del aula activa
**aprendieron más y sintieron que aprendían menos**; la correlación entre aprendizaje real y
sensación de aprendizaje fue **negativa**. [E]

Consecuencia brutal para un autodidacta: **su termómetro está invertido**. El material que se lee
cómodo y deja sensación de dominio (un vídeo bien hecho, una lección clara) es el que menos enseña;
el ejercicio que la deja incómoda y con dudas es el que funciona. Sin profesor, no hay nadie que le
diga eso, así que **hay que decírselo por escrito y pronto**, y hay que enseñarle a no fiarse de la
sensación como criterio de avance. [D]

**(b) Los que peor lo hacen son los que peor lo estiman.**
León, Panadero y García-Martínez (2023) metaanalizaron **160 artículos, 29.352 participantes**, y
encontraron una **tendencia general a la sobreestimación** en la autoevaluación. Y —esto es lo
accionable— la sobreestimación **se reduce con feedback, con experiencia previa en autoevaluarse,
con conocimiento del contenido y con criterios explícitos**. [E]

Es decir: la autoevaluación no es una capacidad fija, **es una destreza que se entrena y que
responde a los andamios**. Un curso sin profesor no puede limitarse a "autoevalúate": tiene que
enseñar a autoevaluarse, dar los criterios, y calibrarlos contra algo externo. Toda la sección 3 es
el desarrollo de esta frase.

### 1.5 Y un tercero, específico de este curso: la muleta

Bastani et al. (*PNAS*, 2025) hicieron el experimento que más importa aquí, con ~1.000 alumnos de
secundaria en Turquía. Con acceso a GPT-4 durante la práctica, el rendimiento **en la práctica**
subió mucho (+48 % con la interfaz tipo ChatGPT). Cuando se les retiró el acceso y se les examinó
solos, **rindieron un 17 % peor que quienes nunca lo habían tenido**. La versión con salvaguardas
—un tutor configurado para dar pistas diseñadas por el profesor en vez de la respuesta— **eliminó el
daño**. [E]

Aplicado a este curso: la alumna va a tener a la IA delante todo el rato, porque la IA *es* el
temario. **El riesgo de que la IA haga el ejercicio en lugar de enseñarlo es estructural, no
anecdótico.** Y la solución conocida también: no prohibir la herramienta, sino **configurar cómo
interviene** — pistas y no respuestas, criterios y no veredictos. Eso es exactamente lo que hacen
las plantillas de la sección 8.

---

## 2. Mecanismos que funcionan sin profesor

Criterio de selección: solo entra lo que (i) tiene respaldo empírico razonable, (ii) **no requiere
que nadie lea el trabajo de la alumna**, y (iii) se puede meter en una plantilla y aplicar
mecánicamente a cada módulo.

### 2.1 Tabla de mecanismos

| Mecanismo | Evidencia | Qué resuelve sin profesor | Cómo se instancia aquí |
|---|---|---|---|
| **Práctica recuperativa** | Adesope et al. (2017): *g* ≈ 0,61 sobre >200 comparaciones; efecto igual en aula que en laboratorio [E] | Sustituye el examen del profesor por autocomprobación honesta | 5 preguntas de recuerdo al inicio de cada sesión núcleo, **de memoria y por escrito, antes de abrir nada** |
| **Práctica espaciada** | Dunlosky et al. (2013) la clasifican junto a la práctica de recuperación como una de las **dos únicas técnicas de utilidad alta** de diez evaluadas [E] | Combate el olvido sin necesidad de repasos programados por otro | Las 5 preguntas mezclan módulo actual, anterior y uno de hace tres semanas |
| **Ejemplos trabajados con desvanecimiento** | Renkl y Atkinson: el desvanecimiento *hacia atrás* mejora transferencia cercana y reduce tiempo; combinado con autoexplicación mejora también la lejana [E] | Sustituye al profesor que hace uno delante y luego te deja hacer | Módulo *n*: ejemplo completo → ejemplo con los 2 últimos pasos en blanco → solo el enunciado |
| **Autoexplicación** | Bisra et al. (2018), metaanálisis de 64 estudios: *g* = 0,55 [E] | Sustituye la pregunta socrática del profesor | Campo obligatorio "por qué he hecho esto así" en cada entregable, **escrito antes de corregir** |
| **Rúbricas** | Panadero y Jonsson (2013): mejoran autorregulación y autoeficacia y reducen ansiedad; León et al. (2023): los **criterios explícitos** reducen la sobreestimación [E] | Sustituye el criterio del profesor por criterio escrito | Una rúbrica por entregable, con criterios **negativos** (sección 3.5) |
| **Listas de comprobación** | Derivado de la literatura de checklists de seguridad y de la evidencia sobre criterios explícitos [D] | Detecta **omisiones**, que es lo que la autoevaluación no ve nunca | 8–12 ítems binarios *observables*, no valorativos |
| **Criterios de éxito explícitos** | Kluger y DeNisi (1996): el feedback mejora en media (*d* = 0,41) pero **en más de un tercio de los casos empeora el rendimiento**, sobre todo cuando apunta a la persona y no a la tarea [E] | Impide que el feedback (incluido el de la IA) se convierta en juicio sobre ella | Cada ejercicio declara arriba **cómo se verá que ha salido bien**, en términos observables |
| **Proyecto hilo** | Mecanismo motivacional y de transferencia; sin metaanálisis limpio, pero es la contramedida directa al hallazgo de Eriksson (§1.3) [D/J] | Da continuidad y hace que el tiempo del curso sea tiempo de trabajo | Doble hilo: uno guiado con clave, uno suyo (sección 7) |
| **Intenciones de implementación** | Gollwitzer y Sheeran (2006): *d* = 0,65 sobre 94 pruebas independientes [E]; en MOOCs, los *planning prompts* aumentaron finalización, mientras que los consejos genéricos de autorregulación **no hicieron nada** [E] | Sustituye al calendario que impone la cohorte | "Si es martes y son las 9:15, abro el módulo" — **fecha, hora y sitio escritos**, no "esta semana" |

### 2.2 Lo que hay que quitar aunque apetezca ponerlo

Dunlosky et al. (2013) clasifican como **utilidad baja**: releer, subrayar, resumir, usar
mnemotécnicas de palabra clave e imágenes mentales. [E] Son exactamente las técnicas que un curso
autodidacta genera por defecto, porque son las que producen sensación de progreso (§1.4a).

Traducción a decisiones concretas de este curso: [D]

- **Nada de vídeos de lección.** Un vídeo es relectura con mejor producción. Si hay vídeo, es de
  *demostración* de una interfaz, dura menos de tres minutos y va acompañado de la transcripción
  escrita, porque la ruta de menús caduca (`dominio-herramientas.md` §8).
- **Nada de resúmenes de la lección al final.** El resumen lo escribe ella y es un entregable.
- **Ningún módulo puede terminar en lectura.** Termina en un artefacto que existe fuera del curso.
- **La regla 20/80**: como mucho el 20 % del tiempo de una sesión es leer.

### 2.3 El mecanismo transversal: el registro

Un autodidacta sin registro no tiene memoria de su propio proceso, y por tanto no puede calibrarse.
Un fichero único, `bitacora.md`, con una línea por sesión: fecha, minutos, qué he hecho, qué he
producido, **qué ha fallado**, y la nota de autoevaluación. [J]

Sirve para tres cosas a la vez: es la base de la práctica espaciada (de ahí salen las preguntas de
repaso), es la evidencia contra la ilusión de fluidez (a las seis semanas puede leer lo que le
parecía imposible en la semana 2), y es lo que hace que un punto de consulta de diez minutos rinda,
porque llega con el historial escrito.

---

## 3. El problema del feedback

Este es el núcleo. Todo lo demás de un curso autodidacta es logística; esto es lo que decide si
aprende algo o si consolida errores durante tres meses.

### 3.1 El enunciado exacto del problema

No es "no tiene quien la corrija". Es más profundo y más incómodo:

> Para saber si su trabajo está bien necesita el criterio que el trabajo debía enseñarle. En el
> momento en que puede evaluarse con fiabilidad, ya no necesita el módulo.

De ahí salen las tres estrategias legítimas, y **no hay una cuarta**: [J]

- **(A) Traer el criterio de fuera y ponerlo por escrito antes** — rúbricas, listas, soluciones
  comentadas, criterios de éxito. El criterio no lo genera ella: lo aplica.
- **(B) Sustituir el juicio por una comprobación** — casos con respuesta conocida, ejecución real.
  No hay que evaluar nada: se mira si sale o no sale.
- **(C) Externalizar el juicio a un tercero** — la IA o la pareja. Con la advertencia de que la IA
  es un tercero **poco fiable de una forma sistemática y predecible** (§3.5).

Todo lo que sigue es la ordenación de esas tres.

### 3.2 Ordenación de mecanismos por eficacia real

"Eficacia real" = probabilidad de que el mecanismo **detecte un defecto que existe** × probabilidad
de que ella **actúe sobre lo detectado**, penalizada por lo que cuesta producirlo o consumirlo. Un
mecanismo perfecto que no se usa vale cero.

| # | Mecanismo | Fiabilidad | Cobertura | Coste | Veredicto |
|---|---|---|---|---|---|
| **1** | **Ejecución real: el artefacto funciona o no funciona** | Máxima | Estrecha | Nulo | El suelo de todo. Solo dice si *funciona*, no si está *bien hecho* |
| **2** | **Batería de casos con respuesta conocida (clave sellada)** | Muy alta | Media | Alto de producción, nulo de uso | **El caballo de batalla del curso** |
| **3** | **Lista de comprobación binaria observable** | Alta | Estrecha pero precisa | Bajo | Lo único que caza **omisiones** |
| **4** | **Solución comentada con anatomía del error** | Alta | Amplia | Alto de producción | Convierte "el mío es distinto" en "el mío tiene el fallo nº 3" |
| **5** | **Rúbrica con criterios negativos + autoevaluación diferida** | Media-alta | Amplia | Medio | Necesita el diferido y el encuadre en tercera persona para funcionar |
| **6** | **IA correctora con rúbrica anclada y protocolo adversarial** | **Media, y variable de forma no aleatoria** | Muy amplia | Bajísimo | Potente y peligroso. Sección 3.5 entera |
| **7** | **Contraste de dos modelos distintos** | Media | Amplia | Bajo | Solo para *detectar* desacuerdo, no para dirimirlo |
| **8** | **Punto de consulta con la pareja** | La más alta de todas | Estrechísima por escasez | Altísimo (6 usos en todo el curso) | No es un mecanismo: es una reserva estratégica (sección 4) |
| **9** | **Autoevaluación libre ("¿me ha quedado bien?")** | ≈ nula | — | Nulo | **Prohibida como mecanismo.** Es el sesgo de §1.4b sin andamio |

Las tres lecturas que importan de esa tabla: [J]

1. **Los tres primeros puestos no requieren juicio de nadie.** La primera decisión de diseño de cada
   módulo no es "qué rúbrica pongo", es **"¿puedo convertir esta evaluación en una comprobación?"**.
   Muchísimas veces se puede, y casi nunca se intenta.
2. **La IA correctora está en el puesto 6, no en el 1.** Es la tentación obvia de un curso de IA sin
   profesor y es la que hay que domar. Es valiosa por cobertura y por inmediatez, no por fiabilidad.
3. **El mecanismo 9 es el que aparece solo si no se pone nada más.** Un curso autodidacta sin
   instrumentos de corrección no es un curso con autoevaluación: es un curso con confirmación de
   sesgo.

### 3.3 Los mecanismos 1–4, que son los que hay que producir

**Mecanismo 1 — El oráculo del mundo.** El mejor corrector disponible y es gratis: la realidad. En
este curso concreto es inusualmente accesible, porque casi todos los artefactos son ejecutables. El
flujo se dispara o no. El Gem responde o alucina. La columna `=AI()` clasifica las 40 filas o
devuelve error en la 12. **Diseñar cada entregable para que tenga un estado observable de
"funciona/no funciona"** es la decisión de diseño más rentable del curso. [J]

Su límite hay que decirlo en voz alta: **funcionar no es estar bien**. Un flujo que se ejecuta
perfectamente y manda un correo con un dato equivocado funciona. Por eso hace falta el 2.

**Mecanismo 2 — La batería de casos con respuesta conocida.** Es el traslado directo del paso 5 del
programa de referencia (`01-analisis-referencia.md` §2), y es el mecanismo que mejor encaja con
*esta* alumna, porque es psicometría con otro nombre: definir el criterio antes de medir, y medir
contra un patrón.

Formato fijo, **10 casos por artefacto**:

- **5 casos normales** — debe acertar los 5. Menos de 5 = no está listo.
- **3 casos límite** — ambiguos a propósito. Aquí no se mide acierto: se mide si **pide aclaración o
  se inventa una decisión**. Inventar es un fallo aunque acierte.
- **2 casos que debe rechazar** — le falta el dato, o la pregunta está fuera de alcance. La respuesta
  correcta es **"no lo sé"** o "esto no lo puedo responder con lo que tengo". Cualquier otra cosa es
  un suspenso, por bien redactada que esté.

Dos reglas que hacen que esto funcione de verdad: [J]

- **Los casos se escriben ANTES de construir el artefacto.** Si se escriben después, se escriben
  para que pasen. Esto es preregistro, y ella lo entiende a la primera si se le nombra así.
- **La clave va sellada.** En el hilo guiado, la respuesta correcta la trae el curso en un fichero
  aparte que ella abre **después** de anotar sus resultados. En el hilo propio, la clave la escribe
  ella el día que diseña los casos, y no la revisa el día que evalúa.

**Mecanismo 3 — La lista de comprobación binaria.** Cada ítem se responde mirando, no juzgando. La
prueba de que un ítem está bien escrito: **dos personas distintas darían la misma respuesta sin
discutir**.

- Mal: "¿el prompt está bien estructurado?" · "¿el flujo es robusto?"
- Bien: "¿hay una frase que diga qué hacer cuando falta un dato? SÍ/NO" · "¿hay algún paso que envíe
  algo a un cliente sin que yo lo apruebe? SÍ/NO" · "¿cada fuente del cuaderno tiene fecha? SÍ/NO"

Sirve para lo que ningún otro mecanismo detecta: **lo que no está**. La autoevaluación revisa lo que
hay delante; no echa de menos lo que nunca se escribió.

**Mecanismo 4 — La solución comentada con anatomía del error.** Una solución modelo sola es poco
útil: lo normal es que la suya sea distinta y no sepa si es distinta-válida o distinta-mala. Lo que
convierte la solución en instrumento de corrección es el **catálogo de fallos típicos con su
firma**: cómo se ve el fallo desde fuera.

Formato: por cada fallo, `nombre corto` · `cómo se reconoce en tu propio trabajo` · `por qué pasa` ·
`arreglo mínimo`. Cinco o seis fallos por módulo, sacados de los errores previsibles del dominio.
Con eso, la pregunta pasa de "¿está bien?" (irresolvible) a "¿tengo el fallo 1? ¿el 2? ¿el 3?"
(resoluble). [J]

### 3.4 Mecanismo 5 — La rúbrica, y los dos trucos que la hacen funcionar sola

Panadero y Jonsson (2013) documentan que las rúbricas mejoran autorregulación y autoeficacia, y León
et al. (2023) que los criterios explícitos reducen la sobreestimación. [E] Pero eso se midió en
contextos con profesor. Sin profesor, una rúbrica normal se autoconcede el aprobado. Dos
modificaciones lo corrigen: [J]

**Truco 1 — Criterios negativos.** Una rúbrica redactada en positivo ("el trabajo demuestra
comprensión de…") es una invitación a buscar evidencia confirmatoria, y quien busca confirmación la
encuentra siempre. Redactada como **síntomas de que está mal**, obliga a falsar.

| Redacción habitual | Redacción de este curso |
|---|---|
| "Las instrucciones del Gem son claras y completas." | "**Señal de fallo:** hay al menos una pregunta razonable de mi trabajo real que el Gem contestaría de dos formas distintas según el día. Escríbela." |
| "El flujo tiene un buen tratamiento de errores." | "**Señal de fallo:** existe un caso en el que el flujo sigue adelante sin el dato que necesita. Nómbralo o declara por escrito que has buscado y no existe." |
| "Se respeta la protección de datos." | "**Señal de fallo:** hay algún campo en este artefacto que, si se filtrara mañana, tendría que comunicar a alguien. Enuméralos." |

Cada criterio negativo **exige una salida escrita**: o encuentras el caso, o declaras explícitamente
que has buscado y no existe. "No aplica" no está permitido como respuesta.

**Truco 2 — Diferido y en tercera persona.** La autoevaluación se hace **al día siguiente**, nunca
al terminar, y con el encuadre "reviso el trabajo de alguien que hace mi puesto". Es el mismo
principio que fundamenta la mitigación más importante contra la adulación de la IA (§3.5): **la
autoría contamina el juicio**, en el modelo y en la persona. Distanciarse de la autoría es gratis y
mejora la detección. [J]

### 3.5 Mecanismo 6 — Usar la propia IA como correctora

Es el caso más relevante de este curso: la herramienta está delante, es gratis, es inmediata, cubre
cualquier cosa y ella ya sabe hablar con ella. Y es, sin protocolo, **el mecanismo más peligroso de
la lista**, porque falla en la misma dirección en la que ella ya está sesgada. El sesgo de
sobreestimación de §1.4b y la adulación del modelo **se suman**: no se cancelan.

#### 3.5.1 Los cinco riesgos, con lo que se sabe de cada uno

**Riesgo 1 · Adulación (sycophancy).** Los modelos se pliegan a la opinión declarada del usuario
aunque sea incorrecta. En un estudio sobre siete familias de modelos, una simple frase de opinión
("creo que la respuesta es X") indujo acuerdo con creencias falsas en una media del **63,7 %** de
los casos (rango 46,6 %–95,1 %). [E] *Cautela honesta: ese estudio usa modelos abiertos pequeños,
de 1B a 8B; no son los modelos que ella va a usar, y las cifras no se trasladan tal cual.* Pero el
fenómeno está documentado también en los modelos de frontera y en producción: OpenAI **retiró una
actualización de GPT-4o en abril de 2025** precisamente por adulación, y publicó el post-mortem
explicando que había pesado demasiado la señal de pulgar arriba/abajo de los usuarios. [E]

Dato accionable y directamente aprovechable: en ese mismo estudio, **la formulación en primera
persona indujo un 13,6 % más de adulación que la misma frase en tercera persona**, mientras que
declarar nivel de experiencia ("soy principiante" / "soy experta") apenas cambió nada (< 4,4 %). [E]
De ahí sale la mitigación 2 de §3.5.2, que es gratis.

**Riesgo 2 · Darle la razón cuando protesta.** Es el riesgo específico de la corrección, porque el
flujo natural es: la IA critica → ella no está de acuerdo → responde en el mismo hilo → la IA cede.
Kim y Khashabi (EMNLP 2025 Findings) muestran justo eso: los modelos como evaluadores **son mucho
más propensos a aceptar un contraargumento cuando llega como turno de conversación posterior que
cuando las dos posturas se presentan a la vez**; se dejan persuadir más si el argumento del usuario
*parece* razonado, aunque la conclusión sea falsa; y **se dejan convencer más por una réplica
informal que por una crítica formal**. [E]

Traducción: **la conversación es el vector del fallo**. Un veredicto en un turno único es
razonablemente sólido; el mismo veredicto tras tres turnos de discusión no vale nada.

**Riesgo 3 · Validación de trabajo mediocre.** Aquí operan dos sesgos documentados de
"LLM-como-juez": la **preferencia por lo verboso** —las respuestas largas puntúan más alto a
igualdad de calidad— y la **auto-preferencia** —el juez favorece texto generado por él mismo. [E]
Los dos apuntan al mismo desastre práctico: un entregable escrito con ayuda de la IA, evaluado por
la IA, en el mismo hilo, **tiene una probabilidad alta de aprobar por construcción**.

**Riesgo 4 · Autocorrección intrínseca que no funciona.** Huang et al. (ICLR 2024) muestran que los
modelos, pidiéndoles que revisen su propia respuesta **sin ninguna información externa**, no mejoran
y a menudo **empeoran**. [E] Corolario duro: *"revísalo tú mismo"* no es un mecanismo de corrección.
Toda corrección con IA que funcione tiene que aportar algo externo al modelo: **una rúbrica que no
ha escrito él, unos casos con respuesta conocida, o el trabajo de otro**.

**Riesgo 5 · La muleta.** El de Bastani et al. (§1.5): mientras la IA está delante, todo sale mejor;
cuando no está, sale peor que si nunca hubiera estado. [E] En este curso el riesgo no es que copie
la solución, es más sutil: que **delegue el criterio** y termine el curso sabiendo pedirle a la IA
que evalúe, sin saber evaluar. Y el criterio es literalmente lo único que el brief dice que no
caduca (`00-perfil.md`: *"las herramientas caducan; el criterio para elegirlas, no"*).

#### 3.5.2 El protocolo, en siete reglas

Esto va literalmente en el material, como página de referencia única, y se cita desde cada rúbrica.

> **Protocolo de corrección con IA — las siete reglas**
>
> **1. Hilo nuevo, siempre.** Nunca se corrige en la conversación donde se construyó. El modelo ya
> está comprometido con lo que ayudó a escribir. Chat en blanco, sin historial, sin memoria del
> proyecto. *(Contra riesgo 3.)*
>
> **2. No es tuyo.** El encuadre es: *"Reviso el trabajo de una compañera que hace mi mismo puesto.
> Tengo que decidir si se lo devuelvo."* Nunca "he hecho esto, ¿qué te parece?". Es la mitigación
> más barata que existe y tiene medida: **13,6 puntos** de diferencia entre primera y tercera
> persona. *(Contra riesgo 1.)*
>
> **3. Nunca preguntes si está bien.** "¿Está bien?" es una pregunta cerrada que invita al sí. La
> instrucción es: **"Enumera los incumplimientos de esta rúbrica. Por cada criterio, cita
> textualmente el fragmento del trabajo que lo incumple, o el que demuestra que se cumple. Si no
> puedes citar un fragmento, no lo afirmes."** La exigencia de cita literal es lo que impide a la
> vez la vaguedad y la invención. *(Contra riesgos 1 y 3.)*
>
> **4. Pega la rúbrica entera, con sus criterios negativos.** Sin rúbrica, el modelo se inventa el
> estándar, y el estándar que se inventa es benévolo. La rúbrica es la información externa sin la
> cual la revisión no funciona. *(Contra riesgo 4.)*
>
> **5. Prohibido discutir en el mismo hilo.** Si no está de acuerdo con una crítica, **no responde**.
> Anota el desacuerdo en la bitácora, corrige o no corrige, y abre un **hilo nuevo** con la versión
> modificada y la misma rúbrica. Si la crítica desaparece, era real y la ha arreglado. Si sigue,
> tiene un problema de verdad. *(Contra riesgo 2 — es la mitigación directa del hallazgo de Kim y
> Khashabi.)*
>
> **6. Dos modelos, y el desacuerdo es la señal.** Misma rúbrica, mismo trabajo, dos herramientas
> distintas (Gemini y ChatGPT, que ya usa las dos). **No para hacer media, ni para quedarse con el
> que le gusta más.** El único uso legítimo: **donde los dos coinciden en un fallo, el fallo es
> casi seguro; donde discrepan, ahí hay algo que ella no entiende todavía**, y eso —no el
> veredicto— es lo que anota. Los desacuerdos acumulados son, además, la mejor materia prima para
> un punto de consulta (sección 4). *(Contra riesgos 1 y 3.)*
>
> **7. Su veredicto no cierra nada.** La IA nunca dice "aprobado". Devuelve **una lista de fallos
> candidatos**. Quien decide si cada fallo es real, mirando el trabajo, es ella. *(Contra riesgo 5:
> el juicio no se delega, se informa.)*

#### 3.5.3 La calibración: el control positivo

Todo lo anterior asume que el corrector, bien encauzado, detecta algo. **Eso hay que comprobarlo, no
suponerlo.** Es un control positivo, y ella lo reconocerá al instante con ese nombre: si el
instrumento no detecta un caso que sabemos positivo, sus negativos no valen nada.

**Mecánica, una vez por escalón:** el curso trae un **cebo** — un artefacto de mentira, en un
fichero sellado, con **tres defectos plantados y documentados** (típicamente: uno visible, uno de
omisión, uno de criterio). Ella lo pasa por el protocolo completo, con la rúbrica real. Después abre
la hoja de defectos plantados y cuenta.

| Resultado | Lectura | Qué hace |
|---|---|---|
| Encuentra los 3 | El instrumento sirve para este tipo de trabajo | Sigue |
| Encuentra 2 | Normal. Detecta lo visible, se le escapa lo de criterio | Sigue, sabiendo que **la omisión y el criterio los tiene que cazar la lista de comprobación**, no la IA |
| Encuentra 1 o 0 | **El instrumento está roto para esta tarea** | Revisa la rúbrica (probablemente sea vaga). Si tras revisarla sigue igual: **esta tarea no se corrige con IA**, y pasa a mecanismos 2–4 |
| Aprueba el cebo entero | Descalificatorio | Ese tipo de trabajo **nunca** se corrige con IA en el resto del curso |

Este es, con diferencia, **el ejercicio más valioso de todo el curso**, y es transferible fuera de
él: es exactamente el procedimiento con el que se valida cualquier sistema de IA que uno vaya a
poner a decidir cosas. Aprender a auditar al corrector es una competencia mayor que aprender a usar
el corrector. [J]

#### 3.5.4 Los cuatro tipos de trabajo que la IA no puede corregir

Frontera explícita, porque es lo que define los puntos de consulta de la sección 4: [J]

1. **Lo que depende de hechos de su empresa que la IA no tiene.** Si el criterio de éxito es "esto
   refleja cómo se hace realmente aquí", el modelo no tiene acceso al referente. Solo lo puede
   verificar ella, o un compañero.
2. **Lo que depende del estado real de su Workspace.** Si un flujo falla, la IA especula sobre
   causas plausibles; no ve su consola ni sus permisos. La lista de comprobación empírica sí, la IA
   no.
3. **Las decisiones de riesgo con consecuencia externa irreversible.** Qué dato se puede meter en
   qué sitio, qué se envía sin revisión humana. Aquí "el modelo dijo que sí" no es una defensa.
4. **Los juicios de escala y de oportunidad.** "¿Merece la pena automatizar esto?" depende de su
   coste real, de la política interna y del volumen. El modelo, preguntado, dirá que sí — porque
   preguntar a un sistema si se debe hacer algo tiene un sesgo obvio hacia el sí.

**Los cuatro son, exactamente, la materia prima legítima de un punto de consulta.**

---

## 4. Diseño de los puntos de consulta con la pareja

### 4.1 El principio de escasez

El recurso hay que tratarlo como lo que es: **escaso, no renovable y con coste relacional**. Un
mentor pagado se gasta sin culpa; una pareja, no. Y un curso que convierta a la pareja en el soporte
técnico de la alumna dañará dos cosas a la vez: la relación y la autonomía que el curso persigue.

**Presupuesto propuesto: 6 consultas de ~10 minutos en todo el curso.** Una hora, repartida en
tres o cuatro meses. Es poco, es sostenible, y por eso se va a usar de verdad. [J]

Un curso que reserve "consultas ilimitadas" obtiene en la práctica **cero**, porque cada consulta
individual compite con la comodidad de no molestar y pierde. Un curso que reserve exactamente seis,
con nombre y momento, obtiene seis.

### 4.2 El filtro de admisión: cuatro preguntas

Antes de gastar un punto, la duda pasa por esto. **Si falla cualquiera de las cuatro, no es un punto
de consulta.** Va impreso en la portada de la bitácora. [J]

1. **¿Lo puede resolver el material?** Si está en la lección, en la solución comentada o en la página
   "Cuando no coincide" → no.
2. **¿Lo puede resolver la IA con el protocolo de §3.5.2?** Si es una pregunta de conocimiento
   general, de redacción o de "cómo se hace X" → no. Que la IA lo explique mal no lo convierte en
   punto de consulta: lo convierte en una pregunta mal hecha.
3. **¿Lo puede resolver mirar?** Si la respuesta está en su pantalla, en su consola o en preguntar a
   su administrador → no. Averiguarlo es el ejercicio.
4. **¿Lo he intentado durante 25 minutos y he anotado lo que he probado?** Si no → no todavía.

Lo que **sí** pasa el filtro es la lista de §3.5.4, más una quinta categoría: **el desbloqueo
emocional en un punto de caída conocido**. Esa es legítima y hay que reconocerla por escrito, porque
si no se nombra se disfraza de duda técnica y gasta el punto peor.

### 4.3 El formato que hace rendir diez minutos

El error clásico es llegar y decir "no me funciona esto". Con eso, diez minutos se van en reconstruir
el contexto y la conversación acaba con él tocando el teclado y ella mirando. Eso es la muleta de
Bastani (§1.5) en versión humana: rendimiento inmediato excelente, aprendizaje negativo.

**La ficha de consulta — cinco campos, escritos ANTES, máximo una cara:**

```
PUNTO DE CONSULTA nº __ · fecha __________ · módulo __________

1. LA PREGUNTA, EN UNA FRASE Y CERRADA
   (que se pueda contestar con «sí», «no» o «la B»)

2. MI HIPÓTESIS
   Creo que ______ porque ______.
   Si tengo razón, esperaría ver ______.

3. QUÉ HE PROBADO YA
   - probé ______ → pasó ______
   - probé ______ → pasó ______

4. EL DATO CONCRETO
   (mensaje de error literal, captura, las dos respuestas que se contradicen)

5. QUÉ HARÉ CON LA RESPUESTA
   Si me dice que sí → ______.  Si me dice que no → ______.
```

**Por qué cada campo está ahí:** [J]

- El campo 1 fuerza una pregunta cerrada. Una pregunta abierta consume los diez minutos en una
  explicación que ella podría haber leído.
- El campo 2 es lo que convierte la consulta en aprendizaje y no en servicio técnico. Comprometerse
  con una predicción antes de recibir la respuesta es práctica recuperativa (§2.1): **comprometerse
  y equivocarse enseña más que oír la respuesta correcta de entrada**.
- El campo 3 evita que él repita lo que ella ya descartó, que es donde se van los minutos.
- El campo 4 es lo único que él no puede deducir y lo que más rendimiento le saca a alguien que sabe:
  un mensaje de error literal poda el árbol de diagnóstico en segundos.
- El campo 5 impide las consultas que no cambian nada.

**Cuatro reglas de la conversación:** [J]

1. **Los cinco primeros minutos, sin pantalla.** Ella explica el problema en voz alta con la ficha
   delante. Muchas veces se resuelve ahí — es autoexplicación (§2.1) con un oyente.
2. **Él no toca el ratón.** Puede decir dónde mirar; no mira él. Regla explícita y acordada de
   antemano, para que no sea una negociación incómoda en el momento.
3. **Sale con una frase escrita**, en su propio lenguaje, en la bitácora, antes de que pase una hora.
4. **Si en diez minutos no se resuelve, se para.** Lo que no cabe en diez minutos no es una consulta:
   es un problema de diseño del curso y se anota como tal.

### 4.4 Los seis puntos, colocados

Cinco tienen momento asignado; uno es comodín. Los momentos están alineados con la escalera de
`dominio-herramientas.md` §7.2. [J]

| # | Momento | Pregunta que se lleva | Por qué aquí y no en otro sitio |
|---|---|---|---|
| **PC-1** | **Fin de semana 1**, tras el diagnóstico del plan de Workspace | *"He deducido que tenemos X y que por tanto no puedo hacer Y. ¿Me equivoco?"* Lleva las cinco comprobaciones empíricas hechas y las capturas | Es un hecho del mundo que el material no puede ver, y **un error aquí contamina el curso entero**. Es el punto con mejor relación consecuencia/coste |
| **PC-2** | **Antes de meter el primer dato real** (semana 2) | Su clasificación de **8 tipos de dato reales** de su puesto (nombre, pasaporte, dirección de la familia de acogida, importe, incidencia médica…) en tres cajones: cuenta de empresa / nunca / depende. Él solo dice de acuerdo o no, y por qué | Riesgo irreversible con consecuencia externa (§3.5.4-3). Es la única decisión del curso donde equivocarse tiene coste fuera del curso |
| **PC-3** | **Tras el primer cebo** (§3.5.3), semana 3–4 | *"Esta es la corrección que me hizo la IA de un trabajo con tres fallos plantados. Encontró dos. ¿Estoy leyendo bien lo que se le escapa?"* | **Es el punto de mayor apalancamiento del curso.** No se revisa su trabajo: se revisa **su instrumento de corrección**, que va a usar cincuenta veces más. Diez minutos aquí valen por todas las correcciones posteriores |
| **PC-4** | **Comodín**, disponible desde la semana 5 | Un fallo de plataforma en el escalón 2 tras agotar la lista de comprobación y la página "Cuando no coincide" | Es el caso canónico de "diez minutos ahorran una tarde" (§3.5.4-2). **No tiene fecha a propósito**: saber que existe un comodín reduce el miedo a atascarse, que es un factor de abandono por sí mismo |
| **PC-5** | **Fin del escalón 2** (semana 7–8) | *"Esta es la frontera que he trazado entre lo que automatizo y lo que no. Aquí están los tres casos donde he dudado. ¿Dónde la moverías?"* | Juicio de escala y oportunidad (§3.5.4-4). Requiere que ella ya tenga dos flujos vivos: antes no hay sustancia sobre la que conversar |
| **PC-6** | **Cierre** | *"Esto es lo que tengo funcionando. ¿Qué es lo siguiente que tendría sentido, y qué tendría que cambiar para que mereciera la pena?"* | Cierra el curso con una orientación que ella no puede darse sola, y evita el final en el vacío (§6, punto 7) |

**Lo que deliberadamente NO es punto de consulta**, y conviene escribirlo para que no se erosione:
revisar un entregable ("¿está bien mi Gem?" → rúbrica + casos), explicar un concepto ("¿qué es MCP?"
→ material), enseñarle a hacer algo ("¿cómo se hace un flujo?" → documentación), o dar ánimos
genéricos. Y una tentación específica de esta configuración: **que él le monte algo "que es un
momento"**. Eso no es una consulta, es un artefacto que ella no sabrá mantener ni depurar, y en el
escalón siguiente será deuda.

### 4.5 La vía de escape

La pareja puede no estar disponible cuando toca. El material no puede tener un paso bloqueante que
dependa de otra persona, o reproduce el peor defecto del curso de referencia (`01-analisis-referencia.md`
§5: la mitad del valor estaba en la cohorte). **Cada punto de consulta lleva su alternativa
degradada escrita justo debajo**, y el curso continúa sin él: [J]

- PC-1 → asumir el escenario más restrictivo (Business Starter) y anotar la suposición en la bitácora
  como pendiente de confirmar.
- PC-2 → aplicar la regla de máxima cautela por defecto: **si dudas, no lo metes**, y lo anotas.
- PC-3 → hacer el cebo dos veces con dos modelos distintos y comparar; el desacuerdo entre modelos
  es un sustituto pobre pero real del juicio externo.
- PC-4 → la caja "si nada de esto funciona": documentar el fallo, **rodearlo** con una solución
  manual, y seguir. Un curso no puede parar por un botón que Google movió.
- PC-5 → la lista de criterios de exclusión de `dominio-academia.md` (riesgo crítico, dependencia de
  terceros, volumen bajo).
- PC-6 → la tabla de escalones de `dominio-herramientas.md` §7.2.

---

## 5. Carga cognitiva y secuenciación

### 5.1 La restricción real, dicha sin optimismo

Jornada completa en un puesto que en verano recibe 250–400 correos al día y donde, según
`dominio-academia.md` §0.2, *"una misma persona atiende el teléfono, contesta el buzón compartido,
resuelve una incidencia de alojamiento y emite una carta de visado en la misma hora"*.

De ahí sale la restricción de diseño más importante de esta sección: **cualquier solución de IA —y
cualquier módulo del curso— que exija "dedicar un rato tranquilo" fracasa.** El curso tiene que
funcionar en trozos interrumpibles.

**Presupuesto honesto: 2 horas semanales de tiempo propio.** Todo lo que se pida por encima de eso
no se hará; se acumulará como deuda, y la deuda acumulada es un mecanismo de abandono documentado.
Es mejor un curso de 18 semanas que se termina que uno de 10 que se abandona en la 3. [J]

**Y el truco que hace que 2 horas alcancen:** una parte importante del trabajo del curso **no cuesta
tiempo adicional**, porque es trabajo del puesto hecho de otra manera. Construir un Gem que redacta
la confirmación de alojamiento no es tiempo de curso: es la tarea P18 hecha una vez despacio en vez
de treinta veces deprisa. **El curso debe declarar explícitamente qué actividades son "tiempo
propio" y cuáles son "tiempo de trabajo".** Sin esa distinción escrita, ella contabilizará todo como
tiempo propio y el curso parecerá el doble de caro de lo que es. [J]

### 5.2 Las tres unidades de tiempo

| Unidad | Duración | Qué cabe dentro | Cuántas por semana |
|---|---|---|---|
| **Micro-sesión** | **10 min** | 5 preguntas de recuperación espaciada + una decisión anotada en la bitácora. **No requiere ordenador ni contexto.** | 2–3 |
| **Sesión núcleo** | **35–45 min** | 1 concepto nuevo + 1 ejemplo trabajado + 1 ejercicio que produce algo | 2 |
| **Bloque de proyecto** | **60–90 min**, en horario de trabajo | Construir o corregir un artefacto del hilo | 1 (o ninguno en semana de pico) |

**Por qué 35–45 y no 25 ni 90.** Por debajo de 30 no cabe un ciclo completo
recordar → ver → hacer → comprobar, y una sesión que no cierra un ciclo deja trabajo a medias, que
es lo que más cuesta retomar. Por encima de 50 la probabilidad de que la sesión no llegue a empezar
crece mucho más rápido que su valor: una sesión de 90 minutos en un puesto interrumpible se aplaza,
y aplazada dos veces está muerta. [J]

### 5.3 Tamaño de módulo y densidad

- **Módulo = 3 sesiones núcleo + 1 bloque de proyecto + 1 evaluación.** Dos semanas naturales.
- **Máximo 3 conceptos nuevos con nombre por sesión núcleo.** Nombre propio = algo que tendrá que
  recordar para el módulo siguiente. Este es el límite de carga cognitiva que más se incumple en
  material técnico, y para alguien sin base es la diferencia entre seguir y desconectar. [D]
- **Máximo 1 herramienta nueva por módulo.** Regla heredada de `dominio-herramientas.md` §7.1
  ("ningún escalón introduce una herramienta nueva antes de haber agotado la anterior").
- **Cada sesión núcleo produce algo que existe fuera del curso.** Aunque sea un párrafo en un
  fichero. Una sesión que solo produce comprensión no deja rastro y alimenta la ilusión de fluidez.
- **Duración total realista: 16–20 semanas.** Con 9–10 módulos. Decirlo desde el principio: un curso
  que se anuncia de 8 semanas y dura 18 se percibe como fracaso propio a la semana 9.

### 5.4 El desvanecimiento, y cuándo hay que dejar de andamiar

El andamiaje tiene fecha de caducidad. El **efecto de reversión de la pericia** dice que el apoyo
que ayuda al novato estorba al que ya sabe: los ejemplos completos, útiles en el módulo 1, en el
módulo 6 se saltan, y un material que se salta pierde autoridad. La progresión, aplicada
mecánicamente por escalón: [D]

| Escalón | Ejemplo trabajado | Ejercicio | Corrección |
|---|---|---|---|
| 0–1 (semanas 1–3) | **Completo**, con la autoexplicación de cada paso escrita | Rehacer el ejemplo con sus datos | Clave sellada, casi todo comprobación |
| 1–1,5 (semanas 4–5) | **Con los dos últimos pasos en blanco** (desvanecimiento hacia atrás) | Variante propia con el mismo esqueleto | Clave + lista de comprobación |
| 2 (semanas 6–8) | **Solo el esqueleto** y los criterios de éxito | Su propio caso, ella elige el enfoque | Rúbrica + IA con protocolo |
| 3 (semanas 9+) | **Solo el enunciado y la rúbrica** | Su propio caso, ella diseña también los criterios | Ella escribe la rúbrica; la IA busca fallos contra ella |

El destino de la progresión es explícito y hay que decirlo: **al final del curso ella escribe las
rúbricas**. Ese es el momento en el que ya no necesita el curso, y es el único criterio honesto de
que ha terminado.

### 5.5 El calendario contra la estacionalidad

Restricción específica que ninguna literatura cubre y que domina sobre todo lo demás. [D]

- **No empezar en junio, julio, agosto ni la primera quincena de septiembre.** Ventana buena:
  **octubre a mayo**, con noviembre–febrero como tramo ideal (temporada baja según
  `dominio-academia.md` §0.3). Nota práctica: hoy es 22 de agosto de 2026, o sea que arrancar en
  **octubre** encaja bien y da margen para producir el material.
- **Modo mínimo declarado de antemano.** Semanas de pico o imprevisto: **una micro-sesión de 10
  minutos y nada más**, y eso cuenta como semana cumplida. Estar en modo mínimo no es fallar; el
  curso lo dice explícitamente. Sin esta cláusula, una semana mala se lee como fracaso, y el fracaso
  percibido es lo que precipita el abandono, no la semana perdida.
- **Ritual de reentrada.** Toda vuelta tras una interrupción empieza por lo mismo: leer las tres
  últimas entradas de la bitácora y responder las 5 preguntas de repaso. Diez minutos, y elimina el
  coste de arranque, que es lo que hace que una pausa de una semana se convierta en el final.
- **Si el proyecto hilo es estacional, no vale.** Un hilo sobre "gestión de llegadas de julio" no se
  puede practicar en enero. El hilo tiene que ser de volumen continuo.

---

## 6. Puntos típicos de caída, y qué se pone justo antes

La sección 1.2 dice que el abandono es episódico y localizable. Esta es la tabla operativa. La
columna que importa es la tercera. [D/J]

| # | Momento | Qué pasa por dentro | **Qué se pone justo antes** |
|---|---|---|---|
| **1** | **Antes de la lección 1** — el 52 % de Reich no llega a empezar | Fricción de arranque: hay que configurar, registrarse, entender el sistema | La sesión 1 **no explica el curso**. Produce un resultado utilizable en 20 minutos con lo que ya tiene abierto. Sin instalar nada, sin pedir nada a nadie. El mapa del curso va **después** del primer resultado, nunca antes |
| **2** | **Días 7–14** — la caída mayor | Se acabó la novedad, aparece el primer coste real, el beneficio aún es abstracto | Un **artefacto que le ahorre tiempo antes del día 10** — y el curso lo dice de antemano y luego lo comprueba: *"apunta cuántos minutos tardas hoy en hacer X; el día 10 lo vuelves a medir"*. Es la prueba objetiva contra la ilusión de fluidez (§1.4a) |
| **3** | **Primer resultado mediocre** — el Gem contesta mal | Atribución interna: *"esto no es para mí"* | La caja **"Lo que vas a ver la primera vez"**, escrita antes del ejercicio, describiendo el resultado mediocre concreto que va a obtener. Y la cita del webinar: *"Ves el resultado. Detrás hay varias decenas de intentos."* Predecir el fallo lo convierte de señal de incompetencia en paso previsto del proceso |
| **4** | **Primer bloqueo técnico real** (escalón 2) | Frustración + no saber si el problema es ella o la plataforma | La página **"Cuando no coincide"** (`dominio-herramientas.md` §8.2) + la lista de 6 comprobaciones + **el comodín PC-4**, cuya existencia se anuncia mucho antes de que haga falta. Saber que hay salida reduce la ansiedad aunque no se use |
| **5** | **Semana de pico o imprevisto** | Se pierde una semana → se percibe fracaso → no se vuelve | El **modo mínimo** y el **ritual de reentrada** (§5.5), escritos en la semana 1, no cuando ya ha fallado |
| **6** | **Transición escalón 2 → 3** (semana 8–9) | Los conceptos se abstraen, el pago está más lejos, la novedad se agotó | Colocar aquí **la automatización de mayor retorno visible**, no antes. Y **PC-5** justo en esta frontera: una conversación de diez minutos sobre su propio criterio es el mejor combustible disponible en el punto donde el material solo ya no tira |
| **7** | **El final sin final** | Se queda a dos módulos, sin evento que marque el fin | **"Terminado" se define en la semana 1 y es observable**: *tres artefactos vivos que uso sin que el curso me lo pida, más una rúbrica escrita por mí*. No es "leer la última lección". Y **PC-6** como cierre con otra persona |

Dos principios transversales que salen de esta tabla: [J]

- **Toda contramedida se escribe antes del punto de caída, no en él.** El modo mínimo redactado la
  semana en que ya ha fallado se lee como excusa; redactado en la semana 1 se lee como plan.
- **Predecir el fallo es la contramedida más barata que existe.** Un fallo anunciado es una etapa;
  un fallo inesperado es un veredicto sobre uno mismo.

---

## 7. El proyecto hilo, y sus trampas

### 7.1 Por qué hilo, y por qué doble

**Por qué hilo:** es la contramedida estructural al hallazgo de §1.3. Si el trabajo del curso es
trabajo del puesto, deja de competir por tiempo libre. Además, es lo que convierte una colección de
módulos en algo con memoria: cada módulo hereda el artefacto del anterior, tal como impone
`dominio-herramientas.md` §7.1.

**Por qué doble.** Un hilo único tiene un fallo fatal en un curso sin profesor: **si el proyecto está
mal elegido, no hay quien lo detecte y el curso entero se hunde con él**. La solución es tener dos:

- **Hilo guiado — el análisis de las encuestas de satisfacción (P27).** Lo trae el curso con datos
  sintéticos multilingües, **clave de corrección sellada, solución comentada y cebos**. Es el
  recomendado por `dominio-herramientas.md` §9.6: riesgo bajo, volumen alto, multilingüe, y hoy no
  se hace, así que no compite con un procedimiento establecido. **Su función principal no es
  producir valor: es ser el patrón calibrado contra el que ella aprende qué es "bien hecho".** Es
  el mecanismo 2 de §3.2 hecho proyecto.
- **Hilo propio — un proceso suyo, elegido en la semana 1 contra criterios explícitos.** Sin clave,
  porque no puede haberla. Se corrige con la rúbrica y el protocolo calibrados en el hilo guiado.

La relación entre los dos es la que resuelve el problema del feedback a escala de proyecto: **el
hilo guiado tiene oráculo y el propio no, así que el guiado va siempre un paso por delante** y le
enseña el criterio que después aplica al suyo. Cada módulo se hace primero en el guiado (con clave)
y después en el propio (sin ella). [J]

### 7.2 Criterios para elegir el hilo propio

Se aplican en la semana 1 sobre el inventario de 32 procesos de `dominio-academia.md`. Filtro
mecánico, no impresionista: [D]

**Requisitos (todos):**
1. Ocurre **al menos una vez por semana durante todo el año** (nada estacional, §5.5).
2. **Lo hace ella**, no un compañero.
3. Los datos que necesita **ya los puede ver** hoy, sin pedir permisos nuevos.
4. La salida es **texto, clasificación o resumen** — no una decisión con consecuencia directa.
5. **No depende de que otra persona cambie de comportamiento.**
6. Riesgo **bajo o medio**. Nunca crítico.

**Descalificadores automáticos**, con nombre y número:
- **P08** (carta de aceptación para visado): riesgo CRÍTICO, un error deniega un visado.
- **P22** (calendario de camas): riesgo CRÍTICO por overbooking.
- **P26** (quejas formales) y **P29** (emergencias 24 h): riesgo CRÍTICO y no deterministas.
- Cualquier proceso que **envíe algo a un cliente sin revisión humana**.

**Candidatos que pasan el filtro limpiamente:** P01 (respuesta a solicitud de información: volumen
altísimo, 70–80 % pregunta lo mismo), P27 (encuestas), P30 (parte semanal: determinista, volumen
semanal fijo, riesgo interno), P32 (mantenimiento de plantillas y FAQ: "el yacimiento del curso"
según `dominio-academia.md` §0.4). P18 (confirmación de alojamiento) es buen candidato **solo con la
regla de "prepara, no envía"**.

### 7.3 Las siete trampas del formato, y su contramedida

| Trampa | Cómo se manifiesta | Contramedida |
|---|---|---|
| **Punto único de fallo** | El proceso elegido resulta ser malo en el módulo 4 y el curso se hunde | **Checkpoint de divorcio** al final del escalón 1: cambiar de hilo propio es un movimiento **legítimo y preautorizado**, no un fracaso. Escrito en la semana 1. Y el hilo guiado sostiene el curso mientras tanto |
| **Ambición** | Elige el proceso más doloroso, que es el más complejo y el más arriesgado | Los criterios de §7.2 aplicados por escrito, con los descalificadores por número de proceso. El proceso más doloroso es el **segundo** proyecto, no el primero |
| **El proyecto se come el temario** | Solo aprende lo que su caso necesita; queda con una solución y sin criterio | **Casos satélite**: cada módulo lleva un ejercicio corto de 15 minutos sobre un proceso **distinto** del hilo. Es lo que hace que el criterio generalice y no se pegue al caso |
| **El temario se come el proyecto** | Aparece un módulo que no encaja y se fuerza el encaje | Se permite explícitamente que un módulo se haga **solo en el hilo guiado**. Forzar el ajuste produce artefactos que ella no usará, y un artefacto que no se usa es peor que ninguno |
| **Dependencia externa** | El proyecto necesita que el administrador habilite algo o que un compañero cambie de hábito | Requisitos 3 y 5 de §7.2, verificados **antes** de empezar, no descubiertos en el módulo 5 |
| **Se termina antes de tiempo** | En la semana 6 el proyecto está acabado y los módulos 7–10 quedan sin dónde aterrizar | El hilo se define como **proceso**, no como artefacto. P27 no es "hacer un informe": es "que el análisis de encuestas esté resuelto", y eso admite capas — clasificar, resumir, detectar tendencia, avisar, informar |
| **El proyecto tapa el aprendizaje** | Acaba con tres cosas funcionando y sin saber por qué funcionan | Autoexplicación obligatoria en cada entregable (§2.1) y, al final, **la rúbrica escrita por ella** (§5.4). Si no puede escribir los criterios de su propio artefacto, el proyecto salió y el curso no |

### 7.4 La regla que atraviesa todo el hilo

De `dominio-herramientas.md` §9.7, y merece ser el lema del curso porque resuelve a la vez el riesgo
de datos, el riesgo reputacional y el problema del feedback:

> **Automatiza la lectura y la preparación; la escritura hacia fuera la firma una persona.**

Para el feedback tiene una consecuencia que no es obvia: **si el artefacto solo prepara y nunca
envía, todos sus errores son recuperables**, y por tanto se puede aprender de ellos sin coste. Un
curso construido sobre artefactos que preparan puede permitirse equivocarse mucho, que es lo que
hace falta para aprender. Uno construido sobre artefactos que envían, no.

---

## 8. Patrones de material

Estos cinco patrones son el producto principal de este documento. Se aplican **mecánicamente**: si un
módulo no se puede escribir con ellos, el problema es del módulo.

### 8.1 Plantilla de lección

```markdown
# M<n>.<s> — <Título en forma de tarea, no de tema>

⏱ <35–45 min> · Necesitas: <lo que debe tener abierto>
Tipo de tiempo: [ tiempo propio | tiempo de trabajo ]

## Antes de leer nada — 5 minutos, de memoria y por escrito
1. <pregunta del módulo anterior>
2. <pregunta del módulo anterior>
3. <pregunta de hace 2–3 módulos>
4. <pregunta de hace 2–3 módulos>
5. <pregunta sobre el proyecto hilo>
> Escribe lo que recuerdes ANTES de mirar. Equivocarte aquí es el ejercicio, no un fallo.
> Respuestas al final de la lección.

## Para qué sirve esto en tu trabajo
<3–5 líneas. Proceso concreto de dominio-academia.md, con su número. Sin abstracciones.>

## El criterio        ← no caduca: sin capturas, sin nombres de menú
<Por qué se hace así. Qué problema resuelve. Cómo se decide si toca.
 Máximo 3 conceptos nuevos con nombre.>

## Los clics de hoy   ← caduca
> Verificado el <fecha>. Si no coincide con tu pantalla, **tu pantalla tiene razón**.
> Ve a «Cuando no coincide».
<Rutas, botones, límites.>

## Ejemplo trabajado
<Completo / con los 2 últimos pasos en blanco / solo esqueleto — según §5.4>
<Cada paso lleva su POR QUÉ, no solo su QUÉ.>

## Lo que vas a ver la primera vez
<Descripción honesta del resultado mediocre que va a obtener. Obligatorio
 en toda lección donde se construya algo por primera vez.>

## Tu turno
→ Ejercicio E<n>.<s>

## Cierre — 3 líneas en la bitácora
- Qué he producido: ______
- Qué ha fallado: ______
- Qué haré distinto la próxima vez: ______

---
### Respuestas de las 5 preguntas
```

**Reglas no negociables:** el bloque de recuperación va **primero**, siempre, y las respuestas al
final. "El criterio" y "Los clics" **nunca se mezclan**. Ninguna lección termina en lectura. Ningún
ejercicio depende de una captura para poder hacerse.

### 8.2 Plantilla de ejercicio

```markdown
# E<n>.<s> — <Lo que vas a producir>

⏱ <minutos> · Hilo: [ guiado (con clave) | propio (sin clave) | satélite ]

## Lo que tienes que producir
<Un artefacto concreto y nombrable. Dónde queda guardado.>

## Criterios de éxito — obsérvalos, no los valores
Al terminar, esto tiene que ser cierto:
- [ ] <observable, verificable mirando>
- [ ] <observable>
- [ ] <observable>

## Cómo lo vas a comprobar
Marca el nivel más alto que aplique — nunca uses uno inferior si hay uno superior disponible:
- [ ] **Se ejecuta** → <cómo dispararlo y qué tiene que pasar>
- [ ] **Batería de 10 casos** → `casos-E<n>.<s>.md` · clave: `CLAVE-E<n>.<s>.md` (**no abrir antes**)
- [ ] **Lista de comprobación** → abajo
- [ ] **Rúbrica + protocolo de IA** → `rubrica-E<n>.<s>.md` + `protocolo-ia.md`

## Antes de comprobar nada: escríbelo
> **Por qué lo he hecho así:** <3–5 líneas, en tus palabras>
> **Dónde creo que falla:** <1 línea>
Esto se escribe ANTES de corregir. Si lo escribes después, no sirve.

## Lista de comprobación
- [ ] <ítem binario y observable>
- [ ] <ítem binario y observable>
… (8–12 ítems)

## Si te atascas
1. <pista concreta>
2. <pista más concreta>
3. <la solución, tras 25 minutos de intento>
> Las pistas se abren en orden, no de golpe.
```

**Regla del atasco:** las pistas están escalonadas y con umbral de tiempo. Un ejercicio sin pistas
produce abandono; con la solución al lado produce muleta (§1.5). Las pistas escalonadas son el
equivalente material de la salvaguarda que en Bastani et al. eliminó el daño.

### 8.3 Plantilla de rúbrica

```markdown
# Rúbrica — E<n>.<s>

Se usa **al día siguiente**, nunca al terminar.
Encuadre obligatorio: *"reviso el trabajo de alguien que hace mi puesto".*

## Bloque 1 · Señales de fallo (obligatorio buscar y responder)
Por cada una: encuentra el caso, o **declara por escrito que has buscado y no existe**.
"No aplica" no es una respuesta admitida.

| # | Señal de fallo | Encontrado | Dónde / por qué no |
|---|---|---|---|
| 1 | Existe una pregunta razonable que esto contestaría de dos formas distintas según el día | ☐ | |
| 2 | Hay un caso en el que sigue adelante sin un dato que necesita | ☐ | |
| 3 | Hay algún dato aquí dentro que, si se filtrara mañana, tendría que comunicar a alguien | ☐ | |
| 4 | Hay un paso que sale hacia fuera sin que yo lo apruebe | ☐ | |
| 5 | <específica del módulo> | ☐ | |

## Bloque 2 · Umbral de "listo"
NO está listo si se cumple **cualquiera** de estas:
- Falla más de 0 de los 5 casos normales.
- Se inventa una decisión en alguno de los 3 casos límite en lugar de pedir aclaración.
- Responde algo distinto de "no lo sé" en alguno de los 2 casos de rechazo.
- Alguna señal de fallo del bloque 1 está marcada y sin arreglar.

## Bloque 3 · Si lo pasas por la IA
Protocolo completo en `protocolo-ia.md`. Recordatorio de las tres que más se olvidan:
hilo nuevo · no digas que es tuyo · **no discutas: abre otro hilo**.

## Mi veredicto (lo firmo yo, no la IA)
[ ] Listo  ·  [ ] Le falta: ______  ·  [ ] Lo dejo así y anoto por qué: ______
```

### 8.4 Plantilla de solución comentada

```markdown
# Solución comentada — E<n>.<s>

## Una solución posible
<El artefacto completo.>

## Por qué está así — decisión a decisión
| Decisión | Por qué esta y no otra | Qué habría pasado con la otra |
|---|---|---|

## Anatomía de los errores típicos
### Fallo 1 · <nombre corto y memorable>
- **Cómo se reconoce en tu propio trabajo:** <señal observable, no abstracta>
- **Por qué pasa:** <la intuición razonable que lo produce>
- **Arreglo mínimo:** <un paso>
### Fallo 2 · … (5–6 fallos)

## Lo que también sería correcto
<2–3 variantes válidas. Impide leer "distinto" como "mal".>

## Lo que parece correcto y no lo es
<1–2 variantes plausibles pero defectuosas, con el defecto explicado.>
```

El bloque final es el que más se olvida y el que más falta hace: sin él, la única forma que tiene de
evaluarse es el parecido con la solución modelo, que es un criterio malo.

### 8.5 Plantilla de punto de consulta

```markdown
# PC-<n> — <Título> · momento: <cuándo>

## Por qué esto merece gastar un punto
<Cuál de los 4 casos de §3.5.4 es. Una línea.>

## Antes de la conversación (obligatorio, se escribe entero)
<La ficha de 5 campos de §4.3, ya rellenada con lo específico de este punto.>

## Cómo se desarrolla
1. Cinco minutos **sin pantalla**: explícalo en voz alta con la ficha delante.
2. Enseña el dato del campo 4.
3. **Él no toca el ratón.**
4. A los 10 minutos se para, esté como esté.

## Después (dentro de la hora siguiente)
En la bitácora, **con tus palabras, no con las suyas**:
- Lo que he entendido: ______
- Lo que cambio a partir de ahora: ______
- Lo que sigue sin cuadrarme: ______

## Si no está disponible
<Alternativa degradada concreta — §4.5. El curso continúa.>
```

### 8.6 Lista de producción: qué tiene que existir para dar un módulo por escrito

Aplicable como comprobación mecánica antes de publicar cada módulo:

- [ ] 3 lecciones con los bloques `El criterio` / `Los clics de hoy` separados y fechados
- [ ] 5 preguntas de recuperación por lección, mezclando módulo actual, anterior y uno de hace 2–3
- [ ] 1 ejemplo trabajado en el nivel de desvanecimiento que toca según §5.4
- [ ] 1 caja "Lo que vas a ver la primera vez" en toda lección donde se construya algo por primera vez
- [ ] 1 ejercicio de hilo guiado **con clave sellada**
- [ ] 1 ejercicio de hilo propio **sin clave**, con rúbrica
- [ ] 1 caso satélite de 15 minutos sobre un proceso distinto del hilo
- [ ] 1 batería de 10 casos (5 normales / 3 límite / 2 de rechazo)
- [ ] 1 lista de comprobación de 8–12 ítems binarios y observables
- [ ] 1 rúbrica con **al menos 3 criterios negativos**
- [ ] 1 solución comentada con 5–6 fallos típicos + "lo que parece correcto y no lo es"
- [ ] Pistas escalonadas en 3 niveles para cada ejercicio
- [ ] **Cero** dependencias de otra persona para poder avanzar
- [ ] **Cero** ejercicios que no se puedan hacer sin la captura de pantalla
- [ ] Todo número volátil, en `datos-volatiles.md`, no en el texto

---

## 9. Resumen ejecutivo

1. **La mitad de la mortalidad ocurre antes de empezar** (52 % en edX). La lección 1 no explica el
   curso: produce algo utilizable en 20 minutos sin instalar ni pedir nada.
2. **Las dos primeras semanas valen más que las diez siguientes.** El abandono es predecible al 80 %
   con datos de la semana 2.
3. **Su termómetro está invertido.** Aprender más se siente peor (Deslauriers), y la autoevaluación
   sobreestima (León et al.) — pero la sobreestimación **se corrige con criterios explícitos y
   feedback**. Ese es el mandato entero del material.
4. **La primera pregunta de diseño de cada módulo no es "qué rúbrica pongo" sino "¿puedo convertir
   esto en una comprobación?"**. Los tres mecanismos de corrección más fiables —ejecución real, casos
   con respuesta conocida, lista binaria— no requieren juicio de nadie.
5. **La IA correctora es el puesto 6 de 9, no el 1.** Vale por cobertura e inmediatez, no por
   fiabilidad, y falla en la misma dirección en la que ella ya está sesgada.
6. **Siete reglas domestican al corrector:** hilo nuevo · no digas que es tuyo (13,6 puntos medidos)
   · nunca "¿está bien?" sino "cita el fragmento que incumple" · pega la rúbrica · **no discutas en el
   mismo hilo** · dos modelos para detectar desacuerdo, no para dirimirlo · el veredicto no cierra.
7. **El control positivo (el cebo) es el ejercicio más valioso del curso.** Un artefacto con tres
   fallos plantados, una vez por escalón. Si el corrector no los ve, sus aprobados no valen nada — y
   eso es psicometría, que es su casa.
8. **Seis puntos de consulta de diez minutos en todo el curso**, con filtro de admisión de cuatro
   preguntas y ficha de cinco campos escrita antes. El de mayor apalancamiento no revisa su trabajo:
   **revisa su corrector** (PC-3). Cada uno lleva su alternativa degradada, porque nada puede
   bloquear.
9. **Dos horas semanales de tiempo propio, 16–20 semanas, sesiones de 35–45 minutos, y arranque en
   octubre.** El pico de junio–septiembre de la academia mata cualquier calendario que lo ignore. El
   modo mínimo y el ritual de reentrada se escriben en la semana 1, no cuando ya ha fallado.
10. **Doble hilo:** uno guiado con clave sellada (encuestas, P27), que es el patrón calibrado, y uno
    suyo sin clave, corregido con los instrumentos que el guiado calibró. Resuelve a la vez la
    motivación, el punto único de fallo y el problema del feedback.

---

## 10. Fuentes

**Abandono y finalización**
- Jordan, K. (2015). *Massive Open Online Course Completion Rates Revisited: Assessment, Length and Attrition*. IRRODL. [ERIC EJ1067937](https://files.eric.ed.gov/fulltext/EJ1067937.pdf)
- Reich, J. y Ruipérez-Valiente, J. A. (2019). *The MOOC pivot*. **Science**, 363(6423), 130-131. [DOI](https://www.science.org/doi/10.1126/science.aav7958) · [PubMed](https://pubmed.ncbi.nlm.nih.gov/30630920/) · cobertura: [Inside Higher Ed](https://www.insidehighered.com/digital-learning/article/2019/01/16/study-offers-data-show-moocs-didnt-achieve-their-goals)
- Eriksson, T., Adawi, T. y Ståhr, C. (2017). *"Time is the bottleneck": a qualitative study exploring why learners drop out of MOOCs*. **Journal of Computing in Higher Education**, 29, 133-146. [DOI](https://doi.org/10.1007/s12528-016-9127-8) · [PDF](https://d-nb.info/1121919162/34)
- Alamri, A. et al. (2019). *Predicting MOOCs Dropout Using Only Two Easily Obtainable Features from the First Week's Activities*. ITS 2019. [Springer](https://link.springer.com/chapter/10.1007/978-3-030-22244-4_20)
- Chen, J. et al. *Temporal prediction of dropouts in MOOCs*. [ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S074756321530279X)

**Cómo se aprende sin profesor**
- Dunlosky, J., Rawson, K. A., Marsh, E. J., Nathan, M. J. y Willingham, D. T. (2013). *Improving Students' Learning With Effective Learning Techniques*. **Psychological Science in the Public Interest**, 14(1), 4-58. [SAGE](https://journals.sagepub.com/doi/abs/10.1177/1529100612453266) · [PDF](https://gwern.net/doc/psychology/spaced-repetition/2013-dunlosky.pdf)
- Adesope, O. O., Trevisan, D. A. y Sundararajan, N. (2017). *Rethinking the Use of Tests: A Meta-Analysis of Practice Testing*. **Review of Educational Research**, 87(3), 659-701. [SAGE](https://journals.sagepub.com/doi/abs/10.3102/0034654316689306)
- Bisra, K., Liu, Q., Nesbit, J. C., Salimi, F. y Winne, P. H. (2018). *Inducing Self-Explanation: a Meta-Analysis*. **Educational Psychology Review**, 30, 703-725. [Springer](https://link.springer.com/article/10.1007/s10648-018-9434-x) · [ERIC](https://eric.ed.gov/?id=EJ1186664)
- Atkinson, R. K., Renkl, A. y Merrill, M. M. (2003). *Transitioning From Studying Examples to Solving Problems: Effects of Self-Explanation Prompts and Fading Worked-Out Steps*. [PDF](https://mrbartonmaths.com/resourcesnew/8.%20Research/Making%20the%20most%20of%20examples/Fading%20out%20and%20Prompts.pdf) · Renkl y Atkinson (2004), *How Fading Worked Solution Steps Works — A Cognitive Load Perspective*, **Instructional Science**. [Springer](https://link.springer.com/article/10.1023/B:TRUC.0000021815.74806.f6)
- Gollwitzer, P. M. y Sheeran, P. (2006). *Implementation Intentions and Goal Achievement: A Meta-Analysis of Effects and Processes*. **Advances in Experimental Social Psychology**, 38, 69-119. [ResearchGate](https://www.researchgate.net/publication/37367696_Implementation_Intentions_and_Goal_Achievement_A_Meta-Analysis_of_Effects_and_Processes)
- Kizilcec, R. F. et al. — sobre por qué los consejos genéricos de autorregulación no funcionan en MOOCs y los *planning prompts* sí. [Recommending Self-Regulated Learning Strategies Does Not Improve Performance in a MOOC](https://www.researchgate.net/publication/301222981_Recommending_Self-Regulated_Learning_Strategies_Does_Not_Improve_Performance_in_a_MOOC) · [The Promises and Pitfalls of SRL Interventions in MOOCs](https://link.springer.com/article/10.1007/s10758-021-09580-9)

**Autoevaluación, rúbricas y feedback**
- León, S. P., Panadero, E. y García-Martínez, I. (2023). *How Accurate Are Our Students? A Meta-analytic Systematic Review on Self-assessment Scoring Accuracy*. **Educational Psychology Review**, 35, 106. [Springer](https://link.springer.com/article/10.1007/s10648-023-09819-0) · [PDF](https://ernestopanadero.es/Publications/Articles/078_Leon_et_al_2023_How_accurate_ar_our_students.pdf)
- Panadero, E. y Jonsson, A. (2013). *The use of scoring rubrics for formative assessment purposes revisited: A review*. **Educational Research Review**, 9, 129-144. [PDF](https://www.ernestopanadero.es/Publications/Articles/004_Panadero_&_Jonsson_2013_The_use_of_scoring_rubrics_for_formative_assessment_purposes_revisited_a_review.pdf)
- Panadero, E. et al. (2023). *Effects of Rubrics on Academic Performance, Self-Regulated Learning, and Self-Efficacy: a Meta-analytic Review*. **Educational Psychology Review**. [Springer](https://link.springer.com/article/10.1007/s10648-023-09823-4) · [PDF](https://ernestopanadero.es/Publications/Articles/081_Panadero_et_al_2023_Effects_of_Rubrics_on_Academic_Performance_Self_Regulated_Learning_and_self_Efficacy.pdf)
- Falchikov, N. y Boud, D. (1989). *Student Self-Assessment in Higher Education: A Meta-Analysis*. **Review of Educational Research**, 59(4), 395-430. [SAGE](https://journals.sagepub.com/doi/abs/10.3102/00346543059004395)
- Kluger, A. N. y DeNisi, A. (1996). *The Effects of Feedback Interventions on Performance*. **Psychological Bulletin**, 119(2), 254-284. [PDF](https://mrbartonmaths.com/resourcesnew/8.%20Research/Marking%20and%20Feedback/The%20effects%20of%20feedback%20interventions.pdf)
- Deslauriers, L., McCarty, L. S., Miller, K., Callaghan, K. y Kestin, G. (2019). *Measuring actual learning versus feeling of learning in response to being actively engaged in the classroom*. **PNAS**, 116(39), 19251-19257. [PNAS](https://www.pnas.org/doi/pdf/10.1073/pnas.1821936116) · [PubMed](https://pubmed.ncbi.nlm.nih.gov/31484770/)

**IA como correctora: adulación, sesgos de juez, y daño al aprendizaje**
- *When Truth Is Overridden: Uncovering the Internal Origins of Sycophancy in Large Language Models* (2025). arXiv:2508.02087. [HTML](https://arxiv.org/html/2508.02087v1) — 63,7 % de media, rango 46,6-95,1 %; +13,6 % con formulación en primera persona. **Aviso: modelos abiertos de 1B-8B.**
- Kim, S. W. y Khashabi, D. (2025). *Challenging the Evaluator: LLM Sycophancy Under User Rebuttal*. **EMNLP 2025 Findings**. [ACL Anthology](https://aclanthology.org/2025.findings-emnlp.1222/)
- OpenAI (2025). *Sycophancy in GPT-4o: What happened and what we're doing about it*. [openai.com](https://openai.com/index/sycophancy-in-gpt-4o/) · [Expanding on what we missed with sycophancy](https://openai.com/index/expanding-on-sycophancy/) · cobertura: [TechCrunch](https://techcrunch.com/2025/04/29/openai-explains-why-chatgpt-became-too-sycophantic)
- Huang, J., Chen, X., Mishra, S., Zheng, H. S., Yu, A., Song, X. y Zhou, D. (2024). *Large Language Models Cannot Self-Correct Reasoning Yet*. **ICLR 2024**. [arXiv](https://arxiv.org/pdf/2310.01798)
- *Self-Preference Bias in LLM-as-a-Judge* (2024). arXiv:2410.21819. [PDF](https://arxiv.org/pdf/2410.21819)
- *Justice or Prejudice? Quantifying Biases in LLM-as-a-Judge* (2024). arXiv:2410.02736. [PDF](https://arxiv.org/pdf/2410.02736) — posición, verbosidad, auto-preferencia
- Bastani, H., Bastani, O., Sungu, A., Ge, H., Kabakcı, Ö. y Mariman, R. (2025). *Generative AI without guardrails can harm learning: Evidence from high school mathematics*. **PNAS**. [PNAS](https://www.pnas.org/doi/10.1073/pnas.2422633122) · [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC12232635/) · [Knowledge@Wharton](https://knowledge.wharton.upenn.edu/article/without-guardrails-generative-ai-can-harm-education/)

---

## 11. Lo que no he podido resolver

- **Cuánto sabe de IA la pareja, y de qué tipo.** El diseño de la sección 4 asume "sabe bastante más
  que ella y puede diagnosticar un fallo de plataforma". Si en realidad su conocimiento es de
  modelos y no de Workspace, **PC-4 (el comodín técnico) pierde casi todo su valor** y habría que
  reasignar ese punto a PC-3 o a PC-5. Es la incógnita que más cambiaría esta sección.
- **Si ella acepta el encuadre de escasez.** Seis puntos es un juicio de diseño [J], no un dato. Si
  la pareja está disponible sin fricción y a ella no le pesa preguntar, el número puede subir — pero
  el **filtro de admisión de §4.2 no debería relajarse aunque suba el número**, porque el filtro es
  lo que protege la autonomía, no el número.
- **Cómo se comportan los modelos de frontera de 2026 en el escenario concreto de corregir con
  rúbrica.** Lo que hay medido es adulación de opinión y sesgos de juez en tareas de comparación de
  respuestas. **No he encontrado datos de "modelo corrigiendo un entregable de un alumno contra una
  rúbrica dada"**, que es exactamente nuestro caso. Por eso el control positivo de §3.5.3 no es un
  adorno: es la única forma de saberlo con su modelo, su rúbrica y su tipo de trabajo.
- **Si el hilo guiado de encuestas (P27) le resultará suficientemente suyo** para sostener la
  motivación, o si lo vivirá como ejercicio de libro. El doble hilo lo cubre parcialmente, pero es
  el supuesto más frágil de la sección 7.
