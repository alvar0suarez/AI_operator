# Diseño del curso · v1

> # Delegar bien
> ### Un proceso tuyo, de punta a punta — y el criterio que se queda cuando cambien las herramientas

**Qué es esto.** El diseño unificado y ejecutable del curso descrito en `curso/00-perfil.md`. Arbitra
entre las dos síntesis independientes —`sintesis-A-continuidad.md`, sesgada a que ella llegue al final, y
`sintesis-B-criterio.md`, sesgada a que lo aprendido le dure— y resuelve cada discrepancia con una
decisión argumentada. Donde A y B coinciden, la coincidencia es doble validación y esa parte va tal cual y
sin volver a defenderse.

**Fuente de verdad:** `curso/00-perfil.md`, revisión del 22.08.2026. **Manda sobre este documento.**
**Fecha:** 23.08.2026.

**La regla del arbitraje, escrita antes de arbitrar nada.** Las dos restricciones son igual de duras:
**que llegue al final** y **que lo aprendido le dure**. Sacrificar cualquiera de las dos invalida el
encargo, porque un curso de criterio abandonado en la semana 4 no enseña criterio, y un curso que se
termina entero y caduca en dieciocho meses no cumple el objetivo 4 del perfil. Por eso ninguna
discrepancia se ha resuelto promediando ni votando: en cada una se ha buscado **la formulación que paga
las dos facturas**, y donde no existía —hay tres sitios— se ha elegido y se ha declarado qué se pierde
(§18).

**Marcas:** **[V]** verificado en fuente primaria · **[R]** reconstrucción razonada · **[E]** evidencia
publicada citada en los informes de dominio · **[NV]** no verificable desde fuera · **[!]** decisión que
no es suya y se escala · **[J]** juicio de diseño de este documento, argumentado y sin respaldo externo.

---

# 0. LA DECISIÓN DE COLUMNA VERTEBRAL, Y EL MAPA DE ARBITRAJES

## 0.1 Columna vertebral — donde A y B coinciden, y por qué la coincidencia importa

**A y B eligen la misma columna vertebral: `arq-3-proceso`. El curso es la transformación de UN proceso
suyo, capa a capa, hasta que funciona, hasta que lo usa sin que nadie se lo pida y hasta que sobrevive a
sus vacaciones.**

Que dos síntesis con sesgos deliberadamente opuestos lleguen a la misma columna vertebral **contra dos de
los cuatro jueces** es el resultado más sólido del corpus, y conviene entender por qué ocurre, porque el
argumento es el mismo desde los dos lados:

> **Lo que hace ganar a arq-1 y a arq-2 en sus lentes son instrumentos, y los instrumentos se trasplantan
> en una página. Lo que hace ganar a arq-3 en la suya es una propiedad de la columna vertebral, y no se
> trasplanta.**

Las puertas, las cinco preguntas y el tercer registro de arq-1 son un mecanismo de tres líneas, una ficha
y una convención de maquetación. Los seis veredictos, la regla del cuatro y la segunda vuelta de arq-2 son
formatos. Todos están injertados abajo. En cambio, **que el artefacto esté en producción sobre su mesa y
el mundo la corrija cada martes** es consecuencia directa de que el curso sea un proceso, y
`dominio-autodidacta.md` §3.2 pone la ejecución real en el puesto 1 de nueve mecanismos de corrección, por
encima de la batería y muy por encima de la IA correctora.

Y las dos síntesis añaden, cada una desde su sesgo, la mitad que le faltaba a la otra:

- **Desde el sesgo de continuidad (A):** abandonar en la semana 12 la deja con un sistema funcionando;
  abandonar un curso de inventario en la semana 4 la deja con una hoja de cálculo, y abandonar un curso de
  escalera en la semana 16 —donde su propio autor admite que se detiene la gente— la deja sin el escalón
  que lo corona.
- **Desde el sesgo de durabilidad (B):** el criterio **no se deduce solo del recorrido**. Una extracción
  sin clasificador produce prosa; una extracción sin contraste externo produce generalidades. Por eso el
  recorrido lleva encima un clasificador dimensional (las cinco preguntas), una rejilla de decisión
  cerrada (los seis veredictos) y un contraste con clave (los dobletes sellados).

**Las dos mitades son la tesis de este documento y ninguna es negociable.**

## 0.2 El límite de la tesis, dicho en la primera página

**Funcionar no es estar bien.** El uso diario detecta que algo molesta; no detecta que el criterio estaba
mal escrito ni que la batería era fácil. **El mundo corrige la utilidad; los instrumentos corrigen el
criterio.** Por eso el aparato de §12 —batería con clave sellada, listas binarias, rúbricas negativas,
tres cebos, cuatro puertas— está entero, y por eso §12.1 le pone además un techo, para que no se convierta
en el trabajo en vez de en su control.

Y el segundo límite, que es el riesgo del ángulo: **un solo proceso puede no dar ocasión de practicar todo
el criterio.** Contra eso hay cuatro contramedidas con nombre —el Mapa de los doce con sus dos pasadas,
los ocho dobletes con clave sellada, la tarde de P27 y la Lista de techos— y el saldo honesto está en §17.

## 0.3 Las quince discrepancias entre A y B, y cómo se han resuelto

Tabla índice. Cada fila se argumenta en su sitio y se recapitula en §18.

| # | Discrepancia | A propone | B propone | Decisión |
|---|---|---|---|---|
| 1 | **Duración y módulos** | 17 sem., 7 módulos (funde medir y traspasar) | 18 sem., 8 módulos | **B**, y la meseta se acorta con un hallazgo dentro, no fundiendo |
| 2 | **Clasificación panorámica** | Mapa corto de 12 en la semana 1 (pretest) + 2.ª vuelta en la 17 | Rejilla de 12 justificada en la semana 14 | **Las dos: son instrumentos distintos.** Pretest sem. 1 · rejilla sem. 14 · delta sem. 17 |
| 3 | **Puertas que bloquean** | Tres | Seis | **Cuatro** [J], con criterio explícito de qué justifica bloquear |
| 4 | **Asistente v1 que cita** | Día 4–5 | Día 3 | **Día 4, con la precondición de B** (detrás del diagnóstico del entorno) |
| 5 | **Motivos tipificados** | Lista cerrada de cinco | Tres + un cuarto con nombre propio | **A**: una sola lista de cinco, usada en los cuatro sitios |
| 6 | **Cuota de noes en la rejilla** | Cuatro de doce, **sin contar las ZP** | Cuatro de doce, ZP incluidas | **A**: excluir las ZP es lo que la hace exigente |
| 7 | **Dobletes** | Siete (por tener 7 módulos) | Ocho | **Ocho** + el mini-doblete de P16 que aporta A |
| 8 | **La tarde de P27** | Obligatoria, 90 min en M3 | Contingente (solo si su proceso es monolingüe) | **A**: un mecanismo contingente no está en el diseño |
| 9 | **Multilingüe en la batería** | Un caso de diez | Un típico **y** un límite | **B**: cuesta cero y cierra el hueco |
| 10 | **Cuarta columna del embudo** | Pregunta durable + límite fechado | Igual, con mejor formulación | **B** en la redacción, **A** en el reparto criterio/clics |
| 11 | **Embudo vacío** | Tres salidas nombradas | Escalera de cuatro pasos con precio declarado | **B** en la escalera, **A** en el plazo («se resuelve el día 3») |
| 12 | **Descarte de los seis** | Por número, aritmética pura | Escribiendo el motivo transferible de los seis | **Híbrido** [J]: descarte por número + tres motivos contra clave |
| 13 | **La Tira** | Seis columnas | Cinco | **B**: cinco. Una pasada menos es una ocasión menos de que se convierta en ritual |
| 14 | **Instrumentos permanentes** | Seis, con el Mapa dentro | Seis, con la rejilla dentro | **B**, y el Mapa pasa a ser el momento de volumen del instrumento 2 |
| 15 | **Nombre del curso** | «Un proceso tuyo, de punta a punta» | «Delegar bien» + subtítulo | **B** |

**Y cuatro piezas que no están en ninguna de las dos** [J], todas nacidas de las cuatro preguntas que el
encargo manda resolver:

| Pieza | Qué resuelve | Dónde |
|---|---|---|
| **El orden de sacrificio por módulo** | Cuánto rigor se le puede pedir sin perderla: lo que se cae primero cuando la semana se tuerce, y lo que no se cae nunca | §6, cada módulo |
| **El techo del 20 % y la regla de retirada** | Cuánta autocorrección es suficiente antes de que se vuelva burocracia | §12.1 |
| **La tarjeta de siete casillas de la semana 1** | Que el pretest del Mapa sea interpretable sin haber enseñado todavía la rejilla | §4.2 |
| **El criterio de qué justifica una puerta que bloquea** | Por qué cuatro y no tres ni seis | §12.3 |

---

# 1. NOMBRE Y TESIS

## 1.1 Nombre

> # Delegar bien
> ### Un proceso tuyo, de punta a punta — y el criterio que se queda cuando cambien las herramientas

**Por qué este y no el de A.** Los dos son buenos y ninguno nombra un producto, una tecnología ni un año.
Gana el de B por dos razones concretas: nombra **la operación** —delegar— en vez de solo el objeto, y su
subtítulo anuncia las dos mitades del encargo en una línea, que es exactamente la gestión de expectativas
que este curso necesita (los objetivos 2 y 4 del perfil, literalmente). El de A, además, contenía el
número de capas —«siete»— en el propio título: un título que hay que reescribir si el mapa cambia de siete
a ocho módulos es un título mal construido.

Y no nombra un rol. Ni «AI Operator», ni «especialista en IA», ni nada que empuje hacia una identidad
profesional que el perfil excluye con todas las letras.

## 1.2 Tesis

> **Se aprende a delegar delegando una cosa entera, no doce a medias. Un proceso llevado de punta a punta
> —hasta que funciona, hasta que ella lo usa sin que nadie se lo pida y hasta que sobrevive a sus
> vacaciones— enseña más criterio que doce diagnósticos sobre papel, porque es el único formato en el que
> cada decisión recibe la respuesta del mundo.**
>
> **Y el criterio no se deduce solo del recorrido: se extrae con un ritual, se clasifica con un
> instrumento y se contrasta contra clave sobre procesos que no son el suyo. El recorrido produce la
> experiencia; los instrumentos la convierten en algo que viaja a otra empresa y a otra herramienta.**
>
> **Corolario que lo convierte en arquitectura:** el curso no la sube por una escalera de herramientas.
> **La escalera aparece sola, por debajo, porque un proceso al que aprietas va pidiendo cosas en ese
> orden.** Primero pide que alguien escriba qué es hacerlo bien. Después, contexto que no haya que volver
> a explicar. Después, dejar de depender de que ella se acuerde. Después, juicio en dos sitios y frenos en
> otros tres. Después, que alguien compruebe si de verdad sirve. Después, poder existir sin ella. Y al
> final, que otra persona lo use.

Cinco corolarios operativos. Los cinco son restricciones de producción, no lemas:

**(a) La unidad del curso es la capa, no la herramienta ni la tarea.** Un módulo se llama «Que ocurra sin
que lo pidas», nunca «Acciones programadas» ni «Automatizar el proceso 27». La capa es anatomía; la
herramienta es la implementación de hoy y vive en un fichero aparte y fechado. **El índice del curso no
puede caducar.**

**(b) La teoría entra cuando el proceso la pide, y solo la que pide.** No hay módulo de panorama ni
catálogo previo. Lo que el proceso no pide se cubre con veinte minutos en seco —el Doblete—, con una fila
de la Lista de techos, o no se cubre y se dice dónde.

**(c) El «no» vive dentro del proceso, no fuera.** El primer entregable serio no es «qué automatizo» sino
**la línea de corte**: el proceso partido en trozos, cada trozo con uno de los seis veredictos y con el
motivo elegido de una lista cerrada. Un proceso partido en trozos con veredicto es el sitio más barato del
mundo para aprender que a veces la respuesta es que no.

**(d) Cada capa se cierra con una extracción escrita, y cuatro de ellas con una condición observable que
bloquea.** Sin profesor, una puerta que bloquea es la única figura que se parece a un «todavía no». Pero
solo bloquean cuatro, y §12.3 escribe por qué exactamente esas.

**(e) El criterio portátil se mide dos veces, no se promete.** Doce tareas suyas clasificadas en la semana
1 con una tarjeta de definiciones, las mismas doce clasificadas en la semana 14 con el criterio ya
adquirido, y el delta leído en la semana 17 con el motivo de cada cambio. **El objetivo 4 del perfil deja
de ser una promesa y pasa a ser una tabla con dos columnas y un delta.**

---

# 2. PERFIL DE ENTRADA Y DE SALIDA

## 2.1 De dónde parte, sin adornos

| Dimensión | Estado en la semana 0 |
|---|---|
| **Formación** | Licenciatura en Psicología. Sin base técnica. **Nunca ha abierto una terminal**, y no va a abrirla en este curso |
| **Puesto** | Atención al cliente en una academia de español para extranjeros de ~30 empleados en Madrid, con alojamiento de larga estancia. **Jornada completa** |
| **Uso de IA** | ChatGPT, Claude y Gemini **como chat**: entra a la web, escribe, lee, copia. No ha guardado nunca un asistente, no ha adjuntado nunca una fuente para que la cite, no ha programado nunca nada |
| **Dominio** | **Experta.** Sabe cosas de su puesto que no están escritas en ningún sitio de la academia. **Esa es la materia prima del curso** |
| **Método** | Operacionalizar un constructo difuso, diseñar instrumentos, evaluar validez, entrevistar. Transferencia FUERTE en ocho de trece correspondencias (`dominio-psicologia.md` §2) |
| **Entorno** | Gemini de pago dentro de la suite de su empresa, recomendado como estándar. **No sabe qué plan ni cómo está configurado** [NV] |
| **Restricciones** | Autodidacta · pareja con conocimientos de IA para consultas puntuales, que **no corrige entregas ni sigue el progreso** · cero presupuesto |
| **Punto ciego declarado** | No tiene mapa de qué existe ni de qué se puede automatizar de su trabajo |
| **Riesgo de perfil** | No es quedarse corta de rigor: **es pasarse.** Un solo proceso es un imán para el perfeccionismo |

**Lo que su formación NO le da**, y va escrito en el material la primera vez que hace falta (M3): entender
por qué el paso 3 de un flujo no ve lo que produjo el paso 1 salvo que se lo pases; tolerancia al trasteo;
pensar en datos estructurados; diagnosticar por qué falla un sistema. Eso es nuevo, se aprende haciendo, y
le va a costar los dos primeros intentos. **Sin esta mitad, la otra mitad es adulación.**

## 2.2 A dónde llega

**Con un objeto en la mano:**

1. **Un proceso suyo funcionando y en uso diario**, con criterio escrito, fuentes fechadas, disparador,
   tope, frenos probados, apagado probado, dueño con nombre y calendario de revisión.
2. **Un número medido con su método**, con la revisión y el mantenimiento restados, con una amenaza a la
   validez que no puede descartar, y **reproducible dentro del ±10 % dos semanas después**.
3. **Una segunda persona** que ha usado su sistema **cinco días laborables sin ella delante**, y la lista
   de lo que ese piloto obligó a arreglar.

**Con un criterio en la cabeza, que es lo que se lleva si mañana cambia de empresa:**

4. **Clasifica cualquier herramienta** —incluida una que el curso no le enseñó y una que no existe hoy—
   respondiendo cinco preguntas, y **deriva de las respuestas** qué salvaguardas necesita y qué datos no
   le puede meter.
5. **Asigna a un proceso cualquiera uno de seis destinos**, dos de los cuales son «aquí no metas IA», con
   el motivo elegido de una lista cerrada de cinco y **citando un hecho observable del proceso**, no una
   impresión.
6. **Escribe el criterio de «bien hecho» antes de construir**, y una batería que lo comprueba.
7. **Mide si algo sirve** y sabe decir qué amenaza a la validez no ha descartado.
8. **Deja lo que monta en condiciones de sobrevivirle**, y sabe explicarlo en treinta segundos sin nombrar
   ninguna herramienta, incluido **lo que no hace**.

**Con una posición, que es lo que pide el objetivo 5:** llega a las conversaciones de su empresa con una
cosa que funciona, un número que aguanta que lo repregunten y **una lista de lo que decidió NO automatizar,
con el motivo**. Esa lista es lo que hace que le crean el resto.

**Y con lo que expresamente NO es:** no es especialista en IA, no ha cambiado de rol, no tiene portfolio,
no tiene certificado, no sabe programar y no es «la de la IA» de la academia. **Sigue siendo la persona de
atención al cliente de una academia de idiomas, haciendo su trabajo con otro método.**

## 2.3 La definición observable de «terminado», fijada en la semana 1

> Un proceso suyo funcionando y **en uso diario sin que el curso se lo pida** · un número medido con su
> método y **reproducido a las dos semanas** · **ocho preguntas fijas** contestadas con sus dos mitades ·
> **ocho dobletes firmados, de los cuales al menos tres terminan en «no aplica», contrastados contra su
> clave** · **el Mapa de los doce con sus dos pasadas y su delta explicado** · **una rúbrica escrita por
> ella y validada contra un cebo** · y **una segunda persona que ha usado su sistema cinco días laborables
> sin ella delante**.

No es «leer la última lección». Y **la rúbrica escrita por ella es el indicador honesto de que ya no
necesita el material**: cuando escribe rúbricas que cazan defectos conocidos, el curso ha terminado su
trabajo.

---

# 3. RESULTADOS DE APRENDIZAJE OBSERVABLES

Verbos de desempeño. Ninguno dice «entenderá», «conocerá» ni «será capaz de valorar». Cada uno con su
evidencia observable y el módulo donde se cierra.

| # | Al terminar, ella… | Evidencia observable | Cierra en |
|---|---|---|---|
| **RA1** | **Elige** un proceso propio aplicando criterios de rechazo observables y **descarta** por escrito los que no pasan | Hoja de elección: 32 procesos tachados y corregidos, seis descartes automáticos, **tres motivos escritos contra clave**, 6–8 candidatos puntuados en cinco columnas, repuesto firmado con fecha | M0 |
| **RA2** | **Describe** un proceso suyo como se ejecuta de verdad —disparador, documentos, decisiones no escritas, salida—, **por observación y no de memoria** | La descripción contiene **al menos dos decisiones que no estaban en su idea previa**. Si no las contiene, se escribió de memoria y se vuelve a observar | M0 |
| **RA3** | **Determina** bajo qué régimen de datos trabaja —entrenamiento, retención, ubicación, contrato, política interna— **o documenta** a quién y cuándo lo preguntó | Ficha del entorno, ocho casillas, **ninguna frase que empiece por «creo que»**. *«Pregunté a X el día D y no obtuve respuesta»* es un resultado válido | M0 |
| **RA4** | **Clasifica cualquier sistema** —incluido uno que el curso no le ha enseñado— con **las cinco preguntas**, y **deriva** qué salvaguardas necesita y qué datos no puede meterle | Ficha rellenada para: su chat de hoy (M0), cada capa (M1–M7) y **una herramienta que el curso no enseñó** (M4), con sus tres comprobaciones | M0 → M4 |
| **RA5** | **Traza la línea de corte** de su proceso: cada trozo con **uno de los seis veredictos**, con el motivo de la lista cerrada de cinco, y para cada «no» **qué sí se puede hacer alrededor** | Al menos un trozo se queda con ella; ningún motivo es «es difícil»; cada «no» lleva un artefacto **nombrable**, no una intención | M1 |
| **RA6** | **Escribe** el criterio de «resultado correcto» en 4–6 indicadores comprobables sí/no contra una fuente, **antes** de tocar ninguna herramienta | Ficha de una cara, sin *adecuado, correcto, natural, profesional, de calidad* sin ancla detrás; **al menos un indicador verificable contra fuente externa**; no todos marcados como críticos | M1 |
| **RA7** | **Construye** una batería de diez casos —5 típicos, 3 límite, 2 de rechazo— apartados **antes** de escribir el prompt, con **un típico y un límite en un idioma minoritario real de su buzón**, y **la vuelve a pasar con fecha** en cada capa | La Tira: cinco columnas fechadas al terminar. Clave sellada escrita el mismo día | M1 → M5 |
| **RA8** | **Sitúa** cada dato que atraviesa su proceso en verde/ámbar/rojo, **marca en qué paso entra y en cuál hay que quitarlo, y quién lo quita**, y **reescribe** casos reales que sobreviven a la prueba de la compañera **y siguen sirviendo** | Mapa de datos, una cara, cuatro columnas; tres casos reescritos útiles y **uno declarado no reescribible** | M2 |
| **RA9** | **Monta** un asistente con fuentes propias fechadas que **cita el documento y su fecha** y **dice «no lo sé»** | 5/5 en típicos · pide aclaración en los 3 límite (inventar es fallo aunque acierte) · «no lo sé» en los 2 de rechazo (acertar es suspenso) | M2 |
| **RA10** | **Reconstruye** una capa suya en otra herramienta **en menos de veinte minutos** y **nombra** qué viajó tal cual, qué hubo que rehacer y qué techo cambió | Ficha de traslado, tres columnas con cosas concretas. *Si no lo consigue en veinte minutos: aprendió la ruta, no la capacidad, y el diagnóstico llega a tiempo* | M2 |
| **RA11** | **Monta** algo con disparador que **prepara, clasifica o avisa y nunca envía**, con tope, y **lo apaga habiéndolo probado** | Cinco casos fabricados disparan y producen las cinco salidas correctas; **un sexto que NO debe disparar no dispara**; el tope se prueba con un lote grande; el apagado está hecho, no imaginado | M3 |
| **RA12** | **Aplica un criterio escrito a decenas de unidades de golpe** y **compara su propia codificación con la del sistema** construyendo la tabla de confusión, **y con la clave del curso** | ≥26/30 de acuerdo · una frase por confusión repetida · acuerdo de la categoría minoritaria mirado aparte · <15 % sin clasificar y **no 0 %** · comparación contra la codificación de referencia | M3 |
| **RA13** | **Escribe su flujo en notación neutra** y **localiza cada pieza en la documentación de otra plataforma que no ha usado**, sin dar de alta ninguna cuenta | Tres líneas: las cinco piezas y su nombre allí · la que allí no existe · la que allí es más fácil | M3 |
| **RA14** | **Distingue** en su proceso qué parte tiene pasos fijos y qué parte necesita juicio, y **argumenta por qué un agente autónomo sería exceso aquí** | Media página con la frontera trazada y los dos puntos de juicio nombrados, cada uno con su criterio escrito | M4 |
| **RA15** | **Escribe** temas prohibidos y condiciones de parada —incluidas **la parada por agencia con convenio** y **la parada por idioma no probado**— y **las prueba con casos fabricados que deben parar** | Cinco casos de parada, cinco paradas observadas con marca y motivo; **un sexto normal que NO para**; «quién revisa» es **un nombre y una hora** | M4 |
| **RA16** | **Reconoce** cuál es el único proceso de su academia que caería en el Anexo III del Reglamento de IA y **a quién lo escala** | Una frase, un nombre, un puesto. Y el verdadero/falso de doce ítems con ≥10 aciertos | M4 |
| **RA17** | **Audita a su propio corrector** con artefactos-cebo de defectos plantados y **decide con ese dato** si la IA sirve para corregir ese tipo de trabajo | Hoja de resultado de los tres cebos + decisión escrita + **al menos un caso registrado en que NO aceptó una crítica de la IA, con el motivo** | M1, M4, M6 |
| **RA18** | **Mide** el efecto en **minutos por unidad**, **resta** revisión y mantenimiento, **nombra** una amenaza que no puede descartar, y **reproduce el número** dos semanas después | Media página sin la palabra «significativo», con la resta hecha; el recálculo cae dentro del **±10 %** o el dossier se reescribe | M5, M7 |
| **RA19** | **Deja el sistema en condiciones de sobrevivirle**: fuentes con fecha y dueño, calendario de revisión, apagado probado, ficha de traspaso | «Quién lo mantiene» responde con **nombre propio**; «cuándo caduca cada fuente» responde con **fecha**; la prueba del hueco está lanzada | M6 |
| **RA20** | **Clasifica doce procesos suyos** con la rejilla, justificando cada uno con **un hecho observable**, y **al menos cuatro** terminan en «ni IA» o «arreglar el proceso primero» —**sin contar las zonas prohibidas**—, cada uno con su «lo que sí alrededor» | El Mapa de los doce, pasada 2, firmado y fechado. Ninguna justificación es una impresión | M6 |
| **RA21** | **Compara sus dos pasadas** del Mapa y **explica cada cambio** con un motivo de la lista cerrada | Dos columnas al lado, X cambios, una frase por cambio, y una frase por cada veredicto que no cambió y sobre el que hoy tiene más confianza | M7 |
| **RA22** | **Escribe la rúbrica** de un artefacto suyo, con ≥3 criterios negativos que exigen salida escrita, y **la valida contra un cebo** | Si el cebo pasa su rúbrica, la rúbrica es blanda y se rehace | M6 |
| **RA23** | **Entrega** su artefacto a otra persona, que lo usa **cinco días laborables sin ella**, y **corrige** lo que el piloto revele | Ficha de traspaso + **lista de al menos dos cosas que hubo que arreglar**. *Si el piloto no reveló nada, no fue un piloto* | M7 |
| **RA24** | **Explica** en treinta segundos, **sin nombrar ninguna herramienta**, qué hace su sistema, qué ahorra y **qué no hace** | La prueba del pasillo, con sus cuatro comprobaciones binarias, ante alguien que no ha visto el artefacto | M7 |
| **RA25** | **Contesta la pregunta fija** al cerrar cada capa, con sus dos mitades, y **firma ocho dobletes** de los cuales **al menos tres son «no aplica»**, contrastándolos contra la clave sellada | Cuaderno de capas: ocho fichas con las seis casillas + ocho dobletes con veredicto y comparación anotada | todos |

**Los tres resultados que hacen falsable la agnosticidad, con su condición de fracaso escrita:**

> Si al terminar no puede **rellenar la ficha de cinco preguntas para una herramienta que el curso no le
> enseñó** (RA4), **reproducir una capa suya en otro sitio en veinte minutos** (RA10) y **localizar las
> piezas de su flujo en la documentación de una plataforma que no ha visto** (RA13), entonces **este fue
> un curso de una herramienta y fracasó**, por muy bien que hayan salido los demás resultados.


---

# 4. LOS SEIS INSTRUMENTOS PERMANENTES

Van antes del mapa de módulos porque todos los módulos cuelgan de ellos, y porque **son lo que queda
cuando el curso se acaba y cuando las herramientas cambien**. Los seis cumplen las mismas cuatro
condiciones, y esas condiciones son el motivo de que sean estos y no otros:

1. **Contestan una pregunta permanente**, no una pregunta de 2026.
2. **No nombran ningún producto** (salvo una línea aislada y fechada, cuando hace falta).
3. **Tienen comprobación mecánica**: se sabe en diez segundos si están bien rellenados.
4. **Los escribe ella.** Un fichero copiado no se relee; uno escrito, sí.

| # | Instrumento | A qué objetivo del perfil sirve | Por qué sobrevive al curso |
|---|---|---|---|
| 1 | **Las cinco preguntas** | 1 (saber qué existe) y 3 (datos) | Clasifica por autonomía cedida, que es una **propiedad** de cualquier sistema, no un catálogo de productos |
| 2 | **La rejilla de los seis veredictos** | 1 y 4 | Las **pruebas** que deciden cada veredicto interrogan la tarea, no la herramienta, y no caducan |
| 3 | **El Expediente del proceso** | 2 (automatizar lo suyo) | Es el sistema, no documentación sobre el sistema |
| 4 | **La Tira** | 2 y 4 | Es una medición de su propio trabajo con fecha; no depende de ninguna herramienta |
| 5 | **El Cuaderno de capas** (cinco preguntas + pregunta fija + doblete) | 4 (criterio portátil) | Es el curso entero escrito en su lenguaje y sin nombres de producto |
| 6 | **La Lista de techos** | 1 | Es un catálogo cuya tercera columna son **condiciones**, y las condiciones no se renombran |

> **Arbitraje 14.** A propone seis instrumentos con el Mapa de los doce dentro y los veredictos disueltos
> en el Cuaderno; B propone seis con la rejilla dentro y el Mapa disuelto. Gana B, y el motivo es de
> categoría: **la rejilla es un instrumento y el Mapa es un momento de uso del instrumento.** Meter el
> momento en la lista y dejar fuera el instrumento habría producido un cuaderno con dos entradas para lo
> mismo. El Mapa de los doce, con sus dos pasadas, se describe dentro del instrumento 2 (§4.2), que es su
> sitio.

Y un séptimo objeto que no es un instrumento sino un hilo de dos minutos: **el Cuaderno de evidencias**
(§4.3), que vive dentro del Expediente y existe desde la semana 3 por una razón operativa y no ceremonial
—**si M7 tuviera que fabricar las pruebas al final, las inventaría**—.

---

## 4.1 Instrumento 1 · LAS CINCO PREGUNTAS — el clasificador

*(injerto de arq-1 §1.2, coincidente en A y B, y el instrumento más portátil de todo el corpus)*

| # | Pregunta | Respuestas, de menos a más autonomía cedida |
|---|---|---|
| **1** | **¿Quién dispara?** | yo, cada vez · un reloj · un suceso · lo decide el sistema |
| **2** | **¿Quién decide los pasos?** | yo, sobre la marcha · yo, de antemano, y quedan fijos · el sistema, sobre la marcha |
| **3** | **¿De dónde saca lo que sabe?** | de lo que le pego en el momento · de fuentes que yo controlo y fecho · de donde quiera |
| **4** | **¿Qué puede tocar?** | nada · leer lo que yo le doy · leer todo lo que yo puedo leer · escribir en lo mío · escribir hacia fuera |
| **5** | **¿Quién firma la salida?** | yo, siempre · yo, por muestreo · nadie |

**Por qué estas cinco y por qué son el instrumento número uno.** Porque clasifican por **una propiedad**
—cuánta autonomía has cedido— y no por un destino de producto: un catálogo de soluciones es una foto del
mercado de este año, y una dimensión se responde igual sobre algo que todavía no existe. Porque las
respuestas **se observan y no se opinan**. Y porque —esto es lo que las hace insustituibles— **las
preguntas 4 y 5 son literalmente protección de datos y salvaguardas**: por eso en este curso el régimen de
datos no va pegado al final, va **dentro del instrumento con el que se clasifica cualquier cosa**. Quien
contesta las cinco ya sabe qué salvaguardas necesita.

**Dónde vive.** Encabeza la ficha de cierre de cada capa. Se rellenan las cinco filas de nuevo y **casi
siempre cambia una sola fila; ver cuál cambia es la lección**:

```
                      M0 chat  →  M1 criterio  →  M2 fuentes  →  M3 disparador  →  M4 juicio
1 ¿Quién dispara?        yo          yo             yo            un suceso ←      un suceso
2 ¿Quién decide pasos?   yo          yo             yo          yo, de antemano   yo, salvo 2 puntos ←
3 ¿De dónde sabe?     lo que pego  lo que pego   fuentes mías ←   fuentes mías     fuentes mías
4 ¿Qué puede tocar?      nada        nada        leer lo mío ←    leer lo mío    escribir en lo mío ←
5 ¿Quién firma?          yo          yo             yo               yo            yo  ← nunca cambia
```

**La fila 5 no cambia en todo el curso, y eso es contenido, no casualidad.** Es la regla que atraviesa el
diseño entero: *automatiza la lectura y la preparación; la escritura hacia fuera la firma una persona.*

**Tres usos, y el tercero es el que hace falsable la agnosticidad:**

1. **Cabecera del cierre de cada capa.** Tres minutos.
2. **Cierre obligatorio de cada fila de la Lista de techos**, porque las preguntas 4 y 5 obligan a declarar
   por escrito sobre qué recursos actúa un sistema.
3. **Ejercicio terminal de M4 (RA4):** rellenarlas para **una herramienta que el curso no ha enseñado**,
   elegida por ella entre lo que le llegue por cualquier vía, leyendo su documentación quince minutos, y
   contestar tres cosas: *¿lo cubre mi plan? ¿puede actuar sobre los recursos donde vive mi trabajo?
   ¿puedo ver qué hizo?* **Es la prueba de que el instrumento funciona sin el curso.**

**Comprobación mecánica:** ¿están las cinco filas rellenadas con una opción de la escala y no con una frase
libre? ¿ha cambiado alguna fila respecto a la capa anterior? *Si no ha cambiado ninguna, esa capa no te ha
dado nada, y merece la pena saberlo.*

**La propiedad que hay que decirle en la semana 1:** el día que un solo producto haga todo —chat, disparo,
flujo y agente en la misma ventana, que es la tendencia— **estas preguntas no sobran: hacen más falta**,
porque el producto deja de forzar la distinción y ya nada, salvo el criterio, le dice cuánta autonomía
acaba de ceder.

---

## 4.2 Instrumento 2 · LA REJILLA DE LOS SEIS VEREDICTOS — el decisor

*(injerto de arq-2 §3.4, coincidente en A y B en el contenido; B aporta el uso doble, dentro y fuera del
proceso, que es lo que lo rentabiliza)*

| # | Veredicto | La prueba que lo decide (sobre la TAREA, no sobre la herramienta) | Ejemplos de su casa |
|---|---|---|---|
| **1** | **NI IA** | **La servilleta:** ¿podrías escribir los pasos en una servilleta y valdrían siempre? Entonces necesitas una fórmula, una plantilla o un calendario | **P02** presupuestos (aritmética sobre una tabla) · **P22** camas (calendario de recursos) |
| **2** | **ARREGLAR EL PROCESO PRIMERO** | La respuesta a «¿de qué documento sale este dato?» es «pregunto a alguien», «el de siempre», o hay dos versiones y nadie sabe cuál manda | **P32** plantillas en seis idiomas sin control de versiones · cualquier tarea cuyo tarifario vigente no pueda nombrar con su fecha |
| **3** | **CHAT, MEJOR USADO** | Poca frecuencia + mucho juicio + conocimiento que no se repite | **P13** cambios de grupo · **P31** el comentario del informe mensual |
| **4** | **ASISTENTE GUARDADO CON FUENTES** | Se repite, el conocimiento está escrito y es estable, el juicio sigue siendo suyo | **P01** las seis preguntas que repite el 70–80 % de los leads · **P10** certificados |
| **5** | **DISPARADOR Y PASOS FIJOS** | Hay un disparador identificable **y** los pasos son siempre los mismos | **P27** encuestas · **P30** parte semanal · **P06** recordatorio de pagos |
| **6** | **FLUJO CON JUICIO** | Hay disparador, pero en dos o tres puntos hay que **evaluar** algo para saber por dónde seguir | **P28** triaje de reseñas · **P20** clasificar y enrutar incidencias (nunca responderlas) |
| **ZP** | **ZONA PROHIBIDA** — no es un veredicto: es **un tachón encima del que hubiera** | El peor error cuesta dinero, un plazo legal o un visado; **o** hay un dato rojo irreducible | **P08** · **P26** · **P29** · **P25** · **P17** · **P22** |

