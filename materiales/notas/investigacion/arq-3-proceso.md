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

---

# 5. LA SEPARACIÓN CRITERIO / CLICS, EN LA PRÁCTICA

No es una recomendación de estilo. Es la convención de producción del material, y si se relaja, el
curso deja de ser agnóstico en tres módulos.

## 5.1 La convención de maquetación: separación física, no dos apartados

Dos apartados dentro de la misma lección son insuficientes por tres motivos: se mezclan al escribir, no
se pueden sustituir en bloque cuando el producto cambia, y no se pueden duplicar por herramienta. La
convención es **separación física en ficheros**, y en este ángulo hay una tercera pieza que las
arquitecturas hermanas no tienen, porque aquí el criterio portátil se extrae con un ritual y el ritual
necesita su propio sitio:

```
curso/
  M3/
    M3.1-capa.md              ← EL CRITERIO. Sin fecha. Sin nombres de producto. Sin capturas
    M3.1-ejercicio.md         ← EL EJERCICIO. Tampoco nombra productos
    M3.1-rubrica.md
    M3.1-solucion.md
    M3-cierre.md              ← LA PREGUNTA FIJA + EL DOBLETE. Nunca nombra productos
    clics/
      M3.1-clics-<entorno-actual>.md   ← fechado, reemplazable, el que usa hoy
      M3.1-clics-<otro-entorno>.md     ← fechado, para la prueba de traslado
  comun/
    datos-volatiles.md        ← TODO número: cupos, límites, precios, qué edición incluye qué
    tres-nombres.md           ← la tabla de equivalencias de nombres. La única página que caduca entera
    cuando-no-coincide.md     ← el procedimiento para cuando el manual y la pantalla discrepan
    protocolo-ia.md           ← las siete reglas de corrección con IA
    expediente-modelo/        ← el recorrido completo hecho sobre P27, con claves selladas y cebos
```

**Cinco reglas de producción, todas mecánicamente comprobables:**

1. **Ningún nombre de producto en un fichero de criterio, de ejercicio o de cierre.** Comprobación real,
   no aspiracional: un `grep -iE` con la lista de productos sobre esos ficheros tiene que devolver
   **cero líneas**. Si devuelve alguna, esa frase va a clics o se reescribe.
2. **Ningún número volátil fuera de `datos-volatiles.md`.** Cupos, límites, precios y qué edición
   incluye qué se referencian, no se copian. Actualizar el curso es actualizar un fichero, no treinta.
3. **Ningún ejercicio puede depender de una captura de pantalla ni de una ruta de menú.** El enunciado
   describe qué se busca («el sitio donde se guardan las instrucciones de este asistente»); la captura
   solo ilustra. Si la captura envejece, el ejercicio sigue haciéndose.
4. **Todo fichero de clics abre con la misma cabecera, sin excepción:**
   > *Verificado el 22 de agosto de 2026 en `<entorno>`. **Si algo no coincide con lo que ves, tu
   > pantalla tiene razón y este texto no.** Ve a `cuando-no-coincide.md`.*
5. **Todo fichero de clics termina con la misma línea:** *«Si esto ha cambiado, lo que sigue siendo
   verdad está en `M3.1-capa.md`.»* Es lo que impide que un cambio de producto se lea como que el curso
   ha caducado.

**Y `cuando-no-coincide.md`**, media página escrita una vez y referenciada desde todos los ficheros de
clics, convierte la caducidad del material de defecto en **competencia enseñada**: buscar el nombre
nuevo en las novedades del proveedor, comprobar si es restricción de plan o de administrador,
preguntarle a la propia IA cómo se llama ahora eso y dónde está, y —solo si nada de eso funciona— el
comodín PC-4. Eso es exactamente lo que va a necesitar alguien que seguirá usando estas herramientas
cinco años después de terminar el curso.

## 5.2 Las dos reglas de redacción que deciden en qué mitad va una frase

La primera es la de siempre y la comparto con la arquitectura 2 porque es correcta:

> **¿Esta frase deja de ser cierta si mañana renombran un producto, o si mañana ella trabaja con otra
> herramienta?** Si sí → clics. Si no → criterio.

Las dos siguientes son de este documento, y son más fáciles de aplicar a las tres de la mañana:

> **La regla del sujeto.** En un fichero de criterio, **el sujeto gramatical de cada frase es el
> proceso, el dato o ella**. Nunca un producto. *«El proceso necesita saber de qué documento sale cada
> dato»* es criterio. *«El asistente admite diez ficheros»* es clic, porque el sujeto es la herramienta.
> Es una comprobación de tres segundos y la puede hacer cualquiera que no haya escrito el curso.

> **La prueba del sustituto.** Sustituye cada nombre de producto por «la herramienta» y relee el
> párrafo. Si deja de tener sentido, el párrafo pertenece a clics. Si sigue teniendo sentido,
> **entonces borra el nombre del producto para siempre**: no hacía falta. Esta segunda mitad es la que
> de verdad limpia el texto, porque el fallo típico no es escribir un párrafo de clics en la mitad de
> criterio: es dejar nombres de producto decorativos en frases que no los necesitaban.

Ejemplos de la conversión, tomados del material real de este curso:

| No se escribe | Se escribe |
|---|---|
| «Crea un Gem» | «Guarda este asistente con nombre, para poder reabrirlo sin volver a explicar el contexto» |
| «Sube el tarifario al cuaderno» | «Dale como fuentes los documentos sobre los que quieres que responda, y exige que cite de cuál sale cada dato» |
| «Workspace Studio no admite unidades compartidas» | «Comprueba, antes de diseñar nada, sobre qué ficheros puede actuar tu herramienta de automatización: casi todas tienen restricciones con recursos compartidos» *(y el límite concreto, en clics)* |
| «Usa la función de IA de la hoja de cálculo» | «Aplica tu criterio a las seiscientas filas de golpe, sin copiar y pegar» |
| «Pon una acción programada semanal» | «Elige qué lo dispara: una fecha del calendario o un suceso. La diferencia decide qué casos vas a poder atender» |

## 5.3 La tabla de tres nombres

Vive en `comun/tres-nombres.md`, es **la única página del curso donde conviven nombres de producto**, y
su función no es enseñar productos: es **desactivar el miedo del principiante a quedarse casado con una
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

> **Nota fija al pie, y es la que hace el trabajo:** *«Esta tabla es la única página del curso que
> caduca por completo. Está fechada. Cuando algún nombre no coincida con tu pantalla, corrígelo tú: es
> tuya. Lo que no cambia es la columna de la izquierda.»*

## 5.4 La prueba de traslado (M2, 25 minutos, tiempo propio)

La agnosticidad no se declara: se ejecuta una vez, y con restricción de datos.

> **Reconstruye el mismo asistente en otra herramienta** —ella ya usa ChatGPT por su cuenta— **usando
> solo material verde**: tarifario, calendario y condiciones generales, que no son datos personales.
> Pásale las mismas diez preguntas de tu batería. Y rellena la ficha:
>
> | Qué viajó tal cual | Qué hubo que rehacer | Qué techo cambió |
> |---|---|---|
> | La ficha de criterio · las fuentes con su fecha y su dueño · la batería de diez casos · la regla de «no lo sé» · la línea de corte | Dónde se guarda · cómo se llama · cuántos ficheros admite · dónde se pega la instrucción | Cuántas fuentes acepta · si cita el fragmento o solo el fichero · si conserva la instrucción entre sesiones |
>
> **Lo que se aprende no es «la otra herramienta también sirve». Es que el ochenta por ciento de tu
> trabajo era el criterio y las fuentes, y eso no estaba dentro de ninguna herramienta.**
>
> **Restricción de datos, y es contenido, no prudencia decorativa:** la prueba se hace **con material
> verde exclusivamente**. Su cuenta personal no tiene contrato de encargado del tratamiento y por ahí no
> pasa ni un dato de un alumno. Que la prueba de traslado sea también un ejercicio de semáforo no es
> casualidad: es el diseño.

**Se corrige sola:** o las tres columnas están rellenas con cosas concretas, o no lo están. Y hay un
criterio negativo: *si la columna «qué viajó tal cual» está vacía, no construiste criterio: construiste
un prompt.*

## 5.5 EJEMPLO REAL DE LAS DOS MITADES DE UNA MISMA LECCIÓN

Se elige **M3.1, «Que ocurra sin que lo pidas»**, porque es la lección donde la tentación de escribir un
manual de producto es máxima —es, literalmente, ir a un sitio y pulsar un botón— y porque es la primera
en la que algo del curso deja de depender de ella.

---

### `M3/M3.1-capa.md` — **EL CRITERIO** *(sin fecha, sin nombres de producto, sin capturas)*

> ## Para qué sirve esto en tu proceso
>
> Hasta ahora, tu proceso funciona **cuando tú te acuerdas**. Esa dependencia tiene dos costes que no se
> ven: los días de mucho trabajo —que son justo cuando más falta hace— es el primer sitio donde se cae;
> y no se puede repartir, porque «acordarse» no se delega. Esta capa quita tu dedo de en medio.
>
> ## Qué es un disparador, y por qué es la decisión y no un detalle
>
> Un disparador es **la condición que hace que el trabajo empiece sin ti**. Solo hay dos clases, y la
> diferencia entre ellas decide qué casos vas a poder atender:
>
> - **Por calendario.** «Cada lunes a las nueve.» Sirve cuando el trabajo se acumula y se puede tratar
>   en lotes: un resumen, un recordatorio, una comprobación periódica. Es el más fácil de razonar,
>   porque siempre sabes cuándo va a ocurrir.
> - **Por suceso.** «Cuando entra algo que cumple X.» Sirve cuando la respuesta tiene que llegar cerca
>   del hecho: un correo que hay que clasificar, un formulario que se acaba de enviar. Es más útil y es
>   más difícil de razonar, porque **no sabes cuántas veces va a ocurrir**.
>
> **Un lunes no es un suceso.** Si tu proceso empieza porque llegó algo, un disparador de calendario te
> obliga a esperar, y esa espera puede ser exactamente lo que hacía valioso el proceso.
>
> ## Las tres cosas sin las cuales un disparador no está terminado
>
> **1. Un tope.** Todo disparador tiene que tener un número por encima del cual **no hace nada y te
> avisa**. La regla, y es la que hay que recordar: *un sistema que produce cuarenta borradores un lunes
> de julio no ayuda, entorpece.* El tope no es una precaución: es lo que convierte una automatización en
> algo de lo que te puedes fiar, porque su comportamiento en el peor día es conocido.
>
> **2. Un apagado que hayas probado.** No que sepas que existe: que lo hayas apagado y vuelto a
> encender. **Un sistema que no sabes apagar no está terminado.** Y hay una razón práctica además de
> la obvia: el día que falle vas a estar nerviosa, y no es el momento de averiguar dónde está el botón.
>
> **3. Una salida que prepara, no que envía.** Esta es la regla que atraviesa el curso entero:
>
> > **Automatiza la lectura y la preparación. La escritura hacia fuera la firma una persona.**
>
> Y el motivo que hay que entender, porque no es prudencia: **si tu sistema solo prepara, todos sus
> errores son recuperables.** Etiquetar es reversible; enviar no. Eso te permite equivocarte mucho, que
> es exactamente lo que hace falta para que esto mejore. Se puede relajar más adelante, proceso a
> proceso y con datos de acierto medidos. **No se relaja por costumbre.**
>
> ## Cuándo NO poner un disparador
>
> - **Si todavía no usas el artefacto por tu cuenta.** Es la comprobación más importante de esta capa:
>   si en la última semana no lo has abierto sin que el curso te lo pidiera, el artefacto no te sirve
>   todavía, y **automatizar algo que no funciona es multiplicar el error**. Vuelve a la capa anterior.
> - **Si el proceso ocurre menos de una vez por semana.** El coste de montar y mantener el disparador no
>   se recupera. Hazlo a mano y ponte un recordatorio.
> - **Si la salida tiene que salir hacia fuera sin que nadie la mire.** Entonces el problema no es el
>   disparador: es que ese trozo no debería estar en la parte entregable de tu línea de corte.
>
> ## El techo de esta capa
>
> Un disparador hace que el trabajo empiece solo, **pero el camino sigue siendo el que dibujaste tú**.
> El caso que no previste sale mal, y sale mal **en silencio**, que es lo peor. Eso es lo que pide la
> capa siguiente.
>
> ## Los clics
>
> → `clics/M3.1-clics-<tu-entorno>.md`

---

### `M3/clics/M3.1-clics-<entorno-actual>.md` — **LOS CLICS** *(fechado y reemplazable)*

