# Síntesis B — Diseño unificado del curso

**Qué es esto.** El diseño completo y ejecutable del curso descrito en `00-perfil.md`. No es un resumen
de las tres arquitecturas candidatas: es **un curso**, construido sobre la columna vertebral de una de
ellas e injertando deliberadamente los instrumentos de las otras dos y las correcciones que los cuatro
jueces han pedido. Donde los jueces se contradicen, decido y argumento (§17).

**Brief:** `00-perfil.md`, revisión del 22.08.2026. **Manda sobre este documento.**
**Fecha:** 23.08.2026.

**Sesgo declarado de esta síntesis, porque condiciona todas las decisiones:** ante cualquier disyuntiva,
**gana lo que consolida criterio transferible sobre lo que produce resultado rápido**. Pero con dos
restricciones que no se negocian: el curso tiene que producir cosas que funcionen en su trabajo, y ella
tiene que llegar al final. Un curso de criterio que se abandona en la semana 4 no enseña criterio: no
enseña nada.

**Marcas:** **[V]** verificado en fuente primaria · **[R]** reconstrucción razonada · **[E]** evidencia
publicada citada en los informes de dominio · **[NV]** no verificable desde fuera · **[!]** decisión que
no es suya y se escala · **[J]** juicio de diseño mío, argumentado y sin respaldo externo.

---

# 0. LA DECISIÓN DE COLUMNA VERTEBRAL, ANTES DE NADA

## 0.1 Qué dicen los jueces y qué hago con ello

| Lente | Ganadora | Nota | Lo que en realidad premia |
|---|---|---|---|
| Supervivencia / abandono | **arq-3** proceso | 8 | Que el artefacto viva en su mesa y el mundo la corrija cada martes; que el muro técnico se desactive en la semana 1; frontera declarada; compromiso externo con fecha |
| Autocorrección sin mentor | **arq-1** escalera | 8,5 | Las **puertas** con condición observable, y en particular la de uso espontáneo. Y las cinco preguntas |
| Durabilidad / portabilidad | **arq-1** escalera | 8,5 | Las **cinco preguntas** (clasificador dimensional) y el **tercer registro** (cómo reconocerlo en una herramienta que no has visto) |
| Encaje con el trabajo real | **arq-2** inventario | 8 | Que verifica el dominio contra su semana con un instrumento, y el **tratamiento multilingüe** |

Dos jueces votan arq-1, uno arq-3, uno arq-2. Y sin embargo la decisión no está reñida, porque **lo que
los jueces 2 y 3 premian en arq-1 no es su orden: son sus instrumentos**. Las cinco preguntas, las
puertas, el tercer registro y la prueba de traducción son piezas **desmontables**: se pueden atornillar a
cualquier columna vertebral sin perder nada. La ordenación por autonomía cedida, en cambio, arrastra los
defectos que su propio autor escribe: veinte semanas, cinco de diez módulos sin capacidad nueva, cuatro
de esas semanas seguidas en el tramo 11–14, el muro del buzón compartido declarado **sin resolver**, y la
frase de su autocrítica 8 —*«he elegido el diseño que se termina antes que el que enseña más»*— que, bajo
mi sesgo, es exactamente la elección que no hay que hacer.

Lo mismo pasa con arq-2: su mejor activo —los seis veredictos, la regla del cuatro, la zona prohibida y
el volumen de juicios— es **contenido**, no arquitectura, y se injerta. Lo que no se injerta es su
columna vertebral, porque su propia autocrítica 13 la desmonta mejor que cualquier juez: *«un Semanario
es un documento, y los documentos no contestan correos»*, y su MOMENTO 1 se titula *«el inventario como
muro»*.

Arq-3, en cambio, tiene lo que **no es desmontable**: un objeto en producción sobre su mesa desde la
semana 5–6, que es el único mecanismo de corrección que funciona todos los días sin gastar rúbrica, sin
gastar pareja y sin depender de su juicio sobre su propio trabajo. Eso es columna vertebral y no se puede
injertar en otra cosa.

> **DECISIÓN 1 · La columna vertebral es la de arq-3: el curso es la transformación de UN proceso suyo,
> capa a capa, hasta que funciona, hasta que lo usa sin que nadie se lo pida y hasta que sobrevive a sus
> vacaciones. Sobre ese esqueleto se atornillan las cinco preguntas de arq-1, sus puertas y su tercer
> registro; y los seis veredictos, la cuota de noes y el rigor multilingüe de arq-2.**

Coincide con la hipótesis del diseñador jefe, con dos diferencias que desarrollo en §17: **los seis
veredictos no van solo en el Doblete —van también dentro de la línea de corte, y ese es el injerto que de
verdad los rentabiliza—**, y **el volumen de juicios se recupera entero (más de treinta), pero colocando
la clasificación masiva en la semana 14 y no en la 3**.

## 0.2 Los diez injertos que definen este diseño

| # | Injerto | De dónde | Qué arregla |
|---|---|---|---|
| 1 | **Las cinco preguntas** como cabecera de la pregunta fija de cada capa | arq-1 §1.2 | El mejor clasificador portátil del corpus, y sus preguntas 4 y 5 son protección de datos incrustada |
| 2 | **Los seis veredictos** como rejilla cerrada, usada **dos veces**: dentro de su proceso (línea de corte) y fuera (dobletes) | arq-2 §3.4 | Objetivo 1 y «cuándo NO usar IA», a coste cero |
| 3 | **El tercer registro**: «cómo reconocerlo en cualquier herramienta», con sus señas | arq-1 §4.1 | El hueco que dejan dos registros: encontrar una función en una pantalla que no ha visto nunca |
| 4 | **Puertas con condición observable** entre capas, incluida la de **uso espontáneo** | arq-1 §1.6 salv. 4 | Sustituto honesto del «todavía no» de un profesor. Sin esto, la tesis del ángulo es falsa |
| 5 | **Clave sellada para los ocho dobletes** | mío, sobre arq-3 §1.6 B | El hueco que el juez 2 caza: la maquinaria de transferencia de arq-3 no tenía oráculo |
| 6 | **La rejilla de los doce**, en la semana 14 | arq-2 M1, recolocada | Recupera el volumen de juicios de arq-2 sin su muro de la semana 3, y con criterio ya adquirido |
| 7 | **El multilingüismo como resultado de aprendizaje**, no como suerte del proceso elegido | arq-2 | El fallo de encaje más serio de arq-3 según el juez 4 |
| 8 | **La columna «lo que sí se puede hacer alrededor»** en la línea de corte y en cada «no» | arq-2 M1 | Que M1 no termine en una lista de renuncias |
| 9 | **Reproducción del número ±10 %**, prueba del pasillo con cuatro comprobaciones binarias y **piloto con criterio negativo** | arq-2 M8 | Corrección del módulo peor autocorregido del curso |
| 10 | **Regla de independencia de plataforma** + **regla del embudo vacío** | arq-1 momento 2 · mía | Que ningún módulo dependa de una casilla de una consola que ella no puede ver; y que la semana 1 no pueda terminar sin proceso |

---

# 1. NOMBRE Y TESIS

## 1.1 Nombre

> # Delegar bien
> ### Un proceso tuyo, de punta a punta — y el criterio que se queda cuando cambien las herramientas

**Por qué este nombre y no otro.** No nombra ningún producto, no nombra ninguna tecnología y no nombra
un rol («AI Operator», «especialista en IA»), que el brief excluye explícitamente porque no quiere
cambiar de puesto. Nombra **la operación** —delegar— y **el objeto** —un proceso suyo—, que son las dos
cosas que van a seguir existiendo en 2029. El subtítulo hace el trabajo de expectativas: dice que el
resultado es un proceso funcionando **y** un criterio que sobrevive al cambio de herramienta, que son
literalmente los objetivos 2 y 4 del perfil.

## 1.2 Tesis

> **Se aprende a delegar delegando una cosa entera, no doce a medias. Un proceso llevado de punta a
> punta —hasta que funciona, hasta que lo usa sin que nadie se lo pida y hasta que sobrevive a sus
> vacaciones— enseña más criterio que doce diagnósticos sobre papel, porque es el único formato en el
> que cada decisión recibe la respuesta del mundo.**
>
> **Y el criterio no se deduce solo del recorrido: se extrae con un ritual, se clasifica con un
> instrumento y se prueba contra procesos que no son el suyo. El recorrido produce la experiencia; los
> tres instrumentos la convierten en algo que viaja.**

La segunda mitad es la aportación de esta síntesis y es donde se separa de arq-3 pura. Arq-3 confía en
que la pregunta fija, contestada ocho veces, destile el criterio. **No basta.** Una extracción sin
clasificador produce prosa; una extracción sin contraste externo produce generalidades. Por eso el
recorrido lleva encima:

1. **un clasificador dimensional** —las cinco preguntas— que se responde sobre cualquier sistema de
   cualquier año, incluidos los que el curso no enseña;
2. **una rejilla de decisión cerrada** —los seis veredictos— que se aplica dentro de su proceso y sobre
   más de treinta procesos ajenos;
3. **un contraste con clave** —los ocho dobletes sellados— que le dice si su juicio sobre un proceso que
   no es el suyo coincide con el correcto, que es la única forma sin profesor de saber si el criterio
   generalizó o se pegó al caso.

Cuatro corolarios operativos, que son restricciones de producción y no lemas:

> **(a) La unidad del curso es la capa, no la herramienta ni la tarea.** Un módulo se llama «Que ocurra
> sin que lo pidas», nunca «Acciones programadas» ni «Automatizar el proceso 27». El índice del curso no
> puede caducar.
>
> **(b) La teoría entra por demanda del proceso, y solo la que el proceso pide.** No hay módulo de
> panorama previo. Lo que el proceso no pide se cubre con veinte minutos en seco (el Doblete), con una
> fila de la Lista de techos, o no se cubre y se dice.
>
> **(c) El «no» vive dentro del proceso, no fuera.** El primer entregable serio no es «qué automatizo»,
> sino **la línea de corte**: el proceso partido en trozos, cada trozo con uno de los seis veredictos y
> el motivo escrito. Un proceso partido en trozos con veredicto es el sitio más barato del mundo para
> aprender que a veces la respuesta es que no.
>
> **(d) Cada capa se cierra con una puerta observable.** No se sube porque el calendario lo diga: se
> sube porque hay algo que se puede mirar y que dice que la capa anterior está agotada. Sin profesor,
> una puerta que bloquea es la única figura que se parece a un «todavía no».

## 1.3 Los dos riesgos de esta tesis, dichos con las peores palabras posibles

**Riesgo 1 — Se le pide comprometerse con un proceso en la semana 1, que es cuando menos criterio
tiene.** La conclusión peligrosa no es «esto es difícil»: es **«creo que he elegido mal y llevo dos
semanas»**, y esa es irreversible si no se anticipa. Respuesta: §5 entera —embudo con criterios de
rechazo observables, prueba de la sombra, repuesto firmado el día 3, divorcio preautorizado con
aritmética escrita, y regla del embudo vacío.

**Riesgo 2 — Un solo proceso puede no dar ocasión de practicar todo el criterio.** Si su proceso no tiene
un trozo determinista puro, nunca choca con «esto no necesita IA». Si no toca datos rojos, la lección de
datos se queda en abstracto. Si es monolingüe, el multilingüismo —que es la propiedad que define su
puesto— desaparece del curso. Respuesta: los ocho dobletes con clave, la rejilla de los doce, el
expediente modelo sobre P27 como ruta de respaldo obligatoria para las lecciones que su proceso no
active, y el multilingüismo elevado a resultado de aprendizaje con ruta alternativa escrita (§6, M2 y
M4).

---

# 2. PERFIL DE ENTRADA Y DE SALIDA

## 2.1 De dónde parte, sin adornos

| Dimensión | Estado en la semana 0 |
|---|---|
| **Uso de IA** | ChatGPT, Claude y Gemini **como chat**: entra a la web, escribe, lee, copia. No ha guardado nunca un asistente, no ha adjuntado nunca una fuente para que la cite, no ha programado nunca nada |
| **Base técnica** | Ninguna. **Nunca ha abierto una terminal**, y no va a abrirla en este curso |
| **Dominio** | **Experta.** Sabe cosas de su puesto que no están escritas en ningún sitio de la academia. Esa es la materia prima |
| **Método** | Licenciatura en Psicología: operacionalizar, diseñar instrumentos, evaluar validez, entrevistar. Transferencia FUERTE en ocho de trece correspondencias (`dominio-psicologia.md` §2) |
| **Entorno** | Gemini de pago dentro de la suite de su empresa. **No sabe qué plan ni cómo está configurado** |
| **Restricciones** | Jornada completa · autodidacta · pareja disponible para consultas puntuales, que no corrige entregas ni sigue el progreso · cero presupuesto |
| **Punto ciego declarado** | No tiene mapa de qué existe ni de qué se puede automatizar de su trabajo |
| **Riesgo de perfil** | No es quedarse corta de rigor: **es pasarse** (`dominio-psicologia.md` §6). Un solo proceso es un imán para el perfeccionismo |

**Lo que su formación NO le da, y va escrito en el material la primera vez que hace falta** (M3):
entender por qué el paso 3 de un flujo no ve lo que produjo el paso 1; tolerancia al trasteo; pensar en
datos estructurados; diagnosticar por qué falla un sistema. Sin esta mitad, la otra mitad es adulación.

## 2.2 A dónde llega

**Con un objeto en la mano:**

- **Un proceso suyo funcionando y en uso diario**, con criterio escrito, fuentes fechadas, disparador,
  tope, frenos probados, apagado probado, dueño con nombre y calendario de revisión.
- **Un número medido con su método**, con el coste de revisión restado y con una amenaza a la validez
  que no puede descartar — y reproducible dos semanas después dentro del ±10 %.
- **Una segunda persona** que ha usado su sistema **una semana entera sin ella delante**, y la lista de
  lo que ese piloto obligó a arreglar.

**Con un criterio en la cabeza, que es lo que se lleva si mañana cambia de empresa:**

- **Clasifica cualquier herramienta** —incluida una que el curso no le enseñó y una que no existe hoy—
  respondiendo cinco preguntas, y **deriva de las respuestas** qué salvaguardas necesita y qué datos no
  le puede meter.
- **Asigna a un proceso cualquiera uno de seis destinos**, dos de los cuales son «no metas IA aquí», y
  justifica el veredicto citando un hecho observable del proceso y no una impresión.
- **Escribe el criterio de «bien hecho» antes de construir**, y una batería que lo comprueba.
- **Mide si algo sirve** y sabe decir qué amenaza a la validez no ha descartado.
- **Deja lo que monta en condiciones de sobrevivirle**, y sabe explicarlo en treinta segundos sin nombrar
  ninguna herramienta, incluido lo que no hace.

**Con una posición, que es lo que pide el objetivo 5:** llega a las conversaciones de su empresa con una
cosa que funciona, un número que aguanta que lo repregunten y **una lista de lo que decidió NO
automatizar, con el motivo**. Esa lista es lo que hace que le crean el resto.

**Y con lo que expresamente NO es:** no es especialista en IA, no ha cambiado de rol, no tiene portfolio,
no tiene certificado, y no sabe programar. **Sigue siendo la persona de atención al cliente de una
academia**, haciendo su trabajo con otro método.

## 2.3 La definición observable de «terminado», fijada en la semana 1

> Un proceso suyo funcionando y en uso diario sin que el curso se lo pida · un número medido con su
> método y reproducido · **ocho preguntas fijas contestadas con sus dos mitades** · **ocho dobletes
> firmados, de los cuales al menos tres terminan en «no aplica», contrastados contra su clave** · doce
> procesos clasificados con la rejilla · una rúbrica escrita por ella y validada contra un cebo · y una
> segunda persona que ha usado su sistema una semana sin ella.

No es «leer la última lección». Y la rúbrica escrita por ella es el indicador honesto de que ya no
necesita el material.

---

# 3. RESULTADOS DE APRENDIZAJE OBSERVABLES

Verbos de desempeño. Cada uno con su evidencia observable y el módulo donde se cierra. Ninguno dice
«entenderá», «conocerá» ni «será capaz de valorar».

| # | Al terminar, ella… | Evidencia observable | Cierra en |
|---|---|---|---|
| **RA1** | **Elige** un proceso propio aplicando criterios de rechazo observables y **descarta** por escrito los que no pasan, con el motivo transferible y no con el número de proceso | Hoja de elección: 6–8 candidatos puntuados en cinco columnas, seis descartes con **motivo escrito**, hoja de sombra de dos días, repuesto firmado con fecha | M0 |
| **RA2** | **Describe** un proceso suyo como se ejecuta de verdad —disparador, documentos, decisiones no escritas, salida—, **por observación y no de memoria** | La descripción contiene **al menos dos decisiones que no estaban en su idea previa**. Si no las contiene, se escribió de memoria y se vuelve a observar | M0 |
| **RA3** | **Determina** bajo qué régimen de datos trabaja —entrenamiento, retención, ubicación, contrato, política interna— **o documenta** a quién y cuándo lo preguntó | Ficha del entorno, ocho casillas, **ninguna frase que empiece por «creo que»**. *«Pregunté a X el día D y no obtuve respuesta»* es un resultado válido | M0 |
| **RA4** | **Clasifica** cualquier sistema —incluido uno que el curso no le ha enseñado— respondiendo **las cinco preguntas**, y **deriva** de esas respuestas qué salvaguardas necesita y qué datos no puede meterle | Ficha de cinco preguntas rellenada para: su chat de hoy (M0), cada capa (M1–M6) y **una herramienta que el curso no enseñó** (M4) | M0 → M4 |
| **RA5** | **Traza la línea de corte** de su proceso: cada trozo con **uno de los seis veredictos** y con el motivo, y para cada «no» **qué sí se puede hacer alrededor** | Al menos un trozo se queda con ella; ningún motivo es «es difícil»; cada «no» tiene un artefacto **nombrable** en la casilla de al lado | M1 |
| **RA6** | **Escribe** el criterio de «resultado correcto» en 4–6 indicadores que otra persona pueda comprobar sí/no contra una fuente, **antes** de tocar ninguna herramienta | Ficha de criterio de una cara, sin *adecuado, correcto, natural, profesional, de calidad* sin ancla detrás; **al menos un indicador verificable contra fuente externa**; no todos marcados como críticos | M1 |
| **RA7** | **Construye** una batería de diez casos —5 típicos, 3 límite, 2 de rechazo— apartados **antes** de escribir el prompt, con **al menos uno en un idioma minoritario real de su buzón**, y **la vuelve a pasar con fecha** en cada capa | La Tira: cinco columnas fechadas al terminar. Clave sellada escrita el mismo día | M1 → M5 |
| **RA8** | **Sitúa** cada dato que atraviesa su proceso en verde/ámbar/rojo, **marca en qué paso entra y en cuál hay que quitarlo, y quién lo quita**, y **reescribe** casos reales que sobreviven a la prueba de la compañera | Mapa de datos del proceso, una cara, cuatro columnas; tres casos reescritos que **siguen produciendo una respuesta útil** y uno declarado no reescribible | M2 |
| **RA9** | **Monta** un asistente con fuentes propias fechadas que **cita el documento y su fecha** y **dice «no lo sé»** cuando la respuesta no está | 5/5 en los típicos, pide aclaración en los 3 límite (inventar es fallo aunque acierte), «no lo sé» en los 2 de rechazo (acertar es suspenso) | M2 |
| **RA10** | **Reconstruye** una capa suya en otra herramienta **en menos de veinte minutos** y **nombra** qué viajó tal cual, qué hubo que rehacer y qué techo cambió | Ficha de traslado con las tres columnas rellenas con cosas concretas. *Si no lo consigue en veinte minutos: aprendió la ruta, no la capacidad, y ese diagnóstico llega a tiempo* | M2 |
| **RA11** | **Monta** algo con disparador que **prepara, clasifica o avisa y nunca envía**, con tope, y **lo apaga habiéndolo probado** | Cinco casos fabricados disparan y producen las cinco salidas correctas; **un sexto que NO debe disparar no dispara**; el tope se prueba con un lote grande; el apagado está hecho, no imaginado | M3 |
| **RA12** | **Escribe su flujo en notación neutra** —DISPARADOR → PASO → CONDICIÓN → SALIDA— y **localiza cada pieza en la documentación de otra plataforma que no ha usado**, sin dar de alta ninguna cuenta | Tres líneas: las cinco piezas y su nombre allí · la pieza que allí no existe · la pieza que allí es más fácil | M3 |
| **RA13** | **Distingue** en su proceso qué parte tiene pasos fijos y qué parte necesita juicio, y **argumenta por qué un agente autónomo sería exceso aquí** | Media página con la frontera trazada y los dos puntos de juicio nombrados, cada uno con su criterio escrito | M4 |
| **RA14** | **Escribe** los temas prohibidos y las condiciones de parada de su sistema —incluida **la parada por idioma no probado**— y **las prueba con casos fabricados que deben parar** | Cinco casos de parada, cinco paradas observadas, cada una con marca visible y motivo en una línea; **un sexto caso normal que NO para**; la respuesta a «quién revisa» es **un nombre y una hora** | M4 |
| **RA15** | **Reconoce** cuál es el único proceso de su academia que caería en el Anexo III del Reglamento de IA y **a quién lo escala** | Una frase, un nombre, un puesto. Y el verdadero/falso de doce ítems con ≥10 aciertos | M4 |
| **RA16** | **Audita a su propio corrector**: detecta los defectos plantados de tres artefactos-cebo repartidos en el curso y **decide con ese dato** si la IA sirve para corregir ese tipo de trabajo | Hoja de resultado de los tres cebos + decisión escrita + **al menos un caso registrado en que NO aceptó una crítica de la IA, con el motivo** | M1, M4, M6 |
| **RA17** | **Mide** el efecto de su sistema en **minutos por unidad**, **resta** revisión y mantenimiento, **nombra** una amenaza a la validez que no puede descartar, y **reproduce el número** dos semanas después | Media página sin la palabra «significativo», con la resta hecha; el recálculo cae dentro del **±10 %** o el dossier se reescribe | M5, M7 |
| **RA18** | **Deja el sistema en condiciones de sobrevivirle**: fuentes con fecha y dueño, calendario de revisión, apagado probado, ficha de traspaso | «Quién lo mantiene» responde con un nombre propio; «cuándo caduca cada fuente» responde con una fecha; la prueba del hueco está hecha | M6 |
| **RA19** | **Asigna uno de los seis veredictos a doce procesos suyos**, justificando cada uno con un **hecho observable** del proceso, y **al menos cuatro** terminan en «ni IA», «arreglar el proceso primero» o zona prohibida, cada uno con su «lo que sí alrededor» | La rejilla de los doce, firmada y fechada; ninguna justificación es una impresión | M6 |
| **RA20** | **Escribe la rúbrica** de un artefacto suyo, con ≥3 criterios negativos que exigen salida escrita, y **la valida contra un cebo** | Si el cebo pasa su rúbrica, la rúbrica es blanda y se rehace | M6 |
| **RA21** | **Entrega** su artefacto a otra persona, que lo usa **una semana laborable sin ella**, y **corrige** lo que el piloto revele | Ficha de traspaso + **lista de al menos dos cosas que hubo que arreglar**. *Si el piloto no reveló nada, no fue un piloto* | M7 |
| **RA22** | **Explica** en treinta segundos, **sin nombrar ninguna herramienta**, qué hace su sistema, qué ahorra y **qué no hace** | La prueba del pasillo, con sus cuatro comprobaciones binarias, ante alguien que no ha visto el artefacto | M7 |
| **RA23** | **Contesta la pregunta fija** al cerrar cada capa, con sus dos mitades obligatorias, y **firma ocho dobletes** de los cuales **al menos tres son «no aplica»**, contrastándolos después contra la clave sellada del curso | Cuaderno de capas: ocho fichas con las seis casillas rellenas + ocho dobletes con veredicto y con la comparación contra clave anotada | todos |

**Los tres resultados que hacen falsable la agnosticidad, y su condición de fracaso escrita:**

> Si al terminar no puede **rellenar la ficha de cinco preguntas para una herramienta que el curso no le
> enseñó** (RA4), **reproducir una capa en otro sitio en veinte minutos** (RA10) y **localizar las piezas
> de su flujo en la documentación de una plataforma que no ha visto** (RA12), entonces **este fue un
> curso de una herramienta y fracasó**, por muy bien que hayan salido los demás resultados.

---

# 4. LOS INSTRUMENTOS PERMANENTES

Seis. Van antes del mapa de módulos porque todos los módulos cuelgan de ellos, y porque **son lo que
queda cuando el curso se acaba y cuando las herramientas cambien**. Los seis cumplen las mismas cuatro
condiciones, y esas condiciones son el motivo de que sean **estos** y no otros:

1. **Contestan una pregunta permanente**, no una pregunta de 2026.
2. **No nombran ningún producto** (salvo una línea aislada y fechada, cuando hace falta).
3. **Tienen comprobación mecánica**: se puede saber en diez segundos si están bien rellenados.
4. **Los escribe ella.** Un fichero copiado no se relee; uno escrito, sí.

## 4.1 La ficha de las cinco preguntas — el clasificador

*(injerto de arq-1 §1.2, y es el instrumento más portátil de todo el corpus)*

| # | Pregunta | Respuestas, de menos a más autonomía cedida |
|---|---|---|
| **1** | **¿Quién dispara?** | yo, cada vez · un reloj · un suceso · lo decide el sistema |
| **2** | **¿Quién decide los pasos?** | yo, sobre la marcha · yo, de antemano, y quedan fijos · el sistema, sobre la marcha |
| **3** | **¿De dónde saca lo que sabe?** | de lo que le pego en el momento · de fuentes que yo controlo y fecho · de donde quiera |
| **4** | **¿Qué puede tocar?** | nada · leer lo que yo le doy · leer todo lo que yo puedo leer · escribir en lo mío · escribir hacia fuera |
| **5** | **¿Quién firma la salida?** | yo, siempre · yo, por muestreo · nadie |

**Por qué estas cinco y por qué son el instrumento número uno de este curso.** Porque clasifican por
**una propiedad** —cuánta autonomía has cedido— y no por un destino de producto. Un catálogo de
soluciones es una foto del mercado de este año; una dimensión se responde igual sobre algo que todavía no
existe. Y porque **las preguntas 4 y 5 son, literalmente, protección de datos y salvaguardas**: por eso
en este curso el bloque de datos no va pegado al final, va dentro del instrumento con el que se clasifica
cualquier cosa.

**Dónde vive.** Encabeza **la pregunta fija de cada capa**. Al cerrar cada capa, se rellenan las cinco
filas de nuevo. **Casi siempre cambia una sola fila, y ver cuál cambia es la lección**:

```
                      M0 chat  →  M1 criterio  →  M2 fuentes  →  M3 disparador  →  M4 juicio
1 ¿Quién dispara?        yo          yo             yo            un suceso ←      un suceso
2 ¿Quién decide pasos?   yo          yo             yo            yo, de antemano  yo, salvo 2 puntos ←
3 ¿De dónde sabe?     lo que pego  lo que pego   fuentes mías ←   fuentes mías     fuentes mías
4 ¿Qué puede tocar?      nada        nada        leer lo mío ←    leer lo mío      escribir en lo mío ←
5 ¿Quién firma?          yo          yo             yo               yo               yo  ← nunca cambia
```

**La fila 5 no cambia en todo el curso, y eso es contenido, no casualidad.** Es la regla que atraviesa el
diseño entero: *automatiza la lectura y la preparación; la escritura hacia fuera la firma una persona*.

**Uso terminal (M4):** rellenar la ficha para **una herramienta que el curso no ha enseñado**, elegida
por ella entre lo que le llegue por cualquier vía, y contestar tres cosas: qué escalón es, qué
salvaguardas necesitaría, qué datos no le podría meter. Ese ejercicio es la prueba de que el instrumento
funciona **sin el curso**.

**Comprobación mecánica:** ¿están las cinco filas rellenadas con una de las opciones de la escala y no
con una frase libre? ¿Ha cambiado alguna fila respecto a la capa anterior? *Si no ha cambiado ninguna,
esa capa no te ha dado nada, y merece la pena saberlo.*

## 4.2 La rejilla de los seis veredictos — el decisor

*(injerto de arq-2 §3.4, y es el mecanismo que cubre a la vez el objetivo 1 y «cuándo NO usar IA»)*

| # | Veredicto | La prueba que lo decide (sobre la TAREA, no sobre la herramienta) | Ejemplos de su casa |
|---|---|---|---|
| **1** | **NI IA** | **La servilleta:** ¿podrías escribir los pasos en una servilleta y valdrían siempre? Entonces necesitas una fórmula, una plantilla o un calendario | **P02** presupuestos (aritmética sobre una tabla) · **P22** camas (calendario de recursos) |
| **2** | **ARREGLAR EL PROCESO PRIMERO** | La respuesta a «¿de qué documento sale este dato?» es «pregunto a alguien», «el de siempre», o hay dos versiones y nadie sabe cuál manda | **P32** plantillas en seis idiomas sin control de versiones · cualquier tarea cuyo tarifario vigente ella no pueda nombrar con su fecha |
| **3** | **CHAT, MEJOR USADO** | Poca frecuencia + mucho juicio + conocimiento que no se repite | **P13** cambios de grupo · **P31** el comentario del informe mensual |
| **4** | **ASISTENTE GUARDADO CON FUENTES** | Se repite, el conocimiento está escrito y es estable, el juicio sigue siendo suyo | **P01** las seis preguntas que repite el 70–80 % de los leads · **P10** certificados |
| **5** | **DISPARADOR Y PASOS FIJOS** | Hay un disparador identificable **y** los pasos son siempre los mismos | **P27** encuestas · **P30** parte semanal · **P06** recordatorio de pagos |
| **6** | **FLUJO CON JUICIO** | Hay disparador, pero en dos o tres puntos hay que **evaluar** algo para saber por dónde seguir | **P28** triaje de reseñas · **P20** clasificar y enrutar incidencias (nunca responderlas) |
| **ZP** | **ZONA PROHIBIDA** — no es un veredicto: es un tachón encima del que hubiera | El peor error cuesta dinero, un plazo legal o un visado; **o** hay un dato rojo irreducible | **P08** visados · **P26** quejas · **P29** emergencias · **P25** reembolsos · **P17** matching · **P22** overbooking |