**Las tres decisiones que hacen que esta rejilla valga y no sea un catálogo disfrazado:**

- **El veredicto 1 va el primero, no al final como advertencia.** «No hace falta IA» es un **destino**, no
  un fracaso. Y el ejemplo canónico es suyo: el presupuesto es aritmética sobre una tabla de precios, y
  meter un modelo de lenguaje ahí **no es ineficiente: es introducir un error posible donde no lo había**.
- **El veredicto 2 tiene nombre propio y casilla propia, y es el que más le va a salir.** No existe en
  ningún curso de IA. Y es **un hallazgo que aportar, no un fracaso**: en una empresa donde lo mal visto es
  no automatizar, llegar diciendo *«esto todavía no se puede automatizar porque nadie sabe cuál es el
  tarifario vigente en alemán»* es trabajo de valor.
- **El agente autónomo NO está en la lista de destinos.** Se define, se explica y se le pone su condición
  de activación en M4, pero no es una opción que ella pueda elegir para una tarea suya, y se dice con todas
  las letras. El motivo es pedagógico y verificable: **el error número uno al clasificar es poner «agente»
  a todo**, porque es la palabra que suena a solución completa y es lo que promete internet. Sacarlo obliga
  a decidir entre lo que sí existe para ella.

### 4.2.1 Dónde se usa: cinco momentos, más de cuarenta juicios

| Momento | Sobre qué | Cuántos juicios | Coste |
|---|---|---|---|
| **M0, día 3** | Los seis descartes automáticos: escribir **el motivo transferible de tres de ellos** y contrastarlos contra la clave del curso | 3 con clave | 10 min |
| **M0, día 3** | **Mapa de los doce, pasada 1**: una letra en las doce filas con más palotes, **sin justificar**, con la tarjeta de definiciones delante | 12 | 20 min |
| **M1, línea de corte** | **Los trozos de su propio proceso**, cada uno con veredicto y motivo | 4–6 | 0 min extra |
| **M1–M7, dobletes** | Ocho procesos que no son el suyo, **con clave sellada** | 8 | 8 × 20 min |
| **M6, semana 14** | **Mapa de los doce, pasada 2**: las mismas doce filas, justificadas con un hecho observable, con la regla del cuatro | 12 | 60 min |
| **M7, semana 17** | **Lectura del delta**: qué veredictos han cambiado y por qué | ~4–6 revisados | 30 min |

**Total: entre cuarenta y cinco y cincuenta juicios sobre procesos reales, en menos de cinco horas
repartidas en dieciocho semanas**, de las cuales **once están contrastadas contra una clave que ella no ha
escrito** (tres motivos de descarte y ocho dobletes). Es más volumen del que produce una arquitectura de
inventario en cuatro semanas de trabajo árido, y se paga en cuotas de veinte minutos.

### 4.2.2 El Mapa de los doce, y por qué son dos pasadas y no una

> **Arbitraje 2, y es el más importante del documento.** A pone la clasificación de doce tareas en la
> semana 1, como **pretest declarado** de veinte minutos y una sola letra por fila, y la repite en la
> semana 17 para leer el delta. B la pone en la semana 14, **justificada**, de sesenta minutos, con la
> regla del cuatro, y argumenta con precisión por qué no puede ir en la semana 3: es trabajo árido en el
> tramo de máxima mortalidad, se hace cuando menos criterio tiene y sin nadie que corrija, y si gobierna
> el orden del curso un error ahí cuesta el curso entero.
>
> **Los dos tienen razón porque están hablando de dos instrumentos distintos con el mismo nombre.** Una
> clasificación de veinte minutos, sin justificar y declarada equivocada de antemano, **no es un
> entregable: es una medida**, y una medida tomada antes de la intervención es exactamente lo que hace
> falta para que el objetivo 4 sea demostrable en vez de afirmado. Una clasificación justificada, con
> hecho observable y con cuota, **es entrenamiento**, y el entrenamiento tiene que ir después del
> criterio porque antes es adivinar.
>
> **Decisión: las dos, y la de A no cuesta nada.** Veinte minutos en la semana 1 con una tarjeta de
> definiciones; sesenta minutos en la semana 14 con el criterio ya adquirido; treinta minutos en la
> semana 17 para leer el delta. Ninguna de las tres facturas que B factura a arq-2 se paga aquí, porque
> la pasada 1 **no gobierna el orden de nada** —para eso está el embudo, que es más barato y más
> observable— y porque está declarada como equivocada.

**Pasada 1 — semana 1, veinte minutos, dentro del embudo.**

1. Sobre los 32 procesos que el curso le entrega ya escritos, marca con un palote los que ha hecho **esta
   semana**.
2. Coge las **doce filas con más palotes**. Esas doce quedan fijadas: son las mismas en las dos pasadas.
3. A cada una le pone **una letra** —1, 2, 3, 4, 5, 6 o ZP— con **la tarjeta de siete casillas** delante.
   **Sin justificar. Sin pensarlo mucho.**
4. Firma y fecha, y **guarda la hoja sin volver a mirarla hasta la semana 14**.

> **LA TARJETA DE SIETE CASILLAS** [J] **— la pieza que hace interpretable el pretest.** En la semana 1
> ella todavía no ha visto la rejilla, que se enseña en M1. Si clasifica sin nada, el pretest mide ruido;
> si se le enseña la rejilla entera en la semana 1, se estropea el módulo donde tiene que aprenderla. La
> solución es intermedia y es la que hace legible el delta: se le entrega **una tarjeta con las siete
> casillas y una línea de definición cada una, sin las pruebas que las deciden**. Así el pretest mide
> **lo que hace con las definiciones**, y el postest mide lo que hace con el criterio. **El delta es
> exactamente lo que el curso ha añadido sobre una definición leída**, que es la pregunta correcta.

Y el material lo enmarca así, que es lo que lo hace funcionar:

> *«Esta clasificación va a estar mal en varios sitios y da igual. No es un entregable: es una medida de
> dónde está hoy tu criterio, tomada antes de que el curso lo toque. En la semana 14 vas a clasificar las
> mismas doce filas otra vez, en serio y con justificación, y en la 17 vas a comparar las dos. La
> diferencia entre las dos columnas es la única prueba objetiva que vas a tener de que este curso te ha
> cambiado la forma de mirar un proceso — y la vas a tener porque hoy has gastado veinte minutos.»*

Coste emocional: cero, porque está declarado que estará mal. Ella lo reconocerá por su nombre: es un
pretest.

**Pasada 2 — semana 14, sesenta minutos, dentro de M6.** Las mismas doce filas, **sin mirar la primera
pasada**, y ahora en serio:

- Cada veredicto se justifica **citando un hecho observable del proceso** —un volumen, un documento, una
  consecuencia— y no una impresión.
- **La regla del cuatro:** al menos cuatro de las doce terminan en **veredicto 1 o veredicto 2**, y **las
  zonas prohibidas no cuentan para los cuatro**.
- Cada uno de esos cuatro lleva su casilla **«lo que sí se puede hacer alrededor»** rellena con un
  artefacto **nombrable**.
- La hoja sale ordenada por `frecuencia × minutos ÷ riesgo`: **es su cola de después del curso**.

> **Arbitraje 6 — por qué las ZP no cuentan para la cuota.** A excluye las zonas prohibidas del recuento;
> B las incluye. Gana A, y el argumento es aritmético: los seis descartes de zona prohibida se resuelven
> **por número de proceso**, sin juicio y sin coste. Si contaran para los cuatro, la cuota se cumpliría
> sola y sería decorativa. Excluyéndolas, **los cuatro tienen que salir de los veredictos 1 y 2, que son
> los únicos que exigen juicio de verdad.** La cuota pasa de ser un trámite a ser un trabajo.

**Lectura del delta — semana 17, treinta minutos, dentro de M7.** Las dos columnas al lado. Por cada
veredicto que ha cambiado, **una frase con el motivo del cambio, elegido de la lista cerrada de cinco**.
Por cada uno que **no** ha cambiado y sobre el que hoy tiene más confianza, **una frase con lo que ahora
sabe que antes no sabía**.

Produce tres cosas de valor distinto: **el delta**, que es el objetivo 4 hecho observable; **la lista de
lo que decidió no automatizar**, que es el entregable de credibilidad de M7 y sale sin trabajo extra; y
**la cola de lo siguiente**, que es lo que hará después del curso.

### 4.2.3 Las comprobaciones de la rejilla, todas binarias

Se aplican **solo a la pasada 2** —la pasada 1 está declarada equivocada, así que comprobarla sería
comprobar dos veces algo que no lo necesita (§12.1, regla 1):

- *¿Cada veredicto cita un hecho observable y no una impresión?* SÍ/NO
- *¿Hay al menos **cuatro** veredictos 1 o 2, **sin contar las zonas prohibidas**?* SÍ/NO
- *¿Algún «no» tiene la casilla «lo que sí alrededor» vacía o con una intención en vez de un artefacto?*
- **La comprobación de las tres filas al azar:** coger tres filas y preguntarse *«¿la hice esta
  semana?»*. Si la respuesta es no en alguna, **la rejilla es aspiracional** y hay que corregirla contra
  lo que de verdad hace. Treinta segundos, y es la que más caza.
- **La señal de fallo que va de frente a por el autoengaño:** *«existe un veredicto 1 o 2 que puse para
  llegar a cuatro, y no porque lo crea.»* Aquí no hay clave posible y depende de su honestidad consigo
  misma. Está reconocido en §17.

---

## 4.3 Instrumento 3 · EL EXPEDIENTE DEL PROCESO

Una carpeta con el nombre de su proceso. **No es documentación: es el sitio donde el proceso vive.** Cada
capa deja dentro exactamente una cosa, y esa lista es el índice del curso.

```
expediente-<mi-proceso>/
  00-como-se-hace-de-verdad.md      ← capa 0: disparador, documentos, decisiones no escritas, salida
  00-hoja-de-sombra.md              ← capa 0: los dos días de observación, en crudo
  00-mapa-de-los-doce.md            ← capa 0: pasada 1, firmada y guardada hasta la semana 14
  01-linea-de-corte.md              ← capa 1: cada trozo con veredicto, motivo y «lo que sí alrededor»
  01-ficha-de-criterio.md           ← capa 1: 4-6 indicadores observables, críticos marcados
  01-casos.md  +  01-CLAVE.md       ← capa 1: la batería, y su clave SELLADA
  02-mapa-de-datos.md               ← capa 2: qué dato entra, en qué paso, dónde se quita y quién
  02-fuentes/                       ← capa 2: cada fuente con FECHA y DUEÑO en la primera línea
  03-disparador.md                  ← capa 3: qué lo lanza, con qué tope, cómo se apaga
  04-frenos.md                      ← capa 4: temas prohibidos, condiciones de parada, quién revisa y a qué hora
  05-evaluacion.md                  ← capa 5: antes, después, coste completo, amenaza no descartada
  06-traspaso.md                    ← capa 6: dueño, caducidades, calendario de revisión, apagado probado
  la-tira.md                        ← la batería pasada en cada capa, una columna fechada
  cuaderno-de-capas.md              ← 8 fichas: cinco preguntas + pregunta fija + doblete
  lista-de-techos.md
  evidencias.md                     ← 3 líneas por capa, para M7
```

**Regla de la primera línea**, que aparece en la capa 2 y no se abandona nunca: todo fichero de
`02-fuentes/` empieza con dos datos, **de cuándo es** y **quién manda sobre él**. Sin eso, un cuaderno con
las condiciones de cancelación del año pasado responde con las del año pasado, **con toda la confianza del
mundo y citando el documento**. La cita no protege de eso; la fecha, sí.

**Por qué una carpeta y no un documento.** Porque el entregable no es un informe: es un sistema con partes
que se tocan por separado y caducan a ritmos distintos. Y porque el día que otra persona lo herede (M6,
M7), **lo que se entrega es esta carpeta y nada más**.

**El Cuaderno de evidencias** (`evidencias.md`): tres líneas al cerrar cada capa, el día que el artefacto
empieza a funcionar. Coste: dos minutos.

```
CAPA __ · fecha ______
- Qué hacía yo antes, y cuántos minutos por unidad:
- Qué hace ahora, y cuántos minutos por unidad:
- Qué NO hace, y qué sigo haciendo yo:
```

Y la tercera línea —*qué NO hace*— es la que después hace creíble todo el dossier: **quien enumera los
límites de su propio sistema se gana el derecho a que le crean el resto.**

---

## 4.4 Instrumento 4 · LA TIRA

Diez casos escritos en M1 y **nunca cambiados**, pasados al cerrar cada capa, con una columna nueva y
**fechada** por capa.

```
CASO                          | como lo hago hoy | +criterio | +fuentes | +disparador | +frenos
                              | 13-oct           | 27-oct    | 10-nov   | 24-nov      | 15-dic
------------------------------|------------------|-----------|----------|-------------|--------
T1  típico, en español        |  SÍ              |   SÍ      |   SÍ     |    SÍ       |   SÍ
T2  típico, en inglés         |  NO              |   SÍ      |   SÍ     |    SÍ       |   SÍ
T3  típico, en neerlandés  ←  |  NO              |   NO      |   SÍ     |    SÍ       |   SÍ
L1  ambiguo: dos categorías   |  inventa         |  inventa  | pregunta |  pregunta   | pregunta
L2  queja educada indirecta ← |  inventa         |  inventa  | inventa  |  pregunta   | pregunta
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
> tarda y cuánta autonomía has cedido.**

Si dentro de tres años le ponen delante una herramienta que hoy no existe, la pregunta que sabrá hacer es
*«¿esto me cambia la calidad o me cambia el disparador?»*. Y no se la habrá contado nadie: la habrá
deducido de cinco columnas de su propio trabajo.

**Tres reglas que la sostienen:**

1. **Los casos se escriben ANTES de construir nada**, y por muestreo cronológico, no elegidos. Si se
   escriben después, se escriben para que pasen. Ella lo reconocerá con su nombre: es preregistro.
2. **La clave va sellada** en un fichero aparte escrito el mismo día, que no se reabre hasta anotar los
   resultados de cada pasada.
3. **Al menos un caso típico y un caso límite están en un idioma minoritario real de su buzón**
   —neerlandés, turco, coreano, polaco—, **nunca en inglés, que es el fácil**.

> **Arbitrajes 9 y 13.** El multilingüe en la batería: A pide un caso de los diez, B pide un típico **y**
> un límite. Gana B: cuesta cero minutos y cierra el hueco por los dos lados, porque un sistema que
> traduce bien lo fácil y se rompe en lo ambiguo **está sin probar**. Y el número de columnas: A propone
> seis, B cinco. Gana B, y el motivo está en §12.1: la Tira es el instrumento con más riesgo de
> convertirse en ritual, y **una pasada menos es una ocasión menos de que se erosione**. Con capas 1, 2, 3
> y 4 más el estado inicial hay exactamente lo que hace falta para leer la curva. En M6 y M7 no se pasa.

**El riesgo de este instrumento, dicho aquí:** es trabajo sin novedad, media hora cada tres semanas, y lo
que no tiene novedad se convierte en ritual o desaparece. **Contramedida: cerrar módulo sin la columna
nueva no está permitido** —es un ítem binario de las puertas de M2→M3 y M3→M4, no un consejo—. Aun así es
el punto frágil que se reconoce en §17.

---

## 4.5 Instrumento 5 · EL CUADERNO DE CAPAS — el extractor de criterio

Un fichero, **ocho entradas de una cara**. Cada entrada tiene tres bloques.

```
CAPA __ · fecha ____

A · LAS CINCO PREGUNTAS       (las cinco filas, y marca cuál ha cambiado respecto a la capa anterior)

B · LA PREGUNTA FIJA          (seis casillas, todas obligatorias)
   1 PROCESO      Vale para cualquier proceso la parte de: __________
                  Era de ESTE proceso la parte de: __________
   2 HERRAMIENTA  Valdría con cualquier herramienta la parte de: __________
                  Era de ESTA herramienta la parte de: __________
   3 TECHO        Esta capa NO PUEDE: __________
                  Lo que lo rompería sería una cosa del tipo: __________
   4 EN MI SEMANA ¿Qué OTRAS tareas mías pedirían esta misma capa? (con su número de proceso)
   5 CUÁNDO NO    La situación en la que esta capa es exceso, y qué usar en su lugar