> *Verificado el 22 de agosto de 2026 en el entorno de trabajo actual. **Si algo no coincide con lo que
> ves, tu pantalla tiene razón y este texto no.** Ve a `cuando-no-coincide.md`.*
>
> **A · Disparador por calendario, sin salir del chat que ya usas.**
> 1. En la aplicación de chat de tu cuenta de trabajo, busca la sección de acciones programadas.
> 2. Escribe la instrucción como si se la dieras a alguien un lunes por la mañana, y fija la frecuencia.
> 3. Límite de acciones activas a la vez: ver `comun/datos-volatiles.md`.
>
> **B · Disparador por suceso, con la herramienta de automatización de la suite.**
> 1. Entra en la web de automatización de la suite con la cuenta de trabajo. Si no te deja entrar, no es
>    un fallo tuyo: tu administrador no la ha activado. Ver `cuando-no-coincide.md`.
> 2. Elige el disparador de la lista (llega un correo que cumple un criterio · llega una respuesta de
>    formulario · se edita un fichero · a una hora fijada).
> 3. Añade los pasos. El paso que llama a tu asistente se llama hoy «preguntar a un asistente»; el que
>    consulta tu cuaderno de fuentes, «preguntar al cuaderno».
> 4. La salida: **borrador en tu bandeja**, o fila en una hoja, o aviso. **No hay ningún paso de esta
>    lección que envíe nada a un cliente.**
>
> **C · Los límites que te vas a encontrar, hoy, en este entorno** *(y por eso la cuarta columna del
> embudo de la semana 1 descartó los procesos que solo viven en recursos compartidos)*:
> - los flujos **fallan con unidades compartidas, carpetas compartidas y hojas con referencias
>   externas**: los ficheros tienen que ser tuyos;
> - **un solo disparador por flujo**;
> - la interfaz solo muestra un número limitado de etiquetas del correo;
> - tu administrador **puede tener pasos desactivados** y no hay forma de saberlo hasta que lo intentas.
>
> **D · Dónde se apaga.** En la misma pantalla donde se crea, hay un interruptor de activo/inactivo.
> **Apágalo y vuelve a encenderlo ahora mismo**, antes de seguir: es el ejercicio, no un consejo.
>
> **Cifras y límites** → `comun/datos-volatiles.md`. *No las copies aquí.*
> *Si esto ha cambiado, lo que sigue siendo verdad está en `M3.1-capa.md`.*

---

**Qué demuestra este ejemplo, y por qué lo he elegido:** la mitad de criterio ocupa el doble que la de
clics, **no menciona ni una vez el nombre de ningún producto**, y seguiría siendo válida palabra por
palabra si mañana su empresa cambiara de proveedor. La mitad de clics es sustituible en veinte minutos
por alguien que no haya escrito el curso. Ese es el criterio de calidad de toda la maquetación. Y
nótese el detalle del apartado C: **el límite de plataforma está en clics, pero la instrucción de
comprobarlo antes de diseñar está en criterio**. Esa es la costura correcta.

## 5.6 Qué se pierde con esta convención, dicho aquí

Dos cosas, y conviene no fingir que salen gratis:

- **La lección se lee peor de corrido.** Saltar entre dos ficheros tiene un coste de atención real. La
  mitigación es que el fichero de clics sea corto, numerado y siempre en el mismo sitio, y que la
  lección termine con un enlace único. No lo elimina.
- **Redactar en capacidades es más lento y más abstracto**, y la abstracción es exactamente lo que peor
  le sienta a alguien sin base técnica en las primeras semanas. La compensación es que el ejercicio y la
  rúbrica viven en la mitad que no caduca, así que el mantenimiento del curso baja de treinta ficheros a
  diez. Y si el material resultara demasiado abstracto, **la reparación correcta no es volver a
  mezclar: es engordar los ficheros de clics y adelgazar el criterio.**

---

# 6. EL MÓDULO DE EVANGELIZACIÓN INTERNA (M7)

## 6.1 Qué NO es, dicho primero porque es donde se estropea

- **No es conseguir el sí.** No hay autorización que pedir. En su empresa usar IA ya está bien visto y
  lo mal visto es no automatizar. Un módulo de venta interna resolvería un problema que ella no tiene y
  le robaría tres semanas a los que sí tiene.
- **No es marketing personal.** Nada de portfolio, nada de landing, nada de «mira lo que tengo ahora en
  mi CV». Ese es el destino del itinerario no técnico de la referencia porque su alumno tipo quiere
  cambiar de sector. La nuestra no quiere cambiar de rol ni de sector — aunque sí quiere que lo
  aprendido le sirva si algún día cambia de empresa, y de eso se encarga la portabilidad del criterio,
  no un portfolio.
- **No es la columna vertebral.** Son tres semanas al final, alimentadas por tres líneas por capa. Si
  fuera la lente del curso entero, el curso dejaría de ser sobre su trabajo y pasaría a ser sobre su
  reputación, y **el criterio se contaminaría**: elegiría lo vistoso sobre lo útil, que es exactamente
  el error del grafo de la referencia.
- **No es evangelizar una idea.** El objeto de la adopción no es «deberíamos usar IA»: es **una cosa
  concreta que ya funciona y que otra persona puede usar**.

## 6.2 Qué es: el enunciado del módulo

> **Demostrar y arrastrar.** Su empresa empuja la IA sin saber bien qué se puede hacer. Lo que cambia esa
> situación no es un argumento: es **una cosa que funciona, un número que se puede reproducir, y una
> segunda persona que la usa sin ella delante.** Este módulo produce esas tres cosas.

Y el principio que lo ordena entero, que es el mismo que atraviesa el curso:

> **La credibilidad se compra con los noes.** Quien llega diciendo *«estas cuatro cosas NO deberían
> automatizarse, y aquí está por qué»* consigue que le crean sobre la quinta. Quien llega diciendo que
> todo se puede automatizar consigue que no le crean sobre nada — y esa es, exactamente, la posición en
> la que su empresa está hoy respecto a la IA.

**Y la ventaja específica de este ángulo, que es su mejor argumento:** el módulo no tiene que fabricar
su materia prima. Llega con un sistema que lleva tres meses en producción sobre su mesa, con una Tira de
cinco columnas fechadas, con un número medido contra una línea base tomada **antes** de construir nada,
y con una lista de noes razonados. Eso no es una demo: es un historial.

## 6.3 Qué enseña — siete piezas, todas con artefacto

**(1) El número y su método, que van juntos o no va ninguno.**
De M5 sale un ahorro en minutos por unidad, con el coste de revisión restado y con una amenaza a la
validez que no se puede descartar. **Las tres cosas se presentan juntas.** Un número sin método es una
promesa, y una promesa que no se cumple quema los tres proyectos siguientes. Aquí su formación es una
ventaja competitiva directa y hay que decírselo así: casi nadie que presenta resultados de IA en una
empresa sabe decir *«esto podría explicarse también porque septiembre no es julio»*, y decirlo es
precisamente lo que hace que se crean el resto.

**(2) Lo que el artefacto NO hace.** Es la tercera línea del Cuaderno de evidencias, y en el dossier va
en su propio apartado, no en letra pequeña. Doble función: es honestidad, y es **gestión de expectativas
operativa** — si el dossier dice «no responde nada sobre visados y para en cuanto aparece la palabra»,
la primera pregunta incómoda ya está contestada antes de que la hagan.

**(3) La demo de tres minutos.** No una presentación: **un antes y un después con un caso real, y un
número.** Aquí la lección de la referencia se aplica invertida: su grafo era espectacular en pantalla y
marginal en valor, y además —lo dijo ella misma— *estaba hecho para el agente, no para el humano*. Lo
que se enseña aquí es aburrido y sirve: la pantalla de antes y la de después, con el reloj al lado.
Guion escrito y cronometrado.

**(4) La prueba del pasillo.** Explicar qué hace, qué ahorra y **qué no hace**, en treinta segundos y
**sin nombrar ninguna herramienta**. Regla de vocabulario dura: se nombra el resultado, no la
tecnología. No *«monté un flujo con un paso de extracción que llama a mi cuaderno de fuentes»*, sino
*«los correos de admisiones llegan ya clasificados y con un borrador hecho, y me ahorra unos ocho
minutos por correo; los de visado no los toca, los deja para mí»*. Esta regla es además la vacuna
contra el efecto que más daño hace a un evangelizador interno: **sonar a que ha descubierto una
religión**.

**(5) LA SEMANA SIN ELLA — el corazón del módulo.**
Una compañera usa el artefacto **cinco días laborables, sin ella delante**. No una demostración
acompañada: uso real, sola.

Es el único test verdadero de adopción y produce siempre el mismo hallazgo, que es lo que lo hace
valioso: **una parte del artefacto era ella.** Instrucciones implícitas, decisiones que tomaba sin darse
cuenta, un fichero que solo ella sabe dónde está, un criterio que nunca escribió porque le parecía
obvio. Lo que el piloto revela es exactamente lo que hay que arreglar para que la cosa sobreviva a sus
vacaciones — **y sobrevivir a sus vacaciones es literalmente la definición operativa de que la
organización lo ha adoptado**, en un negocio donde agosto vacía la oficina y julio la desborda.

El entregable del piloto **no es «salió bien»**: es la **lista de lo que hubo que arreglar**, y tiene
que tener al menos dos entradas. *Si el piloto no reveló nada, no fue un piloto: estuviste mirando por
encima del hombro.*

**(6) La ficha de traspaso**, que viene ya hecha de M6 y aquí se entrega de verdad: qué fuente caduca y
cada cuánto · quién la revisa, **con nombre** · qué batería se vuelve a pasar cuando se toque algo ·
cómo se apaga, probado. Es lo que convierte «una cosa que hizo ella» en «una cosa que tiene la
academia». Y es también protección propia: un artefacto sin dueño y sin fecha se degrada, y cuando se
degrada el recuerdo que queda no es «faltaba mantenimiento», es «aquello de la IA no funcionaba».

**(7) La conversación del proceso de otra persona** — la semilla de contagio, y a la vez el octavo
doblete.
Veinte minutos con una compañera, aplicando **solo la capa 0** a un proceso de ella: qué lo dispara, qué
documentos abre, qué decisiones toma que no están escritas, qué sale y a dónde va. **No se construye
nada y no se promete nada.** Se escribe la descripción en una página y se le devuelve para que la
corrija.

Por qué esto es lo que contagia y una presentación no:
- **Es la técnica que ella ya sabe hacer y que un perfil técnico no puede aportar** (`dominio-psicologia.md`
  C9): entrevista semiestructurada, estructura de embudo, preguntar por el último caso concreto y no
  por la norma, preguntar por la excepción, y devolver el procedimiento escrito para que lo corrijan —
  porque corrigiendo se saca más que preguntando.
- **El encuadre que funciona no es «quiero automatizar tu tarea»** —eso pone a cualquiera a la
  defensiva— **sino «quiero aprender a hacerlo yo bien para no molestarte cada vez»**. Y es verdad,
  además, que es la mejor manera de conseguirlo.
- Y produce el efecto que ningún dossier produce: la otra persona ve su propio proceso escrito por
  primera vez. **Ahí es donde alguien pide algo.**

**Y las cuatro reglas de arranque, todas derivadas de lo que el curso ya ha hecho:**

| Regla | Por qué |
|---|---|
| **Empieza por un proceso que no sea de nadie** | Un proyecto que mejora la tarea de una compañera empieza con una persona a la defensiva; uno que hace lo que nadie hacía empieza con cero resistencia. **La elección del primer proceso es el 80 % de su adopción**, y por eso el embudo de M0 no era solo una cuestión de riesgo |
| **Enseña el resultado, no el proceso** | La primera vez se enseña lo que sale, no cómo se hizo. El «cómo» se cuenta cuando alguien lo pide, que es la señal de que ya hay adopción |
| **Ofrece el trabajo, no la herramienta** | *«Te paso el resumen de las incidencias de alojamiento de este mes»* gana siempre a *«te enseño a montar un clasificador»* |
| **Deja que lo pidan** | La segunda persona no se recluta: aparece cuando ve el primer resultado. **Si a las tres semanas nadie ha pedido nada, el artefacto no era tan útil como parecía — y eso también es un resultado del curso**, no un fracaso personal |

## 6.4 Cómo se autocorrige sin mentor — el punto donde este módulo se juega su credibilidad

Es el módulo más difícil de autocorregir de los ocho, porque su criterio de éxito es **la conducta de
otras personas**, que ella no controla. Decirlo es obligatorio. Y aun así hay cinco mecanismos, cuatro
de ellos comprobaciones y no juicios:

1. **El piloto es el corrector, y es binario.** Otra persona lo usó cinco días laborables sin ella, o no
   lo usó. Se cuenta. Y el entregable es la lista de arreglos, con al menos dos entradas. Ese es el
   criterio negativo del módulo.
2. **La reproducción del número.** Dos semanas después, con la ficha de método delante, vuelve a
   calcular el ahorro. **Si no sale el mismo número ±10 %, el número no era reproducible y el dossier se
   reescribe.** Es un test-retest de su propio instrumento y no necesita a nadie.
3. **La prueba del pasillo, cronometrada.** Treinta segundos, a alguien que no ha visto el artefacto.
   Comprobaciones binarias: *¿nombré alguna herramienta? ¿la otra persona pudo repetirme qué hace? ¿dije
   un número? ¿dije qué NO hace?*
4. **Rúbrica del dossier, con criterios negativos y salida escrita obligatoria** (sin «no aplica»):
   - *Hay en el dossier un número cuyo método no puedo reproducir delante de alguien.* ☐
   - *Hay una afirmación que no podría defender si alguien la comprobara la semana que viene.* ☐
   - *El apartado «qué NO hace» está vacío o dice generalidades.* ☐
   - *La respuesta a «quién lo mantiene» no es una persona con nombre.* ☐
   - *No hay ninguna forma de apagarlo, o la hay pero no la he probado.* ☐
   - *Presento como resultado del sistema algo que en realidad hago yo a mano después.* ☐
