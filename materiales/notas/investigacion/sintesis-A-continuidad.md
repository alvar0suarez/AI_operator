# Síntesis A — Diseño unificado del curso

> **«Un proceso tuyo, de punta a punta»**
> *Siete capas para convertir una tarea que hoy haces a mano en un sistema que otra persona puede usar
> sin ti — y el criterio para saber cuándo no hacerlo.*

**Fecha:** 23.08.2026.
**Fuente de verdad del encargo:** `curso/00-perfil.md`. Manda sobre este documento.
**Documentos que da por leídos:** `01-analisis-referencia.md`; `dominio-academia.md` (P01–P32);
`dominio-rgpd.md` (semáforo, E-01…E-06); `dominio-herramientas.md` (escalones y límites verificados);
`dominio-autodidacta.md` (mecanismos 1–9, protocolo de siete reglas, puntos de caída);
`dominio-psicologia.md` (C1–C13, EP-01…EP-14); las tres arquitecturas candidatas y los cuatro
veredictos de los jueces.

**Marcas:** **[V]** verificado en fuente primaria · **[R]** reconstrucción razonada · **[E]** evidencia
publicada citada en los informes de dominio · **[NV]** no verificable desde fuera · **[!]** decisión
que no es suya y se escala · **[J]** juicio de diseño mío, argumentado y sin respaldo externo.

**Sesgo declarado de esta síntesis.** Ante cualquier disyuntiva, gana lo que reduce el riesgo de
abandono: victoria antes que rigor completo, menos semanas, menos aridez al principio, recompensa
visible pronto. Sin degradar el curso: los cinco objetivos del perfil siguen cubiertos y hay una
sección (§17) donde digo qué he pagado por este sesgo.

---

# 0. LA DECISIÓN DE SÍNTESIS, Y DÓNDE ME APARTO DE LOS JUECES

## 0.1 Qué gana y por qué

**Columna vertebral: `arq-3-proceso.md`.** El curso recorre un proceso suyo por capas.

Dos de los cuatro jueces coronaron `arq-1-escalera` (lentes de autocorrección y de durabilidad), uno
`arq-3` (supervivencia) y uno `arq-2` (encaje con el trabajo real). Elijo `arq-3` y el argumento es
estructural, no de recuento de votos:

> **Lo que hace ganar a arq-1 y a arq-2 en sus lentes son instrumentos, y los instrumentos se
> trasplantan en una página. Lo que hace ganar a arq-3 en la suya es una propiedad de la columna
> vertebral, y no se trasplanta.**

Concretando. La mejor idea de arq-1 —las puertas con condición observable— es un mecanismo de tres
líneas que funciona igual encima de cualquier eje; su segunda mejor idea —las cinco preguntas— es una
ficha; la decisiva para el juez 3 —el tercer registro «cómo reconocerlo en cualquier herramienta»— es
una convención de maquetación. Las mejores de arq-2 —los seis veredictos, la regla del cuatro, la
segunda vuelta, la tabla de tres filas al azar— son formatos. Todas ellas están injertadas abajo.

En cambio, la ventaja de arq-3 —**el artefacto está en producción sobre su mesa desde la semana 1 y el
mundo la corrige cada martes**— es consecuencia directa de que el curso sea un proceso y no un
recorrido ni un inventario. `dominio-autodidacta.md` §3.2 pone la **ejecución real** en el puesto 1 de
nueve mecanismos de corrección, por encima de la batería y muy por encima de la IA correctora. Un
diseño que maximiza el mecanismo 1 durante diecisiete semanas parte con una ventaja que ninguna
rúbrica compensa. Y bajo mi sesgo declarado hay un segundo argumento que pesa igual: **abandonar en la
semana 12 la deja con un sistema funcionando**; abandonar arq-2 en la semana 4 la deja con una hoja de
cálculo, y abandonar arq-1 en la semana 16 —donde su propio autor admite que se detiene la gente— la
deja sin el escalón que corona el curso.

## 0.2 Dónde me aparto de los jueces, y por qué

**(1) Contra el juez 3, mantengo la cuarta columna del embudo — pero reescrita.**
El juez 3 pide no injertarla: dice que codifica un límite concreto de un producto de 2026 dentro de la
mitad de criterio. Tiene razón en la crítica y se equivoca en la conclusión. Los jueces 1 y 4 la
llaman la mejor decisión de diseño del corpus, y es cierto: convierte un muro de la semana 9 en
aritmética de la semana 1. La reparación correcta no es quitarla, es **partirla por la costura
correcta**:

- En la mitad de criterio, la pregunta durable, que hay que hacerle a cualquier herramienta de
  automatización de cualquier año: **«¿sobre qué ficheros puede actuar de verdad esta herramienta, y
  los que yo abro están entre ellos?»** Eso es válido en 2030.
- En `comun/datos-volatiles.md`, fechado: el límite concreto de hoy —falla con unidades compartidas,
  carpetas compartidas y hojas con referencias externas [V]— y el −3 que hoy descalifica.

Así se cobra en la semana 1 sin meter un bug de producto en la mitad que no caduca.

**(2) Contra el juez 4, sostengo que la cobertura multilingüe SÍ se puede añadir a posteriori.**
El juez 4 dice que es un fallo estructural de arq-3: «no se puede añadir cobertura multilingüe si el
hilo elegido es monolingüe». No es cierto en este puesto. Todos sus procesos de volumen son
multilingües por naturaleza (P01: 6–12 idiomas; P18; P20; P27: 10+), así que el embudo no puede
seleccionar un hilo monolingüe salvo que ella lo fuerce. Y aunque lo forzara, tres piezas lo
garantizan por diseño y están abajo: **un caso frontera obligatorio en un idioma minoritario real** en
la batería de M1, **la parada por idioma no probado** como freno obligatorio de M4, y **la tarde de
P27** en M3, que es una clasificación en lote de comentarios en diez idiomas con clave sellada.

**(3) Contra el juez 2, no importo las cinco puertas de arq-1: importo tres.**
Las puertas son su mejor idea y las injerto, pero cinco puertas en un curso sin profesor son cinco
sitios donde parar. Pongo tres, exactamente donde construir sobre arena sale caro (§12.3). Y añado la
regla que arq-1 no escribe: **una puerta cerrada no es un suspenso, es una semana más en la misma
capa, y esa semana está presupuestada** —por eso M4 dura tres semanas y no dos.

**(4) Contra el juez 2 y con el juez 4 a la vez, en la regla del cuatro.** El juez 2 quiere sustituir
la cuota por motivos tipificados; el juez 4 quiere los seis veredictos con su cuota. Se hacen las tres
cosas y se apilan (§9.2): descartes aritméticos por número de proceso (gratis, sin criterio) + **cinco
motivos tipificados contra lista cerrada** + una cuota de cuatro **de la que las zonas prohibidas no
cuentan**, para que los cuatro tengan que salir de los veredictos 1 y 2, que son los que exigen
juicio.

**(5) Contra los cuatro, acorto el curso a diecisiete semanas y a siete módulos.**
Ninguna arquitectura baja de 18. La cola de arq-3 —siete semanas seguidas sin funcionalidad nueva— es
su peor defecto y todos los jueces lo señalan. Fundo «medir» y «dejarlo vivo» en un solo módulo de
tres semanas: la meseta baja de siete semanas a seis y desaparece una frontera de módulo, que es un
sitio menos donde el curso puede leerse como terminado.

**(6) Acepto sin reservas las correcciones obligatorias.** La del juez 4 sobre P08 (§10.4): la
comprobación que caza el nombre mal transcrito **no puede leer el pasaporte**, y la versión admisible
es otra. La del juez 2 sobre los dobletes: **clave sellada**, no solo comprobación formal. Y escribo
la autocrítica (§17), que en arq-3 se citaba siete veces y no existía.

## 0.3 Los injertos, en una tabla

| # | Qué se injerta | De dónde | Dónde entra | Qué repara |
|---|---|---|---|---|
| I1 | **El asistente con tres fuentes verdes**, escalonado al día 4–5 | arq-2 M0 | M0 | Los tres módulos de sequía de artefacto de arq-3 |
| I2 | **Las cinco preguntas** (quién dispara / quién decide los pasos / de dónde saca lo que sabe / qué puede tocar / quién firma) | arq-1 §1.2 | Instrumento 1; cabecera de cada cierre de capa; ejercicio de M4 | El clasificador portátil que arq-3 no tenía |
| I3 | **Los seis veredictos + zona prohibida** como rejilla cerrada del doblete | arq-2 §3.4 | Instrumento 4 | El objetivo 1, «peor servido por este ángulo» según su propia arq-3 |
| I4 | **El Mapa corto (12 veredictos, 20 min) y su segunda vuelta** | arq-2 M1 + M7/M9 | Instrumento 5 | El objetivo 4: 31 juicios en cuatro horas en vez de 8 en tres |
| I5 | **La puerta con uso espontáneo** (≥5 usos sin que el curso lo pida) | arq-1 salvaguarda 4 | Puerta M2→M3 | «El mundo la corrige» es falso si no lo usa |
| I6 | **La columna «lo que sí se puede hacer alrededor»**, con artefacto nombrable | arq-2 Mapa | Línea de corte de M1 | El momento «esto no me sirve para lo que de verdad me duele» |
| I7 | **El tercer registro: «cómo reconocerlo en cualquier herramienta»** | arq-1 §4.1 | Convención de producción (§8) | El hueco de abrir una pantalla que no ha visto nunca |
| I8 | **Independencia de plataforma como restricción de producción** | arq-1 momento 2 | M3 y M4 | Que un administrador pueda romper el curso |
| I9 | **La prueba de traslado nº 2, en notación neutra y sobre papel** | arq-2 M4 | M3 | Agnosticidad en el tramo más específico de plataforma |
| I10 | **El hallazgo a las 48 horas, prometido por escrito** | arq-2 momento 1 | Hoja de sombra, M0 | Convierte el peaje de observar en pago |
| I11 | **Campos «qué otras filas la piden» y «cuándo NO usarla»** | arq-2 ficha de capacidad | Pregunta fija (§4.4) | El monocultivo, riesgo 2 declarado de arq-3 |
| I12 | **Clave sellada para los siete dobletes** | juez 2 | Instrumento 4 | El único mecanismo de transferencia sin oráculo |
| I13 | **Reproducción del número ±10 %** | arq-2 M8 | M5 | Que su medida sea estable, no solo honesta |
| I14 | **Tres filas al azar: «¿la hice esta semana?»** | arq-2 M1 | M0 | Inventario aspiracional |
| I15 | **La tarde de P27** (lote + doble codificación + tabla de confusión, con clave del curso) | arq-1 M3 / arq-2 M3 | M3 | Restaura el mejor mecanismo de nivel 1 y el oráculo escrito por el curso |
| I16 | **Nota [NV] sobre el perfil de competencia de la pareja** | arq-2 §7.3 | §12.5 | Fallo silencioso de un punto de consulta |
| I17 | **Movilidad declarada del módulo de adopción** | arq-1 §3.1 | §13, momento 3 | Un calendario roto leído como curso abandonado |
| I18 | **Regla del embudo vacío** | ninguna: hueco señalado por el juez 1 | M0 | Que el filtro la deje sin candidatos |

---

# 1. NOMBRE Y TESIS

## 1.1 Nombre

> **«Un proceso tuyo, de punta a punta»**
> *Siete capas para convertir una tarea que hoy haces a mano en un sistema que otra persona puede usar
> sin ti — y el criterio para saber cuándo no hacerlo.*

El título no nombra ninguna herramienta, ninguna tecnología y ningún año. El índice del curso tampoco
(§6). Es la primera aplicación de la regla que gobierna todo el material.

## 1.2 Tesis

> **Se aprende haciendo una cosa entera, no doce a medias. Un proceso llevado de punta a punta —hasta
> que funciona, hasta que ella lo usa sin que nadie se lo pida y hasta que sobrevive a sus
> vacaciones— enseña más criterio que doce diagnósticos sobre papel, porque es el único formato en el
> que cada decisión recibe la respuesta del mundo.**
>
> Y el corolario que lo convierte en arquitectura: **el curso no la sube por una escalera de
> herramientas. La escalera aparece sola, por debajo, porque un proceso al que aprietas va pidiendo
> cosas en ese orden.** Primero pide que alguien escriba qué es hacerlo bien. Después, contexto que no
> haya que volver a explicar. Después, dejar de depender de que ella se acuerde. Después, juicio en
> dos sitios y frenos en otros tres. Después, que alguien compruebe si de verdad sirve. Y al final,
> poder existir sin ella.

Cuatro corolarios operativos, y los cuatro son restricciones de diseño, no lemas:

**(a) La unidad del curso es la capa, no la herramienta ni la tarea.** Un módulo se llama «Que ocurra
sin que lo pidas», nunca «Acciones programadas». La capa es anatomía; la herramienta es la
implementación de hoy y vive en un fichero aparte y fechado.

**(b) La teoría entra cuando el proceso la pide, y solo la que pide.** No hay módulo de panorama ni
catálogo previo. Lo que el proceso no pide se cubre con veinte minutos en seco —el Doblete— o no se
cubre, y se dice dónde.

**(c) El «no» vive dentro del proceso, no fuera.** El primer entregable serio no es «qué automatizo»
sino **la línea de corte**: qué trozos entrego, qué trozos se quedan conmigo y por qué. Un proceso
partido en trozos con veredicto es el sitio más barato del mundo para aprender que a veces la
respuesta es que no.

**(d) El criterio portátil no se predica: se extrae con un ritual y se mide dos veces.** Se extrae al
cerrar cada capa con una pregunta fija de dos mitades obligatorias, y se **mide** comparando su
clasificación de doce tareas propias en la semana 1 con la misma clasificación en la semana 17. El
objetivo 4 del perfil deja de ser una promesa y pasa a ser una tabla con dos columnas y un delta.

## 1.3 El límite de la tesis, dicho en la misma página

**Funcionar no es estar bien.** El uso diario detecta que algo molesta; no detecta que el criterio
estaba mal escrito ni que la batería era fácil. **El mundo corrige la utilidad; los instrumentos
corrigen el criterio.** Por eso el aparato de §12 —batería con clave sellada, listas binarias,
rúbricas negativas, tres cebos, tres puertas— está entero y no se adelgaza por tener un artefacto en
producción.

Y el segundo límite, que es el riesgo del ángulo: **un solo proceso puede no dar ocasión de practicar
todo el criterio.** Contra eso hay tres contramedidas con nombre —el Mapa corto y su segunda vuelta,
los siete dobletes con clave sellada, y la tarde de P27— y el saldo honesto está en §17.

---

# 2. PERFIL DE ENTRADA Y DE SALIDA

## 2.1 Entrada, sin adornos

| | |
|---|---|
| **Formación** | Licenciatura en Psicología. Sin base técnica. Nunca ha abierto una terminal |
| **Puesto** | Atención al cliente en una academia de español para extranjeros de ~30 empleados en Madrid, con alojamiento de larga estancia. Jornada completa |
| **Uso actual de IA** | ChatGPT, Claude y Gemini **como chat**: entra, escribe, lee, copia. No diseña procesos, no construye nada, no conoce el uso agéntico |
| **Entorno** | Su empresa paga Gemini y lo recomienda como estándar. **No sabe qué plan tienen ni cómo está configurado** |
| **Apoyo** | Autodidacta. Pareja con conocimientos de IA para consultas puntuales: no corrige entregas ni sigue el progreso |
| **Lo que ya tiene a favor** | Es la experta del dominio: sabe cosas de ese trabajo que no están escritas en ningún sitio de la empresa. Y sabe operacionalizar, diseñar instrumentos y evaluar si algo mide lo que dice medir |
| **Lo que su formación NO le da** | Montar un flujo. Que el paso 3 no ve lo que produjo el paso 1 salvo que se lo pases. Eso es nuevo, se aprende haciendo, y le va a costar los dos primeros intentos |

## 2.2 Salida, definida como conductas y no como conocimientos

Al terminar, y esto es lo que se puede observar sin creerla:

1. **Tiene un proceso suyo funcionando** —con disparador, frenos, revisor con nombre y apagado
   probado— **y lo usa a diario sin que el curso se lo pida**.
2. **Sabe decir qué ahorra y con qué método lo midió**, con la revisión restada y con una amenaza a la
   validez que no puede descartar. Y el número se le vuelve a salir igual dos semanas después.
3. **Clasifica cualquier herramienta que le pongan delante** —incluida una que el curso no le enseñó y
   una que no existe hoy— con las cinco preguntas, y **deriva de ahí qué salvaguardas necesita y qué
   datos no le puede meter**.
4. **Clasifica un proceso cualquiera** —suyo, de una compañera o de otra empresa— en uno de seis
   destinos, dos de los cuales son «aquí no metas IA», con el motivo elegido de una lista cerrada de
   cinco.
5. **Sabe qué no debe tocar y por qué**, en forma transferible: no una lista de prohibiciones, sino
   cinco motivos que se aplican a un caso nuevo.
6. **Ha entregado su sistema a otra persona**, que lo usó una semana entera sin ella, y ha arreglado lo
   que ese piloto reveló.
7. **Escribe la rúbrica de un artefacto suyo** con al menos tres criterios negativos, y la valida
   contra un cebo. Ese es el indicador honesto de que ya no necesita el material.

Y lo que **no** es la salida, escrito porque es la deriva natural: no es AI specialist, no es cambio
de rol, no es portfolio, no es una colección de herramientas, y no es «la de la IA» de la academia.

---

# 3. RESULTADOS DE APRENDIZAJE OBSERVABLES

Verbos de desempeño. Ninguno dice «entenderá», «conocerá» ni «será capaz de valorar». Cada uno con su
evidencia observable y el módulo donde se cierra.

| # | Al terminar, ella… | Evidencia observable | Cierra en |
|---|---|---|---|
| **RA1** | **Elige** un proceso propio para delegar aplicando criterios de rechazo observables, y **descarta** por escrito los que no pasan, con el motivo | Hoja de elección: 32 procesos tachados, seis descartes aritméticos, 6–8 candidatos puntuados en cinco columnas, dos días de hoja de sombra | M0 |
| **RA2** | **Describe** un proceso suyo como se ejecuta de verdad —disparador, documentos, decisiones no escritas, salida— **sin escribirlo de memoria** | La descripción contiene **al menos dos decisiones que no estaban en su idea previa del proceso** | M0 |
| **RA3** | **Clasifica** doce tareas suyas en seis destinos + zona prohibida, y **repite la clasificación** cuatro meses después marcando qué ha cambiado y por qué | Mapa corto (sem. 1) + segunda vuelta (sem. 17) + una frase por cada veredicto que cambió | M0 → M6 |
| **RA4** | **Determina** bajo qué régimen de datos trabaja —plan, licencia, retención, política escrita— **o documenta** a quién y cuándo lo preguntó | Ficha del entorno, ocho casillas, **ninguna frase que empiece por «creo que»** | M0 |
| **RA5** | **Traza la línea de corte** de su proceso: qué entrega, qué se queda con ella, con el motivo elegido de una lista cerrada, **y qué sí se puede hacer alrededor de cada «no»** | Al menos un trozo se queda con ella; ningún motivo es «es difícil»; cada «no» lleva un artefacto **nombrable** al lado | M1 |
| **RA6** | **Escribe** el criterio de «resultado correcto» en 4–6 indicadores que otra persona pueda comprobar sí/no contra una fuente, **antes** de tocar ninguna herramienta | Ficha de criterio de una cara, sin *adecuado, correcto, natural, profesional, de calidad* sin ancla detrás | M1 |
| **RA7** | **Construye** una batería de diez casos —5 típicos, 3 límite, 2 de rechazo, **uno de ellos en un idioma minoritario real de su trabajo**— apartados antes de escribir el prompt, y **la vuelve a pasar con fecha** en cada capa | La Tira: una columna por capa, con fecha, seis columnas al terminar | M1 → M5 |
| **RA8** | **Sitúa** cada dato que atraviesa su proceso en verde/ámbar/rojo, **marca en qué paso entra y en cuál hay que quitarlo y quién lo quita**, y **reescribe** tres casos reales que sobreviven a la prueba de la compañera **y siguen sirviendo** | Mapa de datos del proceso (una cara) + 3 casos reescritos útiles + 1 declarado no reescribible | M2 |
| **RA9** | **Monta** un asistente con fuentes propias fechadas que **cita el documento y su fecha** y **responde «no lo sé»** a lo que está fuera de alcance | 5/5 en típicos · pide aclaración en los 3 límite · «no lo sé» en los 2 de rechazo | M2 |
| **RA10** | **Reconstruye** una capa suya en otra herramienta y **nombra** qué viajó tal cual, qué hubo que rehacer y qué techo cambió | Ficha de traslado, tres columnas rellenas con cosas concretas | M2 |
| **RA11** | **Monta** algo con disparador que **prepara, clasifica o avisa y nunca envía**, con tope, y **lo apaga habiéndolo probado** | Cinco casos fabricados disparan y producen las cinco salidas correctas; **un sexto que NO debe disparar** no dispara; el apagado está hecho, no imaginado | M3 |
| **RA12** | **Aplica un criterio escrito a decenas de unidades de golpe** y **compara su propia codificación con la del sistema** construyendo la tabla de confusión | ≥26/30 de acuerdo · una frase por cada confusión repetida · acuerdo de la categoría minoritaria mirado aparte · <15 % en «sin clasificar» y **no 0 %** | M3 |
| **RA13** | **Describe cualquier sistema con las cinco preguntas** —incluido uno que el curso no le ha enseñado— y **deriva** qué salvaguardas necesita y qué datos no puede meterle | Ficha de cinco preguntas rellenada para una herramienta que el curso no enseñó | M4 |
| **RA14** | **Distingue** en su proceso qué parte tiene pasos fijos y qué parte necesita juicio, y **argumenta por qué un agente autónomo sería exceso aquí** | Media página con la frontera trazada y los dos puntos de juicio nombrados | M4 |
| **RA15** | **Escribe** temas prohibidos y condiciones de parada y **las prueba con casos fabricados que deben parar**, incluida **la parada por idioma no probado** | Cinco casos de parada, cinco paradas vistas; el sexto, normal, no para; el revisor es **una persona con nombre y una hora** | M4 |
| **RA16** | **Reconoce** cuál es el único proceso de su academia que caería en el Anexo III del Reglamento de IA y **a quién lo escala** | Una frase, un nombre, un puesto | M4 |
| **RA17** | **Audita a su propio corrector** con artefactos-cebo de defectos plantados y **decide con ese dato** si la IA sirve para corregir ese tipo de trabajo | Hoja de resultado de los tres cebos + decisión escrita + **al menos un caso registrado en que NO aceptó una crítica de la IA, con el motivo** | M1, M4, M6 |
| **RA18** | **Mide** el efecto de su sistema en minutos por unidad, **resta** revisión y mantenimiento, **nombra** una amenaza a la validez que no puede descartar, y **reproduce el número** dos semanas después | Media página sin la palabra «significativo», con la resta hecha; recálculo dentro de ±10 % | M5 |
| **RA19** | **Deja el sistema en condiciones de sobrevivirle**: fuentes con fecha y dueño, calendario de revisión, apagado probado, ficha de traspaso | La ficha responde con **nombre propio** a «quién lo mantiene» y con **fecha** a «cuándo caduca cada fuente» | M5 |
| **RA20** | **Entrega** su artefacto a otra persona que lo usa **cinco días laborables sin ella**, y **corrige** lo que el piloto revele | Ficha de traspaso + **lista de al menos dos cosas que hubo que arreglar** | M6 |
| **RA21** | **Explica** en treinta segundos, **sin nombrar ninguna herramienta**, qué hace su sistema, qué ahorra y **qué no hace** | La prueba del pasillo, con alguien que no ha visto el artefacto, y sus cuatro comprobaciones binarias | M6 |
| **RA22** | **Contesta la pregunta fija** al cerrar cada capa, con sus dos mitades, y **firma siete dobletes** de los cuales **al menos tres terminan en «no aplica» o «no compensa»**, contrastados contra clave sellada | Cuaderno de capas: siete cierres con las ocho casillas rellenas y siete dobletes con veredicto y contraste | todos |
| **RA23** | **Escribe la rúbrica** de un artefacto suyo con ≥3 criterios negativos y **la valida contra un cebo** | Si el cebo pasa su rúbrica, la rúbrica es blanda y se rehace | M6 |

**Criterio de «curso terminado», fijado en la semana 1 y observable:**

> **Un proceso suyo en producción y en uso diario sin que el curso se lo pida · un número medido con su
> método y reproducido a las dos semanas · siete preguntas fijas contestadas con sus dos mitades ·
> tres dobletes terminados en «no aplica» · un Mapa corto con su segunda vuelta y su delta explicado ·
> una rúbrica escrita por ella y validada contra un cebo · y una segunda persona que ha usado su
> sistema cinco días laborables sin ella delante.**

No es «leer la última lección». RA23 es el indicador honesto de que ya no necesita el material.

**Los dos que hacen falsable la agnosticidad**, y hay que decirlo con las peores palabras: si al
terminar no puede rellenar la ficha de cinco preguntas para una herramienta que el curso no enseñó
(RA13) y no puede reconstruir una capa suya en otro sitio (RA10), **entonces el curso fue un curso de
una herramienta y fracasó**, por muy bien que hayan salido los demás resultados.

---

# 4. LOS SEIS INSTRUMENTOS PERMANENTES

Van antes del mapa de módulos porque todos los módulos cuelgan de ellos. Son seis objetos que viven
más allá de las diecisiete semanas. **Por qué exactamente seis: cada uno sirve a un objetivo distinto
del perfil, y el sexto sirve al que ninguno de los otros cinco cubría.**

