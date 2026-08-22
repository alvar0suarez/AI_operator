# Arquitectura 3 — «Un proceso real, de punta a punta, y luego contagiarlo»

**Ángulo:** el curso es la transformación de **un** proceso suyo, elegido pronto y llevado hasta que
funciona de verdad y ella lo usa a diario. Cada módulo añade **una capa a la misma cosa**. La teoría
entra cuando el proceso la exige. La última fase convierte eso en algo que sus compañeros adopten.

**Brief:** `00-perfil.md`, revisado por segunda vez el 22.08.2026. **Manda sobre este documento.**
**Fecha:** 22.08.2026.

**Documentos que da por leídos:** `00-perfil.md`, `01-analisis-referencia.md`, `dominio-academia.md`
(P01–P32), `dominio-rgpd.md` (E-01…E-06, el semáforo), `dominio-herramientas.md` (escalones 0–4 y
límites de plataforma verificados), `dominio-autodidacta.md` (mecanismos de corrección, puntos de
caída, plantillas), `dominio-psicologia.md` (C1–C13, EP-01…EP-14, los nueve falsos amigos), las seis
notas `fuente-*.md`, y las arquitecturas hermanas `borrador-arq-1-escalera.md`,
`borrador-arq-2-inventario.md` y `arq-2-inventario.md`.

**Convención de marcas:** **[V]** verificado en fuente primaria · **[R]** reconstrucción razonada ·
**[E]** evidencia publicada citada en los documentos de dominio · **[NV]** no verificable desde fuera ·
**[!]** decisión que no es suya y se escala · **[J]** juicio de diseño mío, argumentado y sin respaldo
externo.

**Relación con las arquitecturas hermanas.** La 1 ordena el curso por **techos de herramienta**; la 2,
por el **inventario de su semana**. Esta ordena el curso por la **anatomía de un proceso delegado**.
Donde converjo con ellas lo digo (varias piezas de corrección sin mentor son comunes porque salen del
mismo informe de dominio y sería absurdo reinventarlas peor); donde me separo, lo argumento. La
comparación explícita está en §1.6 y la parte incómoda, en §14.

---

# 0. Resumen en dieciséis líneas

1. El curso **no recorre herramientas ni recorre su inventario: recorre un proceso**. Uno solo, suyo,
   elegido en la primera semana con un filtro observable, y llevado hasta que funciona y lo usa.
2. Los módulos son **capas**, y las capas son la anatomía de cualquier tarea que se delega: verla,
   escribir qué es un resultado correcto, darle contexto, quitarle el dedo del disparador, meterle
   juicio y frenos, medirla, dejarla viva sin ti, y contagiarla.
3. **La escalera del perfil se respeta literalmente, pero no es el plan de estudios: es lo que le pasa
   a un proceso cuando lo aprietas.** Chat mejor usado = capa 2. Automatización = capa 3. Agente =
   capa 4. No se «suben escalones»: se choca con techos dentro de lo mismo.
4. La teoría entra cuando el proceso la pide, y **solo la que pide**. Nada de panorama previo.
5. **El criterio portátil se extrae con una pregunta fija al cerrar cada capa**, y se responde en tres
   líneas con una regla mecánica: toda respuesta tiene dos mitades —lo que vale para cualquier proceso
   y lo que era de *este*—. Una respuesta sin la mitad negativa está mal.
6. La contramedida a que un solo proceso vuelva el curso monocultivo es **el Doblete**: cada capa se
   repite en seco, veinte minutos, sobre un proceso distinto. **Al menos tres de los ocho dobletes
   tienen que terminar en «aquí no aplica».**
7. La contramedida a elegir mal el proceso es **la prueba de la sombra**: dos días laborables de
   observación con tres criterios de rechazo observables, antes de comprometerse. Y un **divorcio
   preautorizado** cuyo coste está acotado por diseño: al final de la capa 1 rehacer todo son dos horas.
8. **El mejor corrector de este diseño es que el artefacto está en producción sobre su propia mesa.**
   El mundo la corrige cada martes. Su límite —detecta fallos de utilidad, no de criterio— es lo que
   justifica todo el aparato de rúbricas, baterías y cebos.
9. **La misma batería de diez casos atraviesa el curso entero**, con una columna nueva y fechada por
   capa. La lectura de esa tabla es la lección central: entre la capa 2 y la capa 5 la calidad apenas
   mejora; lo que cambia es **quién dispara y cuánto cuesta**.
10. El curso es **agnóstico de herramienta y lo demuestra físicamente**: criterio y clics viven en
    ficheros distintos, con dos reglas de redacción comprobables —la regla del sujeto y la prueba del
    sustituto— y una prueba de traslado real.
11. **La protección de datos no es transversal difusa: es una capa del proceso.** El artefacto es el
    **mapa de datos del proceso**, y se hace cuando toca meterle datos, no antes ni después.
12. «Saber qué existe» se construye por **techos**: cada capa declara qué no puede hacer y qué clase de
    cosa lo rompería. Nueve techos escritos por ella = el catálogo, y no caduca porque son condiciones.
13. **La evangelización interna es el módulo M7**, va al final porque consume el número de M5, y su
    prueba de éxito es una sola: **la semana sin ella**.
14. Seis puntos de consulta de diez minutos con su pareja, con ficha escrita antes y alternativa
    degradada en todos. El primero audita **el razonamiento de su elección**, no su trabajo.
15. **Ocho módulos, 18 semanas, dos horas propias por semana, cero euros, arranque en octubre.**
16. Y la frontera declarada desde la semana 1: **al acabar M4 (semana 11) ya hay curso**. M5–M7 es
    donde se cobran los objetivos 4 y 5, y donde este diseño se juega si sirve para algo más que
    resolver un martes.

---

# 1. TESIS

## 1.1 Enunciado

> **Se aprende haciendo una cosa entera, no doce a medias. Un proceso llevado de punta a punta —hasta
> que funciona, hasta que ella lo usa sin que nadie se lo pida y hasta que sobrevive a sus
> vacaciones— enseña más criterio que doce diagnósticos sobre papel, porque es el único formato en el
> que cada decisión recibe la respuesta del mundo.**
>
> Y su corolario, que es lo que convierte esto en una arquitectura y no en un lema:
> **el curso no la lleva por una escalera de herramientas. La escalera aparece sola, por debajo,
> porque un proceso al que aprietas va pidiendo cosas en ese orden.** Primero pide que alguien escriba
> qué es hacerlo bien. Después pide contexto que no haya que volver a explicar. Después pide dejar de
> depender de que ella se acuerde. Después pide juicio en dos sitios y frenos en otros tres. Después
> pide que alguien compruebe si de verdad sirve. Y al final —solo al final— pide poder existir sin ella.

Tres corolarios operativos:

> **(a) La unidad del curso es la capa, no la herramienta ni la tarea.** Un módulo se llama «Que ocurra
> sin que lo pidas», no «Acciones programadas» ni «Automatizar el proceso 27». La capa es la anatomía;
> la herramienta es la implementación de hoy y vive en un apéndice fechado.
>
> **(b) La teoría entra por demanda del proceso, y solo la que el proceso pide.** No hay módulo de
> panorama, no hay catálogo previo, no hay lección de «qué es un agente» antes de que el proceso se
> quede corto. Lo que no pide el proceso se cubre con veinte minutos en seco (el Doblete) o no se
> cubre, y se dice.
>
> **(c) El «no» vive dentro del proceso, no fuera.** El primer entregable serio del curso no es «qué
> automatizo» sino **la línea de corte**: qué trozos de este proceso entrego y qué trozos se quedan
> conmigo, con el motivo escrito. Un proceso partido en trozos con veredicto es el sitio más barato
> del mundo para aprender que a veces la respuesta es que no.

## 1.2 Por qué esta tesis es la correcta para ESTA alumna con ESTOS objetivos

Siete argumentos, en orden de peso. Los cinco primeros son específicos de ella: con otro perfil no
serían igual de fuertes.

**(a) Porque su objetivo literal es un cambio de hábito, y un hábito solo se sustituye si el gesto
nuevo gana al viejo en su propia mano, todos los días.**
El perfil dice *«salir del hábito del chat»*. Un hábito no se cambia con un mapa ni con doce
veredictos: se cambia cuando el gesto antiguo produce un resultado peor que el nuevo, **en la tarea que
ella hace de todas formas**. Un curso que produce un artefacto que ella usa el martes siguiente compite
con el hábito en su propio terreno; un curso que produce documentos compite con él en abstracto y
pierde. Este es el único ángulo cuyo entregable **es** el hábito nuevo.

**(b) Porque es el único formato en el que el mundo corrige, y sin mentor eso vale más que cualquier
rúbrica.**
`dominio-autodidacta.md` §3.2 ordena los mecanismos de corrección por eficacia real y pone en primer
lugar la **ejecución real** —el artefacto funciona o no funciona— precisamente porque no requiere el
juicio de nadie. Un proceso en producción sobre su mesa maximiza ese mecanismo: cada día que lo usa, lo
prueba. Un proceso que solo se diseña sobre papel no lo activa nunca. **La decisión de diseño más
rentable de un curso sin profesor es meter el artefacto en producción cuanto antes**, y este ángulo es
el que lo hace desde la semana 2.

Su límite hay que decirlo en la misma frase, porque si no esto sería trampa: **funcionar no es estar
bien**. El uso diario detecta que algo molesta; no detecta que el criterio estaba mal escrito ni que la
batería era fácil. Por eso todo el aparato de §3 —batería con clave sellada, listas binarias, rúbricas
negativas, cebos— sigue estando entero. El mundo corrige la utilidad; los instrumentos corrigen el
criterio.

**(c) Porque la profundidad es la única forma de que vea la curva de iteración, y esa curva es la
lección anti-hype más importante que puede llevarse.**
La mejor frase de la referencia está escrita, no dicha, en su última diapositiva: *«Ves el resultado.
Detrás hay varias decenas de intentos.»* La rejilla del frame `0046` cuantifica **72 intentos fallidos
por 3 buenos**. Un curso que hace doce cosas a un cuarto de profundidad **nunca le enseña eso**: le
enseña doce primeras versiones, que es exactamente el material del que está hecha la ilusión de que la
IA es una varita. Llevar una cosa hasta la versión cuatro es la única manera de que descubra por
experiencia que la versión dos es donde estaba el valor, y que la versión uno siempre parece un
borrador. `dominio-autodidacta.md` §1.4a documenta que su termómetro está invertido: lo que se siente
cómodo enseña menos. Doce cosas a medias se sienten estupendamente.