5. **PC-6** (§7): la prueba del pasillo con alguien que sabe de IA y **no conoce la academia** es el
   evaluador ideal para detectar las dos cosas que ella no puede ver desde dentro: **jerga** y
   **sobreafirmación**.

**Y lo que este módulo NO puede corregir, escrito para que no se disimule:** si su compañera no usa el
artefacto, hay al menos cuatro explicaciones —el artefacto es malo, la compañera está desbordada, la
tarea no era suya, no hubo tiempo— y el material no le da forma de distinguirlas. Lo único que puede
hacer es **registrar cuál cree que es y por qué**, y volver a intentarlo con otra persona o con otro
momento del año. Es el único punto del curso donde una alumna diligente puede hacerlo todo bien y salir
sin saber si lo hizo bien. Ver §14.1.

## 6.5 Dónde va y por qué exactamente ahí

| Alternativa | Por qué no |
|---|---|
| Al principio, como encuadre motivador | No hay nada que enseñar todavía. Y arranca el curso con la mirada puesta en lo que piensen los demás, que es exactamente el desvío que el brief prohíbe |
| Repartido por todos los módulos | Convertiría cada capa en una pieza de comunicación y contaminaría el criterio: se elegiría lo vistoso sobre lo útil |
| Después de M4, cuando el sistema ya funciona | Tentador, porque ahí ya hay algo que enseñar. Pero **no hay número**, y un dossier sin número medido es una opinión con formato de informe |
| **Al final, después de medir y después de dejarlo mantenible** ← **la elegida** | Consume la salida de M5 **y** la de M6. No se evangeliza lo que no está medido, y no se traspasa lo que no tiene dueño ni fecha. Además llega en el momento en que el material solo ya no tira: el único incentivo disponible en la semana 16 es que **alguien de fuera use lo que has hecho**, y ese es precisamente el contenido del módulo |
| Al final, pero sin hilo previo | El Cuaderno de evidencias existe desde la semana 3 justamente porque, sin él, M7 tendría que reconstruir números de memoria — es decir, inventarlos |

## 6.6 Qué produce, en una lista

1. **Un dossier de una cara**: qué hace · qué ahorra y con qué método se midió · **qué no hace** · quién
   lo mantiene · cómo se apaga.
2. **Un guion de demo de tres minutos**, cronometrado, con un antes y un después reales.
3. **La semana sin ella, ejecutada**, y su lista de arreglos.
4. **Una descripción del proceso de otra persona**, escrita por ella y corregida por su dueña.
5. **La lista de lo que decidió no automatizar**, con el motivo — heredada de la línea de corte de M1 y
   de los ocho dobletes, y actualizada.
6. **Una nota de media página** para quien lleve la política de uso de IA, si en M0 resultó que no
   existe ninguna. No es venta: es cerrar el hueco que ella misma detectó en la semana 1, y es el
   hallazgo con mejor relación valor/esfuerzo de todo el curso.

---

# 7. LOS PUNTOS DE CONSULTA CON SU PAREJA

## 7.1 El principio, antes de la lista

El recurso es **escaso, no renovable y con coste relacional**. Un mentor pagado se gasta sin culpa; una
pareja, no. Y un curso que convierta a la pareja en su soporte técnico dañaría dos cosas a la vez: la
relación y la autonomía que el curso persigue.

**Presupuesto: seis consultas de diez minutos en todo el curso** — una hora repartida en cuatro meses.
Un curso que reserve «consultas ilimitadas» obtiene en la práctica **cero**, porque cada consulta compite
con la comodidad de no molestar y pierde. Un curso que reserve exactamente seis, con nombre y momento,
obtiene seis.

**Filtro de admisión, impreso en la portada del cuaderno.** Si falla cualquiera de las cuatro, no es
punto de consulta: (1) ¿lo resuelve el material? (2) ¿lo resuelve la IA con el protocolo de siete
reglas? (3) ¿lo resuelve **mirar** —su pantalla, su consola, preguntar a su administrador—? (4) ¿lo he
intentado veinticinco minutos y he anotado lo que he probado?

**Ficha de cinco campos, escrita ANTES, máximo una cara:** la pregunta en una frase **cerrada** · mi
hipótesis y qué esperaría ver si tengo razón · qué he probado ya y qué pasó · **el dato concreto**
(mensaje de error literal, las dos respuestas que se contradicen) · qué haré con cada respuesta posible.

**Cuatro reglas de la conversación:** los cinco primeros minutos **sin pantalla** · **él no toca el
ratón** · sale con una frase escrita en su propio lenguaje dentro de la hora siguiente · **a los diez
minutos se para, esté como esté**.

## 7.2 Dónde caen, y por qué exactamente ahí

| # | Momento | Qué lleva | Por qué ahí y no en otro sitio |
|---|---|---|---|
| **PC-1** | **Fin de M0** (sem. 2) | *«He deducido que tenemos el plan X, que por eso no puedo hacer Y, y que por eso he descartado estos tres procesos y elegido este. ¿El razonamiento se sostiene?»* Con las comprobaciones empíricas hechas y la hoja de sombra delante | **Es el punto de mayor consecuencia de este ángulo entero**, porque todo lo demás se construye encima. Y está formulado con precisión para lo que él sí puede auditar: **el razonamiento y los hechos de plataforma**, no los hechos de la academia, que no conoce. Un error aquí contamina dieciocho semanas; diez minutos aquí es la mejor relación consecuencia/coste del curso |
| **PC-2** | **Inicio de M2** (sem. 5), justo antes de cargar fuentes reales | Su clasificación de **ocho tipos de dato reales** de su puesto en tres cajones: cuenta de empresa / nunca / depende. Y tres casos ya seudonimizados, con la pregunta *«¿tú sabrías de quién hablo?»* | **Es la única decisión del curso con consecuencia externa irreversible**, y el momento es exacto: es cuando pasa de pegar texto a subir ficheros, que es donde cambia el orden de magnitud del riesgo. Y para la prueba de la compañera hace falta, por definición, **una mirada de fuera** que ella no puede tener sobre su propio material |
| **PC-3** | **Fin de M1** (sem. 4), tras el primer cebo | *«Esta es la corrección que me hizo la IA de un trabajo con tres fallos plantados. Encontró dos. ¿Estoy leyendo bien lo que se le escapa?»* | **El de mayor apalancamiento.** No se revisa su trabajo: se revisa **su instrumento de corrección**, que va a usar cincuenta veces más. Diez minutos aquí valen por todas las correcciones posteriores |
| **PC-4** | **Comodín**, disponible desde M3 | Un fallo de plataforma tras agotar la lista de seis comprobaciones y la página «cuando no coincide» | Caso canónico de «diez minutos ahorran una tarde». **No tiene fecha a propósito**: saber que existe un comodín reduce el miedo a atascarse, que es un factor de abandono por sí mismo, aunque no llegue a usarse |
| **PC-5** | **Fin de M4** (sem. 11) | *«Esta es la línea de corte con la que he terminado, y estos son los tres sitios donde dudé. ¿Dónde la moverías?»* | Juicio de escala y oportunidad: preguntarle a un modelo si algo debe automatizarse tiene un sesgo obvio hacia el sí, así que aquí el modelo no sirve. Y requiere que ya tenga el sistema funcionando: antes no hay sustancia sobre la que conversar. Cae además exactamente en la frontera de abandono (§11, momento 3) |
| **PC-6** | **M7** (sem. 17) | La prueba del pasillo, en treinta segundos, y después: *«¿qué he dicho que no podría defender si alguien lo comprobara?»* | Alguien que sabe de IA y **no conoce la academia** es el evaluador ideal para las dos cosas que ella no puede ver desde dentro: **jerga** y **sobreafirmación**. Y cierra el curso con otra persona, que evita el final en el vacío |

**Un uso de otra persona que NO gasta punto:** barajar las respuestas de la prueba ciega de M5 y guardar
la clave. Es una función mecánica de cinco minutos, no una consulta, y vale cualquier compañera de la
academia.

## 7.3 Lo que deliberadamente NO es punto de consulta

Revisar un entregable (*«¿está bien mi asistente?»* → rúbrica y batería), explicar un concepto (*«¿qué es
MCP?»* → material), enseñarle a hacer algo (→ documentación), o dar ánimos genéricos. Y la tentación
específica de esta configuración: **que él le monte algo «que es un momento»**. Eso no es una consulta:
es un artefacto que ella no sabrá mantener ni depurar, y en la capa siguiente será deuda. En un curso
cuyo entregable es **un sistema que tiene que sobrevivirle a ella**, un trozo que no entiende es
literalmente el peor regalo posible.

## 7.4 Las alternativas degradadas

El material no puede tener un paso bloqueante que dependa de otra persona, o reproduce el peor defecto
del curso de referencia (la mitad de su valor estaba en la cohorte). Cada punto lleva la suya escrita
justo debajo:

- **PC-1** → asumir el escenario más restrictivo, elegir el proceso con la puntuación más alta que no
  dependa de ninguna función dudosa, y anotar la suposición como pendiente de confirmar.
- **PC-2** → regla de máxima cautela: **si dudas, no lo metes**, y lo anotas. Y la prueba de la
  compañera se hace con **cualquier compañera de la academia**, que además es la evaluadora literal del
  criterio («¿sabrías de quién hablo?»).
- **PC-3** → hacer el cebo dos veces con dos modelos distintos y comparar; el desacuerdo entre modelos
  es un sustituto pobre pero real del juicio externo.
- **PC-4** → documentar el fallo, **rodearlo** con una solución manual y seguir. Un curso no puede
  pararse por un botón que alguien movió.
- **PC-5** → la lista de descalificadores por número de proceso y los criterios de la línea de corte.
- **PC-6** → hacer la prueba del pasillo con una compañera de otro departamento. Detecta jerga peor y
  sobreafirmación igual de bien.

---

# 8. «SABER QUÉ EXISTE» SIN CATÁLOGO MUERTO, Y CÓMO SE ENSEÑA A NO USAR IA

## 8.1 El objetivo 1, resuelto con tres mecanismos y ningún listado de productos

El objetivo 1 del perfil es *«saber qué existe: que existen agentes, que existen automatizaciones, qué
se puede automatizar de su trabajo y qué no»*. Los tres términos van pegados a **su trabajo**. No pide
un mapa del sector: pide saber qué hay disponible para lo que ella hace. Un curso que conteste con un
recorrido de productos está contestando a otra pregunta, y además contesta con la mitad que caduca.

Este es, además, **el objetivo peor servido por este ángulo**, y lo digo aquí y no solo en la
autocrítica: un proceso solo se encuentra con las tecnologías que necesita. Tres mecanismos lo cubren, y
después está la valoración honesta de hasta dónde llegan.

**Mecanismo 1 · La Lista de techos (§3.4).** El catálogo no se enumera: **se genera**. Cada capa
declara, en la parte 3 de la pregunta fija, qué no puede hacer y **qué clase de cosa lo rompería**. Ocho
capas, ocho techos, más los que aparezcan por el camino. La tercera columna —la condición de
activación— es la que convierte un catálogo en criterio, porque las condiciones no caducan aunque los
productos sí.

Y la propiedad que lo hace funcionar: **una fila se escribe en el momento en que el proceso choca con
el techo**, no en un módulo de panorama. La fila del agente se escribe en la capa 4, cuando ya tiene un
sistema con juicio en dos puntos y entiende exactamente qué le falta. Antes de eso, «agente» es una
palabra; ahí es una carencia concreta con nombre.

**Mecanismo 2 · Los ocho dobletes.** Fuerzan encuentros con procesos que **no son el suyo** y que piden
cosas que su proceso no pide: uno pide una fórmula y no un modelo (P02), otro es zona prohibida por
normativa viva (P08), otro es determinista puro (P30), otro tiene un freno que viene del RGPD y no de la
calidad (P28), otro no se deja medir en minutos (P12), otro necesita una fuente de verdad antes que una
automatización (P32). **Seis clases distintas de respuesta en menos de tres horas**, todas emitidas
justo después de haber hecho esa misma cosa de verdad.

**Mecanismo 3 · La caja del fondo, una sola vez, en M4 y no antes.**
Media página, con el eje puesto en la condición y no en el producto — que es la diferencia entre una
tabla que hay que rehacer cada año y una que se revisa:

| Qué haría falta para que me tocara | La clase de cosa que lo haría | Qué es hoy, para que lo reconozca si me hablan de ello |
|---|---|---|
| Tener que tocar un sistema que no está en mi suite (el software académico, la pasarela de pago, el mensajero, el portal de una agencia) | Una plataforma de automatización externa | *(nombres de hoy en `tres-nombres.md`)*. Ojo: mete un proveedor más entre mis datos y yo, y eso hay que pesarlo |
| Tener una tarea cuyos pasos no pueda dibujar de antemano | Un agente: le das el objetivo y los límites y decide los pasos | Están detrás de planes que mi empresa casi con seguridad no tiene, y necesitarían tocar recursos compartidos |
| Necesitar que una herramienta lea de una fuente mía con permisos acotados | Un conector, y el estándar por el que se conectan | Para mí hoy es **vocabulario, no herramienta**. Lo que sí me sirve es el principio de debajo: **conectar solo a lo necesario** |
| Tener que procesar decenas de ficheros locales de forma repetida | Un agente con acceso al sistema de ficheros | Revisar doscientos contratos de estancia larga buscando una cláusula sería el caso |
| Que las fuentes pasen de decenas a cientos y el asistente empiece a perderse | Arquitecturas de recuperación sobre corpus grandes | Con veinte fuentes bien fechadas no me hace falta nada de eso |
| Que me hablen de un sitio «de la misma empresa, gratis, donde se prueban prompts» | Una superficie de desarrollador | **Trampa silenciosa:** sus propios términos dicen que no metas información personal. Parece seguro porque entras con la cuenta de siempre, y no lo es |