**Las tres decisiones que hacen que esta rejilla valga y no sea un catálogo disfrazado:**

- **El veredicto 1 va el primero, no al final como advertencia.** «No hace falta IA» es un **destino**,
  no un fracaso. Y el ejemplo canónico es suyo: el presupuesto es aritmética sobre una tabla de precios,
  y meter un modelo de lenguaje ahí **no es ineficiente: es introducir un error posible donde no lo
  había**.
- **El veredicto 2 tiene nombre propio y casilla propia, y es el que más le va a salir.** No existe en
  ningún curso de IA. Y es un **hallazgo que aportar, no un fracaso**: en una empresa donde lo mal visto
  es no automatizar, llegar diciendo *«esto todavía no se puede automatizar porque nadie sabe cuál es el
  tarifario vigente en alemán»* es trabajo de valor.
- **El agente autónomo NO está en la lista de destinos.** Se define, se explica y se le pone su condición
  de activación en M4, pero no es una opción que ella pueda elegir para una tarea suya, y se dice con
  todas las letras. El motivo es pedagógico y verificable: el error número uno al clasificar es poner
  «agente» a todo, porque es la palabra que suena a solución completa y es lo que promete internet.
  Sacarlo obliga a decidir entre lo que sí existe para ella.

**Dónde se usa — y este es el injerto que la rentabiliza, porque arq-2 la usaba una vez y aquí se usa
tres:**

| Momento | Sobre qué | Cuántos juicios |
|---|---|---|
| **M0**, día 3 | Los seis descartes automáticos: escribir el **motivo transferible** de cada zona prohibida, no el número | 6 |
| **M1**, línea de corte | **Los trozos de su propio proceso.** Cada trozo recibe un veredicto | 4–6 |
| **M1–M7**, dobletes | Ocho procesos que no son el suyo, **con clave sellada** | 8 |
| **M6**, la rejilla de los doce | Doce procesos suyos, ya con criterio | 12 |
| **M7**, segunda vuelta | Releer los doce y marcar qué veredictos han cambiado y por qué | ~4 revisados |

**Total: más de treinta juicios sobre procesos reales**, que es exactamente el número que hace de esto una
operación entrenada y no una definición leída — y es el mecanismo que el juez 3 reclamaba, conseguido sin
el Semanario de once columnas de la semana 3.

**Comprobación mecánica:** ¿cada veredicto cita un hecho observable del proceso (un volumen, un
documento, una consecuencia) y no una impresión? ¿Hay al menos cuatro noes de doce? ¿Cada «no» tiene un
artefacto **nombrable** en la casilla «lo que sí alrededor»?

## 4.3 La Tira — el medidor

Diez casos escritos en M1 y **nunca cambiados**, pasados al cerrar cada capa, en una hoja con una columna
nueva y **fechada** por capa.

```
CASO                          | como lo hago hoy | +criterio | +fuentes | +disparador | +frenos
                              | 13-oct           | 27-oct    | 10-nov   | 24-nov      | 15-dic
------------------------------|------------------|-----------|----------|-------------|--------
T1  típico, en español        |  SÍ              |   SÍ      |   SÍ     |    SÍ       |   SÍ
T2  típico, en inglés         |  NO              |   SÍ      |   SÍ     |    SÍ       |   SÍ
T3  típico, en neerlandés  ←  |  NO              |   NO      |   SÍ     |    SÍ       |   SÍ
...
L1  ambiguo: dos categorías   |  inventa         |  inventa  | pregunta |  pregunta   | pregunta
L2  queja educada indirecta   |  inventa         |  inventa  | inventa  |  pregunta   | pregunta
R1  fuera de alcance          |  responde        | no lo sé  | no lo sé |  no lo sé   |  PARAR
R2  menciona salud            |  responde        | responde  | no lo sé |   PARAR     |  PARAR
                              |                  |           |          |             |
MINUTOS POR UNIDAD            |   14             |   11      |    6     |     4       |    4
QUIÉN DISPARA                 |   yo             |   yo      |   yo     |  el suceso  | el suceso
```

**La lección central del curso no se cuenta: se lee en su propia hoja.**

> Entre la tercera y la quinta columna **la calidad apenas se mueve**. Casi toda la calidad se gana en la
> capa 1 y la capa 2 —cuando alguien escribe qué es hacerlo bien y le da fuentes con fecha— y a partir de
> ahí solo se puede perder. Lo que cambia al añadir capas no es la calidad: es **quién dispara, cuánto
> tarda y cuánta autonomía has cedido**.

Si dentro de tres años le ponen delante una herramienta que no existe hoy, la pregunta que sabrá hacer es
*«¿esto me cambia la calidad o me cambia el disparador?»*. Y no se la habrá contado nadie: la habrá
deducido de cinco columnas de su propio trabajo.

**Tres reglas que la sostienen:**
1. **Los casos se escriben ANTES de construir nada**, por muestreo cronológico y no elegidos. Si se
   escriben después, se escriben para que pasen. Es preregistro y se le nombra así.
2. **La clave va sellada** en un fichero aparte escrito el mismo día, que no se reabre hasta anotar los
   resultados de cada pasada.
3. **Al menos un caso típico y un caso límite están en un idioma minoritario real de su buzón** —
   neerlandés, turco, coreano, polaco—, **no en inglés, que es el fácil**. Es la salvaguarda multilingüe
   convertida en instrumento (§6, M1).

**Riesgo de este instrumento, dicho aquí:** es trabajo sin novedad, media hora cada tres semanas, y lo
que no tiene novedad se convierte en ritual o desaparece. Contramedida: **cerrar módulo sin la columna
nueva no está permitido** — es un ítem binario de la puerta, no un consejo. Aun así es el punto frágil
que reconozco en §17.3.

## 4.4 El Cuaderno de capas — el extractor de criterio

Un fichero, ocho entradas de una cara. Cada entrada tiene tres bloques: **la ficha de las cinco
preguntas** (§4.1), **la pregunta fija** y **el doblete** (§9.2).

```
CAPA __ · fecha ____

A · LAS CINCO PREGUNTAS      (las cinco filas, y cuál ha cambiado respecto a la capa anterior)

B · LA PREGUNTA FIJA
1. PROCESO      Vale para cualquier proceso la parte de: __________
                Era de ESTE proceso la parte de: __________
2. HERRAMIENTA  Valdría con cualquier herramienta la parte de: __________
                Era de ESTA herramienta la parte de: __________
3. TECHO        Esta capa NO PUEDE: __________
                Lo que lo rompería sería una cosa del tipo: __________
4. EN MI SEMANA ¿Qué OTRAS tareas mías pedirían esta misma capa? (con su número de proceso)
5. CUÁNDO NO    La situación en la que esta capa es exceso, y qué usar en su lugar

C · EL DOBLETE               (§9.2, con su veredicto de los seis, y la clave abierta después)
```

**La regla de las dos mitades, que es lo que lo hace autocorregible:** cada respuesta del bloque B tiene
una mitad positiva y una negativa, **y las dos son obligatorias**. Si escribe que todo vale para todo, no
ha separado nada: ha resumido. Si escribe que nada vale fuera de aquí, tampoco.

**Los campos 4 y 5 son injerto de la ficha de capacidad de arq-2** (§3.2, campos 2 y 5), y están aquí por
la razón que da el juez 1: son **el parche más barato contra el monocultivo**. Sin ellos, un curso de un
solo proceso nunca obliga a conectar la capa con el resto de su semana. Con ellos, cada capa produce dos
o tres candidatos para después del curso, y esos candidatos son la materia prima de la rejilla de los
doce en M6.

**Comprobación mecánica, diez segundos:**
- ¿Están rellenas **las seis** casillas del bloque B? SÍ/NO
- ¿Aparece algún nombre de producto fuera de la línea de techo? SÍ/NO
- ¿El techo dice algo que **la capa no puede hacer**, y no algo que **ella todavía no sabe hacer**?
  SÍ/NO *(injerto de arq-2: es el error más común al escribir un techo, y es el que invalida el
  instrumento entero como criterio)*
- ¿El campo 4 cita al menos un número de proceso? SÍ/NO
- ¿El doblete tiene veredicto firmado **y** la comparación contra clave anotada? SÍ/NO
- Al cerrar el curso: ¿hay **al menos tres** dobletes con veredicto «no aplica»? SÍ/NO

## 4.5 La Lista de techos — el catálogo, generado por el propio recorrido

No se lee: **se escribe**, una fila al cerrar cada capa, a partir del campo 3 de la pregunta fija. Tres
columnas, y la tercera es la que convierte un catálogo en criterio.

| Lo que esta capa no puede hacer | La clase de cosa que sí podría | **Qué tendría que cambiar para que me tocara** |
|---|---|---|
| Un asistente guardado recuerda sus instrucciones, **no recuerda lo que pasó ayer** | Un sistema con memoria persistente y auditable | Que necesitara continuidad entre sesiones **y** pudiera comprobar qué recuerda. Hoy no puedo auditarlo, así que no me fío |
| Un disparador por reloj **no reacciona a que haya pasado algo** | Un disparador por suceso | Nada: eso es la capa siguiente. *(Esta fila se tacha en la capa 3, y tacharla es el ejercicio)* |
| Mi automatización **no puede actuar sobre recursos que no son míos** | Un permiso delegado, o una plataforma de automatización externa | Que alguien me delegue una etiqueta o carpeta propia dentro del recurso compartido, **o** que el flujo tenga que tocar algo fuera de esta suite |
| Un flujo con juicio **sigue siendo un camino que dibujé yo** | Un agente: le das objetivo y límites y él decide los pasos | Que aparezca una tarea cuyos pasos no pueda dibujar de antemano **y** que exista un plan que lo incluya **y** que los datos lo permitan. Hoy fallan las tres |
| Nada de lo mío **puede procesar decenas de ficheros locales de golpe** | Un agente con acceso al sistema de ficheros | Una tarea repetida del tipo «revisar 200 contratos de estancia larga buscando una cláusula» |

**Cuatro propiedades que hacen que esto no muera:** la tercera columna son **condiciones**, y las
condiciones no se renombran · cada fila se escribe **cuando el proceso choca con el techo**, no en un
módulo de panorama —la fila del agente se escribe en la capa 4, cuando ya tiene un sistema con juicio y
entiende exactamente qué le falta— · **la escribe ella** · y **tachar una fila con fecha es un
ejercicio**, cuando la capa siguiente rompe el techo anterior. La lista se lee, al final, como el registro
de por dónde ha ido subiendo.

## 4.6 El Expediente del proceso — el objeto que el curso transforma

Una carpeta con el nombre del proceso. **No es documentación: es el sitio donde el proceso vive.** Cada
capa deja dentro exactamente una cosa, y esa lista es el índice del curso.

```
expediente-<mi-proceso>/
  00-como-se-hace-de-verdad.md      ← capa 0: disparador, documentos, decisiones no escritas, salida
  00-hoja-de-sombra.md              ← capa 0: los dos días de observación, en crudo
  01-linea-de-corte.md              ← capa 1: cada trozo con veredicto, motivo y «lo que sí alrededor»
  01-ficha-de-criterio.md           ← capa 1: 4-6 indicadores observables, críticos marcados
  01-casos.md  +  01-CLAVE.md       ← capa 1: la batería, y su clave SELLADA
  02-mapa-de-datos.md               ← capa 2: qué dato entra, en qué paso, dónde se quita y quién
  02-fuentes/                       ← capa 2: cada fuente con FECHA y DUEÑO en la primera línea
  03-disparador.md                  ← capa 3: qué lo lanza, con qué tope, cómo se apaga
  04-frenos.md                      ← capa 4: temas prohibidos, condiciones de parada, quién revisa
  05-evaluacion.md                  ← capa 5: antes, después, coste completo, amenaza no descartada
  06-traspaso.md                    ← capa 6: dueño, caducidades, calendario, apagado probado
  la-tira.md                        ← la batería pasada en cada capa, una columna fechada
  cuaderno-de-capas.md              ← 8 fichas: cinco preguntas + pregunta fija + doblete
  lista-de-techos.md
  evidencias.md                     ← 3 líneas por capa, para M7
```

**Regla de la primera línea**, que aparece en la capa 2 y no se abandona nunca: todo fichero de
`02-fuentes/` empieza con dos datos, **de cuándo es** y **quién manda sobre él**. Sin eso, un cuaderno con
las condiciones de cancelación del año pasado responde con las del año pasado, **con toda la confianza del
mundo y citando el documento**. La cita no protege de eso; la fecha, sí.

**El Cuaderno de evidencias vive dentro** (`evidencias.md`) y son tres líneas al cerrar cada capa, el día
que el artefacto empieza a funcionar. Coste: dos minutos.

```
CAPA __ · fecha ______
- Qué hacía yo antes, y cuántos minutos por unidad:
- Qué hace ahora, y cuántos minutos por unidad:
- Qué NO hace, y qué sigo haciendo yo:
```

Existe desde la semana 3 por una razón operativa y no ceremonial: **si M7 tuviera que fabricar las
pruebas al final, las inventaría.** Un número reconstruido de memoria en la semana 16 no es un número. Y
la tercera línea —*qué NO hace*— es la que después hace creíble todo el dossier: quien enumera los
límites de su propio sistema se gana el derecho a que le crean el resto.

---

# 5. EL PROYECTO HILO

## 5.1 Qué es y qué no es

**Es un proceso real de su puesto**, elegido en la semana 1 con un filtro observable, y llevado durante
dieciocho semanas hasta que funciona, hasta que lo usa a diario sin que el curso se lo pida y hasta que
otra persona lo usa una semana sin ella.

**No es un ejercicio.** El trabajo del curso es trabajo del puesto. Eso no es una comodidad: es la
contramedida estructural a la primera causa documentada de abandono —21 de 34 abandonos mencionan el
tiempo [E, Eriksson et al., *«Time is the bottleneck»*]—. Y por eso **el material declara en cada sesión
si es tiempo propio o tiempo de trabajo**: sin esa distinción escrita, ella lo contabilizará todo como
tiempo propio y el curso parecerá el doble de caro de lo que es.

**No es el proceso que más le duele.** El más doloroso es el más complejo y el más arriesgado: en su
puesto es el matching de alojamiento (P17) o la hoja de camas (P22), es decir, categorías especiales del
RGPD y riesgo crítico de overbooking. **El proceso más doloroso es el segundo proyecto, y eso va
escrito** en la semana 1 para que la renuncia no se lea como una limitación del curso.

## 5.2 El embudo de elección — noventa minutos, días 2 y 3

| Paso | Duración | Qué hace | Por qué así |
|---|---|---|---|
| 1 | 20 min | Recibe **la lista de los 32 procesos ya escrita**. Tacha los que en su academia no ocurren o no lleva ella; corrige los volúmenes; añade lo que falte; marca con un palote los que ha hecho **esta semana** | Reconocer es mucho más barato que recordar. Una hoja en blanco delante de alguien cansado produce ocho filas y abandono; una lista de 32 para corregir produce veinticinco filas en veinte minutos. **Y cada tachadura es verificación del dominio contra su realidad** |
| 2 | 15 min | **Descarte de los seis**, y aquí la variante importante: no se descartan por número, **se descartan escribiendo el motivo transferible** de cada uno | Un descarte por número es aritmética y no enseña nada. Un descarte con motivo escrito son **seis juicios** y es la primera aplicación de la zona prohibida. La lista de motivos correctos está en §9.3 y se abre **después** |
| 3 | 10 min | **Regla estacional:** *«si no lo hago en enero, no vale»* | Protege contra montar el curso sobre julio y practicarlo en temporada baja. Su volumen se multiplica por tres entre febrero y julio |
| 4 | 20 min | Puntúa los 6–8 supervivientes en **cinco columnas observables** (abajo) | Ninguna columna admite «depende» |
| 5 | 40 min en 2 días | **La prueba de la sombra** (§5.3) | Es donde se cae la elección equivocada |
| 6 | 10 min | Nombra el **proceso de repuesto** y firma la fecha | El repuesto existe desde el día 3, no desde la crisis |

**Las cinco columnas, y las cinco son observables:**

| Columna | +2 | 0 | −3 (descalifica) |
|---|---|---|---|
| ¿Cuántas veces esta semana? | 5 o más | 1–4 | 0 |
| Datos que toca (semáforo) | solo verde | ámbar seudonimizable | **rojo irreducible** |
| Consecuencia del peor error | interna, se arregla | molesta a un cliente | **dinero, plazo legal o visado** |
| **¿Sobre qué puedo actuar yo?** — ¿los ficheros y buzones que abro son míos, o son de todos? | **míos** | **una copia mía sirve** | **solo existen en un recurso compartido** |
| ¿Sé cómo se hace bien? | perfectamente | más o menos | depende de otra persona |

**+1 de desempate: si el proceso ocurre en tres o más idiomas.** Es un desempate, no un requisito, y su
motivo está en §6, M2: el multilingüismo es la propiedad que distingue su puesto de cualquier pyme, y si
el hilo lo tiene, la lección cae sobre material suyo en vez de sobre el expediente modelo.

> **La cuarta columna, y por qué está redactada así.** Es la mejor decisión de diseño de arq-3 y el juez 3
> pedía **no** injertarla, porque en su formulación original —*«los ficheros que abro, ¿son míos o
> compartidos?»*, con su −3— codifica un límite concreto de un producto de 2026 dentro de la mitad de
> criterio del curso, en la decisión número uno de la semana 1.
>
> **Tiene razón en el diagnóstico y se equivoca en el remedio, y la solución es reformularla.** La
> pregunta durable no es de producto: es **la pregunta 4 de las cinco preguntas, hecha sobre su propia
> cuenta antes de construir nada** — *¿sobre qué recursos puedo yo actuar, no mirar, sin pedirle permiso a
> nadie?* Los permisos sobre recursos compartidos acotan **cualquier** plataforma de automatización de
> cualquier año; lo que caduca es el límite numérico concreto, y ese vive en el fichero de clics y en
> `datos-volatiles.md`.
>
> Con esa redacción se conserva lo que los jueces 1 y 4 consideran la mejor decisión del corpus —cobrar
> el muro del buzón compartido en la semana 1, cuando descartar cuesta diez minutos, en vez de en la
> semana 9, cuando la conclusión que saca es *«esta herramienta no sirve para mi trabajo»*— sin meter un
> bug de 2026 en la mitad que no debe caducar. Y de paso, la primera vez que usa el instrumento número
> uno del curso, lo usa **sobre sí misma**.

## 5.3 La prueba de la sombra — dos días laborables, tres minutos al día

Antes de comprometerse, durante dos días, **cada vez que ejecuta el proceso candidato anota tres cosas**:
cuántos minutos ha tardado, qué documento ha abierto, y **qué decisión ha tomado que no estaba escrita en
ninguna parte**.

**Tres criterios de rechazo, ninguno de opinión:**

| Lo que ve en la hoja | Qué significa | Veredicto |
|---|---|---|
| **En dos días no lo ha ejecutado ni una vez** | No es tan frecuente como cree. La frecuencia percibida y la real no coinciden casi nunca | **Descartado.** Pasa al siguiente |
| **No ha abierto ningún documento** | No hay contexto que dar: es juicio puro. Un asistente con fuentes no tiene qué morder | **Descartado.** Este proceso es «chat mejor usado» (veredicto 3) y ahí se queda |
| **Las decisiones no escritas son cada vez distintas** | No es un proceso: es una serie de casos | **Descartado**, o se acota al trozo que sí se repite |

**No cuesta tiempo extra: se hace mientras trabaja.** Y la hoja de sombra es ya la primera versión de la
descripción de la capa 0, más la **línea base** que M5 va a necesitar —medida **antes** de construir nada,
que es lo que la hace honesta.

> **Nota metodológica que va en el material, porque es su casa.** Esto es muestreo de eventos, no
> introspección. *La gente describe sus procedimientos como cree que deberían ser, no como los ejecuta*
> (`dominio-psicologia.md` C9), y los atajos y excepciones —que son justo lo que rompe una
> automatización— no se verbalizan espontáneamente. Por eso no se pregunta: se observa. Y por eso el
> tercer campo es el que más rinde: **es el inventario de todo lo que un sistema no sabría hacer**.

**El hallazgo a las 48 horas, prometido por escrito** *(injerto de arq-2, momento 1 punto 5)*. El material
predice lo que la observación va a revelar, antes de que ocurra:

> *«En estos dos días vas a descubrir dos cosas incómodas. La primera: que este proceso lo haces menos
> veces de las que crees, o bastantes más. La segunda: que has tomado tres o cuatro decisiones que no
> están escritas en ningún sitio de la academia y que solo sabes tú. Eso no es un fallo del ejercicio:
> es el activo del curso. Es lo que ninguna herramienta puede darte hecho, y es la razón por la que este
> curso lo puedes hacer tú y no un informático. Anótalo como el primer hallazgo, en el Cuaderno de
> evidencias.»*

Sin esta caja, los dos días de sombra son un peaje dentro del tramo de máxima mortalidad. Con ella, son
un pago.

## 5.4 La regla del embudo vacío — el hueco que ninguna arquitectura cubría

El juez 1 lo caza y tiene razón: exigir ≥5 ejecuciones semanales, solo datos verdes, actuación sobre
recursos propios y «sé hacerlo perfectamente» **puede descartar casi todo lo que ella hace**, porque el
centro de gravedad de su puesto vive en `info@`. Si el día 3 no sobreviven al menos dos candidatos, el
material trae la escalera de relajación, **en este orden y por escrito**:

| Orden | Qué se relaja | Qué se paga a cambio |
|---|---|---|
| 1 | La cuarta columna acepta **«una copia mía sirve»** como suficiente (0, no −3) | Se abre una fila en la línea de corte: *«mantener la copia al día son N minutos por semana y ese coste se resta en M5»*. El coste no desaparece: se hace visible |
| 2 | La frecuencia baja de **≥5 por semana a ≥1 por semana**, si el proceso tarda más de 15 minutos por ejecución | La Tira tendrá menos pasadas. Se compensa pasando la batería también sobre casos históricos |
| 3 | Se **parte un proceso grande** y se toma el trozo que sí califica | La línea de corte de M1 se hace más importante, no menos: ya viene medio hecha |
| 4 | Se adopta **P27 (análisis de las encuestas de satisfacción)** como proceso propio | Es el expediente modelo: pierde el efecto sorpresa de las claves selladas, y a cambio gana el mejor primer proyecto que existe en su lista |

**Y lo que NO se relaja nunca, en ninguna circunstancia:** la columna de datos (un rojo irreducible sigue
descalificando) y la columna de consecuencia (dinero, plazo legal o visado sigue descalificando). Esas dos
no son de comodidad: son la razón de existir del filtro.

## 5.5 La alternativa si el hilo falla: repuesto y divorcio preautorizado

**El repuesto se nombra el día 3, no el día de la crisis.** Es el segundo de la lista puntuada, y se firma
con fecha. Nombrar un plan B cuando ya se ha dudado se lee como excusa; nombrarlo en la semana 1 se lee
como plan.

**El divorcio está preautorizado y tiene aritmética escrita:**

> Al final de M1 lo único construido son cuatro documentos: la descripción del proceso, la línea de
> corte, la ficha de criterio y la batería de diez casos. **Rehacer las cuatro cosas sobre el proceso de
> repuesto son aproximadamente dos horas**, porque el método ya lo sabe y lo único que cambia es el
> contenido. A partir de M2 el divorcio ya cuesta caro. **Por eso el checkpoint está exactamente ahí y no
> después.**

Es decir: **el diseño concentra el riesgo del ángulo en las primeras cuatro semanas y lo hace barato
justo mientras es probable.** Es una respuesta estructural, no motivacional.

## 5.6 El expediente modelo — P27, y qué papel juega exactamente

El curso trae el recorrido completo **ya hecho** sobre **P27, el análisis de las encuestas de
satisfacción**: las ocho capas, con sus artefactos, sus fallos típicos y sus **claves selladas**.

**Por qué P27 y no otro.** Cuatro análisis independientes convergen: riesgo **bajo** (no hay dinero, no
hay plazo legal, no lo ve ningún cliente); volumen **alto** (600–800 respuestas al año); es el proceso
**más multilingüe** de su lista (10+ idiomas); **hoy no se hace** porque nadie tiene tiempo, así que no
compite con ningún procedimiento establecido; y es el que **más solapa con su formación** (análisis de
contenido, libro de códigos, estilos de respuesta culturales). Que el proyecto más útil sea también el
más seguro es un regalo del dominio.

**Tres funciones, y no una cuarta:**
1. **Ejemplo trabajado con desvanecimiento**: en M0 va entero, en M4 le faltan los dos últimos pasos, en
   M6 solo trae la lista de comprobación de la rúbrica.
2. **Fuente de los tres cebos** y de las claves selladas de los ocho dobletes.
3. **Proceso de repuesto por defecto** si su elección se cae y no tiene otra (§5.4, paso 4), y **ruta de
   respaldo obligatoria** para las dos lecciones que su proceso podría no activar: la clasificación en
   lote (M3) y el multilingüismo (M2 y M4).

**No es un segundo hilo que ella ejecute.** Se lee y se usa como clave; no se hace. Es la decisión más
discutible del diseño y la defiendo en §17.2.

---

# 6. MAPA COMPLETO DE MÓDULOS

**Ocho módulos, 18 semanas, 2 h propias por semana** más el trabajo que es trabajo del puesto. **Arranque
en octubre**: el pico de junio–septiembre de la academia (250–400 correos/día) mata cualquier calendario
que lo ignore, y noviembre–febrero es su temporada baja.

**Estructura fija de módulo**, y no se toca: **3 sesiones núcleo de 35–45 min de tiempo propio + 1 bloque
de proyecto de 60–90 min en horario de trabajo + el cierre de capa (cinco preguntas + pregunta fija +
doblete + columna nueva de la Tira, 40 min).**

**Una frontera declarada desde la semana 1, y esto es diseño anti-abandono, no una rebaja:**

> **Al terminar M4 (semana 11) ya hay curso:** un proceso suyo funcionando, en uso, con frenos probados
> y apagado probado. **M5, M6 y M7 son donde se cobran los objetivos 4 y 5** —criterio portátil y
> evangelización— y son la parte que más rinde a doce meses vista. Decirlo así, y no fingir que las
> dieciocho semanas son un bloque indivisible, es lo que evita que la semana 12 se lea como fracaso.

---

## M0 · Capa 0 — Ver el proceso, y elegir cuál · semanas 1–2

**Cambio mental.** Tres, y el tercero es el que más cuesta.
*«Lo primero no es la IA: es mirar qué hago realmente.»*
*«Lo que creo que hago y lo que hago no son lo mismo, y la diferencia es exactamente lo que rompería una
automatización.»*
*«El mismo texto en la misma pantalla es seguro o inseguro según con qué cuenta haya entrado.»*

**Contenidos.**
1. Las cinco preguntas, presentadas y aplicadas por primera vez **a su chat de hoy**.
2. Muestreo de eventos frente a introspección: por qué un proceso se observa y no se recuerda.
3. Las **cuatro preguntas que definen cualquier plan de cualquier proveedor en cualquier año**, más la
   quinta, que es la que suele decidir: *¿alguien lo ha configurado y ha dejado dicho por escrito qué se
   puede meter?*
4. El semáforo verde/ámbar/rojo y la línea entre cuenta personal y cuenta de empresa.
5. Los seis motivos transferibles de zona prohibida.

**Qué construye.**
1. **Día 1, 25 minutos: la primera victoria, dentro del proceso candidato.** Instrucciones permanentes
   guardadas —quién es, dónde trabaja, en qué idiomas escribe, qué tono usa, qué no debe hacer nunca— y
   usadas **hoy** sobre un correo real pendiente. Cronometrado antes y después. Sin instalar nada, sin
   pedir nada a nadie, sin hablar con nadie. **El mapa del curso va después de este resultado, nunca
   antes.**
2. **Día 3, 30 minutos: el asistente que cita, con tres fuentes verdes** — tarifario vigente, calendario
   académico y condiciones generales— que contesta las seis preguntas que repite el 70–80 % de sus leads
   **diciendo de qué documento sale cada dato**. *(Injerto 1 del juez 1, escalonado a propósito: ver la
   caja de abajo.)*
3. **Días 2–3: el embudo de noventa minutos** (§5.2) y **la prueba de la sombra** (§5.3).
4. **`00-como-se-hace-de-verdad.md`**: el proceso descrito como se ejecuta —disparador, documentos que
   abre, decisiones que toma y no están escritas, salida y a dónde va—, escrito **a partir de la hoja de
   sombra**, no de memoria.
5. **La ficha del entorno**, ocho casillas, con los mensajes literales para copiar y pegar **y** las
   comprobaciones empíricas por si nadie contesta.
6. **La tarjeta del lunes** impresa al lado de la pantalla.
7. **Proceso de repuesto nombrado y firmado.**

> **Por qué la victoria del día 1 y el asistente del día 3 son dos cosas distintas.** El juez 1 pide
> injertar el asistente con tres fuentes verdes de arq-2 —el mejor premio del día 1 de los tres
> diseños— para eliminar las tres semanas de sequía de artefacto de arq-3. Y a la vez señala que **es la
> apuesta más frágil de las tres**, porque exige encontrar la superficie de asistentes, adjuntar
> ficheros y conseguir que cite, todo antes de saber qué edición tiene contratada la empresa; la propia
> autocrítica 8 de arq-2 lo admite: *«si esa caja no funciona, la primera experiencia del curso es un
> fracaso y no hay red debajo»*.
>
> **La solución es escalonarlo, no elegir.** El día 1 se mantiene el premio pequeño y a prueba de fallo
> (instrucciones permanentes + un correo real cronometrado): funciona en cualquier plan, en cualquier
> herramienta, sin diagnóstico previo. El día 3, con el diagnóstico del entorno ya hecho, se monta el
> premio grande. Si el día 3 falla, **ya hay una victoria detrás** y el fallo es información —«mi
> edición no lo incluye»— y no un veredicto. Con esto, las semanas 3–4 de documentación transcurren con
> algo suyo funcionando encima de la mesa, que era el objetivo del injerto.