**(d) Porque es el uso más rentable de su formación, sin halagarla — y también el más incómodo.**
`dominio-psicologia.md` sitúa el solapamiento fuerte en dos operaciones: **operacionalizar** (escribir
el criterio antes de construir, C1) y **evaluar** (C2, C3b, C5, C7, C13). Las dos son capas de este
recorrido y las dos se hacen **sobre el mismo objeto**, que es la condición de que la evaluación
signifique algo: una batería de diez casos que se vuelve a pasar cinco veces sobre el mismo sistema es
un instrumento; diez casos distintos sobre doce sistemas distintos no son nada.
Y la mitad incómoda, que va escrita en el material: **su riesgo no es quedarse corta de rigor, es
pasarse** (`dominio-psicologia.md` §6). Un solo proceso es un imán para el perfeccionismo. La regla que
lo contiene es explícita y se repite: **el montaje se hace rápido y sucio; el rigor se gasta entero en
la evaluación.**

**(e) Porque un proceso vivo es la única evangelización que funciona, y ella pide exactamente eso.**
El objetivo 5 no es conseguir permiso: es **evidenciar valor** y **arrancar un proyecto de forma que la
organización lo adopte**. Lo que se adopta no es una idea ni un dossier: es una cosa que ya funciona,
que tiene un número reproducible detrás y que otra persona puede usar sin la autora delante. Este
ángulo es el único en el que el módulo de evangelización no tiene que fabricar su materia prima:
**la tiene desde la semana 4**. Los otros dos ángulos también llegan ahí; este llega con un objeto que
lleva tres meses en producción, que es una diferencia de credibilidad real.

**(f) Porque elimina la competencia por el tiempo, que es la primera causa documentada de abandono.**
Eriksson et al. titularon su estudio *«Time is the bottleneck»*: 21 de 34 abandonos mencionan el tiempo
[E]. La contramedida no es motivacional sino estructural: **que el trabajo del curso sea trabajo del
puesto**. Aquí la coincidencia es máxima, porque el objeto del curso es una tarea que ella tiene que
hacer igualmente. El material declara en cada sesión si es **tiempo propio** o **tiempo de trabajo**;
sin esa distinción escrita lo contabilizará todo como tiempo propio y el curso parecerá el doble de
caro de lo que es.

**(g) Porque el criterio portátil se puede extraer con un ritual, y un ritual es lo único que sobrevive
a un curso sin profesor.**
El brief pide que el criterio se extraiga «explícitamente al final de cada módulo con una pregunta
fija». Eso solo es posible si hay **algo concreto de lo que extraerlo**. Se puede preguntar «¿qué de
esto vale para cualquier proceso?» a alguien que acaba de construir una cosa; a alguien que acaba de
leer un panorama, no. La pregunta fija es el mecanismo, y este ángulo es el que le da objeto.

## 1.3 Cómo esta tesis cumple la corrección de brief sobre agnosticidad

No con una declaración. Con cuatro decisiones estructurales, todas comprobables:

| Decisión | Qué significa en la práctica |
|---|---|
| **Los módulos se titulan por capa, nunca por producto** | «Que ocurra sin que lo pidas», no «Acciones programadas». El índice del curso no caduca |
| **Criterio y clics viven en ficheros distintos** | `L3.1-capa.md` (sin fecha, sin nombres de producto) y `L3.1-clics-<entorno>.md` (fechado, reemplazable, uno por entorno). Ver §5 |
| **Cada capa cierra con la pregunta fija, y su segunda mitad es la herramienta** | *«¿Qué de esto valdría con cualquier herramienta, y qué era de esta?»* Contestada ocho veces, por escrito, por ella |
| **Una prueba de traslado real, no una promesa** | En M2, reconstruir la misma capa en otra herramienta con material verde y rellenar la ficha de qué viajó y qué hubo que rehacer |

Y el listón de admisión, aplicado párrafo a párrafo:

> **¿Le seguirá sirviendo dentro de dos o tres años?** Si no, o va al fichero de clics, o no entra.
> Nada por estar de moda. Y la prueba operativa que decide en qué mitad va una frase:
> **¿deja de ser cierta si mañana renombran un producto o si mañana trabaja con otro?** Si sí, está en
> la mitad equivocada.

**Lo único específico de su entorno que hay que resolver pronto** —qué plan de Gemini tiene contratada
la empresa y cómo está configurado— es tarea de M0, y hasta eso se enseña agnóstico: **las cuatro
preguntas que definen cualquier plan de cualquier proveedor** son criterio; la ruta para averiguarlas
en una consola concreta es clic.

## 1.4 Cómo esta tesis cumple la corrección de brief sobre evangelización

**Demostrar y arrastrar, no pedir permiso.** Su empresa empuja la IA con bastante desconocimiento de lo
que se puede hacer. No hay autorización que pedir: usar IA está bien visto y lo mal visto es no
automatizar. Lo que falta es **evidencia** y **una forma de arrancar que termine en adopción**.

Tres restricciones de diseño, y las tres son restricciones, no adornos:

1. **Va después de medir.** M7 consume el número de M5. Un número sin método es una promesa, y una
   promesa incumplida quema los tres proyectos siguientes.
2. **Es un módulo, no una lente.** El resto del curso no se reescribe «pensando en el público
   interno». Si la evangelización fuera la columna vertebral, el curso dejaría de ser sobre su trabajo
   y pasaría a ser sobre su reputación — que es exactamente el desvío del itinerario no técnico de la
   referencia, cuyo destino es un portfolio y una landing porque su alumno tipo quiere cambiar de
   sector. La nuestra no.
3. **Pero deja un hilo barato desde la semana 2:** tres líneas por capa en el **Cuaderno de
   evidencias**. Sin ese hilo, M7 tendría que reconstruir los números de memoria, que es lo mismo que
   inventarlos.

Y el enunciado del módulo, que es la frase que lo ordena entero:

> **Lo que hace que una organización adopte algo no es un argumento: es que la cosa siga funcionando
> la semana que tú no estás.**

## 1.5 Los dos riesgos de esta tesis, enunciados con las peores palabras posibles antes de defenderla

**Riesgo 1 — Si elige mal el proceso, el curso se resiente entero.**
No es un riesgo teórico. Su puesto tiene procesos que *parecen* el caso ideal de IA y son trampas: el
matching alumno-familia (P17) concentra salud, religión y potencialmente orientación sexual en una
casilla de texto libre; la hoja de camas (P22) tiene riesgo crítico de overbooking; las cartas de
visado (P08) dependen de normativa que cambia de un año para otro. Y en la semana 1 ella tiene **el
mínimo criterio que va a tener en todo el curso**, porque el criterio es justamente lo que el curso
enseña. La incoherencia es real y hay que mirarla de frente.

**Riesgo 2 — Un solo proceso puede no dar ocasión de practicar todo el criterio.**
Si su proceso no tiene un trozo determinista puro, nunca chocará con «esto no necesita IA». Si no
maneja datos rojos, la lección de datos se queda en abstracto. Si nunca hay un caso que deba pararse,
las condiciones de parada son teoría. Un curso monocultivo produce a alguien que sabe hacer **una**
cosa, que es exactamente lo contrario del objetivo 4.

## 1.6 LAS DOS SALVAGUARDAS

Ninguna es una advertencia. Las dos son mecanismos: si se quitan, el curso se rompe de forma visible,
que es la propiedad que define una salvaguarda de verdad.

---

### SALVAGUARDA A · La elección no es una apuesta: es una prueba con criterios de rechazo observables

Cuatro piezas, y ninguna requiere juicio experto que ella todavía no tiene.

**A1 · El embudo de noventa minutos (M0, días 2 y 3).**

| Paso | Duración | Qué hace | Por qué así |
|---|---|---|---|
| 1 | 20 min | Recibe la lista de los **32 procesos de `dominio-academia.md` ya escrita**. Tacha los que en su academia no ocurren o no lleva ella. Marca con un palote los que ha hecho **esta semana** | Reconocer es mucho más barato que recordar. Una hoja en blanco delante de alguien cansado produce ocho filas y abandono; una lista de 32 para corregir produce veinticinco filas en veinte minutos |
| 2 | 10 min | **Descarte por número, sin pensar:** fuera P08 (visados), P17 (matching), P22 (camas), P25 (reembolsos), P26 (quejas formales), P29 (emergencias). Y fuera todo lo estacional, con una regla de una línea: *«si no lo hago en enero, no vale»* | Es aritmética, no criterio. Los seis descartes vienen de `dominio-rgpd.md` §8.3 y `dominio-academia.md` §1.1, y protegen precisamente contra el riesgo 1. La regla estacional protege contra montar el curso sobre julio y practicarlo en enero |
| 3 | 20 min | Puntúa los 6–8 supervivientes en **cinco columnas observables** (abajo) | Ninguna columna admite «depende» |
| 4 | 40 min repartidos en 2 días | **La prueba de la sombra** (A2) | Es donde se cae la elección equivocada |
| 5 | 10 min | Nombra el **proceso de repuesto** (el segundo de la lista) y firma la fecha | El repuesto existe desde el día 3, no desde la crisis |

Las cinco columnas del paso 3, y las cinco son observables:

| Columna | +2 | 0 | −3 (descalifica) |
|---|---|---|---|
| ¿Cuántas veces esta semana? | 5 o más | 1–4 | 0 |
| Datos que toca (semáforo de `dominio-rgpd.md` §2.4) | solo verde | ámbar seudonimizable | **rojo irreducible** |
| Consecuencia del peor error | interna, se arregla | molesta a un cliente | **dinero, plazo legal o visado** |
| **Los ficheros que abro, ¿son míos o compartidos?** | **míos** | **una copia mía sirve** | **solo existe en un recurso compartido** |
| ¿Sé cómo se hace bien? | perfectamente | más o menos | depende de otra persona |

> **La cuarta columna es la aportación de diseño de este ángulo y no está en ninguna de las
> arquitecturas hermanas.** `dominio-herramientas.md` §1.2.h documenta [V] que la automatización nativa
> de su entorno **falla con unidades compartidas, carpetas compartidas y hojas con referencias
> externas**, y que el centro de gravedad de su puesto es exactamente eso: los buzones `info@` y
> `accommodation@` y la hoja de camas. En las otras arquitecturas ese límite aparece en el módulo 4 o 9
> y se gestiona como mala noticia. **Aquí entra en el criterio de elección, en la semana 1, y se cobra
> antes de que haya nada construido encima.** Es la diferencia entre descubrir el muro cuando cuesta
> diez minutos y descubrirlo cuando cuesta seis semanas.

**A2 · La prueba de la sombra (dos días laborables, tres minutos al día).**
Antes de comprometerse, durante dos días, **cada vez que ejecuta el proceso candidato anota tres
cosas**: cuántos minutos ha tardado, qué documento ha abierto, y qué decisión ha tomado que no estaba
escrita en ninguna parte.

Y tres criterios de rechazo, ninguno de opinión:

| Lo que ve en la hoja | Qué significa | Veredicto |
|---|---|---|
| **En dos días no lo ha ejecutado ni una vez** | No es tan frecuente como cree. La frecuencia percibida y la real no coinciden casi nunca | **Descartado.** Pasa al siguiente |
| **No ha abierto ningún documento** | No hay contexto que dar: es juicio puro. Un asistente con fuentes no tiene qué morder | **Descartado.** Este proceso es «chat mejor usado» y ahí se queda |
| **Las decisiones no escritas son cada vez distintas** | El proceso no es un proceso: es una serie de casos | **Descartado**, o se acota a un trozo que sí se repite |

Si sobrevive, el proceso **es el proceso**, y la hoja de sombra ya es la primera versión de la
descripción de la tarea que pide la capa 0. La prueba no cuesta tiempo extra: se hace mientras trabaja.

> **Nota metodológica que va en el material, porque es su casa.** Esto es muestreo de eventos, no
> introspección. `dominio-psicologia.md` C9: *la gente describe sus procedimientos como cree que
> deberían ser, no como los ejecuta*, y los atajos y excepciones —que son justo lo que rompe una
> automatización— no se verbalizan espontáneamente. Por eso no se pregunta: se observa. Y por eso el
> tercer campo, *«qué decisión he tomado que no estaba escrita»*, es el que más rinde: es el inventario
> de todo lo que un sistema no sabría hacer.

**A3 · El divorcio preautorizado, con el coste acotado por diseño.**
Al final de M1 hay un **checkpoint de divorcio**: cambiar de proceso es un movimiento legítimo,
escrito y firmado desde la semana 1. Y lo que hace que esto no sea un consuelo sino una salvaguarda es
la aritmética:

> **Al final de M1 lo único construido son la descripción del proceso, la línea de corte, la ficha de
> criterio y la batería de diez casos. Rehacer las cuatro cosas sobre el proceso de repuesto son
> aproximadamente dos horas, porque el método ya lo sabe y lo único que cambia es el contenido.**
> A partir de M2 el divorcio ya cuesta caro. Por eso el checkpoint está exactamente ahí y no después.

Es decir: **el diseño concentra el riesgo del ángulo en las primeras cuatro semanas y lo hace barato
justo mientras es probable.** Esa es la respuesta al riesgo 1, y es estructural, no motivacional.

**A4 · El expediente modelo.**
El curso trae el recorrido completo **ya hecho** sobre P27 (análisis de las encuestas de satisfacción):
las ocho capas, con sus artefactos, sus fallos típicos y sus claves selladas. No es un segundo hilo que
ella deba ejecutar —eso duplicaría el trabajo y este ángulo existe precisamente para no hacer doce
cosas a medias—: es **el ejemplo trabajado con desvanecimiento** (`dominio-autodidacta.md` §2.1 y
§5.4), la fuente de los cebos, y el **proceso de repuesto por defecto** si su elección se cae y no
tiene otra.

Por qué P27 y no otro: cuatro análisis independientes convergen. Riesgo **bajo** (no hay dinero, no hay
plazo legal, no lo ve ningún cliente), volumen **alto** (600–800 respuestas al año), es el proceso
**más multilingüe** de su lista (10+ idiomas), **hoy no se hace** porque nadie tiene tiempo, y es el que
**más solapa con su formación** (análisis de contenido, libro de códigos, estilos de respuesta
culturales). Que el proyecto más útil sea también el más seguro no es coincidencia buscada: es un
regalo del dominio.

*(El coste de que el expediente modelo sea lectura y no ejecución está reconocido en §14.3.)*

---

### SALVAGUARDA B · El Doblete: cada capa se repite en seco sobre un proceso que no es el suyo

**El mecanismo.** Al cerrar cada capa, **veinte minutos**, sobre papel, aplicando la misma capa a un
proceso distinto de su lista de 32. No se construye nada. Se contesta a cuatro preguntas y se firma un
veredicto.

```
DOBLETE de la capa __ · proceso: P__ · fecha: ____ · 20 minutos

1. Si tuviera que aplicar esta capa aquí, ¿qué haría exactamente? (3-5 líneas)
2. ¿Qué cambiaría respecto a lo que hice en mi proceso?
3. ¿Hay algo de esta capa que aquí NO tendría sentido? ¿Por qué?
4. VEREDICTO:  [ ] aplica igual   [ ] aplica con cambios   [ ] no aplica, y este es el motivo
```

**Y la regla que lo hace funcionar, que es una cuota y la defiendo como tal:**

> **De los ocho dobletes, al menos tres tienen que terminar en «no aplica» o en «aplica pero no
> compensa». Si tienes menos de tres, no has transferido: has repetido. Vuelve.**

La justificación no es estética. Cruzando los 32 procesos de `dominio-academia.md` con lo que la
plataforma puede hacer de verdad (`dominio-herramientas.md` §3.3), el reparto real da entre cinco y
siete «noes» por cada doce procesos. Tres de ocho es un suelo prudente, no una cuota inventada. Su
función psicológica es la que importa: **convierte el «no» en algo que hay que encontrar**, y desactiva
de raíz el sesgo que produce un curso de IA por su mera existencia — preguntarle a un curso de IA si
algo debe hacerse con IA tiene un sesgo obvio hacia el sí.

**Los ocho dobletes, asignados a propósito para que cada capa choque con un tipo distinto de «no»:**

| Capa | Doblete | Respuesta correcta, y qué enseña |
|---|---|---|
| 0 · Ver el proceso | **P29** emergencias 24 h | *No aplica.* Un proceso de riesgo crítico, no determinista y bajo presión no se mapea para delegarlo: se mapea para **no** delegarlo. Enseña que describir un proceso no compromete a automatizarlo |
| 1 · Criterio | **P02** presupuestos | *Aplica, y el resultado es que no hace falta IA.* Es aritmética sobre una tabla de precios. Escribir el criterio es lo que hace visible que el criterio se cumple con una fórmula. **Es el ejemplo canónico del escalón −1** |
| 2 · Contexto | **P08** carta de aceptación para visado | *No aplica*, y el motivo transferible no es «es difícil» sino **«la normativa cambia de un año para otro, y congelar dentro de un artefacto un conocimiento que caduca es fabricar un error futuro»** |
| 3 · Disparador | **P30** parte semanal a dirección académica | *Aplica igual, y con la mínima IA posible.* Determinista puro. Enseña que «automatizar» no significa «meter un modelo» |
| 4 · Juicio y frenos | **P28** respuesta a reseñas online | *Aplica con cambios:* clasificar y preparar sí, publicar **nunca** — y el motivo no es de calidad, es de RGPD: confirmar públicamente que alguien fue alumno y tuvo un problema ya es una cesión de datos |
| 5 · Medir | **P12** check-in del lunes | *No aplica limpiamente:* el valor de ese proceso es la percepción de calidad de toda la estancia, y eso no se mide en minutos por unidad. Enseña **deficiencia del criterio** (`dominio-psicologia.md` C2b) con un caso suyo |
| 6 · Que sobreviva sin ti | **P32** mantenimiento de plantillas y FAQ | *Aplica igual, y es el diagnóstico correcto de P32:* el problema no es que falte automatización, es que **falta una fuente de verdad**. Es un hallazgo que aportar, no un fracaso |
| 7 · Que lo adopten | **el proceso de una compañera**, elegido por ella | Es a la vez el último doblete y la primera semilla de contagio. Ver §6.3 |

**Por qué esto no es un parche.** Ocho dobletes × 20 minutos = **menos de tres horas** en dieciocho
semanas. Es barato, cabe en una micro-sesión, y produce ocho veredictos firmados sobre procesos que no
son el suyo. No sustituye a los treinta juicios que produce una arquitectura de inventario; **lo digo
en la autocrítica y no lo disimulo** (§14.2). Lo que sí hace, y una arquitectura de inventario no hace,
es que cada uno de esos ocho juicios se emita **inmediatamente después de haber hecho esa misma cosa de
verdad**, que es cuando un juicio sobre un proceso ajeno vale algo.

---

### LA PREGUNTA FIJA — el tercer mecanismo, que el brief pide por su nombre

Al cerrar cada capa, tres líneas escritas por ella, en su lenguaje, en el mismo fichero:

```
LA PREGUNTA FIJA — capa __ · fecha ____

1. PROCESO   Lo que he hecho aquí valdría para cualquier proceso en la parte de: __________
             Y era de ESTE proceso la parte de: __________
2. HERRAMIENTA  Valdría con cualquier herramienta la parte de: __________
             Y era de ESTA herramienta la parte de: __________
3. TECHO     Esta capa no puede: __________
             Y lo que lo rompería sería una cosa del tipo: __________
```

**La regla de las dos mitades, que es lo que la hace autocorregible:** cada respuesta tiene una mitad
positiva y una negativa, y **las dos son obligatorias**. Si escribe que todo vale para todo, no ha
separado nada: ha resumido. Si escribe que nada vale fuera de aquí, tampoco. La comprobación es
binaria y de cinco segundos: *¿están rellenas las seis casillas? SÍ/NO*.

Y el destino de las tres partes:

- La parte 1 alimenta el Doblete: lo que dice que vale para cualquier proceso es exactamente lo que va
  a probar veinte minutos después sobre otro.
- La parte 2 es el mecanismo de agnosticidad del curso, contestado ocho veces por escrito.
- La parte 3 construye la **Lista de techos**, que es cómo se cubre «saber qué existe» sin catálogo
  muerto (§8.1).

---

## 1.7 Lo que esta tesis rechaza, y por qué

| Alternativa | Por qué se rechaza |
|---|---|
| **Empezar por un recorrido de lo que existe** (chat, asistentes, cuadernos, flujos, agentes, MCP) | Es el catálogo muerto. Se lee cómodo, produce sensación de aprendizaje —que es un mal indicador [E, Deslauriers]— y a los diez días no queda nada porque no cuelga de nada suyo. Además es la mitad del material que caduca |
| **Ordenar el curso por la escalera de herramientas** (arquitectura 1) | Es un buen diseño y su propia autocrítica dice el problema: *«ordena el curso por autonomía de la herramienta, no por dificultad del criterio»*, con riesgo de producir tres tutoriales encadenados. Con el brief agnóstico corregido, ese riesgo sube, no baja |
| **Ordenar el curso por el inventario de su semana** (arquitectura 2) | Entrena la operación de clasificar más veces que este ángulo, y eso es una ventaja real. Su coste es el que su propia autocrítica admite: **un Semanario es un documento, y los documentos no contestan correos**. Cuatro semanas de mapa antes de tener algo que funcione es un riesgo de arranque grande en un curso sin profesor, y es donde peor duele |
| **El doble hilo de `dominio-autodidacta.md` §7.1** (uno guiado con clave + uno propio) | Es la recomendación del informe y la desoigo a propósito. Con dos horas propias por semana, ejecutar dos veces cada capa **es hacer dos cosas a medias**, que es literalmente lo que este ángulo existe para evitar. El sustituto es el expediente modelo como lectura con clave sellada más los cebos. **El coste está reconocido en §14.3** |
| **Seguir los cinco pasos de la referencia como columna vertebral** | Son correctos y se usan enteros —mis capas 0 y 1 son su paso 2, mi capa 2 es su paso 3, mi capa 4 es su paso 4 y mi capa 5 es su paso 5—, pero su orden asume cohorte, mentores, dos públicos y un alumno que quiere entrar en el sector de la IA |
| **Elegir el proceso más doloroso** | El más doloroso es el más complejo y el más arriesgado. En su puesto es el matching de alojamiento o la hoja de camas: categorías especiales del RGPD y riesgo crítico. El proceso más doloroso es el **segundo** proyecto, y eso va escrito |
| **Hacer el curso «multiherramienta» de verdad, montando todo dos veces** | Duplicaría la fricción y produciría competencia en ninguna. La agnosticidad se consigue con la pregunta fija, la separación física criterio/clics y **una** prueba de traslado acotada |