**Y una decisión deliberada: el agente autónomo no está en la lista de destinos posibles para su
proceso.** Se define, se explica y se le pone su condición de activación en M4, pero no es una opción
que ella pueda elegir para su tarea, y eso se dice con todas las letras. El motivo es pedagógico y
verificable: el error número uno al clasificar es poner «agente» a todo, porque es la palabra que suena
a solución completa y es lo que promete internet. Sacarlo de la lista obliga a decidir entre lo que sí
existe para ella.

**Hasta dónde llega esto, honestamente.** Cubre lo que su proceso toca y lo que los dobletes rozan. **No
cubre** el panorama del sector, ni le da una opinión informada sobre familias de herramientas que no ha
visto. Si en dos años le preguntan en una entrevista «¿qué herramientas de automatización conoces?», la
respuesta honesta de este curso es *«conozco la anatomía y sé leer el catálogo de pasos de una que no he
visto nunca»* — que es mejor respuesta de lo que parece, pero no es la que da un curso de panorama. La
arquitectura 2 sirve este objetivo mejor que esta, y está dicho en §14.2.

## 8.2 Cómo se enseña a NO usar IA cuando no toca

Seis mecanismos, de más estructural a más operativo. **Ninguno es una advertencia suelta, y los seis
producen algo que se puntúa** — porque lo que no se evalúa, no se hace.

**1 · La línea de corte: el «no» es interior al proceso.**
Este es el mecanismo propio de este ángulo y el más fuerte de los seis. El entregable central de M1 no
es «qué automatizo» sino **el proceso partido en trozos, cada trozo con veredicto y motivo**. La rúbrica
es tajante: *si no hay ningún trozo que se quede contigo, está mal resuelto*, y *si el motivo es «es
difícil», está mal*. Los motivos legítimos son tres y se enseñan como tales:

| Motivo legítimo para que un trozo se quede con ella | Ejemplo de su casa |
|---|---|
| **Riesgo**: el error lo paga un cliente, una administración o la caja | Cualquier trozo que toque importes, plazos de visado o disponibilidad de alojamiento |
| **Conocimiento que caduca**: la regla cambia más deprisa de lo que se puede mantener el artefacto | Requisitos consulares, que se reordenaron en 2025 y volverán a cambiar |
| **No hay fuente de verdad**: nadie puede nombrar el documento vigente ni su dueño | El tarifario en alemán, que lleva meses desactualizado y nadie lo sabe |

Y hay un cuarto que no es de riesgo sino de escalón, y que merece su propio nombre porque es el que
nadie enseña: **este trozo no necesita un modelo de lenguaje, necesita una fórmula, un filtro o un
calendario.** Es el escalón −1, y su ejemplo canónico es suyo: **el presupuesto (P02) es aritmética
sobre una tabla de precios.** Meter un modelo ahí no es ineficiente: **es introducir un error posible
donde no lo había.** Es también el doblete de M1, para que no se quede en teoría.

**2 · La regla de los tres noes en los dobletes.** De ocho, al menos tres tienen que terminar en «no
aplica» o «aplica pero no compensa». Convierte el «no» en algo que hay que **encontrar**, y desactiva el
sesgo que produce un curso de IA por su mera existencia. La cuota está justificada con el reparto real
del dominio (§1.6 B) y su riesgo —fabricar noes de conveniencia— está reconocido en §14.7.

**3 · Las zonas prohibidas, con el motivo y no solo la prohibición**, porque una prohibición sin motivo
no se transfiere a un caso nuevo:

| Proceso | Por qué no, dicho de forma transferible |
|---|---|
| **P08** carta de aceptación para visado | Riesgo crítico y **normativa viva**. **Congelar dentro de un artefacto un conocimiento que caduca es fabricar un error futuro** |
| **P26** quejas formales | Una respuesta que **admite responsabilidad por escrito compromete a la empresa**. Y los modelos son complacientes: la complacencia por escrito, en una queja, es exposición legal |
| **P29** emergencias 24 h | Personas, menores, responsabilidad civil, y un alumno en estado de shock con nivel A1 |
| **P25** reembolsos | Datos bancarios y riesgo de fraude por suplantación en el cambio de cuenta |
| **P17** matching con familia de acogida | Concentra **salud, religión y potencialmente orientación sexual** en una casilla de texto libre. Es el proceso que **más parece** el caso ideal de IA, y por eso es la trampa |
| **P22** calendario de camas | Riesgo crítico por overbooking, y además es un calendario de recursos: escalón −1 |
| **P05 / P16** nivelación y exámenes | **Anexo III del Reglamento de IA**: *evaluar el nivel educativo* es alto riesgo. Aplazado al 02.12.2027, **no cancelado**. Lo suyo no es decidirlo **[!]**: es reconocerlo y avisar |

Y la regla de oro que hace todo esto memorable, y que se recuerda cuando una lista de artículos no:

> **De todo su trabajo, el único trocito que está en la lista de alto riesgo es el que decide el nivel
> de un alumno. Todo lo demás —redactar, traducir, resumir, clasificar, preparar borradores— no lo
> está.** Esa asimetría se recuerda.

**4 · El coste completo como criterio de descarte, no como cálculo de justificación** (M5). *Un sistema
que ahorra ocho minutos y cuesta diez de revisión es una pérdida disfrazada de modernidad.* Y la métrica
de vanidad tiene nombre: **que se ejecute cada lunes no es que funcione.**

**5 · La opción segura suele ser también la más eficiente, y eso hay que demostrarlo, no predicarlo.**
El mejor ejemplo, y va en M2: **no transcribas la llamada.** Escribe tú un resumen de cuatro líneas al
colgar, ya seudonimizado, y trabaja con ese resumen. Es más rápido que subir un audio de doce minutos,
no genera un tratamiento nuevo ni un destinatario nuevo, y de paso piensas el caso. Enseñado así, «no
usar IA» deja de ser una renuncia y pasa a ser una decisión de eficiencia.

**6 · Se evalúa.** La línea de corte tiene rúbrica, los dobletes tienen cuota, el coste completo tiene
resta obligatoria, y la lista de noes es un entregable de M7 y la pieza que le da credibilidad al
dossier. Si no se puntúa, no se hace.

---

# 9. PROTECCIÓN DE DATOS, INTEGRADA

## 9.1 El principio de diseño: no es un módulo, y tampoco es «transversal» en abstracto

Un módulo de protección de datos se lee una vez, se aprueba y se olvida. Y además produce parálisis,
cuando el objetivo es que **use más la IA, no menos: que la use en el sitio correcto**. Un bloque de
protección de datos que produce parálisis ha fallado.

Pero «transversal» tampoco basta como respuesta, porque suele significar «repartido y por tanto de
nadie». En este ángulo la protección de datos tiene una forma concreta: **es una de las capas del
proceso, con su artefacto propio**, y aparece en tres momentos, cada uno **pegado a la acción que
desbloquea**, nunca antes ni después.

| Capa | Dónde | Qué contiene | **Por qué exactamente ahí** |
|---|---|---|---|
| **Antes de tocar nada** | **M0**, día 1 y día 3 | Cuenta de empresa frente a cuenta personal · **las cuatro preguntas que definen cualquier plan** · qué edición, qué licencia, qué retención, qué política escrita · **el semáforo verde/ámbar/rojo impreso** · y **la columna de datos en el criterio de elección del proceso** | **Es la semana en la que va a empezar a pegar cosas.** Todo lo demás se construiría sobre un suelo que no ha mirado. Y aquí hay una decisión propia de este ángulo: **el color de los datos es una de las cinco columnas con las que elige el proceso**, con un −3 que descalifica. Es decir, la protección de datos no llega a frenar el proyecto: **decide cuál es el proyecto** |
| **Cuando le mete datos** | **M2**, antes de cargar fuentes | **El mapa de datos del proceso** (§9.2) · por qué quitar el nombre no basta · cuasi-identificadores · **la prueba de la compañera** · la regla de los adjuntos | **Es el momento exacto en que pasa de pegar texto a subir ficheros.** Al pegar ves lo que envías; al adjuntar, no. Un Excel va **completo** —todas las filas, las columnas ocultas, la hoja que se llama «datos antiguos»—, un PDF de pasaporte va entero, una foto lleva coordenadas. Ese salto es donde cambia el orden de magnitud del riesgo |
| **Cuando algo actúa sin que ella mire** | **M4**, con los frenos | Lista de temas prohibidos · condiciones de parada · *nada sale al cliente sin que un humano le dé a enviar* · **el aviso de IA del art. 50**, en vigor desde el 02.08.2026 · registro de qué se generó y quién lo aprobó · plan para el día que falle, **incluido valorar si hay brecha [!]** · y el **Anexo III** aplicado a su academia | **Es cuando algo empieza a actuar sin que ella revise cada paso.** Antes de M4 no hacía falta; después de M4 sería tarde |

**Capa permanente:** la **tarjeta del lunes** impresa al lado de la pantalla desde la semana 1, con seis
preguntas que caben en una nota adhesiva. Si una regla necesita que te pares a pensar, no sobrevive a un
martes de julio con trescientos correos sin abrir.

## 9.2 El artefacto propio de este ángulo: el mapa de datos del proceso

Un semáforo genérico se lee y se olvida. **Un semáforo aplicado al único proceso que está construyendo
se usa**, porque contesta una pregunta que tiene delante. Una cara, cuatro columnas:

| Dato que atraviesa el proceso | Color | **Dónde entra en el flujo** | **Dónde hay que quitarlo, y quién lo quita** |
|---|---|---|---|
| Nombre y apellidos del alumno | Ámbar | En el correo entrante | Antes de pegar nada: lo quito yo, a mano |
| Nacionalidad + edad + fecha de llegada + barrio | **Ámbar peligroso** | En el cuerpo del correo | Se **generalizan**, no se borran: «alumno», «esta semana», «familia de acogida». Combinados identifican a una persona entre 1.400 |
| Nº de pasaporte o NIE | **Rojo** | Adjunto en la reserva | **No entra nunca.** Si necesito un dato de ahí, lo escribo yo a mano, y solo ese |
| IBAN, tarjeta, justificante de pago | **Rojo** | Adjunto o cuerpo | **No entra nunca**, en ninguna herramienta |
| Alergia, dieta médica, medicación | **Rojo** | Formulario de preferencias | **No entra nunca**, ni seudonimizado. Se degrada al mínimo funcional si el texto lo exige: «una intolerancia alimentaria» |
| Cualquier dato de un **menor** | **Rojo absoluto** | Grupos escolares, estancias de 16-17 | **Nunca, en ninguna herramienta, ni seudonimizado.** Sin excepciones |
| Dirección del alojamiento junto al nombre | **Rojo** | Confirmación de alojamiento | No entra. Localiza físicamente a una persona |
| Tarifario, calendario, condiciones, plantillas | **Verde** | Documentos de la academia | **No son datos personales.** Entran sin pensar, y por eso el proceso puede empezar aquí |

**Cuatro cosas que este artefacto hace y un semáforo genérico no:**

1. **Sitúa el punto de corte en el flujo, que es lo que convierte la regla en un gesto.** Saber que un
   pasaporte es rojo no cambia nada un martes; saber que **el pasaporte entra como adjunto en el paso
   dos y por eso el paso dos nunca sube el adjunto original** sí.
2. **Nombra quién lo quita.** Si la respuesta no es una persona o un paso concreto, no hay corte: hay
   una intención.
3. **Es reutilizable como hábito portátil.** Un mapa de datos por proceso vale en cualquier empresa y en
   cualquier año, y no menciona ninguna herramienta.
4. **Muestra que la mayoría de su proceso empezó en verde**, que es el mensaje que evita la parálisis:
   la protección de datos no le prohíbe trabajar, le dice **por dónde empezar**.

## 9.3 Las cinco decisiones que hacen que esto funcione y no asuste

1. **La regla de los menores es tajante y sin excepciones**, más restrictiva de lo que la norma exige en
   todos los supuestos, **a propósito**: una regla con excepciones no sobrevive a julio.
2. **Cada decisión que no es suya va marcada [!] y con el nombre de a quién se escala.** El riesgo
   específico de este perfil es que, por ser la que más se preocupa, acabe siendo de facto la
   responsable de cumplimiento de la academia. El material lo prohíbe explícitamente: *tu papel no es
   ser la responsable de cumplimiento; tu papel es no ser tú el agujero, y saber cuándo hay que levantar
   la mano.*