**Capacidad que entrena.** **Mirar un proceso y describirlo como es.** Es la más portátil del curso y la
que ella pide con el nombre de «criterio portátil». Se enseña transferible por construcción: se describe
por observación y no por introspección, con tres campos y dos días; ese método vale para cualquier
proceso, de cualquier empresa, en cualquier año, y no menciona ninguna tecnología.

**Entregable.** La carpeta del expediente con seis ficheros: hoja de elección puntuada, hoja de sombra,
`00-como-se-hace-de-verdad.md`, ficha del entorno, tarjeta del lunes, repuesto firmado. Más la ficha de
las cinco preguntas rellenada para su chat de hoy.

**Duración realista.** 2 semanas. **~2 h 30 de tiempo propio** (25 min el día 1 + 30 min el día 3 + 90
min del embudo + 25 min de la ficha del entorno), más 3 min/día de sombra y el cronometraje, que **son
tiempo de trabajo**. El material lo declara línea a línea.

**Mecanismo de autocorrección.**
- **Ejecución real y cronómetro.** El correo del día 1 salió mejor y en menos tiempo, o no.
- **La batería sellada de diez preguntas del asistente del día 3**, escritas **antes** de montarlo.
  Umbral: falla >0 de los 5 típicos → no está listo; se inventa una decisión en alguno de los 3 límite
  → no está listo; contesta algo distinto de «no lo sé» en alguno de los 2 de rechazo → no está listo.
- **Los tres criterios de rechazo de la prueba de la sombra.** No hay nada que valorar: se mira la hoja.
- **La comprobación que más caza, y cuesta un minuto:** *¿tu descripción contiene al menos dos decisiones
  que no estaban en tu idea previa del proceso?* Si no, la escribiste de memoria y hay que volver a
  observar. **Es la única forma sin mentor de detectar el error más caro de la capa.**
- **La pantalla corrige el plan.** Las comprobaciones empíricas se corrigen solas, y enseñan de paso lo
  que necesitará cuando el material envejezca: **la documentación dice una cosa y la instancia dice otra,
  y manda la instancia.**
- **Rúbrica de la ficha del entorno, con un estándar de suspenso brutal y muy útil:** *si en algún punto
  has escrito «creo que», «supongo que» o «me suena que», está mal resuelto.* «No lo sé y lo pregunté el
  día 14» sí vale. Distinguir lo que sabes de lo que supones es el mismo estándar que va a necesitar para
  evaluar respuestas de una IA, y por eso va el primero.

**Doblete (20 min): P29, emergencias 24 h.** Aplicar la capa 0 a un proceso que **no se va a delegar
nunca**. Veredicto correcto: *ZP; y sin embargo describirlo sirve* —para tener el protocolo escrito—
**pero no para entregarlo**. Enseña que mapear un proceso no compromete a automatizarlo, que es justo el
reflejo que hay que romper.

**PUERTA M0 → M1 — se pasa cuando:**
- [ ] Existe la ficha del entorno con las ocho casillas **y ninguna frase que empiece por «creo que»**.
- [ ] Hay un proceso elegido con **ningún −3** y con la hoja de sombra de dos días hecha.
- [ ] `00-como-se-hace-de-verdad.md` contiene **al menos dos decisiones no previstas**.
- [ ] El proceso de repuesto está **nombrado y firmado con fecha**.
- [ ] Hay una **línea base medida**, no estimada: minutos por unidad, tres mediciones.

**PC-1 al final de la semana 2.**

---

## M1 · Capa 1 — Qué es hacerlo bien, y qué trozos no entrego · semanas 3–4

**Cambio mental.** Dos, y son los dos más caros del curso.
*«El cuello de botella no es el prompt: es que nadie ha escrito nunca qué cuenta como respuesta correcta
en esta tarea.»*
Y el segundo, que no tiene que creer por autoridad porque lo deduce de algo que sabe desde tercero de
carrera:

> **Un modelo de lenguaje es el instrumento con la validez aparente más alta y la garantía de validez de
> contenido más baja que vas a manejar en tu vida. Está optimizado para producir texto plausible: la
> plausibilidad es su función objetivo, no un efecto secundario.**

**Contenidos.**
1. Operacionalizar: de un constructo difuso a indicadores observables (EP-01).
2. Anclas conductuales para el tono (EP-02): tres frases completas por nivel, sacadas de correos que
   envió de verdad.
3. **Los seis veredictos** (§4.2), presentados aquí y aplicados **dentro** de su proceso.
4. Tabla de especificaciones de una batería (EP-03) y diseño de ítems sin pista en el enunciado (C4).
5. Los diez apartados (EP-06) y el sesgo del experimentador.
6. El protocolo de corrección con IA, siete reglas, primera aplicación.

**Qué construye.**
1. **La línea de corte** (`01-linea-de-corte.md`), y es el entregable más importante del módulo: el
   proceso **partido en trozos**, y cada trozo con:
   - **uno de los seis veredictos**;
   - el **motivo**, si se queda con ella, elegido de una **lista cerrada de tres**: riesgo · conocimiento
     que caduca · no hay fuente de verdad;
   - y —injerto de arq-2— **«lo que sí se puede hacer alrededor»**, rellenado con un **artefacto
     nombrable**, no con una intención.
2. **La ficha de criterio** (EP-01): definición en una frase, 4–6 dimensiones, un indicador observable
   por dimensión, críticos marcados, punto de corte. **Una cara.**
3. **Las anclas de tono** (EP-02). Ese fichero **es** el contexto de tono de la capa 2, no un
   calentamiento.
4. **Los diez apartados** (EP-06): diez casos reales sacados **por orden cronológico, no elegidos**, y
   cerrados antes de escribir una línea de instrucción.
5. **La batería de diez casos y su clave sellada**, con **al menos un típico y un límite en un idioma
   minoritario real de su buzón**.
6. **La Tira**, columnas 1 y 2.

> **Por qué los seis veredictos entran aquí y no en un módulo de panorama, y por qué dentro del proceso
> y no sobre una lista de tareas.** Este es el injerto que más cambia el diseño respecto a la hipótesis
> de partida. Aplicar la rejilla **a los trozos de su propio proceso** es mejor que aplicarla a doce
> procesos ajenos, por tres razones: es donde aparecen de verdad el veredicto 1 —casi todo proceso real
> tiene un trozo que es aritmética— y el veredicto 2 —casi todo proceso real tiene un trozo cuya fuente
> de verdad nadie puede nombrar—; obliga a partir el proceso, que es la operación que ningún principiante
> hace y la que más criterio produce; y **no cuesta ni un minuto extra**, porque la línea de corte existía
> igual, solo que con veredicto libre. Cambiar un veredicto libre por una rejilla cerrada de seis
> destinos convierte una decisión en una clasificación reutilizable.

**Capacidad que entrena.** **Operacionalizar** y **decidir el destino de un trozo de trabajo**.
Transferencia FUERTE (`dominio-psicologia.md` C1): es la misma operación que hizo en la carrera, con otro
objeto. Y un matiz que va en el mismo párrafo porque le ahorra una pregunta: **aquí no estás estimando
nada, estás decidiendo.** No hay criterio verdadero que descubrir; hay criterio explícito y defendible, o
no hay nada.

**Entregable.** Línea de corte + ficha de criterio + anclas + diez apartados + batería con clave sellada
+ Tira con dos columnas. **Es el módulo más denso en trabajo mental y el más ligero en clics de todo el
curso**: casi todo es un documento. La sesión 1 empieza **pasando la batería contra su forma actual de
trabajar y viendo que saca 4 de 10**, para que la ficha de criterio nazca como respuesta a un fallo
observado y no como deberes previos.

**Duración realista.** 2 semanas.

**Mecanismo de autocorrección.**
- **Ctrl+F sobre la ficha de criterio.** Si aparecen «adecuado», «correcto», «natural», «profesional» o
  «de calidad» **sin un ancla detrás**, no ha operacionalizado: ha renombrado el constructo.
  Autocorrección mecánica perfecta, cinco segundos.
- **Prueba de tamaño:** la ficha cabe en una cara. Una rúbrica de dos páginas no se usa nunca.
- **Dos ítems que arq-3 no tenía y que vienen de arq-1:** *¿al menos un indicador es verificable contra
  una fuente externa? ¿están todos marcados como críticos?* Si todos son críticos, no ha priorizado.
- **Rúbrica de la línea de corte, con dos criterios negativos que deciden el módulo:**
  *(a) si no hay ningún trozo que se quede contigo, está mal resuelto — vuelve;*
  *(b) si el motivo de algún «se queda conmigo» es «es difícil», está mal.*
  Y el tercero, del injerto: *(c) si algún trozo con veredicto 1, 2 o ZP tiene la casilla «lo que sí
  alrededor» vacía o con una intención en vez de un artefacto nombrable, está mal.*
- **Los diez apartados se abren al final, y tiene que fallar al menos uno.** Si no falla ninguno,
  sospecha del muestreo antes que celebrar: *si tu batería la pasa entera a la primera, tu batería es
  fácil; no es que tu sistema sea bueno.*
- **Y el criterio no se toca.** Si al abrirlos le dan ganas de cambiar la ficha para que aprueben, **lo
  anota y no lo cambia**. Ese impulso es el dato más interesante del ejercicio y tiene nombre.
- **CEBO 1 (control positivo).** El curso trae una **línea de corte de mentira**, de una academia
  inventada, con **tres defectos plantados y documentados** en un fichero sellado: uno visible (un trozo
  con datos rojos marcado como «lo entrego»), uno de omisión (falta el trozo de revisión humana antes de
  que algo salga), y uno de criterio (un trozo determinista clasificado como veredicto 5 cuando es
  veredicto 1). Ella lo corrige con la rúbrica y **después** abre la hoja de defectos. **Si encuentra 1 o
  0, ese tipo de trabajo no se corrige con IA en el resto del curso.**

**Doblete (20 min): P02, presupuestos.** Escribir su ficha de criterio hace visible que todos los
indicadores se cumplen con una fórmula: semanas × tipo de curso × alojamiento × suplemento de verano ×
descuento por volumen. **Veredicto correcto: 1, NI IA.** Y meter un modelo de lenguaje ahí no es
ineficiente: **es introducir un error posible donde no lo había**. Clave sellada.

**Checkpoint de divorcio, al final del módulo** (§5.5).

**PUERTA M1 → M2 — se pasa cuando:**
- [ ] La ficha de criterio **pasa el Ctrl+F**, cabe en una cara y tiene al menos un indicador verificable
      contra fuente externa.
- [ ] La línea de corte tiene **al menos un trozo que se queda con ella**, ningún motivo es «es difícil»,
      y **cada «no» tiene su artefacto nombrable**.
- [ ] La batería está escrita, tiene **al menos un caso en idioma minoritario**, la clave está sellada y
      la Tira tiene **dos columnas fechadas**.
- [ ] El cebo 1 está hecho y anotado. Si encontró 1 o 0 defectos, la decisión sobre la IA correctora
      está **escrita**.

**PC-3 al final de la semana 4** (sobre el cebo, no sobre su trabajo).

---

## M2 · Capa 2 — Que sepa de dónde sale cada dato · semanas 5–6

**Cambio mental.** *«La memoria fiable es un fichero, no una sensación.»* Y la tríada que los
principiantes mezclan siempre: **fuente de verdad** (hechos, desde una sola dirección) ≠ **memoria**
(acuerdos que permanecen) ≠ **procedimiento** (pasos y formato de salida). Confundirlas produce el error
más común: meter el tarifario **dentro** de las instrucciones. Funciona en enero y miente en marzo,
porque las instrucciones no se revisan y los documentos sí.

**Contenidos.**
1. Las tres cosas que hacen que una base de fuentes sea un instrumento y no un cajón: responde solo desde
   ahí · dice de qué documento sale cada dato · **puede negarse**.
2. **La fecha y el dueño como parte de la fuente.**
3. **«No lo sé» es una respuesta correcta, hay que exigirla explícitamente con fórmula literal y hay que
   probarla a propósito.**
4. Seudonimización de verdad: cuasi-identificadores, no solo el nombre. La regla de los adjuntos.
5. **El multilingüismo como decisión de diseño, no como detalle** (ver caja).
6. Las tres señas que identifican esta capacidad en cualquier herramienta (§8.2).

**Qué construye.**
1. **El mapa de datos del proceso** (§10.2): cada dato que lo atraviesa, su color, **en qué paso entra y
   en cuál hay que quitarlo, y quién lo quita**. Una cara.
2. **Las fuentes**, con **fecha y dueño en la primera línea de cada una**. Copias, nunca maestros.
3. **El asistente v2**, que responde citando el documento y su fecha y que **dice «no lo sé»**.
4. **La prueba de traslado** (§8.4).
5. **La Tira**, tercera columna.

> **El multilingüismo, y por qué está aquí como contenido y no como suerte.** Es el fallo de encaje más
> serio que el juez 4 le encuentra a esta columna vertebral: en arq-3 el multilingüismo **no aparece en
> ningún resultado de aprendizaje**, de modo que la propiedad que define su puesto —P01 en 6–12 idiomas,
> P27 en 10+, la dirección del alojamiento siempre también en español para el taxista, *«traducir la
> queja es media resolución»* en P20, y las seis versiones de plantilla que envejecen calladas en P32—
> dependía del proceso que le tocara. Aquí entra en tres sitios, con nombre:
>
> 1. **Instrucción de diseño, en la capa 2:** *las fuentes están en español y la respuesta va en el idioma
>    de la persona.* Es una separación de capas —conocimiento frente a presentación— y no una
>    traducción, y por eso es criterio y no truco.
> 2. **Instrumento, en la batería (M1):** al menos un caso típico y un caso límite **en un idioma
>    minoritario real de su buzón** —neerlandés, turco, coreano, polaco—, **no en inglés, que es el
>    fácil**. Un sistema que se prueba solo en inglés está sin probar.
> 3. **Freno, en la capa 4:** *parar si el mensaje llega en un idioma que no está entre los que has
>    probado.*
>
> **Y la ruta de respaldo, escrita por delante:** si su proceso resulta ser monolingüe, los tres
> ejercicios se hacen sobre el expediente modelo (P27), que es el proceso más multilingüe de su lista.
> El resultado de aprendizaje no depende de la suerte de la elección.

**Capacidad que entrena.** **Contexto con procedencia.** Tres piezas transferibles, ninguna con nombre de
producto: **citar no es un adorno, es lo que hace que revisar cueste cinco segundos en lugar de una
investigación** —y esa diferencia es la que hace que la revisión se siga haciendo en julio—; **«no lo sé»
hay que exigirlo y probarlo**; y **una fuente sin fecha y sin dueño no es una fuente, es un papel** —el
dueño es quien puede cambiarla, la fecha es lo que te dice si mirarla.

**Entregable.** Mapa de datos + fuentes fechadas y con dueño + asistente que cita y se abstiene + ficha
de traslado + Tira con tres columnas.

**Duración realista.** 2 semanas.

**Mecanismo de autocorrección.**
- **La batería, tercera columna**, con umbral asimétrico: falla >0 de los 5 típicos → no está listo; se
  inventa una decisión en alguno de los 3 límite **aunque acierte** → no está listo; contesta algo
  distinto de «no lo sé» en alguno de los 2 de rechazo → no está listo. **Una respuesta correcta a un
  caso de rechazo es un suspenso**, porque significa que responde desde fuera de sus fuentes.
- **Lista de comprobación binaria, diez ítems observables:** *¿cada fuente tiene fecha en la primera
  línea? ¿cada fuente tiene un nombre de persona como dueño? ¿alguna respuesta cita un documento que no
  contiene el dato —comprobado abriendo tres al azar—? ¿hay una frase que diga qué hacer cuando falta un
  dato? ¿he subido el maestro de algo en vez de una copia? ¿hay algún precio o fecha escritos dentro de
  las instrucciones en vez de en una fuente?*
- **La prueba de la compañera**, sobre tres casos seudonimizados: *¿podría [nombre de una compañera
  concreta] saber de quién hablo leyendo esto?* Si sí, sigue quitando. **Y el criterio del otro lado, que
  casi nadie pone:** el texto resultante tiene que **seguir sirviendo**; si la respuesta que produce es
  inservible, has quitado contexto que no era identificador.
- **La prueba de traslado se corrige sola**: o las tres columnas están rellenas con cosas concretas, o no.
  Criterio negativo: *si la columna «qué viajó tal cual» está vacía, no construiste criterio: construiste
  un prompt.* Y el diagnóstico de arq-1: **si no consigue montarlo en veinte minutos, no aprendió la
  capacidad, aprendió la ruta** — y ese diagnóstico llega a tiempo de corregirlo.

**Doblete (20 min): P08, carta de aceptación para visado.** **Veredicto correcto: ZP.** Y el motivo
transferible es el que hay que saber decir: *«la normativa de extranjería cambia de un año para otro, y
congelar dentro de un artefacto un conocimiento que caduca es fabricar un error futuro»*. Es el doblete
que mejor entrena el criterio portátil, porque **no metas conocimiento volátil dentro de un artefacto**
vale para cualquier dominio. Clave sellada.

> **Y la corrección obligatoria que pide el juez 4, incorporada aquí como parte de la solución
> comentada.** Arq-2 proponía como «lo que sí se puede hacer alrededor» de P08 *«montar la comprobación
> que caza el nombre mal transcrito desde el pasaporte»*. **Eso está mal y hay que decirlo**: mete un
> documento de identidad en la herramienta, y el semáforo lo clasifica como **rojo absoluto — nunca, en
> ninguna herramienta, ni imagen ni PDF**. La versión admisible ataca el mismo mecanismo de error sin que
> el pasaporte entre en ningún sitio: **una comprobación determinista de consistencia entre los campos
> que ella ya ha tecleado a mano** —expediente ↔ carta ↔ factura ↔ certificado—, que además es veredicto
> 1 y no necesita ningún modelo. Este ejemplo vale doble: enseña el «lo que sí alrededor» y enseña que
> una alternativa mal pensada puede ser peor que el «no».

**PUERTA M2 → M3 — se pasa cuando:**
- [ ] La batería da **5/5 en los típicos**, **pide aclaración** en los 3 límite y dice **«no lo sé»** en
      los 2 de rechazo.
- [ ] **Ha usado el asistente al menos cinco veces en una semana SIN que el curso se lo pidiera.**
- [ ] La prueba de traslado está hecha y las tres columnas están rellenas.
- [ ] El mapa de datos tiene, en cada fila ámbar o roja, **un paso concreto y una persona** en la columna
      «dónde se quita y quién».

> **La segunda condición es la puerta más importante del curso, y es injerto directo de arq-1** (§1.6,
> salvaguarda 4). No mide si aprendió la lección: **mide si el artefacto le sirve**, que es la única
> forma honesta de saberlo sin profesor, y es una medida conductual, externa a su juicio sobre su propio
> trabajo. Arq-3 tenía esta idea enterrada como consejo dentro del «cuándo NO poner un disparador»; aquí
> sube a condición de paso, porque **la tesis entera de esta columna vertebral —que el mundo la corrige
> cada martes— es falsa si ella no lo usa**. Y con su frase asociada, que va en negrita en el material:
> **automatizar algo que no usas es multiplicar un error que ni siquiera has visto.**
>
> **Qué hacer si la puerta no se abre**, escrito por delante para que no se lea como fracaso: no se
> avanza, y se hace el diagnóstico de tres preguntas — *¿no lo abro porque no me acuerdo (→ ponlo donde
> ya miras)? ¿porque contesta peor que yo (→ vuelve a la ficha de criterio)? ¿o porque esta tarea en
> realidad no la hago tanto (→ el embudo se equivocó, y ahí está el repuesto)?* Las tres tienen salida.

---

## M3 · Capa 3 — Que ocurra sin que lo pidas · semanas 7–8

**Cambio mental.** *«Automatizar no es una herramienta nueva: es quitar el dedo del disparador.»* Es el
momento psicológico del curso —la primera vez que algo pasa sin que ella lo pida— y por eso llega en la
semana 7 y no en la 14.

**Contenidos.**
1. **Solo hay dos clases de disparador** y la diferencia decide qué casos vas a poder atender: por
   **calendario** («cada lunes a las nueve») y por **suceso** («cuando entra algo que cumple X»).
   **Un lunes no es un suceso.**
2. **Las tres cosas sin las cuales un disparador no está terminado:** un **tope** · un **apagado
   probado** · una **salida que prepara y no envía**.
3. **Automatiza donde ya viven tus datos**: el criterio que decide entre plataformas de automatización en
   cualquier año. La que reutiliza lo que ya tienes gana a la más potente; y la que mete a un proveedor
   nuevo entre tus datos y tú tiene que ganar por mucho para compensarlo.
4. Notación neutra de un flujo: DISPARADOR → PASO → CONDICIÓN → SALIDA.
5. Cuándo **no** poner un disparador.

**Qué construye.** El trozo de su proceso que la línea de corte marcó como entregable, **con disparador**,
más el tope, más el apagado probado. Y la **prueba de portabilidad nº 2** (§8.4).

Y la regla que gobierna la capa entera, en negrita en el material:

> **Automatiza la lectura y la preparación. La escritura hacia fuera la firma una persona.**
>
> Y la razón, que no es prudencia sino diseño de aprendizaje: **si el artefacto solo prepara, todos sus
> errores son recuperables, y por eso puedes permitirte equivocarte mucho — que es exactamente lo que
> hace falta para aprender.** Etiquetar es reversible; enviar no. Se puede relajar más adelante, proceso
> a proceso y con datos de acierto medidos. **No se relaja por costumbre.**

**Los límites, por delante y no al tercer intento fallido.** En la primera página del módulo: la
automatización nativa de su entorno **falla con unidades compartidas, carpetas compartidas y hojas con
referencias externas** [V]; un solo disparador por flujo; tope de etiquetas visibles; el administrador
puede tener pasos desactivados y no hay forma de saberlo hasta intentarlo. **Como la cuarta columna del
embudo de M0 ya descartó los procesos que solo viven en recursos compartidos, aquí esto no debería ser una
sorpresa sino una confirmación** — y esa es exactamente la función de haber puesto la restricción en el
criterio de elección.

> **REGLA ESTRUCTURAL DE INDEPENDENCIA DE PLATAFORMA** *(injerto de arq-1, momento 2, punto 6)*:
> **ningún módulo posterior depende de que el constructor de flujos esté habilitado.** M3 tiene que
> tener **dos rutas escritas por delante**: (A) un disparador por reloj **dentro del chat que ya usa**,
> que existe en todos los planes; (B) un disparador por suceso con la herramienta de automatización de la
> suite, si el administrador la tiene activada. La ruta A basta para cerrar la capa, para pasar la
> puerta y para que M4 tenga sobre qué ejercitar los frenos. Si la B no está disponible, **se pierde
> comodidad y volumen, no aprendizaje**, y el material lo dice así: no es un fallo suyo ni del curso.

**Capacidad que entrena.** **Disparador.** La transferencia es limpia porque la anatomía es universal, y
la prueba de portabilidad nº 2 la hace observable: escribir el flujo en notación neutra y localizar cada
pieza en la documentación de otra plataforma, **sin dar de alta ninguna cuenta**.

**Entregable.** `03-disparador.md` con su tipo declarado y justificado, el tope, el apagado probado y la
prueba de los seis casos anotada con fecha. Más la ficha de portabilidad nº 2, tres líneas. Más la Tira,
cuarta columna.

**Duración realista.** 2 semanas, y es el primer módulo con probabilidad real de desbordarse: dos
sesiones de 45 min de tiempo propio más un bloque de proyecto de 90 min en horario de trabajo.

**Mecanismo de autocorrección.**
- **Se dispara o no se dispara.** El corrector más fiable que existe, y aquí está entero.
- **La prueba de los cinco casos fabricados, uno por categoría, y un sexto que NO debe disparar** — que
  es el que casi nadie prueba. Cinco salidas correctas y una no-salida, o no las hay.
- **La prueba del tope:** meterle un lote grande a propósito y comprobar que se detiene y avisa.
- **La prueba de apagado.** Se apaga de verdad y se vuelve a encender. *Un sistema que no sabes apagar no
  está terminado* — y hay una razón práctica además de la obvia: el día que falle vas a estar nerviosa, y
  no es el momento de averiguar dónde está el interruptor.
- **Lista de comprobación de plataforma, seis ítems binarios**, escrita como síntomas y reutilizable como
  diagnóstico: *¿el fichero que toca está en un recurso compartido? ¿la hoja usa referencias externas?
  ¿tiene más de un disparador? ¿hay algún paso que escriba hacia fuera? ¿lo he probado con un caso que
  debe NO disparar? ¿sé cómo se apaga y lo he apagado hoy?*
- **La Tira, cuarta columna**, con la lectura contraintuitiva escrita: *si la calidad ha mejorado respecto
  a la capa 2, sospecha: probablemente reescribiste el criterio por el camino, y eso es mérito tuyo, no
  del disparador.*
- **PC-4, el comodín**, disponible desde aquí.

**Doblete (20 min): P30, el parte semanal a dirección académica.** Determinista puro. **Veredicto
correcto: 5, y con la mínima IA posible en el camino crítico.** Enseña que «automatizar» no significa
«meter un modelo», que es la confusión más extendida y la que más caro sale. Clave sellada.

**PUERTA M3 → M4 — se pasa cuando:**
- [ ] El disparador está vivo, los cinco casos disparan, **el sexto no dispara**, el tope se ha probado y
      el apagado se ha ejecutado.
- [ ] La prueba de portabilidad nº 2 está hecha, con sus tres líneas.
- [ ] **Ha visto fallar algo y sabe por qué falló.** *(Si a estas alturas no ha fallado nada, el material
      trae un fallo provocado: un caso fabricado que rompe el flujo por un motivo concreto y
      diagnosticable.)*

> **La tercera condición es la otra puerta de arq-1** (3→4) y es igual de deliberada: **sin haber visto un
> fallo no hay criterio para dar autonomía a nada.** El fallo provocado es un control positivo aplicado
> al sistema, exactamente como el cebo lo es a la correctora.

---

## M4 · Capa 4 — Juicio donde hace falta, frenos donde hace falta · semanas 9–11

**Tres semanas, no dos.** Es el único módulo al que se le da aire antes del final, y se dice por qué: es
la frontera conceptual del curso y el punto donde más gente se cae.

**Cambio mental.** Dos.
*«Un agente no es una automatización mejor: es una automatización que **ha renunciado a ser predecible** a
cambio de poder afrontar casos que no previste. En atención al cliente esa renuncia se paga a conciencia y
solo donde compensa.»* Y la dirección del error que casi nadie enseña: **un agente puede ser exceso.** Si
los pasos son fijos, meterle juicio lo hace más caro, más lento y menos auditable.
Y el segundo: *«el riesgo no es el del día 1, es el del día 60.»* Sesgo de automatización: a la tercera
semana se deja de revisar. **La confianza no es una salvaguarda.**

**Contenidos.**
1. Qué es un punto de juicio y por qué solo va donde el camino se bifurca por algo que no puedes escribir
   de antemano.
2. **Tema prohibido ≠ condición de parada.** Uno dice **de qué** no se habla; el otro dice **cuándo** se
   deja de trabajar aunque el tema estuviera permitido. Las dos hacen falta y se confunden siempre.
3. **Parar no es callarse:** no producir salida + dejar marca visible donde ella ya mira + decir por qué
   paró, en una línea.
4. **Quién revisa es una persona con nombre y una hora**, no un procedimiento.
5. El plan para cuando falle, en cinco pasos.
6. El aviso de que se interactúa con una IA; el Anexo III aplicado a su academia; el privilegio mínimo.
7. **Un aviso sobre su propia formación** (ver abajo).
8. La caja del fondo: qué existe, qué haría falta para que le tocara.

**Qué construye.**
1. **El juicio, confinado a dos o tres puntos concretos** de su proceso, cada uno con su criterio escrito
   y justificable.
2. **La lista de temas prohibidos** (`04-frenos.md`), en negativo y sin matices: *nunca respondas sobre
   requisitos o plazos de visado; nunca cites importes; nunca confirmes disponibilidad de alojamiento;
   nunca respondas a una queja formal; nunca menciones salud. Si el tema aparece, aunque no use esas
   palabras, escribe SOLO: DERIVAR A PERSONA — motivo: <tema>, y para.*
3. **Las condiciones de parada**, seis, y las seis con motivo: no encuentro la respuesta en mis fuentes ·
   la persona está enfadada o menciona abogado, reclamación u hoja de reclamaciones · salud o menor
   implicado · el importe supera X · **el mensaje viene de una agencia y menciona un acuerdo o convenio
   particular** · **el mensaje llega en un idioma que no está entre los que he probado**.
4. **El punto de revisión humana, con nombre propio y hora.**
5. **El plan para cuando falle**: detectar, parar, reparar con la persona (llamada, no correo), corregir
   el sistema añadiendo ese caso a la batería, y valorar si hay brecha de datos — **esto último no lo
   decide ella [!]**, lo escala el mismo día.
6. **La ficha de las cinco preguntas aplicada a una herramienta que el curso no ha enseñado** (RA4).
7. **La Tira**, quinta columna.

> **La condición de parada por agencia no es un adorno de dominio: es la que más dinero vale.** Entre el
> 30 % y el 50 % de las matrículas entran por agencias intermediarias (P03), que tienen **tarifas netas y
> condiciones de cancelación pactadas por convenio, distintas de las públicas**, y el sistema no las
> conoce. Aplicar la tarifa pública a una agencia con tarifa neta rompe el margen o rompe la relación
> comercial, **y se multiplica por quince alumnos**.

