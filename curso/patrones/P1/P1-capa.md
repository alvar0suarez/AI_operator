# Patrón 1 · La pregunta repetida

```
================================================================================
 Semanas 3 y 4 · ~2 h de tiempo propio · escalón: usar mucho mejor el chat
 Lo que montas: un asistente que responde con TUS fuentes, cita de dónde sale
 cada dato, y sabe decir «no lo sé».
================================================================================
```

## 1 · Qué es, y cómo se reconoce

**Alguien pregunta algo cuya respuesta ya está escrita en algún sitio.**

Es el patrón de más volumen de tu profesión y el que menos se mira, porque cada
mensaje suelto parece trivial. Lo que no es trivial es que sean seis mil al año.

**Las tres señas:**

1. **Se repite.** No una pregunta parecida: la misma, con otras palabras.
2. **La respuesta existe y está escrita**, aunque esté repartida en tres documentos.
3. **La respuesta es estable.** Cambia con el tarifario, no con quien pregunta.

**Si las tres se cumplen, es este patrón.** Y si falla la segunda —la respuesta no
está escrita en ningún sitio— **no es este patrón y no hay nada que automatizar
todavía**. Eso se trata en la sección 4.

### La seña que lo distingue del patrón que se le parece

Este patrón se confunde constantemente con el **patrón 3, el texto que hay que
redactar con reglas**. Los dos acaban en un correo que sale a una persona. La
diferencia está en **dónde está la dificultad**:

| | **Patrón 1 · la pregunta repetida** | **Patrón 3 · redactar con reglas** |
|---|---|---|
| Dónde está la dificultad | **Encontrar el dato correcto** entre tus documentos | **Cómo decirlo**: tono, orden, qué se calla |
| Si te doy el dato | El problema está resuelto | El problema sigue entero |
| Qué se rompe si falla | Dice un precio que no es | Suena mal, promete de más, o hiere |
| Cómo se comprueba | **¿La cifra coincide con la fuente?** | ¿Un compañero lo habría mandado así? |

> **La prueba, en una frase:** *si te dieran la respuesta correcta escrita en un
> papel, ¿ya estaría resuelto?* Si sí, es el patrón 1. Si aún tendrías que pensar
> cómo decirlo, es el 3.
>
> Y muchos mensajes son **los dos, en este orden**: primero encuentras el dato,
> después lo redactas. Está bien que sean dos: **se montan por separado y se
> comprueban por separado**, y así cuando algo falla sabes cuál de los dos falló.

---

## 2 · El caso de Meridiano

Abre `meridiano/buzon.md`. De los cuarenta mensajes, **una parte grande es este
patrón**: preguntas cuya respuesta está en el tarifario, en el calendario o en las
condiciones de alojamiento.

Y hay **cuatro que parecen este patrón y cuya respuesta no está en ninguna
fuente**. No te digo cuáles. Encontrarlos es la mitad del ejercicio, y es lo que
separa un sistema en el que puedes confiar de uno que responde siempre.

---

## 3 · Qué solución le toca, y por qué

**Un asistente guardado con fuentes propias.** El escalón 1 de la escalera: sigues
usando un chat, pero deja de empezar en blanco.

Tres cosas lo definen, y las tres son exigibles:

### (a) Fuentes propias, no lo que el modelo sepa del mundo

Le das **tus documentos** y le exiges que responda **solo** a partir de ellos. Un
modelo sabe muchísimo sobre academias de idiomas en general, y todo ese
conocimiento es exactamente lo que no quieres: **produce respuestas plausibles y
falsas**, que son las peores que existen porque no se detectan leyendo.

### (b) La regla de la primera línea

Todo documento que uses como fuente empieza con tres datos, y esto no se abandona
en el resto del curso:

> **De cuándo es · quién manda sobre ella · a quién gana y a quién pierde si se
> contradicen.**

- **La fecha** te dice si mirarla.
- **El dueño** te dice quién puede cambiarla.
- **La precedencia** te dice qué pasa cuando dos fuentes tuyas dicen cosas
  distintas — y eso pasa siempre.