---

# 2. RESULTADOS DE APRENDIZAJE OBSERVABLES

Verbos de desempeño. Cada uno con su evidencia observable y el módulo donde se cierra. Ninguno dice
«entenderá», «conocerá» ni «será capaz de valorar».

| # | Al terminar, ella… | Evidencia observable | Cierra en |
|---|---|---|---|
| **RA1** | **Elige** un proceso propio para delegar aplicando criterios de rechazo observables, y **descarta** por escrito los que no pasan, con el motivo | Hoja de elección con 6–8 candidatos puntuados, los seis descartes por número tachados, y una hoja de sombra de dos días | M0 |
| **RA2** | **Describe** un proceso suyo como se ejecuta de verdad —disparador, documentos que abre, decisiones no escritas, salida— sin escribirlo de memoria | La descripción contiene **al menos dos decisiones que no estaban en su idea previa del proceso**. Si no las contiene, se hizo de memoria | M0 |
| **RA3** | **Determina** bajo qué régimen de datos trabaja: qué plan, qué licencia, qué retención, qué política escrita — **o documenta** a quién y cuándo lo preguntó | Ficha del entorno con las ocho casillas y **ninguna frase que empiece por «creo que»** | M0 |
| **RA4** | **Traza la línea de corte** de su proceso: qué trozos entrega y qué trozos se quedan con ella, con el motivo | Al menos un trozo se queda con ella y el motivo no es «es difícil» sino riesgo, caducidad del conocimiento o falta de fuente de verdad | M1 |
| **RA5** | **Escribe** el criterio de «resultado correcto» en 4–6 indicadores que otra persona pueda comprobar sí/no contra una fuente, **antes** de tocar ninguna herramienta | Ficha de criterio de una cara, sin *adecuado, correcto, natural, profesional, de calidad* sin ancla detrás | M1 |
| **RA6** | **Construye** una batería de diez casos —5 típicos, 3 límite, 2 de rechazo— con casos apartados **antes** de escribir el prompt, y **la vuelve a pasar con fecha** en cada capa | La Tira: una hoja con una columna por capa y fecha en cada columna, cinco columnas al terminar | M1 → M5 |
| **RA7** | **Sitúa** cada dato que atraviesa su proceso en verde/ámbar/rojo, **marca en qué punto del flujo entra y en cuál hay que quitarlo**, y **reescribe** un caso real que sobrevive a la prueba de la compañera | Mapa de datos del proceso, de una cara, más tres casos reescritos que **siguen produciendo una respuesta útil** y uno declarado no reescribible | M2 |
| **RA8** | **Monta** un asistente con fuentes propias que **cita el documento y su fecha** y que **responde «no lo sé»** a lo que está fuera de alcance | 5/5 en los típicos, pide aclaración en los 3 límite, «no lo sé» en los 2 de rechazo | M2 |
| **RA9** | **Reconstruye** una capa suya en una herramienta distinta y **nombra** qué viajó tal cual y qué hubo que rehacer | Ficha de traslado con las tres columnas rellenas con cosas concretas | M2 |
| **RA10** | **Monta** algo con disparador que **prepara, clasifica o avisa y nunca envía**, y **lo apaga habiéndolo probado** | Se dispara con cinco casos fabricados y produce las cinco salidas correctas; **un sexto caso que NO debe disparar** no dispara; la prueba de apagado está hecha, no imaginada | M3 |
| **RA11** | **Distingue** en su proceso qué parte tiene pasos fijos y qué parte necesita juicio, y **argumenta por qué un agente autónomo sería exceso aquí** | Media página con la frontera trazada y los dos puntos de juicio nombrados | M4 |
| **RA12** | **Escribe** la lista de temas prohibidos y las condiciones de parada de su propio sistema, y **las prueba con casos fabricados que deben parar** | Cinco casos de parada, cinco paradas. La respuesta a «quién revisa» es **una persona con nombre** | M4 |
| **RA13** | **Reconoce** cuál es el único proceso de su academia que caería en el Anexo III del Reglamento de IA y **a quién lo escala** | Una frase, un nombre, un puesto | M4 |
| **RA14** | **Audita a su propio corrector**: detecta los defectos plantados de un artefacto-cebo y **decide con ese dato** si la IA sirve para corregir ese tipo de trabajo | Hoja de resultado del cebo + decisión escrita + al menos un caso registrado en que **no** aceptó una crítica de la IA, con el motivo | M1, M4 |
| **RA15** | **Mide** el efecto de su sistema en minutos por unidad, **resta** revisión y mantenimiento y **nombra** una amenaza a la validez que no puede descartar | Media página de evaluación, sin la palabra «significativo», con la resta hecha | M5 |
| **RA16** | **Deja el sistema en condiciones de sobrevivirle**: fuentes con fecha y dueño, calendario de revisión, apagado probado y ficha de traspaso | La ficha de traspaso responde con nombre propio a «quién lo mantiene» y con fecha a «cuándo caduca cada fuente» | M6 |
| **RA17** | **Entrega** su artefacto a otra persona, que lo usa **una semana sin ella**, y **corrige** lo que ese piloto revele | Ficha de traspaso + resultado del piloto + **lista de al menos dos cosas que hubo que arreglar** | M7 |
| **RA18** | **Explica** en treinta segundos, sin nombrar ninguna herramienta, qué hace su sistema, qué ahorra y **qué no hace** | La prueba del pasillo, superada con alguien que no ha visto el artefacto | M7 |
| **RA19** | **Contesta la pregunta fija** al cerrar cada capa, con sus dos mitades, y **firma ocho dobletes** de los cuales **al menos tres son «no aplica»** | El cuaderno de capas: ocho preguntas fijas con las seis casillas rellenas y ocho dobletes con veredicto | todos |
| **RA20** | **Escribe la rúbrica** de un artefacto suyo, con ≥3 criterios negativos, y **la valida contra un cebo** | Si el cebo pasa su rúbrica, la rúbrica es blanda y se rehace | M6 |

**Criterio de «curso terminado», definido en la semana 1 y observable:**

> **Un proceso suyo funcionando y en uso diario sin que el curso se lo pida · un número medido con su
> método · ocho preguntas fijas contestadas con sus dos mitades · tres dobletes que terminaron en «no
> aplica» · una rúbrica escrita por ella · y una segunda persona que ha usado su sistema una semana
> entera sin ella delante.**

No es «leer la última lección». Y RA20 es el indicador honesto de que ya no necesita el material.

---

# 3. LOS CINCO INSTRUMENTOS PERMANENTES

Van antes del mapa de módulos porque todos los módulos cuelgan de ellos. Son cinco ficheros que viven
más allá de las dieciocho semanas.

## 3.1 El Expediente del proceso — el objeto que el curso transforma

Una carpeta con el nombre del proceso. **No es documentación: es el sitio donde el proceso vive.** Cada
capa deja dentro exactamente una cosa, y esa lista es el índice del curso:

```
expediente-<mi-proceso>/
  00-como-se-hace-de-verdad.md      ← capa 0: disparador, documentos, decisiones no escritas, salida
  00-hoja-de-sombra.md              ← capa 0: los dos días de observación, en crudo
  01-linea-de-corte.md              ← capa 1: qué entrego y qué se queda conmigo, con motivo
  01-ficha-de-criterio.md           ← capa 1: 4-6 indicadores observables, críticos marcados
  01-casos.md  +  01-CLAVE.md       ← capa 1: la batería, y su clave SELLADA
  02-mapa-de-datos.md               ← capa 2: qué dato entra, dónde, y dónde hay que quitarlo
  02-fuentes/                       ← capa 2: cada fuente con FECHA y DUEÑO en la primera línea
  03-disparador.md                  ← capa 3: qué lo lanza, con qué tope, cómo se apaga
  04-frenos.md                      ← capa 4: temas prohibidos, condiciones de parada, quién revisa
  05-evaluacion.md                  ← capa 5: antes, después, coste completo, amenaza no descartada
  06-traspaso.md                    ← capa 6: dueño, caducidades, calendario de revisión, apagado
  la-tira.md                        ← la batería pasada en cada capa, una columna por fecha
  cuaderno-de-capas.md              ← 8 preguntas fijas + 8 dobletes
  evidencias.md                     ← 3 líneas por capa, para M7
```

**Por qué una carpeta y no un documento.** Porque el entregable de este curso no es un informe: es un
sistema con partes que se tocan por separado y caducan a ritmos distintos. Y porque el día que otra
persona lo herede (M6, M7), lo que se entrega es esta carpeta y nada más.

**Regla de la primera línea, que aparece en la capa 2 y no se abandona nunca:** todo fichero de
`02-fuentes/` empieza con dos datos — **de cuándo es** y **quién manda sobre él**. Sin eso, un cuaderno
con las condiciones de cancelación del año pasado responde con las del año pasado, con toda la
confianza del mundo.

## 3.2 La Tira — la misma batería, capa a capa, con fecha

Diez casos escritos en M1 y **nunca cambiados**, pasados al terminar cada capa, en una hoja con una
columna nueva por capa. Al final tiene esta forma:

```
CASO                          | como lo hago hoy | +criterio | +fuentes | +disparador | +frenos
                              | 13-oct           | 27-oct    | 10-nov   | 24-nov      | 15-dic
------------------------------|------------------|-----------|----------|-------------|--------
T1  caso típico 1             |  SÍ              |   SÍ      |   SÍ     |    SÍ       |   SÍ
T2  caso típico 2             |  NO              |   SÍ      |   SÍ     |    SÍ       |   SÍ
...
L1  ambiguo: dos categorías   |  inventa         |  inventa  | pregunta |  pregunta   | pregunta
L2  queja educada indirecta   |  inventa         |  inventa  | inventa  |  pregunta   | pregunta
L3  vacío de contenido        |  inventa         | pregunta  | pregunta |  pregunta   | pregunta
R1  fuera de alcance          |  responde        | no lo sé  | no lo sé |  no lo sé   |  PARAR
R2  menciona salud            |  responde        | responde  | no lo sé |   PARAR     |  PARAR
                              |                  |           |          |             |
MINUTOS POR UNIDAD            |   14             |   11      |    6     |     4       |    4
QUIÉN LO DISPARA              |   yo             |   yo      |   yo     |  el suceso  | el suceso
```