3. **Nada normativo se congela dentro de un artefacto.** Las fechas del Reglamento de IA, el estado del
   marco de transferencias a Estados Unidos y la ley española viven en un fichero de contexto **con
   fecha visible** que se revisa. Y eso es, además, el mejor ejemplo pedagógico del curso de la
   diferencia entre conocimiento estable y conocimiento volátil — que es exactamente la distinción que
   hay que dominar para construir fuentes que no envejezcan mal.
4. **El encuadre no es de permiso, es de aportación.** No está pidiendo autorización para nada: ya usa
   la herramienta, se la ha dado su empresa, y usarla está bien visto. Está entendiendo la configuración
   antes de apoyarse en ella. Si la academia nunca se lo ha planteado, **acaba siendo ella quien propone
   la política**, que es el mejor resultado posible — y no es venta interna: es su propio trabajo.
5. **La transición con su cuenta personal se resuelve sin moralina**, porque la moralina no cambia
   hábitos y además sería injusta: lo que hace es lo que hace casi todo el mundo. Se traza una línea
   limpia —cosas suyas y prácticas con casos inventados, en la personal; **cualquier cosa que venga de
   un correo, una llamada o un expediente de un cliente**, en la de empresa— y se da el argumento que
   de verdad convence, que no es «es ilegal»:

   > **Si mañana un alumno ejerce su derecho de supresión y la academia tiene que certificar que ha
   > borrado sus datos de todos los sitios, tu cuenta personal es un sitio que la academia no puede
   > tocar y del que ni siquiera sabe que existe.** No es que hayas hecho nada malo: es que has creado,
   > sin querer, un almacén de datos de clientes fuera del alcance de la empresa. Y eso, cuando aparece,
   > no tiene arreglo posible: no se puede desandar.

## 9.4 El dato que cambia la posición mental con la que se estudia esto

Merece salir en la primera página del curso: **el artículo 4 del Reglamento de IA, en vigor desde
febrero de 2025, obliga a las empresas que usan IA a garantizar un nivel suficiente de alfabetización en
IA de su personal.** Dicho de otro modo: **el curso que está haciendo es, técnicamente, cumplimiento
normativo de su empresa.** No es un extra que se paga a sí misma en su tiempo libre por pura iniciativa:
es una obligación de la academia que ella está cubriendo.

---

# 10. QUÉ SE QUEDA FUERA, A PROPÓSITO

## 10.1 Fuera porque el brief lo excluye

| Fuera | Por qué |
|---|---|
| **«Cómo conseguir el sí», venta interna, pedir autorización** | En su empresa usar IA ya está bien visto y **lo mal visto es no automatizar**. Un módulo de permiso resuelve un problema que ella no tiene. Lo que sí entra —evidenciar y contagiar— es otra cosa y está en M7 |
| **Portfolio, landing page, «lo que tengo ahora en mi CV»** | Es el destino del itinerario no técnico de la referencia porque **su alumno tipo quiere entrar en el sector de la IA**. La nuestra no quiere cambiar de rol ni de sector. Lo que sí quiere —que le sirva si cambia de empresa— lo da la portabilidad del criterio, no una web |
| **Certificado, insignia, «ahora eres AI Operator»** | No busca cambiar de rol. Y un certificado sin evaluador y sin rúbrica no certifica nada. La definición de «terminado» de §2 es observable y no la firma nadie |
| **Convertirse en AI specialist** | El objetivo es trabajar mejor en lo suyo. Todo lo que empuje hacia «ser la persona de la IA» como identidad profesional está fuera, incluido el vocabulario |
| **Cualquier cosa vistosa** | El grafo de la referencia es el caso de estudio: espectacular en pantalla, marginal en valor para un puesto de atención al cliente, y —dicho por su propia autora— *hecho para el agente, no para el humano*. Aquí el artefacto útil es aburrido: un asistente que cita, un triaje que etiqueta, un vigilante que avisa |
| **Construir y vender aplicaciones** | Ni siquiera la referencia lo promete, y con razón: *«construir algo para uso interno y publicarlo en internet son dos mundos distintos»* |

## 10.2 Fuera por el listón de durabilidad, con su condición de reentrada

| Fuera | Reducido a | Condición para que entre |
|---|---|---|
| **Plataformas de automatización externas como módulo** | **Una fila de la caja del fondo** + el criterio *automatiza donde ya viven tus datos* | Que su proceso tenga que tocar algo fuera de su suite. Entonces la siguiente parada es una plataforma externa; y una que haya que autoalojar, solo si aparece alguien técnico que la mantenga |
| **Escribir código, aunque lo escriba la IA** | **Media página informativa** | Que la automatización nativa se quede corta **y** haya quien mantenga el script. En el momento en que falla hay que leer un error de programador, y eso es una dependencia que ella no puede cubrir |
| **La superficie de desarrollador «gratis y de la misma empresa»** | **Cinco líneas, con aviso explícito** | Ninguna. Es la trampa más silenciosa del panorama y por eso se nombra: parece profesional, se entra con la cuenta de siempre, y sus términos dicen literalmente que no metas información personal |
| **Conectores y su estándar, como práctica** | **Vocabulario + el principio de privilegio mínimo** | Que monte algo fuera de su suite, o que alguien se lo configure y ella solo lo use |
| **Arquitecturas de recuperación sobre corpus grandes** | **Una fila de la caja del fondo** | Que las fuentes pasen de decenas a cientos y el asistente empiece a perderse |
| **Herramientas agénticas de escritorio y de terminal** | **Un apéndice de lectura, opcional, sin entregable** | Una tarea que exija procesar decenas de ficheros locales de forma repetida. **Si termina el curso sin abrir el apéndice, el curso ha funcionado igual**, y eso va en su primera línea |
| **Comparativas y nombres de modelo** | Nada | Ninguna. *«Da bastante igual qué modelo uses mientras no gastes miles en tokens.»* El material no se apoya en ningún nombre de modelo, a propósito: es el detalle que menos importa y el que más rápido caduca |

## 10.3 Fuera por rigor mal invertido

- **Estadística inferencial.** Nada de significación, valor p ni tamaño muestral sobre doce casos. Aquí
  no se estima un parámetro de una población: se comprueba la cobertura de un instrumento contra un
  criterio fijado. **Doce casos bien elegidos valen más que doscientos al azar.**
- **Consistencia interna aplicada a la batería.** Directamente incorrecto: una batería de casos **debe
  ser heterogénea**. Si tuviera consistencia interna alta sería porque está mal construida. En un banco
  de pruebas la heterogeneidad es una virtud, al revés que en una escala.
- **Prompt engineering como colección de trucos.** El curso enseña **el criterio antes del prompt**. Un
  prompt bueno que se escribe una vez y se pierde no vale nada; el mismo guardado con sus fuentes es
  infraestructura.
- **Vídeos de lección.** Un vídeo es relectura con mejor producción, y la relectura está clasificada
  como técnica de utilidad baja. Si hay vídeo, es de demostración de una interfaz, dura menos de tres
  minutos y va con transcripción escrita — porque la ruta de menús caduca y el texto se corrige.
- **Cualquier ejercicio de metodología sin artefacto reutilizable.** El riesgo de este perfil no es
  quedarse corta de rigor: es pasarse. Si un ejercicio le lleva más de lo que le llevaría hacer la
  tarea a mano durante un mes, está mal calibrado y se recorta.

## 10.4 Fuera por decisión propia de este ángulo, que es la más discutible

**La segunda automatización.** El curso construye **una** cosa. No hay un segundo proceso, no hay un
proyecto paralelo, no hay un hilo guiado que ella ejecute además del suyo. El expediente modelo se lee y
se usa como clave; no se hace.

Es la decisión más discutible del diseño y la defiendo así: con dos horas propias por semana, **dos
procesos son dos procesos a medias**, que es exactamente lo que este ángulo existe para evitar. El
segundo proceso es lo primero que hará **después** del curso, y para eso está la Lista de techos, la
rúbrica escrita por ella y la ficha de traspaso. El coste —perder el oráculo calibrado del hilo guiado—
está reconocido y compensado parcialmente en §14.3.

---

# 11. LOS TRES MOMENTOS DE MAYOR RIESGO DE ABANDONO

Criterio de selección: **probabilidad × irreversibilidad de la conclusión que saca**. Se descarta como
candidato el «primer resultado mediocre» —cuando el asistente contesta mal la primera vez— no porque sea
improbable (lo es), sino porque **su contramedida es barata, conocida y ya está incorporada en cada
módulo**: la caja *«lo que vas a ver la primera vez»*, escrita antes del ejercicio, que describe el
resultado mediocre concreto que va a obtener. Un fallo anunciado es una etapa; un fallo inesperado es un
veredicto sobre uno mismo. Y la cita de la referencia, que es la mejor frase del webinar y está en su
diapositiva 22 de 22: *«Ves el resultado. Detrás hay varias decenas de intentos.»*

---

## MOMENTO 1 · Días 1–10 — el arranque, y la sospecha de haber elegido mal

**Qué pasa por dentro.** El 52 % de los inscritos en un curso autodidacta **nunca llega a empezar** [E],
y la caída mayor está en los días 7–14. Aquí se acumulan tres cosas, y la tercera es específica de este
ángulo: la fricción de arranque; el beneficio del curso todavía es abstracto mientras el coste ya es
real; y —lo propio de aquí— **se le pide comprometerse con un proceso en la semana 1, que es cuando
menos criterio tiene**. La conclusión peligrosa no es «esto es difícil», es **«creo que he elegido mal y
llevo dos semanas»**, y esa es irreversible si no se anticipa.

**Qué se pone justo antes:**

1. **La sesión 1 no explica el curso: produce un resultado utilizable en veinticinco minutos**, con lo
   que ya tiene abierto, sin instalar nada y sin hablar con nadie. Instrucciones permanentes + un correo
   real hecho con ellas + minutos cronometrados antes y después. **El mapa del curso va después del
   primer resultado, nunca antes.**
2. **La elección no es una apuesta: es una prueba con tres criterios de rechazo observables** (§1.6 A2).
   Se le quita el peso de «acertar» y se le da un procedimiento. Y **el proceso de repuesto está
   nombrado y firmado el día 3**, no el día de la crisis.
3. **El divorcio preautorizado, con su aritmética escrita**: al final de M1, cambiar de proceso cuesta
   unas dos horas, porque lo único construido son cuatro documentos y el método ya lo sabe. **Escrito
   en la semana 1**, se lee como plan; escrito cuando ya ha dudado, como excusa.
4. **El contrato de una página, antes de empezar:** 18 semanas · 2 h semanales de tiempo propio ·
   **0 €** · nada que instalar · nada que pedirle a nadie · **la frontera de M4** · y la definición
   observable de «terminado». Un curso que se anuncia de ocho semanas y dura dieciocho se percibe como
   fracaso propio en la novena.
5. **El diagnóstico del entorno no puede bloquear.** Las comprobaciones empíricas están en la misma
   página que los mensajes, no en un anexo, y la rúbrica declara que *«pregunté a X el día D y no
   obtuve respuesta»* **es un resultado válido**.
6. **El modo mínimo y el ritual de reentrada, redactados en la semana 1**: una micro-sesión de diez
   minutos cuenta como semana cumplida; toda vuelta tras una pausa empieza leyendo las tres últimas
   entradas del cuaderno y respondiendo las cinco preguntas de repaso.
7. **PC-1 al final de la semana 2**: otra persona implicada en el punto de máxima mortalidad, y
   revisando exactamente la decisión que le da miedo.

---

## MOMENTO 2 · Semanas 7–9 — el primer bloqueo que no es culpa suya

**Qué pasa por dentro.** Es el riesgo específico de trabajar sobre un proceso real, y el que más me
preocuparía en producción. La automatización nativa de su entorno **falla con unidades compartidas,
carpetas compartidas y hojas con referencias externas** [V]. El centro de gravedad de su puesto **es un
buzón compartido y una hoja de camas compartida**. Es decir: la primera vez que intente automatizar su
trabajo de verdad, la herramienta puede decirle que no. Y la conclusión que se saca de ahí no es «me he
equivocado de carpeta»: es **«esta herramienta no sirve para mi trabajo»**, y detrás, *«este curso no
sirve para mi trabajo»*.

**Qué se pone justo antes:**

1. **La contramedida principal está seis semanas antes: la cuarta columna del embudo de elección.**
   Los procesos que solo viven en recursos compartidos se descartaron en la semana 1, cuando descartar
   costaba diez minutos. Esta es la aportación de diseño de este ángulo al problema, y es preventiva en
   vez de paliativa.
2. **Aun así, el límite va en la primera página del módulo, con nombre y por escrito**, no en una fe de
   erratas. *«Los primeros disparadores se construyen sobre tu propio buzón de empresa y sobre copias
   tuyas, y eso no es una versión de juguete: es la restricción real de la herramienta.»*
3. **La lista de seis comprobaciones de plataforma**, entregada **antes** del primer disparador y
   reutilizable como diagnóstico. Convierte un bloqueo en una comprobación con resultado, que es lo
   contrario de un veredicto sobre una misma.
4. **La página «cuando no coincide»**, que convierte la caducidad del material en competencia enseñada:
   *si algo no coincide con lo que ves, tu pantalla tiene razón y este texto no.*