> **El aviso sobre su propia formación, y va en serio.** Esta es la única lección del curso donde su
> formación juega **en contra**, y por eso se dice aquí y no en una nota al pie. El reflejo entrenado de
> una psicóloga ante alguien que se queja es **validar, empatizar y hacerse cargo**. Los dos primeros
> están bien y son una ventaja real. El tercero, por escrito, en una queja formal, **es una admisión de
> responsabilidad que compromete a su empresa**. Y los modelos son complacientes por construcción: si le
> pides que redacte una respuesta empática a una queja, te va a dar un texto estupendo que dice *«tienes
> razón, la habitación estaba en malas condiciones»*, y sonará mucho mejor que el correcto. La línea que
> hay que ver: **reconocer la experiencia, no calificar el hecho**; describir lo que se ha hecho, no
> juzgar lo que pasó; y evitar el *«lamentamos que te sientas así»*, que suena a disculpa y funciona como
> invalidación — es el peor de los dos mundos. Importes, plazos legales, responsabilidad y compensaciones
> **no los decide ella y no los decide el sistema**. Se escalan. **[!]**

**Capacidad que entrena.** **Juicio acotado y condiciones de parada.** Y aquí la honestidad incómoda,
dicha sin disculparse porque es cierta y porque lo alcanzable es lo que se sostiene:

> **Su escalón 3 realista es «un proceso con juicio en dos o tres puntos», no «un agente autónomo que
> gestiona el buzón».** La barrera número uno no es técnica ni de capacidad suya: es de **licencia** —los
> agentes de verdad están detrás de planes que su empresa casi con seguridad no tiene [V]—, de
> **permisos** —un agente útil necesitaría el buzón compartido y la hoja de camas— y de **datos** —sus
> procesos de más volumen mezclan salud, religión, menores y documentación de identidad—.

Y la formulación que impide que eso envejezca mal *(injerto de arq-1 §12.3)*: **el módulo no afirma «los
agentes están fuera de tu alcance»**. Le hace **rellenar la ficha de cinco preguntas para el agente que
tenga delante ese día** y comprobar tres cosas concretas: ¿lo cubre mi plan? ¿puede actuar sobre los
recursos donde vive mi trabajo? ¿puedo ver qué hizo? Si en 2028 las tres respuestas son sí, **el módulo
funciona mejor, no peor**: le da luz verde con criterio.

**Entregable.** `04-frenos.md` con sus cuatro apartados + `04-casos-de-parada.md` con cinco casos
fabricados y su resultado observado con fecha + la ficha de cinco preguntas de una herramienta ajena +
media página con la frontera pasos-fijos / juicio + Tira con cinco columnas.

**Duración realista.** 3 semanas.

**Mecanismo de autocorrección.**
- **Cinco casos de parada fabricados que DEBEN parar**, y el quinto es un **ítem discriminante
  diseñado**: alguien que pregunta *«¿cuánto tarda el papeleo para poder venir?»* **sin decir la palabra
  visado**. *Los cuatro primeros los para cualquier lista; el quinto separa una lista de palabras de una
  lista de temas.*
- **Y el sexto caso, normal, que NO debe parar.** Si también para, **los frenos son demasiado anchos: el
  sistema no hace nada, y eso no es seguridad, es inutilidad**. El fallo del otro lado siempre está
  escrito.
- **Rúbrica con criterios negativos y salida escrita obligatoria** (sin «no aplica»): la lista incluye
  importes, plazos de visado, disponibilidad y salud **aunque su proceso no los toque hoy** —los sistemas
  se expanden solos y la lista se escribe para el sistema de dentro de seis meses—; la respuesta a «quién
  revisa» es **un nombre y una hora**; y **ninguna salida llega a un cliente sin que una persona le dé a
  enviar** — si su diseño lo permite, vuelve al principio.
- **Señal de fallo que predice su propia aparición:** *algún borrador suena estupendo y admite
  responsabilidad. Aparece casi siempre. Cuando aparezca, es el mejor ejemplo del curso de por qué la
  validez aparente no basta.*
- **Verdadero/falso de doce ítems** sobre el marco de datos, autocorrección instantánea. Menos de 10
  aciertos → releer.
- **CEBO 2**, ahora sobre una lista de frenos.
- **Y la calibración de la correctora por entregable, que es la mejor pieza de todo el corpus sobre este
  punto:** *este es el entregable del curso donde menos hay que fiarse de la corrección con IA, porque le
  estás pidiendo a un modelo complaciente que juzgue si otro modelo es demasiado complaciente. Usa la IA
  aquí solo para el bloque 1 de la rúbrica, y el bloque 2 lo compruebas mirando.* **Esta regla se
  generaliza en §12.4: la fiabilidad de la correctora se gradúa por entregable, no se aplica igual en
  todas partes.**

**Doblete (20 min): P28, respuesta a reseñas online.** **Veredicto correcto: 6 con recorte** — clasificar
y preparar sí, **publicar nunca**. Y el motivo no es de calidad, es de protección de datos: confirmar
públicamente que alguien fue alumno y tuvo un problema **ya es una cesión de datos**. Es el doblete que
mejor enseña que un freno puede venir de un sitio que no es la calidad del texto. Clave sellada.

**PUERTA M4 → M5 — la frontera declarada — se pasa cuando:**
- [ ] Los cinco casos de parada **paran** y **el sexto no para**.
- [ ] Cada parada deja **marca visible donde ella mira** y **dice por qué**, en una línea.
- [ ] «Quién revisa» es **un nombre y una hora**.
- [ ] **No existe ningún camino por el que algo llegue a un cliente sin que una persona le dé a enviar.**
- [ ] La ficha de cinco preguntas de una herramienta ajena está rellena, con sus tres comprobaciones.

**PC-5 al final del módulo.** Y aquí, cinco semanas antes de que ocurra, **se anuncia el compromiso
externo de M7**: *«en la semana 17 una compañera va a usar esto una semana entera sin ti.»*

---

## M5 · Capa 5 — Medirlo sin engañarme · semanas 12–13

**Cambio mental.** *«Que el sistema se ejecute cada lunes no es que sirva. Puede ejecutarse
impecablemente y no cambiar nada, porque el informe que produce no lo lee nadie o porque los borradores se
reescriben siempre.»* **Evaluación de proceso ≠ evaluación de resultado.**

**El gancho, que no es metodológico sino de deseo.** Este módulo **no se presenta como «vamos a
evaluar»**. Se presenta así: *«vas a poder decir cuánto ahorras y defenderlo si alguien lo comprueba»*.
Es el único módulo del curso cuyo motivo se puede formular enteramente en términos de lo que ella ya
quiere: el número es la munición del objetivo 5.

**Contenidos.** Línea base y diseño pre-post · **minutos por unidad** y por qué no «horas a la semana» ·
coste completo · las seis amenazas a la validez interna traducidas a su caso · deficiencia y contaminación
del criterio (C2b) · la cadena causal en cinco flechas (EP-14) · la prueba ciega (EP-08).

**Qué construye.**
1. **Media página de evaluación, con fecha**: el número antes (de la hoja de sombra de M0, medida
   **antes** de construir nada, que es lo que la hace honesta), el número después, el **coste completo**
   —montaje + revisión + mantenimiento—, **cuál de las seis amenazas podría explicar el resultado** y qué
   mediría para descartarla.
2. **La prueba ciega** (EP-08, *«el ejercicio con mejor relación valor/esfuerzo del curso»*): cinco
   respuestas suyas de hace meses y diez salidas del sistema sobre casos comparables, **sin marcas de
   origen, barajadas por otra persona**, puntuadas con la ficha de criterio de M1.
3. **La cadena causal en cinco flechas**, con el eslabón que no depende de ella subrayado.
4. **La lectura completa de la Tira**: una frase por columna diciendo qué aportó esa capa. *Si no puede
   escribir esa frase para alguna columna, esa capa no le aportó nada, y merece la pena saberlo.*

**Herramienta y por qué: una hoja de cálculo, un cronómetro y una persona que baraje.** Deliberado: **la
evaluación no se hace con la herramienta evaluada.** Pedirle a un modelo que juzgue lo que él mismo
produjo acumula dos sesgos documentados —preferencia por lo verboso y auto-preferencia— que apuntan al
mismo desastre: aprobar por construcción.

**Capacidad que entrena.** **Medir si sirve.** Es la más portátil de todas y la que ningún curso de IA da,
porque es metodología y no producto. Se enseña con su vocabulario **declarando el préstamo**: *«en el
mundo de la IA a la batería la llaman evals o tests de regresión; el nombre psicométrico —ítems ancla—
dice mejor para qué sirven, que es hacer comparables dos momentos distintos.»*

**Entregable.** `05-evaluacion.md` (media página) + resultado de la prueba ciega + cadena causal + la Tira
leída, con una frase por columna.

**Duración realista.** 2 semanas. La prueba ciega es una tarde.

**Mecanismo de autocorrección.**
- **La prueba ciega es autocorrección en estado puro.** No hay rúbrica que discutir: o acierta
  identificando cuáles eran suyas, o no; o ganan las suyas, o no. Y el patrón que aparece casi siempre
  —el sistema empata o gana en las dimensiones no críticas y pierde en la exactitud del dato— **le dice
  exactamente dónde poner la revisión humana**, que es la decisión que el curso entero perseguía.
- **Prohibiciones de vocabulario como comprobación mecánica.** Si aparece «significativo», está mal: aquí
  no se estima un parámetro poblacional, se comprueba la cobertura de un instrumento contra un criterio
  fijado. Si la medida es «horas a la semana» en vez de **minutos por unidad**, está mal: es lo único que
  sobrevive a que su volumen se multiplique por tres entre febrero y julio.
- **La resta obligatoria.** Si no ha restado revisión y mantenimiento, está mal. Y si el saldo es negativo
  y aun así quiere conservarlo por otra razón —menos errores, menos carga mental, respuesta más rápida al
  cliente—, **que lo diga y mida esa otra razón**: es legítimo, pero entonces el ahorro de tiempo no era
  el objetivo.
- **Una amenaza que no puede descartar, nombrada obligatoriamente.** Las seis, traducidas: historia
  (septiembre no es julio) · maduración (ella misma ha mejorado en la tarea) · regresión a la media
  (eligió lo que más dolía, y lo que más duele suele medirse en su peor semana) · instrumentación ·
  reactividad de la medida (la semana que se cronometra se trabaja más rápido — y este juega **a favor**:
  el ahorro real es mayor que el medido) · atrición (si deja de usarlo los días de agobio, la muestra
  final son los días tranquilos).
- El único favor humano del módulo —**barajar**— son cinco minutos y **no consume punto de consulta**:
  vale cualquier compañera.

**Caja obligatoria «lo que vas a ver la primera vez».** *«Es posible que el ahorro sea menor de lo que
esperabas. Si eso pasa, es un resultado del curso, no un fracaso tuyo — y es exactamente el tipo de
resultado que casi nadie publica. Antes de decidir nada, comprueba las dos cosas que casi siempre lo
explican: que estés midiendo por unidad y no por semana, y que hayas contado el tiempo de revisión en el
lado correcto de la resta.»*

**Doblete (20 min): P12, el check-in del lunes.** **Veredicto correcto: no aplica limpiamente.** El valor
de ese proceso es que fija la percepción de calidad de toda la estancia, y eso no se mide en minutos por
unidad. Es **deficiencia del criterio** (C2b) con un caso de su casa, y enseña la vacuna contra la métrica
de vanidad mejor que cualquier explicación. Clave sellada.

**PUERTA M5 → M6:** el número existe, **la resta está hecha**, hay una amenaza nombrada, y la Tira tiene
una frase escrita por columna.

---

## M6 · Capa 6 — Que sobreviva sin ti, y el resto de tu semana · semanas 14–15

**Cambio mental.** *«Un sistema sin dueño y sin fecha se degrada. Y cuando se degrada, el recuerdo que
queda en la empresa no es “faltaba mantenimiento”: es “aquello de la IA no funcionaba”.»*

**Contenidos.** Caducidad y dueño de cada fuente · calendario de revisión · apagado probado · escribir la
propia rúbrica · **y la rejilla de los doce**, que es la mitad nueva de este módulo.

**Qué construye.**
1. **La ficha de traspaso** (`06-traspaso.md`): qué fuente caduca y cada cuánto · **quién la revisa, con
   nombre** · qué batería se vuelve a pasar cuando se toque algo · cómo se apaga, probado · y qué hacer
   el día que falle.
2. **El calendario de revisión**, con la próxima fecha escrita.
3. **La rúbrica escrita por ella**, con al menos tres criterios negativos, sin usar la del curso — **y
   validada contra el CEBO 3**: si el cebo pasa su rúbrica, su rúbrica es blanda y se rehace.
4. **LA REJILLA DE LOS DOCE.** Sesenta minutos, una sola sesión: coge doce procesos suyos —de los que
   sobrevivieron al tachón de M0 y de los que fueron apareciendo en el campo 4 de las ocho preguntas
   fijas— y **asigna a cada uno uno de los seis veredictos**, con una frase de justificación que **cite un
   hecho observable** (un volumen, un documento, una consecuencia) y no una impresión. **Regla del
   cuatro:** al menos cuatro de los doce tienen que acabar en veredicto 1, veredicto 2 o zona prohibida.
   Y cada uno de esos cuatro lleva su casilla **«lo que sí se puede hacer alrededor»** rellena con un
   artefacto nombrable. Sale ordenada por `frecuencia × minutos ÷ riesgo`: **es su cola de después del
   curso**.
5. **El apéndice del escalón 4**, marcado como opcional y como lectura.

> **Por qué la rejilla está aquí, en la semana 14, y no en la semana 3.** Es la corrección de fondo que
> esta síntesis le hace a arq-2, y es lo que permite recuperar sus más de treinta juicios sin heredar su
> muro. Arq-2 pone la clasificación de doce tareas en las semanas 3–4, y paga tres facturas que sus
> propias autocríticas admiten: es **trabajo árido colocado exactamente donde más gente se cae**
> (momento 1); es una clasificación hecha **cuando menos criterio tiene**, sin nadie que la corrija
> (autocrítica 12); y **el orden de los seis módulos siguientes cuelga de ella**, así que un error ahí
> cuesta el curso entero.
>
> Aquí las tres facturas desaparecen: llega en la semana 14, cuando ya ha hecho la línea de corte, cinco
> dobletes con clave y tiene un sistema en producción, es decir, **con el criterio ya adquirido**; no
> gobierna el orden de nada, así que un error cuesta una fila y no un curso; y **cae exactamente en la
> meseta de novedad baja**, donde el material solo ya no tira y hace falta algo que produzca un
> resultado enseñable. Su salida —la cola de después del curso y la lista de noes— es además la materia
> prima directa del dossier de M7.
>
> **Lo que se pierde con este cambio, dicho aquí:** el criterio panorámico se entrena **después** de
> construir en vez de antes, así que no guía la elección del hilo. Lo asumo: para guiar la elección ya
> está el embudo de M0, que es más barato y más observable.

**Capacidad que entrena.** **Hacer que un artefacto sobreviva a su autora** y **clasificar procesos a
volumen**. La primera es puramente organizativa, no tiene nada de tecnológica y es la que más vale dentro
de tres años y en otra empresa: *¿qué de esto caduca y cada cuánto? ¿quién es la persona que lo mira?
¿cómo se apaga?* La segunda es el objetivo 4 en su forma más directa.

**Entregable.** Ficha de traspaso + calendario + rúbrica propia validada contra cebo + **la rejilla de los
doce firmada y fechada**.

**Duración realista.** 2 semanas, con aire.

**Mecanismo de autocorrección.**
- **La validación de su rúbrica contra el cebo 3** es un control positivo aplicado al instrumento que ella
  misma acaba de fabricar, y **es el criterio honesto de que ha terminado el curso**: cuando escribe las
  rúbricas, ya no lo necesita. El cebo 3 tiene además **función temporal declarada**: *si tu lectura como
  correctora se ha degradado en cuatro meses, se detecta aquí.*
- **Lista binaria de la ficha de traspaso:** *¿hay un nombre de persona en «quién lo mantiene»? ¿hay una
  fecha en cada fuente? ¿hay una fecha en «próxima revisión»? ¿está probado el apagado? ¿alguien que no
  sea yo podría encontrar la carpeta?*
- **La prueba del hueco:** dejar el sistema **una semana sin tocarlo** y comprobar qué se ha
  desactualizado. Es barata y es la única forma de ver la degradación antes de que la vea un cliente.
- **Lista binaria de la rejilla, doce ítems observables:** *¿hay alguna fila que no hayas hecho esta
  semana ni la pasada? ¿hay al menos cuatro veredictos 1, 2 o ZP? ¿cada veredicto cita un hecho
  observable? ¿algún «no» tiene la casilla «lo que sí» vacía? ¿hay más de tres veredictos 6? ¿alguna fila
  con consecuencia «dinero, plazo legal o visado» no lleva el tachón?*
- **La comprobación de las tres filas al azar** *(injerto de arq-2)*: coger tres filas y preguntarse
  *«¿la hice esta semana?»*. Si la respuesta es no en alguna, **la rejilla es aspiracional** y hay que
  corregirla contra lo que de verdad hace.

**Doblete (20 min): P32, mantenimiento de plantillas y FAQ.** **Veredicto correcto: 2, arreglar el proceso
primero.** Ahí el problema no es que falte automatización: **falta una fuente de verdad**. Se actualiza la
versión española del tarifario y las otras cinco se quedan viejas durante meses. Es el riesgo «alto y
silencioso» del inventario, y es **un hallazgo que aportar, no un fracaso**: en una empresa donde lo mal
visto es no automatizar, llegar diciendo *«esto todavía no se puede automatizar porque nadie sabe cuál es
el tarifario vigente en alemán»* es trabajo de valor. Va derecho al dossier de M7. Clave sellada.

**PUERTA M6 → M7:** la ficha de traspaso pasa su lista binaria · la rúbrica propia **no deja pasar el
cebo** · la rejilla tiene doce filas con al menos cuatro noes y sus «lo que sí».

---

## M7 · Capa 7 — Que lo adopten: evidenciar y contagiar · semanas 16–18

Desarrollado entero en §11. Resumen de ficha:

**Cambio mental.** *«Un artefacto que solo funciona conmigo delante no es un sistema de la academia: es
una manía mía. Lo que hace que otros lo adopten no es convencerles: es que puedan usarlo sin mí, que yo
pueda enseñar el número, y que sepa decir también qué no hace.»*

**Qué construye.** El **dossier de una cara** · la **demo de tres minutos** guionizada y cronometrada ·
**la semana sin ella** (el piloto) · la **conversación del proceso de otra persona** · la **lista de lo
que decidió no automatizar** (heredada de la línea de corte, los ocho dobletes y la rejilla de los doce) ·
y, si en M0 resultó que no existe, **una nota de media página para quien lleve la política de uso de IA**.

**Duración realista. 3 semanas**, y es el único módulo con una espera que no depende de ella: el piloto
dura una semana natural y no se puede acelerar.

**Mecanismo de autocorrección.** El piloto es la corrección y es binario, con su criterio negativo
—**la lista de arreglos tiene que tener al menos dos entradas**—, más la reproducción del número ±10 %,
más la prueba del pasillo con sus cuatro comprobaciones binarias, más la rúbrica del dossier con criterios
negativos, más PC-6. Detalle completo en §11.4.

**Doblete (20 min): el proceso de una compañera.** Es a la vez el octavo doblete y la primera semilla de
contagio. Sin clave sellada, y se dice por qué: es el único cuyo veredicto correcto no lo puede saber el
curso, porque depende de un proceso que el curso no conoce. **Lo que sí trae clave es la ejecución:** la
lista de comprobación de si la entrevista se hizo bien (§11.3, punto 7).

---

## 6.1 Vista de conjunto

| M | Sem. | Capa | Qué sale del expediente | Escalón del perfil | Corrección dominante | Puerta |
|---|---|---|---|---|---|---|
| **M0** | 1–2 | 0 · Ver el proceso | Elección puntuada + sombra + descripción real + ficha del entorno + 2 victorias | 1 · chat | Cronómetro · tres rechazos observables · la pantalla | Entorno sin «creo que» · 2 decisiones no previstas · repuesto firmado · línea base medida |
| **M1** | 3–4 | 1 · Criterio y línea de corte | Línea de corte con los 6 veredictos + ficha de criterio + anclas + batería sellada | 1 · chat | Ctrl+F · muestra apartada · **cebo 1** | Ficha pasa Ctrl+F · ≥1 trozo se queda · cada «no» con su «sí» · Tira con 2 columnas |
| **M2** | 5–6 | 2 · Contexto con procedencia | Mapa de datos + fuentes fechadas + asistente que cita y se abstiene + traslado | 1 · chat | Batería (col. 3) · lista binaria · prueba de la compañera | 5/5 típicos · **≥5 usos espontáneos en una semana** · traslado hecho |
| **M3** | 7–8 | 3 · Disparador | Disparador + tope + apagado probado + notación neutra | 2 · automatización | Se dispara o no · **el caso que NO debe disparar** | Seis casos correctos · tope y apagado probados · **ha visto fallar algo y sabe por qué** |
| **M4** | 9–11 | 4 · Juicio y frenos | Temas prohibidos + 6 condiciones de parada + revisor con nombre y hora + plan de fallo + 5 preguntas sobre herramienta ajena | 3 · agentes | Cinco paradas + el sexto que no para · rúbrica negativa · **cebo 2** | Cinco paran, el sexto no · marca y motivo · nombre y hora · nada sale sin firma |
| — | — | — | **FRONTERA DECLARADA: al acabar M4 ya hay curso** | — | — | — |
| **M5** | 12–13 | 5 · Medir | Evaluación de media página + prueba ciega + lectura de la Tira | transversal | **La prueba ciega** | Resta hecha · amenaza nombrada · una frase por columna |
| **M6** | 14–15 | 6 · Sobrevivir sin ti | Ficha de traspaso + rúbrica propia + **la rejilla de los doce** | transversal | Su rúbrica contra el **cebo 3** · prueba del hueco | Traspaso completo · rúbrica no deja pasar el cebo · doce filas con ≥4 noes |
| **M7** | 16–18 | 7 · Que lo adopten | Dossier + demo + **la semana sin ella** + lista de noes + entrevista ajena | **adicional** | **El piloto**, con ≥2 arreglos | — |
| — | — | apéndice | *(lectura opcional: qué hay más arriba)* | 4 · opcional | ninguna | — |

**Herramientas nuevas en 18 semanas: dos o tres**, según lo que su proceso pida —un asistente con
fuentes, un disparador, y en algunos casos una aplicación en lote— y ninguna se introduce antes de que el
proceso se haya quedado corto sin ella. **Coste: cero euros.** Si el curso acaba costando dinero, el
diagnóstico estaba mal.

---

# 7. LA ESCALERA DE CAPACIDADES DEL PERFIL, Y DÓNDE SE CUMPLE CADA PELDAÑO

El perfil pide una progresión explícita: **usar mucho mejor el chat → automatizaciones → agentes cuando la
tarea lo justifique → herramientas avanzadas, al final y opcionales.** Este diseño **la respeta
literalmente**, pero no la usa como plan de estudios, y la diferencia importa:

> **La escalera no es el temario: es lo que le pasa a un proceso cuando lo aprietas.** No se «suben
> escalones» porque el calendario lo diga: se choca con techos dentro de la misma cosa, y cada techo se
> siente en su trabajo real antes de que nadie lo explique.

| Peldaño del perfil | Dónde se cumple | Qué es el techo que lo empuja al siguiente, **sentido y no leído** | Cómo se ve en las cinco preguntas |
|---|---|---|---|
| **0 · Chat a pelo** *(donde está hoy)* | Estado de partida, medido en M0 y M1 con la primera columna de la Tira: **saca 4 de 10** | *«Cada conversación empieza en blanco y le vuelvo a explicar la academia. Y no sé con qué cuenta entro ni qué protege esa cuenta»* | P3 = «lo que le pego en el momento» |
| **1 · Usar mucho mejor el chat** | **M0** (instrucciones permanentes, día 1) → **M1** (el criterio escrito) → **M2** (fuentes propias con fecha, cita y «no lo sé») | *«Se acuerda de sus instrucciones, no de lo que pasó ayer. Y sigue esperando a que yo lo abra cada vez»* | **P3 pasa a «fuentes que yo controlo y fecho»**. Y aquí es donde se gana casi toda la calidad del curso |
| **2 · Automatizaciones** | **M3** (disparador por reloj, ruta A; por suceso, ruta B) | *«Dispara los lunes. No reacciona a que **haya pasado algo**.»* Y después: *«siempre el mismo camino: el caso que no previste sale mal, y sale mal en silencio»* | **P1 pasa de «yo» a «un reloj» y luego a «un suceso»**; P2 se congela en «yo, de antemano» |
| **3 · Agentes, cuando la tarea lo justifique** | **M4**, en su forma alcanzable: **juicio confinado a dos o tres puntos**, con frenos y condiciones de parada | *«Sigue siendo un camino que dibujé yo»*. Y la conclusión honesta: **su escalón 3 realista es un proceso con juicio, no un agente autónomo**, por licencia, permisos y datos — no por capacidad suya | **P2 se abre en dos o tres puntos concretos**; P4 pasa a «escribir en lo mío»; **P5 no cambia nunca** |
| **4 · Avanzado (tipo terminal)** | **Apéndice de lectura, sin entregable.** *Si termina el curso sin abrirlo, el curso ha funcionado igual*, y eso va en su primera línea | La condición que lo activaría: una tarea que exija **procesar decenas de ficheros locales de forma repetida** — revisar doscientos contratos de estancia larga buscando una cláusula | P2 pasa entera al sistema. **Y ahí está el pago: renuncia a ser predecible** |

**Tres decisiones sobre la escalera que conviene dejar escritas:**

1. **El escalón 5 se conoce, no se sube — pero la afirmación no se congela.** El módulo no dice «los
   agentes están fuera de tu alcance», que es una falsedad desmotivadora esperando a ocurrir. Le hace
   **rellenar la ficha de cinco preguntas para el agente que tenga delante ese día** y comprobar tres
   cosas: ¿lo cubre mi plan? ¿puede actuar sobre los recursos donde vive mi trabajo? ¿puedo ver qué hizo?
   Si en 2028 las tres son sí, **el módulo funciona mejor, no peor.**
2. **Existe un escalón −1, y va antes que todos los demás: NI IA.** Es el veredicto 1 de la rejilla, con
   su prueba de la servilleta y su ejemplo canónico suyo (P02, el presupuesto). Un curso que empieza la
   escalera en el peldaño 1 enseña a subir; uno que empieza en el −1 enseña a decidir.
3. **La escalera se lee, no se cuenta.** La lectura de la Tira en M5 —cinco columnas fechadas de su propio
   trabajo— produce la conclusión que ninguna lección puede producir igual de bien: **subir de escalón no
   mejora la respuesta; cambia quién la pide y cuánta autonomía has cedido.** Esa es la frase que le
   permitirá juzgar cualquier herramienta futura sin que se la vendan.

---

# 8. LA SEPARACIÓN CRITERIO / CLICS

No es una recomendación de estilo. Es **la convención de producción del material**, y si se relaja, el
curso deja de ser agnóstico en tres módulos.

## 8.1 Tres registros, no dos

Dos registros dejan un hueco **justo donde está el valor**: cómo encuentras esa función en una herramienta
que nunca has visto. Por eso son tres *(injerto de arq-1 §4.1, y es la pieza de portabilidad que el juez 3
señala como decisiva)*.

| Registro | Qué contiene | Dónde vive | ¿Caduca? |
|---|---|---|---|
| **EL CRITERIO** | Por qué se hace así · qué problema resuelve · cómo se decide si toca · cómo se comprueba · qué puede salir mal · el techo | Fichero de lección | **No** |
| **LAS SEÑAS** — *cómo reconocerlo en cualquier herramienta* | Descripción funcional de qué hay que buscar, y **las señas que distinguen esta capacidad de otra que se le parece**, con su condición de fallo | Fichero de lección, en caja aparte marcada | **Casi no** |
| **LOS CLICS** | Rutas, nombres de botón, capturas, límites numéricos, planes | **Otro fichero**, fechado, uno por entorno | **Sí, y da igual** |

## 8.2 Qué es exactamente el registro de señas, con su ejemplo

Es un **test funcional de reconocimiento**, no una tabla de nombres de producto. Para la capacidad de la
capa 2:

> **Qué estás buscando**, en palabras que no dependen de ningún producto: un sitio donde se cree **un
> espacio con nombre**, se le adjunten documentos, y las respuestas se limiten a ellos.
>
> **Las tres señas que te dicen que has encontrado la capacidad correcta:**
> 1. **Las fuentes siguen ahí mañana**, sin volver a subirlas.
> 2. **La respuesta dice de qué documento sale.** Si no cita, no es esto.
> 3. **Puedes listar qué hay dentro** y quitar una fuente sin rehacerlo todo.
>
> **Si falta cualquiera de las tres, lo que tienes es un adjunto en una conversación**, que es otra cosa y
> dura lo que dure esa conversación. Es la confusión más frecuente y la que hace que la gente crea que
> ya tiene esto montado cuando no lo tiene.
>
> **Señas de que la herramienta NO sirve para este uso:** no permite quitar fuentes · mezcla lo que le has
> dado con lo que sabe de fuera sin distinguirlo · no hay forma de ver cuántas fuentes hay.

Eso es lo que sirve el día que entre en otra empresa y le abran una pantalla desconocida. Una tabla de
tres nombres de producto, por su propia declaración, **caduca por completo**.

## 8.3 Estructura de ficheros y las cinco reglas de producción, todas mecánicamente comprobables