Una fuente sin fecha no es una fuente: es un papel. En el corpus de Meridiano hay
una que es bastante más vieja que las otras dos, y no está señalada.

### (c) Citar, y poder decir «no lo sé»

**Dos exigencias, y la segunda es la difícil.**

**Citar** no es un adorno de rigor: es lo que **abarata la revisión**. Si cada
respuesta dice de qué documento sale, comprobarla cuesta diez segundos. Si no lo
dice, cuesta buscarlo tú, y entonces el sistema no te ha ahorrado nada.

**«No lo sé» hay que exigirlo por escrito y hay que probarlo**, porque el
comportamiento por defecto es el contrario. Un modelo al que le faltan datos
**rellena el hueco** con algo verosímil y bien escrito. No miente por maldad:
completa, que es lo que hace. Y en tu trabajo, un precio verosímil y falso llega
a un cliente.

> **La instrucción que funciona, y por qué:** en vez de *«si no lo sabes, dilo»*,
> escribe *«si el dato no está en las fuentes, responde exactamente: NO ESTÁ EN
> MIS FUENTES — falta: <qué falta>»*.
>
> **Le das algo que hacer en vez de algo que no hacer**, y te deja una marca que
> puedes buscar. Es la misma idea que el `[COMPROBAR: ___]` de los fundamentos, y
> funciona por lo mismo.

---

## 4 · Cuándo NO es este patrón

Cuatro desenlaces, y **tres de los cuatro no acaban en montar nada**. Eso no es un
fracaso del patrón: es el patrón funcionando.

### (a) La respuesta no está escrita en ningún sitio

Llega, y bastante. *«¿Puedo quedarme tres semanas más en la misma habitación?»* —
y resulta que eso no está decidido en ninguna parte, se resuelve caso a caso y
depende de quién lo mire.

**Veredicto: arreglar el proceso primero.** No hay nada que automatizar hasta que
alguien decida qué se contesta. Y ojo con la tentación de montarlo igual: un
asistente alimentado con una respuesta que no existe **se la inventa con seguridad**.

> **Esto no es un callejón sin salida: es un hallazgo, y es de los que valen.**
> Llegar a tu jefa diciendo *«tenemos cuatro preguntas frecuentes cuya respuesta
> no está escrita en ningún sitio, y aquí están»* es trabajo de valor, y
> probablemente lo primero útil que vas a poder aportar.

### (b) Hay dos versiones y nadie sabe cuál manda

Mira `meridiano/plantillas.md`. Dos plantillas de la misma respuesta, las dos en
uso, incompatibles en cuatro puntos.

**Mismo veredicto, y más urgente**: un sistema alimentado con las dos responde con
seguridad y se equivoca la mitad de las veces, **sin que nada lo delate**. Antes de
montar: decidir cuál manda, ponerle fecha, tirar la otra.

### (c) La respuesta depende de quién pregunta

En Meridiano hay estudiantes que llegan **por agencia**, con tarifa neta pactada
que no es la pública. La pregunta es la misma —*«¿cuánto cuesta?»*— y la respuesta
correcta es distinta.

**Aquí no falta información: falta una decisión previa.** El sistema tiene que
**clasificar antes de responder**, y eso ya no es este patrón: es el patrón 4. La
salida correcta aquí es **no responder y derivar**.

> Es el error más caro y más silencioso de este patrón, porque el sistema
> responde perfectamente… la pregunta equivocada.

### (d) El mensaje no se contesta nunca

Reclamaciones formales, cualquier cosa con un menor, salud, visados, una familia
de acogida preocupada por alguien. **Zona prohibida.** No es que el sistema lo haga
mal: es que ni siquiera se le enseña.

---

## 5 · Montarlo

Ver `P1-ejercicio.md`.

---

## 6 · Comprobar si funciona

Ver `P1-bateria.md`. Diez casos, y **tres de ellos son los que de verdad miden**:
los dos que el sistema **debe rechazar** y el hostil, que intenta darle
instrucciones.

> **Cinco casos que salen bien los consigue cualquiera.** Lo que separa un sistema
> en el que puedes confiar de uno que suena bien es qué hace con lo que **no** debe
> contestar.