5. **PC-4, el comodín, cuya existencia se anuncia mucho antes de que haga falta.** Saber que hay salida
   reduce la ansiedad aunque no se use.
6. **La caja «si nada de esto funciona»: documenta el fallo, rodéalo con una solución manual y sigue.**
   Un curso no puede pararse por un botón que alguien movió. Y hay una salida específica que el material
   nombra porque es la que más veces resuelve esto en una empresa pequeña: **pedir que le deleguen una
   etiqueta o una carpeta propia dentro del recurso compartido**. Es una petición a otra persona —lo que
   el diseño prometía no necesitar— y por eso está aquí y no en el camino principal.

---

## MOMENTO 3 · Semanas 11–14 — la meseta del «ya me sirve»

**Qué pasa por dentro.** Es el riesgo propio de este ángulo, y no aparece en los otros dos con esta
forma. Al terminar M4 **el sistema funciona y ella lo usa**. El dolor que la trajo al curso está
resuelto. Y justo entonces vienen tres módulos que no añaden funcionalidad: medir, dejarlo mantenible y
contagiarlo. Novedad baja, beneficio inmediato bajo, esfuerzo mental alto. **El abandono aquí no se
siente como abandono: se siente como haber terminado.** Y esa es exactamente la razón por la que es
peligroso, porque los objetivos 4 y 5 del perfil —criterio portátil y evangelización— viven enteros en
ese tramo.

**Qué se pone justo antes:**

1. **La frontera declarada desde la semana 1**, y con estas palabras: *«al acabar M4 ya tienes lo que
   viniste a buscar. Lo que viene después es lo que hace que esto te siga sirviendo dentro de dos años y
   en otra empresa, y es la parte que nadie hace.»* Nombrar la meseta antes de llegar a ella es lo que
   la convierte en un tramo y no en un final.
2. **El gancho de M5 no es metodológico, es de deseo: el número.** Ella quiere evidenciar valor —es su
   objetivo 5, formulado por ella— y **el número es la munición**. M5 no se presenta como «vamos a
   evaluar»: se presenta como *«vas a poder decir cuánto ahorras y defenderlo si alguien lo comprueba»*.
   Es el único módulo del curso cuyo motivo se puede formular enteramente en términos de lo que ella ya
   quiere.
3. **La lectura de la Tira completa como primera sesión de M5.** Cinco columnas de su propio trabajo,
   con fecha. A las trece semanas puede leer lo que en la semana 3 le parecía imposible. Es la evidencia
   objetiva contra la ilusión de fluidez, y es gratis.
4. **La cláusula del resultado decepcionante, escrita antes de medir:** *si la medición dice que ahorras
   poco, eso es un resultado del curso y no un fracaso tuyo.* Y las razones legítimas alternativas
   enumeradas de antemano —menos errores, menos carga mental, respuesta más rápida al cliente— con la
   instrucción de **medir esa otra razón** si es la que importa. La honestidad de la medición está
   protegida por adelantado, que es la única forma de que la medición sea honesta.
5. **PC-5 exactamente en la frontera** (fin de M4). Una conversación de diez minutos sobre su propio
   criterio es el mejor combustible disponible en el punto donde el material solo ya no tira. Y el
   objeto de la conversación —*«¿dónde moverías la línea de corte?»*— es intrínsecamente halagador de su
   trabajo sin ser halago: se conversa sobre criterio, que es lo que ya tiene.
6. **El compromiso externo de M7 se anuncia en M4, no en M7.** *«En la semana 17 una compañera va a usar
   esto una semana entera sin ti.»* Anunciarlo con cinco semanas de antelación convierte M5 y M6 en
   preparación de algo con fecha y con otra persona dentro, que es el mecanismo de permanencia más
   fuerte que hay disponible en un curso sin cohorte.
7. **El hallazgo vistoso se coloca en M6, no antes:** el doblete de P32 produce lo que ningún otro
   artefacto del curso produce —**una lista de errores reales que nadie en la academia sabía que
   existían**: precios del año pasado circulando en la plantilla alemana desde hace meses. Es el momento
   del curso en que su trabajo produce un hallazgo y no un ahorro, y por eso está donde el material solo
   ya no tira.

---

# 12. UNA LECCIÓN COMPLETA, DESARROLLADA

Se desarrolla **M4.2 — «Dónde tiene que pararse»**, la segunda sesión núcleo de la capa 4. Se elige por
cuatro razones: (a) es el contenido **más durable de todo el curso** —una condición de parada se escribe
igual hoy, en 2029 y en cualquier herramienta—; (b) es el punto donde la protección de datos, el riesgo
reputacional y el diseño de sistemas se tocan, así que enseña la textura real del material; (c) es el
único sitio del curso donde la formación de la alumna juega **en contra** y hay que decírselo; y (d) no
está desarrollado en ninguna de las arquitecturas hermanas, así que añade material en vez de repetirlo.

Se muestran las **cinco piezas** que componen una lección en este curso: el criterio, los clics, el
ejercicio, la rúbrica y la solución comentada.

---

## 12.1 `M4/M4.2-capa.md` — EL CRITERIO

```markdown
# M4.2 — Dónde tiene que pararse

⏱ 40 min · Necesitas: tu línea de corte (01), tu batería (01-casos) y el sistema
funcionando.
Tipo de tiempo: [ tiempo propio ]

## Antes de leer nada — 5 minutos, de memoria y por escrito

1. En tu batería, ¿qué tiene que contestar el sistema en los dos casos de rechazo,
   y qué cuenta como fallo aunque la respuesta esté bien redactada?
2. ¿Por qué cada fuente tuya lleva una fecha y un nombre en la primera línea?
3. De tu línea de corte: nombra un trozo que se quedó contigo y di por cuál de los
   tres motivos.
4. ¿Qué diferencia hay entre un disparador de calendario y uno de suceso, y por qué
   te importó a ti?
5. ¿Cuál es el tope de tu sistema y qué pasa cuando se supera?

> Escribe lo que recuerdes ANTES de mirar. Equivocarte aquí es el ejercicio, no un
> fallo. Respuestas al final de la lección.

## Para qué sirve esto en tu proceso

Tu sistema ya hace algo sin que se lo pidas. Eso significa que, a partir de hoy, va a
encontrarse con casos que tú no previste — y va a hacer algo con ellos. La pregunta de
esta lección no es qué hace bien: es **qué hace cuando no debería hacer nada**.

En tu trabajo esto no es un refinamiento. Tus clientes son extranjeros que se juegan un
visado, un semestre y un viaje pagado; entre el 30 % y el 50 % de las matrículas vienen
por agencias que reservan por volumen, así que un error se multiplica por quince; y las
reseñas son un canal de captación. El ahorro de tiempo se nota en la oficina, en
silencio. El fallo se nota en internet, en público y en el idioma del alumno.

## El criterio

### 1. La confianza no es una salvaguarda

Si la seguridad de un sistema depende de que alguien se acuerde de revisar, el sistema
no es seguro: **es seguro hasta el primer día de mucho trabajo.** Y en tu negocio el día
de mucho trabajo no es una sorpresa: se llama julio.

De ahí sale la única regla que no falla, y todas las demás son refuerzos de esta:

> **Nada sale a un cliente sin que una persona le dé a enviar.**

Coste: cinco segundos por pieza. Beneficio: elimina de golpe una categoría entera de
fallos. Se puede relajar más adelante, proceso a proceso y con datos de acierto
medidos. **No se relaja por costumbre**, y hay un motivo que conviene entender: el
riesgo de un sistema no es el del día 1, es el del día 60. El día 1 revisas todo. El
día 60 el sistema acierta el 95 % de las veces, te has relajado, y **el 5 % restante
pasa sin revisión**. La degradación no viene del error: viene de la confianza.

### 2. Una lista de temas prohibidos se escribe en negativo y sin matices

No es una guía de estilo: es una lista de temas sobre los que el sistema **nunca** se
pronuncia, aunque sepa la respuesta y aunque la respuesta sea correcta. Se escribe así:

> «Nunca respondas sobre requisitos o plazos de visado. Nunca cites importes. Nunca
> confirmes disponibilidad de alojamiento. Nunca respondas a una queja formal. Nunca
> menciones salud. Si el tema aparece, escribe SOLO: DERIVAR A PERSONA, y para.»

Tres propiedades que la hacen funcionar:

- **En negativo, no en positivo.** «Responde solo sobre X» deja fuera lo que no
  imaginaste; «nunca sobre Y» cierra Y para siempre.
- **Sin matices.** Un «salvo que...» convierte la lista en un problema de
  interpretación, y las interpretaciones no sobreviven a un martes de julio.
- **Se escribe para el sistema de dentro de seis meses, no para el de hoy.** Los
  sistemas se expanden solos: alguien añade una fuente, alguien amplía el disparador, y
  de pronto contesta cosas que no contestaba. Por eso la lista incluye importes, plazos
  de visado, disponibilidad y salud **aunque tu proceso hoy no los toque**.

**Y hay un criterio objetivo para construirla en vez de improvisarla:** los temas
prohibidos coinciden con los procesos de riesgo alto y crítico de tu inventario. No es
una lista de intuiciones: es una lista derivada.

### 3. Una condición de parada es distinta de un tema prohibido

Un tema prohibido dice **de qué** no se habla. Una condición de parada dice **cuándo**
se deja de trabajar, aunque el tema estuviera permitido. Las dos hacen falta y se
confunden todo el rato.

Las cinco condiciones que tiene que llevar cualquier sistema tuyo, y el motivo de cada
una:

| Condición | Por qué |
|---|---|
| **No encuentro la respuesta en mis fuentes** | Es «no lo sé» convertido en freno. Un sistema que nunca se niega no es que lo sepa todo: es que no lo has probado bien |
| **La persona está enfadada** | El coste de un error se multiplica, y la respuesta correcta deja de ser informativa |
| **Se menciona abogado, reclamación u hoja de reclamaciones** | A partir de ahí todo lo escrito es material de un expediente |
| **Se menciona salud, o hay un menor implicado** | Categoría especial y régimen reforzado. No es una cuestión de calidad de la respuesta |
| **El importe supera X** | Porque tú tampoco decides por encima de X, y el sistema no puede tener más autoridad que tú |

**La condición de parada es lo que separa un asistente de un problema.** Y la prueba de
que existe de verdad no es que esté escrita: es que **haya un caso fabricado que la
dispare y que hayas visto pararse el sistema**.

### 4. Parar no es callarse

Un sistema que para y no dice nada es peor que uno que no para, porque el caso
desaparece. Parar significa tres cosas a la vez:

1. **No producir la salida.**
2. **Dejar una marca visible** donde tú vas a mirar de todas formas: una etiqueta, una
   fila, un aviso.
3. **Decir por qué paró**, en una línea. «Paré porque el texto menciona un plazo de
   visado» te ahorra abrir el caso para averiguarlo.

### 5. Quién revisa es una persona, no un procedimiento

Si la respuesta a «¿quién revisa antes de que esto salga?» es «se revisa», **no hay
revisión**. Tiene que haber un nombre. Y si el nombre eres tú siempre, entonces tu
sistema tiene un punto único de fallo que se llama tus vacaciones — lo cual es un
problema real y se resuelve en la capa 6, pero conviene saberlo desde hoy.

### 6. Un aviso sobre tu propia formación, y va en serio

Esta es la única lección del curso donde tu formación juega **en contra**, y por eso te
lo digo aquí y no en una nota al pie.

El reflejo entrenado de una psicóloga ante alguien que se queja es **validar,
empatizar y hacerse cargo**. Los dos primeros están bien y son una ventaja real. El
tercero, por escrito, en una queja formal, **es una admisión de responsabilidad que
compromete a tu empresa**.

Y los modelos de lenguaje son complacientes por construcción: si le pides que redacte
una respuesta empática a una queja, te va a dar un texto estupendo que dice «tienes
razón, la habitación estaba en malas condiciones». Sonará mucho mejor que el correcto.
La diferencia entre las dos formulaciones es exactamente la línea que hay que ver:

- Reconocer la **experiencia**, no calificar el **hecho**: *«entiendo que llegar y
  encontrarte la habitación así fue una mala llegada»* frente a *«tienes razón, la
  habitación estaba mal»*.
- Describir lo que **se ha hecho**, no juzgar lo que pasó: *«hemos hablado con la
  familia y hemos revisado el registro de llegada»*.
- Y evitar el **«lamentamos que te sientas así»**, que suena a disculpa y funciona como
  invalidación: es el peor de los dos mundos.

Importes, plazos legales, responsabilidad y compensaciones **no los decides tú y no los
decide el sistema**. Se escalan. [!]

## Cuándo NO poner un freno

- **Cuando el freno duplica la revisión humana que ya existe.** Si absolutamente todo
  pasa por tus ojos antes de salir, añadir cinco condiciones de parada no añade
  seguridad: añade ruido y hace que dejes de mirar los avisos. Los frenos son para lo
  que **no** miras.
- **Cuando el tema prohibido es tan amplio que el sistema no puede hacer nada.** Si tu
  lista prohíbe hablar de todo lo que el proceso trata, el problema no son los frenos:
  es que ese trozo no debería estar en la parte entregable de tu línea de corte.

## El techo de esta capa

Un sistema con frenos hace bien lo que hace y no hace lo que no debe. **Sigue sin
decirte si merece la pena.** Puede pararse impecablemente cada vez que toca, y ahorrarte
cuatro minutos al mes. Eso es lo que pide la capa siguiente.

## Los clics

→ `clics/M4.2-clics-<tu-entorno>.md`

## Tu turno
→ Ejercicio E4.2

## Cierre — 3 líneas en la bitácora
- Qué he producido: ______
- Qué ha fallado: ______
- Qué haré distinto la próxima vez: ______

---
### Respuestas de las 5 preguntas
```