```
curso/
  M3/
    M3.1-capa.md              ← EL CRITERIO + LAS SEÑAS. Sin fecha. Sin nombres de producto
    M3.1-ejercicio.md         ← EL EJERCICIO. Tampoco nombra productos
    M3.1-rubrica.md
    M3.1-solucion.md
    M3-cierre.md              ← 5 preguntas + pregunta fija + doblete. Nunca nombra productos
    clics/
      M3.1-clics-<entorno-actual>.md   ← fechado, reemplazable
      M3.1-clics-<otro-entorno>.md     ← fechado, para la prueba de traslado
  comun/
    datos-volatiles.md        ← TODO número: cupos, límites, precios, qué edición incluye qué
    tres-nombres.md           ← equivalencias de nombres. La única página que caduca entera
    cuando-no-coincide.md     ← qué hacer cuando el manual y la pantalla discrepan
    protocolo-ia.md           ← las siete reglas de corrección con IA
    claves/                   ← claves selladas: batería, ocho dobletes, tres cebos
    expediente-modelo/        ← el recorrido completo hecho sobre P27
```

1. **Ningún nombre de producto en un fichero de criterio, de señas, de ejercicio o de cierre.**
   Comprobación real, no aspiracional: un `grep -iE` con la lista de productos sobre esos ficheros tiene
   que devolver **cero líneas**. Si devuelve alguna, esa frase va a clics o se reescribe.
2. **Ningún número volátil fuera de `datos-volatiles.md`.** Cupos, límites, precios y qué edición incluye
   qué se **referencian**, no se copian. Actualizar el curso es actualizar un fichero, no treinta.
3. **Ningún ejercicio puede depender de una captura ni de una ruta de menú.** Prueba mecánica, ejecutada
   una vez sobre el material terminado: **se borra el directorio `clics/` entero y todos los ejercicios
   siguen siendo enunciables**. Uno que deje de poderse hacer está mal escrito y se reescribe.
4. **Todo fichero de clics abre con la misma cabecera:** *«Verificado el <fecha> en <entorno>. **Si algo
   no coincide con lo que ves, tu pantalla tiene razón y este texto no.** Ve a `cuando-no-coincide.md`.»*
5. **Todo fichero de clics termina con la misma línea:** *«Si esto ha cambiado, lo que sigue siendo verdad
   está en `M3.1-capa.md`.»* Es una línea, y es lo que impide que un botón renombrado se lea como que el
   curso entero ha caducado.

**Y las dos reglas de redacción que deciden en qué mitad va una frase a las tres de la mañana** *(de
arq-3 §5.2, y son las mejores del corpus porque atacan el fallo real):*

> **La regla del sujeto.** En un fichero de criterio, **el sujeto gramatical de cada frase es el proceso,
> el dato o ella**. Nunca un producto. *«El proceso necesita saber de qué documento sale cada dato»* es
> criterio. *«El asistente admite diez ficheros»* es clic, porque el sujeto es la herramienta.
>
> **La prueba del sustituto.** Sustituye cada nombre de producto por «la herramienta» y relee el párrafo.
> Si deja de tener sentido, el párrafo pertenece a clics. Si sigue teniendo sentido, **entonces borra el
> nombre para siempre**: no hacía falta. **Esta segunda mitad es la que de verdad limpia el texto**,
> porque el fallo típico no es escribir un párrafo de clics en la mitad de criterio: es dejar nombres de
> producto decorativos en frases que no los necesitaban.

Ejemplos de la conversión, con material real de este curso:

| No se escribe | Se escribe |
|---|---|
| «Crea un Gem» | «Guarda este asistente con nombre, para poder reabrirlo sin volver a explicar el contexto» |
| «Sube el tarifario al cuaderno» | «Dale como fuentes los documentos sobre los que quieres que responda, y exige que cite de cuál sale cada dato» |
| «Workspace Studio no admite unidades compartidas» | «Comprueba, **antes de diseñar nada**, sobre qué ficheros puede actuar tu herramienta de automatización: casi todas tienen restricciones con recursos compartidos» *(y el límite concreto, en clics)* |
| «Pon una acción programada semanal» | «Elige qué lo dispara: una fecha del calendario o un suceso. La diferencia decide qué casos vas a poder atender» |

**Nótese la costura de la tercera fila, que es la correcta y la que responde a la objeción del juez 3
sobre la cuarta columna del embudo: el límite concreto de la plataforma está en clics; la instrucción de
comprobarlo antes de diseñar está en criterio.**

## 8.4 Las tres pruebas de portabilidad, y qué demuestra cada una

La agnosticidad no se declara: se ejecuta tres veces, con entregable, y **con restricción de datos**.

| # | Dónde | Qué se hace | Coste | Qué demuestra |
|---|---|---|---|---|
| **P1** | M2 | **Reconstruye el mismo asistente en otra herramienta** —ella ya usa ChatGPT por su cuenta— **usando solo material verde** (tarifario, calendario, condiciones, que **no son datos personales**). Le pasa las mismas diez preguntas | 25 min | Que el criterio y las fuentes viajan. Y si **no lo consigue en 20 min**: aprendió la ruta, no la capacidad |
| **P2** | M3 | **Sobre papel y documentación, sin dar de alta nada:** escribe su flujo en notación neutra `DISPARADOR → PASO → CONDICIÓN → SALIDA` y localiza cada pieza en la documentación de **otra** plataforma de automatización | 20 min | Que sabe **leer el catálogo de pasos de una herramienta que no ha visto nunca**. Es la habilidad que usará dentro de tres años |
| **P3** | M4 | **La ficha de cinco preguntas para una herramienta que el curso no enseñó**, más su fila en la Lista de techos con la **condición** que la activaría | 20 min | Que el clasificador funciona **sin el curso** |

Ficha de P1, y se corrige sola:

| Qué viajó tal cual | Qué hubo que rehacer | Qué techo cambió |
|---|---|---|
| La ficha de criterio · las fuentes con su fecha y su dueño · la batería de diez casos · la regla de «no lo sé» · la línea de corte | Dónde se guarda · cómo se llama · cuántos ficheros admite · dónde se pega la instrucción | Cuántas fuentes acepta · si cita el fragmento o solo el fichero · si conserva la instrucción entre sesiones |

> **Lo que se aprende no es «la otra herramienta también sirve». Es que el ochenta por ciento de tu
> trabajo era el criterio y las fuentes, y eso no estaba dentro de ninguna herramienta.**
>
> **Restricción de datos, y es contenido, no prudencia decorativa:** P1 se hace **con material verde
> exclusivamente**. Su cuenta personal no tiene contrato de encargado del tratamiento, y por ahí no pasa
> ni un dato de un alumno. Que la prueba de portabilidad sea también un ejercicio de semáforo no es
> casualidad: es el diseño. **P2 y P3 no tocan ningún dato porque son sobre papel.**

**Honestidad sobre el alcance de las tres, porque su nombre promete más de lo que dan:** demuestran que
**el criterio viaja**, no que ella sabría trabajar de verdad en otra herramienta con datos reales. Es
suficiente para el objetivo declarado —saltar sin fricción, no ser experta en dos entornos— pero hay que
llamarlas por lo que son: pruebas de portabilidad **del criterio**.

## 8.5 Ejemplo real: las tres mitades de una misma lección

Se elige **M3.1, «Que ocurra sin que lo pidas»**, porque es donde la tentación de escribir un manual de
producto es máxima —es, literalmente, ir a un sitio y pulsar un botón—.

### `M3/M3.1-capa.md` — EL CRITERIO *(sin fecha, sin nombres de producto, sin capturas)*

> ## Para qué sirve esto en tu proceso
>
> Hasta ahora tu proceso funciona **cuando tú te acuerdas**. Esa dependencia tiene dos costes que no se
> ven: los días de mucho trabajo —que son justo cuando más falta hace— es el primer sitio donde se cae; y
> no se puede repartir, porque «acordarse» no se delega. Esta capa quita tu dedo de en medio.
>
> ## Qué es un disparador, y por qué es la decisión y no un detalle
>
> Un disparador es **la condición que hace que el trabajo empiece sin ti**. Solo hay dos clases, y la
> diferencia entre ellas decide qué casos vas a poder atender:
>
> - **Por calendario.** «Cada lunes a las nueve.» Sirve cuando el trabajo se acumula y se puede tratar en
>   lotes. Es el más fácil de razonar, porque siempre sabes cuándo va a ocurrir.
> - **Por suceso.** «Cuando entra algo que cumple X.» Sirve cuando la respuesta tiene que llegar cerca del
>   hecho. Es más útil y más difícil de razonar, porque **no sabes cuántas veces va a ocurrir**.
>
> **Un lunes no es un suceso.** Si tu proceso empieza porque llegó algo, un disparador de calendario te
> obliga a esperar, y esa espera puede ser exactamente lo que hacía valioso el proceso.
>
> ## Las tres cosas sin las cuales un disparador no está terminado
>
> **1. Un tope.** Un número por encima del cual **no hace nada y te avisa**. *Un sistema que produce
> cuarenta borradores un lunes de julio no ayuda, entorpece.* El tope no es una precaución: es lo que
> convierte una automatización en algo de lo que te puedes fiar, porque **su comportamiento en el peor día
> es conocido**.
>
> **2. Un apagado que hayas probado.** No que sepas que existe: que lo hayas apagado y vuelto a encender.
> **Un sistema que no sabes apagar no está terminado.** El día que falle vas a estar nerviosa, y no es el
> momento de averiguar dónde está el interruptor.
>
> **3. Una salida que prepara, no que envía.** *Automatiza la lectura y la preparación; la escritura hacia
> fuera la firma una persona.* Y el motivo, que no es prudencia: **si tu sistema solo prepara, todos sus
> errores son recuperables**, y eso te permite equivocarte mucho, que es exactamente lo que hace falta
> para que esto mejore.
>
> ## Cuándo NO poner un disparador
>
> - **Si todavía no usas el artefacto por tu cuenta.** *(Es la puerta de este módulo: cinco usos
>   espontáneos en una semana. Automatizar algo que no usas es multiplicar un error que ni siquiera has
>   visto.)*
> - **Si el proceso ocurre menos de una vez por semana.** El coste de montar y mantener no se recupera.
> - **Si la salida tiene que salir hacia fuera sin que nadie la mire.** Entonces el problema no es el
>   disparador: es que ese trozo no debería estar en la parte entregable de tu línea de corte.
>
> ## El techo de esta capa
>
> Un disparador hace que el trabajo empiece solo, **pero el camino sigue siendo el que dibujaste tú**. El
> caso que no previste sale mal, y sale mal **en silencio**, que es lo peor. Eso es lo que pide la capa
> siguiente.

### `M3/M3.1-capa.md`, caja de señas — CÓMO RECONOCERLO EN CUALQUIER HERRAMIENTA

> **Qué estás buscando:** un sitio donde se declare *qué hace que esto empiece* por separado de *qué pasa
> después*. Casi siempre está en un apartado que habla de «automatizaciones», «flujos», «tareas» o
> «acciones».
>
> **Las tres señas de que has encontrado un disparador de verdad:**
> 1. Puedes **elegir entre al menos una condición de reloj y una condición de suceso**. Si solo hay
>    reloj, tienes media capacidad y conviene saberlo antes de diseñar.
> 2. Existe una **lista visible de lo que está activo**, y puedes desactivar una cosa sin borrarla.
> 3. Hay algún sitio donde **ver que se ejecutó** — un historial, un registro, un aviso. **Si no puedes
>    comprobar que se ejecutó, no puedes fiarte de que se ejecutó.**
>
> **Señas de que no sirve para tu caso, y hay que verlas antes y no después:** no dice sobre qué recursos
> puede actuar · no hay forma de limitar cuántas veces se ejecuta · no hay historial.
>
> **Y la comprobación que hay que hacer siempre, en cualquier herramienta y en cualquier año, antes de
> diseñar nada:** *¿sobre qué ficheros y qué buzones puede actuar esto — no leer: actuar— con mi cuenta y
> sin pedirle permiso a nadie?* Casi todas las herramientas de automatización tienen restricciones con
> recursos compartidos, y esa restricción decide qué procesos puedes automatizar y cuáles no.

### `M3/clics/M3.1-clics-<entorno-actual>.md` — LOS CLICS *(fechado y reemplazable)*

> *Verificado el 22 de agosto de 2026 en el entorno de trabajo actual. **Si algo no coincide con lo que
> ves, tu pantalla tiene razón y este texto no.** Ve a `cuando-no-coincide.md`.*
>
> **A · Ruta obligatoria: disparador por calendario, sin salir del chat que ya usas.**
> 1. En la aplicación de chat de tu cuenta de trabajo, busca la sección de acciones programadas.
> 2. Escribe la instrucción como si se la dieras a alguien un lunes por la mañana, y fija la frecuencia.
> 3. Límite de acciones activas a la vez → `comun/datos-volatiles.md`.
>
> **B · Ruta opcional: disparador por suceso, con la herramienta de automatización de la suite.**
> 1. Entra con la cuenta de trabajo. Si no te deja, no es un fallo tuyo: tu administrador no la ha
>    activado. Ve a `cuando-no-coincide.md`. **La ruta A basta para cerrar esta capa y para pasar la
>    puerta.**
> 2. Elige el disparador de la lista. 3. Añade los pasos. 4. La salida: **borrador en tu bandeja**, fila
>    en una hoja o aviso. **Ningún paso de esta lección envía nada a un cliente.**
>
> **C · Los límites que te vas a encontrar hoy en este entorno** *(y por eso la cuarta columna del embudo
> de la semana 1 descartó los procesos que solo viven en recursos compartidos)*: los flujos **fallan con
> unidades compartidas, carpetas compartidas y hojas con referencias externas** · **un solo disparador por
> flujo** · la interfaz solo muestra un número limitado de etiquetas · tu administrador puede tener pasos
> desactivados y no hay forma de saberlo hasta que lo intentas.
>
> **D · Dónde se apaga.** En la misma pantalla donde se crea. **Apágalo y vuelve a encenderlo ahora
> mismo**, antes de seguir: es el ejercicio, no un consejo.
>
> **Cifras y límites** → `comun/datos-volatiles.md`. *No las copies aquí.*
> *Si esto ha cambiado, lo que sigue siendo verdad está en `M3.1-capa.md`.*

**Qué demuestra este ejemplo.** La mitad de criterio ocupa el doble que la de clics, **no menciona ni una
vez el nombre de ningún producto**, y seguiría siendo válida palabra por palabra si mañana su empresa
cambiara de proveedor. La caja de señas cubre el hueco que los otros dos registros dejan. Y la de clics es
sustituible en veinte minutos por alguien que no haya escrito el curso.

## 8.6 Qué se pierde con esta convención, dicho aquí

- **La lección se lee peor de corrido.** Saltar entre ficheros tiene un coste de atención real. Mitigación:
  el fichero de clics es corto, numerado y siempre en el mismo sitio, y la lección termina con un enlace
  único. No lo elimina.
- **Redactar en capacidades es más lento y más abstracto**, y la abstracción es exactamente lo que peor le
  sienta a alguien sin base técnica en las primeras semanas. Compensación: el ejercicio y la rúbrica viven
  en la mitad que no caduca, así que el mantenimiento del curso baja de treinta ficheros a diez. **Y si el
  material resultara demasiado abstracto, la reparación correcta no es volver a mezclar: es engordar los
  ficheros de clics y adelgazar el criterio.**

---

# 9. «SABER QUÉ EXISTE», Y CÓMO SE ENSEÑA A NO USAR IA CUANDO NO TOCA

## 9.1 El objetivo 1, resuelto con cuatro mecanismos y ningún listado de productos

El objetivo 1 del perfil es *«saber qué existe: que existen agentes, que existen automatizaciones, qué se
puede automatizar de su trabajo y qué no»*. **Los tres términos van pegados a su trabajo.** No pide un
mapa del sector: pide saber qué hay disponible para lo que ella hace. Un curso que conteste con un
recorrido de productos está contestando a otra pregunta, y además contesta con la mitad que caduca.

Este es el objetivo peor servido por una columna vertebral de un solo proceso, y por eso lleva cuatro
mecanismos y no uno. **Tres de los cuatro son injertos.**

**Mecanismo 1 · La rejilla de los seis veredictos, usada más de treinta veces** (§4.2). Es el catálogo, y
solo se aprende asignándolo. La diferencia entre *«un agente decide sus propios pasos»* y *«el triaje de
reseñas es lo único de mi lista donde hay que evaluar algo para saber por dónde seguir»* es la diferencia
entre una definición y un conocimiento.

**Mecanismo 2 · La Lista de techos** (§4.5). El catálogo no se enumera: **se genera**. Cada capa declara
qué no puede hacer y **qué clase de cosa lo rompería**, y la tercera columna son **condiciones**, que es lo
que convierte un catálogo en criterio. Y la propiedad que lo hace funcionar: **una fila se escribe en el
momento en que el proceso choca con el techo**, no en un módulo de panorama. La fila del agente se escribe
en la capa 4, cuando ya tiene un sistema con juicio en dos puntos y entiende exactamente qué le falta.
Antes de eso, «agente» es una palabra; ahí es una carencia concreta con nombre.

**Mecanismo 3 · Los ocho dobletes con clave sellada** (§9.2). Ocho encuentros con procesos que **no son el
suyo** y que piden cosas que su proceso no pide.

**Mecanismo 4 · La caja del fondo, una sola vez, en M4 y no antes.** Media página, con **el eje puesto en
la condición y no en el producto** — que es la diferencia entre una tabla que hay que rehacer cada año y
una que se revisa:

| Qué haría falta para que me tocara | La clase de cosa que lo haría | Qué es hoy, para reconocerlo si me hablan de ello |
|---|---|---|
| Tener que actuar sobre un sistema que no está en mi suite (el software académico, la pasarela de pago, el mensajero, el portal de una agencia) | Una plataforma de automatización externa | *(nombres en `tres-nombres.md`)*. Ojo: **mete un proveedor más entre mis datos y yo, y eso hay que pesarlo** |
| Tener una tarea cuyos pasos no pueda dibujar de antemano | Un agente: le das objetivo y límites y decide los pasos | Están detrás de planes que mi empresa casi con seguridad no tiene, y necesitarían actuar sobre recursos compartidos |
| Necesitar que una herramienta lea de una fuente mía con permisos acotados | Un acceso acotado y el estándar por el que se conectan | Para mí hoy es **vocabulario, no herramienta**. Lo que sí me sirve es el principio: **conectar solo a lo necesario, y a una carpeta, no al disco** |
| Tener que procesar decenas de ficheros locales de forma repetida | Un agente con acceso al sistema de ficheros | Revisar doscientos contratos de estancia larga buscando una cláusula sería el caso |
| Que mis fuentes pasen de decenas a cientos y el asistente empiece a perderse | Arquitecturas de recuperación sobre corpus grandes | Con veinte fuentes bien fechadas no me hace falta nada de eso |
| Que me hablen de un sitio «de la misma empresa, gratis, donde se prueban prompts» | Una superficie de desarrollador | **Trampa silenciosa:** sus propios términos dicen que no metas información personal. Parece seguro porque entras con la cuenta de siempre, y no lo es |

**Y la segunda vuelta, en M7** *(injerto del juez 3)*: releer la rejilla de los doce y la caja del fondo y
marcar **qué veredictos y qué condiciones han cambiado** en cuatro meses. Es lo que convierte un catálogo
en un instrumento con vida, y es **el ensayo de lo que va a tener que hacer sola cada año**.

**Hasta dónde llega esto, honestamente.** Cubre lo que su proceso toca, lo que los dobletes rozan y lo que
la rejilla clasifica: más de treinta procesos. **No cubre** el panorama del sector ni le da una opinión
informada sobre familias de herramientas que no ha visto. Si en dos años le preguntan «¿qué herramientas
de automatización conoces?», la respuesta honesta de este curso es *«conozco la anatomía y sé leer el
catálogo de pasos de una que no he visto nunca»* — que es mejor respuesta de lo que parece, pero no es la
que da un curso de panorama, y este curso no lo es a propósito.

## 9.2 El Doblete: cada capa se repite en seco sobre un proceso que no es el suyo

**El mecanismo.** Al cerrar cada capa, **veinte minutos**, sobre papel, aplicando la misma capa a un
proceso distinto de su lista. No se construye nada. Se contestan cuatro preguntas y se firma un veredicto
**de los seis**.

```
DOBLETE de la capa __ · proceso: P__ · fecha: ____ · 20 minutos

1. Si tuviera que aplicar esta capa aquí, ¿qué haría exactamente? (3-5 líneas)
2. ¿Qué cambiaría respecto a lo que hice en mi proceso?
3. ¿Hay algo de esta capa que aquí NO tendría sentido? ¿Por qué?
4. VEREDICTO (uno de los seis, o ZP): ____   Motivo, citando un hecho del proceso: ____

— y solo después de firmar: abre `comun/claves/doblete-<capa>.md` y anota en qué coincides y en qué no.
```

> **LOS OCHO DOBLETES LLEVAN CLAVE SELLADA, Y ESTE ES EL INJERTO QUE MÁS ARREGLA DEL DISEÑO ORIGINAL.**
> El juez 2 lo caza con precisión: en arq-3, los ocho dobletes —**toda la maquinaria de transferencia del
> curso**— tenían corrección **solo formal**: la lista comprobaba que existieran y que sumaran la cuota,
> no que el veredicto fuera correcto. Y lo absurdo es que **la respuesta correcta de cada uno ya estaba
> escrita** en el propio documento; solo faltaba sellarla como clave, que es la convención que el curso
> aplica religiosamente a la batería.
>
> Con la clave sellada, los ocho dobletes dejan de ser un ritual y pasan a ser **ocho contrastes con
> oráculo**, que es la única forma sin profesor de saber si el criterio generalizó o se pegó al caso. Y
> resuelve parcialmente la renuncia al doble hilo (§17.2): recupera ocho puntos de calibración externa sin
> ejecutar un segundo proceso.
>
> **Y la regla de lectura de la clave, que va escrita:** *si no coincides, no reescribas tu veredicto.
> Escribe en una línea por qué creías lo que creías. Ese desacuerdo es el dato, y es material del punto
> de consulta.*

**Los ocho dobletes, asignados a propósito para que cada capa choque con un tipo distinto de «no»:**

| Capa | Doblete | Veredicto de la clave, y qué enseña |
|---|---|---|
| 0 · Ver el proceso | **P29** emergencias 24 h | **ZP.** Un proceso de riesgo crítico, no determinista y bajo presión no se mapea para delegarlo: se mapea para **no** delegarlo. Enseña que describir un proceso no compromete a automatizarlo |
| 1 · Criterio | **P02** presupuestos | **Veredicto 1, NI IA.** Es aritmética sobre una tabla de precios. Escribir el criterio es lo que hace visible que se cumple con una fórmula. **Es el ejemplo canónico del escalón −1** |
| 2 · Contexto | **P08** carta de aceptación para visado | **ZP**, y el motivo transferible no es «es difícil» sino **«la normativa cambia de un año para otro, y congelar dentro de un artefacto un conocimiento que caduca es fabricar un error futuro»** |
| 3 · Disparador | **P30** parte semanal a dirección académica | **Veredicto 5, con la mínima IA posible.** Determinista puro. Enseña que «automatizar» no significa «meter un modelo» |
| 4 · Juicio y frenos | **P28** respuesta a reseñas online | **Veredicto 6 con recorte:** clasificar y preparar sí, publicar **nunca** — y el motivo no es de calidad, es de datos: confirmar públicamente que alguien fue alumno y tuvo un problema **ya es una cesión** |
| 5 · Medir | **P12** check-in del lunes | **No se deja medir así.** Su valor es la percepción de calidad de toda la estancia, y eso no se mide en minutos por unidad. Enseña **deficiencia del criterio** con un caso de su casa |
| 6 · Sobrevivir sin ti | **P32** mantenimiento de plantillas y FAQ | **Veredicto 2, arreglar el proceso primero.** No falta automatización: **falta una fuente de verdad**. Es un hallazgo que aportar, no un fracaso |
| 7 · Que lo adopten | **el proceso de una compañera** | Sin clave de veredicto —el curso no conoce ese proceso—, pero **con clave de ejecución**: la lista de si la entrevista se hizo bien |

**Y la cuota, que defiendo como tal:**

> **De los ocho dobletes, al menos tres tienen que terminar en «no aplica», «ni IA» o «arreglar el proceso
> primero». Si tienes menos de tres, no has transferido: has repetido. Vuelve.**

La justificación no es estética: cruzando los 32 procesos con lo que la plataforma puede hacer de verdad,
**el reparto real da entre cinco y siete noes por cada doce procesos**. Tres de ocho es un suelo prudente.
Su función psicológica es la que importa: **convierte el «no» en algo que hay que encontrar**, y desactiva
de raíz el sesgo que produce un curso de IA por su mera existencia — preguntarle a un curso de IA si algo
debe hacerse con IA tiene un sesgo obvio hacia el sí.

**El riesgo de la cuota, y por qué aquí es menor que en arq-2.** Una cuota puede fabricar noes de
conveniencia, y eso depende de su honestidad en el peor sitio posible: consigo misma. **Pero aquí hay
clave sellada.** Un no de conveniencia sobre un doblete cuyo veredicto correcto es «aplica igual» se
detecta al abrir la clave. Es exactamente lo que arq-2 no podía hacer con la regla del cuatro sobre su
Semanario, y es la razón por la que la cuota de los dobletes es más fiable que la cuota de la rejilla.
*(En la rejilla de los doce no hay clave posible: ahí la señal de fallo es la comprobación de las tres
filas al azar y el ítem «existe un veredicto 1 o 2 que puse para llegar a cuatro, no porque lo crea».)*

**Coste total: ocho por veinte minutos = menos de tres horas en dieciocho semanas.** Y cada uno de esos
ocho juicios se emite **inmediatamente después de haber hecho esa misma cosa de verdad**, que es cuando un
juicio sobre un proceso ajeno vale algo.

## 9.3 Cómo se enseña a NO usar IA cuando no toca — siete mecanismos, y los siete se evalúan

Ninguno es una advertencia suelta. **Todos producen algo que se puntúa**, porque lo que no se evalúa no se
hace.

**1 · La línea de corte: el «no» es interior al proceso.** Es el mecanismo propio de esta columna
vertebral y el más fuerte de los siete. El entregable central de M1 no es «qué automatizo» sino **el
proceso partido en trozos, cada trozo con veredicto y motivo**. Rúbrica tajante: *si no hay ningún trozo
que se quede contigo, está mal resuelto*, y *si el motivo es «es difícil», está mal*. Los motivos legítimos
son tres:

| Motivo legítimo | Ejemplo de su casa |
|---|---|
| **Riesgo**: el error lo paga un cliente, una administración o la caja | Cualquier trozo que toque importes, plazos de visado o disponibilidad de alojamiento |
| **Conocimiento que caduca**: la regla cambia más deprisa de lo que se puede mantener el artefacto | Requisitos consulares, que se reordenaron en 2025 y volverán a cambiar |
| **No hay fuente de verdad**: nadie puede nombrar el documento vigente ni su dueño | El tarifario en alemán, que lleva meses desactualizado y nadie lo sabe |

Y el cuarto, que no es de riesgo sino de escalón y merece nombre propio porque es el que nadie enseña:
**este trozo no necesita un modelo de lenguaje, necesita una fórmula, un filtro o un calendario.** Es el
escalón −1 y su ejemplo canónico es suyo: **el presupuesto es aritmética sobre una tabla de precios**.
Meter un modelo ahí no es ineficiente: **es introducir un error posible donde no lo había.**

**2 · La regla del cuatro en la rejilla de los doce** y **la regla de los tres noes en los dobletes**
(§9.2). Con la diferencia de fiabilidad ya dicha: la de los dobletes tiene clave; la de la rejilla, señal
de fallo.

**3 · «Lo que sí se puede hacer alrededor», exigido con artefacto nombrable.** Es la mejor contramedida
escrita en cualquiera de las tres arquitecturas contra el momento en que un «no» se lee como *«entonces
esto no me sirve para lo que de verdad me duele»*. **El módulo no termina con una lista de renuncias:
termina con un sí concreto por cada no.** Ejemplos que trae el material:

| No se puede | Pero sí se puede |
|---|---|
| **P17** matching con familias (salud, religión, potencialmente orientación sexual en una casilla de texto libre) | **P18** confirmación de alojamiento: 700–800 al año, plantilla con diez variables, sin datos de salud. Y **P20** triaje de incidencias: clasificar y enrutar sí, responder no |
| **P08** redactar la carta de visado (normativa viva) | Una **comprobación determinista de consistencia entre los campos que ella ya ha tecleado a mano** —expediente ↔ carta ↔ factura ↔ certificado—, que ataca el mismo mecanismo de error **sin que el documento de identidad entre en ningún sitio** |
| **P26** responder una queja formal | **Clasificarla, extraer los hechos comprobables y preparar el expediente** para la persona que sí decide |
| **P22** decidir la asignación de camas | El **aviso** cuando dos reservas se solapan: es un filtro, es veredicto 1, y no necesita ningún modelo |

**4 · Las zonas prohibidas, con el motivo y no solo la prohibición**, porque una prohibición sin motivo no
se transfiere a un caso nuevo. **Y se escriben en M0, día 3, por ella**, contrastando después contra la
lista del curso:

| Proceso | Por qué no, dicho de forma transferible |
|---|---|
| **P08** carta de aceptación para visado | Riesgo crítico y **normativa viva**. Congelar conocimiento que caduca dentro de un artefacto es fabricar un error futuro |
| **P26** quejas formales | Una respuesta que **admite responsabilidad por escrito compromete a la empresa**. Y los modelos son complacientes: la complacencia por escrito, en una queja, es exposición legal |
| **P29** emergencias 24 h | Personas, menores, responsabilidad civil, y un alumno en estado de shock con nivel A1 |
| **P25** reembolsos | Datos bancarios y riesgo de fraude por suplantación en el cambio de cuenta |
| **P17** matching con familia de acogida | Concentra **salud, religión y potencialmente orientación sexual** en una casilla de texto libre. Es el proceso que **más parece** el caso ideal de IA, y por eso es la trampa |
| **P22** calendario de camas | Riesgo crítico por overbooking, y además es un calendario de recursos: escalón −1 |
| **P05 / P16** nivelación y exámenes | **Anexo III del Reglamento de IA**: *evaluar el nivel educativo* es alto riesgo. Aplazado al 02.12.2027, **no cancelado**. Lo suyo no es decidirlo **[!]**: es reconocerlo y avisar |