**Y aquí está la lección central del curso, que no se cuenta: se lee en su propia hoja.**

> Entre la tercera y la quinta columna **la calidad de la respuesta apenas se mueve**. Casi toda la
> calidad se gana en la capa 1 y la capa 2 —cuando alguien escribe qué es hacerlo bien y le da fuentes
> con fecha— y a partir de ahí solo se puede perder. Lo que cambia al añadir capas no es la calidad:
> es **quién dispara, cuánto tarda y cuánta autonomía has cedido**.

Si dentro de tres años le ponen delante una herramienta que no existe hoy, la pregunta que sabrá hacer
es *«¿esto me cambia la calidad o me cambia el disparador?»*, que es la pregunta correcta. Y no se la
habrá contado nadie: la habrá deducido de cinco columnas de su propio trabajo.

**Dos reglas que la sostienen:**
1. **Los casos se escriben ANTES de construir nada** y con muestreo, no elegidos. Si se escriben
   después, se escriben para que pasen. Ella reconocerá la operación con su nombre: es preregistro.
2. **La clave va sellada** en un fichero aparte, escrito el mismo día, que no se reabre hasta anotar
   los resultados de cada pasada.

**El riesgo de este instrumento, dicho aquí:** es trabajo sin novedad, media hora cada tres semanas, y
las cosas sin novedad se convierten en ritual o desaparecen. La contramedida es que **el cierre de cada
módulo no está permitido sin la columna nueva**: es un ítem binario de la lista de comprobación, no un
consejo. Aun así, es el punto frágil que reconozco en §14.6.

## 3.3 El Cuaderno de capas — ocho preguntas fijas y ocho dobletes

Un fichero, ocho entradas de una cara. Cada entrada: la pregunta fija con sus seis casillas (§1.6) más
el doblete con su veredicto. **Es el curso entero en su lenguaje y sin nombres de producto.**

Su lista de comprobación es binaria y de diez segundos:

- ¿Están rellenas **las seis** casillas de la pregunta fija? SÍ/NO
- ¿Aparece algún nombre de producto fuera de la línea de techo? SÍ/NO
- ¿El techo dice algo que la capa **no puede hacer**, y no algo que ella todavía no sabe hacer? SÍ/NO
- ¿El doblete tiene veredicto firmado? SÍ/NO
- Al cerrar el curso: ¿hay **al menos tres** dobletes con veredicto «no aplica»? SÍ/NO

## 3.4 La Lista de techos — el catálogo, generado por el propio recorrido

No se lee: **se escribe**, una fila al cerrar cada capa, a partir de la parte 3 de la pregunta fija.
Tres columnas, y la tercera es la que convierte un catálogo en criterio:

| Lo que esta capa no puede hacer | La clase de cosa que sí podría | Qué tendría que cambiar para que me tocara |
|---|---|---|
| Un asistente guardado recuerda sus instrucciones, **no recuerda lo que pasó ayer** | Un sistema con memoria persistente y auditable | Que necesitara continuidad entre sesiones **y** pudiera comprobar qué recuerda. Hoy no puedo auditarlo, así que no me fío |
| Un disparador por horario **no reacciona a que haya pasado algo** | Un disparador por suceso | Nada: eso es la capa siguiente. *(Esta fila se tacha en la capa 3, y tacharla es el ejercicio)* |
| Mi automatización **no puede tocar los ficheros compartidos** de la academia | Herramientas de automatización externas, o un permiso delegado sobre el recurso compartido | Que alguien me delegue una etiqueta o una carpeta propia dentro del buzón compartido, **o** que el flujo tenga que tocar algo fuera de esta suite: entonces la siguiente parada es una plataforma de automatización externa |
| Un flujo con juicio **sigue siendo un camino que dibujé yo** | Un agente: le das el objetivo y los límites y él decide los pasos | Que aparezca una tarea cuyos pasos no pueda dibujar de antemano **y** que exista un plan que lo incluya **y** que los datos lo permitan. Hoy fallan las tres |
| Nada de lo mío **puede procesar decenas de ficheros locales de golpe** | Un agente con acceso al sistema de ficheros | Una tarea repetida del tipo «revisar 200 contratos de estancia larga buscando una cláusula» |

**Cuatro propiedades que hacen que esto no muera:**

1. **La tercera columna es la que no caduca.** Un catálogo dice qué hay; esta columna dice bajo qué
   condición cambiaría su decisión. «Tocar algo fuera de esta suite» seguirá siendo verdad cuando todo
   se llame de otra manera.
2. **Cada fila se escribe en el momento en que el proceso choca con el techo**, no en un módulo de
   panorama. La fila del agente se escribe en la capa 4, cuando ya tiene un flujo con juicio y entiende
   exactamente qué le falta.
3. **La escribe ella.** Un fichero copiado no se relee; uno escrito, sí.
4. **Tachar una fila es un ejercicio.** Cuando la capa siguiente rompe el techo anterior, se tacha con
   fecha. La lista se lee, al final, como el registro de por dónde ha ido subiendo.

## 3.5 El Cuaderno de evidencias — el hilo barato de la evangelización

Tres líneas al cerrar cada capa, el día que el artefacto empieza a funcionar. Coste: dos minutos.

```
CAPA __ · fecha ______
- Qué hacía yo antes, y cuántos minutos por unidad:
- Qué hace ahora, y cuántos minutos por unidad:
- Qué NO hace, y qué sigo haciendo yo:
```

Existe desde la semana 3 por una razón operativa, no ceremonial: **si M7 tuviera que fabricar las
pruebas al final, las inventaría.** Un número reconstruido de memoria en la semana 16 no es un número.
Y la tercera línea —*qué NO hace*— es la que después hace creíble a todo el dossier: quien enumera los
límites de su propio sistema se gana el derecho a que le crean el resto.

---

# 4. MAPA DE MÓDULOS

**Ocho módulos, 18 semanas, 2 h propias/semana** más el trabajo que es trabajo del puesto. Arranque en
**octubre**: el pico de junio–septiembre de la academia (250–400 correos/día) mata cualquier calendario
que lo ignore, y noviembre–febrero es su temporada baja.

**Una frontera declarada desde la semana 1, y esto es diseño anti-abandono, no una rebaja:**

> **Al terminar M4 (semana 11) ya hay curso:** un proceso suyo funcionando, en uso, con frenos y con
> apagado probado. **M5, M6 y M7 son donde se cobran los objetivos 4 y 5** —criterio portátil y
> evangelización— y son la parte que más rinde a doce meses vista. Decirlo así, y no fingir que las
> dieciocho semanas son un bloque indivisible, es lo que evita que la semana 12 se lea como fracaso.

Formato de cada ficha: **título · cambio mental · qué construye · duración realista · qué capacidad
entrena y cómo se enseña de forma transferible · cómo se autocorrige sin mentor · el doblete · la
pregunta fija**.

Estructura fija de módulo (heredada de `dominio-autodidacta.md` §5.3, y no se toca):
**3 sesiones núcleo de 35–45 min + 1 bloque de proyecto de 60–90 min en horario de trabajo + el cierre
de capa (pregunta fija + doblete + columna nueva de la Tira, 40 min).**

---

## M0 · Capa 0 — Ver el proceso, y elegir cuál (semanas 1–2)

**Cambio mental.** Tres, y el tercero es el que más cuesta.
*«Lo primero no es la IA: es mirar qué hago realmente.»*
*«Lo que creo que hago y lo que hago no son lo mismo, y la diferencia es exactamente lo que rompería una
automatización.»*
*«El mismo texto en la misma pantalla es seguro o inseguro según con qué cuenta haya entrado.»*

**Qué construye.**
1. **Día 1, 25 minutos: la primera victoria, dentro del proceso candidato.** Instrucciones permanentes
   guardadas —quién es, dónde trabaja, en qué idiomas escribe, qué tono usa, qué no debe hacer nunca— y
   usadas **hoy** sobre un correo real que tiene pendiente. Cronometrado antes y después. Sin instalar
   nada, sin pedir nada a nadie, sin hablar con nadie. **El mapa del curso va después de este resultado,
   nunca antes.**
2. **Días 2–3: el embudo de noventa minutos** (§1.6 A1) y **la prueba de la sombra** (§1.6 A2).
3. **`00-como-se-hace-de-verdad.md`**: el proceso descrito como se ejecuta —disparador, documentos que
   abre, decisiones que toma que no están escritas, salida y a dónde va—, escrito **a partir de la hoja
   de sombra**, no de memoria.
4. **La ficha del entorno**: qué plan, si su cuenta tiene licencia, qué retención, si hay política
   escrita — con los mensajes literales para copiar y pegar y las comprobaciones empíricas por si nadie
   contesta.
5. **La tarjeta del lunes** impresa al lado de la pantalla: el semáforo verde/ámbar/rojo.
6. **Proceso de repuesto nombrado y firmado.**

**Duración realista.** 2 semanas. **~2 h de tiempo propio** (25 min el día 1 + 90 min del embudo + 25
min de la ficha del entorno), más 3 min/día de sombra y el cronometraje, que **son tiempo de trabajo**.
El material lo declara así, línea a línea.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad: **mirar un proceso y describirlo como es**. Es la más portátil del curso y la que ella pide
con el nombre de «criterio portátil», y se enseña transferible por construcción:
- **Se describe por observación, no por introspección.** Muestreo de eventos, tres campos, dos días. Ese
  método vale para cualquier proceso de cualquier empresa en cualquier año, y no menciona ninguna
  tecnología.
- **Las cuatro preguntas que definen cualquier plan de cualquier proveedor** sustituyen a la tabla de
  planes: *¿entrenan con lo que escribo? ¿cuánto lo guardan y quién decide? ¿dónde se procesa? ¿hay
  contrato de encargado del tratamiento?* Más la quinta, que suele decidir de verdad: *¿alguien lo ha
  configurado y ha dejado dicho por escrito qué se puede meter?* Es el ejemplo más limpio del curso de
  criterio frente a clic, y va el primero a propósito.
- **El techo de la capa:** describir un proceso no lo mejora. Una descripción no contesta correos.

**Cómo se autocorrige.**
- **Ejecución real.** El correo del día 1 salió mejor y en menos tiempo, o no. Cronómetro, no opinión.
- **La prueba de la sombra tiene tres criterios de rechazo observables** (§1.6 A2). No hay nada que
  valorar: se mira la hoja.
