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