| # | Instrumento | A qué objetivo del perfil sirve | Por qué sobrevive al curso |
|---|---|---|---|
| 1 | **Las cinco preguntas** | 1 (saber qué existe) y 3 (datos) | Clasifica por autonomía cedida, que es una propiedad de cualquier sistema, no un catálogo de productos |
| 2 | **El Expediente del proceso** | 2 (automatizar lo suyo) | Es el sistema, no documentación sobre el sistema |
| 3 | **La Tira** | 2 y 4 | Es una medición de su propio trabajo con fecha; no depende de ninguna herramienta |
| 4 | **El Cuaderno de capas** (pregunta fija + doblete) | 4 (criterio portátil) | Es el curso entero escrito en su lenguaje y sin nombres de producto |
| 5 | **El Mapa corto y su segunda vuelta** | 1 y 4 | Convierte el criterio panorámico en una tabla con delta medible |
| 6 | **La Lista de techos** | 1 | Es un catálogo cuya tercera columna son condiciones, y las condiciones no se renombran |

Y un séptimo objeto que no es un instrumento sino un hilo de dos minutos: **el Cuaderno de evidencias**
(§11.3).

---

## 4.1 Instrumento 1 · LAS CINCO PREGUNTAS *(injerto I2, de arq-1 §1.2)*

| # | Pregunta | Respuestas, de menos a más autonomía cedida |
|---|---|---|
| **1** | **¿Quién dispara?** | yo, cada vez · un reloj · un suceso · lo decide el sistema |
| **2** | **¿Quién decide los pasos?** | yo, sobre la marcha · yo, de antemano, y quedan fijos · el sistema, sobre la marcha |
| **3** | **¿De dónde saca lo que sabe?** | de lo que le pego en el momento · de fuentes que yo controlo y fecho · de donde quiera |
| **4** | **¿Qué puede tocar?** | nada · leer lo que yo le doy · leer todo lo que yo puedo leer · escribir en lo mío · escribir hacia fuera |
| **5** | **¿Quién firma la salida?** | yo, siempre · yo, por muestreo · nadie |

**Por qué estas cinco y no otras, y por qué son el instrumento número uno.** Porque son las únicas que
cambian de respuesta al subir de capa, porque las respuestas **se observan y no se opinan**, y porque
—y esto es lo que las hace insustituibles— **las preguntas 4 y 5 son literalmente protección de datos
y salvaguardas**. El régimen de datos no va pegado al final del curso: está dentro del instrumento con
el que se clasifica cualquier herramienta. Quien contesta las cinco ya sabe qué salvaguardas necesita.

**Cómo se usan en este curso, y son tres usos:**

1. **Cabecera del cierre de cada capa.** Se rellena la tabla completa; **normalmente cambia una sola
   fila, y ver cuál cambia es la lección.** Coste: tres minutos.
2. **Ejercicio de M4:** rellenarlas para **una herramienta que el curso no ha enseñado**, leyendo su
   documentación quince minutos. Es RA13 y es la prueba de que el instrumento funciona sin el curso.
3. **Cierre obligatorio de cada ficha de la Lista de techos**, porque las preguntas 4 y 5 obligan a
   declarar por escrito sobre qué recursos actúa un sistema — que es exactamente el punto ciego que el
   juez 4 detecta en los diseños de inventario.

**La propiedad que hay que decirle en la semana 1:** el día que un solo producto haga todo —chat,
disparo, flujo y agente en la misma ventana, que es la tendencia— **estas preguntas no sobran: hacen
más falta**, porque el producto deja de forzar la distinción y ya nada, salvo el criterio, le dice
cuánta autonomía acaba de ceder.

---

## 4.2 Instrumento 2 · EL EXPEDIENTE DEL PROCESO

Una carpeta con el nombre de su proceso. **No es documentación: es el sitio donde el proceso vive.**
Cada capa deja dentro exactamente una cosa, y esa lista es el índice del curso.

```
expediente-<mi-proceso>/
  00-como-se-hace-de-verdad.md      ← capa 0: disparador, documentos, decisiones no escritas, salida
  00-hoja-de-sombra.md              ← capa 0: los dos días de observación, en crudo
  01-linea-de-corte.md              ← capa 1: qué entrego, qué se queda conmigo, motivo, y el «sí» de al lado
  01-ficha-de-criterio.md           ← capa 1: 4-6 indicadores observables, críticos marcados
  01-casos.md  +  01-CLAVE.md       ← capa 1: la batería, y su clave SELLADA
  02-mapa-de-datos.md               ← capa 2: qué dato entra, en qué paso, dónde hay que quitarlo, quién lo quita
  02-fuentes/                       ← capa 2: cada fuente con FECHA y DUEÑO en la primera línea
  03-disparador.md                  ← capa 3: qué lo lanza, con qué tope, cómo se apaga
  04-frenos.md                      ← capa 4: temas prohibidos, condiciones de parada, quién revisa y a qué hora
  05-evaluacion.md                  ← capa 5: antes, después, coste completo, amenaza no descartada
  05-traspaso.md                    ← capa 6: dueño, caducidades, calendario de revisión, apagado probado
  la-tira.md                        ← la batería pasada en cada capa, una columna por fecha
  cuaderno-de-capas.md              ← 7 cierres + 7 dobletes
  evidencias.md                     ← 3 líneas por capa, para M6
```

**Regla de la primera línea, que aparece en la capa 2 y no se abandona nunca:** todo fichero de
`02-fuentes/` empieza con dos datos — **de cuándo es** y **quién manda sobre él**. Sin eso, un cuaderno
con las condiciones de cancelación del año pasado responde con las del año pasado, con toda la
confianza del mundo y citando el documento. La cita no protege de eso; la fecha, sí.

**Por qué una carpeta y no un documento.** Porque el entregable no es un informe: es un sistema con
partes que se tocan por separado y caducan a ritmos distintos. Y porque el día que otra persona lo
herede (M5, M6), lo que se entrega es esta carpeta y nada más.

---

## 4.3 Instrumento 3 · LA TIRA

Diez casos escritos en M1 y **nunca cambiados**, pasados al cerrar cada capa, con una columna nueva y
fechada por capa.

```
CASO                          | como lo hago hoy | +criterio | +fuentes | +disparador | +frenos
                              | 13-oct           | 27-oct    | 10-nov   | 24-nov      | 15-dic
------------------------------|------------------|-----------|----------|-------------|--------
T1  típico                    |  SÍ              |   SÍ      |   SÍ     |    SÍ       |   SÍ
T2  típico                    |  NO              |   SÍ      |   SÍ     |    SÍ       |   SÍ
T5  típico, en neerlandés     |  NO              |   NO      |   SÍ     |    SÍ       |   SÍ
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

> Entre la tercera y la sexta columna **la calidad apenas se mueve**. Casi toda la calidad se gana en
> la capa 1 y la capa 2 —cuando alguien escribe qué es hacerlo bien y le da fuentes con fecha— y a
> partir de ahí solo se puede perder. Lo que cambia al añadir capas no es la calidad: es **quién
> dispara, cuánto tarda y cuánta autonomía has cedido.**

Si dentro de tres años le ponen delante una herramienta que hoy no existe, la pregunta que sabrá hacer
es *«¿esto me cambia la calidad o me cambia el disparador?»*. Y no se la habrá contado nadie: la habrá
deducido de seis columnas de su propio trabajo.

**Tres reglas que la sostienen:**

1. **Los casos se escriben ANTES de construir nada**, y por muestreo cronológico, no elegidos. Si se
   escriben después, se escriben para que pasen. Ella reconocerá la operación con su nombre: es
   preregistro.
2. **La clave va sellada** en un fichero aparte, escrito el mismo día, que no se reabre hasta anotar
   los resultados de cada pasada.
3. **Uno de los diez casos está en un idioma minoritario real de su trabajo** —neerlandés, turco,
   coreano, polaco—, **nunca en inglés, que es el fácil**. Es la salvaguarda multilingüe más barata
   que existe y va escrita como requisito, no como sugerencia.

**El riesgo de este instrumento, dicho aquí:** es trabajo sin novedad, media hora cada tres semanas, y
lo que no tiene novedad se convierte en ritual o desaparece. La contramedida es que **el cierre de
módulo no está permitido sin la columna nueva**: es un ítem binario de la lista de comprobación y una
de las tres puertas lo comprueba. Aun así es el punto frágil que reconozco en §17.

---

## 4.4 Instrumento 4 · EL CUADERNO DE CAPAS

Siete entradas de una cara. Cada entrada tiene tres partes: la tabla de las cinco preguntas, la
pregunta fija y el doblete.

### 4.4.1 La pregunta fija, con la regla de las dos mitades

```
CIERRE DE LA CAPA __ · fecha ____

A · LAS CINCO PREGUNTAS       (marca la fila que ha cambiado hoy)
   1 ¿quién dispara? ______   2 ¿quién decide los pasos? ______
   3 ¿de dónde saca lo que sabe? ______   4 ¿qué puede tocar? ______
   5 ¿quién firma la salida? ______

B · LA PREGUNTA FIJA          (seis casillas, todas obligatorias)
   1 PROCESO      Vale para cualquier proceso la parte de: __________
                  Era de ESTE proceso la parte de: __________
   2 HERRAMIENTA  Valdría con cualquier herramienta la parte de: __________
                  Era de ESTA herramienta la parte de: __________
   3 TECHO        Esta capa NO puede: __________
                  Lo que lo rompería sería una cosa del tipo: __________

C · LAS DOS CASILLAS CONTRA EL MONOCULTIVO      ← injerto I11, de arq-2 §3.2
   4 ¿Qué OTRAS filas de mi Mapa corto pedirían esta capa? (con su número de proceso)
   5 ¿CUÁNDO NO usar esta capa? (la situación en la que es exceso, y qué usar en su lugar)
```

**La regla que la hace autocorregible:** cada respuesta de B tiene una mitad positiva y una negativa, y
**las dos son obligatorias**. Si escribe que todo vale para todo, no ha separado nada: ha resumido. Si
escribe que nada vale fuera de aquí, tampoco. La comprobación es binaria y de cinco segundos:
*¿están rellenas las seis casillas de B y las dos de C? SÍ/NO*.

**Y una comprobación que caza el error más común al escribir un techo** *(injerto de arq-2)*:
*¿la casilla 3 dice algo que la CAPA no puede hacer, y no algo que ella todavía no sabe hacer? SÍ/NO*.
Esa distinción —no-puede frente a no-sé-todavía— es la que convierte un techo en diagnóstico en vez de
en queja, y es lo que le permitirá depurar una herramienta que no ha visto nunca.

**Destino de cada parte:** la casilla 1 alimenta el doblete · la 2 es el mecanismo de agnosticidad,
contestado siete veces por escrito · la 3 construye la Lista de techos · la 4 rompe el monocultivo · la
5 es la vacuna contra el «todo con IA».

### 4.4.2 El Doblete, con los seis veredictos y con clave sellada *(injertos I3 e I12)*

Al cerrar cada capa, **veinte minutos, sobre papel**, aplicando la misma capa a un proceso que no es el
suyo. No se construye nada.

```
DOBLETE de la capa __ · proceso P__ · fecha ____ · 20 min

1. Si tuviera que aplicar esta capa aquí, ¿qué haría exactamente? (3-5 líneas)
2. ¿Qué cambiaría respecto a lo que hice en mi proceso?
3. ¿Hay algo de esta capa que aquí NO tendría sentido? ¿Por qué?

4. VEREDICTO — uno solo:
   [1] ni IA                        [4] asistente con fuentes
   [2] arreglar el proceso primero  [5] disparador y pasos fijos
   [3] chat, mejor usado            [6] flujo con juicio
   [ZP] zona prohibida — es un tachón encima del veredicto que hubiera

5. MOTIVO — elegido de la lista cerrada, no redactado libre:
   [ ] riesgo: el error lo paga un cliente, una administración o la caja
   [ ] conocimiento que caduca más deprisa de lo que puedo mantener el artefacto
   [ ] no hay fuente de verdad: nadie puede nombrar el documento vigente ni su dueño
   [ ] las reglas son de otro: el procedimiento lo fija una institución ajena
   [ ] no necesita un modelo: necesita una fórmula, una plantilla o un calendario

6. → ABRIR LA CLAVE SELLADA de este doblete. ¿Coincide el veredicto? ¿Y el motivo?
   Si no coincide: ¿en qué me he apoyado yo que la clave no usa, o al revés?