- **La comprobación que más caza, y cuesta un minuto:** *¿tu descripción contiene al menos dos
  decisiones que no estaban en tu idea previa del proceso?* Si no las contiene, la escribiste de
  memoria y hay que volver a la sombra. Esta es la única forma sin mentor de detectar el error más
  caro de la capa.
- **La pantalla corrige el plan.** Las comprobaciones empíricas se corrigen solas, y enseñan de paso lo
  que necesitará cuando el material envejezca: **la documentación dice una cosa y la instancia dice
  otra, y manda la instancia.**
- **Rúbrica de la ficha del entorno, ocho casillas, con un estándar de suspenso brutal y muy útil:**
  *si en algún punto has escrito «creo que», «supongo que» o «me suena que», está mal resuelto.* «No lo
  sé y lo pregunté el día 14» sí vale. Distinguir lo que sabes de lo que supones es el mismo estándar
  que necesitará para evaluar respuestas de una IA, y por eso va el primero.

**Caja obligatoria «lo que vas a ver la primera vez».**
*«Vas a descubrir dos cosas incómodas. La primera: que este proceso lo haces menos veces de las que
crees, o más. La segunda: que en dos días has tomado tres o cuatro decisiones que no están escritas en
ningún sitio de la academia, y que solo sabes tú. Eso no es un fallo del ejercicio. Eso es el activo
del curso: es lo que ninguna herramienta puede darte hecho, y es la razón por la que este curso lo
puedes hacer tú y no un informático.»*

**Doblete (20 min): P29, emergencias 24 h.** Aplicar la capa 0 a un proceso que **no se va a delegar
nunca**. Veredicto correcto: describirlo sirve —para tener el protocolo escrito— pero no para
entregarlo. Enseña que mapear un proceso no compromete a automatizarlo, que es justo el reflejo que
hay que romper.

**Pregunta fija.** *Lo que vale para cualquier proceso: observar dos días en vez de recordar, y anotar
las decisiones no escritas. Lo que era de este: los tres documentos concretos que abro. Lo que vale con
cualquier herramienta: las cinco preguntas del régimen de datos. Lo que era de esta: dónde se mira el
distintivo. Techo: una descripción no hace el trabajo.*

**Punto de consulta PC-1** al final de la semana 2 (§7).

---

## M1 · Capa 1 — Qué es hacerlo bien, y qué trozos no entrego (semanas 3–4)

**Cambio mental.** Dos, y son los dos más caros del curso.
*«El cuello de botella no es el prompt: es que nadie ha escrito nunca qué cuenta como respuesta
correcta en esta tarea.»*
Y el segundo, que ella no tiene que creer por autoridad porque lo deduce de algo que sabe desde tercero
de carrera:

> **Un modelo de lenguaje es el instrumento con la validez aparente más alta y la garantía de validez
> de contenido más baja que vas a manejar en tu vida. Está optimizado para producir texto plausible: la
> plausibilidad es su función objetivo, no un efecto secundario.**

**Qué construye.**
1. **La línea de corte** (`01-linea-de-corte.md`): el proceso partido en trozos, y cada trozo con
   veredicto — *lo entrego · lo entrego con revisión mía antes de que salga · se queda conmigo*— y el
   motivo escrito. **Es el entregable más importante del módulo y el que la rúbrica protege más duro.**
2. **La ficha de criterio** (EP-01 de `dominio-psicologia.md`): definición en una frase, 4–6
   dimensiones, un indicador observable por dimensión, críticos marcados, punto de corte. **Una cara.**
3. **Las anclas de tono** (EP-02): tres frases completas —bajo, medio, alto— para dos dimensiones,
   sacadas de correos que envió de verdad. Ese fichero **es** el contexto de tono de la capa 2, no un
   calentamiento.
4. **Los diez apartados** (EP-06): diez casos reales sacados **por orden cronológico, no elegidos**, y
   cerrados antes de escribir una línea de instrucción.
5. **La Tira**, primera y segunda columna: la batería pasada contra cómo lo hace hoy, y contra la
   primera versión con criterio.

**Duración realista.** 2 semanas. Es el módulo más denso en trabajo mental y **el más ligero en clics
de todo el curso**: casi todo es un documento. Su sesión 1 empieza pasando la batería contra su forma
actual de trabajar y viendo que saca 4 de 10, para que la ficha de criterio nazca como respuesta a un
fallo observado y no como deberes previos.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad: **operacionalizar**. `dominio-psicologia.md` C1 la marca como transferencia FUERTE: es la
misma operación que hizo en la carrera, con otro objeto. Y hay un matiz que hay que dar en el mismo
párrafo porque le ahorra una pregunta: **aquí no estás estimando nada, estás decidiendo**. No hay
criterio verdadero que descubrir; hay criterio explícito y defendible, o no hay nada.
Transferibilidad: la ficha de criterio no menciona ninguna herramienta por construcción, y la batería
—5 típicos, 3 límite, 2 de rechazo, con tabla de especificaciones— es un instrumento que se pasa a
cualquier cosa que produzca texto.

**Cómo se autocorrige.**
- **Ctrl+F sobre la ficha de criterio.** Si aparecen «adecuado», «correcto», «natural», «profesional» o
  «de calidad» **sin un ancla detrás**, no ha operacionalizado: ha renombrado el constructo.
  Autocorrección mecánica perfecta, cinco segundos.
- **Prueba de tamaño:** la ficha cabe en una cara. Una rúbrica de dos páginas no se usa nunca.
- **Rúbrica de la línea de corte, con dos criterios negativos que deciden el módulo:**
  *(a) si no hay ningún trozo que se quede contigo, está mal resuelto — vuelve;*
  *(b) si el motivo de algún «se queda conmigo» es «es difícil», está mal: los motivos legítimos son
  riesgo, conocimiento que caduca, o que no existe una fuente de verdad que consultar.*
- **Los diez apartados se abren al final, y tiene que fallar al menos uno.** Si no falla ninguno,
  sospecha del muestreo antes que celebrar: *si tu batería la pasa entera a la primera, tu batería es
  fácil; no es que tu sistema sea bueno.*
- **Y el criterio no se toca.** Si al abrirlos le dan ganas de cambiar la ficha para que aprueben, **lo
  anota y no lo cambia**. Ese impulso es el dato más interesante del ejercicio y tiene nombre: sesgo
  del experimentador.
- **El primer cebo (control positivo).** El curso trae una **línea de corte de mentira**, de una
  academia inventada, con **tres defectos plantados y documentados** en un fichero sellado: uno visible
  (un trozo con datos rojos marcado como «lo entrego»), uno de omisión (falta el trozo de revisión
  humana antes de que algo salga), y uno de criterio (un trozo determinista clasificado como si
  necesitara un modelo). Ella lo corrige con la rúbrica y **después** abre la hoja de defectos. Si
  encuentra 1 o 0, **ese tipo de trabajo no se corrige con IA en el resto del curso**.
- **El protocolo de corrección con IA, siete reglas**, primera aplicación: hilo nuevo · no digas que es
  tuyo · nunca «¿está bien?» sino «enumera los incumplimientos de esta rúbrica y cita textualmente el
  fragmento que los incumple» · pega la rúbrica entera · **prohibido discutir en el mismo hilo** · dos
  modelos, y el desacuerdo es la señal, no el veredicto · su veredicto no cierra nada.

**Checkpoint de divorcio, al final del módulo.** Cambiar de proceso es legítimo y está preautorizado
desde la semana 1, y **cuesta unas dos horas** (§1.6 A3).

**Doblete (20 min): P02, presupuestos.** Escribir su ficha de criterio hace visible que todos los
indicadores se cumplen con una fórmula sobre la tabla de precios: número de semanas × tipo de curso ×
alojamiento × suplemento de julio-agosto × descuento por volumen. Veredicto: **aquí no hace falta IA**,
y meter un modelo de lenguaje no es ineficiente, **es introducir un error posible donde no lo había**.
Es el ejemplo canónico del escalón −1 y viene del árbol de decisión de la referencia, que corta en los
dos sentidos.

**Pregunta fija.** *Techo de la capa: un criterio escrito no produce respuestas; solo permite juzgarlas.*

---

## M2 · Capa 2 — Que sepa de dónde sale cada dato (semanas 5–6)

**Cambio mental.** *«La memoria fiable es un fichero, no una sensación.»* Y la tríada que los
principiantes mezclan siempre y que la referencia nombra bien: **fuente de verdad** (hechos, desde una
sola dirección) ≠ **memoria** (acuerdos que permanecen) ≠ **procedimiento** (pasos y formato).

**Qué construye.**
1. **El mapa de datos del proceso** (§9): cada dato que atraviesa el proceso, su color, en qué punto
   del flujo entra y en cuál hay que quitarlo. Una cara.
2. **Las fuentes**, con **fecha y dueño en la primera línea de cada una**. Para su proceso, las que
   toque: tarifario vigente, calendario académico, condiciones generales, protocolo de incidencias,
   FAQ. Tarifas, calendario y condiciones **no son datos personales**: se puede empezar en verde.
3. **El asistente v2**, que responde citando el documento y su fecha, y que **dice «no lo sé»** cuando
   la respuesta no está.
4. **La prueba de traslado** (§5.4).
5. **La Tira**, tercera columna.

**Duración realista.** 2 semanas.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad: **contexto con procedencia**. Tres piezas transferibles, ninguna con nombre de producto:
- **Citar no es un adorno: es lo que hace que revisar cueste cinco segundos en lugar de una
  investigación**, y por eso es lo que hace que la revisión se siga haciendo en julio.
- **«No lo sé» es una respuesta correcta, hay que exigirla explícitamente y hay que probarla a
  propósito.** Un sistema que nunca dice «no lo sé» no es que lo sepa todo: es que no lo has probado
  bien.
- **Una fuente sin fecha y sin dueño no es una fuente**, es un papel. El dueño es quien puede
  cambiarla; la fecha es lo que te dice si mirarla.

**Cómo se autocorrige.**
- **La batería, tercera columna.** Umbral: falla >0 de los 5 típicos → no está listo; se inventa una
  decisión en alguno de los 3 límite (aunque acierte) → no está listo; contesta algo distinto de «no lo
  sé» en alguno de los 2 de rechazo → no está listo.
- **Lista de comprobación binaria, diez ítems observables:** *¿cada fuente tiene fecha en la primera
  línea? ¿cada fuente tiene un nombre de persona como dueño? ¿alguna respuesta cita un documento que no
  está en las fuentes? ¿hay una frase que diga qué hacer cuando falta un dato? ¿he subido el maestro de
  algo, en vez de una copia?*
- **La prueba de la compañera**, sobre tres casos seudonimizados: *¿podría [nombre de una compañera
  concreta] saber de quién hablo leyendo esto?* Si sí, sigue quitando. Y el criterio del otro lado, que
  es el que casi nadie pone: **el prompt resultante tiene que seguir sirviendo**; si la respuesta que
  da es inservible, has quitado contexto que no era identificador.