---

## 7 · Los datos de este patrón

| Qué | Semáforo | Qué haces |
|---|---|---|
| Tus fuentes: tarifario, políticas, condiciones | **verde** | Se suben tal cual. No identifican a nadie |
| La pregunta que te llega de una persona | **ámbar** | Se seudonimiza antes de pegarla |
| Nombre, correo, teléfono, número de expediente | **rojo** | No entran. Y no hacen falta para contestar |

**La prueba de que has seudonimizado de verdad**, que ya viste en fundamentos:

> Si una compañera pudiera leer lo que has pegado y saber de quién hablas, no está
> seudonimizado.

Quitar el nombre y dejar *«la estudiante coreana de 19 años del grupo B1 de los
martes»* no es seudonimizar: eso identifica mejor que el nombre.

**Y el atajo que casi siempre funciona en este patrón:** para probar tu asistente
**no necesitas el mensaje real de nadie**. Escribe tú una versión equivalente. Dos
minutos, mismo valor de prueba, ningún dato de por medio.

---

## 8 · Cómo se traslada

### A otro sector

Este patrón es el mismo en todas partes. Cambian los documentos, no la estructura:

| Sector | Las fuentes | La pregunta repetida |
|---|---|---|
| Ecommerce | Política de devoluciones, plazos, tallas | *«¿Cuánto tarda un reembolso?»* |
| Software | Documentación, planes, límites | *«¿Esto está incluido en mi plan?»* |
| Clínica | Cartera de servicios, coberturas, preparaciones | *«¿Tengo que venir en ayunas?»* |
| Inmobiliaria | Condiciones, requisitos, gastos | *«¿Qué papeles necesito para alquilar?»* |

**Y las cuatro trampas también viajan enteras**, que es lo que hace útil el
patrón: en los cuatro sectores hay preguntas cuya respuesta no está escrita, hay
dos versiones de algo, hay respuestas que dependen del tipo de cliente, y hay
mensajes que no se contestan nunca.

### A una tarea real de tu trabajo

Al cerrar este patrón, llévalo a **una tarea tuya de verdad**. Es la parte que
sustituye al mundo real, así que es la que más importa.

```
TRASLADO · patrón 1 · fecha ______

La pregunta repetida de mi trabajo que voy a probar:  ______
¿Está escrita la respuesta? ¿dónde?                   ______
¿Hay más de una versión?  sí / no  — ¿cuál manda?     ______
¿La respuesta cambia según quién pregunte?  sí / no   ______
Qué seudonimizo, y cómo:                              ______
¿Aguantó?  sí / no / a medias  —  qué falló:          ______
```

> **La regla que gobierna todos los traslados:** del curso sale el método, no los
> datos. Lo que traes de tu trabajo es **la forma de la tarea**, no su contenido.

---

## 9 · El techo de este patrón

Escrito ya, para que cuando lo notes no lo leas como un fallo tuyo. Esta es tu
segunda fila en la **lista de techos**:

| Lo que esto no puede hacer | La clase de cosa que sí podría | Qué tendría que cambiar para que me tocara |
|---|---|---|
| **No sabe lo que pasó ayer.** Recuerda sus fuentes, no vuestras conversaciones | Un sistema con memoria auditable | Que necesitara continuidad **y** pudiera comprobar qué recuerda. Hoy no puedo auditarlo |
| **No se entera de que has cambiado el tarifario.** Sigue respondiendo con el documento que subiste | Fuentes conectadas al documento vivo | Que la herramienta pudiera leer el documento donde está, en vez de una copia |
| **No dispara solo.** Tú abres, tú preguntas, tú copias | Un disparador | Nada: eso es el patrón 5. *(Esta fila se tacha entonces, y tacharla es el ejercicio)* |
| **No decide a quién responde de una forma y a quién de otra** | Un clasificador delante | Nada: eso es el patrón 4 |

**Las dos últimas filas se van a tachar en este mismo curso.** Las dos primeras,
no — y saber cuál de tus techos se rompe pronto y cuál no es, exactamente, el
criterio que este curso te deja.