```

**Por qué la rejilla cerrada y no un veredicto libre.** Un veredicto libre («aplica / aplica con
cambios / no aplica») produce una frase; una rejilla de seis destinos produce **una clasificación
reutilizable**, que es exactamente lo que el objetivo 4 pide y lo que arq-3 servía peor. Cuesta cero
minutos extra.

**Por qué la clave sellada.** Es la corrección que el juez 2 exige y tiene razón: sin ella, el
mecanismo con el que se transfiere el criterio a procesos ajenos no tiene oráculo, y comprobar «¿hay
veredicto firmado? SÍ/NO» es comprobar la forma, no la función. Las respuestas correctas ya están
razonadas; sellarlas cuesta un fichero.

**La regla de los tres noes, defendida como cuota:**

> **De los siete dobletes, al menos tres tienen que terminar en «no aplica» o en «aplica pero no
> compensa». Si tienes menos de tres, no has transferido: has repetido.**

Cruzando los 32 procesos con lo que la plataforma puede hacer de verdad, el reparto real da entre
cinco y siete noes por cada doce procesos. Tres de siete es un suelo prudente. Su función es
psicológica: **convierte el «no» en algo que hay que encontrar**, y desactiva de raíz el sesgo que
produce un curso de IA por su mera existencia.

### 4.4.3 Los siete dobletes, asignados para que cada capa choque con un tipo distinto de «no»

| Capa | Doblete | Clave sellada: veredicto y motivo | Qué enseña |
|---|---|---|---|
| 0 · Ver el proceso | **P29** emergencias 24 h | **ZP** · riesgo | Describir un proceso **no** compromete a delegarlo. Se mapea para **no** delegarlo |
| 1 · Criterio y corte | **P02** presupuestos | **1** · no necesita un modelo | Escalón −1. Meter un modelo aquí no es ineficiente: **es introducir un error posible donde no lo había** |
| 2 · Contexto | **P08** carta de aceptación para visado | **ZP** · conocimiento que caduca | *No metas conocimiento volátil dentro de un artefacto.* El motivo transferible vale para cualquier dominio |
| 3 · Disparador | **P30** parte semanal *(20 min)* + **P16** exámenes oficiales *(10 min)* | **5** · —  /  **5** · las reglas son de otro | Que «automatizar» no significa «meter un modelo». Y que hay procesos cuyas reglas y plazos los fija el Instituto Cervantes, no la academia |
| 4 · Juicio y frenos | **P28** respuesta a reseñas online | **6 con tachón de publicación** · riesgo | Que un freno puede venir de un sitio que no es la calidad del texto: confirmar públicamente que alguien fue alumno **ya es una cesión de datos** |
| 5 · Medir y traspasar | **P12** check-in del lunes *(20 min)* + **P32** plantillas y FAQ *(20 min)* | **no se deja medir** · deficiencia del criterio  /  **2** · no hay fuente de verdad | Que hay valor que no cabe en minutos por unidad. Y que a veces el problema no es que falte automatización: **es que falta una fuente de verdad** |
| 6 · Que lo adopten | **el proceso de una compañera** | — (no hay clave: es una entrevista) | La capa 0 aplicada a un proceso ajeno, con su dueña delante. Semilla de contagio |

Siete dobletes × veinte minutos ≈ **dos horas y media en diecisiete semanas**. Cubren nueve procesos y
cuatro clases distintas de «no». No sustituyen a los treinta juicios de una arquitectura de inventario
—para eso está el instrumento 5—, pero cada uno se emite **inmediatamente después de haber hecho esa
misma cosa de verdad**, que es cuando un juicio sobre un proceso ajeno vale algo.

---

## 4.5 Instrumento 5 · EL MAPA CORTO Y SU SEGUNDA VUELTA *(injerto I4)*

**Es la pieza nueva de esta síntesis y la que repara el peor defecto de la columna vertebral
elegida.** [J]

El juez 3 tiene razón cuando dice que el criterio panorámico es una operación entrenada por repetición
y que ocho dobletes son pocos. El juez 1 tiene razón cuando dice que cuatro semanas de Semanario
árido en el tramo de máxima mortalidad matan el curso. **Las dos cosas son ciertas y no se contradicen:
lo que hay que abaratar no es el número de juicios, es el coste de cada juicio.**

### Pasada 1 — semana 1, veinte minutos, dentro del embudo

Sobre los 32 procesos de `dominio-academia.md` que el curso le entrega ya escritos, y que su primera
operación es **tachar** —lo que no ocurre en su academia, lo que no lleva ella— y **corregir**
volúmenes:

1. Marca con un palote los que ha hecho **esta semana**.
2. Coge las **doce filas con más palotes**.
3. A cada una le pone **una letra**: 1, 2, 3, 4, 5, 6 o ZP. **Sin justificar. Sin pensarlo mucho.**
4. Firma y fecha.

**Y el material lo enmarca así, que es lo que lo hace funcionar:**

> *«Esta clasificación va a estar mal en varios sitios y da igual. No es un entregable: es una medida
> de dónde está hoy tu criterio, tomada antes de que el curso lo toque. En la semana 17 vas a
> clasificar las mismas doce filas otra vez y vas a comparar. La diferencia entre las dos columnas es
> la única prueba objetiva que vas a tener de que este curso te ha cambiado la forma de mirar un
> proceso — y la vas a tener porque hoy has gastado veinte minutos, no porque yo te lo diga.»*

Es un pretest y ella lo reconoce por su nombre. Coste real: veinte minutos. Coste emocional: cero,
porque está declarado que estará mal.

### Pasada 2 — semana 17, cuarenta minutos, dentro de M6

Las mismas doce filas, la misma rejilla, **sin mirar la primera pasada hasta haber terminado**. Y
después:

- Se ponen las dos columnas al lado.
- Por cada veredicto que ha cambiado: **una frase con el motivo del cambio**, elegido de la lista
  cerrada de cinco motivos.
- Por cada veredicto que **no** ha cambiado y sobre el que hoy tiene más confianza: **una frase con lo
  que ahora sabe que antes no sabía**.

**Qué produce, y son tres cosas de valor distinto:**

1. **El delta es el objetivo 4 hecho observable.** No «ha adquirido criterio portátil»: doce filas, X
   cambios, con motivo tipificado.
2. **La lista de lo que decidió no automatizar**, que es el entregable de credibilidad de M6 y sale de
   aquí sin trabajo extra: son las filas con veredicto 1, 2 y ZP.
3. **La cola de lo siguiente**, que es lo que hará después del curso: las filas con veredicto 4, 5 o 6
   que no eran su hilo.

### Las tres comprobaciones del Mapa corto, todas binarias

- *¿Hay alguna de las doce filas con **cero palotes**? SÍ/NO* → si sí, es aspiracional.
- **La comprobación de las tres filas al azar** *(injerto I14)*: coger tres filas al azar y preguntarse
  *«¿la hice esta semana?»*. Si la respuesta es no en alguna, **el inventario es aspiracional y hay que
  volver a contar palotes**. Treinta segundos, y es la que más caza.
- *¿Hay al menos **cuatro** veredictos 1 o 2, **sin contar las zonas prohibidas**? SÍ/NO* → §9.2.

---

## 4.6 Instrumento 6 · LA LISTA DE TECHOS

No se lee: **se escribe**, una fila al cerrar cada capa, a partir de la casilla 3 de la pregunta fija.
Tres columnas, y la tercera es la que convierte un catálogo en criterio.

| Lo que esta capa no puede hacer | La clase de cosa que sí podría | Qué tendría que cambiar para que me tocara |
|---|---|---|
| Una descripción de un proceso **no hace el trabajo** | Nada: es el punto de partida | — |
| Un criterio escrito **no produce respuestas**; solo permite juzgarlas | Un asistente con ese criterio dentro | Nada: eso es la capa siguiente. *(Fila tachada en la capa 2)* |
| Un asistente guardado recuerda sus instrucciones, **no recuerda lo que pasó ayer** | Un sistema con memoria persistente y auditable | Que necesitara continuidad entre sesiones **y** pudiera comprobar qué recuerda. Hoy no puedo auditarlo, así que no me fío |
| Un disparador por horario **no reacciona a que haya pasado algo** | Un disparador por suceso | Nada: eso es la capa siguiente. *(Fila tachada en la capa 3)* |
| Mi automatización **no puede tocar los ficheros compartidos** de la academia | Automatización externa, o un permiso delegado sobre el recurso compartido | Que alguien me delegue una etiqueta o carpeta propia dentro del buzón compartido, **o** que el flujo tenga que tocar algo fuera de esta suite |
| Un flujo con juicio **sigue siendo un camino que dibujé yo** | Un agente: le das el objetivo y los límites y decide los pasos | Que aparezca una tarea cuyos pasos no pueda dibujar de antemano **y** que exista un plan que lo incluya **y** que los datos lo permitan. Hoy fallan las tres |
| Nada de lo mío **procesa decenas de ficheros locales de golpe** | Un agente con acceso al sistema de ficheros | Una tarea repetida del tipo «revisar 200 contratos de estancia larga buscando una cláusula» |
| Medir dice si sirve hoy, **no si seguirá sirviendo cuando cambie el tarifario** | Un calendario de revisión y un dueño | Nada: eso es la capa siguiente. *(Fila tachada en la capa 6)* |

**Cuatro propiedades que hacen que esto no muera:**

1. **La tercera columna no caduca.** Un catálogo dice qué hay; esta columna dice bajo qué condición
   cambiaría su decisión. «Tocar algo fuera de esta suite» seguirá siendo verdad cuando todo se llame
   de otra manera.
2. **Cada fila se escribe en el momento en que el proceso choca con el techo**, no en un módulo de
   panorama. La fila del agente se escribe en la capa 4, cuando ya tiene un sistema con juicio en dos
   puntos y entiende exactamente qué le falta. Antes de eso, «agente» es una palabra; ahí es una
   carencia concreta con nombre.
3. **La escribe ella.** Un fichero copiado no se relee; uno escrito, sí.
4. **Tachar una fila es un ejercicio.** Cuando la capa siguiente rompe el techo anterior, se tacha con
   fecha. La lista se lee al final como el registro de por dónde ha ido subiendo, y **eso es
   exactamente el objetivo 1 del perfil servido sin catálogo muerto**.

---

# 5. EL PROYECTO HILO

## 5.1 Qué proceso, y por qué se elige en la semana 1 pese al riesgo

El proceso lo elige ella en la semana 1, con un embudo de noventa minutos. La objeción es evidente y
hay que mirarla de frente: **es cuando menos criterio tiene**, porque el criterio es justo lo que el
curso enseña. La respuesta no es motivacional, es estructural: **el riesgo del ángulo se concentra en
las cuatro primeras semanas y se hace barato justo mientras es probable** (§5.5).

## 5.2 El embudo de noventa minutos (M0, días 2 y 3)

| Paso | Duración | Qué hace | Por qué así |
|---|---|---|---|
| 1 | 20 min | Recibe **los 32 procesos ya escritos**. Tacha los que en su academia no ocurren o no lleva ella. Corrige volúmenes. Marca con palote los de **esta semana** | Reconocer es mucho más barato que recordar. Una hoja en blanco delante de alguien cansado produce ocho filas y abandono; una lista de 32 para corregir produce veinticinco filas en veinte minutos |
| 1b | 20 min | **El Mapa corto**: una letra de veredicto en las doce filas con más palotes | §4.5. Es un pretest, no un entregable |
| 2 | 10 min | **Descarte por número, sin pensar:** fuera P08, P17, P22, P25, P26, P29. Y fuera lo estacional, con una regla de una línea: **«si no lo hago en enero, no vale»** | Es aritmética, no criterio. Los seis descartes vienen del semáforo de datos y de la tabla de riesgo. La regla estacional protege contra montar el curso sobre julio y practicarlo en enero, con un volumen que se triplica entre febrero y julio |
| 3 | 20 min | Puntúa los 6–8 supervivientes en **cinco columnas observables** | Ninguna columna admite «depende» |
| 4 | 40 min en 2 días | **La prueba de la sombra** | Es donde se cae la elección equivocada |
| 5 | 10 min | Nombra el **proceso de repuesto** y firma la fecha | El repuesto existe desde el día 3, no desde la crisis |

**Las cinco columnas del paso 3:**

| Columna | +2 | 0 | −3 (descalifica) |
|---|---|---|---|
| ¿Cuántas veces esta semana? | 5 o más | 1–4 | 0 |
| Datos que toca (semáforo) | solo verde | ámbar seudonimizable | **rojo irreducible** |
| Consecuencia del peor error | interna, se arregla | molesta a un cliente | **dinero, plazo legal o visado** |
| **¿Puede mi herramienta de automatización actuar sobre los ficheros que abro?** | **sí: son míos** | **una copia mía sirve** | **no: solo existen en un recurso compartido** ⓘ | 
| ¿Sé cómo se hace bien? | perfectamente | más o menos | depende de otra persona |

> **ⓘ Sobre la cuarta columna, y aquí me aparto del juez 3** (§0.2, punto 1). La **pregunta** está en la
> mitad de criterio porque es durable: hay que hacérsela a cualquier herramienta de automatización de
> cualquier año, y la formulación no menciona ningún producto. El **límite concreto de hoy** —la
> automatización nativa de su entorno falla con unidades compartidas, carpetas compartidas y hojas con
> referencias externas [V]— vive fechado en `comun/datos-volatiles.md`, junto con la puntuación de −3
> que hoy aplica. Si mañana esa restricción desaparece, se cambia un fichero y la columna sigue siendo
> correcta.
>
> **Por qué esta columna existe y por qué es la aportación de diseño más rentable del curso:** el
> centro de gravedad de su puesto son los buzones `info@` y `accommodation@` y una hoja de camas
> compartida. En las otras dos arquitecturas ese límite aparece en la semana 9 y se gestiona como mala
> noticia; una de ellas confiesa por escrito que no lo ha resuelto. Aquí entra en el criterio de
> elección de la semana 1 y **se cobra antes de que haya nada construido encima**. La diferencia entre
> «he elegido un proceso que no encaja» (semana 1, cuesta dos horas) y «esta herramienta no sirve para
> mi trabajo» (semana 9, atribución irreversible) es la diferencia entre seguir y abandonar.

## 5.3 La prueba de la sombra (dos días laborables, tres minutos al día)

Antes de comprometerse, durante dos días, cada vez que ejecuta el proceso candidato **anota tres
cosas**: cuántos minutos ha tardado · qué documento ha abierto · **qué decisión ha tomado que no
estaba escrita en ninguna parte**.

Tres criterios de rechazo, ninguno de opinión:

| Lo que ve en la hoja | Qué significa | Veredicto |
|---|---|---|
| **En dos días no lo ha ejecutado ni una vez** | No es tan frecuente como cree. La frecuencia percibida y la real no coinciden casi nunca | **Descartado.** Pasa al siguiente |
| **No ha abierto ningún documento** | No hay contexto que dar: es juicio puro. Un asistente con fuentes no tiene qué morder | **Descartado.** Ese proceso es «chat, mejor usado» y ahí se queda |
| **Las decisiones no escritas son cada vez distintas** | No es un proceso: es una serie de casos | **Descartado**, o se acota al trozo que sí se repite |

**Nota metodológica que va en el material, porque es su casa.** Esto es muestreo de eventos, no
introspección. *La gente describe sus procedimientos como cree que deberían ser, no como los ejecuta*,
y los atajos y excepciones —que son justo lo que rompe una automatización— no se verbalizan
espontáneamente. Por eso no se pregunta: se observa. Y por eso el tercer campo es el que más rinde: es
el inventario de todo lo que un sistema no sabría hacer.

**El hallazgo prometido a las 48 horas** *(injerto I10)*. El material predice por escrito lo que la
observación va a revelar, para que los dos días de peaje sean pago:

> *«A las cuarenta y ocho horas vas a descubrir una de estas tres cosas, y probablemente dos: que este
> proceso lo haces bastante menos veces de las que creías, o bastante más; que no sabes con certeza
> cuál de tus documentos es el vigente; o que en dos días has tomado tres o cuatro decisiones que no
> están escritas en ningún sitio de la academia y que solo sabes tú. Eso no es un fallo del ejercicio:
> es el primer hallazgo del curso, tiene nombre de proceso, y va derecho al Cuaderno de evidencias. Es
> lo que ninguna herramienta puede darte hecho, y es la razón por la que este curso lo puedes hacer tú
> y no un informático.»*

## 5.4 La regla del embudo vacío *(injerto I18 — hueco que ninguna arquitectura cubría)*

El juez 1 lo señala y tiene razón: exigir ≥5 ejecuciones semanales + solo verde + ficheros propios +
«sé hacerlo perfectamente» puede descartar buena parte de lo que ella hace, porque casi todo su stack
—buzón, hoja de camas, Excel maestro, WhatsApp Business, carpeta de plantillas— es compartido.

> **Si el embudo te deja con cero candidatos, no es un fallo del embudo ni tuyo: es un hallazgo, y
> tiene tres salidas escritas. Se resuelve el día 3, no la semana 6.**
>
> **Salida A — pedir delegación.** Un mensaje de dos líneas a quien administre el buzón: *«¿me podéis
> dar una etiqueta (o una carpeta) propia dentro de `info@` sobre la que yo pueda actuar?»* Es la
> petición que más veces resuelve esto en una empresa pequeña, no cuesta dinero, no cuesta licencia y
> no es pedir permiso para nada: es pedir un permiso técnico concreto. Va en el camino alternativo y
> no en el principal porque depende de otra persona.
>
> **Salida B — bajar el listón y acotar el trozo.** La frecuencia baja de ≥5/semana a ≥2/semana, y el
> proceso se acota a un trozo. **No pierdes nada:** la línea de corte de M1 iba a partirlo de todos
> modos, y un trozo con criterio, fuentes, disparador y frenos es un sistema completo aunque sea
> pequeño.
>
> **Salida C — adoptar P27.** El análisis de las respuestas de la encuesta de satisfacción. Es tuyo,
> está en tu lista, es riesgo bajo, tiene 600–800 respuestas al año, es el proceso más multilingüe que
> tienes y **hoy no lo hace nadie porque nadie tiene tiempo** — así que no compite con ningún
> procedimiento establecido ni se lo quitas a nadie. Es el proceso de repuesto por defecto y el curso
> trae su recorrido completo ya hecho.

## 5.5 La alternativa si falla: el divorcio preautorizado, con la aritmética escrita

Al final de M1 hay un **checkpoint de divorcio**. Cambiar de proceso es un movimiento legítimo,
escrito y firmado desde la semana 1. Lo que hace que no sea un consuelo sino una salvaguarda es el
número:

> **Al final de M1 lo único construido son la descripción del proceso, la línea de corte, la ficha de
> criterio y la batería de diez casos. Rehacer las cuatro cosas sobre el proceso de repuesto son
> aproximadamente dos horas, porque el método ya lo sabes y lo único que cambia es el contenido.** A
> partir de M2 el divorcio ya cuesta caro. Por eso el checkpoint está exactamente ahí y no después.

## 5.6 El expediente modelo (P27), y qué es y qué no es

El curso trae el recorrido completo **ya hecho** sobre P27: las siete capas, con sus artefactos, sus
fallos típicos y sus claves selladas. **No es un segundo hilo que ella ejecute** —eso duplicaría el
trabajo y este ángulo existe para no hacer dos cosas a medias—. Es tres cosas:

1. El **ejemplo trabajado con desvanecimiento** del que salen las soluciones comentadas.
2. La **fuente de los tres cebos**.
3. El **proceso de repuesto por defecto** si su elección se cae.

Y hay **una excepción deliberada, que sí se ejecuta**: la tarde de P27 en M3 (§6.5, injerto I15).

---

# 6. MAPA COMPLETO DE MÓDULOS

**Siete módulos, 17 semanas, 2 h propias por semana** más el trabajo que es trabajo del puesto.
Arranque en **octubre**: el pico de junio–septiembre (250–400 correos/día) mata cualquier calendario
que lo ignore, y noviembre–febrero es su temporada baja.

**Estructura fija de módulo:** 3 sesiones núcleo de 35–45 min · 1 bloque de proyecto de 60–90 min **en
horario de trabajo** · el cierre de capa (cinco preguntas + pregunta fija + columna nueva de la Tira +
doblete, ~55 min).

**Una frontera declarada desde la semana 1, y es diseño anti-abandono, no una rebaja:**

> **Al terminar M4 (semana 11) ya hay curso:** un proceso suyo funcionando, en uso, con frenos y con
> apagado probado. **M5 y M6 son donde se cobran los objetivos 4 y 5** —criterio portátil y
> evangelización— y son la parte que más rinde a doce meses vista. Decirlo así, y no fingir que las
> diecisiete semanas son un bloque indivisible, es lo que evita que la semana 12 se lea como fracaso.

## 6.0 Vista de conjunto

| M | Sem. | Capa | Cambio mental en una frase | Qué sale del expediente | Escalón del perfil | Corrección dominante |
|---|---|---|---|---|---|---|
| **M0** | 1–2 | 0 · Ver el proceso | «Lo primero no es la IA: es mirar qué hago realmente» | Primera victoria · asistente v1 · hoja de sombra · descripción real · ficha del entorno · Mapa corto | 1 · chat | Cronómetro + tres rechazos observables + la pantalla |
| **M1** | 3–4 | 1 · Criterio y corte | «El cuello de botella no es el prompt: es que nadie ha escrito qué cuenta como respuesta correcta» | Línea de corte · ficha de criterio · anclas de tono · batería + clave sellada | 1 · chat | Ctrl+F + los diez apartados + **cebo 1** |
| **M2** | 5–6 | 2 · Contexto con procedencia | «La memoria fiable es un fichero, no una sensación» | Mapa de datos · fuentes fechadas · asistente v2 que cita y se abstiene · ficha de traslado | 1 · chat | Batería col. 3 + lista binaria + prueba de la compañera |
| **M3** | 7–8 | 3 · Disparador y lote | «Automatizar no es una herramienta nueva: es quitar el dedo del disparador» | Disparador · tope · apagado probado · la tarde de P27 · notación neutra | 2 · automatización | Se dispara o no + el caso que NO debe disparar + tabla de confusión |
| **M4** | 9–11 | 4 · Juicio y frenos | «Un agente no es una automatización mejor: ha renunciado a ser predecible» | Puntos de juicio · temas prohibidos · condiciones de parada · revisor con nombre y hora · plan de fallo · cinco preguntas sobre una herramienta ajena | 3 · agentes | Cinco paradas fabricadas + rúbrica negativa + **cebo 2** |
| **M5** | 12–14 | 5+6 · Medir y traspasar | «Que se ejecute cada lunes no es que sirva» | Evaluación · prueba ciega · lectura de la Tira · ficha de traspaso · calendario de revisión | transversal | La prueba ciega + la reproducción del número |
| **M6** | 15–17 | 7 · Que lo adopten | «Lo que hace que una organización adopte algo es que siga funcionando la semana que tú no estás» | Dossier · demo de 3 min · **la semana sin ella** · segunda vuelta del Mapa corto · rúbrica propia validada | **adicional** | **El piloto** + **cebo 3** |
| — | — | apéndice | *(lectura opcional, sin entregable)* | Lo que hay más arriba | 4 · opcional | ninguna |

**Herramientas nuevas en 17 semanas: dos o tres**, según lo que su proceso pida. **Coste: cero euros.**
Si el curso acaba costando dinero, el diagnóstico estaba mal.

---

## 6.1 M0 · Capa 0 — Ver el proceso, y elegir cuál (semanas 1–2)

**Cambios mentales.** Tres, y el tercero es el que más cuesta.
*«Lo primero no es la IA: es mirar qué hago realmente.»*
*«Lo que creo que hago y lo que hago no son lo mismo, y la diferencia es exactamente lo que rompería
una automatización.»*
*«El mismo texto en la misma pantalla es seguro o inseguro según con qué cuenta haya entrado.»*

### Secuencia interna, y por qué exactamente ésta

**Día 1 · 25 minutos · La primera victoria, a prueba de fallo.**
Instrucciones permanentes guardadas —quién es, dónde trabaja, en qué idiomas escribe, qué tono usa,
qué no debe hacer nunca— y usadas **hoy** sobre un correo real que tiene pendiente. Cronometrado antes
y después. Sin instalar nada, sin pedirle nada a nadie, sin hablar con nadie. **El mapa del curso va
después de este resultado, nunca antes.**

**Días 2–3 · 90 minutos · El embudo** (§5.2), con el Mapa corto dentro. Y en paralelo, **la prueba de
la sombra**: 3 min/día, tiempo de trabajo.

**Días 4–5 · 25 minutos · El asistente v1 que cita** *(injerto I1, de arq-2)*.
Un asistente guardado con **tres fuentes verdes** —tarifario vigente, calendario académico y
condiciones generales, que **no son datos personales**— que contesta las seis preguntas que repite el
70–80 % de sus leads **citando de qué documento sale cada dato**. Se usa esa misma tarde.

> **Por qué escalonado al día 4 y no el día 1, que es donde arq-2 lo pone.** Porque el día 1 tiene que
> ser a prueba de fallo, y montar un asistente con tres ficheros que cite, en veinticinco minutos, por
> alguien que nunca ha abierto una terminal y que todavía no sabe qué plan tiene su empresa, **no lo
> es**: la propia arq-2 admite que «si esa caja no funciona, la primera experiencia del curso es un
> fracaso y no hay red debajo». Al día 4 ya ha ganado una vez, ya ha mirado su entorno y ya tiene el
> proceso elegido. El premio grande sigue llegando en la primera semana, y llega con red debajo.
>
> **Y qué repara este injerto.** Sin él, arq-3 no tiene ningún artefacto real hasta la semana 5, y las
> semanas 3–4 —que son documentación pura, el módulo «más ligero en clics de todo el curso»—
> transcurren en seco justo después de la luna de miel. Con él, esas dos semanas transcurren con algo
> suyo funcionando encima de la mesa, y —esto es lo mejor— **M1 empieza pasando la batería contra el
> asistente v1 y viendo que saca 4 de 10**. La ficha de criterio nace como respuesta a un fallo
> observado en algo suyo, no como deberes previos. El «esto ya lo hice» que arq-2 sufre en su M2 aquí
> no ocurre, porque M2 no repite el asistente: lo **repara**.

**Semana 2:**
- **`00-como-se-hace-de-verdad.md`**, escrito **a partir de la hoja de sombra**, no de memoria:
  disparador, documentos que abre, decisiones no escritas, salida y a dónde va.
- **La ficha del entorno**: qué plan, si su cuenta tiene licencia, qué retención, si hay política
  escrita — con los mensajes literales para copiar y pegar **y las comprobaciones empíricas por si
  nadie contesta**.
- **La tarjeta del lunes** impresa al lado de la pantalla: el semáforo verde/ámbar/rojo.
- **Proceso de repuesto nombrado y firmado.**
- **PC-1.**

### Capacidad que entrena, y cómo se enseña transferible

**Mirar un proceso y describirlo como es.** Es la más portátil del curso.
- **Se describe por observación, no por introspección.** Muestreo de eventos, tres campos, dos días.
  Vale para cualquier proceso, de cualquier empresa, en cualquier año, y no menciona ninguna
  tecnología.
- **Las cuatro preguntas que definen cualquier plan de cualquier proveedor** sustituyen a la tabla de
  planes: *¿entrenan con lo que escribo? ¿cuánto lo guardan y quién decide? ¿dónde se procesa? ¿hay
  contrato de encargado del tratamiento?* Más la quinta, que suele decidir de verdad: *¿alguien lo ha
  configurado y ha dejado dicho por escrito qué se puede meter?* Es el ejemplo más limpio del curso de
  criterio frente a clic, y va el primero a propósito.

### Entregable

Hoja de elección + hoja de sombra + `00-como-se-hace-de-verdad.md` + ficha del entorno + Mapa corto +
asistente v1 + proceso de repuesto firmado.

### Cómo se autocorrige

- **Ejecución real.** El correo del día 1 salió mejor y en menos tiempo, o no. Cronómetro, no opinión.
- **Los tres criterios de rechazo de la sombra** (§5.3). No hay nada que valorar: se mira la hoja.
- **La comprobación que más caza, y cuesta un minuto:** *¿tu descripción contiene al menos dos
  decisiones que no estaban en tu idea previa del proceso?* Si no las contiene, la escribiste de
  memoria y hay que volver a la sombra. **Es la única forma sin mentor de detectar el error más caro
  de la capa.**
- **Las tres filas al azar** sobre el Mapa corto (§4.5).
- **La pantalla corrige el plan.** Las comprobaciones empíricas se corrigen solas, y enseñan de paso
  lo que necesitará cuando el material envejezca: **la documentación dice una cosa y la instancia dice
  otra, y manda la instancia.**
- **Rúbrica de la ficha del entorno, ocho casillas, con un estándar de suspenso brutal y muy útil:**
  *si en algún punto has escrito «creo que», «supongo que» o «me suena que», está mal resuelto.* «No lo
  sé y lo pregunté el día 14» **sí vale**. Distinguir lo que sabes de lo que supones es el mismo
  estándar que necesitará para evaluar respuestas de una IA, y por eso va el primero.
- **Batería sellada de diez preguntas** para el asistente v1, escritas **antes** de montarlo.

### Puedes pasar a M1 cuando…

- Existe la ficha del entorno con las ocho casillas, **o** con la frase *«pregunté a X el día D y no
  obtuve respuesta»*.
- Hay un proceso elegido **con puntuación positiva y ningún −3**, y un repuesto firmado.
- La hoja de sombra tiene dos días y **la descripción contiene dos decisiones no previstas**.
- Hay una **línea base medida**, no estimada: minutos por unidad, tres mediciones.

---

## 6.2 M1 · Capa 1 — Qué es hacerlo bien, y qué trozos no entrego (semanas 3–4)

**Cambios mentales.** Los dos más caros del curso.
*«El cuello de botella no es el prompt: es que nadie ha escrito nunca qué cuenta como respuesta
correcta en esta tarea.»*
Y el segundo, que no tiene que creer por autoridad porque lo deduce de algo que sabe desde tercero de
carrera:

> **Un modelo de lenguaje es el instrumento con la validez aparente más alta y la garantía de validez
> de contenido más baja que vas a manejar en tu vida. Está optimizado para producir texto plausible: la
> plausibilidad es su función objetivo, no un efecto secundario.**

### Qué construye

1. **La línea de corte** (`01-linea-de-corte.md`): el proceso partido en trozos, cada trozo con
   veredicto —*lo entrego · lo entrego con revisión mía antes de que salga · se queda conmigo*—, el
   motivo elegido de la lista cerrada de cinco, y **la columna «lo que sí se puede hacer alrededor»**
   *(injerto I6)*. **Es el entregable más importante del módulo y el que la rúbrica protege más
   duro.**
2. **La ficha de criterio**: definición en una frase, 4–6 dimensiones, un indicador observable por
   dimensión, críticos marcados, punto de corte. **Una cara.**
3. **Las anclas de tono**: tres frases completas —bajo, medio, alto— para dos dimensiones, sacadas de
   correos que envió de verdad. Ese fichero **es** el contexto de tono de la capa 2, no un
   calentamiento.
4. **Los diez apartados**: diez casos reales sacados **por orden cronológico, no elegidos**, y cerrados
   antes de escribir una línea de instrucción. **Uno de ellos en un idioma minoritario real.**
5. **La Tira**, columnas 1 y 2: la batería contra el asistente v1 (que saca 4/10) y contra la primera
   versión con criterio.

### La columna «lo que sí se puede hacer alrededor» *(injerto I6)*

La línea de corte de arq-3 exige motivo para cada trozo que se queda con ella, pero **no exige
compensación**. Con el injerto de arq-2, el módulo **no termina con una lista de renuncias: termina con
un sí concreto por cada no**. La rúbrica la exige rellena con **un artefacto nombrable, no con una
intención**.

Ejemplos, con la corrección obligatoria que pide el juez 4 aplicada:

| No se puede | Lo que sí, alrededor |
|---|---|
| **P17** matching alumno ↔ familia | **P18** confirmación de alojamiento: 700–800 al año, plantilla con diez variables, ningún dato de salud. Y **P20** triaje de incidencias: clasificar y enrutar sí, responder no |
| **P08** redactar la carta de aceptación para visado | **Una comprobación determinista de consistencia entre los campos que tú ya has tecleado a mano**: que el nombre, la fecha de nacimiento y las fechas del curso coincidan entre el expediente, la carta, la factura y el certificado. Ataca el mismo mecanismo de error documentado en P04 —el nombre transcrito mal se propaga a cuatro documentos— **sin que el pasaporte entre en ninguna herramienta**, porque un documento de identidad es rojo absoluto: nunca, ni imagen ni PDF |
| **P26** responder una queja formal | Preparar el **expediente** de la queja: reunir el histórico, las fechas y lo que dicen las condiciones vigentes **en la fecha de la reserva**. Redactar, no |
| **P22** hoja de camas | Una comprobación diaria que **avisa** de discrepancias entre la hoja de camas y el listado de reservas. Avisa, no corrige |

### Cómo se autocorrige

- **Ctrl+F sobre la ficha de criterio.** Si aparecen «adecuado», «correcto», «natural», «profesional»
  o «de calidad» **sin un ancla detrás**, no ha operacionalizado: ha renombrado el constructo.
  Autocorrección mecánica perfecta, cinco segundos.
- **Prueba de tamaño:** la ficha cabe en una cara. Una rúbrica de dos páginas no se usa nunca.
- **Los dos ítems que atacan la calidad sustantiva del criterio**, que es lo que ningún filtro mecánico
  alcanza *(de arq-1, y es poco, y está reconocido como tal en §17.3)*: *¿hay **al menos un indicador
  verificable contra una fuente externa** —un documento, una tabla, un dato que no dependa de tu
  impresión? SÍ/NO* · *¿están **todos** los indicadores marcados como críticos? Si sí, no has
  priorizado: vuelve y deja como críticos solo los que suspenderían el trabajo por sí solos.*
- **Rúbrica de la línea de corte, con dos criterios negativos que deciden el módulo:**
  *(a) si no hay ningún trozo que se quede contigo, está mal resuelto — vuelve;*
  *(b) si el motivo de algún «se queda conmigo» es «es difícil», está mal: los motivos legítimos son
  los cinco de la lista cerrada.*
  Y un tercero, del injerto: *(c) si algún «no» tiene la casilla «lo que sí, alrededor» vacía o con una
  intención en vez de un artefacto nombrable, está mal resuelto.*
- **Los diez apartados se abren al final, y tiene que fallar al menos uno.** Si no falla ninguno,
  **sospecha del muestreo antes que celebrar**: *si tu batería la pasa entera a la primera, tu batería
  es fácil; no es que tu sistema sea bueno.*
- **Y el criterio no se toca.** Si al abrirlos le dan ganas de cambiar la ficha para que aprueben, **lo
  anota y no lo cambia**. Ese impulso es el dato más interesante del ejercicio y tiene nombre: sesgo
  del experimentador.
- **CEBO 1 (control positivo).** El curso trae una **línea de corte de mentira**, de una academia
  inventada, con **tres defectos plantados y documentados** en un fichero sellado: uno visible (un
  trozo con datos rojos marcado como «lo entrego»), uno de omisión (falta el trozo de revisión humana
  antes de que algo salga) y uno de criterio (un trozo determinista clasificado como si necesitara un
  modelo). Ella lo corrige con la rúbrica y **después** abre la hoja de defectos. **Si encuentra 1 o 0,
  ese tipo de trabajo no se corrige con IA en el resto del curso.**
- **El protocolo de corrección con IA, siete reglas**, primera aplicación (§12.4).

### Checkpoint de divorcio, al final del módulo (§5.5).

### Puedes pasar a M2 cuando…

- La línea de corte pasa sus tres criterios negativos.
- La ficha de criterio pasa el Ctrl+F y cabe en una cara.
- La batería tiene diez casos, clave sellada, **y uno en idioma minoritario**.
- La Tira tiene dos columnas fechadas.
- El cebo 1 está pasado y el veredicto sobre la IA correctora está escrito.

---

## 6.3 M2 · Capa 2 — Que sepa de dónde sale cada dato (semanas 5–6)

**Cambio mental.** *«La memoria fiable es un fichero, no una sensación.»* Y la tríada que los
principiantes mezclan siempre: **fuente de verdad** (hechos, desde una sola dirección) ≠ **memoria**
(acuerdos que permanecen) ≠ **procedimiento** (pasos y formato de salida).

### Qué construye

1. **El mapa de datos del proceso** (§10.2): cada dato que atraviesa el proceso, su color, **en qué
   paso entra** y **dónde hay que quitarlo y quién lo quita**. Una cara.
2. **Las fuentes**, con **fecha y dueño en la primera línea de cada una**.
3. **El asistente v2**: el v1 del día 4, ahora con el criterio de M1 dentro, con las anclas de tono,
   con fuentes fechadas, que **cita el documento y su fecha** y que **dice «no lo sé»** cuando la
   respuesta no está. Y con la instrucción multilingüe explícita: **las fuentes están en español y la
   respuesta va en el idioma de la persona.**
4. **La prueba de traslado nº 1** (§8.4).
5. **La Tira**, columna 3.

### Capacidad, y cómo se enseña transferible

**Contexto con procedencia.** Tres piezas, ninguna con nombre de producto:
- **Citar no es un adorno: es lo que hace que revisar cueste cinco segundos en lugar de una
  investigación**, y por eso es lo que hace que la revisión se siga haciendo en julio.
- **«No lo sé» es una respuesta correcta, hay que exigirla explícitamente y hay que probarla a
  propósito.** Un sistema que nunca dice «no lo sé» no es que lo sepa todo: es que no lo has probado
  bien.
- **Una fuente sin fecha y sin dueño no es una fuente, es un papel.** El dueño es quien puede
  cambiarla; la fecha es lo que te dice si mirarla.

**Y el tercer registro, que es la pieza portátil de este módulo** *(injerto I7)*:

> **Las tres señas de que has encontrado esta capacidad en una herramienta que no has visto nunca:**
> 1. **Las fuentes siguen ahí mañana**, sin volver a subirlas.
> 2. **La respuesta dice de qué documento sale.** Si no cita, no es esto.
> 3. **Puedes listar qué hay dentro** y quitar una fuente sin rehacerlo todo.
>
> **Si falta cualquiera de las tres, lo que tienes es un adjunto en una conversación**, que es otra
> cosa y dura lo que dure esa conversación. Es la confusión más frecuente y la que hace que la gente
> crea que tiene esto montado cuando no lo tiene.

### Cómo se autocorrige

- **La batería, columna 3.** Umbral asimétrico: falla >0 de los 5 típicos → no está listo · se inventa
  una decisión en alguno de los 3 límite, **aunque acierte** → no está listo · contesta algo distinto
  de «no lo sé» en alguno de los 2 de rechazo → no está listo. **Una respuesta correcta a un caso de
  rechazo es un suspenso.**
- **Lista de comprobación binaria, diez ítems observables:** *¿cada fuente tiene fecha en la primera
  línea? ¿cada fuente tiene un nombre de persona como dueño? ¿alguna respuesta cita un documento que
  no está en las fuentes? ¿he abierto tres documentos citados y encontrado la frase? ¿hay una frase
  que diga qué hacer cuando falta un dato? ¿he subido el maestro de algo en vez de una copia? ¿hay un
  precio o una fecha escritos dentro de las instrucciones en vez de en una fuente?*
- **La prueba de la compañera**, sobre tres casos seudonimizados: *¿podría [nombre de una compañera
  concreta] saber de quién hablo leyendo esto?* Si sí, sigue quitando. Y el criterio del otro lado,
  que es el que casi nadie pone: **el prompt resultante tiene que seguir sirviendo**; si la respuesta
  que da es inservible, has quitado contexto que no era identificador.
- **PC-2 aquí**, justo antes de cargar fuentes reales.

### Puerta M2 → M3 *(injerto I5, de arq-1 salvaguarda 4)* — la más importante del curso

> **No se pasa a la capa 3 hasta que las tres cosas son ciertas:**
> 1. La batería da **5/5** en los típicos, **pide aclaración** en los 3 límite y dice **«no lo sé»** en
>    los 2 de rechazo.
> 2. **Has usado el asistente al menos cinco veces en una semana SIN que el curso te lo pidiera.**
> 3. La prueba de traslado está hecha y sus tres columnas están rellenas con cosas concretas.

**Por qué la condición 2 es la más importante que hay escrita en este documento.** No mide si aprendió
la lección: **mide si el artefacto le sirve**, que es la única cosa que un curso sin profesor no puede
preguntarle a ella misma y sí puede contar. Y hay una razón de fondo: **la tesis entera de esta
arquitectura —«el mundo la corrige cada martes»— es falsa si ella no lo usa.** Si el asistente no se
usa espontáneamente, el asistente está mal, y **automatizar algo que está mal es multiplicar el
error**.

**Y la regla que hace que una puerta cerrada no sea un suspenso:** *si la puerta no se abre, no has
fracasado: te quedas una semana más en la capa 2 arreglando lo que hace que no lo uses. Esa semana
está presupuestada.* Y hay una lista de tres causas típicas con su arreglo mínimo: *no está donde
trabajas* (llévalo al sitio donde ya miras) · *tarda más que hacerlo a mano* (el criterio es
demasiado largo: recórtalo) · *no te fías de lo que devuelve* (faltan citas o falta la fórmula de
negativa).

---

## 6.4 M3 · Capa 3 — Que ocurra sin que lo pidas (semanas 7–8)

**Cambio mental.** *«Automatizar no es una herramienta nueva: es quitar el dedo del disparador.»* Es el
momento psicológico del curso —la primera vez que algo pasa sin que ella lo pida— y por eso llega en la
semana 7 y no en la 14.

### Qué construye

1. **El disparador** sobre el trozo que la línea de corte marcó como entregable, con su tipo declarado
   (por calendario o por suceso) y su justificación.
2. **El tope**: *si la lista supera N, no hagas nada y avísame.* Un sistema que genera cuarenta
   borradores un lunes de julio no ayuda, entorpece. **Enseñar a poner topes es enseñar diseño.**
3. **El apagado, probado de verdad**, no imaginado.
4. **La tarde de P27** (§6.5).
5. **La notación neutra** y la prueba de traslado nº 2 (§8.4).
6. **La Tira**, columna 4.

Y la regla que gobierna la capa entera:

> **Automatiza la lectura y la preparación. La escritura hacia fuera la firma una persona.**
>
> Y la razón, que no es prudencia sino diseño de aprendizaje: **si el artefacto solo prepara, todos sus
> errores son recuperables, y por eso puedes permitirte equivocarte mucho — que es exactamente lo que
> hace falta para aprender.** Etiquetar es reversible; enviar no. Se puede relajar más adelante,
> proceso a proceso y con datos de acierto medidos. **No se relaja por costumbre.**

### La restricción de producción que hace este módulo a prueba de administradores *(injerto I8)*

> **Ningún módulo posterior puede depender de que el constructor de flujos esté habilitado.**
>
> Consecuencias escritas, no aspiracionales:
> - **M3 debe tener una ruta de disparo por reloj dentro del chat que ella ya usa**, que no requiere
>   ninguna consola, ningún permiso de administrador y ninguna licencia extra. Esa ruta es el camino
>   principal, y el constructor de flujos es la ruta ampliada.
> - **M4 (frenos) tiene que poder ejercitarse sobre el asistente aunque no exista flujo.** Los temas
>   prohibidos y las condiciones de parada viven dentro de las instrucciones del asistente; el flujo,
>   si existe, solo añade la bifurcación y la marca.
> - Si el administrador tiene la automatización nativa desactivada, **se pierde comodidad y cero
>   hilo**, y el material lo dice con esas palabras: no es un fallo suyo ni del curso.

**Y los límites, por delante y no al tercer intento fallido.** En la primera página del módulo, no en
una fe de erratas: los flujos de su entorno **fallan con unidades compartidas, carpetas compartidas y
hojas con referencias externas** [V]; un solo disparador por flujo; tope de etiquetas visibles; el
administrador puede tener pasos desactivados y no hay forma de saberlo hasta intentarlo. Como la
cuarta columna del embudo de M0 ya descartó los procesos que solo viven en recursos compartidos,
**aquí esto no debería ser una sorpresa sino una confirmación** — y esa es exactamente la función de
haber puesto la restricción en el criterio de elección.

### Cómo se autocorrige

- **Se dispara o no se dispara.** El corrector más fiable que existe, y aquí está entero.
- **La prueba de los cinco casos fabricados**, uno por categoría, **y un sexto que NO debe disparar**,
  que es el que casi nadie prueba. Cinco salidas correctas y una no-salida, o no las hay.
- **La prueba de apagado.** Se apaga de verdad y se vuelve a encender. *Un sistema que no sabes apagar
  no está terminado.* Y hay una razón práctica: el día que falle vas a estar nerviosa, y no es el
  momento de averiguar dónde está el botón.
- **La prueba del tope:** meterle un lote grande a propósito y comprobar que se detiene.
- **Lista de comprobación de plataforma, seis ítems binarios**, escrita como síntomas y reutilizable
  como diagnóstico: *¿el fichero que toca está en una unidad compartida? ¿la hoja usa referencias
  externas? ¿tiene más de un disparador? ¿hay algún paso que escriba fuera? ¿lo he probado con un caso
  que debe NO disparar? ¿sé cómo se apaga y lo he apagado?*
- **La Tira, columna 4**, con la lectura contraintuitiva escrita: *si la calidad ha mejorado respecto a
  la capa 2, sospecha: probablemente reescribiste el criterio por el camino, y eso es mérito tuyo, no
  del disparador.*
- **PC-4, el comodín**, disponible desde aquí.

### Puerta M3 → M4

> **El disparador ha corrido al menos una semana entera sobre casos reales, y has visto fallar algo y
> sabes por qué falló.** Si a estas alturas no ha fallado nada, **el material trae un fallo provocado**
> y se ejecuta: un caso fabricado que el disparador se traga en silencio.
>
> Motivo: **sin haber visto un fallo no hay criterio para dar autonomía a nada**, que es exactamente lo
> que pide la capa siguiente.

---

## 6.5 La tarde de P27 *(injerto I15)* — dentro de M3, sesión 2

**Qué es.** Una sesión de 90 minutos, tiempo de trabajo, sobre un material que el curso trae ya
preparado: **treinta comentarios reales de encuestas de satisfacción en diez idiomas** y **un libro de
códigos cerrado** (5–8 categorías con definición operativa, criterios de inclusión y exclusión, dos
ejemplos prototípicos y **dos ejemplos frontera con la decisión ya tomada y justificada**).

**Qué hace ella, en este orden:**
1. **Codifica los treinta a mano**, con el libro de códigos delante. Sin ver nada más.
2. **Aplica el mismo libro de códigos a los treinta de golpe** con su asistente, en lote.
3. **Construye la tabla de confusión** entre sus códigos y los del sistema.
4. Escribe **una frase por cada confusión que se repite**.
5. Mira el acuerdo de la **categoría menos frecuente por separado** —si el 60 % son de alojamiento, un
   clasificador que dijera siempre «alojamiento» acertaría el 60 %.
6. **Abre la clave sellada del curso**: la codificación de referencia de los treinta. Compara **sus**
   códigos con la referencia, no solo los del sistema.

**Umbrales, por los dos lados:** ≥26/30 de acuerdo con el sistema · **menos del 15 % en «sin
clasificar»**, y **si cae 0 %, está forzando encajes**.

**Por qué esto existe, y son cinco razones, todas de reparación:**

1. **Restaura el mejor mecanismo de corrección de nivel 1 que hay**, que en arq-3 era contingente: si
   su proceso no incluye clasificación en lote, nunca hace la doble codificación con tabla de
   confusión. El juez 2 lo señala como el tercer defecto de arq-3 y tiene razón.
2. **Restaura el oráculo escrito por el curso.** arq-3 renuncia al doble hilo y con él a que alguna
   clave la escriba alguien que no sea ella; aquí hay una clave que ella no ha escrito, contra la que
   puede calibrarse. Es la calibración que faltaba.
3. **Garantiza la práctica multilingüe** con independencia del hilo elegido. Diez idiomas, comentarios
   reales, y el fallo típico anunciado: **el sistema clasifica peor en los idiomas que no son inglés**,
   y los estilos de respuesta culturales hacen que un mismo grado de descontento se exprese de forma
   muy distinta según de dónde venga el alumno.
4. **Es la capacidad «una instrucción, N unidades» sin depender de ningún producto.** El artefacto
   portátil no es la implementación: **es el libro de códigos**, y el ejercicio obliga a decirlo:
   *«nombra dos formas distintas de aplicar tu libro de códigos a 600 filas y di qué cambia entre
   ellas»*. Lo que cambia es la comodidad y el volumen; lo que no cambia es la calidad de la
   clasificación.
5. **Si su hilo se cae más adelante, medio P27 ya está hecho.** Es la salida C del embudo vacío con
   ventaja.

**Y lo que NO es:** no es un segundo hilo. Son 90 minutos una sola vez, con material provisto y clave
sellada. El curso sigue construyendo **una** cosa.

---

## 6.6 M4 · Capa 4 — Juicio donde hace falta, frenos donde hace falta (semanas 9–11)

**Tres semanas, no dos.** Es el único módulo al que se le da aire antes del final, y se dice por qué:
es la frontera conceptual del curso, es donde más gente se cae, y es donde una puerta cerrada tiene que
poder costar una semana sin romper el calendario.

**Cambios mentales.** Dos.
*«Un agente no es una automatización mejor: es una automatización que **ha renunciado a ser
predecible** a cambio de poder afrontar casos que no previste. En atención al cliente esa renuncia se
paga a conciencia y solo donde compensa.»* Y la dirección del error que casi nadie enseña: **un agente
puede ser exceso.** Si los pasos son fijos, meterle juicio lo hace más caro, más lento y menos
auditable.
Y el segundo: *«el riesgo no es el del día 1, es el del día 60.»* Sesgo de automatización: a la tercera
semana se deja de revisar. **La confianza no es una salvaguarda.**

### Qué construye

1. **El juicio, confinado a dos o tres puntos concretos**, cada uno con su criterio escrito y
   justificable.
2. **La lista de temas prohibidos** (`04-frenos.md`), en negativo y sin matices: *nunca respondas sobre
   requisitos o plazos de visado; nunca cites importes; nunca confirmes disponibilidad de alojamiento;
   nunca respondas a una queja formal; nunca menciones salud. Si el tema aparece, aunque no use esas
   palabras, escribe SOLO: DERIVAR A PERSONA — motivo: <tema>, y para.*
3. **Las condiciones de parada**, seis, y la sexta es el injerto multilingüe:
   - no encuentro la respuesta en mis fuentes;
   - la persona está enfadada, o menciona abogado, reclamación u hoja de reclamaciones;
   - hay un menor implicado, o se menciona salud;
   - el importe supera X;
   - **el mensaje viene de una agencia y menciona un acuerdo o convenio particular** — porque las
     agencias tienen tarifas netas y condiciones de cancelación pactadas, distintas de las públicas, y
     un error se multiplica por quince alumnos;
   - **el mensaje llega en un idioma que no está entre los que has probado.**
4. **Parar no es callarse**, y son tres cosas a la vez: no producir la salida · dejar **una marca
   visible donde tú ya miras** · **decir por qué paró, en una línea**.
5. **El punto de revisión humana, con nombre propio y con hora.** *«<nombre>, antes de las 18:00 del
   mismo día.»* Un revisor sin plazo no es un revisor.
6. **El plan para cuando falle**, en cinco pasos: detectar · parar · reparar con la persona (llamada,
   no correo) · corregir el sistema añadiendo ese caso a la batería · y valorar si hay brecha de datos
   — **esto último no lo decide ella [!]**, lo escala el mismo día.
7. **Las cinco preguntas aplicadas a una herramienta que el curso no ha enseñado** (RA13), leyendo su
   documentación quince minutos, con las tres comprobaciones concretas: *¿lo cubre mi plan? ¿puede
   tocar los recursos donde vive mi trabajo? ¿puedo ver qué hizo?*
8. **La caja del fondo**, una sola vez y aquí (§9.1).
9. **La Tira**, columna 5.

### La honestidad incómoda, dicha sin disculparse

> **Su capa 4 realista es «un proceso con juicio en dos o tres puntos», no «un agente autónomo que
> gestiona el buzón».** La barrera número uno no es técnica ni de capacidad suya: es **de licencia**
> —los agentes de verdad están detrás de planes que su empresa casi con seguridad no tiene [V]—, de
> **permisos** —un agente útil necesitaría el buzón compartido y la hoja de camas— y de **datos** —sus
> procesos de más volumen mezclan salud, religión, menores y documentación de identidad—.

Y la reparación que arq-1 hizo sobre sí misma y que aquí se adopta entera: **el módulo no afirma «los
agentes están fuera de tu alcance».** Le hace rellenar la ficha de cinco preguntas para el agente que
tenga delante ese día y comprobar las tres cosas. **Si en 2028 las tres respuestas son sí, el módulo
funciona mejor, no peor: le da luz verde con criterio.** Un «no» sin condición de revisión es dogma; un
«no» con condición envejece bien.

### Cómo se autocorrige

- **Cinco casos de parada fabricados que DEBEN parar**, y el quinto es el ítem discriminante: *alguien
  que pregunta «¿cuánto tarda el papeleo para poder venir?» sin decir la palabra visado.* **Los cuatro
  primeros los para cualquier lista; el quinto separa una lista de palabras de una lista de temas.**
- **Un sexto caso normal que NO debe parar.** Si también para, **los frenos son demasiado anchos: el
  sistema no hace nada y eso no es seguridad, es inutilidad.** El fallo del otro lado siempre está
  escrito.
- **Rúbrica con criterios negativos y salida escrita obligatoria** (sin «no aplica»). Siete señales de
  fallo, y la sexta predice su propia aparición: *algún borrador suena estupendo y admite
  responsabilidad. Aparece casi siempre.*
- **Verdadero/falso de doce ítems** sobre el marco de datos, autocorrección instantánea. Menos de 10
  aciertos → releer.
- **CEBO 2**, ahora sobre una lista de frenos de mentira.
- **PC-5 al final del módulo.**

### El aviso sobre su propia formación, que va en el material y no en una nota al pie

Es la única lección del curso donde su formación juega **en contra**. El reflejo entrenado de una
psicóloga ante alguien que se queja es **validar, empatizar y hacerse cargo**. Los dos primeros están
bien y son una ventaja real. El tercero, por escrito, en una queja formal, **es una admisión de
responsabilidad que compromete a su empresa**. Y los modelos son complacientes por construcción: si le
pide una respuesta empática a una queja, le va a dar un texto estupendo que dice «tienes razón, la
habitación estaba en malas condiciones», y sonará mucho mejor que el correcto.

- Reconocer la **experiencia**, no calificar el **hecho**.
- Describir lo que **se ha hecho**, no juzgar lo que pasó.
- Y evitar el **«lamentamos que te sientas así»**, que suena a disculpa y funciona como invalidación:
  es el peor de los dos mundos.

Importes, plazos legales, responsabilidad y compensaciones **no los decide ella y no los decide el
sistema**. Se escalan. **[!]**

### Puerta M4 → M5

> Los cinco casos de parada **pararon y lo has visto** · el sexto **no paró** · cada parada dejó marca
> y dijo por qué · la respuesta a «quién revisa» es **un nombre y una hora** · el apagado está
> **probado**, no escrito · y **no existe ningún camino por el que algo llegue a un cliente sin que una
> persona le dé a enviar**. Si el último es SÍ, se vuelve al principio del módulo.

---

## 6.7 M5 · Capas 5 y 6 — ¿Sirve, y sobrevive sin mí? (semanas 12–14)

**Tres semanas. Es la fusión de «medir» y «dejarlo vivo», y es una decisión mía contra las tres
arquitecturas** (§0.2, punto 5). Motivo: la meseta baja de siete semanas a seis, desaparece una
frontera de módulo, y los dos contenidos son el mismo movimiento —*comprobar que sirve y dejarlo en
condiciones de que siga sirviendo sin ti*— que además es exactamente lo que M6 consume.

**Cambios mentales.** Dos.
*«Que el sistema se ejecute cada lunes no es que sirva. Puede ejecutarse impecablemente y no cambiar
nada, porque el informe que produce no lo lee nadie o porque los borradores se reescriben siempre.»*
**Evaluación de proceso ≠ evaluación de resultado.**
Y: *«un sistema sin dueño y sin fecha se degrada. Y cuando se degrada, el recuerdo que queda en la
empresa no es “faltaba mantenimiento”: es “aquello de la IA no funcionaba”.»*

### Semanas 12–13 · Medir

1. **Media página de evaluación, con fecha**: el número antes (de la hoja de sombra de M0, medida
   **antes** de construir nada, que es lo que la hace honesta) · el número después · el **coste
   completo** —montaje + revisión + mantenimiento— · **cuál de las seis amenazas a la validez interna
   podría explicar el resultado** y qué mediría para descartarla.
2. **La prueba ciega**, el ejercicio con mejor relación valor/esfuerzo del curso: cinco respuestas
   suyas de hace meses y diez salidas del sistema sobre casos comparables, **sin marcas de origen,
   barajadas por otra persona**, puntuadas con la ficha de criterio de M1.
3. **La cadena causal en cinco flechas**, con el eslabón que no depende de ella subrayado.
4. **La lectura completa de la Tira**: una frase escrita por columna diciendo qué aportó esa capa. Si
   no puede escribir esa frase para alguna columna, esa capa no le aportó nada, y merece la pena
   saberlo.

**Herramienta y por qué: una hoja de cálculo, un cronómetro y una persona que baraje.** Deliberado:
**la evaluación no se hace con la herramienta evaluada.** Pedirle a un modelo que juzgue lo que él
mismo produjo acumula dos sesgos documentados —preferencia por lo verboso y auto-preferencia— que
apuntan al mismo desastre: aprobar por construcción.

### Semana 14 · Traspasar

5. **La ficha de traspaso**: qué fuente caduca y cada cuánto · **quién la revisa, con nombre** · qué
   batería se vuelve a pasar cuando se toque algo · cómo se apaga, probado · y qué hacer el día que
   falle.
6. **El calendario de revisión**, con la próxima fecha escrita.
7. **La prueba del hueco**: dejar el sistema una semana sin tocarlo y comprobar qué se ha
   desactualizado. Se lanza aquí y **se recoge durante la semana del piloto de M6**, que es una semana
   en la que ella no lo va a tocar de todos modos. Coste real: cero.

### Cómo se autocorrige

- **La prueba ciega es autocorrección en estado puro.** No hay rúbrica que discutir: o acierta
  identificando cuáles eran suyas, o no; o ganan las suyas, o no. Y el patrón que aparece casi
  siempre —el sistema empata o gana en las dimensiones no críticas y **pierde en la exactitud del
  dato**— **le dice exactamente dónde poner la revisión humana**, que es la decisión que el curso
  entero perseguía.
- **Prohibiciones de vocabulario como comprobación mecánica.** Si aparece «significativo», está mal:
  aquí no se estima un parámetro poblacional, se comprueba la cobertura de un instrumento contra un
  criterio fijado. Si la medida es «horas a la semana» en vez de **minutos por unidad**, está mal: es
  lo único que sobrevive a que su volumen se multiplique por tres entre febrero y julio.
- **La resta obligatoria.** Si no ha restado revisión y mantenimiento, está mal. Y si el saldo es
  negativo y aun así quiere conservarlo por otra razón —menos errores, menos carga mental, respuesta
  más rápida al cliente—, **que lo diga y mida esa otra razón**: es legítimo, pero entonces el ahorro
  de tiempo no era el objetivo.
- **Una amenaza que no puede descartar, nombrada obligatoriamente.** Las seis, traducidas a su caso:
  historia (septiembre no es julio) · maduración (ella misma ha mejorado en la tarea) · regresión a la
  media (eligió lo que más dolía, y lo que más duele suele medirse en su peor semana) ·
  instrumentación · reactividad de la medida (la semana que se cronometra se trabaja más rápido — y
  este juega **a favor**: el ahorro real es mayor que el medido) · atrición (si deja de usarlo los días
  de agobio, la muestra final son los días tranquilos).
- **La reproducción del número a las dos semanas** *(injerto I13)*: con la ficha de método delante,
  vuelve a calcular. **Si no sale el mismo número ±10 %, el número no era reproducible y la evaluación
  se reescribe.** Es un test-retest de su propio instrumento y no consume a nadie. *(Se ejecuta ya en
  M6, sobre el dossier.)*
- **Lista binaria de la ficha de traspaso:** *¿hay un nombre de persona en «quién lo mantiene»? ¿hay
  una fecha en cada fuente? ¿hay una fecha en «próxima revisión»? ¿está probado el apagado? ¿alguien
  que no sea yo podría encontrar la carpeta?*
- El único favor humano del módulo —**barajar**— son cinco minutos y **no consume punto de consulta**:
  vale cualquier compañera.

### Caja obligatoria «lo que vas a ver la primera vez»

> *«Es posible que el ahorro sea menor de lo que esperabas. Si eso pasa, es un resultado del curso, no
> un fracaso tuyo — y es exactamente el tipo de resultado que casi nadie publica. Antes de decidir
> nada, comprueba las dos cosas que casi siempre lo explican: que estés midiendo por unidad y no por
> semana, y que hayas contado el tiempo de revisión en el lado correcto de la resta.»*

### Puedes pasar a M6 cuando…

Hay un número con su método, con la resta hecha y con una amenaza nombrada · la prueba ciega está
hecha y barajada por otra persona · la ficha de traspaso pasa su lista binaria · **y hay una persona
con nombre que ha aceptado usar el sistema cinco días la semana que viene.**

---

## 6.8 M6 · Capa 7 — Que lo adopten (semanas 15–17)

Desarrollado entero en §11.

**Cambio mental.** *«Un artefacto que solo funciona conmigo delante no es un sistema de la academia:
es una manía mía. Lo que hace que otros lo adopten no es convencerles: es que puedan usarlo sin mí, y
que yo pueda enseñar el número y decir también qué no hace.»*

**Qué construye.** El **dossier de una cara** · la **demo de tres minutos** guionizada y cronometrada ·
**la semana sin ella** (el piloto) · **la segunda vuelta del Mapa corto** con su delta · la
**conversación del proceso de otra persona** · la **lista de lo que decidió no automatizar** · y **su
propia rúbrica, validada contra el cebo 3**.

**Duración: 3 semanas**, y es el único módulo con una espera que no depende de ella.

**Movilidad declarada** *(injerto I17)*, y va escrita **en la semana 1**:

> **M6 no abre ninguna puerta y nada depende de él.** Si el piloto no se puede hacer en la semana 16
> porque tu compañera está de vacaciones, de baja o desbordada, **M6 se retrasa las semanas que haga
> falta y el curso no se rompe**. Un calendario roto por la agenda de otra persona no es un curso
> abandonado, y conviene tenerlo escrito antes de que ocurra, porque es la clase de cosa que en la
> semana 16 se lee como el final.

---

# 7. LA ESCALERA DE CAPACIDADES DEL PERFIL, Y DÓNDE SE CUMPLE CADA PELDAÑO

El perfil pide una progresión explícita. **Se respeta literalmente, pero no es el plan de estudios: es
lo que le pasa a un proceso cuando lo aprietas.** No se «suben escalones»: se choca con techos dentro
de lo mismo, y el techo se escribe en la Lista de techos el día que se choca con él.

| Peldaño del perfil | Dónde se cumple | Qué lo cierra, observable | Cómo cambian las cinco preguntas |
|---|---|---|---|
| **1 · «Usar mucho mejor el chat que ya tiene. Salir de pregunto y copio»** | M0 (instrucciones permanentes + asistente v1) · M1 (criterio escrito antes del prompt) · M2 (fuentes fechadas, cita, «no lo sé») | Batería 5/5 típicos, aclaración en límite, «no lo sé» en rechazo · **y uso espontáneo ≥5 veces/semana** | P3 pasa de «lo que le pego» a «fuentes que yo controlo y fecho» |
| **2 · «Automatizaciones de tareas sencillas y repetitivas»** | M3 (disparador + tope + apagado + lote) | Cinco casos disparan, el sexto no, el apagado está probado, el tope se ha visto detener | P1 pasa de «yo» a «un reloj» y después a «un suceso»; P2 se congela en «yo, de antemano» |
| **3 · «Agentes, cuando la tarea lo justifique»** | M4 (juicio en 2–3 puntos + frenos + las cinco preguntas sobre un agente real) | Los cinco casos de parada paran; y **la ficha de cinco preguntas rellenada para un agente que el curso no enseñó**, con las tres comprobaciones (plan, permisos, observabilidad) | P2 se abre en dos o tres puntos concretos. **Lo que NO ocurre: P2 no pasa entera al sistema, y se dice por qué** |
| **4 · «Herramientas más avanzadas tipo Claude Code: al final y opcionales»** | Apéndice de lectura, sin entregable | **Ninguno.** Si termina el curso sin abrirlo, el curso ha funcionado igual, y eso va en su primera línea | — |

**Y el peldaño −1, que el perfil no pide y que es la mitad del criterio:** *ni IA*. Se cumple en el
doblete de M1 (P02, presupuestos: aritmética sobre una tabla de precios) y en el veredicto 1 del Mapa
corto. Meter un modelo de lenguaje ahí no es ineficiente: **es introducir un error posible donde no lo
había.**

**Una lectura honesta que va escrita en la semana 1, para que la escalera no le enseñe permanentemente
los peldaños que no va a pisar:** *no vas a montar un agente autónomo en este curso, y no es por ti. Es
por el plan que tiene tu empresa, por los permisos de tu buzón y por los datos que manejas. Las tres
cosas están escritas en la Lista de techos con la condición que las cambiaría. El día que alguna
cambie, tú vas a ser la persona de tu academia que sepa qué preguntarle a ese agente antes de dejarle
tocar nada — que es más de lo que sabe hoy casi nadie que ya los está usando.*

---

# 8. LA SEPARACIÓN CRITERIO / CLICS

No es una recomendación de estilo. Es la convención de producción, y si se relaja, el curso deja de ser
agnóstico en tres módulos.

## 8.1 Tres registros, no dos *(injerto I7, de arq-1 §4.1)*

Dos registros dejan un hueco justo donde está el valor: **cómo encuentras esa función en una
herramienta que nunca has visto**. Por eso son tres.

| Registro | Qué contiene | Dónde vive | ¿Caduca? |
|---|---|---|---|
| **EL CRITERIO** | Por qué se hace así · qué problema resuelve · cómo se decide si toca · cómo se comprueba · qué puede salir mal · el techo | `M3.1-capa.md` | **No** |
| **CÓMO SE RECONOCE EN CUALQUIER HERRAMIENTA** | Descripción funcional de lo que hay que buscar y **las señas que distinguen esta capacidad de otra que se le parece**, con su fallo declarado | En el mismo fichero, en caja aparte | **Casi no** |
| **LOS CLICS** | Rutas, nombres de botón, límites numéricos, capturas | `clics/M3.1-clics-<entorno>.md`, **fechado** | **Sí, y da igual** |

## 8.2 Estructura de ficheros

```
curso/
  M3/
    M3.1-capa.md              ← CRITERIO + CÓMO SE RECONOCE. Sin fecha. Sin nombres de producto
    M3.1-ejercicio.md         ← EL EJERCICIO. Tampoco nombra productos
    M3.1-rubrica.md
    M3.1-solucion.md
    M3-cierre.md              ← LAS CINCO PREGUNTAS + LA PREGUNTA FIJA + EL DOBLETE
    clics/
      M3.1-clics-<entorno-actual>.md   ← fechado, reemplazable
      M3.1-clics-<otro-entorno>.md     ← fechado, para la prueba de traslado
  comun/
    datos-volatiles.md        ← TODO número: cupos, límites, precios, qué edición incluye qué,
                                 y el −3 de la cuarta columna del embudo
    tres-nombres.md           ← la tabla de equivalencias. La única página que caduca entera
    cuando-no-coincide.md     ← qué hacer cuando el manual y la pantalla discrepan
    protocolo-ia.md           ← las siete reglas de corrección con IA
    claves/                   ← claves selladas: batería, dobletes, cebos, codificación de P27
    expediente-modelo/        ← el recorrido completo sobre P27