C · EL DOBLETE                (§9.2: veinte minutos, un proceso ajeno, un veredicto, y la clave después)
```

**La regla de las dos mitades, que es lo que lo hace autocorregible:** cada respuesta del bloque B tiene
una mitad positiva y una negativa, **y las dos son obligatorias**. Si escribe que todo vale para todo, no
ha separado nada: ha resumido. Si escribe que nada vale fuera de aquí, tampoco. La comprobación es binaria
y de cinco segundos.

**Los campos 4 y 5 son el parche más barato contra el monocultivo**, que es el riesgo declarado de esta
columna vertebral: sin ellos, un curso de un solo proceso nunca obliga a conectar la capa con el resto de
su semana. Con ellos, cada capa produce dos o tres candidatos, y esos candidatos alimentan la cola de
después del curso.

**Destino de cada casilla:** la 1 alimenta el doblete · la 2 es el mecanismo de agnosticidad, contestado
ocho veces por escrito · la 3 construye la Lista de techos · la 4 rompe el monocultivo · la 5 es la vacuna
contra el «todo con IA».

**Comprobación mecánica, diez segundos:**
- ¿Están rellenas **las seis** casillas del bloque B? SÍ/NO
- ¿Aparece algún nombre de producto fuera de la línea de techo? SÍ/NO
- ¿El techo dice algo que **la capa no puede hacer**, y no algo que **ella todavía no sabe hacer**? SÍ/NO
  *(es el error más común al escribir un techo, y es el que invalida el instrumento entero como criterio)*
- ¿El campo 4 cita al menos un número de proceso? SÍ/NO
- ¿El doblete tiene veredicto firmado **y** la comparación contra clave anotada? SÍ/NO
- Al cerrar el curso: ¿hay **al menos tres** dobletes terminados en «no aplica», «ni IA» o «arreglar el
  proceso primero»? SÍ/NO

---

## 4.6 Instrumento 6 · LA LISTA DE TECHOS — el catálogo, generado por el propio recorrido

No se lee: **se escribe**, una fila al cerrar cada capa, a partir de la casilla 3 de la pregunta fija.
Tres columnas, y la tercera es la que convierte un catálogo en criterio.

| Lo que esta capa no puede hacer | La clase de cosa que sí podría | **Qué tendría que cambiar para que me tocara** |
|---|---|---|
| Una descripción de un proceso **no hace el trabajo** | Nada: es el punto de partida | — |
| Un criterio escrito **no produce respuestas**; solo permite juzgarlas | Un asistente con ese criterio dentro | Nada: eso es la capa siguiente. *(Fila tachada en la capa 2)* |
| Un asistente guardado recuerda sus instrucciones, **no recuerda lo que pasó ayer** | Un sistema con memoria persistente y auditable | Que necesitara continuidad entre sesiones **y** pudiera comprobar qué recuerda. Hoy no puedo auditarlo, así que no me fío |
| Un disparador por reloj **no reacciona a que haya pasado algo** | Un disparador por suceso | Nada: eso es la capa siguiente. *(Fila tachada en la capa 3)* |
| Mi automatización **no puede actuar sobre recursos que no son míos** | Un permiso delegado, o una plataforma de automatización externa | Que alguien me delegue una etiqueta o carpeta propia dentro del recurso compartido, **o** que el flujo tenga que tocar algo fuera de esta suite |
| Un flujo con juicio **sigue siendo un camino que dibujé yo** | Un agente: le das el objetivo y los límites y decide los pasos | Que aparezca una tarea cuyos pasos no pueda dibujar de antemano **y** que exista un plan que lo incluya **y** que los datos lo permitan. Hoy fallan las tres |
| Medir dice si sirve hoy, **no si seguirá sirviendo cuando cambie el tarifario** | Un calendario de revisión y un dueño | Nada: eso es la capa siguiente. *(Fila tachada en la capa 6)* |
| Nada de lo mío **procesa decenas de ficheros locales de golpe** | Un agente con acceso al sistema de ficheros | Una tarea repetida del tipo «revisar 200 contratos de estancia larga buscando una cláusula» |

**Cuatro propiedades que hacen que esto no muera:**

1. **La tercera columna no caduca.** Un catálogo dice qué hay; esta columna dice **bajo qué condición
   cambiaría su decisión**. «Tocar algo fuera de esta suite» seguirá siendo verdad cuando todo se llame de
   otra manera.
2. **Cada fila se escribe en el momento en que el proceso choca con el techo**, no en un módulo de
   panorama. **La fila del agente se escribe en la capa 4**, cuando ya tiene un sistema con juicio en dos
   puntos y entiende exactamente qué le falta. Antes de eso, «agente» es una palabra; ahí es una carencia
   concreta con nombre.
3. **La escribe ella.**
4. **Tachar una fila es un ejercicio.** Cuando la capa siguiente rompe el techo anterior, se tacha con
   fecha. La lista se lee al final como el registro de por dónde ha ido subiendo, y **eso es exactamente el
   objetivo 1 del perfil servido sin catálogo muerto.**


---

# 5. EL PROYECTO HILO

## 5.1 Qué es y qué no es

**Es un proceso real de su puesto**, elegido en la semana 1 con un filtro observable, y llevado durante
dieciocho semanas hasta que funciona, hasta que lo usa a diario sin que el curso se lo pida y hasta que
otra persona lo usa una semana sin ella.

**No es un ejercicio.** El trabajo del curso es trabajo del puesto. Eso no es una comodidad: es la
contramedida estructural a la primera causa documentada de abandono —21 de 34 abandonos mencionan el
tiempo [E]—. Y por eso **el material declara en cada sesión si es tiempo propio o tiempo de trabajo**: sin
esa distinción escrita, ella lo contabilizará todo como tiempo propio y el curso parecerá el doble de caro
de lo que es.

**No es el proceso que más le duele.** El más doloroso es el más complejo y el más arriesgado: en su
puesto es el matching de alojamiento (P17) o la hoja de camas (P22), es decir, categorías especiales del
RGPD y riesgo crítico de overbooking. **El proceso más doloroso es el segundo proyecto, y eso va escrito
en la semana 1** para que la renuncia no se lea como una limitación del curso.

**Y la objeción hay que mirarla de frente: se le pide comprometerse en la semana 1, que es cuando menos
criterio tiene.** La respuesta no es motivacional, es estructural: **el riesgo del ángulo se concentra en
las cuatro primeras semanas y se hace barato justo mientras es probable** (§5.5).

## 5.2 El embudo de elección — noventa minutos, días 2 y 3

| Paso | Duración | Tipo | Qué hace | Por qué así |
|---|---|---|---|---|
| 1 | 20 min | trabajo | Recibe **los 32 procesos ya escritos**. Tacha los que en su academia no ocurren o no lleva ella; corrige volúmenes; añade lo que falte; marca con palote los de **esta semana** | **Reconocer es mucho más barato que recordar.** Una hoja en blanco delante de alguien cansado produce ocho filas y abandono; una lista de 32 para corregir produce veinticinco filas en veinte minutos. Y **cada tachadura es verificación del dominio contra su realidad** |
| 2 | 20 min | propio | **Mapa de los doce, pasada 1** (§4.2.2) | Es un pretest, no un entregable |
| 3 | 10 min | trabajo | **Descarte de los seis, por número y sin pensar:** fuera P08, P17, P22, P25, P26, P29. Y después, **escribir el motivo transferible de tres de ellos** eligiéndolo de la lista cerrada de cinco, y abrir la clave | Ver la caja de abajo |
| 4 | 5 min | trabajo | **Regla estacional:** *«si no lo hago en enero, no vale»* | Protege contra montar el curso sobre julio y practicarlo en temporada baja: su volumen se multiplica por tres entre febrero y julio |
| 5 | 20 min | trabajo | Puntúa los 6–8 supervivientes en **cinco columnas observables** | Ninguna columna admite «depende» |
| 6 | 40 min en 2 días | trabajo | **La prueba de la sombra** (§5.3) | Es donde se cae la elección equivocada |
| 7 | 10 min | propio | Nombra el **proceso de repuesto** y firma la fecha | El repuesto existe desde el día 3, no desde la crisis |

> **Arbitraje 12 — el descarte de los seis** [J]. A lo hace **por número de proceso**, sin criterio: *«es
> aritmética, no criterio»*, y para la semana 1 eso es exactamente lo correcto, porque un descarte que no
> depende de que ella escriba nada es un descarte que no puede salir mal. B lo hace **escribiendo el motivo
> transferible de los seis**, y también tiene razón: un descarte por número no enseña nada, y son seis
> juicios gratis en el momento en que más falta hace tener algo que contrastar.
>
> **Decisión: las dos operaciones, en este orden y con este reparto.** El **descarte es automático y por
> número** —eso es lo que protege la supervivencia de la semana 1 y lo que garantiza que los seis
> procesos peligrosos salgan sí o sí—. Y **después**, en diez minutos, escribe el motivo de **tres de los
> seis** —no de los seis— eligiéndolo de la lista cerrada, y **abre la clave del curso para
> contrastarlos**. Tres y no seis porque el rendimiento marginal del cuarto es bajo y el coste emocional
> de la semana 1 no lo es. Y **con clave**, porque un motivo escrito sin oráculo es una frase; con
> oráculo es la primera calibración del curso, y llega en el día 3.

**Las cinco columnas del paso 5, y las cinco son observables:**

| Columna | +2 | 0 | −3 (descalifica) |
|---|---|---|---|
| ¿Cuántas veces esta semana? | 5 o más | 1–4 | 0 |
| Datos que toca (semáforo) | solo verde | ámbar seudonimizable | **rojo irreducible** |
| Consecuencia del peor error | interna, se arregla | molesta a un cliente | **dinero, plazo legal o visado** |
| **¿Sobre qué puedo actuar yo?** — *¿sobre qué recursos puedo actuar yo, no mirar, sin pedirle permiso a nadie?* | **son míos** | **una copia mía sirve** | **solo existen en un recurso compartido** ⓘ |
| ¿Sé cómo se hace bien? | perfectamente | más o menos | depende de otra persona |

**+1 de desempate: si el proceso ocurre en tres o más idiomas.** Es un desempate, no un requisito: si el
hilo lo tiene, la lección multilingüe de M2 y M4 cae sobre material suyo en vez de sobre el expediente
modelo.

> **ⓘ Arbitraje 10 — la cuarta columna.** Es la mejor decisión de diseño del corpus y el juez 3 pedía
> explícitamente **no** injertarla, porque en su formulación original —*«los ficheros que abro, ¿son míos
> o compartidos?»*, con su −3— codifica un límite concreto de un producto de 2026 dentro de la mitad de
> criterio del curso, en la decisión número uno de la semana 1. **A y B coinciden en que tiene razón en el
> diagnóstico y se equivoca en el remedio, y las dos la parten por la misma costura.** Se toma **la
> formulación de B**, que es mejor: *«¿sobre qué recursos puedo actuar yo, no mirar, sin pedirle permiso a
> nadie?»* — que es **la pregunta 4 de las cinco preguntas aplicada a su propia cuenta**, es durable, no
> menciona ningún producto y, de paso, hace que la primera vez que use el instrumento número uno del curso
> lo use **sobre sí misma**. Y se toma **el reparto de A**: el límite concreto de hoy —la automatización
> nativa de su entorno falla con unidades compartidas, carpetas compartidas y hojas con referencias
> externas [V]— y el −3 que hoy aplica viven **fechados en `comun/datos-volatiles.md`**. Si mañana esa
> restricción desaparece, se cambia un fichero y la columna sigue siendo correcta.
>
> **Por qué esta columna es la aportación de diseño más rentable del curso:** el centro de gravedad de su
> puesto son los buzones `info@` y `accommodation@` y una hoja de camas compartida. En las otras
> arquitecturas ese límite aparece en la semana 9 y se gestiona como mala noticia; una de ellas confiesa
> por escrito que no lo ha resuelto. Aquí entra en el criterio de elección de la semana 1 y **se cobra
> antes de que haya nada construido encima**. La diferencia entre «he elegido un proceso que no encaja»
> (semana 1, cuesta dos horas) y «esta herramienta no sirve para mi trabajo» (semana 9, atribución
> irreversible) es la diferencia entre seguir y abandonar.

## 5.3 La prueba de la sombra — dos días laborables, tres minutos al día

Antes de comprometerse, durante dos días, **cada vez que ejecuta el proceso candidato anota tres cosas**:
cuántos minutos ha tardado · qué documento ha abierto · **qué decisión ha tomado que no estaba escrita en
ninguna parte**.

**Tres criterios de rechazo, ninguno de opinión:**

| Lo que ve en la hoja | Qué significa | Veredicto |
|---|---|---|
| **En dos días no lo ha ejecutado ni una vez** | No es tan frecuente como cree. La frecuencia percibida y la real no coinciden casi nunca | **Descartado.** Pasa al siguiente |
| **No ha abierto ningún documento** | No hay contexto que dar: es juicio puro. Un asistente con fuentes no tiene qué morder | **Descartado.** Ese proceso es «chat, mejor usado» (veredicto 3) y ahí se queda |
| **Las decisiones no escritas son cada vez distintas** | No es un proceso: es una serie de casos | **Descartado**, o se acota al trozo que sí se repite |

**No cuesta tiempo extra: se hace mientras trabaja.** Y la hoja de sombra es ya la primera versión de la
descripción de la capa 0, más **la línea base** que M5 va a necesitar —medida **antes** de construir nada,
que es lo que la hace honesta—.

> **Nota metodológica que va en el material, porque es su casa.** Esto es **muestreo de eventos, no
> introspección**. *La gente describe sus procedimientos como cree que deberían ser, no como los ejecuta*,
> y los atajos y excepciones —que son justo lo que rompe una automatización— no se verbalizan
> espontáneamente. Por eso no se pregunta: se observa. Y por eso el tercer campo es el que más rinde: **es
> el inventario de todo lo que un sistema no sabría hacer.**

**El hallazgo prometido a las 48 horas.** El material predice por escrito lo que la observación va a
revelar, para que los dos días de peaje sean pago:

> *«En estos dos días vas a descubrir dos cosas incómodas. La primera: que este proceso lo haces menos
> veces de las que crees, o bastantes más. La segunda: que has tomado tres o cuatro decisiones que no
> están escritas en ningún sitio de la academia y que solo sabes tú. Eso no es un fallo del ejercicio: es
> el activo del curso. Es lo que ninguna herramienta puede darte hecho, y es la razón por la que este
> curso lo puedes hacer tú y no un informático. Anótalo como el primer hallazgo, en el Cuaderno de
> evidencias.»*

Sin esta caja, los dos días de sombra son un peaje dentro del tramo de máxima mortalidad. Con ella, son un
pago.

## 5.4 La regla del embudo vacío — el hueco que ninguna arquitectura cubría

Exigir ≥5 ejecuciones semanales, solo datos verdes, actuación sobre recursos propios y «sé hacerlo
perfectamente» **puede descartar casi todo lo que ella hace**, porque casi todo su stack —buzón, hoja de
camas, Excel maestro, mensajería, carpeta de plantillas— es compartido.

> **Si el día 3 no sobreviven al menos dos candidatos, no es un fallo del embudo ni tuyo: es un hallazgo,
> y tiene salidas escritas. Se resuelve el día 3, no la semana 6.**

**La escalera de relajación, en este orden y con el precio declarado en cada paso** *(formulación de B,
plazo de A)*:

| Orden | Qué se relaja | Qué se paga a cambio |
|---|---|---|
| 1 | **Pedir delegación.** Un mensaje de dos líneas a quien administre el buzón: *«¿me podéis dar una etiqueta (o una carpeta) propia dentro de `info@` sobre la que yo pueda actuar?»* | **Depende de otra persona**, que es exactamente lo que el diseño prometía no necesitar. Por eso es el paso 1 pero va por el camino alternativo: se pide y se sigue sin esperar |
| 2 | La cuarta columna acepta **«una copia mía sirve»** como suficiente (0, no −3) | Se abre una fila en la línea de corte: *«mantener la copia al día son N minutos por semana»*, **y ese coste se resta en M5**. El coste no desaparece: se hace visible |
| 3 | La frecuencia baja de **≥5 por semana a ≥1 por semana**, si el proceso tarda más de 15 minutos por ejecución | La Tira tendrá menos pasadas reales. Se compensa pasando la batería también sobre casos históricos |
| 4 | Se **parte un proceso grande** y se toma el trozo que sí califica | Ninguno real: **la línea de corte de M1 iba a partirlo de todos modos**, y un trozo con criterio, fuentes, disparador y frenos es un sistema completo aunque sea pequeño |
| 5 | Se adopta **P27** (análisis de las respuestas de la encuesta de satisfacción) | Es el expediente modelo: **pierde el efecto sorpresa de algunas claves selladas**, y a cambio gana el mejor primer proyecto que existe en su lista |

**Y lo que NO se relaja nunca, en ninguna circunstancia:** la columna de datos —un rojo irreducible sigue
descalificando— y la columna de consecuencia —dinero, plazo legal o visado sigue descalificando—. **Esas
dos no son de comodidad: son la razón de existir del filtro.**

## 5.5 El repuesto y el divorcio preautorizado, con la aritmética escrita

**El repuesto se nombra el día 3, no el día de la crisis.** Es el segundo de la lista puntuada, y se firma
con fecha. Nombrar un plan B cuando ya se ha dudado se lee como excusa; nombrarlo en la semana 1 se lee
como plan.

**Al final de M1 hay un checkpoint de divorcio**, y lo que hace que no sea un consuelo sino una salvaguarda
es el número:

> Al final de M1 lo único construido son cuatro documentos: la descripción del proceso, la línea de corte,
> la ficha de criterio y la batería de diez casos. **Rehacer las cuatro cosas sobre el proceso de repuesto
> son aproximadamente dos horas**, porque el método ya lo sabes y lo único que cambia es el contenido. A
> partir de M2 el divorcio ya cuesta caro. **Por eso el checkpoint está exactamente ahí y no después.**

## 5.6 El expediente modelo — P27, y qué papel juega exactamente

El curso trae el recorrido completo **ya hecho** sobre **P27, el análisis de las respuestas de la encuesta
de satisfacción**: las ocho capas, con sus artefactos, sus fallos típicos y sus **claves selladas**.

**Por qué P27 y no otro.** Cuatro análisis independientes convergen: riesgo **bajo** (no hay dinero, no hay
plazo legal, no lo ve ningún cliente); volumen **alto** (600–800 respuestas al año); es el proceso **más
multilingüe** de su lista (10+ idiomas); **hoy no lo hace nadie** porque nadie tiene tiempo, así que no
compite con ningún procedimiento establecido ni se lo quita a nadie; y es el que **más solapa con su
formación** (análisis de contenido, libro de códigos, estilos de respuesta culturales). Que el proyecto más
útil sea también el más seguro es un regalo del dominio.

**Cuatro funciones, y no una quinta:**
1. **Ejemplo trabajado con desvanecimiento:** en M0 va entero, en M4 le faltan los dos últimos pasos, en
   M6 solo trae la lista de comprobación de la rúbrica.
2. **Fuente de los tres cebos** y de las claves selladas de los ocho dobletes.
3. **Proceso de repuesto por defecto** (§5.4, paso 5).
4. **El material de la tarde de P27** (§6.4), que es la única parte que ella **ejecuta**.

**No es un segundo hilo.** Se lee y se usa como clave; no se hace. Con dos horas propias por semana, dos
procesos son dos procesos a medias, que es exactamente lo que esta columna vertebral existe para evitar.
La excepción es de noventa minutos y está declarada.

---

# 6. MAPA COMPLETO DE MÓDULOS

**Ocho módulos, 18 semanas, 2 h propias por semana** más el trabajo que es trabajo del puesto.
**Arranque en octubre**: el pico de junio–septiembre (250–400 correos/día, 60–90 matrículas/semana) mata
cualquier calendario que lo ignore, y noviembre–febrero es su temporada baja.

**Estructura fija de módulo, y no se toca:** 3 sesiones núcleo de 35–45 min de tiempo propio · 1 bloque de
proyecto de 60–90 min **en horario de trabajo** · el cierre de capa (cinco preguntas + pregunta fija +
doblete + la columna nueva de la Tira cuando toca), **40 min**.

> **Arbitraje 1 — la duración.** A comprime a **17 semanas y 7 módulos** fundiendo «medir» y «dejarlo
> vivo» en un solo módulo de tres semanas, con el argumento correcto de que la meseta baja de siete
> semanas a seis y desaparece una frontera de módulo, que es un sitio menos donde el curso puede leerse
> como terminado. B mantiene **18 semanas y 8 módulos**.
>
> **Gana B, por tres razones y una confesión.** (1) La fusión hace que el módulo **más denso y menos
> gratificante** del curso sea también **el más largo**, justo en la meseta: tres semanas seguidas de
> metodología y mantenimiento sin funcionalidad nueva es peor que dos más dos con una frontera en medio.
> (2) A tuvo que empujar la reproducción del número al módulo siguiente «para que quepa», que es el
> síntoma clásico de un módulo sobrecargado. (3) B mete **la rejilla de los doce dentro de M6**, es decir,
> pone **un hallazgo dentro de la meseta** en vez de acortarla: eso ataca el mismo problema por el lado
> correcto, porque lo que mata en la semana 14 no es que haya una frontera de módulo, es que no pasa nada
> interesante. Y la confesión: **la propia autocrítica 4 de A dice que la fusión es «la decisión con menos
> respaldo de todo el documento» y señala la costura por si hay que soltarla.** Se suelta.
>
> **Pero el argumento de A no se tira: se paga por otra vía.** La meseta se acorta subjetivamente con las
> siete piezas del momento 3 (§13), con la frontera declarada en M4 y con el hallazgo de P32 y la rejilla
> colocados en M6.

**Una frontera declarada desde la semana 1, y esto es diseño anti-abandono, no una rebaja:**

> **Al terminar M4 (semana 11) ya hay curso:** un proceso suyo funcionando, en uso, con frenos probados y
> apagado probado. **M5, M6 y M7 son donde se cobran los objetivos 4 y 5** —criterio portátil y
> evangelización— y son la parte que más rinde a doce meses vista. Decirlo así, y no fingir que las
> dieciocho semanas son un bloque indivisible, es lo que evita que la semana 12 se lea como fracaso.

## 6.0 Vista de conjunto

| M | Sem. | Capa | Qué sale del expediente | Escalón del perfil | Corrección dominante | Frontera |
|---|---|---|---|---|---|---|
| **M0** | 1–2 | 0 · Ver el proceso | Elección puntuada · sombra · descripción real · ficha del entorno · Mapa pasada 1 · **dos victorias** | 1 · chat | Cronómetro · tres rechazos observables · la pantalla | **PUERTA** (2 condiciones) |
| **M1** | 3–4 | 1 · Criterio y línea de corte | Línea de corte con los 6 veredictos · ficha de criterio · anclas · batería sellada · Tira 1–2 | 1 · chat | La muestra apartada · Ctrl+F · **cebo 1** | Lista de cierre + **checkpoint de divorcio** |
| **M2** | 5–6 | 2 · Contexto con procedencia | Mapa de datos · fuentes fechadas · asistente que cita y se abstiene · traslado · Tira 3 | 1 · chat | Batería col. 3 · lista binaria · prueba de la compañera | **PUERTA** (uso espontáneo ≥5) |
| **M3** | 7–8 | 3 · Disparador y lote | Disparador · tope · apagado probado · **la tarde de P27** · notación neutra · Tira 4 | 2 · automatización | Se dispara o no · el sexto que NO debe disparar · tabla de confusión | **PUERTA** (ha visto fallar algo) |
| **M4** | 9–11 | 4 · Juicio y frenos | Puntos de juicio · temas prohibidos · 6 paradas · revisor con nombre y hora · plan de fallo · 5 preguntas sobre herramienta ajena · Tira 5 | 3 · agentes | Cinco paradas + el sexto que no para · rúbrica negativa · **cebo 2** | **PUERTA** · **FRONTERA: aquí ya hay curso** |
| **M5** | 12–13 | 5 · Medir | Evaluación de media página · prueba ciega · cadena causal · lectura de la Tira | transversal | **La prueba ciega barajada por un tercero** | Lista de cierre |
| **M6** | 14–15 | 6 · Sobrevivir sin ti | Ficha de traspaso · calendario · rúbrica propia validada · **Mapa pasada 2** · prueba del hueco lanzada | transversal | Su rúbrica contra el **cebo 3** | Lista de cierre |
| **M7** | 16–18 | 7 · Que lo adopten | Dossier · demo · **la semana sin ella** · delta del Mapa · entrevista ajena · lista de noes | **adicional** | **El piloto**, con ≥2 arreglos | — |
| — | — | apéndice | *(lectura opcional, sin entregable)* | 4 · opcional | ninguna | — |

**Herramientas nuevas en 18 semanas: dos o tres**, según lo que su proceso pida, y ninguna antes de que el
proceso se haya quedado corto sin ella. **Coste: cero euros.** Si el curso acaba costando dinero, el
diagnóstico estaba mal.

## 6.0.1 La regla del orden de sacrificio [J] — la respuesta operativa a «cuánto rigor sin perderla»

Ningún plan de dos horas semanales sobrevive intacto a una jornada completa en una academia. **Un curso
que no dice qué se cae primero deja que se caiga lo importante**, porque en una semana mala se abandona lo
que cuesta más, y lo que cuesta más suele ser lo que más enseña.

> **Cada módulo declara, por escrito y antes de empezarlo, tres cosas:**
> **(a) el núcleo que no se cae nunca** — sin eso el módulo no ha ocurrido;
> **(b) el orden en que se cae lo demás**, con la semana concreta a la que se aplaza;
> **(c) la versión reducida de cada pieza aplazable** — no «hazlo cuando puedas», sino «hazlo con tres
> frases en vez de con seis».
>
> **Y la regla que lo hace funcionar: «caerse» significa aplazarse a una semana nombrada, no desaparecer.**
> Una pieza sin fecha de reentrada no se aplaza: se pierde.

Los dos módulos donde esto decide si sigue o no son M0 y M1, y ahí va escrito en la primera página.

---

## 6.1 M0 · Capa 0 — Ver el proceso, y elegir cuál · semanas 1–2

**Cambios mentales.** Tres, y el tercero es el que más cuesta.
*«Lo primero no es la IA: es mirar qué hago realmente.»*
*«Lo que creo que hago y lo que hago no son lo mismo, y la diferencia es exactamente lo que rompería una
automatización.»*
*«El mismo texto en la misma pantalla es seguro o inseguro según con qué cuenta haya entrado.»*

### La semana 1, día a día, con el tiempo declarado

| Día | Qué | Min. | Tipo |
|---|---|---|---|
| **1** | **La primera victoria, a prueba de fallo.** Instrucciones permanentes guardadas —quién es, dónde trabaja, en qué idiomas escribe, qué tono usa, qué no debe hacer nunca— y usadas **hoy** sobre un correo real pendiente. Cronometrado antes y después | 25 | propio |
| **2** | **La ficha del entorno**, ocho casillas, con los mensajes literales para copiar y pegar **y las comprobaciones empíricas por si nadie contesta** | 25 | propio |
| **2–3** | **La hoja de sombra** | 3/día | trabajo |
| **3** | **El embudo** (§5.2), pasos 1 y 3–5 | 55 | trabajo |
| **3** | **Mapa de los doce, pasada 1** | 20 | propio |
| **4** | **El asistente v1 que cita**, con tres fuentes verdes, **y su batería sellada de diez preguntas escritas antes** | 30 | propio |
| **5** | **El proceso de repuesto**, nombrado y firmado | 10 | propio |

**Semana 1: 1 h 50 de tiempo propio.** Semana 2: la descripción `00-como-se-hace-de-verdad.md` (30 min),
la tarjeta del lunes impresa (5 min), el cierre de la capa 0 con el doblete de P29 (40 min) y **PC-1**
(10 min) — **1 h 25**. **M0 completo: ~3 h 15 de tiempo propio en dos semanas.**

> **Arbitraje 4 — cuándo entra el asistente que cita.** Es el mejor premio del día 1 de las tres
> arquitecturas —un asistente con tarifario, calendario y condiciones vigentes que contesta las seis
> preguntas que repite el 70–80 % de sus leads **diciendo de qué documento sale cada dato**— y también **la
> apuesta más frágil**: exige encontrar la superficie de asistentes, adjuntar ficheros y conseguir que cite,
> por alguien que nunca ha abierto una terminal. A lo escalona al **día 4–5**, detrás del embudo. B lo pone
> el **día 3**, detrás del diagnóstico del entorno, y su argumento es mejor que el de A: **es el diagnóstico
> lo que decide si esa caja va a funcionar**, no el embudo.
>
> **Decisión: el día de A con la razón de B.** Va el **día 4**, detrás del diagnóstico del entorno (día 2)
> **y** del embudo (día 3). El día 3 ya carga 75 minutos entre embudo y Mapa; añadir ahí la pieza frágil
> del módulo es exactamente lo que no hay que hacer en la semana de máxima mortalidad. El premio grande
> sigue llegando dentro de la primera semana, y llega **con dos redes debajo**: una victoria del día 1 y un
> diagnóstico que ya le dice si su edición lo incluye. Si falla, el fallo es información —*«mi plan no lo
> tiene»*— y no un veredicto.
>
> **Y qué repara este injerto:** sin él, no hay ningún artefacto real hasta la semana 5, y las semanas 3–4
> —que son documentación pura, el módulo más ligero en clics de todo el curso— transcurren en seco justo
> después de la luna de miel. Con él, **M1 empieza pasando la batería contra el asistente v1 y viendo que
> saca 4 de 10**: la ficha de criterio nace como respuesta a un fallo observado en algo suyo, no como
> deberes previos. Y M2 no repite el asistente: **lo repara**.

### Contenidos

1. Las cinco preguntas, presentadas y aplicadas por primera vez **a su chat de hoy**.
2. Muestreo de eventos frente a introspección: por qué un proceso se observa y no se recuerda.
3. **Las cuatro preguntas que definen cualquier plan de cualquier proveedor en cualquier año** —*¿entrenan
   con lo que escribo? ¿cuánto lo guardan y quién decide? ¿dónde se procesa? ¿hay contrato de encargado del
   tratamiento?*— más la quinta, que suele decidir de verdad: *¿alguien lo ha configurado y ha dejado dicho
   por escrito qué se puede meter?* Es el ejemplo más limpio del curso de criterio frente a clic, y va el
   primero a propósito.
4. El semáforo verde/ámbar/rojo y la línea entre cuenta personal y cuenta de empresa.
5. **La tarjeta de siete casillas** (§4.2.2) y los cinco motivos transferibles.

### Capacidad que entrena

**Mirar un proceso y describirlo como es.** Es la más portátil del curso y la que ella pide con el nombre
de «criterio portátil». Se enseña transferible por construcción: **se describe por observación y no por
introspección**, con tres campos y dos días. Ese método vale para cualquier proceso, de cualquier empresa,
en cualquier año, y no menciona ninguna tecnología.

### Cómo se autocorrige

- **Ejecución real y cronómetro.** El correo del día 1 salió mejor y en menos tiempo, o no.
- **Los tres criterios de rechazo de la sombra.** No hay nada que valorar: se mira la hoja.
- **La comprobación que más caza, y cuesta un minuto:** *¿tu descripción contiene al menos dos decisiones
  que no estaban en tu idea previa del proceso?* Si no las contiene, la escribiste de memoria y hay que
  volver a observar. **Es la única forma sin mentor de detectar el error más caro de la capa.**
- **La batería sellada de diez preguntas del asistente v1**, escritas **antes** de montarlo.
- **La pantalla corrige el plan.** Las comprobaciones empíricas se corrigen solas, y enseñan de paso lo que
  necesitará cuando el material envejezca: **la documentación dice una cosa y la instancia dice otra, y
  manda la instancia.**
- **El estándar de suspenso de la ficha del entorno, que es brutal y muy útil:** *si en algún punto has
  escrito «creo que», «supongo que» o «me suena que», está mal resuelto.* **«No lo sé y lo pregunté el día
  14» sí vale.** Distinguir lo que sabes de lo que supones es el mismo estándar que va a necesitar para
  evaluar respuestas de una IA, y por eso va el primero.

> **Nota de deduplicación** (§12.1, regla 1): la ficha del entorno **son** ocho casillas; poner encima una
> rúbrica de ocho ítems sería comprobar dos veces lo mismo. La ficha se corrige con **un solo criterio**,
> el de arriba, y con las comprobaciones empíricas. Y la comprobación de las tres filas al azar **no** se
> aplica al Mapa pasada 1, porque el pretest está declarado equivocado de antemano: se aplica en M6.

### Doblete · P29, emergencias 24 h · 20 min

Aplicar la capa 0 a un proceso que **no se va a delegar nunca**. **Clave: ZP.** Y sin embargo describirlo
sirve —para tener el protocolo escrito— **pero no para entregarlo**. Enseña que **mapear un proceso no
compromete a automatizarlo**, que es justo el reflejo que hay que romper en la semana 2.

### Orden de sacrificio de M0

- **Núcleo que no se cae nunca:** la hoja de sombra de dos días · el embudo con sus cinco columnas · el
  repuesto firmado. Sin las tres, el curso no tiene sobre qué construirse.
- **Se cae primero:** la ficha del entorno completa → versión reducida de **dos casillas** (retención y
  política escrita), y las otras seis se completan en la semana 5, antes de PC-2, que es cuando de verdad
  hacen falta.
- **Se cae segundo:** el asistente v1 → se aplaza al **día 1 de la semana 3**, y M1 empieza pasándole la
  batería igualmente.
- **No se aplaza nunca el Mapa pasada 1**, porque una medida que se toma tarde no es una medida: son 20
  minutos y su valor entero depende de la fecha.

### PUERTA M0 → M1 — bloquea, con dos condiciones y no cinco

- [ ] **La hoja de sombra tiene dos días y ninguno de los tres criterios de rechazo se ha activado** (o se
      ha activado y se ha cambiado de candidato).
- [ ] **`00-como-se-hace-de-verdad.md` contiene al menos dos decisiones no previstas.**

Lo demás —ficha del entorno, repuesto, línea base— se firma en la lista de cierre pero **no bloquea**,
porque *«pregunté a X el día D y no obtuve respuesta»* es un resultado válido y porque ninguna de esas
piezas se corrompe si llega una semana tarde.

> **Por qué esta puerta existe pese a estar en el tramo de máxima mortalidad, y por qué son dos
> condiciones.** A no pone puerta aquí; B pone cinco condiciones. La sombra es **el corrector más barato
> del corpus para el error más caro del arranque**, y todo el curso cuelga de la elección del hilo: si
> pasa mal, se descubre en la semana 9 y ya no tiene arreglo. Pero una puerta de cinco condiciones en la
> semana 2 es un muro. **Dos condiciones, las dos observables en treinta segundos, y las dos con el mismo
> arreglo: dos días más de observación.** Y la frase que la acompaña: *«si esta puerta no se abre, no has
> fracasado: tienes dos días más de mirar tu propio trabajo, que es la parte del curso que más rinde.»*

**PC-1 al final de la semana 2.**


---

## 6.2 M1 · Capa 1 — Qué es hacerlo bien, y qué trozos no entrego · semanas 3–4

**Cambios mentales.** Los dos más caros del curso.
*«El cuello de botella no es el prompt: es que nadie ha escrito nunca qué cuenta como respuesta correcta en
esta tarea.»*
Y el segundo, que no tiene que creer por autoridad porque lo deduce de algo que sabe desde tercero de
carrera:

> **Un modelo de lenguaje es el instrumento con la validez aparente más alta y la garantía de validez de
> contenido más baja que vas a manejar en tu vida. Está optimizado para producir texto plausible: la
> plausibilidad es su función objetivo, no un efecto secundario.**

### Qué construye

1. **La línea de corte** (`01-linea-de-corte.md`) — **el entregable más importante del módulo**: el proceso
   **partido en trozos**, y cada trozo con **uno de los seis veredictos**, con el **motivo** de la lista
   cerrada de cinco si se queda con ella, y con **«lo que sí se puede hacer alrededor»** rellenado con un
   **artefacto nombrable**, no con una intención.
2. **La ficha de criterio**: definición en una frase, 4–6 dimensiones, un indicador observable por
   dimensión, críticos marcados, punto de corte. **Una cara.**
3. **Las anclas de tono**: tres frases completas —bajo, medio, alto— para dos dimensiones, **sacadas de
   correos que envió de verdad**. Ese fichero **es** el contexto de tono de la capa 2, no un calentamiento.
4. **La batería de diez casos y su clave sellada**: 5 típicos, 3 límite, 2 de rechazo, sacados **por orden
   cronológico y no elegidos**, con **un típico y un límite en idioma minoritario real**, y cerrados antes
   de escribir una línea de instrucción.
5. **La Tira, columnas 1 y 2.** La sesión 1 del módulo empieza **pasando la batería contra el asistente v1
   y viendo que saca 4 de 10**.

> **Por qué los seis veredictos entran aquí y dentro del proceso, y no en un módulo de panorama.** Aplicar
> la rejilla **a los trozos de su propio proceso** es mejor que aplicarla a doce procesos ajenos, por tres
> razones: es donde aparecen de verdad el veredicto 1 —casi todo proceso real tiene un trozo que es
> aritmética— y el veredicto 2 —casi todo proceso real tiene un trozo cuya fuente de verdad nadie puede
> nombrar—; obliga a **partir el proceso**, que es la operación que ningún principiante hace y la que más
> criterio produce; y **no cuesta ni un minuto extra**, porque la línea de corte existía igual, solo que
> con veredicto libre. Cambiar un veredicto libre por una rejilla cerrada convierte una decisión en una
> **clasificación reutilizable**.

### Los cinco motivos tipificados — la lista cerrada, y se usa en los cuatro sitios

> **Arbitraje 5.** A propone **una lista cerrada de cinco motivos**; B propone tres para la línea de corte
> más un cuarto con nombre propio («no necesita un modelo») más un quinto tratado aparte como mecanismo
> («las reglas son de otro»). **Gana A**, y el motivo es de instrumento, no de contenido: los dos cubren lo
> mismo, pero **B produce dos listas distintas para la misma operación** —una para la línea de corte y otra
> para las zonas prohibidas— y una sola lista usada en cuatro sitios se aprende, mientras que dos listas
> parecidas se confunden. La lista es esta y no cambia en todo el curso:

| Motivo | Qué significa | Ejemplo de su casa |
|---|---|---|
| **Riesgo** | El error lo paga un cliente, una administración o la caja | Cualquier trozo que toque importes, plazos de visado o disponibilidad de alojamiento |
| **Conocimiento que caduca** | La regla cambia más deprisa de lo que se puede mantener el artefacto | Requisitos consulares, que se reordenaron en 2025 y volverán a cambiar |
| **No hay fuente de verdad** | Nadie puede nombrar el documento vigente ni su dueño | El tarifario en alemán, que lleva meses desactualizado y nadie lo sabe |
| **Las reglas son de otro** | El procedimiento, los plazos y la plataforma los fija una institución ajena | La inscripción y las tasas de los exámenes oficiales, que van por la plataforma del Instituto Cervantes, con plazos rígidos que no se recuperan |
| **No necesita un modelo** | Necesita una fórmula, una plantilla, un filtro o un calendario | El presupuesto: aritmética sobre una tabla de precios. **El escalón −1** |

**Se usa en:** la línea de corte (M1) · los tres motivos de descarte con clave (M0) · el veredicto de cada
doblete (M1–M7) · la justificación de la pasada 2 y del delta (M6, M7).

### La columna «lo que sí se puede hacer alrededor»

La línea de corte exige motivo para cada trozo que se queda con ella, pero **sin esta columna no exige
compensación**. Con ella, el módulo **no termina con una lista de renuncias: termina con un sí concreto por
cada no**, y la rúbrica la exige rellena con **un artefacto nombrable**.

| No se puede | Lo que sí, alrededor |
|---|---|
| **P17** matching con familias (salud, religión y potencialmente orientación sexual en una casilla de texto libre) | **P18** confirmación de alojamiento: 700–800 al año, plantilla con diez variables, ningún dato de salud. Y **P20** triaje de incidencias: clasificar y enrutar sí, responder no |
| **P08** redactar la carta de aceptación para visado (normativa viva) | **Una comprobación determinista de consistencia entre los campos que ella ya ha tecleado a mano** —expediente ↔ carta ↔ factura ↔ certificado—, que ataca el mismo mecanismo de error documentado en P04 **sin que el documento de identidad entre en ningún sitio**, y que además es veredicto 1: no necesita ningún modelo |
| **P26** responder una queja formal | **Clasificarla, extraer los hechos comprobables y preparar el expediente** —histórico, fechas y condiciones vigentes **en la fecha de la reserva**— para la persona que sí decide. Redactar, no |
| **P22** decidir la asignación de camas | El **aviso** cuando dos reservas se solapan: es un filtro, es veredicto 1, y no necesita ningún modelo |

> **La corrección obligatoria sobre P08, que A y B aceptan las dos y que este documento hereda entera.**
> Hay una versión tentadora y equivocada del «lo que sí alrededor» de las cartas de visado: *montar la
> comprobación que caza el nombre mal transcrito desde el pasaporte*. **Eso mete un documento de identidad
> en la herramienta, y el pasaporte es rojo absoluto: nunca, en ninguna herramienta, ni imagen ni PDF.** La
> versión admisible es la de la tabla, y **vale doble como material didáctico**: enseña qué es un «lo que
> sí alrededor» y enseña que **una alternativa mal pensada puede ser peor que el «no»**.

### Cómo se autocorrige

- **Mecanismo dominante: la muestra apartada.** Los diez casos se abren al final y **tiene que fallar al
  menos uno**. Si no falla ninguno, **sospecha del muestreo antes que celebrar**: *si tu batería la pasa
  entera a la primera, tu batería es fácil; no es que tu sistema sea bueno.*
- **Y el criterio no se toca.** Si al abrirlos le dan ganas de cambiar la ficha para que aprueben, **lo
  anota y no lo cambia**. Ese impulso es el dato más interesante del ejercicio y tiene nombre: sesgo del
  experimentador.
- **Ctrl+F sobre la ficha de criterio.** Si aparecen «adecuado», «correcto», «natural», «profesional» o «de
  calidad» **sin un ancla detrás**, no ha operacionalizado: ha renombrado el constructo. Cinco segundos.
- **Prueba de tamaño:** la ficha cabe en una cara. Una rúbrica de dos páginas no se usa nunca.
- **Los dos ítems que atacan la calidad sustantiva**, que es lo que ningún filtro mecánico alcanza —y es
  poco, y está reconocido como tal en §17—: *¿hay **al menos un indicador verificable contra una fuente
  externa**? ¿están **todos** marcados como críticos? Si sí, no has priorizado.*
- **Rúbrica de la línea de corte, con tres criterios negativos que deciden el módulo:**
  *(a) si no hay ningún trozo que se quede contigo, está mal resuelto — vuelve;*
  *(b) si el motivo de algún «se queda conmigo» es «es difícil», está mal: los motivos legítimos son los
  cinco de la lista;*
  *(c) si algún trozo con veredicto 1, 2 o ZP tiene la casilla «lo que sí alrededor» vacía o con una
  intención en vez de un artefacto nombrable, está mal.*
- **CEBO 1 (control positivo).** El curso trae una **línea de corte de mentira**, de una academia
  inventada, con **tres defectos plantados y documentados** en un fichero sellado: uno **visible** (un trozo
  con datos rojos marcado como «lo entrego»), uno de **omisión** (falta el trozo de revisión humana antes de
  que algo salga) y uno de **criterio** (un trozo determinista clasificado como veredicto 5 cuando es
  veredicto 1). Ella lo corrige con la rúbrica y **después** abre la hoja de defectos. **Si encuentra 1 o 0,
  ese tipo de trabajo no se corrige con IA en el resto del curso.**
- **El protocolo de corrección con IA, siete reglas**, primera aplicación (§12.4).

### Doblete · P02, presupuestos · 20 min

Escribir su ficha de criterio hace visible que todos los indicadores se cumplen con una fórmula: semanas ×
tipo de curso × alojamiento × suplemento de verano × descuento por volumen. **Clave: veredicto 1, NI IA,
motivo «no necesita un modelo».** Y meter un modelo de lenguaje ahí no es ineficiente: **es introducir un
error posible donde no lo había.** Es el ejemplo canónico del escalón −1.

### Orden de sacrificio de M1

- **Núcleo que no se cae nunca:** la línea de corte con sus veredictos y motivos · la batería de diez casos
  con clave sellada. Todo el resto del curso los usa.
- **Se cae primero:** las anclas de tono → versión reducida de **tres frases en vez de seis** (una dimensión
  en vez de dos), y la segunda dimensión se completa en la semana 5, dentro de M2, que es donde se usan.
- **Se cae segundo:** el **cebo 1** → se aplaza a **la semana 5**, y **PC-3 se mueve con él**, porque PC-3
  es literalmente una conversación sobre el resultado del cebo. Aplazarlos juntos no rompe nada; aplazar
  uno solo desperdicia un punto de consulta.
- **Nunca se recorta la ficha de criterio a menos de cuatro indicadores.** Por debajo de cuatro no es un
  criterio: es una preferencia.

### Lista de cierre M1 → M2 — **no bloquea**

- [ ] La ficha de criterio pasa el Ctrl+F, cabe en una cara y tiene al menos un indicador verificable contra
      fuente externa.
- [ ] La línea de corte pasa sus tres criterios negativos.
- [ ] La batería tiene diez casos, clave sellada, y **un típico y un límite en idioma minoritario**.
- [ ] La Tira tiene dos columnas fechadas.
- [ ] El cebo 1 está pasado y el veredicto sobre la IA correctora está **escrito**.

> **Por qué aquí no hay puerta.** B pone una; A no. La comprobación sustantiva de esta capa **no existe**
> —nadie puede decirle si su ficha de criterio mide lo que importa (§17)— así que una puerta aquí
> bloquearía sobre criterios de forma, que es lo que una puerta no debe hacer. Y hay una razón más fuerte:
> **al final de M1 ya hay un punto de parada, el checkpoint de divorcio.** Dos figuras de parada seguidas
> en el tramo de mortalidad es una de más. Lo que sí caza esta capa cuando está mal es la columna 3 de la
> Tira, dos semanas después, y ahí sí hay puerta.

### Checkpoint de divorcio, al final del módulo (§5.5). **PC-3 al final de la semana 4**, sobre el cebo.

---

## 6.3 M2 · Capa 2 — Que sepa de dónde sale cada dato · semanas 5–6

**Cambio mental.** *«La memoria fiable es un fichero, no una sensación.»* Y la tríada que los principiantes
mezclan siempre: **fuente de verdad** (hechos, desde una sola dirección) ≠ **memoria** (acuerdos que
permanecen) ≠ **procedimiento** (pasos y formato de salida). Confundirlas produce el error más común:
**meter el tarifario dentro de las instrucciones.** Funciona en enero y miente en marzo, porque las
instrucciones no se revisan y los documentos sí.

### Qué construye

1. **El mapa de datos del proceso** (§10.3): cada dato que lo atraviesa, su color, **en qué paso entra** y
   **dónde hay que quitarlo y quién lo quita**. Una cara.
2. **Las fuentes**, con **fecha y dueño en la primera línea de cada una**. Copias, nunca maestros.
3. **El asistente v2**: el v1 del día 4, ahora con el criterio de M1 dentro, con las anclas de tono, con
   fuentes fechadas, que **cita el documento y su fecha**, que **dice «no lo sé»** cuando la respuesta no
   está, y con la instrucción multilingüe explícita: **las fuentes están en español y la respuesta va en el
   idioma de la persona.**
4. **La prueba de portabilidad nº 1** (§8.4).
5. **La Tira, columna 3.**

> **El multilingüismo, y por qué está aquí como contenido y no como suerte.** Es el fallo de encaje más
> serio que el juez 4 le encuentra a esta columna vertebral: la propiedad que define su puesto —P01 en
> 6–12 idiomas, P27 en 10+, la dirección del alojamiento siempre también en español para el taxista,
> *«traducir la queja es media resolución»* en P20, las seis versiones de plantilla que envejecen calladas
> en P32— dependía del proceso que le tocara. Aquí entra en **cuatro sitios, con nombre y sin depender de
> la suerte**:
> 1. **Instrucción de diseño, en la capa 2:** *las fuentes están en español y la respuesta va en el idioma
>    de la persona.* Es una separación de capas —conocimiento frente a presentación— y no una traducción, y
>    por eso es criterio y no truco.
> 2. **Instrumento, en la batería (M1):** un típico **y** un límite en un idioma minoritario real de su
>    buzón, **no en inglés, que es el fácil**. Un sistema que se prueba solo en inglés está sin probar.
> 3. **Ejecución garantizada, en la tarde de P27 (M3):** treinta comentarios reales en diez idiomas,
>    **obligatoria e independiente del hilo elegido**.
> 4. **Freno, en la capa 4:** *parar si el mensaje llega en un idioma que no está entre los que has
>    probado.*

### Capacidad que entrena, y cómo se enseña transferible

**Contexto con procedencia.** Tres piezas, ninguna con nombre de producto:
- **Citar no es un adorno: es lo que hace que revisar cueste cinco segundos en lugar de una
  investigación**, y por eso es lo que hace que la revisión se siga haciendo en julio.
- **«No lo sé» es una respuesta correcta, hay que exigirla explícitamente con fórmula literal y hay que
  probarla a propósito.** Un sistema que nunca dice «no lo sé» no es que lo sepa todo: es que no lo has
  probado bien.
- **Una fuente sin fecha y sin dueño no es una fuente, es un papel.** El dueño es quien puede cambiarla; la
  fecha es lo que te dice si mirarla.

**Y las señas, que son la pieza portátil de este módulo** (§8.2).

### Cómo se autocorrige

- **Mecanismo dominante: la batería, columna 3, con umbral asimétrico.** Falla >0 de los 5 típicos → no
  está listo · se inventa una decisión en alguno de los 3 límite, **aunque acierte** → no está listo ·
  contesta algo distinto de «no lo sé» en alguno de los 2 de rechazo → no está listo. **Una respuesta
  correcta a un caso de rechazo es un suspenso**, porque significa que responde desde fuera de sus fuentes.
- **Lista de comprobación binaria, diez ítems observables:** *¿cada fuente tiene fecha en la primera línea?
  ¿cada fuente tiene un nombre de persona como dueño? ¿he abierto tres documentos citados al azar y he
  encontrado la frase? ¿alguna respuesta cita un documento que no está en las fuentes? ¿hay una frase que
  diga qué hacer cuando falta un dato? ¿he subido el maestro de algo en vez de una copia? ¿hay un precio o
  una fecha escritos dentro de las instrucciones en vez de en una fuente?*
- **La prueba de la compañera**, sobre tres casos seudonimizados: *¿podría [nombre de una compañera
  concreta] saber de quién hablo leyendo esto?* Si sí, sigue quitando. **Y el criterio del otro lado, que
  casi nadie pone:** el texto resultante **tiene que seguir sirviendo**; si la respuesta que produce es
  inservible, ha quitado contexto que no era identificador.
- **La prueba de portabilidad se corrige sola:** o las tres columnas están rellenas con cosas concretas, o
  no. Criterio negativo: *si la columna «qué viajó tal cual» está vacía, no construiste criterio:
  construiste un prompt.* Y el diagnóstico: **si no consigue montarlo en veinte minutos, no aprendió la
  capacidad, aprendió la ruta** — y ese diagnóstico llega a tiempo de corregirlo.
- **PC-2 aquí**, justo antes de cargar fuentes reales.

### Doblete · P08, carta de aceptación para visado · 20 min

**Clave: ZP, motivo «conocimiento que caduca».** Y el motivo transferible es el que hay que saber decir:
*«la normativa de extranjería cambia de un año para otro, y congelar dentro de un artefacto un conocimiento
que caduca es fabricar un error futuro»*. Es el doblete que mejor entrena el criterio portátil, porque **no
metas conocimiento volátil dentro de un artefacto** vale para cualquier dominio.

### Orden de sacrificio de M2

- **Núcleo que no se cae nunca:** las fuentes con fecha y dueño · la regla de «no lo sé» probada · la
  columna 3 de la Tira. Sin las tres, M3 automatiza algo que no está.
- **Se cae primero:** la prueba de portabilidad nº 1 → se aplaza a **la semana 8**, dentro de M3, donde ya
  hay otra prueba de portabilidad y se hacen las dos seguidas.
- **Se cae segundo:** la instrucción multilingüe → nunca se cae del todo, pero puede reducirse a **un solo
  idioma probado**, declarándolo en la lista de frenos de M4 como parada por idioma no probado.
- **El mapa de datos no se aplaza nunca**, porque va delante de cargar fuentes reales y después sería tarde.

### PUERTA M2 → M3 — bloquea. **La más importante del curso**

- [ ] La batería da **5/5 en los típicos**, **pide aclaración** en los 3 límite y dice **«no lo sé»** en los
      2 de rechazo.
- [ ] **Ha usado el asistente al menos cinco veces en una semana SIN que el curso se lo pidiera.**
- [ ] La prueba de portabilidad está hecha y sus tres columnas rellenas.
- [ ] El mapa de datos tiene, en cada fila ámbar o roja, **un paso concreto y una persona** en la columna
      «dónde se quita y quién».

> **Por qué la segunda condición es la más importante que hay escrita en este documento.** No mide si
> aprendió la lección: **mide si el artefacto le sirve**, que es la única cosa que un curso sin profesor no
> puede preguntarle a ella misma y sí puede **contar**. Es una medida conductual, externa a su juicio sobre
> su propio trabajo, que es justo el punto ciego que la literatura sobre autoevaluación describe. Y hay una
> razón de fondo: **la tesis entera de esta columna vertebral —«el mundo la corrige cada martes»— es falsa
> si ella no lo usa.** Con su frase asociada, en negrita en el material: **automatizar algo que no usas es
> multiplicar un error que ni siquiera has visto.**
>
> **Qué hacer si la puerta no se abre**, escrito por delante: no se avanza, **y no es un suspenso: es una
> semana más en la capa 2, y esa semana está presupuestada** (§12.3). Con el diagnóstico de tres preguntas:
> *¿no lo abro porque no me acuerdo* → ponlo donde ya miras*? ¿porque contesta peor que yo* → vuelve a la
> ficha de criterio*? ¿o porque esta tarea en realidad no la hago tanto* → el embudo se equivocó, y ahí
> está el repuesto*?* Las tres tienen salida.

---

## 6.4 M3 · Capa 3 — Que ocurra sin que lo pidas · semanas 7–8

**Cambio mental.** *«Automatizar no es una herramienta nueva: es quitar el dedo del disparador.»* Es el
momento psicológico del curso —la primera vez que algo pasa sin que ella lo pida— y por eso llega en la
semana 7 y no en la 14.

### Qué construye

1. **El disparador** sobre el trozo que la línea de corte marcó como entregable, con su tipo declarado —por
   calendario o por suceso— y su justificación. **Un lunes no es un suceso.**
2. **El tope**: *si la lista supera N, no hagas nada y avísame.* **Un sistema que produce cuarenta
   borradores un lunes de julio no ayuda, entorpece.** El tope no es una precaución: es lo que convierte una
   automatización en algo de lo que te puedes fiar, porque **su comportamiento en el peor día es conocido**.
3. **El apagado, probado de verdad**, no imaginado.
4. **La tarde de P27** (§6.4.1).
5. **La notación neutra y la prueba de portabilidad nº 2** (§8.4).
6. **La Tira, columna 4.**

Y la regla que gobierna la capa entera:

> **Automatiza la lectura y la preparación. La escritura hacia fuera la firma una persona.**
>
> Y la razón, que no es prudencia sino diseño de aprendizaje: **si el artefacto solo prepara, todos sus
> errores son recuperables, y por eso puedes permitirte equivocarte mucho — que es exactamente lo que hace
> falta para aprender.** Etiquetar es reversible; enviar no. Se puede relajar más adelante, proceso a
> proceso y con datos de acierto medidos. **No se relaja por costumbre.**

### La restricción de producción que hace este módulo a prueba de administradores

> **Ningún módulo posterior puede depender de que el constructor de flujos esté habilitado.** M3 tiene
> **dos rutas escritas por delante**:
> - **Ruta A (principal y obligatoria):** un disparador **por reloj dentro del chat que ella ya usa**, que
>   no requiere consola, ni permiso de administrador, ni licencia extra. **Basta para cerrar la capa, para
>   pasar la puerta y para que M4 tenga sobre qué ejercitar los frenos.**
> - **Ruta B (ampliada):** disparador por suceso con la herramienta de automatización de la suite, si el
>   administrador la tiene activada.
>
> Si la B no está disponible, **se pierde comodidad y volumen, no aprendizaje**, y el material lo dice con
> esas palabras: no es un fallo suyo ni del curso.

**Y los límites, por delante y no al tercer intento fallido.** En la primera página del módulo: los flujos
de su entorno **fallan con unidades compartidas, carpetas compartidas y hojas con referencias externas**
[V]; un solo disparador por flujo; tope de etiquetas visibles; el administrador puede tener pasos
desactivados y no hay forma de saberlo hasta intentarlo. **Como la cuarta columna del embudo ya descartó
los procesos que solo viven en recursos compartidos, aquí esto no debería ser una sorpresa sino una
confirmación** — y esa es exactamente la función de haber puesto la restricción en el criterio de elección.

### Cómo se autocorrige

- **Mecanismo dominante: se dispara o no se dispara.** El corrector más fiable que existe, y aquí está
  entero.
- **La prueba de los cinco casos fabricados**, uno por categoría, **y un sexto que NO debe disparar**, que
  es el que casi nadie prueba. Cinco salidas correctas y una no-salida, o no las hay.
- **La prueba del tope:** meterle un lote grande a propósito y comprobar que se detiene y avisa.
- **La prueba de apagado.** Se apaga de verdad y se vuelve a encender. *Un sistema que no sabes apagar no
  está terminado* — y hay una razón práctica además de la obvia: **el día que falle vas a estar nerviosa, y
  no es el momento de averiguar dónde está el interruptor.**
- **Lista de comprobación de plataforma, seis ítems binarios**, escrita como síntomas y reutilizable como
  diagnóstico: *¿el fichero que toca está en un recurso compartido? ¿la hoja usa referencias externas?
  ¿tiene más de un disparador? ¿hay algún paso que escriba hacia fuera? ¿lo he probado con un caso que debe
  NO disparar? ¿sé cómo se apaga y lo he apagado hoy?*
- **La Tira, columna 4**, con la lectura contraintuitiva escrita: *si la calidad ha mejorado respecto a la
  capa 2, sospecha: probablemente reescribiste el criterio por el camino, y eso es mérito tuyo, no del
  disparador.*
- **PC-4, el comodín**, disponible desde aquí.

### Doblete · P30, el parte semanal a dirección académica · 20 min

Determinista puro. **Clave: veredicto 5, y con la mínima IA posible en el camino crítico.** Enseña que
**«automatizar» no significa «meter un modelo»**, que es la confusión más extendida y la que más caro sale.

### Mini-doblete · P16, exámenes oficiales · 10 min

*(pieza que aporta A y que B no tiene; se conserva porque el motivo que enseña no lo cubre ningún otro)*
**Clave: veredicto 5, motivo «las reglas son de otro».** La inscripción, las tasas y los plazos viven en la
plataforma del Instituto Cervantes; los plazos son rígidos y no se recuperan. **El motivo transferible no
es de riesgo ni de datos: es que el proceso es ajeno.** Automatizar la parte que uno controla de un proceso
cuyas reglas pone otro produce un sistema que se rompe el día que el otro cambia algo, sin avisar. Es una
categoría de «no» que va a encontrarse en cualquier empresa.

### Orden de sacrificio de M3

- **Núcleo que no se cae nunca:** el disparador por ruta A, con tope y apagado probado · los seis casos
  (cinco que disparan y uno que no) · **la tarde de P27**.
- **Se cae primero:** la ruta B → no se intenta, y se anota en la Lista de techos.
- **Se cae segundo:** la prueba de portabilidad nº 2 → se aplaza a **la semana 10**, dentro de M4.
- **El mini-doblete de P16 se cae sin coste** y se recupera en M6 si hay hueco.

### PUERTA M3 → M4 — bloquea

- [ ] El disparador ha corrido **al menos una semana entera sobre casos reales**; los cinco casos disparan,
      **el sexto no**, el tope se ha probado y el apagado se ha ejecutado.
- [ ] La tarde de P27 está hecha, con su tabla de confusión y sus dos umbrales.
- [ ] **Ha visto fallar algo y sabe por qué falló.** *Si a estas alturas no ha fallado nada, el material
      trae un fallo provocado: un caso fabricado que el disparador se traga en silencio.*

> **Motivo: sin haber visto un fallo no hay criterio para dar autonomía a nada**, que es exactamente lo que
> pide la capa siguiente. El fallo provocado es **un control positivo aplicado al sistema**, igual que el
> cebo lo es a la correctora.

### 6.4.1 La tarde de P27 — noventa minutos, tiempo de trabajo, dentro de M3

> **Arbitraje 8.** A la hace **obligatoria** y la declara «la única excepción al una-sola-cosa». B mantiene
> P27 como **ruta de respaldo contingente**, que se activa solo si su proceso resulta ser monolingüe o no
> tener clasificación en lote.
>
> **Gana A, y el argumento es duro: un mecanismo contingente no está en el diseño.** Si su proceso incluye
> clasificación en lote, la ruta de respaldo no se ejecuta y ella nunca hace la doble codificación; si no la
> incluye, se ejecuta pero llega como parche. En los dos casos, **el mejor mecanismo de corrección de nivel
> 1 que existe para juzgar la calidad de un clasificador queda a merced de la suerte**, que es exactamente
> lo que el juez 2 señala como el tercer defecto de esta columna vertebral. Noventa minutos, una sola vez,
> con material provisto: el precio es bajísimo y lo que compra es lo más caro del curso.

**Qué es.** Una sesión sobre material que el curso trae ya preparado: **treinta comentarios reales de
encuestas de satisfacción en diez idiomas** y **un libro de códigos cerrado** (5–8 categorías con
definición operativa, criterios de inclusión y exclusión, dos ejemplos prototípicos y **dos ejemplos
frontera con la decisión ya tomada y justificada**).

**Qué hace ella, en este orden:**
1. **Codifica los treinta a mano**, con el libro de códigos delante. Sin ver nada más.
2. **Aplica el mismo libro de códigos a los treinta de golpe** con su asistente, en lote.
3. **Construye la tabla de confusión** entre sus códigos y los del sistema.
4. Escribe **una frase por cada confusión que se repite**.
5. Mira el acuerdo de la **categoría menos frecuente por separado** —si el 60 % son de alojamiento, un
   clasificador que dijera siempre «alojamiento» acertaría el 60 %.
6. **Abre la clave sellada del curso**: la codificación de referencia de los treinta. Compara **sus**
   códigos con la referencia, no solo los del sistema.

**Umbrales, por los dos lados:** ≥26/30 de acuerdo con el sistema · **menos del 15 % en «sin clasificar»**,
y **si cae 0 %, está forzando encajes**.

**Cinco razones por las que existe, todas de reparación:**

1. **Restaura el mejor mecanismo de corrección de nivel 1**, que de otro modo es contingente.
2. **Restaura el oráculo escrito por el curso.** Es el único sitio del curso donde **compara su propio
   juicio contra una clave que ella no ha escrito**, sobre una tarea que ha hecho de verdad. Es la
   calibración que se pierde al renunciar al doble hilo.
3. **Garantiza la práctica multilingüe con independencia del hilo elegido.** Y el fallo típico va
   anunciado: **el sistema clasifica peor en los idiomas que no son inglés**, y los estilos de respuesta
   culturales hacen que un mismo grado de descontento se exprese de forma muy distinta según de dónde venga
   el alumno.
4. **Es la capacidad «una instrucción, N unidades» sin depender de ningún producto.** El artefacto portátil
   no es la implementación: **es el libro de códigos**, y el ejercicio obliga a decirlo — *«nombra dos
   formas distintas de aplicar tu libro de códigos a 600 filas y di qué cambia entre ellas»*. Lo que cambia
   es la comodidad y el volumen; lo que no cambia es la calidad de la clasificación.
5. **Si su hilo se cae más adelante, medio P27 ya está hecho.**

**Y lo que NO es:** no es un segundo hilo. Son noventa minutos una sola vez, con material provisto y clave
sellada. **El curso sigue construyendo una cosa.**


---

## 6.5 M4 · Capa 4 — Juicio donde hace falta, frenos donde hace falta · semanas 9–11

**Tres semanas, no dos.** Es el único módulo al que se le da aire antes del final, y se dice por qué: es la
frontera conceptual del curso, es donde más gente se cae, y es donde una puerta cerrada tiene que poder
costar una semana sin romper el calendario.

**Cambios mentales.** Dos.
*«Un agente no es una automatización mejor: es una automatización que **ha renunciado a ser predecible** a
cambio de poder afrontar casos que no previste. En atención al cliente esa renuncia se paga a conciencia y
solo donde compensa.»* Y la dirección del error que casi nadie enseña: **un agente puede ser exceso.** Si
los pasos son fijos, meterle juicio lo hace más caro, más lento y menos auditable.
Y el segundo: *«el riesgo no es el del día 1, es el del día 60.»* Sesgo de automatización: a la tercera
semana se deja de revisar. **La confianza no es una salvaguarda.**

### Qué construye

1. **El juicio, confinado a dos o tres puntos concretos**, cada uno con su criterio escrito y justificable.
2. **La lista de temas prohibidos** (`04-frenos.md`), en negativo y sin matices: *nunca respondas sobre
   requisitos o plazos de visado; nunca cites importes; nunca confirmes disponibilidad de alojamiento;
   nunca respondas a una queja formal; nunca menciones salud. Si el tema aparece, aunque no use esas
   palabras, escribe SOLO: DERIVAR A PERSONA — motivo: `<tema>`, y para.*
   **Tema prohibido ≠ condición de parada.** Uno dice **de qué** no se habla; el otro dice **cuándo** se
   deja de trabajar aunque el tema estuviera permitido. Las dos hacen falta y se confunden siempre.
3. **Las condiciones de parada, seis, y las seis con motivo:**
   - no encuentro la respuesta en mis fuentes;
   - la persona está enfadada, o menciona abogado, reclamación u hoja de reclamaciones;
   - hay un menor implicado, o se menciona salud;
   - el importe supera X;
   - **el mensaje viene de una agencia y menciona un acuerdo o convenio particular**;
   - **el mensaje llega en un idioma que no está entre los que has probado.**
4. **Parar no es callarse**, y son tres cosas a la vez: no producir la salida · dejar **una marca visible
   donde tú ya miras** · **decir por qué paró, en una línea**. En un buzón de 250–400 correos al día en
   pico, un freno mudo equivale a perder el caso.
5. **El punto de revisión humana, con nombre propio y con hora.** *«<nombre>, antes de las 18:00 del mismo
   día.»* **Un revisor sin plazo no es un revisor.**
6. **El plan para cuando falle**, en cinco pasos: detectar · parar · reparar con la persona (llamada, no
   correo) · corregir el sistema añadiendo ese caso a la batería · y valorar si hay brecha de datos —
   **esto último no lo decide ella [!]**, lo escala el mismo día.
7. **Las cinco preguntas aplicadas a una herramienta que el curso no ha enseñado** (RA4), con sus tres
   comprobaciones: *¿lo cubre mi plan? ¿puede actuar sobre los recursos donde vive mi trabajo? ¿puedo ver
   qué hizo?*
8. **La caja del fondo**, una sola vez y aquí (§9.1).
9. **La Tira, columna 5.**

> **La condición de parada por agencia no es un adorno de dominio: es la que más dinero vale.** Entre el
> 30 % y el 50 % de las matrículas entran por agencias intermediarias (P03), que tienen **tarifas netas y
> condiciones de cancelación pactadas por convenio, distintas de las públicas**, y el sistema no las
> conoce. Aplicar la tarifa pública a una agencia con tarifa neta rompe el margen o rompe la relación
> comercial, **y se multiplica por quince alumnos**.

### La honestidad incómoda, dicha sin disculparse

> **Su capa 4 realista es «un proceso con juicio en dos o tres puntos», no «un agente autónomo que gestiona
> el buzón».** La barrera número uno no es técnica ni de capacidad suya: es de **licencia** —los agentes de
> verdad están detrás de planes que su empresa casi con seguridad no tiene [V]—, de **permisos** —un agente
> útil necesitaría el buzón compartido y la hoja de camas— y de **datos** —sus procesos de más volumen
> mezclan salud, religión, menores y documentación de identidad—.

Y la formulación que impide que eso envejezca mal: **el módulo no afirma «los agentes están fuera de tu
alcance»**, que es una falsedad desmotivadora esperando a ocurrir. Le hace **rellenar la ficha de cinco
preguntas para el agente que tenga delante ese día** y comprobar las tres cosas. **Si en 2028 las tres
respuestas son sí, el módulo funciona mejor, no peor: le da luz verde con criterio.** Un «no» sin condición
de revisión es dogma; un «no» con condición envejece bien.

### El aviso sobre su propia formación, que va en el material y no en una nota al pie

Es la única lección del curso donde su formación juega **en contra**. El reflejo entrenado de una psicóloga
ante alguien que se queja es **validar, empatizar y hacerse cargo**. Los dos primeros están bien y son una
ventaja real. El tercero, por escrito, en una queja formal, **es una admisión de responsabilidad que
compromete a su empresa**. Y los modelos son complacientes por construcción: si le pide una respuesta
empática a una queja, le va a dar un texto estupendo que dice *«tienes razón, la habitación estaba en malas
condiciones»*, y **sonará mucho mejor que el correcto**.

- Reconocer la **experiencia**, no calificar el **hecho**.
- Describir lo que **se ha hecho**, no juzgar lo que pasó.
- Evitar el **«lamentamos que te sientas así»**, que suena a disculpa y funciona como invalidación: es el
  peor de los dos mundos.

Importes, plazos legales, responsabilidad y compensaciones **no los decide ella y no los decide el
sistema**. Se escalan. **[!]**

### Cómo se autocorrige

- **Mecanismo dominante: cinco casos de parada fabricados que DEBEN parar**, y el quinto es un **ítem
  discriminante diseñado**: alguien que pregunta *«¿cuánto tarda el papeleo para poder venir?»* **sin decir
  la palabra visado**. *Los cuatro primeros los para cualquier lista; el quinto separa una lista de palabras
  de una lista de temas.*
- **Y el sexto caso, normal, que NO debe parar.** Si también para, **los frenos son demasiado anchos: el
  sistema no hace nada, y eso no es seguridad, es inutilidad.** El fallo del otro lado siempre está escrito.
- **Rúbrica con criterios negativos y salida escrita obligatoria** (sin «no aplica»): la lista incluye
  importes, plazos de visado, disponibilidad y salud **aunque su proceso no los toque hoy** —los sistemas se
  expanden solos y la lista se escribe para el sistema de dentro de seis meses—; «quién revisa» es un nombre
  y una hora; y **ninguna salida llega a un cliente sin que una persona le dé a enviar**.
- **Señal de fallo que predice su propia aparición:** *algún borrador suena estupendo y admite
  responsabilidad. **Aparece casi siempre.** Cuando aparezca, es el mejor ejemplo del curso de por qué la
  validez aparente no basta.*
- **Verdadero/falso de doce ítems** sobre el marco de datos, autocorrección instantánea. Menos de 10
  aciertos → releer.
- **CEBO 2**, ahora sobre una lista de frenos de mentira.
- **Y la descalificación de la correctora, que aquí está en ROJO** (§12.4): *este es el entregable del curso
  donde menos hay que fiarse de la corrección con IA, porque **le estás pidiendo a un modelo complaciente
  que juzgue si otro modelo es demasiado complaciente**. La IA solo para buscar señales de fallo; **el
  umbral de listo se comprueba mirando pararse el sistema.***

### Doblete · P28, respuesta a reseñas online · 20 min

**Clave: veredicto 6 con recorte** — clasificar y preparar sí, **publicar nunca**. Y el motivo no es de
calidad, es de protección de datos: **confirmar públicamente que alguien fue alumno y tuvo un problema ya
es una cesión de datos**. Es el doblete que mejor enseña que **un freno puede venir de un sitio que no es
la calidad del texto**.

### Orden de sacrificio de M4

- **Núcleo que no se cae nunca:** la lista de temas prohibidos · las seis condiciones de parada · los seis
  casos probados · el revisor con nombre y hora. Es la capa que protege a un cliente real.
- **Se cae primero:** la ficha de cinco preguntas sobre una herramienta ajena → se aplaza a **la semana 15**,
  dentro de M6, donde encaja con la Lista de techos. *Es lo único aplazable de este módulo y aun así hay que
  hacerlo: es uno de los tres resultados que hacen falsable la agnosticidad.*
- **Se cae segundo:** el plan de fallo en cinco pasos → versión reducida de **tres líneas**: a quién aviso,
  qué apago, y a quién escalo si hay datos de por medio.
- **La tercera semana de M4 está presupuestada para que una puerta cerrada no rompa el calendario.** Si no
  hace falta, se adelanta M5.

### PUERTA M4 → M5 — bloquea. Y **FRONTERA DECLARADA: al acabar M4 ya hay curso**

- [ ] Los cinco casos de parada **pararon y lo has visto**; **el sexto no paró**.
- [ ] Cada parada dejó **marca visible donde ella mira** y **dijo por qué**, en una línea.
- [ ] «Quién revisa» es **un nombre y una hora**.
- [ ] **No existe ningún camino por el que algo llegue a un cliente sin que una persona le dé a enviar.**
      *Si existe, se vuelve al principio del módulo.*
- [ ] El apagado está **probado**, no escrito.

**PC-5 al final del módulo.** Y aquí, cinco semanas antes de que ocurra, **se anuncia el compromiso externo
de M7**: *«en la semana 17 una compañera va a usar esto una semana entera sin ti.»*

---

## 6.6 M5 · Capa 5 — Medirlo sin engañarme · semanas 12–13

**Cambio mental.** *«Que el sistema se ejecute cada lunes no es que sirva. Puede ejecutarse impecablemente
y no cambiar nada, porque el informe que produce no lo lee nadie o porque los borradores se reescriben
siempre.»* **Evaluación de proceso ≠ evaluación de resultado.**

**El gancho, que no es metodológico sino de deseo.** Este módulo **no se presenta como «vamos a evaluar»**.
Se presenta así: *«vas a poder decir cuánto ahorras y defenderlo si alguien lo comprueba»*. Es el único
módulo del curso cuyo motivo se puede formular enteramente en términos de lo que ella ya quiere: **el
número es la munición del objetivo 5.**

### Qué construye

1. **Media página de evaluación, con fecha**: el número antes (de la hoja de sombra de M0, medida **antes**
   de construir nada, que es lo que la hace honesta) · el número después · el **coste completo** —montaje +
   revisión + mantenimiento— · **cuál de las seis amenazas a la validez interna podría explicar el
   resultado** y qué mediría para descartarla.
2. **La prueba ciega**, el ejercicio con mejor relación valor/esfuerzo del curso: cinco respuestas suyas de
   hace meses y diez salidas del sistema sobre casos comparables, **sin marcas de origen, barajadas por
   otra persona**, puntuadas con la ficha de criterio de M1.
3. **La cadena causal en cinco flechas**, con el eslabón que no depende de ella subrayado.
4. **La lectura completa de la Tira**: una frase escrita por columna diciendo qué aportó esa capa. *Si no
   puede escribir esa frase para alguna columna, esa capa no le aportó nada, y merece la pena saberlo.*

**Herramienta y por qué: una hoja de cálculo, un cronómetro y una persona que baraje.** Deliberado: **la
evaluación no se hace con la herramienta evaluada.** Pedirle a un modelo que juzgue lo que él mismo produjo
acumula dos sesgos documentados —preferencia por lo verboso y auto-preferencia— que apuntan al mismo
desastre: **aprobar por construcción**.

### Cómo se autocorrige

- **Mecanismo dominante: la prueba ciega es autocorrección en estado puro.** No hay rúbrica que discutir: o
  acierta identificando cuáles eran suyas, o no; o ganan las suyas, o no. Y el patrón que aparece casi
  siempre —**el sistema empata o gana en las dimensiones no críticas y pierde en la exactitud del dato**—
  **le dice exactamente dónde poner la revisión humana**, que es la decisión que el curso entero perseguía.
- **Prohibiciones de vocabulario como comprobación mecánica.** Si aparece «significativo», está mal: aquí no
  se estima un parámetro poblacional, **se comprueba la cobertura de un instrumento contra un criterio
  fijado**. Si la medida es «horas a la semana» en vez de **minutos por unidad**, está mal: es lo único que
  sobrevive a que su volumen se multiplique por tres entre febrero y julio.
- **La resta obligatoria.** Si no ha restado revisión y mantenimiento, está mal. Y si el saldo es negativo y
  aun así quiere conservarlo por otra razón —menos errores, menos carga mental, respuesta más rápida al
  cliente—, **que lo diga y mida esa otra razón**: es legítimo, pero entonces el ahorro de tiempo no era el
  objetivo.
- **Una amenaza que no puede descartar, nombrada obligatoriamente.** Las seis, traducidas a su caso:
  **historia** (septiembre no es julio) · **maduración** (ella misma ha mejorado en la tarea) · **regresión a
  la media** (eligió lo que más dolía, y lo que más duele suele medirse en su peor semana) ·
  **instrumentación** · **reactividad de la medida** (la semana que se cronometra se trabaja más rápido — y
  este juega **a favor**: el ahorro real es mayor que el medido) · **atrición** (si deja de usarlo los días
  de agobio, la muestra final son los días tranquilos).
- **La IA queda inhabilitada en este entregable** (§12.4, ROJO).
- El único favor humano del módulo —**barajar**— son cinco minutos y **no consume punto de consulta**: vale
  cualquier compañera.

**Caja obligatoria «lo que vas a ver la primera vez».**

> *«Es posible que el ahorro sea menor de lo que esperabas. Si eso pasa, es un resultado del curso, no un
> fracaso tuyo — y es exactamente el tipo de resultado que casi nadie publica. Antes de decidir nada,
> comprueba las dos cosas que casi siempre lo explican: que estés midiendo por unidad y no por semana, y que
> hayas contado el tiempo de revisión en el lado correcto de la resta.»*

### Doblete · P12, el check-in del lunes · 20 min

**Clave: no se deja medir así.** El valor de ese proceso es que **fija la percepción de calidad de toda la
estancia**, y eso no se mide en minutos por unidad. Es **deficiencia del criterio** con un caso de su casa,
y enseña la vacuna contra la métrica de vanidad mejor que cualquier explicación.

### Orden de sacrificio de M5

- **Núcleo que no se cae nunca:** el número con su resta y su amenaza nombrada. Sin él, M7 no tiene qué
  enseñar y el objetivo 5 se queda sin munición.
- **Se cae primero:** la cadena causal en cinco flechas → se aplaza a M7, donde se usa para escribir las tres
  preguntas escépticas del dossier.
- **Se cae segundo:** la prueba ciega → se aplaza a **la semana 14**, pero **no más allá**, porque su
  resultado decide dónde va la revisión humana.
- **La lectura de la Tira no se aplaza**: es la primera sesión del módulo y es el antídoto de la meseta.

### Lista de cierre M5 → M6 — **no bloquea**

- [ ] Hay un número con su método, con **la resta hecha** y con **una amenaza nombrada**.
- [ ] La prueba ciega está hecha **y barajada por otra persona**.
- [ ] La Tira tiene una frase escrita por columna.

> **Por qué aquí no hay puerta:** después de M4 no se construye nada encima. Una puerta solo se justifica
> cuando lo siguiente se apoya en lo anterior y el apoyo es caro de deshacer (§12.3). De M5 en adelante, lo
> que hay son consecuencias, no cimientos.

---

## 6.7 M6 · Capa 6 — Que sobreviva sin ti, y el resto de tu semana · semanas 14–15

**Cambio mental.** *«Un sistema sin dueño y sin fecha se degrada. Y cuando se degrada, el recuerdo que
queda en la empresa no es “faltaba mantenimiento”: es “aquello de la IA no funcionaba”.»*

### Qué construye

1. **La ficha de traspaso** (`06-traspaso.md`): qué fuente caduca y cada cuánto · **quién la revisa, con
   nombre** · qué batería se vuelve a pasar cuando se toque algo · cómo se apaga, probado · y qué hacer el
   día que falle.
2. **El calendario de revisión**, con la próxima fecha escrita.
3. **La rúbrica escrita por ella**, con al menos tres criterios negativos, **sin usar la del curso**, y
   **validada contra el CEBO 3**.
4. **EL MAPA DE LOS DOCE, PASADA 2** (§4.2.2). Sesenta minutos, una sola sesión.
5. **La prueba del hueco, lanzada aquí y recogida en M7:** dejar el sistema una semana sin tocarlo y
   comprobar qué se ha desactualizado. **Se recoge durante la semana del piloto**, que es una semana en la
   que ella no lo va a tocar de todos modos. **Coste real: cero.** *(Es el ajuste que aporta A y que ahorra
   una semana entera de calendario.)*
6. **El apéndice del escalón 4**, marcado como opcional y como lectura.

### Capacidad que entrena

**Hacer que un artefacto sobreviva a su autora**, que es puramente organizativa, no tiene nada de
tecnológica y es la que más vale dentro de tres años y en otra empresa: *¿qué de esto caduca y cada cuánto?
¿quién es la persona que lo mira? ¿cómo se apaga?* Y **clasificar procesos a volumen**, que es el objetivo
4 en su forma más directa.

### Cómo se autocorrige

- **Mecanismo dominante: la validación de su rúbrica contra el cebo 3.** Es un control positivo aplicado al
  instrumento que ella misma acaba de fabricar, y **es el criterio honesto de que ha terminado el curso**:
  cuando escribe las rúbricas, ya no lo necesita. *Si el cebo pasa su rúbrica, la rúbrica es blanda y se
  rehace.* Y tiene **función temporal declarada**: *si tu lectura como correctora se ha degradado en cuatro
  meses, se detecta aquí*, comparando el resultado con el del cebo 1.
- **Lista binaria de la ficha de traspaso, cinco ítems:** *¿hay un nombre de persona en «quién lo
  mantiene»? ¿hay una fecha en cada fuente? ¿hay una fecha en «próxima revisión»? ¿está probado el apagado?
  ¿alguien que no sea yo podría encontrar la carpeta?*
- **Las cinco comprobaciones de la pasada 2** (§4.2.3), incluida la de las tres filas al azar.

### Doblete · P32, mantenimiento de plantillas y FAQ · 20 min

**Clave: veredicto 2, arreglar el proceso primero.** Ahí el problema no es que falte automatización:
**falta una fuente de verdad.** Se actualiza la versión española del tarifario y las otras cinco se quedan
viejas durante meses. Es el riesgo «alto y silencioso» del inventario, y es **un hallazgo que aportar, no un
fracaso**. Va derecho al dossier de M7.

> **Por qué P32 y la pasada 2 están aquí y no antes.** Los dos producen **lo que ningún otro artefacto del
> curso produce: una lista de errores reales que nadie en la academia sabía que existían** —precios del año
> pasado circulando en la plantilla alemana desde hace meses—. Es el momento del curso en que su trabajo
> produce **un hallazgo y no un ahorro**, y por eso está colocado donde el material solo ya no tira. **Un
> hallazgo es mucho mejor combustible que un ahorro cuando quedan tres semanas.**

### Orden de sacrificio de M6

- **Núcleo que no se cae nunca:** la ficha de traspaso · **la pasada 2 del Mapa**. La primera es lo que
  convierte «una cosa que hizo ella» en «una cosa que tiene la academia»; la segunda es la mitad del objetivo
  4 y sin ella el delta no existe.
- **Se cae primero:** la rúbrica propia y el cebo 3 → se aplazan a **la semana 18**, dentro de M7. Es el
  indicador de «ya no necesito el material» y funciona igual de bien al final.
- **Se cae segundo:** el apéndice del escalón 4 → no tiene entregable y se puede no leer nunca.
- **La prueba del hueco no se aplaza porque no cuesta nada**: es dejar de tocar algo.

### Lista de cierre M6 → M7 — **no bloquea**

- [ ] La ficha de traspaso pasa su lista binaria de cinco ítems.
- [ ] La rúbrica propia **no deja pasar el cebo 3**.
- [ ] La pasada 2 tiene doce filas, **al menos cuatro veredictos 1 o 2 sin contar las ZP**, y sus «lo que sí».
- [ ] **Hay una persona con nombre que ha aceptado usar el sistema cinco días la semana que viene.**

---

## 6.8 M7 · Capa 7 — Que lo adopten: evidenciar y contagiar · semanas 16–18

Desarrollado entero en §11. Resumen de ficha:

**Cambio mental.** *«Un artefacto que solo funciona conmigo delante no es un sistema de la academia: es una
manía mía. Lo que hace que otros lo adopten no es convencerles: es que puedan usarlo sin mí, que yo pueda
enseñar el número, y que sepa decir también qué no hace.»*

**Qué construye.** El **dossier de una cara** · la **demo de tres minutos** guionizada y cronometrada · **la
semana sin ella** (el piloto) · **la lectura del delta** del Mapa · la **conversación del proceso de otra
persona** · la **lista de lo que decidió no automatizar** · **la reproducción del número ±10 %** · y, si en
M0 resultó que no existe, **una nota de media página para quien lleve la política de uso de IA**.

**Duración: 3 semanas**, y es el único módulo con una espera que no depende de ella: el piloto dura una
semana natural y no se puede acelerar.

**Doblete · el proceso de una compañera · 20 min.** Es a la vez el octavo doblete y la primera semilla de
contagio. **Sin clave de veredicto** —el curso no conoce ese proceso—, pero **con clave de ejecución**: la
lista binaria de si la entrevista se hizo bien (§11.3).

**Movilidad declarada, y va escrita en la semana 1:**

> **M7 no abre ninguna puerta y nada depende de él.** Contiene además una espera de una semana natural que
> no depende de ella. Por eso, **si el calendario se rompe —una baja, un pico adelantado, una compañera que
> no está disponible— M7 se puede mover, retrasar o partir sin que eso rompa nada, y sin que el calendario
> roto se lea como curso abandonado.** Un módulo cuyo final depende de la agenda de otra persona tiene que
> llevar escrito, desde el principio, que puede ocurrir en marzo.

**Orden de sacrificio de M7:** núcleo que no se cae nunca, **el piloto y su lista de arreglos**; se cae
primero la demo de tres minutos (el dossier la sustituye); se cae segundo la nota sobre la política de uso.

---

# 7. LA ESCALERA DE CAPACIDADES DEL PERFIL, Y DÓNDE SE CUMPLE CADA PELDAÑO

El perfil pide una progresión explícita: **usar mucho mejor el chat → automatizaciones → agentes cuando la
tarea lo justifique → herramientas avanzadas, al final y opcionales.** Este diseño **la respeta
literalmente**, pero no la usa como plan de estudios, y la diferencia importa:

> **La escalera no es el temario: es lo que le pasa a un proceso cuando lo aprietas.** No se «suben
> escalones» porque el calendario lo diga: **se choca con techos dentro de la misma cosa**, y cada techo se
> siente en su trabajo real antes de que nadie lo explique — y se escribe en la Lista de techos el día que
> se choca con él.

| Peldaño del perfil | Dónde se cumple | El techo que empuja al siguiente, **sentido y no leído** | Cómo se ve en las cinco preguntas |
|---|---|---|---|
| **0 · Chat a pelo** *(donde está hoy)* | Estado de partida, medido en M1 con la primera columna de la Tira: **saca 4 de 10** | *«Cada conversación empieza en blanco y le vuelvo a explicar la academia. Y no sé con qué cuenta entro ni qué protege esa cuenta»* | P3 = «lo que le pego en el momento» |
| **1 · Usar mucho mejor el chat** | **M0** (instrucciones permanentes + asistente v1) → **M1** (el criterio escrito antes del prompt) → **M2** (fuentes propias con fecha, cita y «no lo sé») | *«Se acuerda de sus instrucciones, no de lo que pasó ayer. Y sigue esperando a que yo lo abra cada vez»* | **P3 pasa a «fuentes que yo controlo y fecho»**. Y aquí es donde se gana casi toda la calidad del curso |
| **2 · Automatizaciones** | **M3** (disparador por reloj, ruta A; por suceso, ruta B; más el lote de la tarde de P27) | *«Dispara los lunes. No reacciona a que **haya pasado algo**.»* Y después: *«siempre el mismo camino: el caso que no previste sale mal, y sale mal en silencio»* | **P1 pasa de «yo» a «un reloj» y luego a «un suceso»**; P2 se congela en «yo, de antemano» |
| **3 · Agentes, cuando la tarea lo justifique** | **M4**, en su forma alcanzable: **juicio confinado a dos o tres puntos**, con frenos, condiciones de parada, y **la ficha de cinco preguntas rellenada para un agente real que el curso no enseñó** | *«Sigue siendo un camino que dibujé yo»*. Y la conclusión honesta: **su escalón 3 realista es un proceso con juicio, no un agente autónomo**, por licencia, permisos y datos — **no por capacidad suya** | **P2 se abre en dos o tres puntos concretos**; P4 pasa a «escribir en lo mío»; **P5 no cambia nunca** |
| **4 · Avanzado (tipo terminal)** | **Apéndice de lectura, sin entregable.** *Si termina el curso sin abrirlo, el curso ha funcionado igual*, y eso va en su primera línea | La condición que lo activaría: **procesar decenas de ficheros locales de forma repetida** — revisar doscientos contratos de estancia larga buscando una cláusula | P2 pasa entera al sistema. **Y ahí está el pago: renuncia a ser predecible** |

**Y el peldaño −1, que el perfil no pide y que es la mitad del criterio: NI IA.** Es el veredicto 1 de la
rejilla, con su prueba de la servilleta y su ejemplo canónico suyo (P02, el presupuesto). **Un curso que
empieza la escalera en el peldaño 1 enseña a subir; uno que empieza en el −1 enseña a decidir.**

**Y la lectura honesta que va escrita en la semana 1**, para que la escalera no le enseñe permanentemente
los peldaños que no va a pisar:

> *No vas a montar un agente autónomo en este curso, y no es por ti. Es por el plan que tiene tu empresa,
> por los permisos de tu buzón y por los datos que manejas. Las tres cosas están escritas en la Lista de
> techos con la condición que las cambiaría. El día que alguna cambie, tú vas a ser la persona de tu
> academia que sepa qué preguntarle a ese agente antes de dejarle tocar nada — que es más de lo que sabe
> hoy casi nadie que ya los está usando.*

**Y la escalera se lee, no se cuenta.** La lectura de la Tira en M5 —cinco columnas fechadas de su propio
trabajo— produce la conclusión que ninguna lección puede producir igual de bien: **subir de escalón no
mejora la respuesta; cambia quién la pide y cuánta autonomía has cedido.**


---

# 8. LA SEPARACIÓN CRITERIO / CLICS

No es una recomendación de estilo. Es **la convención de producción del material**, y si se relaja, el
curso deja de ser agnóstico en tres módulos. A y B coinciden en todo este bloque; va tal cual, con la
formulación más afilada de cada una.

## 8.1 Tres registros, no dos

Dos registros dejan un hueco **justo donde está el valor**: cómo encuentras esa función en una herramienta
que nunca has visto. Por eso son tres.

| Registro | Qué contiene | Dónde vive | ¿Caduca? |
|---|---|---|---|
| **EL CRITERIO** | Por qué se hace así · qué problema resuelve · cómo se decide si toca · cómo se comprueba · qué puede salir mal · el techo | `M3.1-capa.md` | **No** |
| **LAS SEÑAS** — *cómo reconocerlo en cualquier herramienta* | Descripción funcional de qué hay que buscar, y **las señas que distinguen esta capacidad de otra que se le parece**, con su condición de fallo | En el mismo fichero, en caja aparte marcada | **Casi no** |
| **LOS CLICS** | Rutas, nombres de botón, capturas, límites numéricos, planes | `clics/M3.1-clics-<entorno>.md`, **fechado**, uno por entorno | **Sí, y da igual** |

## 8.2 Qué es exactamente el registro de señas, con su ejemplo

Es **un test funcional de reconocimiento**, no una tabla de nombres de producto. Para la capacidad de la
capa 2:

> **Qué estás buscando**, en palabras que no dependen de ningún producto: un sitio donde se cree **un
> espacio con nombre**, se le adjunten documentos, y las respuestas se limiten a ellos.
>
> **Las tres señas de que has encontrado la capacidad correcta:**
> 1. **Las fuentes siguen ahí mañana**, sin volver a subirlas.
> 2. **La respuesta dice de qué documento sale.** Si no cita, no es esto.
> 3. **Puedes listar qué hay dentro** y quitar una fuente sin rehacerlo todo.
>
> **Si falta cualquiera de las tres, lo que tienes es un adjunto en una conversación**, que es otra cosa y
> dura lo que dure esa conversación. Es la confusión más frecuente y la que hace que la gente crea que ya
> tiene esto montado cuando no lo tiene.
>
> **Señas de que la herramienta NO sirve para este uso:** no permite quitar fuentes · mezcla lo que le has
> dado con lo que sabe de fuera sin distinguirlo · no hay forma de ver cuántas fuentes hay.

Y para la capa 3, con la pregunta que ata este registro con la cuarta columna del embudo:

> **Las tres señas de un disparador de verdad:** puedes elegir entre **al menos una condición de reloj y
> una de suceso** —si solo hay reloj, tienes media capacidad y conviene saberlo antes de diseñar— · hay una
> **lista visible de lo que está activo** y puedes desactivar sin borrar · hay algún sitio donde **ver que
> se ejecutó**. **Si no puedes comprobar que se ejecutó, no puedes fiarte de que se ejecutó.**
>
> **Y la comprobación que hay que hacer siempre, en cualquier herramienta y en cualquier año, antes de
> diseñar nada:** *¿sobre qué ficheros y qué buzones puede **actuar** esto —no leer: actuar— con mi cuenta y
> sin pedirle permiso a nadie?* Casi todas las herramientas de automatización tienen restricciones con
> recursos compartidos, y esa restricción decide qué procesos puedes automatizar y cuáles no.

**Eso es lo que sirve el día que entre en otra empresa y le abran una pantalla desconocida.** Una tabla de
tres nombres de producto, por su propia declaración, **caduca por completo**.

## 8.3 Estructura de ficheros y las siete reglas de producción, todas mecánicamente comprobables

```
curso/
  M3/
    M3.1-capa.md              ← EL CRITERIO + LAS SEÑAS. Sin fecha. Sin nombres de producto
    M3.1-ejercicio.md         ← EL EJERCICIO. Tampoco nombra productos
    M3.1-rubrica.md           ← con su bloque 3: hasta dónde llega la IA en ESTE entregable
    M3.1-solucion.md
    M3-cierre.md              ← 5 preguntas + pregunta fija + doblete. Nunca nombra productos
    clics/
      M3.1-clics-<entorno-actual>.md   ← fechado, reemplazable
      M3.1-clics-<otro-entorno>.md     ← fechado, para la prueba de portabilidad
  comun/
    datos-volatiles.md        ← TODO número: cupos, límites, precios, qué edición incluye qué,
                                 el −3 de la cuarta columna, y las fechas del marco normativo
    tres-nombres.md           ← equivalencias. La única página que caduca entera
    cuando-no-coincide.md     ← qué hacer cuando el manual y la pantalla discrepan
    protocolo-ia.md           ← las siete reglas de corrección con IA
    claves/                   ← claves selladas: batería, ocho dobletes, tres cebos, codificación de P27,
                                 tres motivos de descarte de M0
    expediente-modelo/        ← el recorrido completo hecho sobre P27
    orden-de-sacrificio.md    ← una tabla por módulo (§6.0.1)