---

## 12.2 `M4/clics/M4.2-clics-<entorno-actual>.md` — LOS CLICS

```markdown
> Verificado el 22 de agosto de 2026 en el entorno de trabajo actual. **Si algo no
> coincide con lo que ves, tu pantalla tiene razón y este texto no.** Ve a
> `cuando-no-coincide.md`.

**A · Dónde vive la lista de temas prohibidos.**
Va **dentro de las instrucciones del asistente**, no en un documento aparte que el
asistente tenga que consultar. Motivo práctico: lo que está en las instrucciones se
aplica siempre; lo que está en una fuente, solo si la consulta.
Si el trozo automatizado no usa el asistente sino un paso de IA suelto del flujo, la
lista va **pegada dentro del texto de ese paso**, entera, cada vez.

**B · Cómo se hace que un paso pare y marque.**
1. En el flujo, después del paso que produce la salida, añade un paso de decisión
   (hoy se llama «comprobar si»).
2. La condición se escribe sobre el texto de la salida: si contiene `DERIVAR A
   PERSONA`, la rama es la de parada.
3. En la rama de parada: **no** el paso que crea el borrador; sí un paso de etiqueta
   (hoy, «añadir etiqueta») y un paso de aviso (hoy, «avisarme por chat»).
4. En el aviso, incluye el motivo. El paso de aviso admite texto libre: mete ahí la
   línea que el asistente ha devuelto.

**C · El tope.**
Se implementa con un paso de conteo antes del bucle: si el número de elementos supera
N, salta directamente al aviso y no ejecuta el resto. Hoy no hay un «tope» como
opción de la interfaz: se construye así.

**D · Límites de hoy que afectan a esta lección.**
- Un flujo tiene **un solo disparador**, así que las condiciones de parada de dos
  disparadores distintos son dos flujos distintos.
- La interfaz muestra un número limitado de etiquetas del correo: si no ves la tuya,
  no es que no exista.
- Tu administrador puede tener pasos desactivados, y no hay forma de saberlo hasta
  que lo intentas.

**Cifras y límites** → `comun/datos-volatiles.md`.
*Si esto ha cambiado, lo que sigue siendo verdad está en `M4.2-capa.md`.*
```

---

## 12.3 `M4/M4.2-ejercicio.md` — EL EJERCICIO

```markdown
# E4.2 — Los frenos de tu sistema, y las cinco paradas que has visto pararse

⏱ 70–90 min · Tipo de tiempo: mitad trabajo, mitad propio

## Lo que tienes que producir

Un fichero `04-frenos.md` dentro de tu expediente, con cuatro apartados:
(a) la lista de temas prohibidos · (b) las condiciones de parada · (c) quién revisa,
con nombre · (d) cómo se apaga.
Y **cinco casos fabricados** en `04-casos-de-parada.md`, cada uno con la condición
que debe disparar y el resultado observado, con fecha.

## Criterios de éxito — obsérvalos, no los valores

Al terminar, esto tiene que ser cierto:
- [ ] Los cinco casos fabricados **han parado de verdad**, y lo has visto.
- [ ] Cada parada ha dejado **una marca visible** donde tú miras de todas formas.
- [ ] Cada parada dice **por qué** paró, en una línea.
- [ ] El apartado (c) contiene **un nombre de persona**.
- [ ] Has apagado el sistema y lo has vuelto a encender.

## Cómo lo vas a comprobar

Marca el nivel más alto que aplique — nunca uses uno inferior si hay uno superior
disponible:
- [x] **Se ejecuta** → los cinco casos fabricados paran, y un sexto caso normal NO
      para. (Si el sexto también para, tus frenos son demasiado anchos y el sistema
      no sirve para nada: ese es el fallo del otro lado y hay que verlo.)
- [ ] Batería con respuesta conocida → los 2 casos de rechazo de tu batería original,
      que ahora deben **parar**, no solo decir «no lo sé».
- [ ] Lista de comprobación → abajo.
- [ ] Rúbrica + protocolo de IA → `M4.2-rubrica.md` + `comun/protocolo-ia.md`.

## Los cinco casos que tienes que fabricar

Escríbelos tú, con material inventado, y que se parezcan de verdad a los que llegan:

1. Uno que **mencione un plazo o un requisito de visado**.
2. Uno que **pregunte un precio** o pida confirmación de un importe.
3. Uno de alguien **claramente enfadado**, sin insultos, con la palabra «reclamación».
4. Uno que **mencione una alergia, una medicación o un problema de salud**.
5. Uno **ambiguo a propósito**: que roce un tema prohibido sin nombrarlo. Por ejemplo,
   alguien que pregunta «¿cuánto tarda el papeleo para poder venir?» sin decir la
   palabra visado.

> El quinto es el que de verdad prueba tus frenos. Los cuatro primeros los para
> cualquier lista; el quinto separa una lista de palabras de una lista de temas.

## Antes de comprobar nada: escríbelo

> **Por qué lo he hecho así:** <3–5 líneas, en tus palabras>
> **Dónde creo que falla:** <1 línea>

Esto se escribe ANTES de corregir. Si lo escribes después, no sirve.

## Lista de comprobación (binaria y observable)

- [ ] ¿La lista de temas prohibidos incluye **importes, plazos de visado,
      disponibilidad y salud**, aunque mi proceso hoy no los toque? SÍ / NO
- [ ] ¿Está escrita **en negativo** y **sin ningún «salvo que»**? SÍ / NO
- [ ] ¿Hay una condición de parada para **«no encuentro la respuesta en mis
      fuentes»**? SÍ / NO
- [ ] ¿Hay una condición para **cliente enfadado**? ¿Y para **abogado o
      reclamación**? ¿Y para **salud o menor**? ¿Y para **importe por encima de X**?
      SÍ / NO
- [ ] Cuando para, ¿deja una marca **donde yo miro de todas formas**? SÍ / NO
- [ ] Cuando para, ¿dice **por qué**? SÍ / NO
- [ ] ¿La respuesta a «quién revisa antes de que salga» es **un nombre de persona**?
      SÍ / NO
- [ ] ¿He **apagado el sistema y lo he vuelto a encender**, hoy? SÍ / NO
- [ ] ¿He probado el **tope** metiéndole un lote grande a propósito? SÍ / NO
- [ ] ¿Hay algún camino por el que algo llegue a un cliente **sin que una persona le
      dé a enviar**? SÍ / NO  ← si es SÍ, vuelve al principio
- [ ] ¿He anotado el resultado de los cinco casos en `04-casos-de-parada.md`, **con
      la fecha de hoy**? SÍ / NO

## Si te atascas

1. Si un caso no para, mira primero **qué devolvió el asistente**, no el flujo. Nueve
   de cada diez veces el freno está bien y lo que falla es que la instrucción no
   incluía ese tema en la lista.
2. Si el quinto caso (el ambiguo) no para, tu lista es de **palabras** y no de
   **temas**. Añade al asistente una frase del tipo «si el mensaje trata de X aunque
   no use la palabra X, aplica la regla igual», y vuelve a probar.
3. *(Tras 25 minutos de intento)* La solución comentada, con los seis fallos típicos.

> Las pistas se abren en orden, no de golpe.
```

---

## 12.4 `M4/M4.2-rubrica.md` — LA RÚBRICA

```markdown
# Rúbrica — E4.2

Se usa **al día siguiente**, nunca al terminar.
Encuadre obligatorio: *«reviso el trabajo de alguien que hace mi puesto y tengo que
decidir si se lo devuelvo».*

## Bloque 1 · Señales de fallo (obligatorio buscar y responder)

Por cada una: encuentra el caso, o **declara por escrito que has buscado y no
existe**. «No aplica» no es una respuesta admitida.

| # | Señal de fallo | ☐ | Dónde / por qué no |
|---|---|---|---|
| 1 | Existe un mensaje razonable de mi trabajo real que este sistema contestaría de dos formas distintas según el día. Escríbelo | ☐ | |
| 2 | Existe un caso en el que el sistema **sigue adelante sin un dato que necesita**. Nómbralo | ☐ | |
| 3 | Hay una condición de parada que **está escrita pero que no he visto dispararse nunca** | ☐ | |
| 4 | Hay algún camino por el que algo sale hacia fuera **sin que yo apruebe** | ☐ | |
| 5 | Hay algún dato dentro de este sistema que, **si se filtrara mañana, tendría que comunicar a alguien** | ☐ | |
| 6 | Algún borrador de los que produce **suena estupendo y admite responsabilidad**. (Aparece casi siempre. Cuando aparezca, es el mejor ejemplo del curso de por qué la validez aparente no basta) | ☐ | |
| 7 | La lista de temas prohibidos **no incluye algo que mi sistema podría tocar dentro de seis meses** si alguien le añade una fuente | ☐ | |

## Bloque 2 · Umbral de «listo»

NO está listo si se cumple **cualquiera** de estas:
- Alguno de los cinco casos fabricados **no paró**.
- El sexto caso, el normal, **también paró** (frenos demasiado anchos: el sistema no
  hace nada y eso no es seguridad, es inutilidad).
- Alguna parada **no dejó marca**, o no dijo por qué.
- La respuesta a «quién revisa» **no es un nombre de persona**.
- El apagado está escrito pero **no probado**.
- Alguna señal de fallo del bloque 1 está marcada y sin arreglar.

## Bloque 3 · Si lo pasas por la IA

Protocolo completo en `comun/protocolo-ia.md`. Las tres que más se olvidan:
**hilo nuevo · no digas que es tuyo · no discutas: abre otro hilo.**
Y una específica de esta rúbrica: pega **la lista de temas prohibidos entera** junto
con la rúbrica. Sin ella el modelo se inventa el estándar, y el estándar que se
inventa es benévolo.

Y una advertencia que vale la pena leer dos veces: **este es el entregable del curso
donde menos hay que fiarse de la corrección con IA**, porque le estás pidiendo a un
modelo complaciente que juzgue si otro modelo es demasiado complaciente. Usa la IA
aquí solo para el bloque 1, y **el bloque 2 lo compruebas mirando**.

## Mi veredicto (lo firmo yo, no la IA)

[ ] Listo · [ ] Le falta: ______ · [ ] Lo dejo así y anoto por qué: ______
```

---

## 12.5 `M4/M4.2-solucion.md` — LA SOLUCIÓN COMENTADA