- **PC-2 aquí** (§7): es el momento exacto en que pasa de pegar texto a subir ficheros, que es donde
  cambia el orden de magnitud del riesgo.

**Doblete (20 min): P08, carta de aceptación para visado.** Veredicto: **no aplica**, y el motivo
transferible es el que hay que saber decir: *«la normativa de extranjería cambia de un año para otro
—el Reglamento y sus instrucciones se reordenaron en 2025—, y congelar dentro de un artefacto un
conocimiento que caduca es fabricar un error futuro.»* Es el doblete que mejor entrena el criterio
portátil, porque **no metas conocimiento volátil dentro de un artefacto** vale para cualquier dominio.

**Pregunta fija.** *Techo de la capa: un asistente guardado recuerda sus instrucciones, no recuerda lo
que pasó ayer; y sigue esperando a que tú lo abras.*

---

## M3 · Capa 3 — Que ocurra sin que lo pidas (semanas 7–8)

**Cambio mental.** *«Automatizar no es una herramienta nueva: es quitar el dedo del disparador.»* Es el
momento psicológico del curso —la primera vez que algo pasa sin que ella lo pida— y por eso llega en la
semana 7 y no en la 14.

**Qué construye.** El trozo de su proceso que la línea de corte marcó como entregable, **con
disparador**. Y las tres piezas que lo convierten en un sistema y no en un juguete:
1. **El disparador**, con su tipo declarado (por horario o por suceso) y su justificación.
2. **El tope**: *si la lista supera N, no hagas nada y avísame.* Un sistema que genera cuarenta
   borradores un lunes de julio no ayuda, entorpece. **Enseñar a poner topes es enseñar diseño.**
3. **El apagado, probado de verdad**, no imaginado.

Y la regla que gobierna la capa entera y que va en negrita en el material:

> **Automatiza la lectura y la preparación. La escritura hacia fuera la firma una persona.**
>
> Y la razón, que no es prudencia sino diseño de aprendizaje: **si el artefacto solo prepara, todos sus
> errores son recuperables, y por eso puedes permitirte equivocarte mucho — que es exactamente lo que
> hace falta para aprender.** Un curso construido sobre artefactos que envían no puede permitírselo.

**Duración realista.** 2 semanas, y es el primer módulo con probabilidad real de desbordarse. Dos
sesiones de 45 min de tiempo propio más un bloque de proyecto de 90 min en horario de trabajo.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad: **disparador**. La transferencia es limpia porque la anatomía es universal: **hay
disparadores de calendario y disparadores de suceso, y la diferencia entre los dos es el techo del
módulo**. Un lunes no es un suceso; que entre un correo, sí. Eso será verdad en cualquier herramienta
durante años.
Y el segundo principio transferible, que decide entre herramientas de automatización en cualquier año:

> **Automatiza donde ya viven tus datos.** La que reutiliza lo que ya tienes gana a la más potente. Y
> la que mete a un proveedor nuevo entre tus datos y tú tiene que ganar por mucho para compensarlo —
> especialmente cuando esos datos incluyen pasaportes, alojamientos y menores.

**Los límites, por delante y no al tercer intento fallido.** En la primera página del módulo, no en una
fe de erratas: la automatización nativa de su entorno **falla con unidades compartidas, carpetas
compartidas y hojas con referencias externas** [V]; un solo disparador por flujo; tope de etiquetas
visibles. Como la cuarta columna del embudo de M0 ya descartó los procesos que solo viven en recursos
compartidos, aquí esto **no debería ser una sorpresa sino una confirmación** — y esa es exactamente la
función de haber puesto la restricción en el criterio de elección.

**Cómo se autocorrige.**
- **Se dispara o no se dispara.** El corrector más fiable que existe, y aquí está entero.
- **La prueba de los cinco casos fabricados**, uno por categoría, y **un sexto que NO debe disparar**,
  que es el que casi nadie prueba. Cinco salidas correctas y una no-salida, o no las hay.
- **La prueba de apagado.** Se apaga de verdad y se vuelve a encender. *Un sistema que no sabes apagar
  no está terminado.*
- **La prueba del tope:** meterle un lote grande a propósito y comprobar que se detiene.
- **Lista de comprobación de plataforma, seis ítems binarios**, escrita como síntomas y reutilizable
  como diagnóstico: *¿el fichero que toca está en una unidad compartida? ¿la hoja usa referencias
  externas? ¿tiene más de un disparador? ¿hay algún paso que escriba fuera? ¿lo he probado con un caso
  que debe NO disparar? ¿sé cómo se apaga y lo he apagado?*
- **La Tira, cuarta columna.** Y aquí la lectura correcta es la contraintuitiva y hay que darla escrita:
  *si la calidad ha mejorado respecto a la capa 2, sospecha: probablemente reescribiste el criterio por
  el camino, y eso es mérito tuyo, no del disparador.*
- **PC-4, el comodín**, disponible desde aquí.

**Doblete (20 min): P30, el parte semanal a dirección académica.** Determinista puro. Veredicto: aplica
igual, **con la mínima IA posible en el camino crítico**. Enseña que «automatizar» no significa «meter
un modelo», que es la confusión más extendida y la que más caro sale.

**Pregunta fija.** *Techo de la capa: un disparador por horario no reacciona a que haya pasado algo; y
un camino fijo se traga en silencio el caso que no previste.*

---

## M4 · Capa 4 — Juicio donde hace falta, frenos donde hace falta (semanas 9–11)

**Tres semanas, no dos.** Es el único módulo al que se le da aire antes del final, y se dice por qué:
es la frontera conceptual del curso y el punto donde más gente se cae.

**Cambio mental.** Dos.
*«Un agente no es una automatización mejor: es una automatización que **ha renunciado a ser
predecible** a cambio de poder afrontar casos que no previste. En atención al cliente esa renuncia se
paga a conciencia y solo donde compensa.»* Y la dirección del error que casi nadie enseña: **un agente
puede ser exceso.** Si los pasos son fijos, meterle juicio lo hace más caro, más lento y menos
auditable.
Y el segundo: *«el riesgo no es el del día 1, es el del día 60.»* Sesgo de automatización: a la tercera
semana se deja de revisar. **La confianza no es una salvaguarda.**

**Qué construye.**
1. **El juicio, confinado a dos o tres puntos concretos** de su proceso, cada uno con su criterio
   escrito y justificable.
2. **La lista de temas prohibidos** (`04-frenos.md`), en negativo y sin matices: *nunca respondas sobre
   requisitos o plazos de visado; nunca cites importes; nunca confirmes disponibilidad de alojamiento;
   nunca respondas a una queja formal; nunca menciones salud. Si el tema aparece, escribe SOLO: DERIVAR
   A PERSONA, y para.*
3. **Las condiciones de parada**: cliente enfadado, mención de abogado u hoja de reclamaciones, salud,
   menor implicado, importe por encima de X, o simplemente no encontrar la respuesta en sus fuentes.
4. **El punto de revisión humana, con nombre propio.**
5. **El plan para cuando falle**, en cinco pasos: detectar, parar, reparar con la persona (llamada, no
   correo), corregir el sistema añadiendo ese caso a la batería, y valorar si hay brecha de datos —
   **esto último no lo decide ella [!]**, lo escala el mismo día.
6. **La Tira**, quinta columna.

**Duración realista.** 3 semanas.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad: **juicio acotado y condiciones de parada**. Y aquí va la honestidad incómoda, dicha sin
disculparse porque es cierta y porque lo alcanzable es lo que se sostiene:

> **Su escalón 3 realista es «un proceso con juicio en dos o tres puntos», no «un agente autónomo que
> gestiona el buzón».** La barrera número uno no es técnica ni de capacidad suya: es **de licencia**
> —los agentes de verdad están detrás de planes que su empresa casi con seguridad no tiene [V]—, de
> **permisos** —un agente útil necesitaría el buzón compartido y la hoja de camas—, y de **datos** —sus
> procesos de más volumen mezclan salud, religión, menores y documentación de identidad—.

Lo transferible de la capa no depende de nada de eso: **la condición de parada es lo que separa un
asistente de un problema**, y se escribe igual en cualquier herramienta y en cualquier empresa. La
lección desarrollada de §12 es precisamente esta.

**Cómo se autocorrige.**
- **Cinco casos de parada fabricados que DEBEN parar.** Si alguno no para, no está listo. Comprobación
  pura, cero rúbrica.
- **Rúbrica con criterios negativos y salida escrita obligatoria** (sin «no aplica»): la lista de temas
  prohibidos incluye **importes, plazos de visado, disponibilidad y salud aunque su proceso no los
  toque hoy** —los sistemas se expanden solos y la lista se escribe para el sistema de dentro de seis
  meses—; la respuesta a «quién revisa antes de que salga» es **una persona con nombre**, no «se
  revisa»; y **ninguna salida llega a un cliente sin que alguien le dé a enviar** — si su diseño lo
  permite, vuelve al principio.
- **Verdadero/falso de doce ítems** sobre el marco de datos (E-05 de `dominio-rgpd.md`), autocorrección
  instantánea. Menos de 10 aciertos → releer.
- **Segundo cebo**, ahora sobre una lista de frenos: cierra el ciclo de control positivo y detecta si su
  corrector se ha degradado en dos meses.
- **PC-5 al final del módulo** (§7).

**Doblete (20 min): P28, respuesta a reseñas online.** Veredicto: **aplica con cambios** — clasificar y
preparar sí, publicar **nunca**. Y el motivo no es de calidad, es de RGPD: confirmar públicamente que
alguien fue alumno y tuvo un problema **ya es una cesión de datos**. Es el doblete que mejor enseña que
un freno puede venir de un sitio que no es la calidad del texto.

**Pregunta fija.** *Techo de la capa: un flujo con juicio sigue siendo un camino que dibujé yo; y sigue
sin decirme si esto sirve para algo.*

---

## M5 · Capa 5 — Medirlo sin engañarme (semanas 12–13)

**Cambio mental.** *«Que el sistema se ejecute cada lunes no es que sirva. Puede ejecutarse
impecablemente y no cambiar nada, porque el informe que produce no lo lee nadie o porque los borradores
se reescriben siempre.»* **Evaluación de proceso ≠ evaluación de resultado.**

**Qué construye.**
1. **Media página de evaluación, con fecha**: el número antes (de la hoja de sombra de M0, medida
   **antes** de construir nada, que es lo que la hace honesta), el número después, el **coste completo**
   —montaje + revisión + mantenimiento—, **cuál de las seis amenazas a la validez interna podría
   explicar el resultado** y qué mediría para descartarla.
2. **La prueba ciega** (EP-08, «el ejercicio con mejor relación valor/esfuerzo del curso»): cinco
   respuestas suyas de hace meses y diez salidas del sistema sobre casos comparables, sin marcas de
   origen, **barajadas por otra persona**, puntuadas con la ficha de criterio de M1.