```

1. **Ningún nombre de producto en un fichero de criterio, de señas, de ejercicio o de cierre.**
   Comprobación real, no aspiracional: un `grep -iE` con la lista de productos sobre esos ficheros tiene que
   devolver **cero líneas**. Si devuelve alguna, esa frase va a clics o se reescribe.
2. **Ningún número volátil fuera de `datos-volatiles.md`.** Se **referencian**, no se copian. Actualizar el
   curso es actualizar un fichero, no treinta.
3. **Ningún ejercicio puede depender de una captura ni de una ruta de menú.** Prueba mecánica, ejecutada una
   vez sobre el material terminado: **se borra el directorio `clics/` entero y todos los ejercicios siguen
   siendo enunciables.** Uno que deje de serlo está mal escrito y se reescribe.
4. **La regla del sujeto.** En un fichero de criterio, **el sujeto gramatical de cada frase es el proceso,
   el dato o ella**. Nunca un producto. *«El proceso necesita saber de qué documento sale cada dato»* es
   criterio; *«el asistente admite diez ficheros»* es clic, porque el sujeto es la herramienta.
5. **La prueba del sustituto.** Sustituye cada nombre de producto por «la herramienta» y relee. Si deja de
   tener sentido, el párrafo pertenece a clics. Si sigue teniendo sentido, **borra el nombre para siempre**:
   no hacía falta. **Esta segunda mitad es la que de verdad limpia el texto**, porque el fallo típico no es
   escribir un párrafo de clics en la mitad de criterio: **es dejar nombres de producto decorativos en
   frases que no los necesitaban.**
6. **Todo fichero de clics abre con la misma cabecera:** *«Verificado el `<fecha>` en `<entorno>`. **Si algo
   no coincide con lo que ves, tu pantalla tiene razón y este texto no.** Ve a `cuando-no-coincide.md`.»*
7. **Todo fichero de clics termina con la misma línea:** *«Si esto ha cambiado, lo que sigue siendo verdad
   está en `M3.1-capa.md`.»* Es una línea, y es lo que impide que un botón renombrado se lea como que el
   curso entero ha caducado. La cabecera cubre la mitad del problema; esta línea cubre la otra.

**Ejemplos de la conversión, con material real de este curso:**

| No se escribe | Se escribe |
|---|---|
| «Crea un Gem» | «Guarda este asistente con nombre, para poder reabrirlo sin volver a explicar el contexto» |
| «Sube el tarifario al cuaderno» | «Dale como fuentes los documentos sobre los que quieres que responda, y exige que cite de cuál sale cada dato» |
| «Tal herramienta no admite unidades compartidas» | «Comprueba, **antes de diseñar nada**, sobre qué ficheros puede actuar tu herramienta de automatización: casi todas tienen restricciones con recursos compartidos» *(y el límite concreto, en clics)* |
| «Pon una acción programada semanal» | «Elige qué lo dispara: una fecha del calendario o un suceso. La diferencia decide qué casos vas a poder atender» |

**Nótese la costura de la tercera fila, que es la que responde a la objeción del juez 3 sobre la cuarta
columna del embudo: el límite concreto de la plataforma está en clics; la instrucción de comprobarlo antes
de diseñar está en criterio.**

**Y `cuando-no-coincide.md`**, media página escrita una vez y referenciada desde todos los ficheros de
clics, convierte la caducidad del material de defecto en **competencia enseñada**: buscar el nombre nuevo
en las novedades del proveedor · comprobar si es restricción de plan o de administrador · preguntarle a la
propia IA cómo se llama ahora eso y dónde está · y —solo si nada funciona— el comodín PC-4.

## 8.4 Las tres pruebas de portabilidad, y qué demuestra cada una

La agnosticidad no se declara: **se ejecuta tres veces, con entregable, y con restricción de datos**.

| # | Dónde | Qué se hace | Coste | Qué demuestra |
|---|---|---|---|---|
| **P1** | M2 | **Reconstruye el mismo asistente en otra herramienta** —ella ya usa ChatGPT por su cuenta— **usando solo material verde** (tarifario, calendario, condiciones: **no son datos personales**). Le pasa las mismas diez preguntas | 25 min, tiempo propio | Que el criterio y las fuentes viajan. Y **si no lo consigue en 20 minutos: aprendió la ruta, no la capacidad** |
| **P2** | M3 | **Sobre papel y documentación, sin dar de alta nada:** escribe su flujo en notación neutra `DISPARADOR → PASO → CONDICIÓN → SALIDA` y localiza cada pieza en la documentación de **otra** plataforma de automatización | 20 min | Que sabe **leer el catálogo de pasos de una herramienta que no ha visto nunca**. Es la habilidad que usará dentro de tres años, y protege la agnosticidad **exactamente en el tramo donde el material se vuelve más específico de plataforma** |
| **P3** | M4 | **La ficha de cinco preguntas para una herramienta que el curso no enseñó**, más su fila en la Lista de techos con la **condición** que la activaría | 20 min | Que el clasificador funciona **sin el curso** |

**Ficha de P1, y se corrige sola:**

| Qué viajó tal cual | Qué hubo que rehacer | Qué techo cambió |
|---|---|---|
| La ficha de criterio · las fuentes con su fecha y su dueño · la batería de diez casos · la regla de «no lo sé» · la línea de corte | Dónde se guarda · cómo se llama · cuántos ficheros admite · dónde se pega la instrucción | Cuántas fuentes acepta · si cita el fragmento o solo el fichero · si conserva la instrucción entre sesiones |

> **Lo que se aprende no es «la otra herramienta también sirve». Es que el ochenta por ciento de tu trabajo
> era el criterio y las fuentes, y eso no estaba dentro de ninguna herramienta.**
>
> **Restricción de datos, y es contenido, no prudencia decorativa:** P1 se hace **con material verde
> exclusivamente**. Su cuenta personal no tiene contrato de encargado del tratamiento y por ahí no pasa ni
> un dato de un alumno. Que la prueba de portabilidad sea también un ejercicio de semáforo no es
> casualidad: **es el diseño.** P2 y P3 no tocan ningún dato porque son sobre papel.

**Honestidad sobre el alcance de las tres, porque su nombre promete más de lo que dan:** demuestran que
**el criterio viaja**, no que ella sabría trabajar de verdad en otra herramienta con datos reales. Es
suficiente para el objetivo declarado —saltar sin fricción, no ser experta en dos entornos— pero hay que
llamarlas por lo que son: **pruebas de portabilidad del criterio**. Está en §17.

## 8.5 La tabla de tres nombres

Vive en `comun/tres-nombres.md`, es **la única página del curso donde conviven nombres de producto**, y su
función no es enseñar productos: es **desactivar el miedo del principiante a quedarse casado con una
herramienta** — el freno mejor documentado del Q&A de la referencia, preguntado tres veces con distintas
palabras.

| Capacidad (lo que dura) | Nombre hoy, A | Nombre hoy, B | Nombre hoy, C |
|---|---|---|---|
| Contexto que se aplica a todas las conversaciones | Instrucciones personalizadas | Instrucciones personalizadas | Preferencias |
| Asistente guardado con instrucciones propias | Gem | GPT personalizado | Proyecto |
| Fuentes propias con cita del fragmento | Cuaderno de fuentes | Ficheros de conocimiento | Ficheros del proyecto |
| Algo que ocurre por horario sin que lo pidas | Acción programada | Tarea programada | Tarea recurrente |
| Flujo con disparador por suceso | Automatización nativa de la suite | Plataforma externa | Plataforma externa |
| Acceso acotado a una fuente | Conector | Conector | Conector / MCP |

> **Nota fija al pie, y es la que hace el trabajo:** *«Esta tabla es la única página del curso que caduca
> por completo. Está fechada. Cuando algún nombre no coincida con tu pantalla, corrígelo tú: es tuya. Lo
> que no cambia es la columna de la izquierda.»*

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

## 9.1 El objetivo 1: por descarte, por veredictos y por techos — los tres, en momentos distintos

El objetivo 1 del perfil es *«saber qué existe: que existen agentes, que existen automatizaciones, qué se
puede automatizar de su trabajo y qué no»*. **Los tres términos van pegados a su trabajo.** No pide un mapa
del sector: pide saber qué hay disponible **para lo que ella hace**. Un curso que conteste con un recorrido
de productos está contestando a otra pregunta, y además contesta con la mitad que caduca.

**Este era el objetivo peor servido por una columna vertebral de un solo proceso, y por eso lleva cuatro
mecanismos y no uno.** La pregunta del encargo —*¿por descarte, por techos o por veredictos?*— tiene una
respuesta clara: **por los tres, en tres momentos distintos, con tres funciones distintas, y en este
orden**, porque el orden es lo que hace que cada uno sea barato cuando ocurre.

| Cuándo | Mecanismo | Qué produce | Por qué **ahí** |
|---|---|---|---|
| **Semana 1, día 3** | **POR DESCARTE.** Seis descartes automáticos por número + **tres motivos escritos contra clave** | La noción de que **hay un fuera antes de que haya un dentro**, y la primera calibración del curso | Cuesta diez minutos y no depende de criterio que todavía no tiene. **El descarte es la única forma de clasificación que se puede hacer bien en la semana 1** |
| **Semana 1 (pretest) y semana 14 (real)** | **POR VEREDICTOS.** La rejilla de seis, aplicada a los trozos de su proceso (M1), a ocho procesos ajenos con clave (M1–M7), y a doce procesos suyos (semanas 1 y 14) | **Más de cuarenta juicios sobre procesos reales**, once de ellos contra clave, y **un delta medible** | La clasificación **sin justificar** puede ir al principio porque es **una medida**; la clasificación **justificada** tiene que ir después del criterio porque **antes es adivinar** |
| **Al cerrar cada capa, ocho veces** | **POR TECHOS.** Una fila en la Lista de techos, con su tercera columna en **condiciones** | El catálogo **generado desde la carencia sentida**, incluido el agente | Una fila se escribe **cuando el proceso choca con el techo**. Antes de eso, «agente» es una palabra; ahí es **una carencia concreta con nombre** |
| **Una vez, en M4** | **LA CAJA DEL FONDO.** El resto del panorama, con el eje puesto en la **condición** y no en el producto | Reconocer de qué le hablan cuando le hablen de ello | Antes de M4 no tiene con qué compararlo; después de M4 llega tarde para el objetivo 1 |

**Y esa es la razón por la que no hay módulo de panorama.** Un catálogo leído en la semana 2 se olvida en
la 4; un catálogo generado en ocho trozos, cada uno el día que hizo falta, se recuerda porque cada fila
tiene una anécdota propia detrás.

### La caja del fondo

Media página, en M4, con el eje puesto en la **condición** — que es la diferencia entre una tabla que hay
que rehacer cada año y una que se revisa.

| Qué haría falta para que me tocara | La clase de cosa que lo haría | Qué es hoy, para reconocerlo si me hablan de ello |
|---|---|---|
| Tener que **actuar** sobre un sistema que no está en mi suite (software académico, pasarela de pago, mensajería, portal de una agencia) | Una plataforma de automatización externa | Ojo: **mete un proveedor más entre mis datos y yo, y eso hay que pesarlo** |
| Tener una tarea **cuyos pasos no pueda dibujar de antemano** | Un agente: le das objetivo y límites y decide los pasos | Están detrás de planes que mi empresa casi con seguridad no tiene, y necesitarían actuar sobre recursos compartidos |
| Necesitar que una herramienta lea de una fuente mía **con permisos acotados** | Un acceso acotado, y el estándar por el que se conectan | Para mí hoy es **vocabulario, no herramienta**. Lo que sí me sirve es el principio: **conectar solo a lo necesario, y a una carpeta, no al disco** |
| Tener que **procesar decenas de ficheros locales** de forma repetida | Un agente con acceso al sistema de ficheros | Revisar doscientos contratos de estancia larga buscando una cláusula sería el caso |
| Que mis fuentes pasen de **decenas a cientos** y el asistente empiece a perderse | Arquitecturas de recuperación sobre corpus grandes | Con veinte fuentes bien fechadas no me hace falta nada de eso |
| Que me hablen de un sitio «de la misma empresa, gratis, donde se prueban prompts» | Una superficie de desarrollador | **Trampa silenciosa:** sus propios términos dicen que no metas información personal. **Parece seguro porque entras con la cuenta de siempre, y no lo es** |

**Hasta dónde llega esto, honestamente.** Cubre lo que su proceso toca, lo que los dobletes rozan y lo que
el Mapa clasifica: más de cuarenta procesos. **No cubre el panorama del sector** ni le da una opinión
informada sobre familias de herramientas que no ha visto. Si en dos años le preguntan «¿qué herramientas de
automatización conoces?», la respuesta honesta de este curso es *«conozco la anatomía, sé leer el catálogo
de pasos de una que no he visto nunca, y sé qué preguntarle antes de dejarla tocar algo»* — que es mejor
respuesta de lo que parece, **pero no es la que da un curso de panorama, y este curso no lo es a
propósito**.

## 9.2 El Doblete: cada capa se repite en seco sobre un proceso que no es el suyo

Al cerrar cada capa, **veinte minutos, sobre papel**, aplicando la misma capa a un proceso distinto de su
lista. No se construye nada.

```
DOBLETE de la capa __ · proceso: P__ · fecha: ____ · 20 minutos