```

## 8.3 Siete reglas de producción, todas mecánicamente comprobables

1. **Ningún nombre de producto en un fichero de criterio, de ejercicio o de cierre.** Comprobación
   real, no aspiracional: un `grep -iE` con la lista de productos sobre esos ficheros tiene que
   devolver **cero líneas**.
2. **Ningún número volátil fuera de `datos-volatiles.md`.** Actualizar el curso es actualizar un
   fichero, no treinta.
3. **Ningún ejercicio puede depender de una captura ni de una ruta de menú.** Prueba mecánica: se borra
   el directorio `clics/` y **todos los ejercicios siguen siendo enunciables**. Uno que deje de serlo
   está mal escrito y se reescribe. Se ejecuta una vez sobre el material terminado.
4. **La regla del sujeto.** En un fichero de criterio, **el sujeto gramatical de cada frase es el
   proceso, el dato o ella**. Nunca un producto. *«El proceso necesita saber de qué documento sale
   cada dato»* es criterio; *«el asistente admite diez ficheros»* es clic, porque el sujeto es la
   herramienta. Comprobación de tres segundos que puede hacer cualquiera.
5. **La prueba del sustituto.** Sustituye cada nombre de producto por «la herramienta» y relee. Si deja
   de tener sentido, el párrafo pertenece a clics. Si sigue teniendo sentido, **borra el nombre para
   siempre**: no hacía falta. Esta segunda mitad es la que de verdad limpia el texto, porque **el fallo
   típico no es escribir un párrafo de clics en la mitad de criterio: es dejar nombres de producto
   decorativos en frases que no los necesitaban.**
6. **Todo fichero de clics abre con la misma cabecera:** *«Verificado el <fecha> en `<entorno>`. **Si
   algo no coincide con lo que ves, tu pantalla tiene razón y este texto no.** Ve a
   `cuando-no-coincide.md`.»*
7. **Todo fichero de clics termina con la misma línea:** *«Si esto ha cambiado, lo que sigue siendo
   verdad está en `M3.1-capa.md`.»* Es lo que impide que un botón renombrado se lea como que el curso
   entero ha caducado. La cabecera cubre la mitad del problema; esta línea cubre la otra.

**Y `cuando-no-coincide.md`**, media página escrita una vez y referenciada desde todos los ficheros de
clics, convierte la caducidad del material de defecto en **competencia enseñada**: buscar el nombre
nuevo en las novedades del proveedor · comprobar si es restricción de plan o de administrador ·
preguntarle a la propia IA cómo se llama ahora eso y dónde está · y —solo si nada funciona— el comodín
PC-4.

## 8.4 Ejemplo concreto y comprobable: M3.1

### `M3/M3.1-capa.md` — **EL CRITERIO** *(sin fecha, sin nombres de producto, sin capturas)*

> ## Para qué sirve esto en tu proceso
>
> Hasta ahora, tu proceso funciona **cuando tú te acuerdas**. Esa dependencia tiene dos costes que no
> se ven: los días de mucho trabajo —que son justo cuando más falta hace— es el primer sitio donde se
> cae; y no se puede repartir, porque «acordarse» no se delega. Esta capa quita tu dedo de en medio.
>
> ## Qué es un disparador, y por qué es la decisión y no un detalle
>
> Un disparador es **la condición que hace que el trabajo empiece sin ti**. Solo hay dos clases, y la
> diferencia decide qué casos vas a poder atender:
>
> - **Por calendario.** «Cada lunes a las nueve.» Sirve cuando el trabajo se acumula y se puede tratar
>   en lotes. Es el más fácil de razonar, porque siempre sabes cuándo va a ocurrir.
> - **Por suceso.** «Cuando entra algo que cumple X.» Sirve cuando la respuesta tiene que llegar cerca
>   del hecho. Es más útil y más difícil de razonar, porque **no sabes cuántas veces va a ocurrir**.
>
> **Un lunes no es un suceso.** Si tu proceso empieza porque llegó algo, un disparador de calendario te
> obliga a esperar, y esa espera puede ser exactamente lo que hacía valioso el proceso.
>
> ## Las tres cosas sin las cuales un disparador no está terminado
> **1. Un tope.** *Un sistema que produce cuarenta borradores un lunes de julio no ayuda, entorpece.*
> **2. Un apagado que hayas probado.** *Un sistema que no sabes apagar no está terminado.*
> **3. Una salida que prepara, no que envía.** *Automatiza la lectura y la preparación; la escritura
> hacia fuera la firma una persona.*
>
> ## Cuándo NO poner un disparador
> - Si todavía no usas el artefacto por tu cuenta *(esto es una puerta, no un consejo: ver M2→M3)*.
> - Si el proceso ocurre menos de una vez por semana: el coste de montarlo y mantenerlo no se recupera.
> - Si la salida tiene que salir hacia fuera sin que nadie la mire: entonces el problema no es el
>   disparador, es que ese trozo no debería estar en la parte entregable de tu línea de corte.
>
> ## CÓMO SE RECONOCE EN CUALQUIER HERRAMIENTA
>
> 🧭 **Qué estás buscando:** un sitio donde se declare **una condición** y **una secuencia de pasos que
> se ejecuta cuando esa condición se cumple**. Suele estar en un apartado que hable de
> «automatizaciones», «flujos», «tareas» o «reglas».
>
> **Las tres señas de que has encontrado la capacidad correcta:**
> 1. **Puedes elegir la condición de una lista**, no solo una hora.
> 2. **Puedes ver el historial de ejecuciones**: cuándo corrió y qué hizo. *(Si no puedes ver qué hizo,
>    no puedes confiar en ello: es el mismo requisito que le pedirás a un agente.)*
> 3. **Hay un interruptor de activo/inactivo** que tú controlas.
>
> **Si falta la 2, lo que tienes no es una automatización: es una caja negra que se ejecuta.**
>
> ## El techo de esta capa
> Un disparador hace que el trabajo empiece solo, **pero el camino sigue siendo el que dibujaste tú**.
> El caso que no previste sale mal, y sale mal **en silencio**, que es lo peor.
>
> ## Los clics → `clics/M3.1-clics-<tu-entorno>.md`

### `M3/clics/M3.1-clics-<entorno-actual>.md` — **LOS CLICS** *(fechado y reemplazable)*

> *Verificado el 23 de agosto de 2026 en el entorno de trabajo actual. **Si algo no coincide con lo que
> ves, tu pantalla tiene razón y este texto no.** Ve a `cuando-no-coincide.md`.*
>
> **A · Disparador por calendario, sin salir del chat que ya usas.** *(Esta es la ruta principal: no
> requiere consola, ni permiso de administrador, ni licencia extra.)*
> 1. En la aplicación de chat de tu cuenta de trabajo, busca la sección de acciones programadas.
> 2. Escribe la instrucción como si se la dieras a alguien un lunes por la mañana, y fija la
>    frecuencia.
> 3. Límite de acciones activas a la vez → `comun/datos-volatiles.md`.
>
> **B · Disparador por suceso, con la herramienta de automatización de la suite.** *(Ruta ampliada. Si
> no te deja entrar, no es un fallo tuyo: tu administrador no la ha activado, y el curso continúa por
> la ruta A.)*
> 1. Elige el disparador de la lista · 2. Añade los pasos · 3. La salida es **borrador en tu bandeja**,
> fila en una hoja o aviso. **Ningún paso de esta lección envía nada a un cliente.**
>
> **C · Los límites que te vas a encontrar hoy en este entorno** *(y por eso la cuarta columna del
> embudo de la semana 1 descartó los procesos que solo viven en recursos compartidos)*: los flujos
> fallan con unidades compartidas, carpetas compartidas y hojas con referencias externas · un solo
> disparador por flujo · la interfaz muestra un número limitado de etiquetas · tu administrador puede
> tener pasos desactivados y no hay forma de saberlo hasta intentarlo.
>
> **D · Dónde se apaga.** En la misma pantalla donde se crea. **Apágalo y vuelve a encenderlo ahora
> mismo**, antes de seguir: es el ejercicio, no un consejo.
>
> *Cifras y límites → `comun/datos-volatiles.md`. No las copies aquí.*
> *Si esto ha cambiado, lo que sigue siendo verdad está en `M3.1-capa.md`.*

**Qué demuestra el ejemplo:** la mitad de criterio ocupa el doble que la de clics, **no menciona ni una
vez el nombre de ningún producto**, y seguiría siendo válida palabra por palabra si su empresa cambiara
de proveedor. La mitad de clics es sustituible en veinte minutos por alguien que no haya escrito el
curso. Y nótese la costura del apartado C: **el límite concreto está en clics; la instrucción de
comprobarlo antes de diseñar está en criterio.**

## 8.5 Las dos pruebas de traslado

**Nº 1 — M2, 25 minutos, tiempo propio, con material verde exclusivamente.**
Reconstruye el mismo asistente en otra herramienta —ella ya usa ChatGPT por su cuenta— usando **solo
tarifario, calendario y condiciones generales, que no son datos personales**. Pásale las mismas diez
preguntas. Rellena la ficha:

| Qué viajó tal cual | Qué hubo que rehacer | Qué techo cambió |
|---|---|---|
| La ficha de criterio · las fuentes con fecha y dueño · la batería · la regla de «no lo sé» · la línea de corte | Dónde se guarda · cómo se llama · cuántos ficheros admite · dónde se pega la instrucción | Cuántas fuentes acepta · si cita el fragmento o solo el fichero · si conserva la instrucción entre sesiones |

> **Lo que se aprende no es «la otra herramienta también sirve». Es que el ochenta por ciento de tu
> trabajo era el criterio y las fuentes, y eso no estaba dentro de ninguna herramienta.**
>
> **Restricción de datos, y es contenido, no prudencia decorativa:** su cuenta personal no tiene
> contrato de encargado del tratamiento y por ahí no pasa ni un dato de un alumno. Que la prueba de
> traslado sea también un ejercicio de semáforo no es casualidad: es el diseño.

Criterio negativo: *si la columna «qué viajó tal cual» está vacía, no construiste criterio: construiste
un prompt.*

**Nº 2 — M3, 20 minutos, sobre papel y documentación, sin dar de alta ninguna cuenta**
*(injerto I9, de arq-2)*.
Escribe tu disparador en **notación neutra** —`DISPARADOR → PASO → PASO → CONDICIÓN → SALIDA`— y
localiza cada pieza en la documentación de **otra** herramienta de automatización. Entregable de tres
líneas: **las cinco piezas y su nombre allí** · **la pieza que allí no existe** · **la pieza que allí es
más fácil**.

> No se construye nada y no se da de alta nada. El objetivo es doble: que compruebe que su flujo es
> describible sin nombrar un producto, y **que localice el catálogo de pasos de una herramienta que no
> ha visto nunca**. Esa segunda habilidad es la que usará dentro de tres años, y protege la
> agnosticidad exactamente en el tramo (M3–M4) donde el material se vuelve más específico de
> plataforma, que es donde arq-3 solo tenía una prueba y con material verde.

## 8.6 La tabla de tres nombres

Vive en `comun/tres-nombres.md`, es **la única página del curso donde conviven nombres de producto**, y
su función no es enseñar productos: es **desactivar el miedo del principiante a quedarse casado con una
herramienta** — el freno mejor documentado del Q&A de la referencia, preguntado tres veces con
distintas palabras.

| Capacidad (lo que dura) | Nombre hoy, A | Nombre hoy, B | Nombre hoy, C |
|---|---|---|---|
| Contexto que se aplica a todas las conversaciones | Instrucciones personalizadas | Instrucciones personalizadas | Preferencias |
| Asistente guardado con instrucciones propias | Gem | GPT personalizado | Proyecto |
| Fuentes propias con cita del fragmento | Cuaderno de fuentes | Ficheros de conocimiento | Ficheros del proyecto |
| Algo que ocurre por horario sin que lo pidas | Acción programada | Tarea programada | Tarea recurrente |
| Flujo con disparador por suceso | Automatización nativa de la suite | Plataforma externa | Plataforma externa |
| Acceso acotado a una fuente | Conector | Conector | Conector / MCP |

> **Nota fija al pie, y es la que hace el trabajo:** *«Esta tabla es la única página del curso que
> caduca por completo. Está fechada. Cuando algún nombre no coincida con tu pantalla, corrígelo tú: es
> tuya. Lo que no cambia es la columna de la izquierda.»*

---

# 9. «SABER QUÉ EXISTE», Y CÓMO SE ENSEÑA A NO USAR IA

## 9.1 El objetivo 1, con cuatro mecanismos y ningún listado de productos

El objetivo 1 del perfil es *«saber qué existe: que existen agentes, que existen automatizaciones, qué
se puede automatizar de su trabajo y qué no»*. Los tres términos van pegados a **su trabajo**. No pide
un mapa del sector: pide saber qué hay disponible para lo que ella hace. Un curso que conteste con un
recorrido de productos está contestando a otra pregunta, y además contesta con la mitad que caduca.

**Éste era el objetivo peor servido por la columna vertebral elegida**, y los cuatro mecanismos que
siguen son la reparación. Los dos primeros son injertos.

**Mecanismo 1 · El Mapa corto y su segunda vuelta** *(injerto I4, §4.5)*. **Veinticuatro
clasificaciones** de tareas suyas, doce en la semana 1 y doce en la semana 17, con la rejilla cerrada de
seis destinos + zona prohibida. El catálogo se aprende porque hay que usarlo veinticuatro veces sobre
su propio trabajo, y el delta entre las dos pasadas es la prueba de que el criterio se ha movido. Coste:
una hora en total.

**Mecanismo 2 · Los siete dobletes con clave sellada** *(injertos I3 e I12, §4.4)*. Siete juicios más,
cada uno emitido **inmediatamente después de haber hecho esa misma cosa de verdad**, sobre nueve
procesos que no son el suyo, y contrastados contra una clave que ella no ha escrito. Coste: dos horas y
media.

**Total: treinta y un juicios sobre procesos reales en menos de cuatro horas.** Es el mismo orden de
magnitud que produce una arquitectura de inventario en cuatro semanas de trabajo árido, y se paga en
cuotas de veinte minutos repartidas por todo el curso.

**Mecanismo 3 · La Lista de techos** *(§4.6)*. El catálogo no se enumera: **se genera**, una fila cada
vez que el proceso choca con un techo. La tercera columna —la condición de activación— es la que
convierte un catálogo en criterio, porque las condiciones no caducan aunque los productos sí. Y la fila
del agente se escribe en la capa 4, cuando ya tiene un sistema con juicio en dos puntos y entiende
exactamente qué le falta. Antes de eso, «agente» es una palabra; ahí es una carencia concreta con
nombre.

**Mecanismo 4 · La caja del fondo, una sola vez, en M4 y no antes.** Media página, con el eje puesto en
la **condición** y no en el producto — que es la diferencia entre una tabla que hay que rehacer cada año
y una que se revisa.

| Qué haría falta para que me tocara | La clase de cosa que lo haría | Qué es hoy, para reconocerlo si me hablan de ello |
|---|---|---|
| Tener que tocar un sistema que no está en mi suite (software académico, pasarela de pago, mensajería, portal de una agencia) | Una plataforma de automatización externa | Ojo: mete un proveedor más entre mis datos y yo, y eso hay que pesarlo |
| Tener una tarea cuyos pasos no pueda dibujar de antemano | Un agente: le das objetivo y límites y decide los pasos | Están detrás de planes que mi empresa casi con seguridad no tiene, y necesitarían tocar recursos compartidos |
| Necesitar que una herramienta lea de una fuente mía con permisos acotados | Un conector, y el estándar por el que se conectan | Para mí hoy es **vocabulario, no herramienta**. Lo que sí me sirve es el principio: **conectar solo a lo necesario, y a una carpeta, no al disco** |
| Tener que procesar decenas de ficheros locales de forma repetida | Un agente con acceso al sistema de ficheros | Revisar doscientos contratos de estancia larga buscando una cláusula sería el caso |
| Que las fuentes pasen de decenas a cientos y el asistente empiece a perderse | Arquitecturas de recuperación sobre corpus grandes | Con veinte fuentes bien fechadas no me hace falta nada de eso |
| Que me hablen de un sitio «de la misma empresa, gratis, donde se prueban prompts» | Una superficie de desarrollador | **Trampa silenciosa:** sus propios términos dicen que no metas información personal. Parece seguro porque entras con la cuenta de siempre, y no lo es |

**Y una decisión deliberada: el agente autónomo no está en la lista de destinos posibles para su
proceso.** Se define, se explica y se le pone su condición de activación en M4, pero no es una opción
que ella pueda elegir para su tarea, y eso se dice con todas las letras. El motivo es pedagógico y
verificable: **el error número uno al clasificar es poner «agente» a todo**, porque es la palabra que
suena a solución completa y es lo que promete internet. Sacarlo de la lista obliga a decidir entre lo
que sí existe para ella.

**Hasta dónde llega esto, honestamente.** Cubre lo que su proceso toca, lo que su semana contiene y lo
que los dobletes rozan. **No cubre** el panorama del sector ni le da una opinión informada sobre
familias de herramientas que no ha visto. Si en dos años le preguntan en una entrevista «¿qué
herramientas de automatización conoces?», la respuesta honesta de este curso es *«conozco la anatomía y
sé leer el catálogo de pasos de una que no he visto nunca, y sé qué preguntarle antes de dejarla tocar
algo»* — que es mejor respuesta de lo que parece, pero no es la que da un curso de panorama.

## 9.2 Cómo se enseña a NO usar IA cuando no toca

Siete mecanismos, de más estructural a más operativo. **Ninguno es una advertencia suelta, y los siete
producen algo que se puntúa** — porque lo que no se evalúa, no se hace.

**1 · La línea de corte: el «no» es interior al proceso.** Es el mecanismo propio de esta columna
vertebral y el más fuerte de los siete. El entregable central de M1 no es «qué automatizo» sino **el
proceso partido en trozos, cada trozo con veredicto y motivo**, y la rúbrica es tajante: *si no hay
ningún trozo que se quede contigo, está mal resuelto*, y *si el motivo es «es difícil», está mal.*

**2 · La lista cerrada de cinco motivos, que es lo que hace transferible cada «no».** Una prohibición
sin motivo no se transfiere a un caso nuevo; **un motivo tipificado se comprueba contra una lista y se
aplica a un proceso que nunca has visto.**

| Motivo | Qué significa | Ejemplo de su casa |
|---|---|---|
| **Riesgo** | El error lo paga un cliente, una administración o la caja | Cualquier trozo que toque importes, plazos de visado o disponibilidad de alojamiento |
| **Conocimiento que caduca** | La regla cambia más deprisa de lo que se puede mantener el artefacto | Requisitos consulares, que se reordenaron en 2025 y volverán a cambiar |
| **No hay fuente de verdad** | Nadie puede nombrar el documento vigente ni su dueño | El tarifario en alemán, que lleva meses desactualizado y nadie lo sabe |
| **Las reglas son de otro** | El procedimiento, los plazos y la plataforma los fija una institución ajena | La inscripción y las tasas de los exámenes oficiales, que van por la plataforma del Instituto Cervantes, con plazos rígidos que no se recuperan |
| **No necesita un modelo** | Necesita una fórmula, una plantilla o un calendario | El presupuesto: aritmética sobre una tabla de precios. **El escalón −1** |

**3 · La regla del cuatro, apilada con las otras dos capas** *(§0.2, punto 4)*. Los jueces se
contradicen aquí y la resolución es apilar:

- **Descalificadores aritméticos, gratis y sin criterio:** P08, P17, P22, P25, P26 y P29 salen del Mapa
  corto con tachón de zona prohibida por número de proceso. No hay nada que juzgar.
- **Motivos tipificados contra lista cerrada** para todo veredicto 1 y 2.
- **Y la cuota, reforzada:** *de tus doce filas, al menos cuatro tienen que acabar en veredicto 1 («ni
  IA») o 2 («arreglar el proceso primero»). **Las zonas prohibidas no cuentan para los cuatro**, porque
  esas son aritmética y salen gratis. Si tienes menos de cuatro, no has clasificado: has hecho una lista
  de deseos.*

Excluir las ZP de la cuota es la corrección que la hace exigente en vez de decorativa: obliga a
encontrar los noes que **sí** requieren juicio. Y la rúbrica lleva la señal de fallo que busca el
autoengaño de frente: *«existe un veredicto 1 o 2 que puse para llegar a cuatro, no porque lo crea».*
Eso sigue dependiendo de su honestidad consigo misma, y es la limitación que reconozco en §17.

**4 · El caso canónico se hace, no se prohíbe.** El presupuesto (P02) se monta **con IA** y **con
fórmula** sobre los mismos veinte casos, se cronometra y se cuentan los errores. Gana la fórmula por
goleada. **Enseñar el «no» haciendo el «sí» y midiendo que pierde es infinitamente más fuerte que
prohibirlo.**

**5 · Las zonas prohibidas, con el motivo y no solo la prohibición:**

| Proceso | Por qué no, dicho de forma transferible |
|---|---|
| **P08** carta de aceptación para visado | Riesgo crítico y **normativa viva**. **Congelar dentro de un artefacto un conocimiento que caduca es fabricar un error futuro** |
| **P26** quejas formales | Una respuesta que **admite responsabilidad por escrito compromete a la empresa**. Y los modelos son complacientes: la complacencia por escrito, en una queja, es exposición legal |
| **P29** emergencias 24 h | Personas, menores, responsabilidad civil, y un alumno en estado de shock con nivel A1 |
| **P25** reembolsos | Datos bancarios y riesgo de fraude por suplantación en el cambio de cuenta |
| **P17** matching con familia de acogida | Concentra **salud, religión y potencialmente orientación sexual** en una casilla de texto libre. Es el proceso que **más parece** el caso ideal de IA, y por eso es la trampa |
| **P22** calendario de camas | Riesgo crítico por overbooking, y además es un calendario de recursos: escalón −1 |
| **P05 / P16** nivelación y exámenes | **Anexo III del Reglamento de IA**: *evaluar el nivel educativo* es alto riesgo. Aplazado, **no cancelado**. Lo suyo no es decidirlo **[!]**: es reconocerlo y avisar |

Y la regla de oro que hace todo esto memorable, y que se recuerda cuando una lista de artículos no:

> **De todo su trabajo, el único trocito que está en la lista de alto riesgo es el que decide el nivel
> de un alumno. Todo lo demás —redactar, traducir, resumir, clasificar, preparar borradores— no lo
> está.** Esa asimetría se recuerda.

**6 · El coste completo como criterio de descarte, no como cálculo de justificación** (M5). *Un sistema
que ahorra ocho minutos y cuesta diez de revisión es una pérdida disfrazada de modernidad.* Y la métrica
de vanidad tiene nombre: **que se ejecute cada lunes no es que funcione.**

**7 · La opción segura suele ser también la más eficiente, y eso se demuestra, no se predica.** El mejor
ejemplo, y va en M2: **no transcribas la llamada.** Escribe tú un resumen de cuatro líneas al colgar, ya
seudonimizado, y trabaja con ese resumen. Es más rápido que subir un audio de doce minutos, no genera un
tratamiento nuevo ni un destinatario nuevo, y de paso piensas el caso. Enseñado así, «no usar IA» deja
de ser una renuncia y pasa a ser una decisión de eficiencia.

**Y un octavo, incómodo: el «no» a la propia arquitectura.** El checkpoint de divorcio de M1 autoriza
por escrito, desde la semana 1, a cambiar de proceso. **Un curso que no permite abandonar una decisión
suya no puede pedirle a ella que abandone las suyas.**

---

# 10. PROTECCIÓN DE DATOS, INTEGRADA

## 10.1 El principio de diseño

Un módulo de protección de datos se lee una vez, se aprueba y se olvida. Y además produce parálisis,
cuando el objetivo es que **use más la IA, no menos: que la use en el sitio correcto.** Un bloque de
protección de datos que produce parálisis ha fallado.

Pero «transversal» tampoco basta como respuesta, porque suele significar «repartido y por tanto de
nadie». Aquí la protección de datos tiene **cuatro anclajes concretos**, y ninguno es un anexo:

| Anclaje | Dónde | Qué contiene | Por qué exactamente ahí |
|---|---|---|---|
| **En el instrumento con el que se clasifica cualquier herramienta** | Instrumento 1, todo el curso | **Las preguntas 4 y 5 de la ficha son literalmente protección de datos**: *¿qué puede tocar? ¿quién firma la salida?* No se puede clasificar un sistema sin contestarlas | Porque así el régimen de datos **se deriva de la clasificación** en vez de pegarse al final. Quien contesta las cinco ya sabe qué salvaguardas necesita |
| **En el criterio con el que se elige el proyecto** | M0, embudo, columna 2 | El semáforo, con **−3 que descalifica** para rojo irreducible | Porque así la protección de datos no llega a frenar el proyecto: **decide cuál es el proyecto** |
| **En el momento en que le mete datos** | M2, antes de cargar fuentes | El **mapa de datos del proceso** (§10.2) · por qué quitar el nombre no basta · cuasi-identificadores · la prueba de la compañera · la regla de los adjuntos | Es el momento exacto en que pasa de **pegar texto** a **subir ficheros**. Al pegar ves lo que envías; al adjuntar, no. Un Excel va **completo** —todas las filas, las columnas ocultas, la hoja que se llama «datos antiguos»—, un PDF de pasaporte va entero, una foto lleva coordenadas |
| **En el momento en que algo actúa sin que ella mire** | M4, con los frenos | Temas prohibidos · condiciones de parada · *nada sale al cliente sin que un humano le dé a enviar* · el deber de avisar de que es una IA · registro de qué se generó y quién lo aprobó · plan para el día que falle, **incluido valorar si hay brecha [!]** · el Anexo III aplicado a su academia | Antes de M4 no hacía falta; después de M4 sería tarde |

**Capa permanente:** la **tarjeta del lunes** impresa al lado de la pantalla desde la semana 1, con seis
preguntas que caben en una nota adhesiva. *Si una regla necesita que te pares a pensar, no sobrevive a
un martes de julio con trescientos correos sin abrir.*

## 10.2 El artefacto propio: el mapa de datos del proceso

Un semáforo genérico se lee y se olvida. **Un semáforo aplicado al único proceso que está construyendo
se usa**, porque contesta una pregunta que tiene delante. Una cara, cuatro columnas:

| Dato que atraviesa el proceso | Color | **En qué paso entra** | **Dónde hay que quitarlo, y quién lo quita** |
|---|---|---|---|
| Nombre y apellidos del alumno | Ámbar | En el correo entrante | Antes de pegar nada: lo quito yo, a mano |
| Nacionalidad + edad + fecha de llegada + barrio | **Ámbar peligroso** | En el cuerpo del correo | Se **generalizan**, no se borran: «alumno», «esta semana», «familia de acogida». Combinados identifican a una persona entre 1.400 |
| Nº de pasaporte o NIE | **Rojo** | Adjunto en la reserva | **No entra nunca**, ni imagen ni PDF. Si necesito un dato de ahí, lo escribo yo a mano, y solo ese |
| IBAN, tarjeta, justificante de pago | **Rojo** | Adjunto o cuerpo | **No entra nunca**, en ninguna herramienta |
| Alergia, dieta médica, medicación | **Rojo** | Formulario de preferencias | **No entra nunca**, ni seudonimizado. Se degrada al mínimo funcional si el texto lo exige: «una intolerancia alimentaria» |
| Cualquier dato de un **menor** | **Rojo absoluto** | Grupos escolares, estancias de 16–17 | **Nunca, en ninguna herramienta, ni seudonimizado.** Sin excepciones |
| Dirección del alojamiento junto al nombre | **Rojo** | Confirmación de alojamiento | No entra. Localiza físicamente a una persona |
| Tarifario, calendario, condiciones, plantillas | **Verde** | Documentos de la academia | **No son datos personales.** Entran sin pensar, y por eso el proceso puede empezar aquí |

**Cuatro cosas que este artefacto hace y un semáforo genérico no:**

1. **Sitúa el punto de corte en el flujo, que es lo que convierte la regla en un gesto.** Saber que un
   pasaporte es rojo no cambia nada un martes; saber que **el pasaporte entra como adjunto en el paso
   dos y por eso el paso dos nunca sube el adjunto original**, sí.
2. **Nombra quién lo quita.** Si la respuesta no es una persona o un paso concreto, no hay corte: hay una
   intención.
3. **Es reutilizable como hábito portátil.** Un mapa de datos por proceso vale en cualquier empresa y en
   cualquier año, y no menciona ninguna herramienta.
4. **Muestra que la mayoría de su proceso empezó en verde**, que es el mensaje que evita la parálisis: la
   protección de datos no le prohíbe trabajar, **le dice por dónde empezar**.

## 10.3 El ejemplo de reidentificación, que es de su casa

> ❌ *«La alumna coreana de 19 años que llegó el 3 de julio y está alojada con la familia de Chamberí
> dice que la comida no le sienta bien y que es celíaca.»*

No hay ni un nombre. Y **cualquiera de sus tres compañeras sabe de quién se habla en dos segundos.** Con
1.400 alumnos al año, nacionalidad + edad + fecha + barrio deja **una sola persona**. Y encima hay un
dato de salud.

> ✅ *«Un alumno de nivel A2 comunica una intolerancia alimentaria no registrada en su ficha inicial y
> pide cambio de régimen de comidas. Redáctame un correo a la familia de acogida explicando el cambio,
> en español, tono cordial y directo, máximo 120 palabras.»*

**La prueba que hay que memorizar, una sola:** *«¿podría una compañera mía saber de quién hablo leyendo
esto?»* Y el criterio del otro lado, que casi nadie pone: **el prompt resultante tiene que seguir
sirviendo.** Si la respuesta es inservible, ha quitado contexto que no era identificador — ése es el
error del otro lado y también hay que verlo.

## 10.4 La corrección obligatoria sobre P08 *(aceptada del juez 4, §0.2 punto 6)*

Hay una versión tentadora y equivocada del «lo que sí se puede hacer alrededor» de las cartas de visado:
*montar la comprobación que caza el nombre mal transcrito desde el pasaporte*. **Eso mete un documento
de identidad en la herramienta, y el pasaporte es rojo absoluto: nunca, en ninguna herramienta, ni
imagen ni PDF.**

**La versión admisible, y ataca el mismo mecanismo de error:** una **comprobación determinista de
consistencia entre campos que ella ya ha tecleado a mano** — que el nombre, la fecha de nacimiento y las
fechas del curso coincidan carácter a carácter entre el expediente, la carta, la factura y el
certificado. Es el error documentado de P04: *un nombre transcrito mal desde el pasaporte reaparece en
la carta de visado, en el certificado y en la factura, y obliga a rehacerlo todo.* La comprobación
funciona igual de bien sin que el documento de identidad entre en ningún sitio, **y encima no necesita
un modelo de lenguaje: es una comparación de cadenas.** Escalón −1.

Esta corrección es además **el mejor ejemplo del curso** de que «lo que sí, alrededor» no es un premio
de consolación: es la reformulación que convierte un no en un artefacto.

## 10.5 Las cinco decisiones que hacen que esto funcione y no asuste

1. **La regla de los menores es tajante y sin excepciones**, más restrictiva de lo que la norma exige en
   todos los supuestos, **a propósito**: una regla con excepciones no sobrevive a julio.
2. **Cada decisión que no es suya va marcada [!] y con el nombre de a quién se escala.** El riesgo
   específico de este perfil es que, por ser la que más se preocupa, acabe siendo de facto la
   responsable de cumplimiento de la academia. El material lo prohíbe explícitamente: *tu papel no es
   ser la responsable de cumplimiento; tu papel es no ser tú el agujero, y saber cuándo hay que
   levantar la mano.* Los tres límites concretos: **no decide la base jurídica, no decide si hace falta
   una evaluación de impacto, no decide si hay brecha notificable.**
3. **Nada normativo se congela dentro de un artefacto.** Las fechas del Reglamento de IA, el estado del
   marco de transferencias y la ley española viven en un fichero **con fecha visible** que se revisa. Y
   eso es, además, el mejor ejemplo pedagógico del curso de la diferencia entre conocimiento estable y
   conocimiento volátil — que es exactamente la distinción que hay que dominar para construir fuentes
   que no envejezcan mal.
4. **El encuadre no es de permiso, es de aportación.** No está pidiendo autorización para nada: ya usa la
   herramienta, se la ha dado su empresa, y usarla está bien visto. Está entendiendo la configuración
   antes de apoyarse en ella. Si la academia nunca se lo ha planteado, **acaba siendo ella quien propone
   la política**, y eso no es venta interna: es su propio trabajo.
5. **La transición con su cuenta personal se resuelve sin moralina**, porque la moralina no cambia
   hábitos y además sería injusta: lo que hace es lo que hace casi todo el mundo. Línea limpia —cosas
   suyas y prácticas con casos inventados, en la personal; **cualquier cosa que venga de un correo, una
   llamada o un expediente de un cliente**, en la de empresa— y el argumento que de verdad convence, que
   no es «es ilegal»:

   > **Si mañana un alumno ejerce su derecho de supresión y la academia tiene que certificar que ha
   > borrado sus datos de todos los sitios, tu cuenta personal es un sitio que la academia no puede
   > tocar y del que ni siquiera sabe que existe.** No es que hayas hecho nada malo: es que has creado,
   > sin querer, un almacén de datos de clientes fuera del alcance de la empresa. Y eso, cuando aparece,
   > no tiene arreglo posible: no se puede desandar.

## 10.6 El dato que cambia la posición mental con la que se estudia esto

Merece salir en la primera página del curso: **el artículo 4 del Reglamento de IA, en vigor desde
febrero de 2025, obliga a las empresas que usan IA a garantizar un nivel suficiente de alfabetización en
IA de su personal.** Dicho de otro modo: **el curso que está haciendo es, técnicamente, cumplimiento
normativo de su empresa.** No es un extra que se paga a sí misma en su tiempo libre por pura iniciativa:
es una obligación de la academia que ella está cubriendo.

---

# 11. EL MÓDULO DE EVANGELIZACIÓN INTERNA (M6)

## 11.1 Qué NO es, dicho primero porque es donde se estropea

- **No es conseguir el sí.** No hay autorización que pedir. En su empresa usar IA ya está bien visto y
  lo mal visto es no automatizar. Un módulo de venta interna resolvería un problema que ella no tiene y
  le robaría tres semanas a los que sí tiene.
- **No es marketing personal.** Nada de portfolio, nada de landing, nada de «mira lo que tengo ahora en
  mi CV». Ese es el destino del itinerario no técnico de la referencia porque su alumno tipo quiere
  cambiar de sector. La nuestra no — aunque sí quiere que lo aprendido le sirva si algún día cambia de
  empresa, y de eso se encarga la portabilidad del criterio, no una web.
- **No es la columna vertebral.** Son tres semanas al final, alimentadas por tres líneas por capa. Si
  fuera la lente del curso entero, el curso dejaría de ser sobre su trabajo y pasaría a ser sobre su
  reputación, y **el criterio se contaminaría**: elegiría lo vistoso sobre lo útil.
- **No es evangelizar una idea.** El objeto de la adopción no es «deberíamos usar IA»: es **una cosa
  concreta que ya funciona y que otra persona puede usar**.

## 11.2 Qué es: el enunciado del módulo

> **Demostrar y arrastrar.** Su empresa empuja la IA sin saber bien qué se puede hacer. Lo que cambia esa
> situación no es un argumento: es **una cosa que funciona, un número que se puede reproducir, y una
> segunda persona que la usa sin ella delante.** Este módulo produce esas tres cosas.

Y el principio que lo ordena entero:

> **La credibilidad se compra con los noes.** Quien llega diciendo *«estas cuatro cosas NO deberían
> automatizarse, y aquí está por qué»* consigue que le crean sobre la quinta. Quien llega diciendo que
> todo se puede automatizar consigue que no le crean sobre nada — y ésa es, exactamente, la posición en
> la que su empresa está hoy respecto a la IA.

**La ventaja específica de esta columna vertebral:** el módulo **no tiene que fabricar su materia
prima**. Llega con un sistema que lleva tres meses en producción sobre su mesa, con una Tira de seis
columnas fechadas, con un número medido contra una línea base tomada **antes** de construir nada, y con
una lista de noes razonados que sale del Mapa corto sin trabajo extra. Eso no es una demo: es un
historial.

## 11.3 El hilo barato que lo hace posible: el Cuaderno de evidencias

Tres líneas al cerrar cada capa, el día que el artefacto empieza a funcionar. Coste: dos minutos.

```
CAPA __ · fecha ______
- Qué hacía yo antes, y cuántos minutos por unidad:
- Qué hace ahora, y cuántos minutos por unidad:
- Qué NO hace, y qué sigo haciendo yo:
```

Existe desde la semana 3 por una razón operativa, no ceremonial: **si M6 tuviera que fabricar las
pruebas al final, las inventaría.** Un número reconstruido de memoria en la semana 15 no es un número. Y
la tercera línea —*qué NO hace*— es la que después hace creíble a todo el dossier: quien enumera los
límites de su propio sistema se gana el derecho a que le crean el resto.

## 11.4 Qué enseña — ocho piezas, todas con artefacto

**(1) El número y su método, que van juntos o no va ninguno.** De M5 sale un ahorro en minutos por
unidad, con el coste de revisión restado y con una amenaza a la validez que no se puede descartar. **Las
tres cosas se presentan juntas.** Un número sin método es una promesa, y una promesa que no se cumple
quema los tres proyectos siguientes. Aquí su formación es una ventaja competitiva directa y hay que
decírselo así: casi nadie que presenta resultados de IA en una empresa sabe decir *«esto podría
explicarse también porque septiembre no es julio»*, y decirlo es precisamente lo que hace que se crean
el resto.

**(2) Lo que el artefacto NO hace.** Es la tercera línea del Cuaderno de evidencias y en el dossier va en
su propio apartado, no en letra pequeña. Doble función: es honestidad, y es **gestión de expectativas
operativa** — si el dossier dice «no responde nada sobre visados y para en cuanto aparece el tema», la
primera pregunta incómoda ya está contestada antes de que la hagan.

**(3) La lista de lo que decidió no automatizar**, con el motivo tipificado. Sale de la segunda vuelta
del Mapa corto: son las filas con veredicto 1, 2 y ZP. **Es la pieza que le da credibilidad a todo lo
demás**, y no cuesta escribirla: ya está escrita.

**(4) La demo de tres minutos.** No una presentación: **un antes y un después con un caso real, elegido
delante y no preparado**, y un número. Se enseña **también dónde falla** y qué salvaguarda lo cubre —
contraintuitivo y cierto: mostrar el fallo es lo que convierte una demo en algo creíble, y es la única
forma de que quien la adopte sepa dónde mirar. Y se termina siempre igual: *«si quieres, te lo dejo
montado para lo tuyo y te paso la hoja de cómo se usa.»* Sin esa frase, la demo es entretenimiento.

**(5) La prueba del pasillo.** Explicar qué hace, qué ahorra y **qué no hace**, en treinta segundos y
**sin nombrar ninguna herramienta**. Regla de vocabulario dura: se nombra el resultado, no la
tecnología. No *«monté un flujo con un paso de extracción que llama a mi cuaderno de fuentes»*, sino
*«los correos de admisiones llegan ya clasificados y con un borrador hecho, y me ahorra unos ocho
minutos por correo; los de visado no los toca, los deja para mí»*. Esta regla es además la vacuna
contra el efecto que más daño hace a un evangelizador interno: **sonar a que ha descubierto una
religión**.

**(6) LA SEMANA SIN ELLA — el corazón del módulo.** Una compañera usa el artefacto **cinco días
laborables, sin ella delante**. No una demostración acompañada: uso real, sola.

Es el único test verdadero de adopción y produce siempre el mismo hallazgo, que es lo que lo hace
valioso: **una parte del artefacto era ella.** Instrucciones implícitas, decisiones que tomaba sin darse
cuenta, un fichero que solo ella sabe dónde está, un criterio que nunca escribió porque le parecía
obvio. Lo que el piloto revela es exactamente lo que hay que arreglar para que la cosa sobreviva a sus
vacaciones — **y sobrevivir a sus vacaciones es literalmente la definición operativa de que la
organización lo ha adoptado**, en un negocio donde agosto vacía la oficina y julio la desborda.

El entregable del piloto **no es «salió bien»**: es la **lista de lo que hubo que arreglar**, y tiene que
tener **al menos dos entradas**. *Si el piloto no reveló nada, no fue un piloto: estuviste mirando por
encima del hombro.*

**(7) La ficha de traspaso**, que viene ya hecha de M5 y aquí se entrega de verdad. Es lo que convierte
«una cosa que hizo ella» en «una cosa que tiene la academia». Y es también protección propia: un
artefacto sin dueño y sin fecha se degrada, y cuando se degrada el recuerdo que queda no es «faltaba
mantenimiento», es «aquello de la IA no funcionaba».

**(8) La conversación del proceso de otra persona** — la semilla de contagio, y a la vez el séptimo
doblete. Veinte minutos con una compañera, aplicando **solo la capa 0** a un proceso de ella: qué lo
dispara, qué documentos abre, qué decisiones toma que no están escritas, qué sale y a dónde va. **No se
construye nada y no se promete nada.** Se escribe la descripción en una página y se le devuelve para que
la corrija.

Por qué esto contagia y una presentación no:
- **Es la técnica que ella ya sabe hacer y que un perfil técnico no puede aportar**: entrevista
  semiestructurada, estructura de embudo, preguntar por el último caso concreto y no por la norma,
  preguntar por la excepción, y devolver el procedimiento escrito para que lo corrijan — **porque
  corrigiendo se saca más que preguntando**.
- **El encuadre que funciona no es «quiero automatizar tu tarea»** —eso pone a cualquiera a la
  defensiva— **sino «quiero aprender a hacerlo yo bien para no molestarte cada vez»**. Y es verdad,
  además.
- Y produce el efecto que ningún dossier produce: **la otra persona ve su propio proceso escrito por
  primera vez. Ahí es donde alguien pide algo.**

## 11.5 Las cuatro reglas de arranque

| Regla | Por qué |
|---|---|
| **Empieza por un proceso que no sea de nadie** | Un proyecto que mejora la tarea de una compañera empieza con una persona a la defensiva; uno que hace lo que nadie hacía empieza con cero resistencia. **La elección del primer proceso es el 80 % de su adopción**, y por eso el embudo de M0 no era solo una cuestión de riesgo |
| **Enseña el resultado, no el proceso** | La primera vez se enseña lo que sale, no cómo se hizo. El «cómo» se cuenta cuando alguien lo pide, que es la señal de que ya hay adopción |
| **Ofrece el trabajo, no la herramienta** | *«Te paso el resumen de las incidencias de alojamiento de este mes»* gana siempre a *«te enseño a montar un clasificador»* |
| **Deja que lo pidan** | La segunda persona no se recluta: aparece cuando ve el primer resultado. **Si a las tres semanas nadie ha pedido nada, el artefacto no era tan útil como parecía — y eso también es un resultado del curso**, no un fracaso personal |

## 11.6 La deuda de adopción, y el riesgo de acabar siendo «la de la IA»

Es la parte que ningún material de este tipo incluye y que en una empresa de treinta personas donde lo
mal visto es no automatizar **va a pasar**:

- **No entregues lo que no puedas mantener.** Todo lo adoptado tiene coste de mantenimiento, y lo paga
  ella. Un flujo que se rompe en julio, con 400 correos al día, no es valor: es un problema que se ha
  creado ella misma y encima con público.
- **Entrega el artefacto y el manual, no el servicio.** La frase que marca el límite: *«esto lo monté yo
  y así se mantiene; si quieres uno para lo tuyo, aquí está cómo se hace.»*
- **El bus factor invertido:** si es la única que sabe cómo funciona, la organización no adopta el
  artefacto, **la adopta a ella**. La ficha de traspaso es la contramedida, y por eso es entregable.
- Es la versión gemela del límite de rol de protección de datos, y se nombra con la misma regla: *tu
  papel no es hacerte cargo de todo; es no ser tú el agujero y saber cuándo levantar la mano.*

## 11.7 Cómo se autocorrige — el punto donde este módulo se juega su credibilidad

Es el módulo más difícil de autocorregir de los siete, porque su criterio de éxito es **la conducta de
otras personas**, que ella no controla. Decirlo es obligatorio. Y aun así hay seis mecanismos, cinco de
ellos comprobaciones y no juicios:

1. **El piloto es el corrector, y es binario.** Otra persona lo usó cinco días laborables sin ella, o no
   lo usó. Se cuenta. Y el entregable es la lista de arreglos, con al menos dos entradas. **Es un test
   que se provoca en vez de esperarse**, y por eso es mejor que preguntar a las dos semanas si alguien
   lo usó espontáneamente — pregunta que admite un sí falso por cortesía.
2. **La reproducción del número** *(injerto I13)*. Dos semanas después de medir, con la ficha de método
   delante, vuelve a calcular. **Si no sale el mismo número ±10 %, el número no era reproducible y el
   dossier se reescribe.** Test-retest de su propio instrumento, sin consumir a nadie.
3. **La prueba del pasillo, cronometrada**, con cuatro comprobaciones binarias: *¿nombré alguna
   herramienta? ¿la otra persona pudo repetirme qué hace? ¿dije un número? ¿dije qué NO hace?*
4. **Rúbrica del dossier, con criterios negativos y salida escrita obligatoria** (sin «no aplica»):
   - *Hay en el dossier un número cuyo método no puedo reproducir delante de alguien.* ☐
   - *Hay una afirmación que no podría defender si alguien la comprobara la semana que viene.* ☐
   - *El apartado «qué NO hace» está vacío o dice generalidades.* ☐
   - *La respuesta a «quién lo mantiene» no es una persona con nombre.* ☐
   - *No hay ninguna forma de apagarlo, o la hay pero no la he probado.* ☐
   - *Presento como resultado del sistema algo que en realidad hago yo a mano después.* ☐
5. **CEBO 3, y con función temporal declarada.** Aquí ella **escribe su propia rúbrica** —≥3 criterios
   negativos, sin usar la del curso— y el curso le pasa un cebo con defectos plantados. **Si el cebo pasa
   su rúbrica, la rúbrica es blanda y se rehace.** Y su segunda función, escrita: **detectar si su
   lectura se ha degradado a los cuatro meses**, comparando el resultado con el del cebo 1 de M1.
6. **PC-6**: la prueba del pasillo con alguien que sabe de IA y **no conoce la academia** es el evaluador
   ideal para las dos cosas que ella no puede ver desde dentro: **jerga** y **sobreafirmación**.

**Y lo que este módulo NO puede corregir, escrito para que no se disimule:** si su compañera no usa el
artefacto, hay al menos cuatro explicaciones —el artefacto es malo, la compañera está desbordada, la
tarea no era suya, no hubo tiempo— y el material no le da forma de distinguirlas con certeza. Lo único
que puede hacer es **registrar cuál cree que es y por qué**, contra una lista de cinco causas con su
arreglo mínimo, y volver a intentarlo con otra persona o en otro momento del año. **Es el único punto del
curso donde una alumna diligente puede hacerlo todo bien y salir sin saber si lo hizo bien**, y hay una
sexta lectura legítima que va escrita antes de que ocurra: **que el artefacto no debía adoptarse**. Un
sistema que solo tiene sentido con ella delante puede ser perfectamente correcto como herramienta
personal. Reconocerlo es un resultado, no una derrota.

## 11.8 Qué produce, en una lista

1. **Un dossier de una cara**: qué hace · qué ahorra y con qué método se midió · **qué no hace** · quién
   lo mantiene · cómo se apaga.
2. **Un guion de demo de tres minutos**, cronometrado, con un antes y un después reales.
3. **La semana sin ella, ejecutada**, y su lista de arreglos con ≥2 entradas.
4. **La segunda vuelta del Mapa corto**, con su delta y sus motivos.
5. **Una descripción del proceso de otra persona**, escrita por ella y corregida por su dueña.
6. **La lista de lo que decidió no automatizar**, con el motivo tipificado.
7. **Su propia rúbrica**, validada contra el cebo 3.
8. **Una nota de media página** para quien lleve la política de uso de IA, si en M0 resultó que no existe
   ninguna. No es venta: es cerrar el hueco que ella misma detectó en la semana 1, y es el hallazgo con
   mejor relación valor/esfuerzo de todo el curso.

---

# 12. SISTEMA COMPLETO DE AUTOCORRECCIÓN SIN MENTOR

## 12.1 El enunciado exacto del problema

No es «no tiene quien la corrija». Es más incómodo:

> **Para saber si su trabajo está bien necesita el criterio que el trabajo debía enseñarle. En el
> momento en que puede evaluarse con fiabilidad, ya no necesita el módulo.**

De ahí salen tres estrategias legítimas y no hay una cuarta: **(A)** traer el criterio de fuera y
ponerlo por escrito **antes** —rúbricas, listas, soluciones comentadas, criterios de éxito—; **(B)**
sustituir el juicio por una comprobación —casos con respuesta conocida, ejecución real—; **(C)**
externalizar el juicio a un tercero —la IA, con la advertencia de que es un tercero poco fiable de
forma sistemática y predecible; o la pareja, que es una reserva estratégica y no un mecanismo.

**La primera decisión de diseño de cada módulo no es «qué rúbrica pongo», es «¿puedo convertir esta
evaluación en una comprobación?».** Muchísimas veces se puede, y casi nunca se intenta.

## 12.2 El sistema, módulo a módulo, ordenado por fiabilidad

| Módulo | Mecanismo dominante (más fiable) | Los que lo respaldan |
|---|---|---|
| **M0** | **Cronómetro y pantalla.** El correo del día 1 salió en menos tiempo o no; las comprobaciones empíricas las contesta la pantalla | Los tres criterios de rechazo de la sombra · las dos decisiones no previstas · las tres filas al azar · rúbrica de ocho casillas con el estándar «creo que» = suspenso · batería sellada del asistente v1 |
| **M1** | **La muestra apartada.** Los diez apartados se abren al final y **tiene que fallar al menos uno** | Ctrl+F sobre palabras prohibidas · prueba de tamaño · rúbrica de la línea de corte con tres criterios negativos · **CEBO 1** con consecuencia descalificatoria · protocolo de siete reglas |
| **M2** | **La batería con clave sellada, columna 3**, con umbral asimétrico: *una respuesta correcta a un caso de rechazo es un suspenso* | Lista binaria de diez ítems · abrir tres documentos citados y buscar la frase · prueba de la compañera con su criterio del otro lado · **PUERTA M2→M3** |
| **M3** | **Ejecución real.** Se dispara o no se dispara | El sexto caso que NO debe disparar · prueba de apagado · prueba del tope · lista de plataforma de seis ítems · **tabla de confusión con umbral por los dos lados** (tarde de P27) · clave de codificación del curso · **PUERTA M3→M4** con fallo provocado |
| **M4** | **Cinco casos de parada fabricados que deben parar, y un sexto que no** | Rúbrica con siete señales de fallo y salida escrita obligatoria · verdadero/falso de doce ítems · **CEBO 2** · **PUERTA M4→M5** |
| **M5** | **La prueba ciega barajada por un tercero** | Resta obligatoria · prohibiciones de vocabulario · amenaza a la validez nombrada · lista binaria de la ficha de traspaso · lectura de la Tira |
| **M6** | **El piloto: cinco días laborables sin ella, o no** | Reproducción del número ±10 % · prueba del pasillo con cuatro binarias · rúbrica del dossier con seis criterios negativos · **CEBO 3** con función temporal |

**Los tres cebos y su cadencia.** M1 (línea de corte de mentira, tres defectos: uno visible, uno de
omisión, uno de criterio) · M4 (lista de frenos de mentira) · M6 (su propia rúbrica contra un cebo). El
tercero cierra el ciclo y tiene una función que los otros dos no: **detectar si su lectura se ha
degradado a los cuatro meses.**

## 12.3 Las tres puertas *(injerto I5, reducido de cinco a tres)*

Una puerta es lo que distingue un mecanismo que te avisa de uno que te para. En un curso sin profesor,
esa diferencia es la que separa una rúbrica de un profesor.

| Puerta | Condición, toda observable | Por qué exactamente ahí |
|---|---|---|
| **M2 → M3** | Batería 5/5 típicos, aclaración en límite, «no lo sé» en rechazo · **uso espontáneo ≥5 veces en una semana sin que el curso lo pida** · prueba de traslado hecha | Automatizar algo que no funciona es multiplicar el error. Y la tesis de este diseño es falsa si ella no lo usa |
| **M3 → M4** | El disparador ha corrido **una semana entera sobre casos reales** y **ha fallado algo y sabe por qué**. Si no ha fallado nada, el material trae un **fallo provocado** | Sin haber visto un fallo no hay criterio para dar autonomía a nada |
| **M4 → M5** | Los cinco casos de parada pararon y el sexto no · cada parada dejó marca y dijo por qué · el revisor es un nombre y una hora · el apagado está probado · **ningún camino llega a un cliente sin que alguien le dé a enviar** | Es la última puerta antes de medir, y medir un sistema sin frenos mide otra cosa |

**Y la regla que hace que una puerta no sea un suspenso**, y que ninguna arquitectura escribe:

> *Una puerta que no se abre no es un fracaso: es una semana más en la misma capa. Esa semana está
> presupuestada —por eso M4 dura tres semanas y no dos— y las tres puertas llevan escritas sus causas
> típicas con su arreglo mínimo.*

## 12.4 La IA correctora: puesto 6 de 9, con protocolo y con descalificación por entregable

La IA está en el puesto 6 de nueve mecanismos, no en el 1. Es valiosa por cobertura y por inmediatez,
no por fiabilidad, y **falla en la misma dirección en la que ella ya está sesgada**: el sesgo de
sobreestimación y la adulación del modelo **se suman, no se cancelan**.

**El protocolo, siete reglas**, en `comun/protocolo-ia.md`, citado desde cada rúbrica:

1. **Hilo nuevo, siempre.** Nunca se corrige en la conversación donde se construyó.
2. **No es tuyo.** *«Reviso el trabajo de una compañera que hace mi mismo puesto. Tengo que decidir si
   se lo devuelvo.»* Es la mitigación más barata que existe y tiene medida.
3. **Nunca preguntes si está bien.** *«Enumera los incumplimientos de esta rúbrica. Por cada criterio,
   cita textualmente el fragmento que lo incumple. Si no puedes citar un fragmento, no lo afirmes.»*
4. **Pega la rúbrica entera, con sus criterios negativos.** Sin rúbrica, el modelo se inventa el
   estándar, y el estándar que se inventa es benévolo.
5. **Prohibido discutir en el mismo hilo.** Si no está de acuerdo, **no responde**: anota, corrige o no
   corrige, y abre un hilo nuevo con la versión modificada y la misma rúbrica. **La conversación es el
   vector del fallo.**
6. **Dos modelos, y el desacuerdo es la señal, no el veredicto.** Donde coinciden, el fallo es casi
   seguro; donde discrepan, ahí hay algo que ella no entiende todavía — y eso, no el veredicto, es lo
   que anota.
7. **Su veredicto no cierra nada.** La IA devuelve una lista de fallos candidatos. Quien decide es ella.

**Y la descalificación por entregable, que es la pieza más fina del corpus y aquí se generaliza a una
tabla** *(de arq-3, rúbrica de E4.2)*. Aplicar el mismo protocolo en todas partes es un error: hay
entregables donde el corrector no puede funcionar por construcción.

| Entregable | ¿IA correctora? | Por qué |
|---|---|---|
| Ficha de criterio (M1) | **Sí, con protocolo** | Es texto contra una rúbrica: es su mejor caso |
| Línea de corte (M1) | **Sí, con protocolo**, y con el cebo 1 delante para saber cuánto se le escapa | Le falta el conocimiento de la academia, así que caza forma y no hechos |
| Batería de diez casos (M1) | **No para juzgar la calidad de la batería** | Preguntarle si tu instrumento es bueno a un modelo que no conoce el dominio es pedir una opinión sin referente. Lo que la juzga es que **falle al menos uno de los diez apartados** |
| Mapa de datos (M2) | **Solo para la forma.** Los hechos los comprueba ella | Ningún modelo sabe qué documentos hay en su academia |
| Lista de frenos (M4) | **Inhabilitada para el umbral de listo** | Le estás pidiendo a un modelo complaciente que juzgue si otro modelo es demasiado complaciente. **La IA solo para buscar señales de fallo; el umbral se comprueba mirando pararse el sistema** |
| Evaluación y número (M5) | **No** | Es aritmética con su cronómetro, y la evaluación no se hace con la herramienta evaluada |
| Dossier (M6) | **Sí para jerga, no para veracidad** | No puede comprobar si el número es reproducible; sí puede contar cuántos nombres de herramienta aparecen |

## 12.5 Los seis puntos de consulta, con alternativa degradada

**El recurso es escaso, no renovable y con coste relacional.** Un mentor pagado se gasta sin culpa; una
pareja, no. **Presupuesto: seis consultas de diez minutos en todo el curso** — una hora repartida en
cuatro meses. Un curso que reserve «consultas ilimitadas» obtiene en la práctica **cero**, porque cada
consulta compite con la comodidad de no molestar y pierde. Uno que reserve exactamente seis, con nombre
y momento, obtiene seis.

**Filtro de admisión**, impreso en la portada del cuaderno. Si falla cualquiera de las cuatro, no es
punto de consulta: *(1) ¿lo resuelve el material? (2) ¿lo resuelve la IA con el protocolo? (3) ¿lo
resuelve **mirar** —su pantalla, su consola, preguntar a su administrador—? (4) ¿lo he intentado
veinticinco minutos y he anotado lo que he probado?*

**Ficha de cinco campos, escrita ANTES, máximo una cara:** la pregunta en una frase **cerrada** · mi
hipótesis y qué esperaría ver si tengo razón · qué he probado y qué pasó · **el dato concreto** (mensaje
de error literal, las dos respuestas que se contradicen) · qué haré con cada respuesta posible.

**Cuatro reglas de la conversación:** los cinco primeros minutos **sin pantalla** · **él no toca el
ratón** · sale con una frase escrita en su propio lenguaje dentro de la hora siguiente · **a los diez
minutos se para, esté como esté.**

**Y el principio de formulación, generalizado a los seis** *(de arq-3 PC-1)*: **cada pregunta se acota a
lo que el consultor PUEDE auditar** —el razonamiento y los hechos de plataforma, no los hechos de la
academia, que no conoce—. Es lo que impide gastar diez minutos irrecuperables en una pregunta que la
otra persona no está en posición de contestar.

| # | Momento | Qué lleva | Por qué ahí | **Alternativa degradada** |
|---|---|---|---|---|
| **PC-1** | Fin de M0 (sem. 2) | *«He deducido que tenemos el plan X, que por eso no puedo hacer Y, y que por eso he descartado estos tres procesos y elegido éste. ¿El razonamiento se sostiene?»* Con las comprobaciones empíricas hechas y la hoja de sombra delante | **Es el punto de mayor consecuencia del ángulo**, porque todo se construye encima. Y está acotado a lo que él puede auditar: razonamiento y hechos de plataforma | Asumir el escenario **más restrictivo**, elegir el proceso con puntuación más alta que no dependa de ninguna función dudosa, y anotar la suposición como pendiente |
| **PC-2** | Inicio de M2 (sem. 5), antes de cargar fuentes reales | Ocho tipos de dato de su puesto clasificados en tres cajones (empresa / nunca / depende) + tres casos ya seudonimizados: *«¿tú sabrías de quién hablo?»* | **La única decisión del curso con consecuencia externa irreversible**, y el momento es exacto: es cuando pasa de pegar texto a subir ficheros | Regla de máxima cautela: **si dudas, no entra**, y se anota. Y la prueba de la compañera se hace con **cualquier compañera de la academia**, que además es la evaluadora literal del criterio |
| **PC-3** | Fin de M1 (sem. 4), tras el cebo 1 | *«Ésta es la corrección que hizo la IA de un trabajo con tres fallos plantados. Encontró dos. ¿Estoy leyendo bien lo que se le escapa?»* | **El de mayor apalancamiento.** No se revisa su trabajo: **se revisa su instrumento de corrección**, que va a usar cincuenta veces más | Pasar el cebo por **dos modelos distintos** y comparar: el desacuerdo entre modelos es un sustituto pobre pero real del juicio externo |
| **PC-4** | **Comodín**, desde M3 | Un fallo de plataforma, tras agotar la lista de seis comprobaciones y `cuando-no-coincide.md` | «Diez minutos ahorran una tarde». **No tiene fecha a propósito:** saber que existe un comodín reduce el miedo a atascarse, que es un factor de abandono por sí mismo aunque no se use | Documentar el fallo, **rodearlo** con una solución manual y seguir. Un curso no puede pararse por un botón que alguien movió |
| **PC-5** | Fin de M4 (sem. 11) | *«Ésta es la línea de corte con la que he terminado, y éstos son los tres sitios donde dudé. ¿Dónde la moverías?»* | Juicio de escala y oportunidad: preguntarle a un modelo si algo debe automatizarse tiene un sesgo obvio hacia el sí. Y **cae exactamente en la frontera de abandono** (§13, momento 3): una conversación sobre su propio criterio es el mejor combustible donde el material solo ya no tira | La lista de descalificadores por número de proceso y los tres criterios negativos de la línea de corte |
| **PC-6** | M6 (sem. 16) | La prueba del pasillo en treinta segundos, y después: *«¿qué he dicho que no podría defender si alguien lo comprobara?»* | Alguien que sabe de IA y **no conoce la academia** es el evaluador ideal para las dos cosas que ella no puede ver desde dentro: **jerga** y **sobreafirmación**. Y cierra el curso con otra persona, que evita el final en el vacío | Hacer la prueba del pasillo con una compañera de otro departamento. Detecta jerga peor y sobreafirmación igual de bien. Y grabarse treinta segundos y contar los nombres de herramienta al día siguiente |

**Un uso de otra persona que NO gasta punto:** barajar las respuestas de la prueba ciega de M5 y guardar
la clave. Función mecánica de cinco minutos, vale cualquier compañera.

**Lo que deliberadamente NO es punto de consulta:** revisar un entregable (*«¿está bien mi asistente?»* →
rúbrica y batería) · explicar un concepto (→ material) · enseñarle a hacer algo (→ documentación) · dar
ánimos. Y la tentación específica de esta configuración: **que él le monte algo «que es un momento»**.
Eso no es una consulta: es un artefacto que ella no sabrá mantener ni depurar, y en la capa siguiente
será deuda. En un curso cuyo entregable es **un sistema que tiene que sobrevivirle a ella**, un trozo que
no entiende es literalmente el peor regalo posible.

**Nota de riesgo [NV]** *(injerto I16, de arq-2 §7.3)*, y hay que escribirla porque es un modo de fallo
silencioso: **todo esto asume que la pareja sabe de plataformas y no solo de modelos.** Si su
conocimiento es de modelos, **PC-4 pierde casi todo su valor** y ese punto se reasigna a PC-3 o a PC-6.
La comprobación es de un minuto y se hace en la semana 1: enseñarle la lista de seis comprobaciones de
plataforma y ver si le suenan. Los otros cinco puntos tienen alternativa degradada por
**indisponibilidad**; éste la necesita también por **incompetencia en el tema concreto**, que es más
probable y más silencioso, porque la consulta ocurre igual y devuelve una respuesta que parece buena.

## 12.6 El registro transversal

Un fichero, `bitacora.md`, una línea por sesión: fecha · minutos · qué he hecho · qué he producido ·
**qué ha fallado** · nota de autoevaluación. Sirve para tres cosas a la vez: es la base de la práctica
espaciada (de ahí salen las cinco preguntas de repaso que abren cada sesión) · es **la evidencia contra
la ilusión de fluidez** (a las diez semanas puede leer lo que le parecía imposible en la semana 2) · y
es lo que hace que un punto de consulta de diez minutos rinda, porque llega con el historial escrito.

---

# 13. PLAN ANTI-ABANDONO

**Dos hechos ordenan esta sección:** el 52 % de los inscritos en un curso autodidacta **nunca llega a
empezar** [E], y el abandono posterior **es episódico y localizable**, no un desgaste uniforme. Si los
momentos son localizables, se les puede poner algo delante.

**Principio transversal:** **toda contramedida se escribe antes del punto de caída, no en él.** El modo
mínimo redactado la semana en que ya falló se lee como excusa; redactado en la semana 1, como plan.

**Uno que NO está en la lista y podría esperarse:** el primer resultado mediocre —cuando el asistente
contesta mal la primera vez—. Es probable, pero su contramedida es barata, conocida y ya está
incorporada en cada módulo: la caja **«lo que vas a ver la primera vez»**, escrita antes del ejercicio,
que describe el resultado mediocre concreto que va a obtener. **Un fallo anunciado es una etapa; un
fallo inesperado es un veredicto sobre uno mismo.** Y la cita de la referencia, que es su mejor minuto:
*«Ves el resultado. Detrás hay varias decenas de intentos.»*

## MOMENTO 1 · Días 1–10 — el arranque, y la sospecha de haber elegido mal

**Qué pasa por dentro.** Tres cosas a la vez, y la tercera es específica de esta columna vertebral: la
fricción de arranque · el beneficio todavía es abstracto mientras el coste ya es real · y **se le pide
comprometerse con un proceso en la semana 1, que es cuando menos criterio tiene**. La conclusión
peligrosa no es «esto es difícil», es **«creo que he elegido mal y llevo dos semanas»**, y ésa es
irreversible si no se anticipa.

**Qué se pone justo antes — ocho piezas, todas estructurales:**

1. **La sesión 1 no explica el curso: produce un resultado utilizable en veinticinco minutos**, con lo
   que ya tiene abierto, sin instalar nada y sin hablar con nadie. **El mapa del curso va después del
   primer resultado, nunca antes.**
2. **El premio grande llega el día 4, no el día 1** *(injerto I1)*: el asistente que cita, con tres
   fuentes verdes. Grande, pero con red debajo, porque el día 1 ya ganó una vez.
3. **La elección no es una apuesta: es una prueba con tres criterios de rechazo observables.** Se le
   quita el peso de «acertar» y se le da un procedimiento.
4. **El proceso de repuesto está nombrado y firmado el día 3**, no el día de la crisis.
5. **El divorcio preautorizado, con su aritmética escrita**: al final de M1 cambiar de proceso cuesta
   unas dos horas. **Escrito en la semana 1** se lee como plan; escrito cuando ya ha dudado, como
   excusa.
6. **El hallazgo prometido a las 48 horas** *(injerto I10)*: el material predice por escrito lo que la
   observación va a revelar y lo nombra **primer hallazgo del curso**. Convierte dos días de peaje en
   pago, dentro del tramo de máxima mortalidad.
7. **El diagnóstico del entorno no puede bloquear.** Las comprobaciones empíricas están en la misma
   página que los mensajes, y la rúbrica declara que *«pregunté a X el día D y no obtuve respuesta»* es
   un resultado válido.
8. **PC-1 al final de la semana 2**: otra persona implicada en el punto de máxima mortalidad, revisando
   exactamente la decisión que le da miedo.

**Y el contrato de una página, antes de empezar:** 17 semanas · 2 h semanales de tiempo propio · **0 €**
· nada que instalar · nada que pedirle a nadie · **la frontera de M4** · **la movilidad de M6** · el
modo mínimo · y la definición observable de «terminado». *Un curso que se anuncia de ocho semanas y
dura diecisiete se percibe como fracaso propio en la novena.*

## MOMENTO 2 · Semanas 7–9 — el primer bloqueo que no es culpa suya

**Qué pasa por dentro.** La automatización nativa de su entorno **falla con unidades compartidas,
carpetas compartidas y hojas con referencias externas** [V], y el centro de gravedad de su puesto **es
un buzón compartido y una hoja de camas compartida**. La primera vez que intente automatizar su trabajo
de verdad, la herramienta puede decirle que no. Y la conclusión que se saca no es «me he equivocado de
carpeta»: es **«esta herramienta no sirve para mi trabajo»**, y detrás, *«este curso no sirve para mi
trabajo»*. Es la única conclusión de todas las simuladas que es irreversible.

**Qué se pone justo antes:**

1. **La contramedida principal está seis semanas antes: la cuarta columna del embudo.** Los procesos que
   solo viven en recursos compartidos se descartaron en la semana 1, cuando descartar costaba diez
   minutos. **Es preventiva en vez de paliativa**, y es la aportación de diseño más rentable del curso.
2. **La regla del embudo vacío** (§5.4), con sus tres salidas escritas, incluida la petición de
   delegación de una etiqueta o carpeta propia. Nadie se queda sin proceso.
3. **La restricción de producción de independencia de plataforma** *(injerto I8)*: la ruta principal de
   M3 es un disparo por reloj **dentro del chat que ya usa**, sin consola ni permisos. Si el
   administrador tiene desactivada la automatización nativa, **se pierde comodidad y cero hilo**.
4. **El límite va en la primera página del módulo, con nombre y por escrito**, no en una fe de erratas.
5. **La lista de seis comprobaciones de plataforma**, entregada **antes** del primer disparador y
   reutilizable como diagnóstico. Convierte un bloqueo en una comprobación con resultado, que es lo
   contrario de un veredicto sobre una misma.
6. **La página `cuando-no-coincide.md`**, que convierte la caducidad del material en competencia
   enseñada: *si algo no coincide con lo que ves, tu pantalla tiene razón y este texto no.*
7. **PC-4, el comodín, cuya existencia se anuncia mucho antes de que haga falta.**
8. **La caja «si nada de esto funciona»: documenta el fallo, rodéalo con una solución manual y sigue.**

## MOMENTO 3 · Semanas 11–14 — la meseta del «ya me sirve»

**Qué pasa por dentro.** Al terminar M4 **el sistema funciona y ella lo usa**. El dolor que la trajo al
curso está resuelto. Y justo entonces vienen dos módulos que no añaden funcionalidad: medir/traspasar y
contagiar. Novedad baja, beneficio inmediato bajo, esfuerzo mental alto. **El abandono aquí no se siente
como abandono: se siente como haber terminado.** Y ésa es exactamente la razón por la que es peligroso,
porque los objetivos 4 y 5 del perfil viven enteros en ese tramo.

**Qué se pone justo antes — y esto es donde más he modificado la columna vertebral:**

1. **La meseta se ha acortado de siete semanas a seis, y de tres módulos a dos** (§0.2, punto 5). Menos
   fronteras de módulo = menos sitios donde el curso puede leerse como terminado.
2. **La frontera se declara en la semana 1, y con estas palabras:** *«al acabar M4 ya tienes lo que
   viniste a buscar. Lo que viene después es lo que hace que esto te siga sirviendo dentro de dos años
   y en otra empresa, y es la parte que nadie hace.»* Nombrar la meseta antes de llegar a ella es lo que
   la convierte en un tramo y no en un final.
3. **El gancho de M5 no es metodológico, es de deseo: el número.** Ella quiere evidenciar valor —es su
   objetivo 5, formulado por ella— y **el número es la munición**. M5 no se presenta como «vamos a
   evaluar»: se presenta como *«vas a poder decir cuánto ahorras y defenderlo si alguien lo
   comprueba»*.
4. **La lectura de la Tira completa como primera sesión de M5.** Seis columnas de su propio trabajo, con
   fecha. A las doce semanas puede leer lo que en la semana 3 le parecía imposible. Es la evidencia
   objetiva contra la ilusión de fluidez, y es gratis.
5. **La cláusula del resultado decepcionante, escrita antes de medir**, con las razones legítimas
   alternativas enumeradas de antemano y la instrucción de **medir esa otra razón** si es la que
   importa. **La honestidad de la medición está protegida por adelantado, que es la única forma de que
   la medición sea honesta.**
6. **PC-5 exactamente en la frontera** (fin de M4). Una conversación de diez minutos sobre su propio
   criterio es el mejor combustible disponible donde el material solo ya no tira. Y el objeto —*«¿dónde
   moverías la línea de corte?»*— es intrínsecamente halagador de su trabajo sin ser halago: se conversa
   sobre criterio, que es lo que ya tiene.
7. **El compromiso externo de M6 se anuncia en M4, no en M6.** *«En la semana 16 una compañera va a usar
   esto una semana entera sin ti.»* Anunciarlo con cinco semanas de antelación convierte M5 en
   preparación de algo **con fecha y con otra persona dentro**, que es el mecanismo de permanencia más
   fuerte disponible en un curso sin cohorte.
8. **El hallazgo vistoso se coloca aquí, no antes:** el doblete de P32 produce lo que ningún otro
   artefacto produce — **una lista de errores reales que nadie en la academia sabía que existían**:
   precios del año pasado circulando en la plantilla alemana desde hace meses. Es el momento del curso
   en que su trabajo produce **un hallazgo y no un ahorro**, y por eso está donde el material solo ya no
   tira.

## El modo mínimo y el ritual de reentrada, redactados en la semana 1

> **Modo mínimo.** Semana de pico o imprevisto: **una micro-sesión de diez minutos y nada más, y eso
> cuenta como semana cumplida.** Estar en modo mínimo no es fallar. El curso lo dice explícitamente y lo
> dice antes de que ocurra.
>
> **Ritual de reentrada.** Toda vuelta tras una pausa empieza igual: leer las tres últimas entradas de
> la bitácora y responder las cinco preguntas de repaso. Diez minutos, y elimina el coste de arranque
> — que es lo que convierte una pausa de una semana en el final.
>
> **Intenciones de implementación, no propósitos.** «Si es martes y son las 9:15, abro el módulo»:
> fecha, hora y sitio escritos, no «esta semana».

---

# 14. DURACIÓN Y DEDICACIÓN REALISTAS

## 14.1 El calendario

| | |
|---|---|
| **Duración total** | **17 semanas**, siete módulos |
| **Arranque** | **Octubre.** El pico de junio–septiembre (250–400 correos/día, 60–90 matrículas/semana) mata cualquier calendario que lo ignore. Noviembre–febrero es temporada baja, y ahí caen las semanas 6–17 |
| **Fin previsto** | Segunda semana de febrero, con margen antes de que empiece a subir el volumen |
| **Tiempo propio** | **2 h por semana.** Total: ~34 horas |
| **Tiempo de trabajo** | El bloque de proyecto (60–90 min/módulo), los palotes, el cronometraje, la sombra y la tarde de P27. **Es trabajo del puesto hecho de otra manera** |
| **Coste** | **0 €.** Nada que instalar, nada que dar de alta, ninguna licencia que pedir. Si el curso acaba costando dinero, el diagnóstico estaba mal |
| **Herramientas nuevas** | Dos o tres en 17 semanas, y ninguna antes de que el proceso se haya quedado corto sin ella |

## 14.2 La declaración de tipo de tiempo, línea a línea

**Cada sesión del material declara arriba si es `[ tiempo propio ]` o `[ tiempo de trabajo ]`.** No es
cosmética: la primera causa documentada de abandono es el tiempo —*«Time is the bottleneck»*, 21 de 34
abandonos [E]— y **sin esa declaración escrita ella lo contabilizará todo como tiempo propio y el curso
parecerá el doble de caro de lo que es.**

Desglose honesto de un módulo tipo de dos semanas:

| Pieza | Duración | Tipo |
|---|---|---|
| 3 sesiones núcleo | 35–45 min cada una | tiempo propio |
| 1 bloque de proyecto | 60–90 min | **tiempo de trabajo** |
| Cierre de capa (cinco preguntas + pregunta fija + columna de la Tira) | ~35 min | tiempo propio |
| Doblete | 20 min | tiempo propio |
| Cuaderno de evidencias | 2 min | — |

Suma de tiempo propio: **~3 h 45 por módulo de dos semanas ≈ 1 h 50 por semana.** Cabe en el
presupuesto declarado, con el margen justo. **M4 y M6 duran tres semanas precisamente porque su
contenido no cabe en dos**, y decirlo es más honesto que comprimirlos y que ella lo descubra.

## 14.3 Las horas, sumadas

| Concepto | Horas propias |
|---|---|
| M0 (2 sem.) | ~3,5 |
| M1 (2 sem.) | ~4 |
| M2 (2 sem.) | ~4 |
| M3 (2 sem.) | ~4 |
| M4 (3 sem.) | ~5,5 |
| M5 (3 sem.) | ~5,5 |
| M6 (3 sem.) | ~5 |
| Los seis puntos de consulta | 1 |
| **Total** | **≈ 32,5 h de tiempo propio en cuatro meses** |

---

# 15. PRUEBA DE DURABILIDAD A DOS AÑOS, MÓDULO POR MÓDULO

**Procedimiento.** Recorrer el mapa suponiendo que en agosto de 2028: (a) los productos se han
renombrado al menos una vez —ya ocurrió tres veces en cinco meses de 2026 con la automatización nativa
de la suite, el cuaderno de fuentes y la herramienta de terminal—; (b) algunas funciones se han movido
de edición o han desaparecido; (c) su empresa ha cambiado de proveedor, o ella ha cambiado de empresa.

| Módulo | Qué es criterio (sigue válido en 2028) | Qué es clic (se rompe) | Coste de reparación |
|---|---|---|---|
| **M0** | El embudo y sus cinco columnas · **la pregunta durable de la cuarta columna** · la prueba de la sombra y sus tres rechazos · describir por observación y no por introspección · las cuatro preguntas que definen cualquier plan · «la misma frase es segura o no según con qué cuenta entres» · «pagar resuelve quién es el proveedor, no qué tratamientos están amparados» · el semáforo · el estándar «no lo sé y lo pregunté» vale / «creo que sí» no · la lista de 32 procesos · el Mapa corto y su rejilla | El distintivo concreto de la pantalla · las comprobaciones empíricas · la ruta de la consola · los mensajes literales · **el −3 concreto de la cuarta columna** | **1 fichero de clics + 1 línea de `datos-volatiles.md`.** El criterio no se toca |
| **M1** | La línea de corte y sus cinco motivos tipificados · el escalón −1 · la ficha de criterio y su prohibición de palabras · las anclas conductuales · la muestra apartada · la tabla de especificaciones · el requisito del caso en idioma minoritario · el cebo como control positivo · el protocolo de siete reglas | **Nada.** Este módulo no tiene fichero de clics | **Cero** |
| **M2** | Fuente de verdad con **fecha y dueño** · citar como forma de abaratar la revisión · «no lo sé» exigible y probable · seudonimización y cuasi-identificadores · la prueba de la compañera **con su criterio del otro lado** · la regla de los adjuntos · el mapa de datos del proceso · el techo de la memoria · **las tres señas de la capacidad** | Dónde se guarda un asistente, cuántos ficheros admite, cómo se llama la superficie de fuentes | **1 fichero de clics + 1 línea de `tres-nombres.md`** |
| **M3** | Disparador por calendario frente a por suceso · el tope · el apagado probado · «prepara, no envíes» y su motivo · «automatiza donde ya viven tus datos» · **la prueba del caso que NO debe disparar** · **las tres señas de una automatización, incluida la de ver el historial** · el libro de códigos · doble codificación · tabla de confusión · umbrales por los dos lados · la notación neutra | Los límites concretos de la plataforma · el catálogo de pasos disponibles · cómo se escribe una clasificación en lote | **1 fichero de clics + la lista de seis comprobaciones**, que hay que reescribir con los límites de la plataforma nueva. **Es la reparación más cara del curso** |
| **M4** | Temas prohibidos frente a condiciones de parada · las seis condiciones y su motivo · «parar no es callarse» · el revisor con nombre y hora · el plan de fallo en cinco pasos · «la confianza no es una salvaguarda» y el riesgo del día 60 · empatía sin admisión · privilegio mínimo · **las cinco preguntas aplicadas a un agente que no existe hoy** | Cómo se implementa una bifurcación y un tope · qué producto está detrás de qué plan · las fechas del marco normativo | **1 fichero de clics + la caja del fondo**, que se revisa entera: **está diseñada para eso, porque su primera columna son condiciones y no productos**. Y `datos-volatiles.md` para las fechas normativas, que caducan más rápido que los productos |
| **M5** | Línea base · minutos por unidad · coste completo · las seis amenazas a la validez interna · proceso frente a resultado · cadena causal · prueba ciega · lectura de la Tira · fuentes con caducidad y dueño · calendario de revisión · apagado probado · la prueba del hueco · la reproducción del número | **Nada.** Es metodología, un cronómetro y una hoja de cálculo | **Cero** |
| **M6** | El número y su método · «qué NO hace» · la demo de tres minutos · la prueba del pasillo y sus cuatro binarias · **la semana sin ella** · la ficha de traspaso · las cuatro reglas de arranque · la entrevista de proceso ajeno · la deuda de adopción · escribir la propia rúbrica y validarla contra un cebo · la segunda vuelta del Mapa corto | **Nada** | **Cero** |

## 15.1 Recuento

| | Módulos | Proporción |
|---|---|---|
| **Sin nada que reparar** (M1, M5, M6) | 3 | 43 % |
| **Reparación de un fichero de clics** (M0, M2) | 2 | 29 % |
| **Reparación media** (M4: clics + revisión de la caja del fondo + fechas normativas) | 1 | 14 % |
| **Reparación cara** (M3: clics + la lista de comprobación de plataforma) | 1 | 14 % |
| **Módulos que habría que rediseñar** | **0** | **0 %** |

**Y por instrumento:** las **cinco preguntas** no caducan (clasifican por autonomía cedida, que es una
propiedad y no un catálogo) · el **Expediente del proceso** no caduca (una academia de idiomas en 2030
seguirá emitiendo cartas de visado y contestando leads) · la **Tira** no caduca · el **Cuaderno de
capas** caduca en siete líneas —la línea de techo de cada cierre— por diseño · el **Mapa corto** no
caduca, y su rejilla de seis veredictos es el instrumento con más riesgo del conjunto (§15.3) · la
**Lista de techos** no caduca porque su tercera columna son condiciones · la **tabla de tres nombres**
caduca **entera**, y por eso está aislada en una sola página fechada.

**Veredicto: no hay que rediseñar.**

## 15.2 Los dos escenarios que no son de producto, y por qué el diseño sale reforzado

**(a) ¿Y si un solo producto acaba haciendo todas las capas?** Es plausible: la tendencia es que la
misma ventana de chat programe, dispare por sucesos y actúe. Si ocurre, **el diseño no se rompe: se
vuelve más necesario**, porque el producto deja de forzar la distinción y **ya nada, salvo el criterio,
le dice cuánta autonomía acaba de ceder**. Las cinco preguntas se responden igual dentro de una sola
ventana, y la Tira sigue mostrando en qué columna se ganó la calidad y en cuál solo cambió el
disparador.

**(b) ¿Y si los modelos dejan de necesitar fuentes citadas?** No hace falta apostar. M2 no enseña «cita
porque alucina»: enseña **cita porque tu revisión tiene que durar cinco segundos y porque una fuente
caducada responde con toda la confianza del mundo**. Ese segundo motivo no depende de la calidad del
modelo: depende de que los tarifarios cambien, y van a seguir cambiando.

## 15.3 Lo que sigue siendo frágil aunque el diseño esté bien

Una prueba de durabilidad que sale limpia del todo es sospechosa. Cuatro cosas:

- **M3 es el punto débil y no tiene arreglo estructural.** La anatomía de un disparador es durable, pero
  **los límites concretos de una plataforma no son un adorno del módulo: son la mitad del módulo**,
  porque son lo que determina si su buzón compartido se puede tocar o no. Si cambia la plataforma, hay
  que volver a averiguar los límites, y eso no se hereda.
- **La rejilla de seis veredictos es mitad clasificador y mitad foto del espacio de soluciones de 2026.**
  El juez 3 tiene razón y hay que escribirlo: las **pruebas** que deciden cada veredicto duran —¿cabe en
  una servilleta? ¿puedes nombrar el documento y su fecha? ¿los pasos son siempre los mismos?— pero los
  destinos 4, 5 y 6 son fronteras de producto. El día que una sola superficie haga las tres, esas tres
  casillas pierden su referente y quedan enteros el 1, el 2 y la zona prohibida. **Mitigación escrita en
  el material:** la rejilla se usa siempre acompañada de las cinco preguntas, que no tienen ese problema,
  y **la segunda vuelta del Mapa corto es el sitio donde se revisa si la rejilla sigue partiendo bien el
  espacio.** Es una mitigación parcial y lo digo como tal.
- **La lista de 32 procesos envejece despacio, pero envejece.** Una normativa de extranjería nueva, un
  canal de captación que desaparece, y hay filas que dejan de existir. Sigue siendo el activo más
  duradero del curso, pero **hay que fecharla como cualquier otra fuente**.
- **Y una asimetría incómoda:** lo que menos caduca de este curso es lo que menos se parece a «un curso
  de IA» —mirar un proceso, escribir criterios, medir, traspasar, contagiar— y lo que más caduca es lo
  que más se parece. Es la mejor prueba de que el listón está bien puesto, y también el motivo por el
  que el material tiene que trabajarse el enganche de M1, M5 y M6 mucho más que el de M3.

---

# 16. QUÉ SE QUEDA FUERA, A PROPÓSITO

## 16.1 Fuera porque el brief lo excluye

| Fuera | Por qué |
|---|---|
| **«Cómo conseguir el sí», venta interna, pedir autorización** | En su empresa usar IA ya está bien visto y **lo mal visto es no automatizar**. Un módulo de permiso resuelve un problema que ella no tiene. Lo que sí entra —evidenciar y contagiar— es otra cosa y está en M6 |
| **Portfolio, landing, prototipo de app, «lo que tengo ahora en mi CV»** | Es el destino del itinerario no técnico de la referencia porque **su alumno tipo quiere entrar en el sector de la IA**. La nuestra no quiere cambiar de rol ni de sector. Lo que sí quiere —que le sirva si cambia de empresa— lo da la portabilidad del criterio, no una web |
| **Certificado, insignia, «ahora eres AI Operator»** | No busca cambiar de rol. Y un certificado sin evaluador y sin rúbrica no certifica nada. La definición de «terminado» de §3 es observable y no la firma nadie |
| **Cualquier cosa vistosa** | El grafo de la referencia es el caso de estudio: espectacular en pantalla, marginal en valor para atención al cliente, y —dicho por su propia autora— *hecho para el agente, no para el humano*. Aquí el artefacto útil es aburrido: un asistente que cita, un triaje que etiqueta, un vigilante que avisa |
| **Construir y vender aplicaciones** | Ni siquiera la referencia lo promete: *«construir algo para uso interno y publicarlo en internet son dos mundos distintos»* |
| **Coleccionar herramientas** | Dos o tres capacidades nuevas en 17 semanas, y ninguna antes de agotar la anterior |

## 16.2 Fuera por el listón de durabilidad, con su condición de reentrada

| Fuera | Reducido a | Condición para que entre |
|---|---|---|
| **Plataformas de automatización externas como módulo** | Una fila de la caja del fondo + el criterio *automatiza donde ya viven tus datos* | Que su proceso tenga que tocar algo fuera de su suite. Y una que haya que autoalojar, solo si aparece alguien técnico que la mantenga |
| **Escribir código, aunque lo escriba la IA** | Media página informativa | Que la automatización nativa se quede corta **y** haya quien mantenga el script. En el momento en que falla hay que leer un error de programador, y eso es una dependencia que ella no puede cubrir |
| **La superficie de desarrollador «gratis y de la misma empresa»** | Cinco líneas, con aviso explícito | **Ninguna.** Es la trampa más silenciosa del panorama y por eso se nombra: parece profesional, se entra con la cuenta de siempre, y sus términos dicen literalmente que no metas información personal |
| **Conectores y su estándar, como práctica** | Vocabulario + el principio de privilegio mínimo | Que monte algo fuera de su suite, o que alguien se lo configure y ella solo lo use |
| **Arquitecturas de recuperación sobre corpus grandes** | Una fila de la caja del fondo | Que las fuentes pasen de decenas a cientos y el asistente empiece a perderse |
| **Herramientas agénticas de escritorio y de terminal** | Un apéndice de lectura, opcional, sin entregable | Una tarea que exija procesar decenas de ficheros locales de forma repetida. **Si termina el curso sin abrir el apéndice, el curso ha funcionado igual**, y eso va en su primera línea |
| **Comparativas y nombres de modelo** | Nada | Ninguna. *«Da bastante igual qué modelo uses mientras no gastes miles en tokens.»* Es el detalle que menos importa y el que más rápido caduca |

## 16.3 Fuera por rigor mal invertido

- **Estadística inferencial.** Nada de significación, valor p ni tamaño muestral sobre doce casos. Aquí
  no se estima un parámetro poblacional: se comprueba la cobertura de un instrumento contra un criterio
  fijado. **Doce casos bien elegidos valen más que doscientos al azar.**
- **Consistencia interna aplicada a la batería.** Directamente incorrecto: una batería **debe ser
  heterogénea**. Si tuviera consistencia interna alta sería porque está mal construida.
- **Prompt engineering como colección de trucos.** El curso enseña **el criterio antes del prompt**. Un
  prompt bueno que se escribe una vez y se pierde no vale nada; el mismo guardado con sus fuentes es
  infraestructura.
- **Vídeos de lección.** Un vídeo es relectura con mejor producción, y la relectura está clasificada como
  técnica de utilidad **baja**. Si hay vídeo, es demostración de una interfaz, dura menos de tres
  minutos, va con transcripción **y vive en la carpeta de clics**.
- **Resúmenes de la lección al final.** El resumen lo escribe ella y es un entregable: la pregunta fija.
- **Cualquier ejercicio de metodología sin artefacto reutilizable.** El riesgo de este perfil no es
  quedarse corta de rigor: **es pasarse**. Si un ejercicio le lleva más de lo que le llevaría hacer la
  tarea a mano durante un mes, está mal calibrado y se recorta. La regla que lo gobierna: **el montaje se
  hace rápido y sucio; el rigor se gasta entero en la evaluación.**

## 16.4 Fuera por decisión propia de esta síntesis, y es la más discutible

**La segunda automatización.** El curso construye **una** cosa. No hay un segundo proceso ni un hilo
guiado paralelo; el expediente modelo se lee y se usa como clave, no se ejecuta — **con la única
excepción declarada de la tarde de P27** (§6.5), que son 90 minutos y existe precisamente para recuperar
lo que renunciar al doble hilo cuesta.

La defiendo así: con dos horas propias por semana, **dos procesos son dos procesos a medias**, que es
exactamente lo que este ángulo existe para evitar. El segundo proceso es lo primero que hará **después**
del curso, y para eso están la Lista de techos, la cola que sale de la segunda vuelta del Mapa corto, su
propia rúbrica y la ficha de traspaso.

## 16.5 Fuera por riesgo, con nombre y número

P08 visados · P17 matching · P22 calendario de camas · P25 reembolsos · P26 quejas formales · P29
emergencias · P05/P16 nivelación y exámenes. **No son «temas avanzados»: son zona prohibida con motivo
escrito**, y **el motivo es el contenido**, porque es lo único que se transfiere a un caso nuevo (§9.2).

---

# 17. AUTOCRÍTICA

Sin esta sección, las dieciséis anteriores no son creíbles. Y es, además, la sección que arq-3 citaba
siete veces sin haberla escrito. Ordenada de más grave a menos.

**1 · He elegido el diseño que se termina antes que el que enseña más, y hay que decirlo así.**
Mi sesgo estaba declarado en el encargo y lo he obedecido, pero obedecerlo tiene un precio contable.
`arq-2` entrena treinta juicios de clasificación sobre procesos reales con justificación escrita; yo
entreno treinta y uno pero **veinticuatro de ellos con una sola letra y sin justificar**. El Mapa corto
es más barato y más superviviente; también es más superficial. Si la alumna resultara ser de las que
terminan cualquier cosa que empiezan, `arq-2` le habría enseñado más criterio panorámico que esto. He
apostado a que no lo es, porque el 52 % no llega a empezar y porque tiene jornada completa — pero es
una apuesta sobre una persona a la que no conozco.

**2 · La cuota de cuatro sigue dependiendo de su honestidad consigo misma, y no tengo forma de
comprobarla.**
He apilado tres capas —descartes aritméticos, motivos tipificados, cuota que excluye las zonas
prohibidas— y sigue siendo cierto lo que dice la autocrítica de `arq-2`: **las cuotas producen
cumplimiento de cuota**. La señal de fallo que lo busca de frente («existe un veredicto 1 o 2 que puse
para llegar a cuatro») depende de que ella se conteste con sinceridad, sin nadie que compruebe. La única
mitigación real que he encontrado es que **la clave sellada de los dobletes sí tiene oráculo**, así que
al menos siete de los treinta y un juicios se contrastan contra algo que ella no escribió. Los otros
veinticuatro, no.

**3 · La calidad sustantiva de su ficha de criterio y de su batería no la comprueba nada, y es un
defecto compartido por las tres arquitecturas.**
Ella escribe la ficha de criterio, ella escribe los diez casos, ella escribe la clave. Puede escribir
cinco indicadores observables e **irrelevantes** y pasar todos los filtros: el Ctrl+F, la prueba de
tamaño, la muestra apartada. El único parche que existe es el de `arq-1` —*al menos un indicador
verificable contra fuente externa; si todos son críticos, no ha priorizado*— y lo he incorporado, y es
poco. **Nadie le va a decir que está midiendo lo que no importa.** La prueba ciega de M5 lo detecta a
medias y trece semanas tarde.

**4 · La fusión de M5 y M6 en un módulo de tres semanas es la decisión con menos respaldo de todo el
documento.**
La he tomado para acortar la meseta, que es el argumento correcto bajo mi sesgo, pero **medir** y
**traspasar** son dos operaciones distintas y he metido una tercera —la reproducción del número— en el
módulo siguiente para que quepa. Si el material resulta denso ahí, la reparación correcta es volver a
partirlo y aceptar dieciocho semanas. Lo digo aquí para que quien produzca el material sepa cuál es la
costura que puede soltarse sin romper nada.

**5 · El módulo de adopción tiene la autocorrección más débil, y su criterio de éxito no lo controla
ella.**
El piloto es binario y se provoca en vez de esperarse, que es lo mejor disponible. Pero si su compañera
no lo usa, hay al menos cuatro explicaciones y el material no le da forma de distinguirlas. **Es el
único punto del curso donde una alumna diligente puede hacerlo todo bien y salir sin saber si lo hizo
bien.** He escrito la sexta lectura legítima —que el artefacto no debía adoptarse— antes de que ocurra,
y es lo único que se puede hacer.

**6 · El problema del buzón compartido está prevenido, no resuelto.**
La cuarta columna del embudo lo cobra en la semana 1 y la regla del embudo vacío ofrece tres salidas.
Pero la salida A —pedir que le deleguen una etiqueta o una carpeta propia— **es una petición a otra
persona, que es exactamente lo que el diseño prometía no necesitar**, y la salida B acota el proceso a
un trozo más pequeño, que es una rebaja real aunque la haya presentado como neutra. Nadie ha resuelto
esto y yo tampoco: lo que he hecho es que se descubra cuando cuesta diez minutos en vez de seis semanas.

**7 · El monocultivo sigue afectando a la disponibilidad de mecanismos, aunque menos.**
La tarde de P27 recupera la doble codificación, la tabla de confusión y la práctica multilingüe con
independencia del hilo. Pero si su proceso no toca datos ámbar ni rojos —y el embudo puntúa **+2** a
«solo verde», es decir, **empuja precisamente hacia ahí**—, el mapa de datos de M2 sale flaco y la
lección de protección de datos se queda más abstracta de lo que debería. Es una contradicción real del
diseño: el filtro que protege el arranque es el mismo que empobrece una de las lecciones. La mitigación
—el ejercicio del semáforo sobre diez correos reales suyos, que **sí** contienen ámbar y rojo, y la
exigencia de declarar uno **no reescribible**— es de M0 y es buena, pero es un ejercicio, no el
proceso.

**8 · La agnosticidad se demuestra con hora y media contra treinta y dos horas.**
Dos pruebas de traslado (25 + 20 min), siete preguntas fijas con su mitad de herramienta, el tercer
registro en cada lección y una ficha de cinco preguntas sobre una herramienta ajena. Es lo mejor que se
me ocurre que quepa en un curso de dos horas semanales, y **la proporción no tranquiliza**. Las dos
pruebas de traslado además nunca tocan la parte difícil: la nº 1 va con material verde porque no puede
ser de otro modo, y la nº 2 es sobre papel. Demuestro que **el criterio viaja**; no demuestro que ella
sabría trabajar de verdad en otra herramienta con datos reales. Hay que llamarlo por su nombre.

**9 · La Tira es la mejor idea del conjunto y la más frágil de mantener.**
Exige sostener diez casos vivos durante diecisiete semanas y volver a pasarlos seis veces. Es poco
trabajo cada vez —media hora— pero es **trabajo sin novedad**, y lo que no tiene novedad se convierte en
ritual o desaparece. Las puertas la fuerzan en dos sitios, pero las puertas se pueden saltar en un curso
sin profesor. Si la Tira se erosiona, la lección central del curso —*la calidad se gana en la capa 1 y
la capa 2; lo demás cambia quién dispara*— desaparece con ella y no hay sustituto.

**10 · El curso le pide a la vez que use la IA como correctora y que no se fíe de ella.**
Tres cebos, siete reglas de protocolo y una tabla de descalificación por entregable es lo mejor que
tengo. Está resuelto en el papel; **no sé si está resuelto en el mes cuarto, un jueves, cansada**. Y hay
un dato que conviene tener escrito: **no existen datos publicados sobre cómo se comporta un modelo de
2026 corrigiendo un entregable contra una rúbrica dada**, que es exactamente nuestro caso. El cebo no es
un adorno: es lo único que tenemos, y puede resultar que la respuesta sea «para este tipo de trabajo, la
IA no corrige».

**11 · Nada de esto lo he visto.**
Los 32 procesos, los volúmenes, el buzón compartido, la carpeta de plantillas con seis versiones: todo
es reconstrucción [R] a partir del sector, no observación de su empresa. El curso está diseñado para que
**su primera tarea sea tachar y corregir** ese mapa, que es la única forma honesta de convertir una
reconstrucción en su realidad. Pero si el mapa está muy equivocado, el M0 habrá que reescribirlo sobre
la marcha y varios ejemplos perderán fuerza precisamente por lo que se supone que los hace fuertes: por
ser concretos.

**12 · Y el dato del que depende medio diseño sigue sin conocerse.**
Qué plan tiene contratada su empresa y cómo está configurado **[NV]**. De ahí depende qué versión de M3
se ejecuta, si la clasificación en lote tiene ruta cómoda o incómoda, y si la automatización por sucesos
existe para ella. He puesto rutas alternativas y la restricción de que ningún módulo dependa del
constructor de flujos, pero **una contingencia no es lo mismo que un diseño**, y no se sabrá hasta la
semana 2, con el curso ya escrito.

---

# 18. DÓNDE ACABA LO HEREDADO Y DÓNDE EMPIEZA LO MÍO

**Heredado de los informes de dominio y de las tres arquitecturas, sin volver a verificar:** los procesos
P01–P32 con sus volúmenes y riesgos · el semáforo, los ejercicios E-01…E-06 y el Anexo III · los
escalones, las capacidades reales de la plataforma y sus límites verificados · los mecanismos de
corrección 1–9, el protocolo de siete reglas y los puntos de caída · las correspondencias C1–C13 y
EP-01…EP-14 · los cinco pasos de la referencia y sus citas.

**Decisiones de diseño mías [J], sin respaldo externo, y quien evalúe este documento debe saberlo:**

- **La elección de columna vertebral** y el argumento de que los instrumentos se trasplantan y una
  propiedad estructural no (§0.1).
- **La compresión a 17 semanas y 7 módulos**, y en particular la fusión de M5 y M6.
- **El Mapa corto y su segunda vuelta como pretest/postest del propio criterio** (§4.5). Es la pieza más
  nueva del documento y la que menos respaldo tiene fuera de la lógica psicométrica.
- **La partición de la cuarta columna del embudo** entre criterio durable y límite fechado (§0.2).
- **La regla del embudo vacío** y sus tres salidas (§5.4).
- **La tarde de P27** como excepción declarada al «una sola cosa» (§6.5).
- **La reducción de cinco puertas a tres** y la regla de que una puerta cerrada cuesta una semana
  presupuestada (§12.3).
- **La cuota de cuatro con las zonas prohibidas excluidas** (§9.2).
- **La lista cerrada de cinco motivos tipificados**, incluidos «las reglas son de otro» y «no necesita un
  modelo».
- **La tabla de descalificación del corrector por entregable** (§12.4).
- **La exigencia de un caso en idioma minoritario real** en la batería y **la parada por idioma no
  probado** como freno obligatorio.
- **La movilidad declarada de M6** y su redacción en la semana 1.