Y la regla de oro que hace todo esto memorable, y que se recuerda cuando una lista de artículos no:

> **De todo su trabajo, el único trocito que está en la lista de alto riesgo es el que decide el nivel de
> un alumno. Todo lo demás —redactar, traducir, resumir, clasificar, preparar borradores— no lo está.**
> Esa asimetría se recuerda.

**5 · El caso donde las reglas son de otro, que ninguna arquitectura salvo arq-1 trabaja.** **P16**,
exámenes oficiales: la inscripción, las tasas y los plazos viven en la plataforma del Instituto Cervantes,
los plazos son rígidos y no se recuperan. **El motivo transferible no es de riesgo ni de datos: es que el
proceso es ajeno.** Automatizar la parte que uno controla de un proceso cuyas reglas pone otro produce un
sistema que se rompe el día que el otro cambia algo, sin avisar. Es una categoría de «no» que va a
encontrarse en cualquier empresa, y por eso está escrita.

**6 · El coste completo como criterio de descarte, no como cálculo de justificación** (M5). *Un sistema
que ahorra ocho minutos y cuesta diez de revisión es una pérdida disfrazada de modernidad.* Y la métrica
de vanidad tiene nombre: **que se ejecute cada lunes no es que funcione.**

**7 · La opción segura suele ser también la más eficiente, y eso se demuestra, no se predica.** El mejor
ejemplo, y va en M2: **no transcribas la llamada.** Escribe tú un resumen de cuatro líneas al colgar, ya
seudonimizado, y trabaja con ese resumen. Es más rápido que subir un audio de doce minutos, no genera un
tratamiento nuevo ni un destinatario nuevo, y de paso piensas el caso. Enseñado así, «no usar IA» deja de
ser una renuncia y pasa a ser **una decisión de eficiencia**.

---

# 10. PROTECCIÓN DE DATOS, INTEGRADA

## 10.1 El principio de diseño

Un módulo de protección de datos se lee una vez, se aprueba y se olvida. Y además **produce parálisis**,
cuando el objetivo es que **use más la IA, no menos: que la use en el sitio correcto.** Un bloque de
protección de datos que produce parálisis ha fallado.

Pero «transversal» tampoco basta, porque suele significar «repartido y por tanto de nadie». Aquí la
protección de datos tiene **tres formas concretas y ninguna es un anexo**:

1. **Está dentro del clasificador.** Las preguntas **4 y 5** de las cinco preguntas —*¿qué puede tocar?
   ¿quién firma la salida?*— **son, literalmente, protección de datos y salvaguardas**. No se puede
   clasificar una herramienta sin contestarlas. Por eso el régimen de datos se **deriva** de la
   clasificación en vez de pegarse al final.
2. **Está dentro del criterio de elección.** El color de los datos es una de las cinco columnas del embudo
   de M0, con un −3 que descalifica. Es decir: **la protección de datos no llega a frenar el proyecto:
   decide cuál es el proyecto.**
3. **Es una capa del proceso, con artefacto propio**: el mapa de datos (§10.2).

## 10.2 Las tres capas, cada una pegada a la acción que desbloquea

| Capa | Dónde | Qué contiene | **Por qué exactamente ahí** |
|---|---|---|---|
| **1 · Antes de tocar nada** | **M0**, días 1 y 3 | Cuenta de empresa frente a personal · **las cuatro preguntas que definen cualquier plan** + la quinta, de su empresa · qué edición, qué licencia, qué retención, qué política escrita · **el semáforo impreso** · **la columna de datos en el criterio de elección** | **Es la semana en la que va a empezar a pegar cosas.** Todo lo demás se construiría sobre un suelo que no ha mirado |
| **2 · Cuando le mete datos** | **M2**, antes de cargar fuentes | **El mapa de datos del proceso** · por qué quitar el nombre no basta · cuasi-identificadores · **la prueba de la compañera** · la regla de los adjuntos | **Es el momento exacto en que pasa de pegar texto a subir ficheros.** Al pegar ves lo que envías; al adjuntar, no. Un Excel va **completo** —todas las filas, las columnas ocultas, la hoja que se llama «datos antiguos»—, un PDF de pasaporte va entero, una foto lleva coordenadas |
| **3 · Cuando algo actúa sin que ella mire** | **M4**, con los frenos | Temas prohibidos · condiciones de parada · *nada sale al cliente sin que un humano le dé a enviar* · **el aviso de IA**, en vigor desde el 02.08.2026 · registro de qué se generó y quién lo aprobó · plan para el día que falle, **incluido valorar si hay brecha [!]** · el **Anexo III** aplicado a su academia | **Es cuando algo empieza a actuar sin que ella revise cada paso.** Antes de M4 no hacía falta; después de M4 sería tarde |

**Capa permanente:** la **tarjeta del lunes** impresa al lado de la pantalla desde la semana 1, con seis
preguntas que caben en una nota adhesiva. *Si una regla necesita que te pares a pensar, no sobrevive a un
martes de julio con trescientos correos sin abrir.*

## 10.3 El artefacto: el mapa de datos del proceso

Un semáforo genérico se lee y se olvida. **Un semáforo aplicado al único proceso que está construyendo se
usa**, porque contesta una pregunta que tiene delante. Una cara, cuatro columnas:

| Dato que atraviesa el proceso | Color | **En qué paso entra** | **Dónde hay que quitarlo, y quién lo quita** |
|---|---|---|---|
| Nombre y apellidos del alumno | Ámbar | En el correo entrante | Antes de pegar nada: lo quito yo, a mano |
| Nacionalidad + edad + fecha de llegada + barrio | **Ámbar peligroso** | En el cuerpo del correo | Se **generalizan**, no se borran: «alumno», «esta semana», «familia de acogida». Combinados identifican a una persona entre 1.400 |
| Nº de pasaporte o NIE | **Rojo** | Adjunto en la reserva | **No entra nunca.** Si necesito un dato de ahí, lo escribo yo a mano, y solo ese |
| IBAN, tarjeta, justificante de pago | **Rojo** | Adjunto o cuerpo | **No entra nunca**, en ninguna herramienta |
| Alergia, dieta médica, medicación | **Rojo** | Formulario de preferencias | **No entra nunca**, ni seudonimizado. Se degrada al mínimo funcional si el texto lo exige: «una intolerancia alimentaria» |
| Cualquier dato de un **menor** | **Rojo absoluto** | Grupos escolares, estancias de 16–17 | **Nunca, en ninguna herramienta, ni seudonimizado. Sin excepciones** |
| Dirección del alojamiento junto al nombre | **Rojo** | Confirmación de alojamiento | No entra. Localiza físicamente a una persona |
| Tarifario, calendario, condiciones, plantillas | **Verde** | Documentos de la academia | **No son datos personales.** Entran sin pensar, y por eso el proceso puede empezar aquí |

**Cuatro cosas que este artefacto hace y un semáforo genérico no:**

1. **Sitúa el punto de corte en el flujo, que es lo que convierte una regla en un gesto.** Saber que un
   pasaporte es rojo no cambia nada un martes; saber que **el pasaporte entra como adjunto en el paso dos
   y por eso el paso dos nunca sube el adjunto original**, sí.
2. **Nombra quién lo quita.** Si la respuesta no es una persona o un paso concreto, no hay corte: hay una
   intención.
3. **Es reutilizable como hábito portátil.** Un mapa de datos por proceso vale en cualquier empresa y en
   cualquier año, y no menciona ninguna herramienta.
4. **Muestra que la mayoría de su proceso empezó en verde**, que es el mensaje que evita la parálisis: la
   protección de datos no le prohíbe trabajar, **le dice por dónde empezar**.

**El ejemplo de reidentificación es de su casa, y es el que se memoriza:** *«La alumna coreana de 19 años
que llegó el 3 de julio y está alojada con la familia de Chamberí dice que la comida no le sienta bien y
que es celíaca.»* Ni un solo nombre — y cualquiera de sus tres compañeras sabe de quién se habla en dos
segundos. Con 1.400 alumnos al año, nacionalidad + edad + fecha + barrio deja **una sola persona**. Y
encima hay un dato de salud. **La prueba que hay que memorizar es una sola:** *¿podría una compañera mía
saber de quién hablo leyendo esto?*

## 10.4 Las cinco decisiones que hacen que esto funcione y no asuste

1. **La regla de los menores es tajante y sin excepciones**, más restrictiva de lo que la norma exige en
   todos los supuestos, **a propósito**: una regla con excepciones no sobrevive a julio.
2. **Cada decisión que no es suya va marcada [!] y con el nombre de a quién se escala.** El riesgo
   específico de este perfil es que, por ser la que más se preocupa, acabe siendo de facto la responsable
   de cumplimiento de la academia. El material lo prohíbe explícitamente: *tu papel no es ser la
   responsable de cumplimiento; tu papel es no ser tú el agujero, y saber cuándo hay que levantar la
   mano.* No decide la base jurídica, no decide si hace falta una evaluación de impacto, no decide si hay
   brecha notificable.
3. **Nada normativo se congela dentro de un artefacto.** Las fechas del Reglamento de IA, el estado del
   marco de transferencias a Estados Unidos y la ley española viven en `datos-volatiles.md`, **con fecha
   visible**, y se revisan. Y eso es, además, **el mejor ejemplo pedagógico del curso** de la diferencia
   entre conocimiento estable y conocimiento volátil, que es exactamente la distinción que hay que
   dominar para construir fuentes que no envejezcan mal.
4. **El encuadre no es de permiso, es de aportación.** No está pidiendo autorización para nada: ya usa la
   herramienta, se la ha dado su empresa, y usarla está bien visto. Está entendiendo la configuración
   antes de apoyarse en ella. Si la academia nunca se lo ha planteado, **acaba siendo ella quien propone
   la política**, que es el mejor resultado posible — y no es venta interna: es su propio trabajo.
5. **La transición con su cuenta personal se resuelve sin moralina**, porque la moralina no cambia hábitos
   y además sería injusta: lo que hace es lo que hace casi todo el mundo. Se traza una línea limpia
   —cosas suyas y prácticas con casos inventados, en la personal; **cualquier cosa que venga de un correo,
   una llamada o un expediente de un cliente**, en la de empresa— y se da el argumento que de verdad
   convence, que no es «es ilegal»:

   > **Si mañana un alumno ejerce su derecho de supresión y la academia tiene que certificar que ha
   > borrado sus datos de todos los sitios, tu cuenta personal es un sitio que la academia no puede tocar
   > y del que ni siquiera sabe que existe.** No es que hayas hecho nada malo: es que has creado, sin
   > querer, un almacén de datos de clientes fuera del alcance de la empresa. Y eso, cuando aparece, no
   > tiene arreglo posible: no se puede desandar.

**Y los dos principios que ordenan las respuestas y no dependen de ningún producto:** *pagar resuelve
quién es el proveedor, no qué tratamientos están amparados* — que su empresa tenga contrato con alguien no
legitima que ella meta ahí un pasaporte. Y *sin indicador, trátalo como cuenta personal* — la única regla
que no falla cuando no sabes.

## 10.5 El dato que cambia la posición mental con la que se estudia esto

Merece salir en la primera página del curso: **el artículo 4 del Reglamento de IA, en vigor desde febrero
de 2025, obliga a las empresas que usan IA a garantizar un nivel suficiente de alfabetización en IA de su
personal.** Dicho de otro modo: **el curso que está haciendo es, técnicamente, cumplimiento normativo de
su empresa.** No es un extra que se paga a sí misma en su tiempo libre por pura iniciativa: es una
obligación de la academia que ella está cubriendo.

---

# 11. EL MÓDULO DE EVANGELIZACIÓN INTERNA — M7 · «Que lo adopten»

## 11.1 Qué NO es, dicho primero porque es donde se estropea

- **No es conseguir el sí.** No hay autorización que pedir. En su empresa usar IA ya está bien visto y **lo
  mal visto es no automatizar**. Un módulo de venta interna resolvería un problema que ella no tiene y le
  robaría tres semanas a los que sí tiene.
- **No es marketing personal.** Nada de portfolio, nada de landing, nada de «mira lo que tengo ahora en mi
  CV». Ese es el destino del itinerario no técnico de la referencia porque **su alumno tipo quiere cambiar
  de sector**. La nuestra no — aunque sí quiere que lo aprendido le sirva si algún día cambia de empresa,
  y de eso se encargan la portabilidad del criterio y los seis instrumentos, no una web.
- **No es pedir presupuesto.** Todo lo que ha montado cuesta cero. Pedir dinero cambia la conversación
  entera y no hace falta.
- **No es una presentación a dirección.** Una presentación es un evento; la adopción es un hábito. Y una
  presentación sin usuario real es una demo.
- **No es la columna vertebral.** Son tres semanas al final, alimentadas por tres líneas por capa. Si
  fuera la lente del curso entero, el curso dejaría de ser sobre su trabajo y pasaría a ser sobre su
  reputación, **y el criterio se contaminaría**: elegiría lo vistoso sobre lo útil, que es exactamente el
  error del grafo de la referencia.
- **No es convencer a nadie de que la IA es buena.** Ya están convencidos. El problema del brief es el
  contrario: **empujan con desconocimiento de lo que se puede hacer.** Lo que falta no es entusiasmo, es
  información realista.

## 11.2 Qué es: el enunciado del módulo

> **Demostrar y arrastrar.** Su empresa empuja la IA sin saber bien qué se puede hacer. Lo que cambia esa
> situación no es un argumento: es **una cosa que funciona, un número que se puede reproducir, y una
> segunda persona que la usa sin ella delante.** Este módulo produce esas tres cosas.

Y el principio que lo ordena entero, que es el mismo que atraviesa el curso:

> **La credibilidad se compra con los noes.** Quien llega diciendo *«estas cuatro cosas NO deberían
> automatizarse, y aquí está por qué»* consigue que le crean sobre la quinta. Quien llega diciendo que
> todo se puede automatizar consigue que no le crean sobre nada — y esa es, exactamente, la posición en la
> que su empresa está hoy respecto a la IA.

**Y la ventaja específica de esta columna vertebral, que es su mejor argumento:** el módulo **no tiene que
fabricar su materia prima**. Llega con un sistema que lleva tres meses en producción sobre su mesa, con
una Tira de cinco columnas fechadas, con un número medido contra una línea base tomada **antes** de
construir nada, con una rejilla de doce veredictos y con una lista de noes razonados. Eso no es una demo:
es un historial.

## 11.3 Qué enseña — siete piezas, todas con artefacto

**(1) El número y su método, que van juntos o no va ninguno.** De M5 sale un ahorro en minutos por unidad,
con el coste de revisión restado y con una amenaza a la validez que no se puede descartar. **Las tres
cosas se presentan juntas.** Un número sin método es una promesa, y una promesa que no se cumple quema los
tres proyectos siguientes. Aquí su formación es una ventaja competitiva directa y hay que decírselo así:
casi nadie que presenta resultados de IA en una empresa sabe decir *«esto podría explicarse también porque
septiembre no es julio»*, y decirlo es precisamente lo que hace que se crean el resto.

**La jerarquía de la evidencia**, que es contenido de primera y se enseña como tal *(de arq-1 §6.3)*:

| Nivel | Evidencia | Por qué pesa lo que pesa |
|---|---|---|
| **1** | **Otra persona usa el artefacto sin ti** | Es un hecho observable, no una afirmación tuya. No admite réplica |
| **2** | **Un hallazgo que nadie sabía** — *«la plantilla alemana lleva meses mandando el precio del año pasado»* | Cambia el marco: no vienes a contar lo que ahorras, vienes con un problema real que has encontrado |
| **3** | **Minutos por unidad, con línea base y coste completo restado** | Es un número honesto y con su amenaza declarada. Sobrevive a que lo repregunten |
| **4** | Una demo | Impresiona y se olvida. Vale solo si termina en el nivel 1 |
| **5** | *«Me ahorra muchísimo tiempo»* | **Vale cero.** Es exactamente lo que dice todo el mundo y por eso ya no significa nada |

Y la regla que ordena la redacción de todo lo que escriba: **una afirmación interna tiene que sobrevivir a
tres preguntas escépticas seguidas.** Se enseña haciendo: coge tu frase, escríbete las tres preguntas más
incómodas que te haría alguien que no te cree, y contéstalas **dentro** de la media página. Aquí su
formación es ventaja directa: las tres preguntas incómodas son, casi siempre, las amenazas a la validez
interna que ya nombró en M5 (*«¿no será que en noviembre hay menos volumen?»* = historia; *«¿no será que
has mejorado tú?»* = maduración).

**(2) Lo que el artefacto NO hace.** Es la tercera línea del Cuaderno de evidencias, y en el dossier va en
su propio apartado, no en letra pequeña. Doble función: es honestidad, y es **gestión de expectativas
operativa** — si el dossier dice «no responde nada sobre visados y para en cuanto aparece el tema», la
primera pregunta incómoda ya está contestada antes de que la hagan.

**(3) La demo de tres minutos, con la regla del caso real.** No una presentación: **un antes y un después
con un caso real, elegido delante, y un número.** Un caso preparado no convence a nadie que haya visto
alguna demo antes, y en 2026 todo el mundo las ha visto. **Se enseña también dónde falla**, y qué
salvaguarda lo cubre: es contraintuitivo y es lo que convierte una demo en algo creíble, y además es la
única forma de que quien la adopte sepa dónde mirar. **Y se termina siempre igual:** *«si quieres, te lo
dejo montado para lo tuyo y te paso la hoja de cómo se usa»*. Sin esa frase, la demo es entretenimiento.
Guion escrito y cronometrado.

**(4) La prueba del pasillo.** Explicar qué hace, qué ahorra y **qué no hace**, en treinta segundos y **sin
nombrar ninguna herramienta**. Regla de vocabulario dura: se nombra el resultado, no la tecnología. No
*«monté un flujo con un paso de extracción que llama a mi cuaderno de fuentes»*, sino *«los correos de
admisiones llegan ya clasificados y con un borrador hecho, y me ahorra unos ocho minutos por correo; los de
visado no los toca, los deja para mí»*. Esta regla es además la vacuna contra el efecto que más daño hace
a un evangelizador interno: **sonar a que ha descubierto una religión**.

**(5) LA SEMANA SIN ELLA — el corazón del módulo.** Una compañera usa el artefacto **cinco días
laborables, sin ella delante**. No una demostración acompañada: uso real, sola.

Es el único test verdadero de adopción y produce siempre el mismo hallazgo, que es lo que lo hace valioso:
**una parte del artefacto era ella.** Instrucciones implícitas, decisiones que tomaba sin darse cuenta, un
fichero que solo ella sabe dónde está, un criterio que nunca escribió porque le parecía obvio. Lo que el
piloto revela es exactamente lo que hay que arreglar para que la cosa sobreviva a sus vacaciones — **y
sobrevivir a sus vacaciones es literalmente la definición operativa de que la organización lo ha
adoptado**, en un negocio donde agosto vacía la oficina y julio la desborda.

**El entregable del piloto no es «salió bien»: es la lista de lo que hubo que arreglar, y tiene que tener
al menos dos entradas.** *Si el piloto no reveló nada, no fue un piloto: estuviste mirando por encima del
hombro.*

**(6) La ficha de traspaso**, que viene hecha de M6 y aquí se entrega de verdad: qué fuente caduca y cada
cuánto · quién la revisa, **con nombre** · qué batería se vuelve a pasar cuando se toque algo · cómo se
apaga, probado. Es lo que convierte «una cosa que hizo ella» en «una cosa que tiene la academia». Y es
también protección propia: un artefacto sin dueño y sin fecha se degrada, y **cuando se degrada el
recuerdo que queda no es «faltaba mantenimiento», es «aquello de la IA no funcionaba»**.

**(7) La conversación del proceso de otra persona** — la semilla de contagio, y a la vez el octavo doblete.
Veinte minutos con una compañera, aplicando **solo la capa 0** a un proceso de ella: qué lo dispara, qué
documentos abre, qué decisiones toma que no están escritas, qué sale y a dónde va. **No se construye nada
y no se promete nada.** Se escribe la descripción en una página y se le devuelve para que la corrija.

Por qué esto contagia y una presentación no:
- **Es la técnica que ella ya sabe hacer y que un perfil técnico no puede aportar** (C9): entrevista
  semiestructurada, estructura de embudo, **preguntar por el último caso concreto y no por la norma**,
  preguntar por la excepción, y **devolver el procedimiento escrito para que lo corrijan — porque
  corrigiendo se saca más que preguntando**.
- **El encuadre que funciona no es «quiero automatizar tu tarea»** —eso pone a cualquiera a la defensiva—
  **sino «quiero aprender a hacerlo yo bien para no molestarte cada vez»**. Y es verdad, además.
- Y produce el efecto que ningún dossier produce: **la otra persona ve su propio proceso escrito por
  primera vez. Ahí es donde alguien pide algo.**

**Su clave sellada es de ejecución, no de veredicto**, y es una lista binaria: *¿preguntaste por el último
caso concreto en vez de por «cómo lo hacéis normalmente»? ¿preguntaste por la excepción? ¿le devolviste la
descripción escrita? ¿aparece en tu descripción al menos una decisión que ella toma y no está escrita en
ningún sitio? ¿prometiste algo?* (esta última tiene que ser NO).

**Y las cuatro reglas de arranque, todas derivadas de lo que el curso ya ha hecho:**

| Regla | Por qué |
|---|---|
| **Empieza por un proceso que no sea de nadie** | Un proyecto que mejora la tarea de una compañera empieza con una persona a la defensiva; uno que hace lo que nadie hacía empieza con cero resistencia. **La elección del primer proceso es el 80 % de su adopción**, y por eso el embudo de M0 no era solo una cuestión de riesgo |
| **Coste de adopción cero** | El resultado se entrega **en el sitio donde esa persona ya mira** —su buzón, la reunión del lunes, el documento que ya abre— y **no** en una herramienta nueva a la que tenga que entrar. **Si adoptar exige que alguien aprenda algo, no se adopta.** Esta regla sola explica la mayor parte de los proyectos internos que mueren funcionando perfectamente |
| **Enseña el resultado, no el proceso** | La primera vez se enseña lo que sale, no cómo se hizo. El «cómo» se cuenta cuando alguien lo pide, que es la señal de que ya hay adopción |
| **Deja que lo pidan** | La segunda persona no se recluta: aparece cuando ve el primer resultado. **Si a las tres semanas nadie ha pedido nada, el artefacto no era tan útil como parecía — y eso también es un resultado del curso**, no un fracaso personal |

**Y la pieza que ningún material de este tipo incluye: la deuda de adopción.** En una empresa de treinta
personas donde lo mal visto es no automatizar, hacerse visible como «la que sabe de IA» tiene un desenlace
muy previsible: que le caiga trabajo ajeno. Cuatro reglas:
- **No entregues lo que no puedas mantener.** Un flujo que se rompe en julio, cuando entran 400 correos al
  día, no es valor: es un problema que ella misma se ha creado, y encima con público.
- **Entrega el artefacto y el manual, no el servicio.** La frase que marca el límite, y conviene tenerla
  escrita: *«esto lo monté yo y así se mantiene; si quieres uno para lo tuyo, aquí está cómo se hace»*.
- **El bus factor invertido:** si es la única que sabe cómo funciona, la organización no adopta el
  artefacto: **la adopta a ella**. La ficha de traspaso es la contramedida, y por eso es entregable.
- **Es la versión gemela del límite de rol de protección de datos [!]**, y se nombra con la misma regla:
  *tu papel no es hacerte cargo de todo; es no ser tú el agujero y saber cuándo levantar la mano.*

## 11.4 Cómo se autocorrige sin mentor — el punto donde este módulo se juega su credibilidad

Es el módulo más difícil de autocorregir de los ocho, porque **su criterio de éxito es la conducta de
otras personas**, que ella no controla. Decirlo es obligatorio. Y aun así hay **cinco mecanismos, cuatro
de ellos comprobaciones y no juicios**:

1. **El piloto es el corrector, y es binario, y se provoca en vez de esperarse.** Otra persona lo usó cinco
   días laborables sin ella, o no lo usó. Se cuenta. Y el entregable es **la lista de arreglos, con al
   menos dos entradas**: ese es el criterio negativo del módulo, y es lo que lo hace infalsificable.
   *(Este mecanismo sustituye a la comprobación de adopción de arq-1 —«¿alguien lo ha usado sin que se lo
   pidieras? SÍ/NO»—, que su propio autor reconoce que admite un SÍ falso por cortesía.)*
2. **La reproducción del número, ±10 %** *(injerto de arq-2, M8)*. Dos semanas después, con la ficha de
   método delante, vuelve a calcular el ahorro. **Si no sale el mismo número dentro del ±10 %, el número
   no era reproducible y el dossier se reescribe.** Es un test-retest de su propio instrumento y no
   necesita a nadie.
3. **La prueba del pasillo, cronometrada, con cuatro comprobaciones binarias** *(injerto de arq-2)*.
   Treinta segundos, a alguien que no ha visto el artefacto, y después: *¿nombré alguna herramienta?
   ¿la otra persona pudo repetirme qué hace? ¿dije un número? ¿dije qué NO hace?* Es corrección de coste
   cero para lo que antes dependía de un punto de consulta.
4. **Rúbrica del dossier, con criterios negativos y salida escrita obligatoria** (sin «no aplica»):
   - *Hay en el dossier un número cuyo método no puedo reproducir delante de alguien.* ☐
   - *Hay una afirmación que no podría defender si alguien la comprobara la semana que viene.* ☐
   - *El apartado «qué NO hace» está vacío o dice generalidades.* ☐
   - *La respuesta a «quién lo mantiene» no es una persona con nombre.* ☐
   - *No hay ninguna forma de apagarlo, o la hay pero no la he probado.* ☐
   - *Presento como resultado del sistema algo que en realidad hago yo a mano después.* ☐
5. **PC-6**: la prueba del pasillo con alguien que **sabe de IA y no conoce la academia** es el evaluador
   ideal para las dos cosas que ella no puede ver desde dentro: **jerga** y **sobreafirmación**.

**Y lo que este módulo NO puede corregir, escrito para que no se disimule:** si su compañera no usa el
artefacto, hay al menos cinco explicaciones —el artefacto es malo · la compañera está desbordada · la
tarea no era suya · el coste de adopción no era cero · no hubo tiempo— y el material no le da forma
infalible de distinguirlas. Lo que sí hace es **preinterpretar el silencio** con una rúbrica de cinco
causas, cada una con su seña y su arreglo mínimo, más **una sexta lectura legítima, escrita antes de que
ocurra: que el artefacto no debía adoptarse.** Un sistema que solo tiene sentido con ella delante puede ser
perfectamente correcto como herramienta personal, y reconocerlo es un resultado, no una derrota.

**Es el único punto del curso donde una alumna diligente puede hacerlo todo bien y salir sin saber si lo
hizo bien.** Está dicho en el material, y está dicho en §17.4.

## 11.5 Dónde va y por qué exactamente ahí

| Alternativa | Por qué no |
|---|---|
| Al principio, como encuadre motivador | No hay nada que enseñar todavía. Y arranca el curso con la mirada puesta en lo que piensen los demás, que es el desvío que el brief prohíbe |
| Repartido por todos los módulos | Convertiría cada capa en una pieza de comunicación y contaminaría el criterio: se elegiría lo vistoso sobre lo útil |
| Después de M4, cuando el sistema ya funciona | Tentador, porque ahí ya hay algo que enseñar. Pero **no hay número**, y un dossier sin número medido es una opinión con formato de informe |
| **Al final, después de medir y después de dejarlo mantenible** ← **la elegida** | Consume la salida de M5 **y** la de M6 **y** la rejilla de los doce. No se evangeliza lo que no está medido, y no se traspasa lo que no tiene dueño ni fecha. Además llega en el momento en que el material solo ya no tira: **el único incentivo disponible en la semana 16 es que alguien de fuera use lo que has hecho**, y ese es precisamente el contenido del módulo |
| Al final, pero sin hilo previo | El Cuaderno de evidencias existe desde la semana 3 justamente porque, sin él, M7 tendría que reconstruir números de memoria — es decir, inventarlos |

**Y una propiedad estructural que se declara por escrito en la semana 1** *(injerto de arq-1 §3.1, la
movilidad de M7, adaptada)*: **M7 no abre ninguna puerta y nada depende de él.** Contiene además una espera
de una semana natural que no depende de ella. Por eso, **si el calendario se rompe —una baja, un pico
adelantado, un piloto que no encuentra compañera disponible— M7 se puede mover, retrasar o partir sin que
eso rompa nada, y sin que el calendario roto se lea como curso abandonado.** Un módulo cuyo final depende
de la agenda de otra persona tiene que llevar escrito, desde el principio, que puede ocurrir en marzo.

## 11.6 Qué produce, en una lista

1. **Un dossier de una cara**: qué hace · qué ahorra y con qué método se midió · **qué no hace** · quién lo
   mantiene · cómo se apaga.
2. **Un guion de demo de tres minutos**, cronometrado, con un antes y un después reales.
3. **La semana sin ella, ejecutada**, y su lista de arreglos con al menos dos entradas.
4. **Una descripción del proceso de otra persona**, escrita por ella y corregida por su dueña.
5. **La lista de lo que decidió no automatizar**, con el motivo — heredada de la línea de corte de M1, de
   los ocho dobletes y de la rejilla de los doce, y actualizada.
6. **La segunda vuelta**: qué veredictos de la rejilla han cambiado en cuatro meses y por qué.
7. **Una nota de media página** para quien lleve la política de uso de IA, si en M0 resultó que no existe
   ninguna. No es venta: es cerrar el hueco que ella misma detectó en la semana 1, y es el hallazgo con
   mejor relación valor/esfuerzo de todo el curso.