1. Si tuviera que aplicar esta capa aquí, ¿qué haría exactamente? (3-5 líneas)
2. ¿Qué cambiaría respecto a lo que hice en mi proceso?
3. ¿Hay algo de esta capa que aquí NO tendría sentido? ¿Por qué?
4. VEREDICTO (uno de los seis, o ZP): ____
   MOTIVO, de la lista cerrada de cinco, citando un hecho del proceso: ____

— y solo después de firmar: abre `comun/claves/doblete-<capa>.md` y anota en qué coincides y en qué no.
```

> **LOS OCHO DOBLETES LLEVAN CLAVE SELLADA**, y A y B coinciden en que es la reparación más importante que
> el corpus necesitaba. Sin ella, **toda la maquinaria de transferencia del curso** tenía corrección solo
> **formal**: la lista comprobaba que existieran y que sumaran la cuota, no que el veredicto fuera correcto.
> Y lo absurdo es que **la respuesta correcta de cada uno ya estaba razonada**; solo faltaba sellarla, que
> es la convención que el curso aplica religiosamente a la batería. Con clave, los ocho dobletes dejan de
> ser un ritual y pasan a ser **ocho contrastes con oráculo externo**, que es la única forma sin profesor de
> saber si el criterio generalizó o se pegó al caso.
>
> **Y la regla de lectura de la clave, que va escrita:** *si no coincides, **no reescribas tu veredicto**.
> Escribe en una línea por qué creías lo que creías. Ese desacuerdo es el dato, y es material de PC-5.*

**Los ocho dobletes, asignados para que cada capa choque con un tipo distinto de «no»:**

| Capa | Doblete | Clave: veredicto y motivo | Qué enseña |
|---|---|---|---|
| 0 · Ver el proceso | **P29** emergencias 24 h | **ZP** · riesgo | Describir un proceso **no** compromete a delegarlo. Se mapea para **no** delegarlo |
| 1 · Criterio y corte | **P02** presupuestos | **1** · no necesita un modelo | El escalón −1. Meter un modelo aquí **es introducir un error posible donde no lo había** |
| 2 · Contexto | **P08** carta de aceptación para visado | **ZP** · conocimiento que caduca | *No metas conocimiento volátil dentro de un artefacto.* El motivo vale para cualquier dominio |
| 3 · Disparador | **P30** parte semanal *(20 min)* + **P16** exámenes oficiales *(10 min)* | **5** · —  /  **5** · las reglas son de otro | Que «automatizar» no significa «meter un modelo». Y que hay procesos **cuyas reglas y plazos los fija una institución ajena** |
| 4 · Juicio y frenos | **P28** respuesta a reseñas online | **6 con tachón de publicación** · riesgo | Que un freno puede venir de un sitio que no es la calidad del texto: **confirmar públicamente que alguien fue alumno ya es una cesión de datos** |
| 5 · Medir | **P12** check-in del lunes | **no se deja medir así** · deficiencia del criterio | Que hay valor que no cabe en minutos por unidad |
| 6 · Sobrevivir sin ti | **P32** plantillas y FAQ | **2** · no hay fuente de verdad | Que a veces el problema no es que falte automatización: **es que falta una fuente de verdad** |
| 7 · Que lo adopten | **el proceso de una compañera** | **sin clave de veredicto** — el curso no conoce ese proceso — **pero con clave de ejecución** | La capa 0 aplicada a un proceso ajeno, con su dueña delante. Semilla de contagio |

**Y la cuota, defendida como tal:**

> **De los ocho dobletes, al menos tres tienen que terminar en «ni IA», «arreglar el proceso primero» o
> zona prohibida. Si tienes menos de tres, no has transferido: has repetido. Vuelve.**

La justificación no es estética: cruzando los 32 procesos con lo que la plataforma puede hacer de verdad,
**el reparto real da entre cinco y siete noes por cada doce procesos**. Tres de ocho es un suelo prudente.
Y su función es psicológica: **convierte el «no» en algo que hay que encontrar**, y desactiva de raíz el
sesgo que produce un curso de IA por su mera existencia — **preguntarle a un curso de IA si algo debe
hacerse con IA tiene un sesgo obvio hacia el sí.**

**El riesgo de la cuota, y por qué aquí es menor.** Una cuota puede fabricar noes de conveniencia, y eso
depende de su honestidad en el peor sitio posible: consigo misma. **Pero aquí hay clave sellada.** Un «no»
de conveniencia sobre un doblete cuyo veredicto correcto es «aplica igual» **se detecta al abrir la clave**.
En el Mapa de los doce no hay clave posible, y ahí la señal de fallo es la comprobación de las tres filas al
azar y el ítem *«existe un veredicto 1 o 2 que puse para llegar a cuatro, no porque lo crea»*. **Esa
asimetría está reconocida en §17.**

**Coste total: ocho por veinte minutos, más diez del mini-doblete = menos de tres horas en dieciocho
semanas.** Y cada uno de esos juicios se emite **inmediatamente después de haber hecho esa misma cosa de
verdad**, que es cuando un juicio sobre un proceso ajeno vale algo.

## 9.3 Cómo se enseña a NO usar IA cuando no toca — ocho mecanismos, y los ocho se evalúan

Ninguno es una advertencia suelta. **Todos producen algo que se puntúa**, porque lo que no se evalúa no se
hace.

**1 · La línea de corte: el «no» es interior al proceso.** Es el mecanismo propio de esta columna vertebral
y el más fuerte de los ocho. El entregable central de M1 no es «qué automatizo» sino **el proceso partido
en trozos, cada trozo con veredicto y motivo**. Rúbrica tajante: *si no hay ningún trozo que se quede
contigo, está mal resuelto*, y *si el motivo es «es difícil», está mal.*

**2 · La lista cerrada de cinco motivos** (§6.2), que es lo que hace **transferible** cada «no». Una
prohibición sin motivo no se transfiere a un caso nuevo; **un motivo tipificado se comprueba contra una
lista y se aplica a un proceso que nunca has visto.**

**3 · Las dos cuotas, con su fiabilidad declarada:** tres noes de ocho dobletes **con clave**, y cuatro
noes de doce en el Mapa **sin clave, con señal de fallo**. Y la exclusión de las zonas prohibidas del
recuento del Mapa (§4.2.2), que es lo que la hace exigente en vez de decorativa.

**4 · El caso canónico se hace, no se prohíbe.** El presupuesto (P02) se monta **con IA** y **con fórmula**
sobre los mismos veinte casos, se cronometra y se cuentan los errores. **Gana la fórmula por goleada.**
Enseñar el «no» haciendo el «sí» y midiendo que pierde es infinitamente más fuerte que prohibirlo.

**5 · «Lo que sí se puede hacer alrededor», exigido con artefacto nombrable.** Es la mejor contramedida
escrita en cualquiera de las tres arquitecturas contra el momento en que un «no» se lee como *«entonces esto
no me sirve para lo que de verdad me duele»*. **El módulo no termina con una lista de renuncias: termina con
un sí concreto por cada no.**

**6 · Las zonas prohibidas, con el motivo y no solo la prohibición:**

| Proceso | Por qué no, dicho de forma transferible |
|---|---|
| **P08** carta de aceptación para visado | Riesgo crítico y **normativa viva**. **Congelar dentro de un artefacto un conocimiento que caduca es fabricar un error futuro** |
| **P26** quejas formales | Una respuesta que **admite responsabilidad por escrito compromete a la empresa**. Y los modelos son complacientes: **la complacencia por escrito, en una queja, es exposición legal** |
| **P29** emergencias 24 h | Personas, menores, responsabilidad civil, y un alumno en estado de shock con nivel A1 |
| **P25** reembolsos | Datos bancarios y riesgo de fraude por suplantación en el cambio de cuenta |
| **P17** matching con familia de acogida | Concentra **salud, religión y potencialmente orientación sexual** en una casilla de texto libre. **Es el proceso que más parece el caso ideal de IA, y por eso es la trampa** |
| **P22** calendario de camas | Riesgo crítico por overbooking, y además es un calendario de recursos: escalón −1 |
| **P05 / P16** nivelación y exámenes | **Anexo III del Reglamento de IA**: *evaluar el nivel educativo* es alto riesgo. **Aplazado, no cancelado.** Lo suyo no es decidirlo **[!]**: es reconocerlo y avisar |

Y la regla de oro que hace todo esto memorable, y que se recuerda cuando una lista de artículos no:

> **De todo su trabajo, el único trocito que está en la lista de alto riesgo es el que decide el nivel de
> un alumno. Todo lo demás —redactar, traducir, resumir, clasificar, preparar borradores— no lo está.**
> Esa asimetría se recuerda.

**7 · El coste completo como criterio de descarte, no como cálculo de justificación** (M5). *Un sistema que
ahorra ocho minutos y cuesta diez de revisión es una pérdida disfrazada de modernidad.* Y la métrica de
vanidad tiene nombre: **que se ejecute cada lunes no es que funcione.**

**8 · La opción segura suele ser también la más eficiente, y eso se demuestra, no se predica.** El mejor
ejemplo, y va en M2: **no transcribas la llamada.** Escribe tú un resumen de cuatro líneas al colgar, ya
seudonimizado, y trabaja con ese resumen. Es más rápido que subir un audio de doce minutos, no genera un
tratamiento nuevo ni un destinatario nuevo, y de paso piensas el caso. Enseñado así, **«no usar IA» deja de
ser una renuncia y pasa a ser una decisión de eficiencia.**

**Y un noveno, incómodo: el «no» a la propia arquitectura.** El checkpoint de divorcio de M1 autoriza por
escrito, desde la semana 1, a cambiar de proceso. **Un curso que no permite abandonar una decisión suya no
puede pedirle a ella que abandone las suyas.**


---

# 10. PROTECCIÓN DE DATOS, INTEGRADA

A y B coinciden en todo este bloque, con una sola diferencia de forma: A lo organiza en cuatro anclajes y B
en tres capas. Se toman **los cuatro anclajes de A**, porque el primero —dentro del clasificador— es el que
explica por qué esto no es un módulo, y las **tres capas temporales de B** como sub-organización de los dos
últimos.

## 10.1 El principio de diseño

Un módulo de protección de datos se lee una vez, se aprueba y se olvida. Y además **produce parálisis**,
cuando el objetivo es que **use más la IA, no menos: que la use en el sitio correcto.** Un bloque de
protección de datos que produce parálisis ha fallado.

Pero «transversal» tampoco basta como respuesta, porque suele significar «repartido y por tanto de nadie».
Aquí tiene **cuatro anclajes concretos, y ninguno es un anexo:**

| Anclaje | Dónde | Qué contiene | Por qué exactamente ahí |
|---|---|---|---|
| **Dentro del instrumento con el que se clasifica cualquier herramienta** | Instrumento 1, todo el curso | **Las preguntas 4 y 5 son literalmente protección de datos**: *¿qué puede tocar? ¿quién firma la salida?* No se puede clasificar un sistema sin contestarlas | Porque así **el régimen de datos se deriva de la clasificación** en vez de pegarse al final. **Quien contesta las cinco ya sabe qué salvaguardas necesita** |
| **Dentro del criterio con el que se elige el proyecto** | M0, embudo, columna 2 | El semáforo, con **−3 que descalifica** para rojo irreducible | Porque así la protección de datos no llega a frenar el proyecto: **decide cuál es el proyecto** |
| **En el momento en que le mete datos** | M2, antes de cargar fuentes | El **mapa de datos del proceso** (§10.3) · por qué quitar el nombre no basta · cuasi-identificadores · la prueba de la compañera · la regla de los adjuntos | **Es el momento exacto en que pasa de pegar texto a subir ficheros.** Al pegar ves lo que envías; al adjuntar, no. **Un Excel va completo** —todas las filas, las columnas ocultas, la hoja que se llama «datos antiguos»—, un PDF de pasaporte va entero, **una foto lleva coordenadas** |
| **En el momento en que algo actúa sin que ella mire** | M4, con los frenos | Temas prohibidos · condiciones de parada · *nada sale al cliente sin que un humano le dé a enviar* · **el deber de avisar de que es una IA** · registro de qué se generó y quién lo aprobó · plan para el día que falle, **incluido valorar si hay brecha [!]** · el **Anexo III** aplicado a su academia | **Antes de M4 no hacía falta; después de M4 sería tarde** |

**Capa permanente:** la **tarjeta del lunes** impresa al lado de la pantalla desde la semana 1, con seis
preguntas que caben en una nota adhesiva. *Si una regla necesita que te pares a pensar, no sobrevive a un
martes de julio con trescientos correos sin abrir.*

## 10.2 Los dos principios que ordenan todo lo demás y no dependen de ningún producto

> **Pagar resuelve quién es el proveedor, no qué tratamientos están amparados.** Que su empresa tenga
> contrato con alguien no legitima que ella meta ahí un pasaporte.
>
> **Sin indicador, trátalo como cuenta personal.** Es la única regla que no falla cuando no sabes.

## 10.3 El artefacto propio: el mapa de datos del proceso

Un semáforo genérico se lee y se olvida. **Un semáforo aplicado al único proceso que está construyendo se
usa**, porque contesta una pregunta que tiene delante. Una cara, cuatro columnas:

| Dato que atraviesa el proceso | Color | **En qué paso entra** | **Dónde hay que quitarlo, y quién lo quita** |
|---|---|---|---|
| Nombre y apellidos del alumno | Ámbar | En el correo entrante | Antes de pegar nada: lo quito yo, a mano |
| Nacionalidad + edad + fecha de llegada + barrio | **Ámbar peligroso** | En el cuerpo del correo | Se **generalizan**, no se borran: «alumno», «esta semana», «familia de acogida». **Combinados identifican a una persona entre 1.400** |
| Nº de pasaporte o NIE | **Rojo** | Adjunto en la reserva | **No entra nunca**, ni imagen ni PDF. Si necesito un dato de ahí, lo escribo yo a mano, y solo ese |
| IBAN, tarjeta, justificante de pago | **Rojo** | Adjunto o cuerpo | **No entra nunca**, en ninguna herramienta |
| Alergia, dieta médica, medicación | **Rojo** | Formulario de preferencias | **No entra nunca**, ni seudonimizado. Se degrada al mínimo funcional si el texto lo exige: «una intolerancia alimentaria» |
| Cualquier dato de un **menor** | **Rojo absoluto** | Grupos escolares, estancias de 16–17 | **Nunca, en ninguna herramienta, ni seudonimizado. Sin excepciones** |
| Dirección del alojamiento junto al nombre | **Rojo** | Confirmación de alojamiento | No entra. **Localiza físicamente a una persona** |
| Tarifario, calendario, condiciones, plantillas | **Verde** | Documentos de la academia | **No son datos personales.** Entran sin pensar, y **por eso el proceso puede empezar aquí** |

**Cuatro cosas que este artefacto hace y un semáforo genérico no:**

1. **Sitúa el punto de corte en el flujo, que es lo que convierte una regla en un gesto.** Saber que un
   pasaporte es rojo no cambia nada un martes; saber que **el pasaporte entra como adjunto en el paso dos y
   por eso el paso dos nunca sube el adjunto original**, sí.
2. **Nombra quién lo quita.** Si la respuesta no es una persona o un paso concreto, no hay corte: hay una
   intención.
3. **Es reutilizable como hábito portátil.** Un mapa de datos por proceso vale en cualquier empresa y en
   cualquier año, y no menciona ninguna herramienta.
4. **Muestra que la mayoría de su proceso empezó en verde**, que es el mensaje que evita la parálisis: **la
   protección de datos no le prohíbe trabajar, le dice por dónde empezar.**

**El ejemplo de reidentificación es de su casa, y es el que se memoriza:**

> ❌ *«La alumna coreana de 19 años que llegó el 3 de julio y está alojada con la familia de Chamberí dice
> que la comida no le sienta bien y que es celíaca.»*

No hay ni un nombre. Y **cualquiera de sus tres compañeras sabe de quién se habla en dos segundos.** Con
1.400 alumnos al año, nacionalidad + edad + fecha + barrio deja **una sola persona**. Y encima hay un dato
de salud.

> ✅ *«Un alumno de nivel A2 comunica una intolerancia alimentaria no registrada en su ficha inicial y pide
> cambio de régimen de comidas. Redáctame un correo a la familia de acogida explicando el cambio, en
> español, tono cordial y directo, máximo 120 palabras.»*

**La prueba que hay que memorizar, una sola:** *¿podría una compañera mía saber de quién hablo leyendo
esto?* **Y el criterio del otro lado, que casi nadie pone: el prompt resultante tiene que seguir
sirviendo.** Si la respuesta es inservible, ha quitado contexto que no era identificador — ese es el error
del otro lado y también hay que verlo.

## 10.4 Las cinco decisiones que hacen que esto funcione y no asuste

1. **La regla de los menores es tajante y sin excepciones**, más restrictiva de lo que la norma exige en
   todos los supuestos, **a propósito**: una regla con excepciones no sobrevive a julio.
2. **Cada decisión que no es suya va marcada [!] y con el nombre de a quién se escala.** El riesgo
   específico de este perfil es que, por ser la que más se preocupa, acabe siendo de facto la responsable de
   cumplimiento de la academia. El material lo prohíbe explícitamente: *tu papel no es ser la responsable de
   cumplimiento; tu papel es **no ser tú el agujero**, y saber cuándo hay que levantar la mano.* Los tres
   límites concretos: **no decide la base jurídica, no decide si hace falta una evaluación de impacto, no
   decide si hay brecha notificable.**
3. **Nada normativo se congela dentro de un artefacto.** Las fechas del Reglamento de IA, el estado del
   marco de transferencias y la ley española viven en `datos-volatiles.md` **con fecha visible**. Y eso es,
   además, **el mejor ejemplo pedagógico del curso** de la diferencia entre conocimiento estable y
   conocimiento volátil — que es exactamente la distinción que hay que dominar para construir fuentes que no
   envejezcan mal.
4. **El encuadre no es de permiso, es de aportación.** No está pidiendo autorización para nada: ya usa la
   herramienta, se la ha dado su empresa, y usarla está bien visto. Está **entendiendo la configuración
   antes de apoyarse en ella**. Si la academia nunca se lo ha planteado, **acaba siendo ella quien propone
   la política**, y eso no es venta interna: es su propio trabajo.
5. **La transición con su cuenta personal se resuelve sin moralina**, porque la moralina no cambia hábitos y
   además sería injusta: lo que hace es lo que hace casi todo el mundo. Línea limpia —cosas suyas y
   prácticas con casos inventados, en la personal; **cualquier cosa que venga de un correo, una llamada o un
   expediente de un cliente**, en la de empresa— y el argumento que de verdad convence, que no es «es
   ilegal»:

   > **Si mañana un alumno ejerce su derecho de supresión y la academia tiene que certificar que ha borrado
   > sus datos de todos los sitios, tu cuenta personal es un sitio que la academia no puede tocar y del que
   > ni siquiera sabe que existe.** No es que hayas hecho nada malo: es que has creado, sin querer, **un
   > almacén de datos de clientes fuera del alcance de la empresa**. Y eso, cuando aparece, no tiene arreglo
   > posible: no se puede desandar.

## 10.5 El dato que cambia la posición mental con la que se estudia esto

Merece salir en la primera página del curso: **el artículo 4 del Reglamento de IA, en vigor desde febrero
de 2025, obliga a las empresas que usan IA a garantizar un nivel suficiente de alfabetización en IA de su
personal.** Dicho de otro modo: **el curso que está haciendo es, técnicamente, cumplimiento normativo de su
empresa.** No es un extra que se paga a sí misma en su tiempo libre por pura iniciativa: **es una
obligación de la academia que ella está cubriendo.**

---

# 11. EL MÓDULO DE EVANGELIZACIÓN INTERNA — M7 · «Que lo adopten»

A y B coinciden en prácticamente todo este bloque. Se toma la unión, con la jerarquía de la evidencia y la
regla del coste de adopción cero que aporta B, y las cuatro reglas de arranque y la deuda de adopción que
las dos comparten.

## 11.1 Qué NO es, dicho primero porque es donde se estropea

- **No es conseguir el sí.** No hay autorización que pedir. En su empresa usar IA ya está bien visto y **lo
  mal visto es no automatizar**. Un módulo de venta interna resolvería un problema que ella no tiene y le
  robaría tres semanas a los que sí tiene.
- **No es marketing personal.** Nada de portfolio, nada de landing, nada de «mira lo que tengo ahora en mi
  CV». Ese es el destino del itinerario no técnico de la referencia porque **su alumno tipo quiere cambiar
  de sector**. La nuestra no — aunque sí quiere que lo aprendido le sirva si algún día cambia de empresa, y
  de eso se encargan **los seis instrumentos permanentes, no una web**.
- **No es pedir presupuesto.** Todo lo que ha montado cuesta cero. Pedir dinero cambia la conversación
  entera y no hace falta.
- **No es una presentación a dirección.** Una presentación es un evento; **la adopción es un hábito**. Y una
  presentación sin usuario real es una demo.
- **No es la columna vertebral.** Son tres semanas al final, alimentadas por tres líneas por capa. Si fuera
  la lente del curso entero, el curso dejaría de ser sobre su trabajo y pasaría a ser sobre su reputación, y
  **el criterio se contaminaría**: elegiría lo vistoso sobre lo útil.
- **No es convencer a nadie de que la IA es buena.** Ya están convencidos. El problema del brief es el
  contrario: **empujan con desconocimiento de lo que se puede hacer.** Lo que falta no es entusiasmo, **es
  información realista**.

## 11.2 Qué es: el enunciado del módulo

> **Demostrar y arrastrar.** Su empresa empuja la IA sin saber bien qué se puede hacer. Lo que cambia esa
> situación no es un argumento: es **una cosa que funciona, un número que se puede reproducir, y una
> segunda persona que la usa sin ella delante.** Este módulo produce esas tres cosas.

Y el principio que lo ordena entero:

> **La credibilidad se compra con los noes.** Quien llega diciendo *«estas cuatro cosas NO deberían
> automatizarse, y aquí está por qué»* consigue que le crean sobre la quinta. Quien llega diciendo que todo
> se puede automatizar consigue que no le crean sobre nada — **y esa es, exactamente, la posición en la que
> su empresa está hoy respecto a la IA.**

**La ventaja específica de esta columna vertebral:** el módulo **no tiene que fabricar su materia prima**.
Llega con un sistema que lleva tres meses en producción sobre su mesa, con una Tira de cinco columnas
fechadas, con un número medido contra una línea base tomada **antes** de construir nada, con doce veredictos
justificados y con una lista de noes razonados. **Eso no es una demo: es un historial.**

## 11.3 Qué enseña — ocho piezas, todas con artefacto

**(1) El número y su método, que van juntos o no va ninguno.** De M5 sale un ahorro en minutos por unidad,
con el coste de revisión restado y con una amenaza a la validez que no se puede descartar. **Las tres cosas
se presentan juntas.** Un número sin método es una promesa, y **una promesa que no se cumple quema los tres
proyectos siguientes**. Aquí su formación es una ventaja competitiva directa y hay que decírselo así: casi
nadie que presenta resultados de IA en una empresa sabe decir *«esto podría explicarse también porque
septiembre no es julio»*, y **decirlo es precisamente lo que hace que se crean el resto**.

**La jerarquía de la evidencia**, que es contenido de primera y se enseña como tal:

| Nivel | Evidencia | Por qué pesa lo que pesa |
|---|---|---|
| **1** | **Otra persona usa el artefacto sin ti** | Es **un hecho observable**, no una afirmación tuya. No admite réplica |
| **2** | **Un hallazgo que nadie sabía** — *«la plantilla alemana lleva meses mandando el precio del año pasado»* | Cambia el marco: no vienes a contar lo que ahorras, **vienes con un problema real que has encontrado** |
| **3** | **Minutos por unidad, con línea base y coste completo restado** | Es un número honesto y con su amenaza declarada. **Sobrevive a que lo repregunten** |
| **4** | Una demo | Impresiona y se olvida. **Vale solo si termina en el nivel 1** |
| **5** | *«Me ahorra muchísimo tiempo»* | **Vale cero.** Es exactamente lo que dice todo el mundo y por eso ya no significa nada |

Y la regla que ordena la redacción de todo lo que escriba: **una afirmación interna tiene que sobrevivir a
tres preguntas escépticas seguidas.** Se enseña haciendo: coge tu frase, escríbete las tres preguntas más
incómodas que te haría alguien que no te cree, y contéstalas **dentro** de la media página. Y aquí su
formación es ventaja directa: **las tres preguntas incómodas son, casi siempre, las amenazas a la validez
interna que ya nombró en M5** (*«¿no será que en noviembre hay menos volumen?»* = historia; *«¿no será que
has mejorado tú?»* = maduración).

**(2) Lo que el artefacto NO hace.** Es la tercera línea del Cuaderno de evidencias y en el dossier va **en
su propio apartado, no en letra pequeña**. Doble función: es honestidad, y es **gestión de expectativas
operativa** — si el dossier dice «no responde nada sobre visados y para en cuanto aparece el tema», la
primera pregunta incómoda ya está contestada antes de que la hagan.

**(3) La lista de lo que decidió no automatizar**, con el motivo tipificado. Sale de la línea de corte, de
los ocho dobletes y del Mapa de los doce: son las filas con veredicto 1, 2 y ZP. **Es la pieza que le da
credibilidad a todo lo demás, y no cuesta escribirla: ya está escrita.**

**(4) La demo de tres minutos, con la regla del caso real.** No una presentación: **un antes y un después
con un caso real, elegido delante y no preparado**, y un número. Un caso preparado no convence a nadie que
haya visto alguna demo antes, y en 2026 todo el mundo las ha visto. **Se enseña también dónde falla** y qué
salvaguarda lo cubre — contraintuitivo y cierto: **mostrar el fallo es lo que convierte una demo en algo
creíble**, y es la única forma de que quien la adopte sepa dónde mirar. Y se termina siempre igual: *«si
quieres, te lo dejo montado para lo tuyo y te paso la hoja de cómo se usa.»* **Sin esa frase, la demo es
entretenimiento.**

**(5) La prueba del pasillo.** Explicar qué hace, qué ahorra y **qué no hace**, en treinta segundos y **sin
nombrar ninguna herramienta**. Regla de vocabulario dura: **se nombra el resultado, no la tecnología**. No
*«monté un flujo con un paso de extracción que llama a mi cuaderno de fuentes»*, sino *«los correos de
admisiones llegan ya clasificados y con un borrador hecho, y me ahorra unos ocho minutos por correo; los de
visado no los toca, los deja para mí»*. Esta regla es además la vacuna contra el efecto que más daño hace a
un evangelizador interno: **sonar a que ha descubierto una religión**.

**(6) LA SEMANA SIN ELLA — el corazón del módulo.** Una compañera usa el artefacto **cinco días laborables,
sin ella delante**. No una demostración acompañada: **uso real, sola**.

Es el único test verdadero de adopción y produce siempre el mismo hallazgo, que es lo que lo hace valioso:
**una parte del artefacto era ella.** Instrucciones implícitas, decisiones que tomaba sin darse cuenta, un
fichero que solo ella sabe dónde está, un criterio que nunca escribió porque le parecía obvio. Lo que el
piloto revela es exactamente lo que hay que arreglar para que la cosa **sobreviva a sus vacaciones** — **y
sobrevivir a sus vacaciones es literalmente la definición operativa de que la organización lo ha
adoptado**, en un negocio donde agosto vacía la oficina y julio la desborda.

**El entregable del piloto no es «salió bien»: es la lista de lo que hubo que arreglar, y tiene que tener al
menos dos entradas.** *Si el piloto no reveló nada, no fue un piloto: estuviste mirando por encima del
hombro.*

**(7) La ficha de traspaso**, que viene hecha de M6 y aquí se entrega de verdad. Es lo que convierte «una
cosa que hizo ella» en «una cosa que tiene la academia». Y es también protección propia: **un artefacto sin
dueño y sin fecha se degrada, y cuando se degrada el recuerdo que queda no es «faltaba mantenimiento», es
«aquello de la IA no funcionaba»**.

**(8) La conversación del proceso de otra persona** — la semilla de contagio, y a la vez el octavo doblete.
Veinte minutos con una compañera, aplicando **solo la capa 0** a un proceso de ella: qué lo dispara, qué
documentos abre, qué decisiones toma que no están escritas, qué sale y a dónde va. **No se construye nada y
no se promete nada.** Se escribe la descripción en una página y **se le devuelve para que la corrija**.

Por qué esto contagia y una presentación no:
- **Es la técnica que ella ya sabe hacer y que un perfil técnico no puede aportar**: entrevista
  semiestructurada, estructura de embudo, **preguntar por el último caso concreto y no por la norma**,
  preguntar por la excepción, y **devolver el procedimiento escrito para que lo corrijan — porque
  corrigiendo se saca más que preguntando**.
- **El encuadre que funciona no es «quiero automatizar tu tarea»** —eso pone a cualquiera a la defensiva—
  **sino «quiero aprender a hacerlo yo bien para no molestarte cada vez»**. Y es verdad, además.
- Y produce el efecto que ningún dossier produce: **la otra persona ve su propio proceso escrito por primera
  vez. Ahí es donde alguien pide algo.**

**Su clave sellada es de ejecución, no de veredicto**, y es una lista binaria: *¿preguntaste por el último
caso concreto en vez de por «cómo lo hacéis normalmente»? ¿preguntaste por la excepción? ¿le devolviste la
descripción escrita? ¿aparece en tu descripción al menos una decisión que ella toma y no está escrita en
ningún sitio? ¿prometiste algo?* **(esta última tiene que ser NO).**

## 11.4 Las cuatro reglas de arranque

| Regla | Por qué |
|---|---|
| **Empieza por un proceso que no sea de nadie** | Un proyecto que mejora la tarea de una compañera empieza con una persona a la defensiva; uno que hace lo que nadie hacía empieza con cero resistencia. **La elección del primer proceso es el 80 % de su adopción**, y por eso el embudo de M0 no era solo una cuestión de riesgo |
| **Coste de adopción cero** | El resultado se entrega **en el sitio donde esa persona ya mira** —su buzón, la reunión del lunes, el documento que ya abre— y **no** en una herramienta nueva a la que tenga que entrar. **Si adoptar exige que alguien aprenda algo, no se adopta.** Esta regla sola explica la mayor parte de los proyectos internos que mueren funcionando perfectamente |
| **Enseña el resultado, no el proceso** | La primera vez se enseña lo que sale, no cómo se hizo. **El «cómo» se cuenta cuando alguien lo pide, que es la señal de que ya hay adopción** |
| **Deja que lo pidan** | La segunda persona no se recluta: aparece cuando ve el primer resultado. **Si a las tres semanas nadie ha pedido nada, el artefacto no era tan útil como parecía — y eso también es un resultado del curso**, no un fracaso personal |

## 11.5 La deuda de adopción, y el riesgo de acabar siendo «la de la IA»

Es la parte que ningún material de este tipo incluye y que en una empresa de treinta personas donde lo mal
visto es no automatizar **va a pasar**:

- **No entregues lo que no puedas mantener.** Todo lo adoptado tiene coste de mantenimiento, y lo paga ella.
  Un flujo que se rompe en julio, con 400 correos al día, no es valor: **es un problema que se ha creado
  ella misma y encima con público.**
- **Entrega el artefacto y el manual, no el servicio.** La frase que marca el límite, y conviene tenerla
  escrita: *«esto lo monté yo y así se mantiene; si quieres uno para lo tuyo, aquí está cómo se hace.»*
- **El bus factor invertido:** si es la única que sabe cómo funciona, **la organización no adopta el
  artefacto: la adopta a ella.** La ficha de traspaso es la contramedida, y por eso es entregable.
- Es la versión gemela del límite de rol de protección de datos, y se nombra con la misma regla: *tu papel
  no es hacerte cargo de todo; es no ser tú el agujero y saber cuándo levantar la mano.*

## 11.6 Cómo se autocorrige — el punto donde este módulo se juega su credibilidad

Es el módulo más difícil de autocorregir de los ocho, porque **su criterio de éxito es la conducta de otras
personas**, que ella no controla. Decirlo es obligatorio. Y aun así hay **cinco mecanismos, cuatro de ellos
comprobaciones y no juicios:**

1. **El piloto es el corrector, es binario, y se provoca en vez de esperarse.** Otra persona lo usó cinco
   días laborables sin ella, o no lo usó. **Se cuenta.** Y el entregable es **la lista de arreglos con al
   menos dos entradas**: ese es el criterio negativo del módulo y es lo que lo hace infalsificable. *(Es
   mejor que preguntar a las dos semanas si alguien lo usó espontáneamente, porque esa pregunta admite un SÍ
   falso por cortesía.)*
2. **La reproducción del número, ±10 %.** Dos semanas después de medir, con la ficha de método delante,
   vuelve a calcular. **Si no sale el mismo número dentro del ±10 %, el número no era reproducible y el
   dossier se reescribe.** Es un test-retest de su propio instrumento y no consume a nadie.
3. **La prueba del pasillo, cronometrada, con cuatro comprobaciones binarias:** *¿nombré alguna herramienta?
   ¿la otra persona pudo repetirme qué hace? ¿dije un número? ¿dije qué NO hace?*
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
artefacto, hay al menos cinco explicaciones —el artefacto es malo · la compañera está desbordada · la tarea
no era suya · el coste de adopción no era cero · no hubo tiempo— y el material **no le da forma infalible de
distinguirlas**. Lo que sí hace es **preinterpretar el silencio** con una rúbrica de cinco causas, cada una
con su seña y su arreglo mínimo, más **una sexta lectura legítima, escrita antes de que ocurra: que el
artefacto no debía adoptarse.** Un sistema que solo tiene sentido con ella delante puede ser perfectamente
correcto como herramienta personal, y **reconocerlo es un resultado, no una derrota**.

**Es el único punto del curso donde una alumna diligente puede hacerlo todo bien y salir sin saber si lo
hizo bien.** Está dicho en el material y está en §17.

## 11.7 Por qué al final y no en otro sitio

| Alternativa | Por qué no |
|---|---|
| Al principio, como encuadre motivador | No hay nada que enseñar todavía. Y arranca el curso **con la mirada puesta en lo que piensen los demás**, que es el desvío que el brief prohíbe |
| Repartido por todos los módulos | Convertiría cada capa en una pieza de comunicación y **contaminaría el criterio**: se elegiría lo vistoso sobre lo útil |
| Después de M4, cuando el sistema ya funciona | Tentador, porque ahí ya hay algo que enseñar. Pero **no hay número**, y un dossier sin número medido es una opinión con formato de informe |
| **Al final, después de medir y después de dejarlo mantenible** ← **la elegida** | Consume la salida de M5 **y** la de M6 **y** el Mapa de los doce. No se evangeliza lo que no está medido, y no se traspasa lo que no tiene dueño ni fecha. Además llega en el momento en que el material solo ya no tira: **el único incentivo disponible en la semana 16 es que alguien de fuera use lo que has hecho** |
| Al final, pero sin hilo previo | El Cuaderno de evidencias existe desde la semana 3 justamente porque, sin él, **M7 tendría que reconstruir números de memoria — es decir, inventarlos** |

## 11.8 Qué produce, en una lista

1. **Un dossier de una cara**: qué hace · qué ahorra y con qué método se midió · **qué no hace** · quién lo
   mantiene · cómo se apaga.
2. **Un guion de demo de tres minutos**, cronometrado, con un antes y un después reales.
3. **La semana sin ella, ejecutada**, y su lista de arreglos con ≥2 entradas.
4. **La lectura del delta del Mapa de los doce**, con el motivo de cada cambio.
5. **Una descripción del proceso de otra persona**, escrita por ella y corregida por su dueña.
6. **La lista de lo que decidió no automatizar**, con el motivo tipificado.
7. **El número reproducido** dentro del ±10 %.
8. **Una nota de media página** para quien lleve la política de uso de IA, si en M0 resultó que no existe
   ninguna. **No es venta: es cerrar el hueco que ella misma detectó en la semana 1**, y es el hallazgo con
   mejor relación valor/esfuerzo de todo el curso.


---

# 12. SISTEMA COMPLETO DE AUTOCORRECCIÓN SIN MENTOR

## 12.1 El enunciado del problema, y el techo que impide que el remedio sea peor

**El problema no es «no tiene quien la corrija». Es más incómodo:**

> **Para saber si su trabajo está bien necesita el criterio que el trabajo debía enseñarle. En el momento
> en que puede evaluarse con fiabilidad, ya no necesita el módulo.**

De ahí salen tres estrategias legítimas y no hay una cuarta: **(A)** traer el criterio de fuera y ponerlo
por escrito **antes** —rúbricas, listas, soluciones comentadas—; **(B)** **sustituir el juicio por una
comprobación** —casos con respuesta conocida, ejecución real—; **(C)** externalizar el juicio a un tercero
—la IA, que es un tercero poco fiable de forma sistemática y predecible; o la pareja, que es una reserva
estratégica y no un mecanismo—.

> **La primera decisión de diseño de cada entregable no es «qué rúbrica pongo». Es: ¿puedo convertir esta
> evaluación en una comprobación?** Muchísimas veces se puede, y casi nunca se intenta.

**Y la advertencia que hay que hacer en la misma frase en la que se hace la afirmación central, porque si
no es trampa:** el mejor corrector de este diseño es que el artefacto está en producción sobre su mesa.
Pero **funcionar no es estar bien**. **El mundo corrige la utilidad; los instrumentos corrigen el
criterio.**

### 12.1.1 Cuánta autocorrección es suficiente — las cuatro reglas que impiden la burocracia [J]

Esta es la cuarta pregunta del encargo y ni A ni B la contestan de frente. Las dos **acumulan** mecanismos
—cada uno bueno por separado— y ninguna escribe el límite. **Un aparato de corrección sin techo se come el
curso**, y en un curso de dos horas semanales eso no es una molestia: es la causa de abandono.

**Regla 1 · Un mecanismo dominante por entregable, y como mucho un respaldo. El tercero se elimina.**
Cada entregable declara cuál es su mecanismo más fiable disponible (§12.2) y cuál lo respalda. Si aparece un
tercero, es porque los dos primeros no son buenos, y entonces **el arreglo es cambiar el primero, no añadir
un cuarto**.

**Regla 2 · Techo del 20 %.** El aparato de corrección de un módulo **no puede pasar del 20 % de su tiempo
propio** — unos **45 minutos por módulo de dos semanas**. Si se pasa, se recorta **por la cola de
fiabilidad**: lo primero que se cae es el mecanismo menos fiable de la tabla, nunca el más fiable.

**Regla 3 · Nada se comprueba dos veces, y toda comprobación produce algo que ya era entregable.** Una
rúbrica que verifica lo que ya verifica una lista binaria es burocracia pura. Aplicando esta regla, este
diseño **retira** cuatro cosas que A o B tenían: la rúbrica de ocho ítems sobre la ficha del entorno —la
ficha ya son ocho casillas y basta con el estándar «creo que» = suspenso—; la comprobación de las tres filas
al azar sobre el pretest del Mapa —el pretest está declarado equivocado—; la sexta columna de la Tira; y el
contraste rutinario de dos modelos, que se conserva **solo** como alternativa degradada de PC-3.

**Regla 4 · La regla de retirada, que es el único mecanismo sobre los mecanismos.**

> **Un mecanismo que en tres usos seguidos no ha cambiado ninguna decisión suya se retira**, y ella lo anota
> en la bitácora con una línea: *«retiro X porque en tres usos no me ha hecho cambiar nada.»* No es
> permiso para saltarse cosas: **es la comprobación de que el aparato de corrección también se evalúa.** Y
> es coherente con lo que el curso le enseña sobre instrumentos: **un ítem que no discrimina se quita.**
>
> **Excepciones que no se pueden retirar nunca:** las cuatro puertas, las claves selladas, los tres cebos y
> la resta de M5. Son los únicos mecanismos cuyo valor no está en cambiar una decisión cada vez, sino en
> **existir el día que haga falta**.

**Y el criterio de fondo, en una frase:** *se admite como mecanismo de corrección lo que cuesta menos de
cinco minutos, o lo que produce un artefacto que ella querría tener de todos modos. Todo lo demás es
burocracia y se recorta.*

## 12.2 Los nueve mecanismos, ordenados por fiabilidad real, y dónde vive cada uno

| # | Mecanismo | Fiabilidad | Dónde vive en este curso |
|---|---|---|---|
| **1** | **Ejecución real: funciona o no funciona** | Máxima, cobertura estrecha | El correo del día 1 · el asistente responde o alucina · el disparador se dispara o no · los cinco casos paran o no · el apagado funciona o no |
| **2** | **Batería con clave sellada** | Muy alta | **La Tira**, cinco pasadas fechadas · las diez preguntas del asistente v1 · **las claves de los ocho dobletes** · **la clave de codificación de la tarde de P27** · los tres motivos de descarte de M0 |
| **3** | **Lista de comprobación binaria observable** | Alta, y **lo único que caza omisiones** | Una por módulo: fuentes (M2, 10 ítems) · plataforma (M3, 6) · frenos (M4, 11) · traspaso (M6, 5) · Mapa (M6, 5) · dossier (M7, 6) |
| **4** | **Solución comentada con anatomía del error** | Alta | Cinco o seis fallos típicos por módulo, cada uno con `cómo se reconoce en tu propio trabajo` · `por qué pasa` · `arreglo mínimo` |
| **5** | **Rúbrica con criterios negativos + autoevaluación diferida** | Media-alta | **Se usa al día siguiente, nunca al terminar**, y con encuadre en tercera persona |
| **6** | **IA correctora con rúbrica anclada y protocolo adversarial** | **Media, y variable de forma no aleatoria** | Con el protocolo de siete reglas, **y graduada por entregable** (§12.4) |
| **7** | **Contraste de dos modelos** | Media | **Solo como alternativa degradada de PC-3.** El desacuerdo es la señal, nunca el veredicto |
| **8** | **Punto de consulta con su pareja** | La más alta, estrechísima por escasez | **Seis en todo el curso** (§12.5) |
| **9** | **Autoevaluación libre** («¿me ha quedado bien?») | ≈ nula | **Prohibida como mecanismo**, y se dice por qué |

**Mecanismo dominante por módulo:**

| Módulo | Dominante | Respaldo único |
|---|---|---|
| **M0** | Cronómetro y pantalla | Los tres criterios de rechazo de la sombra |
| **M1** | **La muestra apartada** (tiene que fallar al menos uno de los diez) | **Cebo 1** |
| **M2** | **La batería, columna 3, con umbral asimétrico** | Lista binaria de diez ítems |
| **M3** | **Ejecución real: se dispara o no** | La tabla de confusión de la tarde de P27 |
| **M4** | **Los cinco casos de parada, y el sexto que no para** | Rúbrica con siete señales de fallo · **cebo 2** |
| **M5** | **La prueba ciega barajada por un tercero** | La resta obligatoria |
| **M6** | **Su rúbrica contra el cebo 3** | Lista binaria de traspaso |
| **M7** | **El piloto: cinco días sin ella, o no** | Reproducción del número ±10 % |

## 12.3 Las cuatro puertas — y el criterio de qué justifica bloquear

> **Arbitraje 3.** A pone **tres** puertas y argumenta que *cinco puertas en un curso sin profesor son cinco
> sitios donde parar*. B pone **seis** y argumenta que *una puerta que bloquea es la única figura que se
> parece a un «todavía no» de un profesor*. Los dos tienen razón sobre lo que están mirando, y ninguno
> escribe **el criterio** que decide cuántas. Este documento lo escribe:
>
> **Una puerta bloquea solo cuando se cumplen las tres condiciones a la vez:**
> **(a)** lo que viene después **se construye encima** de lo anterior;
> **(b)** si lo anterior está mal, **el error se multiplica** en vez de sumarse;
> **(c)** **deshacerlo más tarde es caro o imposible.**
> Donde falta alguna de las tres, **la frontera lleva lista de cierre y no puerta**, porque una parada sin
> multiplicación de error es solo una parada.

Aplicando el criterio salen **cuatro**, y las cuatro caen en la primera mitad del curso — que es exactamente
donde debe estar el aparato que bloquea, porque de M5 en adelante **no hay cimientos, hay consecuencias**.

| Puerta | Condición, toda observable | (a) se construye encima | (b) el error se multiplica | (c) deshacerlo es caro |
|---|---|---|---|---|
| **M0 → M1** | Hoja de sombra de dos días sin criterio de rechazo activado · **dos decisiones no previstas** en la descripción | Todo el curso | Un proceso mal elegido contamina las dieciocho semanas | Sí, a partir de M2 |
| **M2 → M3** | Batería 5/5 típicos, aclaración en límite, «no lo sé» en rechazo · **uso espontáneo ≥5 veces en una semana sin que el curso lo pida** · traslado hecho | M3 y M4 | **Automatizar algo que no funciona es multiplicar el error** | Sí: hay que rehacer el flujo |
| **M3 → M4** | El disparador ha corrido **una semana entera** sobre casos reales, seis casos correctos, tope y apagado probados · **ha visto fallar algo y sabe por qué** | M4 | **Sin haber visto un fallo no hay criterio para dar autonomía a nada** | Sí |
| **M4 → M5** | Los cinco casos de parada pararon y el sexto no · cada parada dejó marca y dijo por qué · revisor con **nombre y hora** · apagado probado · **ningún camino llega a un cliente sin que alguien le dé a enviar** | M5, M6, M7 | **Medir un sistema sin frenos mide otra cosa**, y además el que paga el error es un cliente | Sí, y con consecuencia externa |

**Las fronteras M1→M2, M5→M6 y M6→M7 llevan lista de cierre firmada, y no bloquean.** En M1 porque la
comprobación sustantiva de esa capa **no existe** —nadie puede decirle si su ficha de criterio mide lo que
importa— y porque **ya hay un punto de parada ahí: el checkpoint de divorcio**. En M5 y M6 porque después no
se construye nada encima.

**Y la regla que hace que una puerta no sea un suspenso, que ninguna arquitectura escribe:**

> **Una puerta que no se abre no es un fracaso: es una semana más en la misma capa. Esa semana está
> presupuestada** —por eso M4 dura tres semanas y no dos— **y las cuatro puertas llevan escritas sus causas
> típicas con su arreglo mínimo.**

## 12.4 La IA correctora: puesto 6 de 9, con protocolo y con calibración por entregable

**El protocolo, siete reglas**, en `comun/protocolo-ia.md`, citado desde cada rúbrica:

1. **Hilo nuevo, siempre.** Nunca se corrige en la conversación donde se construyó.
2. **No es tuyo.** *«Reviso el trabajo de una compañera que hace mi mismo puesto. Tengo que decidir si se lo
   devuelvo.»* Es la mitigación más barata que existe y tiene medida [E].
3. **Nunca preguntes si está bien.** *«Enumera los incumplimientos de esta rúbrica. Por cada criterio, cita
   textualmente el fragmento que lo incumple. Si no puedes citar un fragmento, no lo afirmes.»*
4. **Pega la rúbrica entera, con sus criterios negativos.** Sin rúbrica, el modelo se inventa el estándar, y
   **el estándar que se inventa es benévolo**.
5. **Prohibido discutir en el mismo hilo.** Si no está de acuerdo, no responde: anota, corrige o no corrige,
   y abre un hilo nuevo con la versión modificada y la misma rúbrica. **La conversación es el vector del
   fallo.**
6. **Dos modelos, y el desacuerdo es la señal, no el veredicto.**
7. **Su veredicto no cierra nada.** Devuelve una lista de fallos **candidatos**. Quien decide es ella.

**Y el resultado de aprendizaje que instrumenta la resistencia a la adulación en vez de predicarla (RA17):**
al terminar el curso tiene que haber **al menos un caso registrado en que decidió NO aceptar una crítica de
la IA, con el motivo escrito**.

### La calibración por entregable — la pieza más fina del sistema

Aplicar el mismo protocolo en todas partes está mal: **hay entregables donde el corrector no puede funcionar
por construcción.** Cada rúbrica declara, en su bloque 3, hasta dónde llega la IA en **ese** entregable:

| Entregable | Nivel | Por qué |
|---|---|---|
| Ficha de criterio (M1) · lista de fuentes (M2) · dossier (M7) | **VERDE — protocolo completo** | Son texto contra una rúbrica y errores de forma y de omisión: es su mejor caso |
| Línea de corte (M1) · Mapa de los doce (M6) | **ÁMBAR — solo el bloque 1** (buscar señales de fallo); el bloque 2 se comprueba mirando | La respuesta correcta depende de **hechos de su academia** que el modelo no tiene: caza forma, no hechos |
| Mapa de datos (M2) | **ÁMBAR — solo la forma** | Ningún modelo sabe qué documentos hay en su academia |
| Batería de diez casos (M1) | **ROJO para juzgar la calidad de la batería** | Preguntarle si tu instrumento es bueno a un modelo que no conoce el dominio es pedir una opinión sin referente. **Lo que la juzga es que falle al menos uno de los diez apartados** |
| **Lista de frenos (M4)** | **ROJO para el umbral de listo** | *Le estás pidiendo a un modelo complaciente que juzgue si otro modelo es demasiado complaciente.* **El umbral se comprueba mirando pararse el sistema** |
| **Evaluación y número (M5)** | **ROJO, inhabilitada** | Pedirle a un modelo que juzgue lo que él mismo produjo acumula **preferencia por lo verboso y auto-preferencia**, y las dos apuntan al mismo desastre: **aprobar por construcción** |

**Es la respuesta más fina que existe a «¿cómo se evita que la IA le dé la razón?»: reconociendo dónde no
puede evitarse.**

### Los tres cebos — control positivo sobre la correctora

| Cebo | Dónde | Sobre qué | Función añadida |
|---|---|---|---|
| **1** | M1 | Una **línea de corte de mentira** con tres defectos plantados: uno **visible**, uno de **omisión**, uno de **criterio** | **Calibra el instrumento antes de usarlo cincuenta veces** |
| **2** | M4 | Una **lista de frenos** con tres defectos plantados | Comprueba que el instrumento sigue sirviendo **en el entregable más difícil** |
| **3** | M6 | Un artefacto pasado por **la rúbrica que ella misma ha escrito** | Doble: **valida su rúbrica** *(si el cebo la pasa, la rúbrica es blanda y se rehace)* **y detecta la degradación de su propia lectura a los cuatro meses** |

| Resultado del cebo | Lectura | Qué hace |
|---|---|---|
| Encuentra los 3 | El instrumento sirve para este tipo de trabajo | Sigue |
| Encuentra 2 | Normal: detecta lo visible, se le escapa lo de criterio | Sigue, **sabiendo que la omisión y el criterio los tiene que cazar la lista de comprobación**, no la IA |
| Encuentra 1 o 0 | **El instrumento está roto para esta tarea** | Revisa la rúbrica (probablemente sea vaga). Si sigue igual: **esta tarea no se corrige con IA**, y pasa a los mecanismos 2–4 |
| Aprueba el cebo entero | Descalificatorio | **Ese tipo de trabajo nunca se corrige con IA en el resto del curso** |

## 12.5 Los seis puntos de consulta, con alternativa degradada

**El recurso es escaso, no renovable y con coste relacional.** Un mentor pagado se gasta sin culpa; una
pareja, no. Y un curso que convierta a la pareja en su soporte técnico daña dos cosas a la vez: **la
relación y la autonomía que el curso persigue**.

**Presupuesto: seis consultas de diez minutos en todo el curso** — una hora repartida en cuatro meses. Un
curso que reserve «consultas ilimitadas» obtiene en la práctica **cero**, porque cada consulta compite con
la comodidad de no molestar y pierde. **Uno que reserve exactamente seis, con nombre y momento, obtiene
seis.**

**Filtro de admisión, impreso en la portada del cuaderno.** Si falla cualquiera de las cuatro, no es punto
de consulta: *(1) ¿lo resuelve el material? (2) ¿lo resuelve la IA con el protocolo? (3) ¿lo resuelve
**mirar** —su pantalla, su consola, preguntar a su administrador—? (4) ¿lo he intentado veinticinco minutos
y he anotado qué he probado?*

**Ficha de cinco campos, escrita ANTES, máximo una cara:** la pregunta en una frase **cerrada** · mi
hipótesis y qué esperaría ver si tengo razón · qué he probado y qué pasó · **el dato concreto** (mensaje de
error literal, las dos respuestas que se contradicen) · qué haré con cada respuesta posible.

**Cuatro reglas de la conversación:** los cinco primeros minutos **sin pantalla** —muchas veces se resuelve
ahí, y eso es autoexplicación con oyente— · **él no toca el ratón** · sale con **una frase escrita en su
propio lenguaje** dentro de la hora siguiente · **a los diez minutos se para, esté como esté**; lo que no
cabe en diez minutos no es una consulta, es un problema de diseño del curso y se anota como tal.

**Y el principio de formulación, generalizado a los seis: cada pregunta se acota a lo que el consultor
PUEDE auditar** —el razonamiento y los hechos de plataforma, **no los hechos de la academia, que no
conoce**—. Gastar diez minutos irrecuperables en una pregunta que la otra persona no está en posición de
contestar es el peor uso posible del recurso.

| # | Momento | Qué lleva | Por qué ahí | **Alternativa degradada** |
|---|---|---|---|---|
| **PC-1** | Fin de **M0** (sem. 2) | *«He deducido que tenemos el plan X, que por eso no puedo hacer Y, y que por eso he descartado estos tres procesos y elegido este. ¿El razonamiento se sostiene?»* Con las comprobaciones empíricas hechas y la hoja de sombra delante | **Es el punto de mayor consecuencia del curso**, porque todo se construye encima. Y está acotado a lo que él sí puede auditar | Asumir el escenario **más restrictivo**, elegir el candidato con puntuación más alta que no dependa de ninguna función dudosa, y anotar la suposición como pendiente |
| **PC-2** | Inicio de **M2** (sem. 5), antes de cargar fuentes reales | Ocho tipos de dato reales clasificados en tres cajones —empresa / nunca / depende— y tres casos ya seudonimizados: *«¿tú sabrías de quién hablo?»* | **La única decisión del curso con consecuencia externa irreversible**, y el momento es exacto: **cuando pasa de pegar texto a subir ficheros** | Regla de máxima cautela: **si dudas, no entra**, y se anota. Y la prueba de la compañera se hace con **cualquier compañera de la academia**, que además es la evaluadora literal del criterio |
| **PC-3** | Fin de **M1** (sem. 4), tras el cebo 1 | *«Esta es la corrección que hizo la IA de un trabajo con tres fallos plantados. Encontró dos. ¿Estoy leyendo bien lo que se le escapa?»* | **El de mayor apalancamiento.** No se revisa su trabajo: **se revisa su instrumento de corrección**, que va a usar cincuenta veces más | Pasar el cebo por **dos modelos distintos** y comparar: el desacuerdo entre modelos es un sustituto pobre pero real del juicio externo |
| **PC-4** | **Comodín**, desde M3 | Un fallo de plataforma tras agotar la lista de seis comprobaciones y `cuando-no-coincide.md` | «Diez minutos ahorran una tarde». **No tiene fecha a propósito:** saber que existe un comodín reduce el miedo a atascarse, **que es un factor de abandono por sí mismo aunque no se use** | Documentar el fallo, **rodearlo** con una solución manual y seguir. Un curso no puede pararse por un botón que alguien movió |
| **PC-5** | Fin de **M4** (sem. 11) | *«Esta es la línea de corte con la que he terminado, estos son los tres sitios donde dudé, y estos son los dos dobletes donde no coincidí con la clave. ¿Dónde la moverías?»* | Juicio de escala y oportunidad: **preguntarle a un modelo si algo debe automatizarse tiene un sesgo obvio hacia el sí**. Y cae exactamente en la frontera de abandono | Los cinco motivos tipificados, los descalificadores por número de proceso, y **los desacuerdos con las claves de los dobletes**, que son la mejor materia prima disponible sin nadie |
| **PC-6** | **M7** (sem. 17) | La prueba del pasillo en treinta segundos, y después: *«¿qué he dicho que no podría defender si alguien lo comprobara?»* | Alguien que **sabe de IA y no conoce la academia** es el evaluador ideal para **jerga** y **sobreafirmación**. Y **cierra el curso con otra persona**, que evita el final en el vacío | Hacer la prueba del pasillo con una compañera de otro departamento. Y grabarse treinta segundos y contar los nombres de herramienta al día siguiente |

**Un uso de otra persona que NO gasta punto:** barajar las respuestas de la prueba ciega de M5 y guardar la
clave. Función mecánica de cinco minutos, vale cualquier compañera.

**Lo que deliberadamente NO es punto de consulta:** revisar un entregable (*«¿está bien mi asistente?»* →
rúbrica y batería) · explicar un concepto (→ material) · enseñarle a hacer algo (→ documentación) · dar
ánimos. **Y la tentación específica de esta configuración: que él le monte algo «que es un momento».** Eso
no es una consulta: es un artefacto que ella no sabrá mantener ni depurar, y en la capa siguiente será
deuda. **En un curso cuyo entregable es un sistema que tiene que sobrevivirle a ella, un trozo que no
entiende es literalmente el peor regalo posible.**

> **NOTA DE RIESGO SOBRE EL PROPIO RECURSO [NV].** **Todo esto asume que su pareja sabe de plataformas y no
> solo de modelos.** Si su conocimiento es de modelos, **PC-4 pierde casi todo su valor** y ese punto se
> reasigna a PC-2 o a PC-5. Es **un modo de fallo silencioso y más probable que la indisponibilidad**,
> porque la consulta ocurre igual y devuelve una respuesta que parece buena. La comprobación es de un minuto
> y se hace en la semana 1: *pregúntale si ha configurado alguna vez una automatización con disparador en
> una suite de empresa.*

## 12.6 El registro transversal

Un fichero, `bitacora.md`, una línea por sesión: fecha · minutos · qué he hecho · qué he producido · **qué
ha fallado** · nota de autoevaluación · **y las retiradas de mecanismos (§12.1.1, regla 4)**. Sirve para
tres cosas a la vez: es la base de la práctica espaciada —de ahí salen las cinco preguntas de repaso que
abren cada sesión— · es **la evidencia contra la ilusión de fluidez** —a las diez semanas puede leer lo que
le parecía imposible en la semana 2— · y es lo que hace que un punto de consulta de diez minutos rinda,
porque llega con el historial escrito.

---

# 13. PLAN ANTI-ABANDONO

**Dos hechos ordenan esta sección:** el 52 % de los inscritos en un curso autodidacta **nunca llega a
empezar** [E], y **el abandono posterior es episódico y localizable**, no un desgaste uniforme. Si los
momentos son localizables, se les puede poner algo delante.

**Dos principios transversales:**
- **Toda contramedida se escribe antes del punto de caída, no en él.** El modo mínimo redactado la semana en
  que ya ha fallado se lee como excusa; redactado en la semana 1, como plan.
- **Predecir el fallo es la contramedida más barata que existe. Un fallo anunciado es una etapa; un fallo
  inesperado es un veredicto sobre uno mismo.**

**Se descarta como candidato al podio «el primer resultado mediocre»** no porque sea improbable, sino
porque su contramedida es barata, conocida y ya está incorporada en cada módulo: la caja *«lo que vas a ver
la primera vez»*, escrita **antes** del ejercicio, que describe el resultado mediocre concreto que va a
obtener. Y la cita de la referencia, que es su mejor minuto: *«Ves el resultado. Detrás hay varias decenas
de intentos.»*

## MOMENTO 1 · Días 1–10 — el arranque, y la sospecha de haber elegido mal

**Qué pasa por dentro.** Tres cosas a la vez, y la tercera es específica de esta columna vertebral: la
fricción de arranque · el beneficio todavía es abstracto mientras el coste ya es real · y **se le pide
comprometerse con un proceso en la semana 1, que es cuando menos criterio tiene**. La conclusión peligrosa
no es «esto es difícil», es **«creo que he elegido mal y llevo dos semanas»**, y esa es irreversible si no
se anticipa.

**Once piezas, todas estructurales:**

1. **La sesión 1 no explica el curso: produce un resultado utilizable en veinticinco minutos**, con lo que
   ya tiene abierto, sin instalar nada y sin hablar con nadie. **El mapa del curso va después del primer
   resultado, nunca antes.**
2. **El premio grande llega el día 4, con dos redes debajo** (§6.1).
3. **La elección no es una apuesta: es una prueba con tres criterios de rechazo observables.** Se le quita
   el peso de «acertar» y se le da un procedimiento.
4. **El repuesto está nombrado y firmado el día 3**, no el día de la crisis.
5. **La regla del embudo vacío** (§5.4): **la semana 1 no puede terminar sin proceso.**
6. **El divorcio preautorizado, con su aritmética escrita**: al final de M1 cambiar de proceso cuesta unas
   dos horas. **Escrito en la semana 1** se lee como plan; escrito cuando ya ha dudado, como excusa.
7. **El hallazgo prometido a las 48 horas** (§5.3): convierte dos días de peaje en pago, dentro del tramo de
   máxima mortalidad.
8. **El orden de sacrificio de M0 y M1** (§6.0.1), escrito **antes** de empezarlos: saber de antemano qué se
   puede aplazar y a qué semana es lo que evita que una semana mala se lea como un fracaso.
9. **El diagnóstico del entorno no puede bloquear.** Las comprobaciones empíricas están en la misma página
   que los mensajes, y la rúbrica declara que *«pregunté a X el día D y no obtuve respuesta»* es un
   resultado válido.
10. **El contrato de una página, antes de empezar:** 18 semanas · 2 h semanales de tiempo propio · **0 €** ·
    nada que instalar · nada que pedirle a nadie · **la frontera de M4** · **la movilidad de M7** · el modo
    mínimo · y la definición observable de «terminado». *Un curso que se anuncia de ocho semanas y dura
    dieciocho se percibe como fracaso propio en la novena.*
11. **PC-1 al final de la semana 2**: otra persona implicada en el punto de máxima mortalidad, revisando
    exactamente la decisión que le da miedo.

## MOMENTO 2 · Semanas 7–9 — el primer bloqueo que no es culpa suya

**Qué pasa por dentro.** La automatización nativa de su entorno **falla con unidades compartidas, carpetas
compartidas y hojas con referencias externas** [V], y el centro de gravedad de su puesto **es un buzón
compartido y una hoja de camas compartida**. La primera vez que intente automatizar su trabajo de verdad, la
herramienta puede decirle que no. Y la conclusión que se saca no es «me he equivocado de carpeta»: es **«esta
herramienta no sirve para mi trabajo»**, y detrás, *«este curso no sirve para mi trabajo»*. **Es la única
conclusión de todas las simuladas que es irreversible.**

**Siete piezas, y la primera es preventiva y no paliativa:**

1. **La contramedida principal está seis semanas antes: la cuarta columna del embudo.** Los procesos que
   solo viven en recursos compartidos se descartaron en la semana 1, **cuando descartar costaba diez
   minutos**.
2. **La regla del embudo vacío** con su escalera de cinco pasos, incluida la petición de delegación de una
   etiqueta o carpeta propia. **Nadie se queda sin proceso.**
3. **La regla de independencia de plataforma:** **la ruta A —disparador por reloj dentro del chat que ya
   usa— basta para cerrar la capa, pasar la puerta y ejercitar los frenos de M4.** Ningún módulo posterior
   depende de que el constructor de flujos esté habilitado.
4. **El límite va en la primera página del módulo, con nombre y por escrito**, no en una fe de erratas.
5. **La lista de seis comprobaciones de plataforma**, entregada **antes** del primer disparador y
   reutilizable como diagnóstico. **Convierte un bloqueo en una comprobación con resultado**, que es lo
   contrario de un veredicto sobre una misma.
6. **La página `cuando-no-coincide.md`**, que convierte la caducidad del material en competencia enseñada.
7. **PC-4, el comodín, cuya existencia se anuncia mucho antes de que haga falta.** Y la caja «si nada de
   esto funciona»: **documenta el fallo, rodéalo con una solución manual y sigue.**

## MOMENTO 3 · Semanas 12–16 — la meseta del «ya me sirve»

**Qué pasa por dentro.** Al terminar M4 **el sistema funciona y ella lo usa**. El dolor que la trajo al
curso está resuelto. Y justo entonces vienen módulos que no añaden funcionalidad: medir, dejarlo
mantenible, clasificar, contagiar. Novedad baja, beneficio inmediato bajo, esfuerzo mental alto. **El
abandono aquí no se siente como abandono: se siente como haber terminado.** Y esa es exactamente la razón
por la que es peligroso, **porque los objetivos 4 y 5 del perfil viven enteros en ese tramo.**

**Ocho piezas:**

1. **La frontera se declara en la semana 1, y con estas palabras:** *«al acabar M4 ya tienes lo que viniste
   a buscar. Lo que viene después es lo que hace que esto te siga sirviendo dentro de dos años y en otra
   empresa, y es la parte que nadie hace.»* **Nombrar la meseta antes de llegar a ella es lo que la
   convierte en un tramo y no en un final.**
2. **El gancho de M5 no es metodológico, es de deseo: el número.** Ella quiere evidenciar valor —es su
   objetivo 5, formulado por ella— y **el número es la munición**.
3. **La lectura de la Tira completa como primera sesión de M5.** Cinco columnas de su propio trabajo, con
   fecha. A las doce semanas puede leer lo que en la semana 3 le parecía imposible. **Es la evidencia
   objetiva contra la ilusión de fluidez, y es gratis.**
4. **El hallazgo, y no el ahorro, se coloca en M6.** El doblete de P32 más el Mapa de los doce producen
   **una lista de errores reales que nadie en la academia sabía que existían** —precios del año pasado
   circulando en la plantilla alemana desde hace meses—. **Un hallazgo es mucho mejor combustible que un
   ahorro cuando quedan tres semanas.** *(Esta es la pieza que sustituye a la compresión de calendario de
   A: en vez de acortar la meseta, se le mete dentro algo que produce resultado enseñable.)*
5. **La cláusula del resultado decepcionante, escrita antes de medir**, con las razones legítimas
   alternativas enumeradas de antemano y la instrucción de **medir esa otra razón** si es la que importa.
   **La honestidad de la medición está protegida por adelantado, que es la única forma de que la medición
   sea honesta.**
6. **PC-5 exactamente en la frontera** (fin de M4). Una conversación de diez minutos sobre su propio
   criterio es el mejor combustible disponible donde el material solo ya no tira. Y el objeto —*«¿dónde
   moverías la línea de corte?»*— **es intrínsecamente halagador de su trabajo sin ser halago**: se conversa
   sobre criterio, que es lo que ya tiene.
7. **El compromiso externo de M7 se anuncia en M4, cinco semanas antes.** *«En la semana 17 una compañera va
   a usar esto una semana entera sin ti.»* **Un compromiso con fecha y con otra persona dentro es el
   mecanismo de permanencia más fuerte disponible en un curso sin cohorte**, y convierte M5 y M6 en
   preparación de algo que va a ocurrir.
8. **El orden de sacrificio de M5 y M6** deja explícito que **el número y el Mapa son el núcleo** y que todo
   lo demás puede correrse. En la meseta, saber qué se puede soltar sin romper nada es lo que impide
   soltarlo todo.

## MOMENTO 4 · El final sin final

**Qué pasa.** Se queda a dos módulos, sin evento que marque el fin, y el curso **se desvanece en vez de
terminar**. **Contramedidas:** la definición observable de «terminado» fijada en la semana 1 (§2.3) · **el
piloto de M7, que es el único evento externo del curso y tiene fecha** · **PC-6 como cierre con otra
persona** · y el calendario de revisión de M6, que fija **la próxima fecha** en que hay que volver a mirar
—lo cual convierte el final del curso en el principio de un mantenimiento, **que es la forma correcta de
terminar algo que tiene que seguir vivo**—.

## El modo mínimo y el ritual de reentrada, redactados en la semana 1

> **Modo mínimo.** Semana de pico o imprevisto: **una micro-sesión de diez minutos y nada más, y eso cuenta
> como semana cumplida.** Estar en modo mínimo no es fallar. El curso lo dice explícitamente y lo dice
> **antes** de que ocurra. Y en modo mínimo, lo que se hace es lo que diga el **orden de sacrificio** del
> módulo, no lo que apetezca.
>
> **Ritual de reentrada.** Toda vuelta tras una pausa empieza igual: leer las tres últimas entradas de la
> bitácora y responder las cinco preguntas de repaso. Diez minutos, y **elimina el coste de arranque, que es
> lo que convierte una pausa de una semana en el final**.
>
> **Intenciones de implementación, no propósitos.** «Si es martes y son las 9:15, abro el módulo»: fecha,
> hora y sitio escritos, no «esta semana».


---

# 14. DURACIÓN Y DEDICACIÓN REALISTAS

## 14.1 El contrato, tal y como se le entrega en la semana 1

> **18 semanas · 8 módulos · 2 horas propias por semana · 0 € · nada que instalar · nada que pedirle a
> nadie para empezar · arranque en octubre.**
> **Frontera declarada: al terminar M4, semana 11, ya hay curso.**
> **M7 es movible: si el piloto no cabe en la semana 17, ocurre en marzo y no pasa nada.**

## 14.2 El reparto por módulo

| M | Semanas | Nº sem. | Horas propias | Tiempo de trabajo | Por qué esa duración |
|---|---|---|---|---|---|
| **M0** | 1–2 | 2 | **~3 h 15** | sombra (3 min/día), embudo (55 min), cronometraje | **Deliberadamente ligero por semana: la mortalidad está aquí.** El grueso es un bloque de proyecto en horario de trabajo |
| **M1** | 3–4 | 2 | **~3 h 45** | línea de corte (45 min) | El más denso mentalmente y **el más ligero en clics de todo el curso**: casi todo es un documento. Se sostiene porque el asistente v1 ya funciona encima de la mesa |
| **M2** | 5–6 | 2 | **~4 h** | carga de fuentes, uso diario | Dos semanas justas. La segunda es casi toda uso real, que es lo que mide la puerta |
| **M3** | 7–8 | 2 | **~4 h** | montaje (90 min) + **la tarde de P27 (90 min)** | **El primer módulo con probabilidad real de desbordarse.** Por eso su orden de sacrificio deja fuera la ruta B y aplaza la portabilidad nº 2 |
| **M4** | 9–11 | **3** | **~5 h 30** | pruebas de parada | **El único módulo con aire antes del final**, y se dice por qué: es la frontera conceptual, es donde más gente se cae, **y es donde una puerta cerrada tiene que poder costar una semana sin romper el calendario** |
| **M5** | 12–13 | 2 | **~4 h** | la prueba ciega (una tarde) | Metodología pura. Dos semanas bastan porque no hay nada que montar |
| **M6** | 14–15 | 2 | **~4 h** | — | **La pasada 2 del Mapa son 60 min de una sola sesión**, y es lo que da a este módulo un resultado enseñable en plena meseta |
| **M7** | 16–18 | **3** | **~4 h 30** | la entrevista (20 min), el piloto | **Tres semanas por una espera que no depende de ella:** el piloto dura una semana natural y no se puede acelerar |
| PC | — | — | **1 h** | — | Seis consultas de diez minutos |
| | | **18** | **≈ 34 h** | ≈ 1 h/semana equivalente | |

**Los dos picos y la meseta, dichos por adelantado:**

| Tramo | Semanas | Carga propia | Nota |
|---|---|---|---|
| Arranque | 1–2 | ~1 h 40/semana | Deliberadamente ligero |
| Denso mental | 3–4 | ~1 h 55/semana | Casi todo documento |
| Construcción | 5–8 | ~2 h/semana | Aquí está el momento psicológico del curso |
| **Pico 1** | **9–11** | **~1 h 50/semana durante tres semanas** | M4. La tercera semana está presupuestada para una puerta cerrada |
| Meseta | 12–15 | ~2 h/semana | Novedad baja. Aquí están las ocho contramedidas del momento 3 |
| **Pico 2** | **16–18** | ~1 h 30/semana **+ una espera de una semana natural** | El piloto no se puede acelerar |

## 14.3 La declaración de tipo de tiempo, línea a línea

**Cada sesión del material declara arriba si es `[ tiempo propio ]` o `[ tiempo de trabajo ]`.** No es
cosmética: la primera causa documentada de abandono es el tiempo —21 de 34 abandonos [E]— y **sin esa
declaración escrita ella lo contabilizará todo como tiempo propio y el curso parecerá el doble de caro de
lo que es.**

Y el tiempo de otras personas también se declara, porque es un recurso y se agota: **barajar la prueba
ciega (5 min) · el piloto de M7 (una semana de uso real, sin supervisión) · los seis puntos de consulta
(1 h en total) = ~1 h 15 en dieciocho semanas**, más la semana del piloto.

## 14.4 Por qué 18 semanas y no 12, ni 17, ni 20

- **No 12:** con dos horas propias por semana, doce semanas no llegan a M5. **Un curso que termina antes de
  medir produce a alguien que ha automatizado algo y no sabe si sirve**, que es exactamente el perfil que su
  empresa ya tiene.
- **No 17** (la propuesta de A): la compresión se conseguía fundiendo medir y traspasar en un módulo de tres
  semanas, **lo que convierte el módulo menos gratificante del curso en el más largo, y justo en la
  meseta**. El objetivo de A —menos sitios donde el curso pueda leerse como terminado— se paga aquí por otra
  vía: la frontera declarada en M4 y el hallazgo colocado dentro de M6 (§13, momento 3, pieza 4).
- **No 20:** cada semana añadida al final es **una semana con menor probabilidad de ocurrir**, y el diseño
  de veinte semanas admite en su propia autocrítica que *«si ella se detiene en la semana 16 —que es
  exactamente donde se detiene la gente— nunca llega al escalón que corona el curso»*. **Dieciocho es el
  punto donde caben los dos objetivos finales sin empujar el cierre más allá de donde la gente llega.**
- **Y arranque en octubre, no en primavera.** El pico de junio–septiembre (250–400 correos al día, 60–90
  matrículas por semana) mata cualquier calendario que lo ignore; noviembre–febrero es su temporada baja. Si
  el curso empezara en primavera, **M4 —el módulo más caro— caería en julio.** Fin previsto: **última semana
  de febrero**, con margen antes de que el volumen empiece a subir.

## 14.5 Qué pasa si el calendario se rompe

- **Modo mínimo:** una micro-sesión de diez minutos **cuenta como semana cumplida**, y lo que se hace en
  ella lo decide **el orden de sacrificio del módulo**, no lo que apetezca.
- **Ritual de reentrada:** leer las tres últimas entradas de la bitácora y responder las cinco preguntas de
  repaso. Diez minutos.
- **M7 es movible por diseño y por escrito.**
- **Y la frontera:** parar en la semana 11 con un sistema funcionando **no es abandonar**. Está escrito desde
  la semana 1, y está escrito precisamente para que parar no se lea como fracaso, porque **un fracaso
  percibido no vuelve y una pausa declarada sí**.

---

# 15. PRUEBA DE DURABILIDAD A DOS AÑOS

**Procedimiento.** Recorrer el mapa suponiendo que en agosto de 2028: (a) los productos se han renombrado al
menos una vez —ya ocurrió tres veces en cinco meses de 2026 con la automatización nativa de la suite, el
cuaderno de fuentes y la herramienta de terminal [V]—; (b) algunas funciones se han movido de edición o han
desaparecido; (c) su empresa ha cambiado de proveedor, **o ella ha cambiado de empresa**.

## 15.1 Recorrido módulo a módulo

| Módulo | Qué es criterio (sigue válido en 2028) | Qué es clic (se rompe) | Coste de reparación |
|---|---|---|---|
| **M0** | El embudo y sus cinco columnas · **la cuarta columna como pregunta de permisos** · la prueba de la sombra y sus tres rechazos · describir por observación y no por introspección · **las cinco preguntas** · las cuatro preguntas que definen cualquier plan + la quinta · «la misma frase es segura o no según con qué cuenta entres» · «pagar resuelve quién es el proveedor, no qué tratamientos están amparados» · el semáforo · el estándar «no lo sé y lo pregunté» vale / «creo que sí» no · la lista de 32 procesos · los cinco motivos · **la tarjeta de siete casillas** | El distintivo concreto de la pantalla · las comprobaciones empíricas · la ruta de la consola · los mensajes literales · **el −3 concreto de la cuarta columna** | **1 fichero de clics + 1 línea de `datos-volatiles.md`.** El criterio no se toca |
| **M1** | La línea de corte y sus cinco motivos · **los seis veredictos y sus pruebas** · el escalón −1 · la ficha de criterio y su prohibición de palabras · las anclas conductuales · la muestra apartada · la tabla de especificaciones · el requisito multilingüe de la batería · el cebo como control positivo · el protocolo de siete reglas | **Nada.** Este módulo no tiene fichero de clics | **Cero** |
| **M2** | Fuente de verdad con **fecha y dueño** · citar como forma de abaratar la revisión · «no lo sé» exigible y probable · **las tres señas de la capacidad** · seudonimización y cuasi-identificadores · la prueba de la compañera **con su criterio del otro lado** · la regla de los adjuntos · el mapa de datos · **la regla multilingüe: fuentes en español, respuesta en el idioma de la persona** · el techo de la memoria | Dónde se guarda un asistente, cuántos ficheros admite, cómo se llama la superficie de fuentes | **1 fichero de clics + 1 línea de `tres-nombres.md`** |
| **M3** | Disparador por calendario frente a suceso · el tope · el apagado probado · «prepara, no envíes» y su motivo · «automatiza donde ya viven tus datos» · **la prueba del caso que NO debe disparar** · **las tres señas del disparador, incluida la del historial** · el libro de códigos · la doble codificación · la tabla de confusión · los umbrales por los dos lados · la notación neutra | Los límites concretos de la plataforma · el catálogo de pasos disponibles · cómo se escribe una clasificación en lote | **1 fichero de clics + la lista de seis comprobaciones**, que hay que reescribir con los límites de la plataforma nueva. **Es la reparación más cara del curso** |
| **M4** | Temas prohibidos frente a condiciones de parada · las seis condiciones y su motivo · **la parada por agencia con convenio** · **la parada por idioma no probado** · «parar no es callarse» · el revisor con nombre y hora · el plan de fallo en cinco pasos · «la confianza no es una salvaguarda» y el riesgo del día 60 · empatía sin admisión · privilegio mínimo · **las cinco preguntas aplicadas a un agente que no existe hoy** | Cómo se implementa una bifurcación y un tope · qué producto está detrás de qué plan · **las fechas del marco normativo** | **1 fichero de clics + la caja del fondo**, que se revisa entera —**está diseñada para eso: su primera columna son condiciones**— y `datos-volatiles.md` para las fechas normativas, que caducan más rápido que los productos |
| **M5** | Línea base · minutos por unidad · coste completo · las seis amenazas a la validez interna · proceso frente a resultado · cadena causal · prueba ciega · la lectura de la Tira | **Nada.** Es metodología, un cronómetro y una hoja de cálculo | **Cero** |
| **M6** | Fuentes con caducidad y dueño · calendario de revisión · apagado probado · la prueba del hueco · escribir la propia rúbrica y validarla contra un cebo · **el Mapa de los doce y la regla del cuatro** · la comprobación de las tres filas al azar | Los nombres de las herramientas del apéndice opcional | **1 párrafo** |
| **M7** | El número y su método · la reproducción ±10 % · «qué NO hace» · **la jerarquía de la evidencia** · la demo de tres minutos · la prueba del pasillo y sus cuatro binarias · **la semana sin ella** · la ficha de traspaso · las cuatro reglas de arranque · la deuda de adopción · la entrevista de proceso ajeno · **la lectura del delta** | **Nada** | **Cero** |

## 15.2 Recuento

| | Módulos | Proporción |
|---|---|---|
| **Sin nada que reparar** (M1, M5, M7) | 3 | 37,5 % |
| **Reparación de un fichero de clics o un párrafo** (M0, M2, M6) | 3 | 37,5 % |
| **Reparación media** (M4) | 1 | 12,5 % |
| **Reparación cara** (M3) | 1 | 12,5 % |
| **Módulos que habría que rediseñar** | **0** | **0 %** |

**Por instrumento:** las **cinco preguntas no caducan** —clasifican por una propiedad, no por un catálogo— ·
la **rejilla de los seis veredictos caduca parcialmente y de forma prevista** (§15.4) · la **Tira no
caduca** · el **Cuaderno de capas caduca en ocho líneas** —la línea de techo de cada ficha— por diseño · la
**Lista de techos no caduca porque su tercera columna son condiciones** · el **Expediente no caduca** —una
academia de idiomas en 2030 seguirá emitiendo cartas de visado y contestando leads— · y la **tabla de tres
nombres caduca entera**, y por eso está aislada en una sola página fechada.

**Veredicto: no hay que rediseñar.**

## 15.3 Cinco cosas que esta prueba obligó a cambiar, y que ya están incorporadas

1. **La cuarta columna del embudo se reformuló** de *«¿los ficheros que abro son míos o compartidos?»* a
   *«¿sobre qué recursos puedo actuar yo, no mirar, sin pedirle permiso a nadie?»*, **y el límite numérico se
   fue a clics.**
2. **Los módulos se titulan por capa y no por lo que se construye.** Un primer esbozo tenía módulos llamados
   «El asistente que cita» y «La columna que clasifica sola». Con eso, **medio índice del curso nacía
   caducado y —peor— el índice enseñaba lo contrario que el contenido.**
3. **Apareció el tercer registro.** Dos registros dejaban sin cubrir la habilidad que más falta va a hacer
   en 2029: **encontrar una función en una pantalla que no ha visto nunca.** La tabla de tres nombres no
   sirve para eso, por su propia declaración; las señas funcionales sí.
4. **La caja del fondo cambió de eje.** Antes listaba productos con una columna de «cuándo te tocaría».
   Ahora **la fila es la condición** y el producto es el ejemplo de hoy. Con el eje anterior había que
   rehacerla entera cada año; con este, se revisa.
5. **Las fechas normativas salieron del texto y se fueron a `datos-volatiles.md`.** **Lo que no cambia son
   los seis principios y la asimetría del Anexo III**, y eso es lo que se queda en el criterio.

## 15.4 Los tres escenarios de 2028, corridos de frente

**(a) ¿Y si un solo producto acaba haciendo todas las capas?** Es plausible: la tendencia es que la misma
ventana de chat programe, dispare por sucesos y actúe. Si ocurre, **este diseño no se rompe: se vuelve más
necesario**, porque **el producto deja de forzar la distinción y ya nada, salvo el criterio, le dice cuánta
autonomía acaba de ceder**. Las cinco preguntas se responden igual dentro de una sola ventana, y la Tira
sigue produciendo la misma lectura: *¿esto me cambia la calidad o me cambia el disparador?*

**(b) ¿Y si los modelos dejan de necesitar fuentes citadas?** No hace falta apostar. **M2 no enseña «cita
porque alucina»**: enseña **cita porque tu revisión tiene que durar cinco segundos y porque una fuente
caducada responde con toda la confianza del mundo**. Ese segundo motivo no depende de la calidad del modelo:
depende de que los tarifarios cambien, **y van a seguir cambiando**.

**(c) ¿Y si la partición de los seis veredictos pierde su referente?** Es la crítica más afilada del juez 3 y
hay que asumirla en vez de esquivarla: **los veredictos 4, 5 y 6 son fronteras de producto de hoy**, y el
día que una sola superficie haga las tres, tres de las seis casillas se quedan sin referente comercial. **Lo
que sobrevive entero es el 1, el 2 y la zona prohibida** — que es el tercio, y es el mejor tercio, porque es
el que contiene los dos noes. Tres decisiones lo mitigan: **las pruebas que deciden cada veredicto
interrogan la tarea, no la herramienta**, y esas preguntas no caducan aunque la casilla se renombre · **la
rejilla convive con las cinco preguntas**, que sí son dimensionales, de modo que si la partición se difumina
la clasificación no desaparece, se hace con el instrumento 1 · y **la revisión está prevista**: la lectura
del delta de M7 pregunta explícitamente *qué condiciones han cambiado*, y esa operación es la que ella
tendrá que repetir cada año, con o sin curso. **Es una mitigación parcial y se dice como tal.**

## 15.5 Lo que sigue siendo frágil aunque el diseño esté bien

Una prueba de durabilidad que sale limpia del todo es sospechosa. Cuatro cosas:

- **M3 es el punto débil y no tiene arreglo estructural.** La anatomía de un disparador es durable, pero
  **los límites concretos de una plataforma no son un adorno del módulo: son la mitad del módulo**, porque
  son lo que determina si su buzón compartido se puede tocar o no. Si cambia la plataforma, hay que volver a
  averiguar los límites, **y eso no se hereda**.
- **La rejilla de seis veredictos** es mitad clasificador y mitad foto del espacio de soluciones de 2026
  (§15.4c).
- **La lista de 32 procesos envejece despacio, pero envejece.** Una normativa de extranjería nueva, un canal
  de captación que desaparece, y hay filas que dejan de existir. Sigue siendo el activo más duradero del
  curso, pero **hay que fecharla como cualquier otra fuente**.
- **Y una asimetría incómoda:** **lo que menos caduca de este curso es lo que menos se parece a «un curso de
  IA»** —mirar un proceso, escribir criterios, medir, traspasar, contagiar— **y lo que más caduca es lo que
  más se parece**. Es la mejor prueba de que el listón está bien puesto, y también **la advertencia de
  producción más importante que deja este documento: el material tiene que trabajarse el enganche de M1,
  M5, M6 y M7 mucho más que el de M3.**

---

# 16. QUÉ SE QUEDA FUERA, A PROPÓSITO

## 16.1 Fuera porque el brief lo excluye

| Fuera | Por qué |
|---|---|
| **«Cómo conseguir el sí», venta interna, argumentarios, plantillas de petición a dirección** | En su empresa usar IA ya está bien visto y **lo mal visto es no automatizar**. Un módulo de permiso resuelve un problema que ella no tiene. Lo que sí entra —evidenciar y contagiar— es otra cosa y está en M7 |
| **Portfolio, landing, prototipo de app, «lo que tengo ahora en mi CV»** | Es el destino del itinerario no técnico de la referencia porque **su alumno tipo quiere entrar en el sector de la IA**. La nuestra no quiere cambiar de rol ni de sector. Lo que sí quiere —que le sirva si cambia de empresa— **lo dan los seis instrumentos permanentes, no una web** |
| **Certificado, insignia, «ahora eres AI Operator»** | No busca cambiar de rol. Y un certificado sin evaluador y sin rúbrica no certifica nada. **La definición de «terminado» de §2.3 es observable y no la firma nadie** |
| **Convertirse en especialista en IA** | El objetivo es trabajar mejor en lo suyo. Todo lo que empuje hacia «ser la persona de la IA» como identidad profesional está fuera, **incluido el vocabulario** |
| **Cualquier cosa vistosa** | El grafo de la referencia es el caso de estudio: espectacular en pantalla, marginal en valor para atención al cliente, y —dicho por su propia autora— *hecho para el agente, no para el humano*. **Aquí el artefacto útil es aburrido**: un asistente que cita, un triaje que etiqueta, un vigilante que avisa |
| **Construir y vender aplicaciones** | Ni siquiera la referencia lo promete: *«construir algo para uso interno y publicarlo en internet son dos mundos distintos»* |
| **Coleccionar herramientas** | Dos o tres capacidades nuevas en dieciocho semanas, y **ninguna antes de haber agotado la anterior** |

## 16.2 Fuera por el listón de durabilidad, con su condición de reentrada

**Un «no» sin condición de revisión es dogma.** Todo lo que sale tiene su fila en la Lista de techos o en la
caja del fondo, con la condición que lo devolvería.

| Fuera | Reducido a | Condición para que entre |
|---|---|---|
| **Plataformas de automatización externas como módulo** | Una fila de la caja del fondo + el criterio *automatiza donde ya viven tus datos* | Que su proceso tenga que actuar sobre algo fuera de su suite. Y una que haya que autoalojar, **solo si aparece alguien técnico que la mantenga** |
| **Escribir código, aunque lo escriba la IA** | Media página informativa | Que la automatización nativa se quede corta **y** haya quien mantenga el script. **En el momento en que falla hay que leer un error de programador, y esa es una dependencia que ella no puede cubrir** |
| **La superficie de desarrollador «gratis y de la misma empresa»** | Cinco líneas, con aviso explícito | **Ninguna.** Es la trampa más silenciosa del panorama y por eso se nombra: parece profesional, se entra con la cuenta de siempre, y **sus términos dicen literalmente que no metas información personal** |
| **Conectores y su estándar, como práctica** | Vocabulario + el principio de privilegio mínimo | Que monte algo fuera de su suite, o que alguien se lo configure y ella solo lo use |
| **Arquitecturas de recuperación sobre corpus grandes** | Una fila de la caja del fondo | Que las fuentes pasen de decenas a cientos y el asistente empiece a perderse |
| **Herramientas agénticas de escritorio y de terminal** | Un apéndice de lectura, opcional, **sin entregable** | Una tarea que exija procesar decenas de ficheros locales de forma repetida. **Si termina el curso sin abrir el apéndice, el curso ha funcionado igual**, y eso va en su primera línea |
| **Comparativas, nombres de modelo, benchmarks** | Nada | **Ninguna.** *«Da bastante igual qué modelo uses mientras no gastes miles en tokens.»* Es el detalle que menos importa y el que más rápido caduca |
| **Tour por los productos de su suite** | Nada | Solo entra lo que su proceso pide o lo que una fila de la rejilla pide. El resto, ni mencionado |

## 16.3 Fuera por rigor mal invertido — el bloque específico de este perfil

**El riesgo de esta alumna no es quedarse corta de rigor: es pasarse.** Un solo proceso es un imán para el
perfeccionismo. La regla que lo contiene se repite en cada módulo: **el montaje se hace rápido y sucio; el
rigor se gasta entero en la evaluación.**

- **Estadística inferencial.** Nada de significación, valor p ni tamaño muestral sobre doce casos. Aquí no se
  estima un parámetro poblacional: **se comprueba la cobertura de un instrumento contra un criterio
  fijado**. **Doce casos bien elegidos valen más que doscientos al azar.**
- **Consistencia interna aplicada a la batería.** Directamente incorrecto: **una batería debe ser
  heterogénea.** Si tuviera consistencia interna alta sería porque está mal construida.
- **Consentimiento informado como equivalente de base jurídica**, y **anonimato de investigación como
  equivalente de anonimización.** Son falsos amigos con consecuencias, y se cortan explícitamente.
- **Prompt engineering como colección de trucos.** El curso enseña **el criterio antes del prompt**. Un
  prompt bueno que se escribe una vez y se pierde no vale nada; el mismo guardado con sus fuentes es
  infraestructura.
- **Vídeos de lección.** Un vídeo es relectura con mejor producción, y la relectura es técnica de utilidad
  baja. Si hay vídeo, es demostración de una interfaz, dura menos de tres minutos, va con transcripción **y
  vive en la carpeta de clics**.
- **Resúmenes de la lección al final.** El resumen lo escribe ella y es un entregable: **la pregunta fija.**
- **Cualquier ejercicio de metodología sin artefacto reutilizable.** Si un ejercicio le lleva más de lo que
  le llevaría hacer la tarea a mano durante un mes, **está mal calibrado y se recorta**.
- **Y todo mecanismo de corrección que no pase el techo del 20 % ni la regla de retirada** (§12.1.1). Es la
  aplicación más incómoda de este apartado, porque recorta cosas buenas: **un mecanismo bueno de más es tan
  dañino como un mecanismo malo**, y en un curso de dos horas semanales lo es más.
- **La estructura de cinco semanas con cuatro lecciones semanales de la referencia.** Asume cohorte, LIVEs y
  mentores. Aquí el ritmo lo pone una jornada completa y el pico de julio.

## 16.4 Fuera por riesgo, con nombre y número

**P08** visados · **P26** quejas formales · **P29** emergencias · **P25** reembolsos · **P17** matching ·
**P22** calendario de camas · **P05/P16** nivelación y exámenes. **No son «temas avanzados»: son zona
prohibida con motivo escrito** (§9.3), y **el motivo es el contenido**, porque es lo único que se transfiere
a un caso nuevo.

## 16.5 Fuera por decisión propia de este diseño, y son las tres discutibles

1. **La segunda automatización.** El curso construye **una** cosa. No hay un segundo proceso ni un hilo
   guiado paralelo; el expediente modelo se lee y se usa como clave, **con la única excepción declarada de la
   tarde de P27** (§6.4.1), que son noventa minutos y existe precisamente para recuperar lo que renunciar al
   doble hilo cuesta. Con dos horas propias por semana, **dos procesos son dos procesos a medias**. El
   segundo proceso es lo primero que hará **después** del curso, y para eso están la cola ordenada del Mapa,
   la Lista de techos, su propia rúbrica y la ficha de traspaso.
2. **El inventario de once columnas como columna vertebral.** Se sustituye por el tachón de los 32 en M0 y
   el Mapa de los doce con sus dos pasadas, que producen **más volumen de juicios** sin cuatro semanas de
   documento árido en el tramo de máxima mortalidad.
3. **La ordenación del curso por la escalera de herramientas.** La escalera se respeta como progresión (§7)
   pero **no gobierna el índice**, porque ordenar por autonomía cedida obliga a subir aunque su realidad
   operativa no llegue a esa altura, y deja el muro del buzón compartido para la semana 9. **Lo que sí se
   toma entero de ese diseño son sus instrumentos: las cinco preguntas, las puertas y el tercer registro.**


---

# 17. AUTOCRÍTICA

Sin esta sección, las dieciséis anteriores no son creíbles. Y hay un motivo extra para escribirla: **la
arquitectura que sirve de columna vertebral citaba una sección de autocrítica que no existía en el fichero,
siete veces, y siempre para aplazar precisamente los límites de sus propios mecanismos.** Ese hueco no se
hereda. Ordenada de más grave a menos.

**1 · La calidad sustantiva de su ficha de criterio y de su batería no la comprueba nada, y es el defecto
compartido por todo el corpus.**
Ella escribe la ficha de criterio, ella escribe los diez casos, ella escribe la clave. **Puede escribir
cinco indicadores observables e irrelevantes y pasar todos los filtros**: el Ctrl+F, la prueba de tamaño, la
muestra apartada. El único parche que existe es *«al menos un indicador verificable contra fuente externa;
si todos son críticos, no ha priorizado»*, y **es poco**. **Nadie le va a decir que está midiendo lo que no
importa.** La prueba ciega de M5 lo detecta a medias y once semanas tarde. Los once contrastes con clave
—tres motivos de descarte y ocho dobletes— **no cubren esto**, porque son sobre procesos ajenos y este fallo
es sobre el suyo.

**2 · La cuota de cuatro en el Mapa depende de su honestidad consigo misma, y no hay forma de
comprobarla.**
Se han apilado tres capas —descartes aritméticos, motivos tipificados contra lista cerrada, y cuota que
excluye las zonas prohibidas— y sigue siendo cierto que **las cuotas producen cumplimiento de cuota**. La
señal de fallo que va de frente —*«existe un veredicto 1 o 2 que puse para llegar a cuatro»*— depende de que
ella se conteste con sinceridad, sin nadie que compruebe. **La única mitigación real es que la cuota de los
dobletes sí tiene clave**, y ahí un «no» de conveniencia se detecta. En el Mapa, no.

**3 · El pretest de la semana 1 está contaminado por diseño, y el delta mide menos de lo que parece.**
La tarjeta de siete casillas (§4.2.2) resuelve que el pretest sea interpretable, pero **no lo hace limpio**:
en la semana 1 ella ya ha visto la rejilla en forma de definiciones, y en la 14 la ha aprendido con sus
pruebas. **El delta mide lo que el curso añade sobre una definición leída, no lo que añade sobre el estado
natural.** Es la lectura correcta y va escrita en el material, pero conviene no venderlo como más de lo que
es: **es una medida de mejora dentro de un instrumento, no una medida de criterio en abstracto.**

**4 · Sigue pidiéndole comprometerse con un proceso en la semana 1.**
Todo el aparato de §5 —sombra, repuesto, divorcio con aritmética, embudo vacío, puerta de dos condiciones—
**acota la ansiedad; no la elimina**. Es el riesgo estructural del ángulo y se paga por elegirlo.

**5 · El problema del buzón compartido está prevenido, no resuelto.**
La cuarta columna lo cobra en la semana 1 y la escalera de relajación ofrece cinco salidas. Pero **la salida
1 —pedir que le deleguen una etiqueta o carpeta propia— es una petición a otra persona, que es exactamente
lo que el diseño prometía no necesitar**, y la salida 4 acota el proceso a un trozo más pequeño, que es una
rebaja real aunque se haya presentado como neutra. **Nadie ha resuelto esto y este documento tampoco:** lo
que hace es que se descubra cuando cuesta diez minutos en vez de seis semanas.

**6 · El módulo de adopción tiene la autocorrección más débil, y su criterio de éxito no lo controla ella.**
El piloto es binario y se provoca en vez de esperarse, que es lo mejor disponible. Pero si su compañera no
lo usa, hay al menos cinco explicaciones y el material no da forma infalible de distinguirlas. **Y hay un
modo de fallo que no se cubre: que el piloto ocurra por cortesía —lo usa porque es ella— y el resultado sea
un falso positivo.** La única mitigación es que el entregable no sea el veredicto sino la lista de arreglos,
y **es una mitigación indirecta**. Es el único punto del curso donde una alumna diligente puede hacerlo todo
bien y salir sin saber si lo hizo bien.

**7 · El monocultivo está mitigado, no eliminado, y hay una contradicción real en el diseño.**
La tarde de P27 recupera la doble codificación, la tabla de confusión, el oráculo externo y la práctica
multilingüe con independencia del hilo. Pero **si su proceso no toca datos ámbar ni rojos —y el embudo puntúa
+2 a «solo verde», es decir, empuja precisamente hacia ahí—, el mapa de datos de M2 sale flaco y la lección
de protección de datos se queda más abstracta de lo que debería.** **Es una contradicción real: el filtro
que protege el arranque es el mismo que empobrece una de las lecciones.** La mitigación —el ejercicio del
semáforo sobre diez correos reales suyos, que **sí** contienen ámbar y rojo, y la exigencia de declarar uno
**no reescribible**— es buena, pero es un ejercicio, no el proceso.

**8 · La agnosticidad se demuestra con poco más de una hora contra treinta y cuatro.**
Tres pruebas de portabilidad (25 + 20 + 20 min), ocho preguntas fijas con su mitad de herramienta, el
registro de señas en cada lección. Es lo mejor que cabe en un curso de dos horas semanales, y **la
proporción no tranquiliza**. Y las tres pruebas **nunca tocan la parte difícil**: P1 va con material verde
porque no puede ser de otro modo, y P2 y P3 son sobre papel. **Se demuestra que el criterio viaja; no se
demuestra que ella sabría trabajar de verdad en otra herramienta con datos reales.** Hay que llamarlo por su
nombre.

**9 · La Tira es la mejor idea del conjunto y la más frágil de mantener.**
Exige sostener diez casos vivos durante dieciocho semanas y volver a pasarlos cuatro veces. Es poco trabajo
cada vez —media hora— pero es **trabajo sin novedad**, y lo que no tiene novedad se convierte en ritual o
desaparece. Dos puertas la fuerzan, **pero las puertas se pueden saltar en un curso sin profesor**. Si la
Tira se erosiona, **desaparece con ella la lección central del curso** —*la calidad se gana en la capa 1 y
la capa 2; lo demás cambia quién dispara*— y no hay sustituto.

**10 · El Mapa de los doce, pasada 2, cae en la semana 14 y puede ser lo primero que se salte.**
Es el precio de haberla movido: en la semana 3 es un muro **pero ocurre**; en la 14 no es un muro **pero
puede no llegar a hacerse**. Las contramedidas —que sea núcleo del orden de sacrificio de M6, que su salida
alimente directamente el dossier de M7, y que el pretest de la semana 1 ya esté hecho y pedir el delta cree
presión de cierre— son razonables, **pero no son una garantía**.

**11 · El techo del 20 % y la regla de retirada son piezas nuevas y no están probadas.**
Son la respuesta a una pregunta que ni A ni B contestan, y son coherentes con lo que el curso enseña sobre
instrumentos. Pero **la regla de retirada se puede usar como coartada**: «este mecanismo no me ha cambiado
nada» es exactamente lo que dirá alguien cansada que quiere saltárselo. La protección —la lista de
excepciones no retirables, y que la retirada haya que escribirla en la bitácora— **es débil**, y si el
diseño falla por algún sitio nuevo, va a fallar por aquí.

**12 · El curso le pide a la vez que use la IA como correctora y que no se fíe de ella.**
Tres cebos, siete reglas de protocolo y una tabla de calibración por entregable es lo mejor que hay. Está
resuelto en el papel; **no se sabe si está resuelto en el mes cuarto, un jueves, cansada**. Y un dato que
conviene tener escrito: **no existen datos publicados sobre cómo se comporta un modelo de 2026 corrigiendo
un entregable contra una rúbrica dada**, que es exactamente nuestro caso. **Los tres cebos no son un adorno:
son lo único que tenemos**, y puede resultar que la respuesta sea *«para este tipo de trabajo, la IA no
corrige»*.

**13 · El módulo de adopción puede volverse en su contra, y la contramedida es de una página contra una
dinámica organizativa.**
En una empresa de treinta personas donde lo mal visto es no automatizar, **hacerse visible como «la que sabe
de IA» tiene un desenlace previsible: que le caiga trabajo ajeno**. Está escrita la contramedida —entregar el
artefacto y el manual, no el servicio; la frase de límite; el bus factor invertido— **y las dinámicas
organizativas suelen ganar a las contramedidas de una página.**

**14 · Nada de esto se ha visto.**
Los 32 procesos, los volúmenes, el buzón compartido, la carpeta de plantillas con seis versiones: **todo es
reconstrucción [R]** a partir del sector, no observación de su empresa. El curso está diseñado para que **su
primera tarea sea tachar y corregir** ese mapa, que es la única forma honesta de convertir una
reconstrucción en su realidad. **Pero si el mapa está muy equivocado, M0 habrá que reescribirlo sobre la
marcha y varios ejemplos perderán fuerza precisamente por lo que se supone que los hace fuertes: por ser
concretos.**

**15 · Y el dato del que depende medio diseño sigue sin conocerse [NV].**
Qué plan tiene contratada su empresa y cómo está configurado. De ahí depende qué versión de M3 se ejecuta, si
la clasificación en lote tiene ruta cómoda o incómoda, y si la automatización por sucesos existe para ella.
Hay contingencia escrita —la regla de independencia de plataforma, la ruta A obligatoria— **pero una
contingencia no es lo mismo que un diseño**, y no se sabrá hasta la semana 2, con el curso ya escrito.

---

# 18. DECISIONES DEL ÁRBITRO

Cada tensión entre A y B, qué opción ganó y por qué. La última columna dice **cuál de las dos restricciones
—llegar al final / que le dure— pagó la decisión**, porque el encargo prohíbe sacrificar cualquiera de las
dos y hay que poder auditar que no se ha hecho.

## 18.1 Las quince discrepancias

| # | Tensión | Gana | Por qué | Restricción que la decide |
|---|---|---|---|---|
| **1** | **Duración: 17 sem./7 módulos (A) vs 18 sem./8 módulos (B)** | **B** | La fusión de A convierte el módulo **menos gratificante** del curso en el **más largo**, y justo en la meseta; empujó una pieza al módulo siguiente «para que quepa»; y **la propia autocrítica 4 de A la declara «la decisión con menos respaldo del documento» y señala la costura por si hay que soltarla**. El objetivo legítimo de A —menos sitios donde el curso pueda leerse como terminado— **se paga por otra vía**: frontera declarada en M4 y un hallazgo (P32 + el Mapa) colocado dentro de la meseta | Las dos: acortar así **no** habría mejorado la continuidad y **sí** habría comprimido criterio |
| **2** | **Clasificación panorámica: pretest de 12 en la semana 1 (A) vs rejilla justificada de 12 en la semana 14 (B)** | **Las dos** | **Están hablando de dos instrumentos con el mismo nombre.** Una clasificación de 20 min sin justificar **es una medida** y tiene que ir antes de la intervención; una clasificación justificada **es entrenamiento** y tiene que ir después del criterio. Ninguna de las tres facturas que B factura al inventario se paga aquí, porque el pretest **no gobierna el orden de nada** y está declarado equivocado | Las dos, y **es la síntesis más rentable del arbitraje**: 20 minutos compran el objetivo 4 hecho observable |
| **3** | **Puertas: tres (A) vs seis (B)** | **Cuatro** [J] | Ninguno de los dos escribe **el criterio** de qué justifica bloquear. Este documento lo escribe: bloquea solo donde **(a)** se construye encima, **(b)** el error se multiplica y **(c)** deshacerlo es caro. Salen cuatro, **y las cuatro caen en la primera mitad**: de M5 en adelante no hay cimientos, hay consecuencias. La de M0→M1 se añade contra A pero **reducida a dos condiciones**, porque está en el tramo de mortalidad | Equilibrio explícito: bloquear donde el error se multiplica (criterio), no bloquear donde solo se para (continuidad) |
| **4** | **Asistente v1: día 4–5 (A) vs día 3 (B)** | **Día 4, con la razón de B** | La razón de B es mejor —lo que decide si esa caja funciona es **el diagnóstico del entorno**, no el embudo— pero su día es peor: el día 3 ya carga 75 min entre embudo y Mapa, y **añadir ahí la pieza más frágil del módulo es lo que no hay que hacer en la semana de máxima mortalidad**. Día 4: el premio grande sigue dentro de la semana 1 y llega con **dos redes debajo** | Continuidad, sin coste de criterio |
| **5** | **Motivos tipificados: lista de cinco (A) vs tres + uno con nombre + uno aparte (B)** | **A** | Cubren lo mismo, pero **B produce dos listas parecidas para la misma operación**. Una lista usada en cuatro sitios se aprende; dos listas parecidas se confunden | Criterio: un instrumento uniforme es lo que viaja |
| **6** | **Cuota de noes: cuatro de doce sin contar ZP (A) vs contándolas (B)** | **A** | Las ZP se resuelven **por número de proceso, sin juicio y sin coste**. Si contaran, la cuota se cumpliría sola. Excluyéndolas, **los cuatro tienen que salir de los veredictos que exigen juicio** | Criterio |
| **7** | **Dobletes: siete (A) vs ocho (B)** | **Ocho** + el mini de P16 que aporta A | Ocho módulos son ocho cierres de capa. Y P16 —«las reglas son de otro»— **es el único sitio del curso donde aparece un motivo de «no» que no es ni de riesgo ni de datos**, y cuesta diez minutos | Criterio |
| **8** | **La tarde de P27: obligatoria (A) vs contingente (B)** | **A** | **Un mecanismo contingente no está en el diseño.** Si su proceso incluye lote, la ruta de respaldo no se ejecuta; si no lo incluye, llega como parche. En los dos casos **el mejor mecanismo de nivel 1 para juzgar un clasificador queda a merced de la suerte**. Y es el único sitio donde ella **compara su propio juicio contra una clave que no ha escrito** sobre algo que ha hecho de verdad | Criterio, y a coste de 90 minutos |
| **9** | **Multilingüe en la batería: un caso (A) vs un típico y un límite (B)** | **B** | Cuesta cero y cierra el hueco por los dos lados: un sistema que traduce bien lo fácil y se rompe en lo ambiguo **está sin probar** | Criterio, coste cero |
| **10** | **Cuarta columna del embudo: dos formulaciones del mismo arreglo** | **Redacción de B, reparto de A** | La redacción de B —*«¿sobre qué recursos puedo actuar yo, no mirar, sin pedir permiso a nadie?»*— **es la pregunta 4 de las cinco preguntas aplicada a su propia cuenta**, y hace que la primera vez que use el instrumento número uno lo use sobre sí misma. El reparto de A pone el límite numérico y el −3 en `datos-volatiles.md`, fechados | Las dos: previene el muro (continuidad) sin meter un bug de 2026 en la mitad que no caduca (criterio) |
| **11** | **Embudo vacío: tres salidas (A) vs escalera de cuatro pasos con precio (B)** | **Escalera de B + plazo de A** | La escalera de B está mejor ingenierada —**precio declarado en cada paso y dos columnas que no se relajan nunca**— y el plazo de A es el que la hace operativa: **se resuelve el día 3, no la semana 6** | Continuidad |
| **12** | **Descarte de los seis: por número (A) vs con motivo escrito (B)** | **Híbrido** [J] | El descarte es **automático y por número** —eso protege la semana 1 y garantiza que los seis peligrosos salgan sí o sí— y **después**, en diez minutos, escribe el motivo de **tres** y **abre la clave**. Tres y no seis porque el rendimiento marginal del cuarto es bajo y el coste emocional de la semana 1 no lo es. **Y con clave, porque un motivo sin oráculo es una frase** | Las dos, y es la respuesta operativa a «cuánto rigor en la semana 1» |
| **13** | **La Tira: seis columnas (A) vs cinco (B)** | **B** | Es el instrumento con más riesgo de convertirse en ritual. **Una pasada menos es una ocasión menos de que se erosione**, y con capas 1–4 más el estado inicial ya se lee la curva entera | Continuidad, sin coste de criterio |
| **14** | **Instrumentos permanentes: Mapa dentro (A) vs rejilla dentro (B)** | **B** | Es un error de categoría: **la rejilla es un instrumento y el Mapa es un momento de uso.** Meter el momento y dejar fuera el instrumento produce un cuaderno con dos entradas para lo mismo | Criterio |
| **15** | **Nombre: «Un proceso tuyo, de punta a punta» (A) vs «Delegar bien» (B)** | **B** | Nombra **la operación** y no solo el objeto, y su subtítulo anuncia las dos mitades del encargo en una línea. Y el de A **llevaba el número de capas dentro del título**: un título que hay que reescribir si el mapa cambia de siete a ocho módulos está mal construido | Criterio |

## 18.2 Las cuatro piezas nuevas, y qué pregunta del encargo contesta cada una

| Pieza | Pregunta que contesta | Qué hace |
|---|---|---|
| **El orden de sacrificio por módulo** (§6.0.1) | *Cuánto rigor sin perderla* | Cada módulo declara **el núcleo que no se cae nunca**, el **orden** en que se cae lo demás **con la semana a la que se aplaza**, y **la versión reducida** de cada pieza aplazable. Ni A ni B lo tienen, y sin él **en una semana mala se cae lo que más enseña**, porque es lo que más cuesta |
| **El techo del 20 % y la regla de retirada** (§12.1.1) | *Cuánta autocorrección antes de que sea burocracia* | Un mecanismo dominante y un respaldo por entregable · **el aparato de corrección no pasa del 20 % del tiempo propio del módulo** · nada se comprueba dos veces · y **un mecanismo que en tres usos no ha cambiado ninguna decisión se retira**, salvo puertas, claves, cebos y la resta. Las dos síntesis **acumulan** mecanismos y ninguna escribe el límite |
| **La tarjeta de siete casillas** (§4.2.2) | *En qué momento se construye el catálogo* | Hace **interpretable el pretest de la semana 1** sin quemar el módulo donde se enseña la rejilla: clasifica con **definiciones**, no con criterio, y el delta mide exactamente lo que el curso añade sobre una definición leída |
| **El criterio de qué justifica una puerta** (§12.3) | *Cuánto rigor / cuánta autocorrección* | Bloquear solo donde **(a)** se construye encima, **(b)** el error se multiplica y **(c)** deshacerlo es caro. Resuelve el 3 contra 6 con un principio en vez de con un promedio |

## 18.3 Las cuatro preguntas del encargo, contestadas en una línea cada una

**1 · Duración total y reparto por módulo.** **18 semanas, 8 módulos**, 2 h propias por semana, ≈34 h en
total. Reparto: 2+2+2+2+**3**+2+2+**3**. Las dos excepciones de tres semanas son **M4** —porque es la
frontera conceptual y porque **una puerta cerrada tiene que poder costar una semana sin romper el
calendario**— y **M7** —porque contiene una espera de una semana natural que no depende de ella—. Arranque
en octubre, fin en la última semana de febrero. Tabla completa en §14.2.

**2 · Cuánto rigor en las primeras cuatro semanas.** **Solo se admite rigor que cumpla las tres: se ejecuta
sobre algo que ya funciona o que ella ya hace · tiene corrección mecánica, no de juicio · y cabe en menos de
treinta minutos por pieza.** En números: **1 h 50 la semana 1, 1 h 25 la semana 2, ~1 h 55 las semanas 3 y
4.** Lo que sí entra en ese tramo porque cumple las tres: la sombra (3 min/día, corrección por tres criterios
observables), el embudo (aritmético), el pretest del Mapa (declarado equivocado), la batería sellada, el
Ctrl+F, la muestra apartada. Lo que **no** entra: la clasificación justificada de doce procesos, cualquier
rúbrica que duplique una lista, y la ficha de cinco preguntas sobre una herramienta ajena. Y sobre todo:
**cada módulo lleva escrito su orden de sacrificio antes de empezarlo**, porque el rigor que se puede pedir
no es un número fijo — **es un núcleo innegociable más una cola aplazable con fecha**.

**3 · Cómo se construye el catálogo de «qué existe».** **Por los tres, en tres momentos y con tres funciones
distintas** (§9.1): **por descarte** en la semana 1 —seis descartes por número más tres motivos contra
clave—, porque es la única clasificación que se puede hacer bien sin criterio; **por veredictos** a lo largo
de todo el curso —cuarenta y tantos juicios, con la clasificación **sin justificar** en la semana 1 como
medida y la **justificada** en la semana 14 como entrenamiento—, porque justificar antes del criterio es
adivinar; y **por techos**, una fila al cerrar cada capa, porque **el catálogo se genera desde la carencia
sentida y su tercera columna son condiciones, que no se renombran**. Más **la caja del fondo**, una sola vez,
en M4. **Y por eso no hay módulo de panorama**: un catálogo leído en la semana 2 se olvida en la 4; uno
generado en ocho trozos, cada uno el día que hizo falta, se recuerda porque **cada fila tiene una anécdota
propia detrás**.

**4 · Cuánta autocorrección antes de que sea burocracia.** **Un mecanismo dominante y como mucho un respaldo
por entregable · techo del 20 % del tiempo propio del módulo · nada se comprueba dos veces · y todo mecanismo
que en tres usos no ha cambiado ninguna decisión se retira y se anota** (§12.1.1). **Y solo cuatro cosas
bloquean**; el resto avisa. Aplicando la regla, este diseño **retira** cuatro piezas que A o B tenían: la
rúbrica de ocho ítems sobre la ficha del entorno, la comprobación de las tres filas al azar sobre el
pretest, la sexta columna de la Tira y el contraste rutinario de dos modelos. **Y lo que no se toca nunca,
porque su valor no está en cambiar una decisión cada vez sino en existir el día que haga falta: las cuatro
puertas, las claves selladas, los tres cebos y la resta de M5.**

## 18.4 Dónde este documento se aparta de las dos síntesis a la vez

Cuatro sitios, y conviene tenerlos localizados por si hay que soltar alguno:

1. **Cuatro puertas.** Ni tres ni seis. Con criterio escrito, y con una puerta añadida en M0→M1 que **ninguna
   de las dos pone** — reducida a dos condiciones porque cae en el tramo de mortalidad.
2. **El descarte híbrido de la semana 1**: automático por número, y después tres motivos **con clave**.
3. **El techo del 20 % y la regla de retirada**, que recortan mecanismos que las dos síntesis consideraban
   buenos. **Es la decisión más incómoda del documento**, porque quita cosas que funcionan.
4. **El pretest con tarjeta de definiciones**, que hace compatibles las dos posiciones sobre el Mapa a costa
   de asumir que el delta está contaminado y decirlo (§17.3).

## 18.5 La costura que se puede soltar

Si al producir el material algo no cabe, **la costura correcta es esta y no otra**: **M7 se parte en dos**
—dossier y demo en la semana 16; piloto, entrevista y delta cuando la agenda de la compañera lo permita—
aceptando que el curso dure diecinueve o veinte semanas **de calendario** sin durar más **de trabajo**. Es la
costura correcta porque **M7 ya está declarado movible desde la semana 1**, porque no abre ninguna puerta y
porque su espera no depende de ella. **Lo que no se debe soltar, en ningún caso, es la tarde de P27, la
pasada 2 del Mapa ni la puerta de uso espontáneo**: son las tres piezas que compran, respectivamente, el
oráculo externo, el objetivo 4 y la verdad de la tesis entera.