```markdown
# Solución comentada — E4.2

## Una lista de frenos posible (del expediente modelo)

TEMAS PROHIBIDOS — el sistema nunca se pronuncia sobre:
  · requisitos, plazos, trámites o probabilidades de visado
  · importes, precios, descuentos, penalizaciones o devoluciones
  · disponibilidad de alojamiento o de plazas
  · el contenido de una queja formal
  · salud, alergias, dietas médicas o medicación
Si el mensaje trata de alguno de estos temas, aunque no use esas palabras:
  devuelve SOLO la línea `DERIVAR A PERSONA — motivo: <tema>` y para.

CONDICIONES DE PARADA — además, para si:
  · no encuentras la respuesta en las fuentes que tienes
  · la persona expresa enfado, o menciona abogado, reclamación u hoja de
    reclamaciones
  · hay un menor implicado
  · el mensaje viene de una agencia y menciona un acuerdo o convenio particular
QUIÉN REVISA: <nombre>, antes de las 18:00 del mismo día.
CÓMO SE APAGA: interruptor del flujo. Probado el <fecha>.

## Por qué está así — decisión a decisión

| Decisión | Por qué esta | Qué pasa con la otra |
|---|---|---|
| «aunque no use esas palabras» | Convierte una lista de palabras en una lista de temas. Es la línea que hace parar el caso ambiguo | El sistema para «¿cuánto cuesta?» y no para «¿me sale muy caro esto?» |
| `DERIVAR A PERSONA — motivo: <tema>` | La marca es procesable: se puede etiquetar por motivo y contar cuántas paradas hay de cada tipo | «No puedo ayudarte con eso» te obliga a abrir el caso para saber por qué |
| «y para» al final | Sin esa palabra, el modelo derivará **y además** intentará ayudar un poco, que es lo peor de los dos mundos | Un mensaje que dice «esto lo verá una persona» y a continuación da un plazo de visado inventado |
| La agencia como condición de parada | No es un tema sensible: es que **las agencias tienen tarifas netas y condiciones de cancelación pactadas por convenio, distintas de las públicas**, y el sistema no las conoce | Aplicar la tarifa pública a una agencia con tarifa neta rompe el margen o rompe la relación comercial. Y se multiplica por quince alumnos |
| «antes de las 18:00 del mismo día» | Un revisor sin plazo no es un revisor | El caso se queda esperando y el cliente escribe otra vez |

## Anatomía de los errores típicos

### Fallo 1 · «La lista de palabras»  ← el más común
- **Cómo se reconoce:** los cuatro primeros casos fabricados paran y el quinto, el
  ambiguo, no.
- **Por qué pasa:** escribiste los temas como si fueran términos de búsqueda.
- **Arreglo mínimo:** añadir «aunque no use esas palabras» y dar un ejemplo frontera
  resuelto dentro de la propia instrucción.

### Fallo 2 · «El freno mudo»
- **Cómo se reconoce:** el sistema para, y tú te enteras tres días después.
- **Por qué pasa:** confundiste «no producir salida» con «parar». Parar son tres
  cosas: no producir, marcar y decir por qué.
- **Arreglo mínimo:** una etiqueta en la bandeja donde ya miras + el motivo en el
  aviso.

### Fallo 3 · «El revisor fantasma»
- **Cómo se reconoce:** en el apartado (c) pone «se revisa antes de enviar».
- **Por qué pasa:** es lo que se escribe cuando la revisora eres tú y te parece
  obvio.
- **Arreglo mínimo:** poner tu nombre y una hora. Y si al escribirlo te das cuenta de
  que solo puedes ser tú, has encontrado el punto único de fallo de tu sistema: eso es
  material de la capa 6, no un problema de hoy.

### Fallo 4 · «El complaciente que suena bien»  ← el más importante y el menos evidente
- **Cómo se reconoce:** entre los borradores hay uno que dice, en un español
  impecable, «tienes razón, hubo un fallo por nuestra parte».
- **Por qué pasa:** los modelos están optimizados para producir texto plausible y
  agradable, y en una queja lo agradable es darte la razón. **La plausibilidad de la
  superficie es su función objetivo, no un efecto secundario.**
- **Arreglo mínimo:** añadir a la lista de temas prohibidos «nunca reconozcas un
  hecho ni una responsabilidad: describe solo lo que se ha comprobado», y añadir ese
  borrador a tu batería como caso que **debe** parar.

### Fallo 5 · «El freno que ahoga»
- **Cómo se reconoce:** el sexto caso —el normal— también para. En una semana, el
  90 % de las entradas acaban en DERIVAR A PERSONA.
- **Por qué pasa:** sobrecorrección tras ver el fallo 4. Es la reacción natural y hay
  que anticiparla.
- **Arreglo mínimo:** mirar las paradas de una semana y separar las que eran
  correctas de las que no. Si más de la mitad no lo eran, el problema no son los
  frenos: es que el trozo automatizado está mal recortado, y eso se arregla en la
  línea de corte, no aquí.

### Fallo 6 · «La lista de hoy»
- **Cómo se reconoce:** la lista solo prohíbe lo que tu proceso toca ahora mismo.
- **Por qué pasa:** parece lo razonable.
- **Arreglo mínimo:** los cuatro fijos —importes, visados, disponibilidad, salud—
  entran siempre, aunque hoy sobren. Los sistemas se expanden solos.

## Lo que también sería correcto

- Poner los temas prohibidos **en el flujo** en vez de en el asistente, si el trozo
  automatizado no usa asistente. Cambia el sitio, no el criterio.
- Una condición de parada adicional por **idioma**: parar si el mensaje llega en un
  idioma que no está entre los que has probado. Es prudente y es tuyo.
- Sustituir «importe por encima de X» por «cualquier importe», si en tu proceso los
  importes no aparecen nunca de forma legítima. Más restrictivo, igual de válido.

## Lo que parece correcto y no lo es

- **Pedirle al sistema que puntúe su propia confianza del 1 al 10 y parar por debajo
  de 7.** Queda precioso y no vale nada: la confianza autoinformada de un modelo no
  está calibrada. Un 7 de una respuesta no es comparable con el 7 de otra. Si quieres
  un criterio de abstención, que sea **verificable**: «¿puedes citar el documento del
  que sale este dato? Si no, para.»
- **Escribir la lista en positivo** («responde solo sobre horarios, direcciones y
  material del curso»). Parece más limpio y deja fuera todo lo que no imaginaste, que
  es justo lo que va a llegar.
- **Poner un aviso automático al cliente diciendo que su caso ha sido derivado.** Es
  una salida hacia fuera sin persona en medio, aunque parezca inocua — y además, desde
  el 02.08.2026, si el cliente interactúa con un sistema de IA hay que informarle de
  ello. Esa línea la marca tu empresa, no tú. [!]
```

---

## 12.6 Qué demuestra esta lección sobre la textura del material

Seis cosas, y son las que hay que poder repetir en las otras cuarenta lecciones:

1. **La mitad de criterio no nombra ni un producto y no lleva fecha.** Se puede leer en 2029 sin cambiar
   una palabra. La mitad de clics es sustituible en veinte minutos.
2. **Todo lo evaluable es observable.** «Los cinco casos pararon» se mira; «los frenos son adecuados»
   no se puede contestar. La rúbrica solo entra donde la comprobación no llega.
3. **El fallo del otro lado siempre está escrito.** No solo «que no pare»: también «que pare siempre».
   Un material que solo avisa en una dirección produce sobrecorrección, que es un fallo tan caro y menos
   visible.
4. **El dominio está dentro, no de adorno.** Las agencias con tarifa neta, las reseñas como canal de
   captación, julio. Sin eso la lección es genérica y ella la lee como quien lee un manual.
5. **La formación de la alumna aparece con sus dos caras.** La ventaja —sabe operacionalizar, sabe
   desconfiar de la validez aparente— y el estorbo —el reflejo de hacerse cargo—, y el estorbo se dice
   con la misma claridad. Sin la segunda mitad, la primera es adulación.
6. **Lo que no es suyo va marcado [!] con quién decide.** Dos veces en una sola lección.

---

# 13. PRUEBA DE DURABILIDAD

**Procedimiento.** Recorrer el mapa de módulos suponiendo que en agosto de 2028: (a) los productos se
han renombrado al menos una vez —cosa que ya ocurrió tres veces en cinco meses de 2026 con la
automatización nativa de la suite, el cuaderno de fuentes y la herramienta de terminal—; (b) algunas
funciones se han movido de edición o han desaparecido; (c) su empresa ha cambiado de proveedor, o ella
ha cambiado de empresa. Y marcar, módulo a módulo, qué se rompe.

## 13.1 Recorrido, módulo a módulo

| Módulo | Qué es criterio (sigue válido en 2028) | Qué es clic (se rompe) | Coste de reparación |
|---|---|---|---|
| **M0** | El embudo de elección y sus cinco columnas · **la prueba de la sombra y sus tres rechazos** · describir por observación y no por introspección · las cuatro preguntas que definen cualquier plan · «la misma frase es segura o no según con qué cuenta entres» · «pagar resuelve quién es el proveedor, no qué tratamientos están amparados» · el semáforo · el estándar «no lo sé y lo pregunté» vale / «creo que sí» no vale · la lista de 32 procesos | El distintivo concreto de la pantalla · las comprobaciones empíricas · la ruta de la consola · los mensajes literales | **1 fichero de clics.** El criterio no se toca |
| **M1** | La línea de corte y sus tres motivos legítimos · el escalón −1 · la ficha de criterio y su prohibición de palabras · las anclas conductuales · la muestra apartada · la tabla de especificaciones de la batería · el protocolo de siete reglas · el cebo como control positivo | **Nada.** Este módulo no tiene fichero de clics | **Cero** |
| **M2** | Fuente de verdad con **fecha y dueño** · citar como forma de abaratar la revisión · «no lo sé» como respuesta exigible y probable · seudonimización y cuasi-identificadores · la prueba de la compañera · la regla de los adjuntos · el mapa de datos del proceso · el techo de la memoria | Dónde se guarda un asistente, cuántos ficheros admite, cómo se llama la superficie de fuentes | **1 fichero de clics + 1 línea de `tres-nombres.md`** |
| **M3** | Disparador por calendario frente a disparador por suceso · el tope · el apagado probado · «prepara, no envíes» y su motivo · «automatiza donde ya viven tus datos» · **la prueba del caso que NO debe disparar** | Los límites concretos de la plataforma (recursos compartidos, un disparador por flujo, tope de etiquetas) · el catálogo de pasos disponibles | **1 fichero de clics + la lista de seis comprobaciones**, que hay que reescribir con los límites de la plataforma nueva. **Es la reparación más cara del curso** |
| **M4** | Temas prohibidos frente a condiciones de parada · las cinco condiciones y su motivo · «parar no es callarse» · el revisor con nombre y hora · el plan de fallo en cinco pasos · «la confianza no es una salvaguarda» y el riesgo del día 60 · empatía sin admisión · privilegio mínimo | Cómo se implementa una bifurcación y un tope hoy · qué producto está detrás de qué plan · las fechas del marco normativo | **1 fichero de clics + la caja del fondo**, que se revisa entera. Está diseñada para eso: su primera columna son condiciones, no productos. **Y `datos-volatiles.md` para las fechas normativas**, que caducan más rápido que los productos |
| **M5** | Línea base · minutos por unidad · coste completo · las seis amenazas a la validez interna · proceso frente a resultado · cadena causal · prueba ciega · la lectura de la Tira | **Nada.** Es metodología, un cronómetro y una hoja de cálculo | **Cero** |
| **M6** | Fuentes con caducidad y dueño · calendario de revisión · apagado probado · escribir la propia rúbrica y validarla contra un cebo · la prueba del hueco | Los nombres de las herramientas del apéndice opcional | **1 párrafo** |
| **M7** | El número y su método · «qué NO hace» · la demo de tres minutos · la prueba del pasillo · **la semana sin ella** · la ficha de traspaso · las cuatro reglas de arranque · la entrevista de proceso ajeno | **Nada** | **Cero** |

## 13.2 Recuento

| | Módulos | Proporción |
|---|---|---|
| **Sin nada que reparar** (M1, M5, M7) | 3 | 37 % |
| **Reparación de un fichero de clics o un párrafo** (M0, M2, M6) | 3 | 37 % |
| **Reparación media** (M4: clics + revisión de la caja del fondo + fechas normativas) | 1 | 13 % |
| **Reparación cara** (M3: clics + la lista de comprobación de plataforma) | 1 | 13 % |
| **Módulos que habría que rediseñar** | **0** | **0 %** |

Y por instrumento: **el Expediente del proceso no caduca** (una academia de idiomas en 2030 seguirá
emitiendo cartas de visado y contestando leads); **la Tira no caduca**; **el Cuaderno de capas caduca en
ocho líneas** —la línea de techo de cada ficha— por diseño; **la Lista de techos no caduca porque su
tercera columna son condiciones**; **el Cuaderno de evidencias no caduca**; y **la tabla de tres nombres
caduca entera**, y por eso está aislada en una sola página fechada.

**Veredicto: no hay que rediseñar.**

## 13.3 Cuatro cosas que esta prueba obligó a cambiar, y que ya están incorporadas

1. **Los módulos dejaron de titularse por lo que se construye y pasaron a titularse por la capa.** Un
   primer esbozo tenía módulos llamados «El asistente que cita» y «La columna que clasifica sola». Con
   eso, medio índice del curso nacía caducado y —peor— **el índice enseñaba lo contrario que el
   contenido**.
2. **La pregunta fija pasó de ser un cierre de módulo a ser un artefacto con dos mitades obligatorias.**
   En su versión original —«¿qué de esto vale para cualquier proceso y cualquier herramienta?»— es una
   invitación a escribir generalidades. Con la mitad negativa obligatoria se vuelve una operación de
   separación, y es autocorregible contando casillas.
3. **La caja del fondo cambió de eje.** Antes listaba productos con una columna de «cuándo te tocaría».
   Ahora **la fila es la condición** y el producto es el ejemplo de hoy. Con el eje anterior había que
   rehacerla entera cada año; con este, se revisa.
4. **Las fechas normativas salieron del texto y se fueron a `datos-volatiles.md`.** El calendario del
   Reglamento de IA ya se movió una vez en 2026 y volverá a moverse; el estado del marco de
   transferencias a Estados Unidos depende de una sentencia pendiente. **Lo que no cambia son los seis
   principios y la asimetría del Anexo III**, y eso es lo que se queda en el criterio.

## 13.4 Lo que sigue siendo frágil aunque el diseño esté bien

Una prueba de durabilidad que sale limpia del todo es sospechosa. Tres cosas:

- **M3 es el punto débil y no tiene arreglo estructural.** La anatomía de un disparador es durable, pero
  **los límites concretos de una plataforma no son un adorno del módulo: son la mitad del módulo**,
  porque son lo que determina si su buzón compartido se puede tocar o no. Si cambia la plataforma, hay
  que volver a averiguar los límites, y eso no se hereda.
- **La lista de 32 procesos envejece despacio, pero envejece.** Una normativa de extranjería nueva, un
  canal de captación que desaparece, y hay filas que dejan de existir. Sigue siendo el activo más
  duradero del curso, pero conviene fecharla como cualquier otra fuente.
- **Y una asimetría incómoda:** lo que menos caduca de este curso es lo que menos se parece a «un curso
  de IA» —mirar un proceso, escribir criterios, medir, traspasar, contagiar— y lo que más caduca es lo
  que más se parece. Es la mejor prueba de que el listón está bien puesto, y también el motivo por el
  que el material tiene que trabajarse el enganche de M1, M5, M6 y M7 mucho más que el de M3.