3. **La cadena causal en cinco flechas** (EP-14), con el eslabón que no depende de ella subrayado.
4. **La lectura completa de la Tira**: una frase escrita por columna diciendo qué aportó esa capa. Si
   no puede escribir esa frase para alguna columna, esa capa no le aportó nada, y merece la pena
   saberlo.

**Duración realista.** 2 semanas. La prueba ciega es una tarde.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad: **medir si sirve**. Es la más portátil de todas y la que ningún curso de IA da, porque es
metodología y no producto. Se enseña con su vocabulario **declarando el préstamo**: *«en el mundo de la
IA a la batería la llaman evals o tests de regresión; el nombre psicométrico —ítems ancla— dice mejor
para qué sirven, que es hacer comparables dos momentos distintos.»*

**Herramienta y por qué: una hoja de cálculo, un cronómetro y una persona que baraje.** Deliberado: **la
evaluación no se hace con la herramienta evaluada.** Pedirle a un modelo que juzgue lo que él mismo
produjo acumula dos sesgos documentados —preferencia por lo verboso y auto-preferencia— que apuntan al
mismo desastre: aprobar por construcción.

**Cómo se autocorrige.**
- **La prueba ciega es autocorrección en estado puro.** No hay rúbrica que discutir: o acierta
  identificando cuáles eran suyas, o no; o ganan las suyas, o no. Y el patrón que aparece casi siempre
  —el sistema empata o gana en las dimensiones no críticas y pierde en la exactitud del dato— **le dice
  exactamente dónde poner la revisión humana**, que es la decisión que el curso entero perseguía.
- **Prohibiciones de vocabulario como comprobación mecánica.** Si aparece «significativo», está mal:
  aquí no se estima un parámetro poblacional, se comprueba la cobertura de un instrumento contra un
  criterio fijado. Si la medida es «horas a la semana» en vez de **minutos por unidad**, está mal: es
  lo único que sobrevive a que su volumen se multiplique por tres entre febrero y julio.
- **La resta obligatoria.** Si no ha restado revisión y mantenimiento, está mal. Y si el saldo es
  negativo y aun así quiere conservarlo por otra razón —menos errores, menos carga mental, respuesta
  más rápida al cliente—, **que lo diga y mida esa otra razón**: es legítimo, pero entonces el ahorro de
  tiempo no era el objetivo.
- **Una amenaza que no puede descartar, nombrada obligatoriamente.** Un pre-post de un solo grupo nunca
  las descarta todas, y decirlo es lo que separa un dato de un argumento comercial. Las seis, traducidas
  a su caso: historia (septiembre no es julio), maduración (ella misma ha mejorado en la tarea),
  regresión a la media (eligió lo que más dolía, y lo que más duele suele medirse en su peor semana),
  instrumentación, reactividad de la medida (la semana que se cronometra se trabaja más rápido — y este
  juega **a favor**: el ahorro real es mayor que el medido) y atrición (si deja de usarlo los días de
  agobio, la muestra final son los días tranquilos).
- El único favor humano del módulo —**barajar**— son cinco minutos y **no consume punto de consulta**:
  vale cualquier compañera.

**Caja obligatoria «lo que vas a ver la primera vez».** *«Es posible que el ahorro sea menor de lo que
esperabas. Si eso pasa, es un resultado del curso, no un fracaso tuyo — y es exactamente el tipo de
resultado que casi nadie publica. Antes de decidir nada, comprueba las dos cosas que casi siempre lo
explican: que estés midiendo por unidad y no por semana, y que hayas contado el tiempo de revisión en el
lado correcto de la resta.»*

**Doblete (20 min): P12, el check-in del lunes.** Veredicto: **no aplica limpiamente.** El valor de ese
proceso es que fija la percepción de calidad de toda la estancia, y eso no se mide en minutos por
unidad. Es **deficiencia del criterio** (`dominio-psicologia.md` C2b) con un caso de su casa, y enseña
la vacuna contra la métrica de vanidad mejor que cualquier explicación.

**Pregunta fija.** *Techo de la capa: medir dice si sirve hoy, no si seguirá sirviendo cuando cambie el
tarifario ni cuando yo no esté.*

---

## M6 · Capa 6 — Que sobreviva sin ti (semanas 14–15)

**Cambio mental.** *«Un sistema sin dueño y sin fecha se degrada. Y cuando se degrada, el recuerdo que
queda en la empresa no es “faltaba mantenimiento”: es “aquello de la IA no funcionaba”.»*

**Qué construye.**
1. **La ficha de traspaso** (`06-traspaso.md`): qué fuente caduca y cada cuánto · **quién la revisa, con
   nombre** · qué batería se vuelve a pasar cuando se toque algo · cómo se apaga, probado · y qué hacer
   el día que falle.
2. **El calendario de revisión**, con la próxima fecha escrita: cuándo se vuelve a pasar la Tira, cuándo
   se revisan las fuentes, cuándo se revisa la Lista de techos.
3. **La rúbrica escrita por ella**, con al menos tres criterios negativos, sin usar la del curso — y
   **validada contra un cebo**: si el cebo pasa su rúbrica, su rúbrica es blanda y se rehace.
4. **El apéndice del escalón 4**, marcado como opcional y como lectura (§10.2).

**Duración realista.** 2 semanas, con aire.

**Qué capacidad entrena y cómo se enseña transferible.**
Capacidad: **hacer que un artefacto sobreviva a su autora**. Es puramente organizativa, no tiene nada
de tecnológica y es la que más vale dentro de tres años y en otra empresa. Las tres preguntas que la
componen valen para cualquier cosa que alguien monte en cualquier sitio: *¿qué de esto caduca y cada
cuánto? ¿quién es la persona que lo mira? ¿cómo se apaga?*

**Cómo se autocorrige.**
- **La validación de su rúbrica contra un cebo** es un control positivo aplicado al instrumento que ella
  misma acaba de fabricar, y **es el criterio honesto de que ha terminado el curso**: cuando escribe las
  rúbricas, ya no lo necesita.
- **Lista binaria de la ficha de traspaso:** *¿hay un nombre de persona en «quién lo mantiene»? ¿hay una
  fecha en cada fuente? ¿hay una fecha en «próxima revisión»? ¿está probado el apagado? ¿alguien que no
  sea yo podría encontrar la carpeta?*
- **La prueba del hueco:** dejar el sistema una semana sin tocarlo y comprobar qué se ha desactualizado.
  Es barata y es la única forma de ver la degradación antes de que la vea un cliente.

**Doblete (20 min): P32, mantenimiento de plantillas y FAQ.** Veredicto: **aplica igual**, y el
diagnóstico correcto es que ahí el problema no es que falte automatización, sino que **falta una fuente
de verdad**: se actualiza la versión española del tarifario y las otras cinco se quedan viejas durante
meses. Es el riesgo «alto y silencioso» del inventario. Y es un hallazgo **que aportar**, no un fracaso:
en una empresa donde lo mal visto es no automatizar, llegar diciendo *«esto todavía no se puede
automatizar porque no sabemos cuál es el tarifario vigente en alemán»* es trabajo de valor. Va derecho
al dossier de M7.

**Pregunta fija.** *Techo de la capa: un sistema puede estar impecablemente mantenido y no usarlo nadie
más que yo.*

---

## M7 · Capa 7 — Que lo adopten: evidenciar y contagiar (semanas 16–18)

**El módulo adicional que el brief reincorpora.** Desarrollado entero en §6.

**Cambio mental.** *«Un artefacto que solo funciona conmigo delante no es un sistema de la academia: es
una manía mía. Lo que hace que otros lo adopten no es convencerles: es que puedan usarlo sin mí, y que
yo pueda enseñar el número y decir también qué no hace.»*

**Qué construye.** El **dossier de una cara** · la **demo de tres minutos** guionizada y cronometrada ·
**la semana sin ella** (el piloto) · la **conversación del proceso de otra persona** · y la **lista de
lo que decidió no automatizar**, que es la pieza que le da credibilidad a todo lo demás.

**Duración realista. 3 semanas**, y es el único módulo con una espera que no depende de ella: el piloto
dura una semana natural y no se puede acelerar.

**Cómo se autocorrige.** El piloto **es** la corrección, y es binario. Ver §6.4, que es donde este
módulo se juega su credibilidad como diseño.

**Doblete (20 min): el proceso de una compañera.** Es a la vez el octavo doblete y la primera semilla de
contagio: veinte minutos aplicando **solo la capa 0** al proceso de otra persona, en voz alta, sin
construir nada. Ver §6.3, punto 7.

**Pregunta fija.** La última, y se contesta sobre el curso entero.

---

## 4.1 Vista de conjunto

| M | Semanas | Capa | Qué sale del expediente | Escalón del perfil | Corrección dominante |
|---|---|---|---|---|---|
| M0 | 1–2 | 0 · Ver el proceso | Descripción real + hoja de sombra + ficha del entorno + primera victoria | 1 · chat | Cronómetro + tres rechazos observables + la pantalla |
| M1 | 3–4 | 1 · Criterio y línea de corte | Línea de corte + ficha de criterio + anclas + batería + clave sellada | 1 · chat | Ctrl+F + muestra apartada + primer cebo |
| M2 | 5–6 | 2 · Contexto con procedencia | Mapa de datos + fuentes fechadas + asistente que cita y se abstiene | 1 · chat | Batería (col. 3) + lista binaria + prueba de la compañera |
| M3 | 7–8 | 3 · Disparador | Disparador + tope + apagado probado | 2 · automatización | Se dispara o no + el caso que NO debe disparar |
| M4 | 9–11 | 4 · Juicio y frenos | Temas prohibidos + condiciones de parada + revisor con nombre + plan de fallo | 3 · agentes | Cinco paradas fabricadas + rúbrica negativa + segundo cebo |
| M5 | 12–13 | 5 · Medir | Evaluación de media página + prueba ciega + lectura de la Tira | transversal | La prueba ciega |
| M6 | 14–15 | 6 · Sobrevivir sin ti | Ficha de traspaso + calendario + rúbrica propia validada | transversal | Su rúbrica contra un cebo |
| M7 | 16–18 | 7 · Que lo adopten | Dossier + demo + **la semana sin ella** + lista de noes | **adicional** | **El piloto** |
| — | — | apéndice | *(lectura opcional: qué hay más arriba)* | 4 · opcional | ninguna |

**Herramientas nuevas en 18 semanas: dos o tres**, según lo que su proceso pida —un asistente con
fuentes, un disparador, y en algunos casos una aplicación en lote— y ninguna se introduce antes de que
el proceso se haya quedado corto sin ella. **Coste: cero euros.** Si el curso acaba costando dinero, el
diagnóstico estaba mal.