---

# 12. SISTEMA COMPLETO DE AUTOCORRECCIÓN SIN MENTOR

## 12.1 El principio que ordena todo el aparato

> **La primera decisión de diseño de cada entregable no es «qué rúbrica pongo». Es: ¿puedo convertir esta
> evaluación en una comprobación?** Muchísimas veces se puede, y casi nunca se intenta.

Y su corolario, que es el que gobierna dónde entra la IA correctora: **la IA está en el puesto 6 de 9 en
fiabilidad, no en el 1.** Es la tentación obvia de un curso de IA sin profesor y es la que hay que domar.
Es valiosa por cobertura e inmediatez, no por fiabilidad.

**Y una advertencia sobre la afirmación central de esta columna vertebral, que hay que hacer en la misma
frase en que se hace la afirmación, porque si no es trampa:** el mejor corrector de este diseño es que el
artefacto está en producción sobre su mesa. Pero **funcionar no es estar bien**. El uso diario detecta que
algo molesta; no detecta que el criterio estaba mal escrito ni que la batería era fácil. **El mundo corrige
la utilidad; los instrumentos corrigen el criterio.** Por eso todo lo que sigue está entero.

## 12.2 Los nueve mecanismos, ordenados por fiabilidad real, y dónde vive cada uno

| # | Mecanismo | Fiabilidad | Dónde vive en este curso |
|---|---|---|---|
| **1** | **Ejecución real: funciona o no funciona** | Máxima, cobertura estrecha | El correo del día 1 · el asistente responde o alucina · el disparador se dispara o no · los cinco casos paran o no · el apagado funciona o no |
| **2** | **Batería con clave sellada** | Muy alta | **La Tira**, cinco pasadas fechadas · las diez preguntas del asistente del día 3 · **las claves de los ocho dobletes** · las claves del expediente modelo |
| **3** | **Lista de comprobación binaria observable** | Alta, y lo único que caza **omisiones** | Una por módulo: fuentes (M2, 10 ítems) · plataforma (M3, 6 ítems) · frenos (M4, 11 ítems) · traspaso (M6, 5 ítems) · rejilla (M6, 12 ítems) · dossier (M7, 6 ítems) |
| **4** | **Solución comentada con anatomía del error** | Alta | Cinco o seis fallos típicos por módulo, cada uno con `cómo se reconoce en tu propio trabajo` · `por qué pasa` · `arreglo mínimo` |
| **5** | **Rúbrica con criterios negativos + autoevaluación diferida** | Media-alta | Se usa **al día siguiente**, nunca al terminar, y con encuadre en tercera persona: *«reviso el trabajo de alguien que hace mi puesto y tengo que decidir si se lo devuelvo»* |
| **6** | **IA correctora con rúbrica anclada y protocolo adversarial** | **Media, y variable de forma no aleatoria** | Con el protocolo de siete reglas, **y graduada por entregable** (§12.4) |
| **7** | **Contraste de dos modelos** | Media | Solo para **detectar** desacuerdo, nunca para dirimirlo. El desacuerdo es materia prima de un punto de consulta |
| **8** | **Punto de consulta con su pareja** | La más alta, estrechísima por escasez | **Seis en todo el curso** (§12.5) |
| **9** | **Autoevaluación libre** («¿me ha quedado bien?») | ≈ nula | **Prohibida como mecanismo**, y se dice por qué |

## 12.3 Las tres piezas que hacen que el sistema no se autoengañe

**(a) LAS PUERTAS.** Seis condiciones de paso observables (§6), y **la única figura de este curso que
bloquea en vez de avisar**. Sin profesor, la diferencia entre un mecanismo que te avisa y uno que te para
es la diferencia entre una rúbrica y un profesor. Las dos decisivas:

- **M2 → M3: «ha usado el asistente al menos cinco veces en una semana sin que el curso se lo pidiera».**
  No mide si aprendió la lección: **mide si el artefacto le sirve**, y es una medida conductual externa a
  su juicio sobre su propio trabajo, que es justo el punto ciego que la literatura sobre autoevaluación
  describe.
- **M3 → M4: «ha visto fallar algo y sabe por qué».** Sin haber visto un fallo no hay criterio para dar
  autonomía a nada. **Si no ha fallado nada, el material trae un fallo provocado.** Es un control positivo
  aplicado al sistema, igual que el cebo lo es a la correctora.

**(b) LOS TRES CEBOS — control positivo sobre la correctora.** Todo el aparato asume que el corrector,
bien encauzado, detecta algo. **Eso hay que comprobarlo, no suponerlo.** Ella lo reconocerá al instante con
su nombre: si el instrumento no detecta un caso que sabemos positivo, sus negativos no valen nada.

| Cebo | Dónde | Sobre qué | Función añadida |
|---|---|---|---|
| **1** | M1 | Una **línea de corte de mentira** con tres defectos plantados: uno visible (trozo con datos rojos marcado «lo entrego»), uno de omisión (falta la revisión humana antes de que algo salga), uno de criterio (trozo determinista clasificado como veredicto 5) | **Calibra el instrumento antes de usarlo cincuenta veces** |
| **2** | M4 | Una **lista de frenos** con tres defectos plantados | Comprueba que el instrumento sigue sirviendo en el entregable más difícil |
| **3** | M6 | Un artefacto pasado por **la rúbrica que ella misma ha escrito** | Doble: valida su rúbrica (*si el cebo la pasa, la rúbrica es blanda y se rehace*) **y detecta la degradación de su propia lectura como correctora a los cuatro meses** |

| Resultado del cebo | Lectura | Qué hace |
|---|---|---|
| Encuentra los 3 | El instrumento sirve para este tipo de trabajo | Sigue |
| Encuentra 2 | Normal: detecta lo visible, se le escapa lo de criterio | Sigue, **sabiendo que la omisión y el criterio los tiene que cazar la lista de comprobación**, no la IA |
| Encuentra 1 o 0 | **El instrumento está roto para esta tarea** | Revisa la rúbrica (probablemente sea vaga). Si sigue igual: **esta tarea no se corrige con IA**, y pasa a los mecanismos 2–4 |
| Aprueba el cebo entero | Descalificatorio | **Ese tipo de trabajo nunca se corrige con IA en el resto del curso** |

**(c) EL PROTOCOLO DE SIETE REGLAS**, página única, citada desde cada rúbrica: hilo nuevo, siempre · no es
tuyo (*«reviso el trabajo de una compañera»*: 13,6 puntos de diferencia medidos entre primera y tercera
persona [E]) · nunca preguntes si está bien, sino *«enumera los incumplimientos de esta rúbrica y cita
textualmente el fragmento que los incumple; si no puedes citar un fragmento, no lo afirmes»* · pega la
rúbrica entera · **prohibido discutir en el mismo hilo** (anota el desacuerdo, corrige o no, y abre un
hilo nuevo con la versión modificada y la misma rúbrica) · dos modelos, y **el desacuerdo es la señal, no
el veredicto** · **su veredicto no cierra nada**: devuelve una lista de fallos candidatos, y quien decide
es ella.

**Y el resultado de aprendizaje que instrumenta la resistencia a la adulación en vez de predicarla
(RA16):** al terminar el curso tiene que haber **al menos un caso registrado en que decidió NO aceptar una
crítica de la IA, con el motivo escrito**.

## 12.4 La calibración de la correctora por entregable — la pieza más fina del sistema

Las tres arquitecturas aplican el mismo protocolo en todas partes. **Eso está mal**, y arq-3 lo detecta en
un solo sitio; aquí se generaliza y se hace regla de producción:

> **Cada rúbrica declara, en su bloque 3, hasta dónde llega la IA en ESE entregable.** Tres niveles:
>
> - **VERDE — la IA corrige con el protocolo completo.** Entregables de forma y de omisión: la ficha de
>   criterio, la lista de fuentes, el mapa de datos, el dossier.
> - **ÁMBAR — la IA solo para el bloque 1 (buscar señales de fallo); el bloque 2 se comprueba mirando.**
>   Entregables donde la respuesta correcta depende de hechos de su academia que el modelo no tiene: la
>   línea de corte, la rejilla de los doce.
> - **ROJO — la IA queda inhabilitada para este entregable, y se dice por qué.** Los dos casos:
>   **la lista de frenos de M4** —*«le estás pidiendo a un modelo complaciente que juzgue si otro modelo
>   es demasiado complaciente»*— y **la evaluación de M5** —pedirle a un modelo que juzgue lo que él mismo
>   produjo acumula preferencia por lo verboso y auto-preferencia, y las dos apuntan al mismo desastre:
>   aprobar por construcción—.

**Es la respuesta más fina que existe a «¿cómo se evita que la IA le dé la razón?»: reconociendo dónde no
puede evitarse.**

## 12.5 Los seis puntos de consulta, con alternativa degradada

**El principio.** El recurso es **escaso, no renovable y con coste relacional**. Un mentor pagado se gasta
sin culpa; una pareja, no. Y un curso que convierta a la pareja en su soporte técnico daña dos cosas a la
vez: la relación y la autonomía que el curso persigue.

**Presupuesto: seis consultas de diez minutos en todo el curso** — una hora repartida en cuatro meses. Un
curso que reserve «consultas ilimitadas» obtiene en la práctica **cero**, porque cada consulta compite con
la comodidad de no molestar y pierde. Uno que reserve exactamente seis, con nombre y momento, obtiene seis.

**Filtro de admisión, impreso en la portada del cuaderno.** Si falla cualquiera de las cuatro, no es punto
de consulta: (1) ¿lo resuelve el material? (2) ¿lo resuelve la IA con el protocolo? (3) ¿lo resuelve
**mirar** —su pantalla, su consola, preguntar a su administrador—? (4) ¿lo he intentado veinticinco
minutos y he anotado qué he probado?

**Ficha de cinco campos, escrita ANTES, máximo una cara:** la pregunta en una frase **cerrada** · mi
hipótesis y qué esperaría ver si tengo razón · qué he probado ya y qué pasó · **el dato concreto** (mensaje
de error literal, las dos respuestas que se contradicen) · qué haré con cada respuesta posible.

**Cuatro reglas de la conversación:** los cinco primeros minutos **sin pantalla** —muchas veces se resuelve
ahí, y eso es autoexplicación con oyente— · **él no toca el ratón** · sale con **una frase escrita en su
propio lenguaje** dentro de la hora siguiente · **a los diez minutos se para, esté como esté**; lo que no
cabe en diez minutos no es una consulta, es un problema de diseño del curso y se anota como tal.

**Y el principio de formulación, que es lo que hace que los diez minutos rindan** *(de arq-3 §7.2)*: **cada
pregunta se acota a lo que el consultor PUEDE auditar** — el razonamiento y los hechos de plataforma, **no
los hechos de la academia, que no conoce**. Gastar diez minutos irrecuperables en una pregunta que la otra
persona no está en posición de contestar es el peor uso posible del recurso.

| # | Momento | Qué lleva | Por qué ahí | **Alternativa degradada** |
|---|---|---|---|---|
| **PC-1** | Fin de **M0** (sem. 2) | *«He deducido que tenemos el plan X, que por eso no puedo hacer Y, y que por eso he descartado estos tres procesos y elegido este. ¿El razonamiento se sostiene?»* Con las comprobaciones empíricas hechas y la hoja de sombra delante | **Es el punto de mayor consecuencia del curso**, porque todo lo demás se construye encima. Y está formulado con precisión para lo que él sí puede auditar | Asumir el escenario **más restrictivo**, elegir el candidato con la puntuación más alta que no dependa de ninguna función dudosa, y anotar la suposición como pendiente de confirmar |
| **PC-2** | Inicio de **M2** (sem. 5), justo antes de cargar fuentes reales | Su clasificación de **ocho tipos de dato reales** en tres cajones —cuenta de empresa / nunca / depende— y tres casos ya seudonimizados: *«¿tú sabrías de quién hablo?»* | **Es la única decisión del curso con consecuencia externa irreversible**, y el momento es exacto: cuando pasa de pegar texto a subir ficheros | Regla de máxima cautela: **si dudas, no lo metes**, y lo anotas. Y la prueba de la compañera se hace con **cualquier compañera de la academia**, que además es la evaluadora literal del criterio |
| **PC-3** | Fin de **M1** (sem. 4), tras el cebo 1 | *«Esta es la corrección que me hizo la IA de un trabajo con tres fallos plantados. Encontró dos. ¿Estoy leyendo bien lo que se le escapa?»* | **El de mayor apalancamiento.** No se revisa su trabajo: se revisa **su instrumento de corrección**, que va a usar cincuenta veces más | Pasar el cebo por **dos modelos distintos** y comparar. El desacuerdo entre modelos es un sustituto pobre pero real del juicio externo |
| **PC-4** | **Comodín**, desde M3 | Un fallo de plataforma tras agotar la lista de seis comprobaciones y `cuando-no-coincide.md` | Caso canónico de «diez minutos ahorran una tarde». **No tiene fecha a propósito**: saber que existe un comodín reduce el miedo a atascarse, que es un factor de abandono por sí mismo, aunque no llegue a usarse | Documentar el fallo, **rodearlo** con una solución manual y seguir. Un curso no puede pararse por un botón que alguien movió |
| **PC-5** | Fin de **M4** (sem. 11) | *«Esta es la línea de corte con la que he terminado, estos son los tres sitios donde dudé, y estos son los dos dobletes donde no coincidí con la clave. ¿Dónde la moverías?»* | Juicio de escala y oportunidad: preguntarle a un modelo si algo debe automatizarse tiene un sesgo obvio hacia el sí, así que aquí el modelo no sirve. Y cae exactamente en la frontera de abandono | Los motivos tipificados de la línea de corte, los descalificadores por número de proceso, y **los desacuerdos con las claves de los dobletes**, que son la mejor materia prima disponible sin nadie |
| **PC-6** | **M7** (sem. 17) | La prueba del pasillo en treinta segundos, y después: *«¿qué he dicho que no podría defender si alguien lo comprobara?»* | Alguien que **sabe de IA y no conoce la academia** es el evaluador ideal para las dos cosas que ella no puede ver desde dentro: **jerga** y **sobreafirmación**. Y cierra el curso con otra persona, que evita el final en el vacío | Hacer la prueba del pasillo **con una compañera de otro departamento**: detecta jerga peor y sobreafirmación igual de bien. Y grabarse treinta segundos y contar los nombres de herramienta al día siguiente |

**Un uso de otra persona que NO gasta punto:** barajar las respuestas de la prueba ciega de M5 y guardar la
clave. Es una función mecánica de cinco minutos y vale cualquier compañera de la academia.

**Lo que deliberadamente NO es punto de consulta:** revisar un entregable (*«¿está bien mi asistente?»* →
rúbrica y batería) · explicar un concepto (→ material) · enseñarle a hacer algo (→ documentación) · dar
ánimos genéricos. **Y la tentación específica de esta configuración: que él le monte algo «que es un
momento».** Eso no es una consulta: es un artefacto que ella no sabrá mantener ni depurar, y en la capa
siguiente será deuda. En un curso cuyo entregable es **un sistema que tiene que sobrevivirle a ella**, un
trozo que no entiende es literalmente el peor regalo posible.

> **NOTA DE RIESGO SOBRE EL PROPIO RECURSO [NV]** *(injerto de arq-2 §7.3, y es la única contingencia
> escrita en todo el corpus sobre el **perfil de competencia** del consultor y no sobre su
> disponibilidad)*: **todo esto asume que su pareja sabe de plataformas y no solo de modelos.** Si su
> conocimiento es de modelos, **PC-4 pierde casi todo su valor** y ese punto se reasigna a PC-2 o a PC-5.
> Es un modo de fallo silencioso y más probable que la indisponibilidad, porque **la consulta ocurre igual
> y devuelve una respuesta que parece buena**. La comprobación es de un minuto y se hace en la semana 1:
> *pregúntale si ha configurado alguna vez una automatización con disparador en una suite de empresa.*

---

# 13. PLAN ANTI-ABANDONO

**Dos hechos ordenan esta sección:** el 52 % de los inscritos en un curso autodidacta **nunca llega a
empezar** [E], y **el abandono posterior es episódico y localizable**, no un desgaste uniforme. Si los
momentos son localizables, se les puede poner algo delante.

**Dos principios transversales:**
- **Toda contramedida se escribe antes del punto de caída, no en él.** El modo mínimo redactado la semana
  en que ya ha fallado se lee como excusa; redactado en la semana 1, como plan.
- **Predecir el fallo es la contramedida más barata que existe.** **Un fallo anunciado es una etapa; un
  fallo inesperado es un veredicto sobre uno mismo.**

**Se descarta como candidato al podio «el primer resultado mediocre»** —cuando el asistente contesta mal
la primera vez— no porque sea improbable, sino porque **su contramedida es barata, conocida y ya está
incorporada en cada módulo**: la caja *«lo que vas a ver la primera vez»*, escrita **antes** del ejercicio,
que describe el resultado mediocre concreto que va a obtener. Y la cita de la referencia, que es su mejor
frase y está en su última diapositiva: *«Ves el resultado. Detrás hay varias decenas de intentos.»* La
rejilla del material de origen cuantifica **72 intentos fallidos por 3 buenos**.

---

## MOMENTO 1 · Días 1–10 — el arranque, y la sospecha de haber elegido mal

**Qué pasa por dentro.** Se acumulan tres cosas, y la tercera es específica de esta columna vertebral: la
fricción de arranque; el beneficio del curso todavía es abstracto mientras el coste ya es real; y **se le
pide comprometerse con un proceso en la semana 1, que es cuando menos criterio tiene**. La conclusión
peligrosa no es «esto es difícil»: es **«creo que he elegido mal y llevo dos semanas»**, y esa es
irreversible.

**Las nueve piezas que se ponen justo antes:**

1. **La sesión 1 no explica el curso: produce un resultado utilizable en veinticinco minutos**, con lo que
   ya tiene abierto, sin instalar nada y sin hablar con nadie. **El mapa del curso va después del primer
   resultado, nunca antes.**
2. **La segunda victoria, el día 3**: el asistente con tres fuentes verdes que cita. Escalonada a
   propósito **detrás** de la primera, para que si falla ya haya una victoria debajo (§6, M0).
3. **La elección no es una apuesta: es una prueba con tres criterios de rechazo observables.** Se le quita
   el peso de «acertar» y se le da un procedimiento.
4. **El repuesto está nombrado y firmado el día 3**, no el día de la crisis.
5. **La regla del embudo vacío**, escrita (§5.4): la semana 1 **no puede terminar sin proceso**.
6. **El divorcio preautorizado, con su aritmética escrita**: al final de M1, cambiar de proceso cuesta unas
   dos horas, porque lo único construido son cuatro documentos y el método ya lo sabe.
7. **El hallazgo prometido a las 48 horas** (§5.3): los dos días de sombra dejan de ser un peaje y pasan a
   ser un pago, dentro del tramo de máxima mortalidad.
8. **El contrato de una página, antes de empezar:** 18 semanas · 2 h semanales de tiempo propio · **0 €** ·
   nada que instalar · nada que pedirle a nadie · **la frontera de M4** · y la definición observable de
   «terminado». *Un curso que se anuncia de ocho semanas y dura dieciocho se percibe como fracaso propio en
   la novena.*
9. **El modo mínimo y el ritual de reentrada, redactados en la semana 1**: una micro-sesión de diez minutos
   **cuenta como semana cumplida**, y estar en modo mínimo no es fallar; toda vuelta tras una pausa empieza
   leyendo las tres últimas entradas del cuaderno y respondiendo las cinco preguntas de repaso.
10. **PC-1 al final de la semana 2**: otra persona implicada en el punto de máxima mortalidad, revisando
    exactamente la decisión que le da miedo.

---

## MOMENTO 2 · Semanas 7–9 — el primer bloqueo que no es culpa suya

**Qué pasa por dentro.** Es el riesgo específico de trabajar sobre un proceso real. La automatización
nativa de su entorno **falla con unidades compartidas, carpetas compartidas y hojas con referencias
externas** [V]. El centro de gravedad de su puesto **es un buzón compartido y una hoja de camas
compartida**. Es decir: la primera vez que intente automatizar su trabajo de verdad, la herramienta puede
decirle que no. Y la conclusión que se saca de ahí no es «me he equivocado de carpeta»: es **«esta
herramienta no sirve para mi trabajo»**, y detrás, *«este curso no sirve para mi trabajo»*. **Es la única
conclusión de todas las simuladas que es irreversible.**

**Seis piezas, y la primera es preventiva y no paliativa:**

1. **La contramedida principal está seis semanas antes: la cuarta columna del embudo de elección.** Los
   procesos que solo viven en recursos compartidos se descartaron en la semana 1, **cuando descartar
   costaba diez minutos**. Es la diferencia entre descubrir el muro cuando cuesta diez minutos y
   descubrirlo cuando cuesta seis semanas.
2. **Aun así, el límite va en la primera página del módulo, con nombre y por escrito**, no en una fe de
   erratas: *«los primeros disparadores se construyen sobre tu propio buzón de empresa y sobre copias
   tuyas, y eso no es una versión de juguete: es la restricción real de la herramienta.»*
3. **La regla de independencia de plataforma** (§6, M3): **la ruta A —disparador por reloj dentro del chat
   que ya usa— basta para cerrar la capa y pasar la puerta.** Ningún módulo posterior depende de que el
   constructor de flujos esté habilitado.
4. **La lista de seis comprobaciones de plataforma**, entregada **antes** del primer disparador y
   reutilizable como diagnóstico. Convierte un bloqueo en una comprobación con resultado, que es lo
   contrario de un veredicto sobre una misma.
5. **La página `cuando-no-coincide.md`**, que convierte la caducidad del material en competencia enseñada:
   buscar el nombre nuevo en las novedades del proveedor · comprobar si es restricción de plan o de
   administrador · preguntarle a la propia IA cómo se llama ahora eso · y, solo si nada funciona, PC-4.
6. **La caja «si nada de esto funciona»: documenta el fallo, rodéalo con una solución manual y sigue.** Y
   la salida específica que el material nombra porque es la que más veces resuelve esto en una empresa
   pequeña: **pedir que le deleguen una etiqueta o una carpeta propia dentro del recurso compartido**. Es
   una petición a otra persona —lo que el diseño prometía no necesitar— y por eso está aquí y no en el
   camino principal.

---

## MOMENTO 3 · Semanas 11–15 — la meseta del «ya me sirve»

**Qué pasa por dentro.** Es el riesgo propio de esta columna vertebral y no aparece en las otras con esta
forma. Al terminar M4 **el sistema funciona y ella lo usa**. El dolor que la trajo al curso está resuelto.
Y justo entonces vienen módulos que no añaden funcionalidad: medir, dejarlo mantenible, clasificar,
contagiarlo. Novedad baja, beneficio inmediato bajo, esfuerzo mental alto. **El abandono aquí no se siente
como abandono: se siente como haber terminado.** Y esa es exactamente la razón por la que es peligroso,
porque **los objetivos 4 y 5 del perfil viven enteros en ese tramo**.

**Siete piezas:**

1. **La frontera declarada desde la semana 1**, y con estas palabras: *«al acabar M4 ya tienes lo que
   viniste a buscar. Lo que viene después es lo que hace que esto te siga sirviendo dentro de dos años y
   en otra empresa, y es la parte que nadie hace.»* **Nombrar la meseta antes de llegar a ella es lo que
   la convierte en un tramo y no en un final.**
2. **El gancho de M5 no es metodológico, es de deseo: el número.** Ella quiere evidenciar valor —es su
   objetivo 5, formulado por ella— y **el número es la munición**. M5 no se presenta como «vamos a
   evaluar»: se presenta como *«vas a poder decir cuánto ahorras y defenderlo si alguien lo comprueba»*.
3. **La lectura de la Tira completa como primera sesión de M5.** Cinco columnas de su propio trabajo, con
   fecha. A las trece semanas puede leer lo que en la semana 3 le parecía imposible. **Es la evidencia
   objetiva contra la ilusión de fluidez, y es gratis.**
4. **La cláusula del resultado decepcionante, escrita antes de medir:** *si la medición dice que ahorras
   poco, eso es un resultado del curso y no un fracaso tuyo.* Y las razones legítimas alternativas
   enumeradas de antemano —menos errores, menos carga mental, respuesta más rápida al cliente— con la
   instrucción de **medir esa otra razón** si es la que importa. **La honestidad de la medición está
   protegida por adelantado, que es la única forma de que la medición sea honesta.**
5. **PC-5 exactamente en la frontera** (fin de M4). Una conversación de diez minutos sobre su propio
   criterio es el mejor combustible disponible en el punto donde el material solo ya no tira. Y el objeto
   —*«¿dónde moverías la línea de corte?»*— es intrínsecamente halagador de su trabajo **sin ser halago**:
   se conversa sobre criterio, que es lo que ya tiene.
6. **El compromiso externo de M7 se anuncia en M4, cinco semanas antes.** *«En la semana 17 una compañera
   va a usar esto una semana entera sin ti.»* Un compromiso con fecha y con otra persona dentro es **el
   mecanismo de permanencia más fuerte disponible en un curso sin cohorte**, y convierte M5 y M6 en
   preparación de algo que va a ocurrir.
7. **El hallazgo vistoso se coloca en M6, no antes.** El doblete de P32 más la rejilla de los doce
   producen lo que ningún otro artefacto del curso produce: **una lista de errores reales que nadie en la
   academia sabía que existían** —precios del año pasado circulando en la plantilla alemana desde hace
   meses—. Es el momento del curso en que su trabajo produce **un hallazgo y no un ahorro**, y por eso está
   donde el material solo ya no tira. **Un hallazgo es mucho mejor combustible que un ahorro cuando quedan
   tres semanas.**

---

## Y un cuarto, menor pero real: el final sin final

**Qué pasa.** Se queda a dos módulos, sin evento que marque el fin, y el curso se desvanece en vez de
terminar. **Contramedidas:** la definición observable de «terminado» fijada en la semana 1 (§2.3) · **el
piloto de M7, que es el único evento externo del curso y tiene fecha** · **PC-6 como cierre con otra
persona** · y el calendario de revisión de M6, que fija la **próxima** fecha en que hay que volver a mirar
—lo cual convierte el final del curso en el principio de un mantenimiento, que es la forma correcta de
terminar algo que tiene que seguir vivo.

---

# 14. DURACIÓN Y DEDICACIÓN

## 14.1 El contrato, tal y como se le entrega en la semana 1

> **18 semanas · 8 módulos · 2 horas propias por semana · 0 € · nada que instalar · nada que pedirle a
> nadie para empezar · arranque en octubre.**
> **Frontera declarada: al terminar M4, semana 11, ya hay curso.**

## 14.2 El desglose honesto, y por qué se declara el tipo de tiempo

| Tipo de tiempo | Qué incluye | Cuánto |
|---|---|---|
| **Tiempo propio** | 3 sesiones núcleo de 35–45 min + el cierre de capa (40 min) | **~2 h/semana** |
| **Tiempo de trabajo** | El bloque de proyecto (60–90 min quincenal), la hoja de sombra, el cronometraje, el uso diario del artefacto, la entrevista de M7 | **~1 h/semana equivalente**, y **no es coste adicional**: es su trabajo hecho de otra manera |
| **Tiempo de otras personas** | Barajar la prueba ciega (5 min) · el piloto de M7 (una semana de uso real de una compañera, sin supervisión) · los seis puntos de consulta (1 h en total) | **~1 h 15 en dieciocho semanas** |

**Por qué la distinción va escrita línea a línea en el material y no es un detalle:** sin ella, **ella lo
contabilizará todo como tiempo propio y el curso parecerá el doble de caro de lo que es**. Y el tiempo es
la primera causa documentada de abandono: 21 de 34 abandonos lo mencionan [E].

## 14.3 Distribución real de la carga, con sus dos picos

| Tramo | Semanas | Carga propia | Nota |
|---|---|---|---|
| Arranque | 1–2 | **2 h 30 en total**, no por semana | Deliberadamente ligero: la mortalidad está aquí |
| Denso mental | 3–4 | 2 h/semana, y es **el más ligero en clics de todo el curso** | Casi todo es un documento. Se sostiene porque el asistente del día 3 ya está funcionando encima de la mesa |
| Construcción | 5–8 | 2 h/semana + bloque de proyecto | Aquí está el momento psicológico del curso |
| **Pico 1** | **9–11** | **2 h 30/semana**, tres semanas | M4 es el único módulo con aire, y se dice por qué |
| Meseta | 12–15 | 2 h/semana | Novedad baja. Aquí están todas las contramedidas del momento 3 |
| **Pico 2** | **16–18** | 2 h/semana + **una espera de una semana natural** | El piloto no se puede acelerar |

## 14.4 Por qué 18 semanas y no 12 ni 20

- **No 12:** con dos horas propias por semana, doce semanas no llegan a M5. Un curso que termina antes de
  medir produce a alguien que ha automatizado algo y no sabe si sirve, que es exactamente el perfil que su
  empresa ya tiene.
- **No 20:** es la duración de arq-1, y su propia autocrítica dice el problema: *«si ella se detiene en la
  semana 16 —que es exactamente donde se detiene la gente— nunca llega al escalón 4 ni al 5»*. Cada semana
  añadida al final es una semana con menor probabilidad de ocurrir. **Dieciocho es el punto donde caben
  los dos objetivos finales sin empujar el cierre más allá de donde la gente llega.**
- **Y arranque en octubre, no en junio.** El pico de junio–septiembre de la academia (250–400 correos al
  día) mata cualquier calendario que lo ignore; noviembre–febrero es su temporada baja. Si el curso
  empezara en primavera, M4 —el módulo más caro— caería en julio.

## 14.5 Qué pasa si el calendario se rompe

- **Modo mínimo:** una micro-sesión de diez minutos **cuenta como semana cumplida**, y el material lo dice
  con esas palabras. Estar en modo mínimo no es fallar.
- **Ritual de reentrada:** toda vuelta tras una pausa empieza leyendo las tres últimas entradas del
  cuaderno y respondiendo las cinco preguntas de repaso. Diez minutos, y elimina el coste de arranque, que
  es lo que convierte una pausa de una semana en el final.
- **M7 es movible por diseño y por escrito** (§11.5): no abre ninguna puerta, nada depende de él y contiene
  una espera que no depende de ella.
- **Y la frontera:** parar en la semana 11 con un sistema funcionando **no es abandonar**. Está escrito
  desde la semana 1, y está escrito precisamente para que parar no se lea como fracaso, porque un fracaso
  percibido no vuelve y una pausa declarada sí.

---

# 15. PRUEBA DE DURABILIDAD A DOS AÑOS

**Procedimiento.** Recorrer el mapa suponiendo que en agosto de 2028: (a) los productos se han renombrado
al menos una vez —cosa que ya ocurrió tres veces en cinco meses de 2026 con la automatización nativa de la
suite, el cuaderno de fuentes y la herramienta de terminal [V]—; (b) algunas funciones se han movido de
edición o han desaparecido; (c) su empresa ha cambiado de proveedor, **o ella ha cambiado de empresa**. Y
marcar, módulo a módulo, qué se rompe.

## 15.1 Recorrido módulo a módulo

| Módulo | Qué es criterio (sigue válido en 2028) | Qué es clic (se rompe) | Coste de reparación |
|---|---|---|---|
| **M0** | El embudo y sus cinco columnas · **la cuarta columna reformulada como pregunta de permisos** · la prueba de la sombra y sus tres rechazos · describir por observación y no por introspección · **las cinco preguntas** · las cuatro preguntas que definen cualquier plan + la quinta · «la misma frase es segura o no según con qué cuenta entres» · «pagar resuelve quién es el proveedor, no qué tratamientos están amparados» · el semáforo · el estándar «no lo sé y lo pregunté» vale / «creo que sí» no · la lista de 32 procesos · los seis motivos de zona prohibida | El distintivo concreto de la pantalla · las comprobaciones empíricas · la ruta de la consola · los mensajes literales | **1 fichero de clics.** El criterio no se toca |
| **M1** | La línea de corte y sus tres motivos legítimos · **los seis veredictos y sus pruebas** · el escalón −1 · la ficha de criterio y su prohibición de palabras · las anclas conductuales · la muestra apartada · la tabla de especificaciones · el protocolo de siete reglas · el cebo como control positivo | **Nada.** Este módulo no tiene fichero de clics | **Cero** |
| **M2** | Fuente de verdad con **fecha y dueño** · citar como forma de abaratar la revisión · «no lo sé» exigible y probable · **las tres señas de la capacidad** · seudonimización y cuasi-identificadores · la prueba de la compañera · la regla de los adjuntos · el mapa de datos · **la regla multilingüe: fuentes en español, respuesta en el idioma de la persona** · el techo de la memoria | Dónde se guarda un asistente, cuántos ficheros admite, cómo se llama la superficie de fuentes | **1 fichero de clics + 1 línea de `tres-nombres.md`** |
| **M3** | Disparador por calendario frente a suceso · el tope · el apagado probado · «prepara, no envíes» y su motivo · «automatiza donde ya viven tus datos» · **la prueba del caso que NO debe disparar** · la notación neutra · **las tres señas del disparador** | Los límites concretos de la plataforma (recursos compartidos, un disparador por flujo, tope de etiquetas) · el catálogo de pasos disponibles | **1 fichero de clics + la lista de seis comprobaciones**, que hay que reescribir con los límites de la plataforma nueva. **Es la reparación más cara del curso** |
| **M4** | Temas prohibidos frente a condiciones de parada · las seis condiciones y su motivo · **la parada por idioma no probado** · **la parada por agencia con convenio** · «parar no es callarse» · el revisor con nombre y hora · el plan de fallo en cinco pasos · «la confianza no es una salvaguarda» y el riesgo del día 60 · empatía sin admisión · privilegio mínimo · **la ficha de cinco preguntas aplicada a una herramienta ajena** | Cómo se implementa una bifurcación y un tope hoy · qué producto está detrás de qué plan · **las fechas del marco normativo** | **1 fichero de clics + la caja del fondo**, que se revisa entera —está diseñada para eso: su primera columna son condiciones—. **Y `datos-volatiles.md` para las fechas normativas**, que caducan más rápido que los productos |
| **M5** | Línea base · minutos por unidad · coste completo · las seis amenazas a la validez interna · proceso frente a resultado · cadena causal · prueba ciega · la lectura de la Tira | **Nada.** Es metodología, un cronómetro y una hoja de cálculo | **Cero** |
| **M6** | Fuentes con caducidad y dueño · calendario de revisión · apagado probado · escribir la propia rúbrica y validarla contra un cebo · la prueba del hueco · **la rejilla de los seis veredictos aplicada a doce procesos** · la regla del cuatro · la comprobación de las tres filas al azar | Los nombres de las herramientas del apéndice opcional | **1 párrafo** |
| **M7** | El número y su método · la reproducción ±10 % · «qué NO hace» · la jerarquía de la evidencia · la demo de tres minutos · la prueba del pasillo y sus cuatro comprobaciones · **la semana sin ella** · la ficha de traspaso · las cuatro reglas de arranque · la deuda de adopción · la entrevista de proceso ajeno | **Nada** | **Cero** |

## 15.2 Recuento

| | Módulos | Proporción |
|---|---|---|
| **Sin nada que reparar** (M1, M5, M7) | 3 | 37 % |
| **Reparación de un fichero de clics o un párrafo** (M0, M2, M6) | 3 | 37 % |
| **Reparación media** (M4: clics + revisión de la caja del fondo + fechas normativas) | 1 | 13 % |
| **Reparación cara** (M3: clics + lista de comprobación de plataforma) | 1 | 13 % |
| **Módulos que habría que rediseñar** | **0** | **0 %** |

**Por instrumento:** las **cinco preguntas no caducan** —clasifican por una propiedad, no por un catálogo— ·
la **rejilla de los seis veredictos** caduca **parcialmente y de forma prevista** (ver §15.4) · la **Tira no
caduca** · el **Cuaderno de capas caduca en ocho líneas** —la línea de techo de cada ficha— por diseño · la
**Lista de techos no caduca porque su tercera columna son condiciones** · el **Expediente no caduca** —una
academia de idiomas en 2030 seguirá emitiendo cartas de visado y contestando leads— · y la **tabla de tres
nombres caduca entera**, y por eso está aislada en una sola página fechada con su nota al pie: *«esta es la
única página del curso que caduca por completo. Corrígela tú: es tuya. Lo que no cambia es la columna de la
izquierda.»*

**Veredicto: no hay que rediseñar.**

## 15.3 Cinco cosas que esta prueba obligó a cambiar, y que ya están incorporadas

1. **La cuarta columna del embudo se reformuló** de *«¿los ficheros que abro son míos o compartidos?»* a
   *«¿sobre qué recursos puedo actuar yo, no mirar, sin pedirle permiso a nadie?»*. La primera codificaba
   un límite de un producto de 2026 dentro de la mitad de criterio; la segunda es una pregunta de permisos
   que acota **cualquier** plataforma de automatización de **cualquier** año — y es, de hecho, la pregunta
   4 de las cinco preguntas aplicada a su propia cuenta. **El límite numérico concreto se fue a clics.**
2. **Los módulos se titulan por capa y no por lo que se construye.** Un primer esbozo tenía módulos
   llamados «El asistente que cita» y «La columna que clasifica sola». Con eso, **medio índice del curso
   nacía caducado y —peor— el índice enseñaba lo contrario que el contenido.**
3. **Apareció el tercer registro.** Dos registros dejaban sin cubrir la habilidad que más falta va a hacer
   en 2029: encontrar una función en una pantalla que no ha visto nunca. La tabla de tres nombres no
   sirve para eso, **por su propia declaración**; las señas funcionales sí.
4. **La caja del fondo cambió de eje.** Antes listaba productos con una columna de «cuándo te tocaría».
   Ahora **la fila es la condición** y el producto es el ejemplo de hoy. Con el eje anterior había que
   rehacerla entera cada año; con este, se revisa.
5. **Las fechas normativas salieron del texto y se fueron a `datos-volatiles.md`.** El calendario del
   Reglamento de IA ya se movió una vez en 2026 y volverá a moverse; el estado del marco de transferencias
   a Estados Unidos depende de una sentencia pendiente. **Lo que no cambia son los seis principios y la
   asimetría del Anexo III**, y eso es lo que se queda en el criterio.

## 15.4 Los tres escenarios de 2028, corridos de frente

**(a) ¿Y si un solo producto acaba haciendo todos los escalones?** Es plausible: la tendencia es que la
misma ventana de chat programe, dispare por sucesos y actúe. Si ocurre, **este diseño no se rompe: se
vuelve más necesario**, porque el producto deja de forzar la distinción y **ya nada, salvo el criterio, le
dice a la persona cuánta autonomía acaba de ceder**. Las cinco preguntas se responden igual dentro de una
sola ventana. Y la Tira sigue produciendo la misma lectura: *¿esto me cambia la calidad o me cambia el
disparador?*

**(b) ¿Y si los modelos dejan de alucinar y de necesitar fuentes citadas?** No hace falta apostar. M2 **no
enseña «cita porque alucina»**: enseña **cita porque tu revisión tiene que durar cinco segundos y porque
una fuente caducada responde con toda la confianza del mundo**. Ese segundo motivo no depende de la calidad
del modelo: depende de que los tarifarios cambien, y van a seguir cambiando.

**(c) ¿Y si la partición de los seis veredictos pierde su referente?** Es la crítica más afilada del juez 3
y hay que asumirla en vez de esquivarla: **los veredictos 4, 5 y 6 son fronteras de producto de hoy**, y el
día en que una sola superficie haga las tres, tres de las seis casillas se quedan sin referente comercial.
**Lo que sobrevive entero es el 1, el 2 y la zona prohibida** — que es el tercio, y es el mejor tercio,
porque es el que contiene los dos noes. Tres decisiones de diseño lo mitigan:
- **Las pruebas que deciden cada veredicto interrogan la tarea, no la herramienta** —*¿cabe en una
  servilleta? ¿puedes nombrar el documento y su fecha? ¿los pasos son siempre los mismos?*—, y esas
  preguntas **no caducan aunque la casilla de destino se renombre**.
- **La rejilla convive con las cinco preguntas**, que sí son dimensionales. Si la partición se difumina, la
  clasificación no desaparece: se hace con el instrumento 1 en vez de con el 2.
- **La revisión está prevista**: la segunda vuelta de M7 pregunta explícitamente *qué condiciones han
  cambiado*, y esa operación es la que ella tendrá que repetir cada año, con o sin curso.

## 15.5 Lo que sigue siendo frágil aunque el diseño esté bien

Una prueba de durabilidad que sale limpia del todo es sospechosa. Tres cosas:

- **M3 es el punto débil y no tiene arreglo estructural.** La anatomía de un disparador es durable, pero
  **los límites concretos de una plataforma no son un adorno del módulo: son la mitad del módulo**, porque
  son lo que determina si su buzón compartido se puede tocar o no. Si cambia la plataforma, hay que volver
  a averiguar los límites, y eso no se hereda.
- **La lista de 32 procesos envejece despacio, pero envejece.** Una normativa de extranjería nueva, un
  canal de captación que desaparece, y hay filas que dejan de existir. Sigue siendo el activo más duradero
  del curso, pero **conviene fecharla como cualquier otra fuente**.
- **Y una asimetría incómoda:** lo que menos caduca de este curso es lo que menos se parece a «un curso de
  IA» —mirar un proceso, escribir criterios, medir, traspasar, contagiar— y lo que más caduca es lo que más
  se parece. Es la mejor prueba de que el listón está bien puesto, **y también el motivo por el que el
  material tiene que trabajarse el enganche de M1, M5, M6 y M7 mucho más que el de M3.**

---

# 16. QUÉ SE QUEDA FUERA, A PROPÓSITO

## 16.1 Fuera porque el brief lo excluye

| Fuera | Por qué |
|---|---|
| **«Cómo conseguir el sí», venta interna, argumentarios, plantillas de petición a dirección** | En su empresa usar IA ya está bien visto y **lo mal visto es no automatizar**. Un módulo de permiso resuelve un problema que ella no tiene. Lo que sí entra —evidenciar y contagiar— es otra cosa y está en M7 |
| **Portfolio, landing page, prototipo de aplicación, «lo que tengo ahora en mi CV»** | Es el destino del itinerario no técnico de la referencia porque **su alumno tipo quiere entrar en el sector de la IA**. La nuestra no quiere cambiar de rol ni de sector. Lo que sí quiere —que le sirva si cambia de empresa— lo dan los seis instrumentos permanentes, no una web |
| **Certificado, insignia, «ahora eres AI Operator»** | No busca cambiar de rol. Y un certificado sin evaluador y sin rúbrica no certifica nada. La definición de «terminado» de §2.3 es observable y no la firma nadie |
| **Convertirse en especialista en IA** | El objetivo es trabajar mejor en lo suyo. Todo lo que empuje hacia «ser la persona de la IA» como identidad profesional está fuera, **incluido el vocabulario** |
| **Cualquier cosa vistosa** | El grafo de la referencia es el caso de estudio: espectacular en pantalla, marginal en valor para un puesto de atención al cliente, y —dicho por su propia autora— *hecho para el agente, no para el humano*. Aquí el artefacto útil es aburrido: un asistente que cita, un triaje que etiqueta, un vigilante que avisa |
| **Construir y vender aplicaciones** | Ni siquiera la referencia lo promete, y con razón: *«construir algo para uso interno y publicarlo en internet son dos mundos distintos»* |
| **Coleccionar herramientas** | Dos o tres capacidades nuevas en dieciocho semanas, y ninguna antes de haber agotado la anterior |

## 16.2 Fuera por el listón de durabilidad, con su condición de reentrada

Un «no» sin condición de revisión es dogma. Todo lo que sale tiene su fila en la Lista de techos o en la
caja del fondo, con la condición que lo devolvería.

| Fuera | Reducido a | Condición para que entre |
|---|---|---|
| **Plataformas de automatización externas como módulo** | Una fila de la caja del fondo + el criterio *automatiza donde ya viven tus datos* | Que su proceso tenga que actuar sobre algo fuera de su suite. Y una que haya que autoalojar, **solo si aparece alguien técnico que la mantenga** |
| **Escribir código, aunque lo escriba la IA** | Media página informativa | Que la automatización nativa se quede corta **y** haya quien mantenga el script. En el momento en que falla hay que leer un error de programador, y **esa es una dependencia que ella no puede cubrir** |
| **La superficie de desarrollador «gratis y de la misma empresa»** | Cinco líneas, con aviso explícito | **Ninguna.** Es la trampa más silenciosa del panorama y por eso se nombra: parece profesional, se entra con la cuenta de siempre, y **sus términos dicen literalmente que no metas información personal** |
| **Conectores y su estándar, como práctica** | Vocabulario + el principio de privilegio mínimo | Que monte algo fuera de su suite, o que alguien se lo configure y ella solo lo use |
| **Arquitecturas de recuperación sobre corpus grandes** | Una fila de la caja del fondo | Que las fuentes pasen de decenas a cientos y el asistente empiece a perderse |
| **Herramientas agénticas de escritorio y de terminal** | Un apéndice de lectura, opcional, **sin entregable** | Una tarea que exija procesar decenas de ficheros locales de forma repetida. **Si termina el curso sin abrir el apéndice, el curso ha funcionado igual**, y eso va en su primera línea |
| **Comparativas y nombres de modelo, benchmarks** | Nada | **Ninguna.** *«Da bastante igual qué modelo uses mientras no gastes miles en tokens.»* El material no se apoya en ningún nombre de modelo, a propósito: es el detalle que menos importa y el que más rápido caduca |
| **Tour por los productos de su suite** | Nada | Solo entra lo que su proceso pide o lo que una fila de la rejilla pide. El resto, ni mencionado |

## 16.3 Fuera por rigor mal invertido — y este es el bloque específico de este perfil

**El riesgo de esta alumna no es quedarse corta de rigor: es pasarse.** Un solo proceso es un imán para el
perfeccionismo. La regla que lo contiene se repite en cada módulo: **el montaje se hace rápido y sucio; el
rigor se gasta entero en la evaluación.**

- **Estadística inferencial.** Nada de significación, valor p ni tamaño muestral sobre doce casos. Aquí no
  se estima un parámetro de una población: **se comprueba la cobertura de un instrumento contra un criterio
  fijado**. Doce casos bien elegidos valen más que doscientos al azar.
- **Consistencia interna aplicada a la batería.** Directamente incorrecto: una batería **debe ser
  heterogénea**. Si tuviera consistencia interna alta sería porque está mal construida. En un banco de
  pruebas la heterogeneidad es una virtud, al revés que en una escala.
- **Consentimiento informado como equivalente de base jurídica**, y **anonimato de investigación como
  equivalente de anonimización**. Son falsos amigos con consecuencias, y se cortan explícitamente.
- **Prompt engineering como colección de trucos.** El curso enseña **el criterio antes del prompt**. Un
  prompt bueno que se escribe una vez y se pierde no vale nada; el mismo guardado con sus fuentes es
  infraestructura.
- **Vídeos de lección.** Un vídeo es relectura con mejor producción, y la relectura es técnica de utilidad
  baja. Si hay vídeo, es demostración de una interfaz, dura menos de tres minutos, va con transcripción
  escrita **y vive en la carpeta de clics**, porque la ruta de menús caduca y el texto se corrige.
- **Cualquier ejercicio de metodología sin artefacto reutilizable.** Si un ejercicio le lleva más de lo que
  le llevaría hacer la tarea a mano durante un mes, **está mal calibrado y se recorta**.
- **La estructura de cinco semanas con cuatro lecciones semanales de la referencia.** Asume cohorte, LIVEs
  y mentores. Aquí el ritmo lo pone una jornada completa y el pico de julio.

## 16.4 Fuera por riesgo, con nombre y número

**P08** visados · **P26** quejas formales · **P29** emergencias · **P25** reembolsos · **P17** matching con
familias · **P22** calendario de camas · **P05/P16** nivelación y exámenes. **No son «temas avanzados»: son
zona prohibida con motivo escrito** (§9.3), y **el motivo es contenido de primera, no una advertencia**,
porque es lo único que se transfiere a un caso nuevo.

## 16.5 Fuera por decisión propia de este diseño, y son las tres discutibles

1. **La segunda automatización.** El curso construye **una** cosa. No hay un segundo proceso y no hay un
   hilo guiado que ella ejecute además del suyo: el expediente modelo se lee y se usa como clave, no se
   hace. Con dos horas propias por semana, **dos procesos son dos procesos a medias**, que es exactamente
   lo que esta columna vertebral existe para evitar. El segundo proceso es lo primero que hará **después**
   del curso, y para eso están la rejilla de los doce ordenada por prioridad, la Lista de techos, la
   rúbrica escrita por ella y la ficha de traspaso. *(El coste, en §17.2.)*
2. **El Semanario de once columnas.** Se sustituye por el tachón de los 32 en M0 y la rejilla de los doce
   en M6, que producen el mismo volumen de juicios sin cuatro semanas de documento en el tramo de máxima
   mortalidad. *(El coste, en §17.3.)*
3. **La ordenación del curso por la escalera de herramientas.** La escalera se respeta como progresión
   (§7) pero no gobierna el índice, porque ordenar por autonomía cedida obliga a subir aunque su realidad
   operativa no llegue a esa altura, y deja el muro del buzón compartido para la semana 9. Lo que sí se
   toma entero de ese diseño son sus instrumentos.

---

# 17. DÓNDE ME APARTO DE LOS JUECES, Y LO QUE ESTE DISEÑO NO RESUELVE

Sin esta sección, las dieciséis anteriores no son creíbles. Y hay un motivo extra para escribirla: **las
tres arquitecturas candidatas tenían autocrítica y arq-3 —la que sirve de columna vertebral— citaba una
sección §14 que no existe en el fichero**, más de diez veces, y siempre para aplazar precisamente los
límites de sus propios mecanismos. Ese hueco no se hereda.

## 17.1 Los cinco sitios donde me aparto de un juez, y por qué

**(1) Contra los jueces 2 y 3: la columna vertebral no es arq-1.**
Los dos la eligen, y los dos la eligen **por sus instrumentos**: las puertas, las cinco preguntas, el
tercer registro, la prueba de traducción. Los cuatro están injertados aquí, enteros. Lo que no se toma es
la ordenación por autonomía cedida, y el argumento decisivo lo escribe su propio autor: *«he elegido el
diseño que se termina antes que el que enseña más»* (autocrítica 8), más veinte semanas, más cinco de diez
módulos sin capacidad nueva, más el muro del buzón compartido declarado **sin resolver** (autocrítica 2).
**Bajo el sesgo de este encargo —criterio transferible por encima de resultado rápido— elegir el diseño que
enseña menos porque se termina antes es exactamente la decisión que no hay que tomar**, sobre todo cuando
el que enseña más se puede terminar igual añadiéndole las puertas.

**(2) Contra el juez 4: la columna vertebral tampoco es arq-2.**
Tiene razón en el diagnóstico —es la que mejor verifica el dominio contra su semana y la única que trata
el multilingüismo con instrumento— y sus dos aportaciones se injertan enteras. Pero su columna vertebral
**es un documento**, y su propia autocrítica 13 lo dice mejor que ningún juez: *«un Semanario es un
documento, y los documentos no contestan correos»*. Su MOMENTO 1 se titula *«el inventario como muro»* y
admite *«hemos puesto el trabajo árido exactamente donde más gente se cae»*. Su volumen de juicios —que es
lo que de verdad vale— **no necesita esa columna vertebral: necesita una rejilla y dos momentos donde
aplicarla**, y eso es lo que hace §4.2.

**(3) Contra el juez 3: la cuarta columna del embudo SÍ se injerta, reformulada.**
Él pide explícitamente **no** injertarla porque codifica un límite de producto de 2026 dentro de la mitad de
criterio. El diagnóstico es correcto y el remedio no: la reformulación de §5.2 —*«¿sobre qué recursos puedo
actuar yo, no mirar, sin pedirle permiso a nadie?»*— es una pregunta de permisos, es durable, es
literalmente la pregunta 4 de su propio instrumento favorito, y conserva lo que los jueces 1 y 4 consideran
la mejor decisión de diseño del corpus. **El límite numérico concreto va a clics, que es donde él quería
mandarlo.**

**(4) Contra el juez 1 (parcialmente): el asistente del día 1 se escalona, no se adelanta.**
Él pide moverlo al día 4–5. Lo muevo al **día 3** y **detrás** del diagnóstico del entorno, no delante,
porque el diagnóstico es lo que decide si esa caja va a funcionar. Y mantengo su razón de fondo: sin ese
segundo artefacto, las semanas 3–4 de documentación transcurren sin nada suyo encima de la mesa.

**(5) Contra los cuatro: el volumen de juicios de arq-2 se recupera, pero en la semana 14.**
Ningún juez propone esto. El juez 3 pide el volumen; el juez 1 advierte contra el muro; el juez 2 señala
que el Mapa de arq-2 se construye **cuando menos criterio tiene y sin nadie que lo corrija**. **Las tres
cosas se satisfacen a la vez colocando la clasificación masiva al final, cuando ya no gobierna nada y ya
hay criterio**, y usando el hueco que deja en M1 para la línea de corte, que es la misma operación sobre
un objeto que ella conoce mejor que nadie.

## 17.2 El coste de renunciar al doble hilo, y cómo se compensa

`dominio-autodidacta.md` §7.1 recomienda **dos hilos**: uno guiado con clave y uno propio sin ella, porque
*«si el proyecto está mal elegido, no hay quien lo detecte y el curso entero se hunde con él»*. **Lo
desoigo**, y el coste es real y concreto: **casi todas las claves las escribe ella, con los mismos puntos
ciegos con los que va a construir.**

Cuatro compensaciones, y hay que juzgarlas por lo que son —una reparación parcial, no una equivalencia—:

1. **Los ocho dobletes llevan clave sellada escrita por el curso** (§9.2). Son ocho contrastes con oráculo
   externo sobre procesos que no son el suyo. **Esta es la compensación fuerte, y es nueva respecto a las
   tres arquitecturas.**
2. **Tres cebos** repartidos (M1, M4, M6), uno por fase, con el tercero con función temporal declarada.
3. **El expediente modelo con desvanecimiento**, que es el hilo guiado convertido en lectura con clave.
4. **Las puertas**, que sustituyen el «todavía no» del profesor por una condición observable.

**Lo que aun así no se cubre, y hay que decirlo:** nadie va a decirle que **su ficha de criterio mide lo
que no importa**. Puede escribir cinco indicadores observables e irrelevantes y pasar todos los filtros. El
único mecanismo que hay contra eso es el ítem *«al menos un indicador verificable contra fuente externa; si
todos son críticos, no ha priorizado»*, y **es poco**. Es el defecto compartido por las tres arquitecturas
y este diseño solo lo mitiga.

## 17.3 Los seis puntos donde este diseño puede fallar

**1 · Sigue pidiéndole comprometerse con un proceso en la semana 1.** Todo el aparato de §5 —sombra,
repuesto, divorcio con aritmética, embudo vacío— **acota la ansiedad; no la elimina**. Es el riesgo
estructural del ángulo y se paga por elegirlo.

**2 · La Tira es la mejor idea del diseño y la más frágil de mantener.** Exige sostener diez casos vivos
durante dieciocho semanas y volver a pasarlos cinco veces. Es poco trabajo cada vez —media hora— pero es
**trabajo sin novedad**, y lo que no tiene novedad se convierte en ritual o desaparece. Si la Tira se
erosiona, **desaparece la lección central del curso**. Las puertas la fuerzan, pero las puertas se pueden
saltar en un curso sin profesor.

**3 · La rejilla de los doce, en la semana 14, puede no llegar a hacerse.** Es el precio de haberla movido:
en arq-2 caía en la semana 3, donde es un muro pero **ocurre**; aquí cae en la meseta, donde no es un muro
pero **puede ser lo primero que se salte**. La contramedida es que sea la puerta de M6 y que su salida sea
materia prima directa de M7, pero no es una garantía.

**4 · El módulo de evangelización sigue siendo el menos autocorregible del curso.** El piloto es binario y
tiene criterio negativo, la reproducción del número es mecánica y la prueba del pasillo se cuenta. Pero
**no se puede dar una rúbrica a «la organización lo adoptó»**, que es la palabra del brief. Y hay un modo
de fallo que no se cubre: que el piloto ocurra **por cortesía** —la usa porque es ella— y el resultado sea
un falso positivo. La única mitigación es que el entregable no sea el veredicto sino la lista de arreglos,
y es una mitigación indirecta.

**5 · El módulo de evangelización puede volverse en su contra, y la contramedida es de una página contra
una dinámica organizativa.** En una empresa de treinta personas donde lo mal visto es no automatizar,
hacerse visible como «la que sabe de IA» tiene un desenlace previsible: que le caiga trabajo ajeno. Está
escrita la contramedida —entregar el artefacto y el manual, no el servicio; la frase de límite; el bus
factor invertido— **y las dinámicas organizativas suelen ganar a las contramedidas de una página.**

**6 · Todo el diseño depende de un dato que no tenemos [NV].** Qué plan tiene contratada su empresa y cómo
está configurado. Si resulta ser la edición reducida, media docena de funciones no existen para ella y M3
pierde su ruta B. Hay contingencia escrita —la regla de independencia de plataforma— **pero una contingencia
no es lo mismo que un diseño**, y no se sabrá hasta la semana 2, con el curso ya escrito.

## 17.4 Lo que no he verificado, y que hay que decir antes de producir material

- **Los 32 procesos, los volúmenes, el buzón compartido, la carpeta de plantillas con seis versiones: todo
  es reconstrucción [R]** a partir del sector, no observación de su empresa. El curso está diseñado para
  que **su primera tarea sea tachar y corregir** ese mapa, que es la única forma honesta de convertir una
  reconstrucción en su realidad. **Pero si el mapa está muy equivocado, M0 tendrá que reescribirse sobre la
  marcha, y varios ejemplos perderán fuerza precisamente por lo que se supone que los hace fuertes: por ser
  concretos.**
- **No existen datos publicados sobre cómo se comporta un modelo de 2026 corrigiendo un entregable contra
  una rúbrica dada**, que es exactamente nuestro caso. **Los tres cebos no son un adorno: son lo único que
  tenemos**, y puede resultar que la respuesta sea *«para este tipo de trabajo, la IA no corrige»*. El
  diseño está preparado para ese resultado —la calibración por entregable de §12.4 lo contempla— pero es
  una posibilidad real y no una hipótesis remota.
- **El multilingüismo está resuelto por diseño, no probado.** La ruta de respaldo sobre el expediente
  modelo existe, pero **si su proceso resulta ser monolingüe, tres de los ejercicios más valiosos se hacen
  sobre material que no es suyo**, y eso baja su rendimiento aunque no lo elimine.
- **La cuota de tres noes en los dobletes es más fiable que la de arq-2 porque hay clave**, pero **la regla
  del cuatro en la rejilla de los doce no tiene clave posible** y depende de su honestidad consigo misma,
  sin nadie que compruebe. La señal de fallo está escrita —*«existe un veredicto 1 o 2 que puse para llegar
  a cuatro, no porque lo crea»*— y no basta.

## 17.5 Y la asimetría que resume el diseño entero

> **Lo que menos caduca de este curso es lo que menos se parece a un curso de IA** —mirar un proceso,
> escribir criterios, partirlo en trozos con veredicto, medir, traspasar, contagiar— **y lo que más caduca
> es lo que más se parece.**

Es la mejor prueba de que el listón está bien puesto. Y es también la advertencia de producción más
importante que deja este documento: **el material tiene que trabajarse el enganche de M1, M5, M6 y M7
mucho más que el de M3**, porque son los módulos donde está el valor duradero y son los que peor se venden
solos.
