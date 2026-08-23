# Dominio — La escalera de herramientas real (agosto de 2026)

**Para qué sirve este documento.** Decidir, con datos verificados y no de memoria, **sobre qué
herramientas se construye el curso**, en qué orden se suben y qué se le pide instalar (idealmente:
nada) en las primeras semanas. El eje es **Gemini**, porque es el estándar de su empresa, y la
escalera pasa por la **automatización** antes que por los agentes.

**Fecha de verificación:** 22 de agosto de 2026. Todo lo de aquí caduca; la sección 8 explica cómo
escribir el material para que sobreviva.

---

## 0. Cómo leer este documento

### 0.1 Marcas de fiabilidad

| Marca | Significado |
|---|---|
| **[V]** | **Verificado en fuente primaria**: Google (workspace.google.com, support.google.com, workspaceupdates.googleblog.com, blog.google), o la web/documentación oficial del proveedor. |
| **[S]** | **Fuente secundaria**: prensa tecnológica o comparadores de precios. Coherente y probablemente cierto, pero **no confirmado en fuente primaria**. Los comparadores de precios de IA son especialmente propensos a inventar nombres de modelos y cifras. |
| **[NV]** | **No verificado.** No he encontrado fuente fiable, o depende de la configuración concreta de su empresa. Se marca explícitamente y no se usa como base de ninguna decisión del curso. |

### 0.2 Advertencia sobre lo que NO he podido verificar

Lo más importante de todo el documento es un dato que **no existe en ninguna web**: qué plan de
Workspace tiene su empresa y cómo lo tiene configurado el administrador. De eso depende
literalmente la mitad de lo que sigue. Está tratado en la sección 1.6, y es la razón por la que ese
diagnóstico es una tarea de la semana 1.

### 0.3 Nomenclatura: 2026 ha sido un año de renombrados

Tres cambios de nombre que hay que tener presentes para no escribir material que ya nace viejo:

- **Workspace Flows → Google Workspace Studio.** Anunciado como "Flows" en 2025; renombrado a
  Workspace Studio, disponibilidad general el 3 de diciembre de 2025 y despliegue completo a partir
  del 14 de enero de 2026 [S, coincidente en varias fuentes; el producto vivo en
  `workspace.google.com/studio/` y `support.google.com/workspace-studio` es **V**].
- **NotebookLM → Gemini Notebook.** Renombrado el **16 de julio de 2026**. Mismo producto, mismos
  cuadernos, misma URL redirigida [V, blog.google].
- **Gemini CLI → Antigravity CLI.** Gemini CLI dejó de servir peticiones para Google AI Pro, Ultra y
  gratuito el **18 de junio de 2026** [V, anuncio en el repo oficial google-gemini/gemini-cli].

Esto ya es, por sí solo, el argumento de la sección 8: en cinco meses han cambiado de nombre tres de
las piezas centrales.

---

## 1. Gemini a fondo

### 1.1 Lo primero: hay tres "Geminis" distintos y confundirlos arruina todo lo demás

Este es el error conceptual número uno y hay que resolverlo en la primera lección del curso, porque
determina qué datos puede meter dentro y qué funciones tiene disponibles.

| | **Gemini app (consumo)** | **Gemini en Google Workspace** | **Gemini Enterprise (Google Cloud)** |
|---|---|---|---|
| Dónde | `gemini.google.com` con cuenta `@gmail.com` o personal | Misma web y barra lateral de Gmail/Docs/Sheets, pero con la cuenta `@suempresa.com` | Producto aparte de Google Cloud |
| Quién lo paga | Ella, o nadie (plan gratuito) | Incluido en el plan de Workspace de la empresa | Licencia adicional por puesto |
| Qué pasa con lo que escribe | Conversaciones seleccionadas **pueden ser revisadas por personas** y usadas para mejorar los servicios; Google avisa expresamente de **no introducir información confidencial** [V, Gemini Apps Privacy Hub] | Los datos **no se usan para entrenar modelos** fuera del dominio y **no los leen revisores humanos** sin permiso, con el DPA de Workspace en vigor [V, Generative AI in Google Workspace Privacy Hub] | Igual que Workspace, más controles de Cloud |
| Precio de referencia (2026) | 0 € / 4,99 $ / 19,99 $ / desde 99,99 $ al mes [S] | Incluido desde ~8,10 €/usuario/mes (ver 1.5) | Desde ~21 $/puesto/mes edición Business, 30 $+ Standard/Plus [S] |

**La consecuencia práctica, y es la frase que debe ir en negrita en el curso:** el mismo texto
escrito en la misma web es seguro o inseguro **según con qué cuenta esté logueada**. Y el riesgo
real, documentado como el fallo típico de las empresas, es exactamente el suyo: *usar Gemini o
ChatGPT personal en otra pestaña del navegador, fuera del perímetro que el administrador cree que
está protegiendo* [S, análisis de seguridad; el mecanismo es **V** por las políticas citadas].

Ella hoy usa ChatGPT por su cuenta. Eso, con datos de alumnos, es el problema de seguridad concreto
que el curso tiene que resolver — no en abstracto, sino diciéndole qué hacer el lunes.

### 1.2 Qué hay realmente dentro de Gemini en 2026

Ordenado de "lo puede usar hoy sin permiso de nadie" a "necesita que alguien lo active".

#### a) Gems — asistentes reutilizables [V]

Un Gem es un conjunto de instrucciones guardado, con nombre, que se puede reabrir sin volver a
explicar el contexto. Se crean en `gemini.google.com` → sección Gems → "Nuevo Gem": nombre,
instrucciones, y opcionalmente ficheros de conocimiento [V, support.google.com/gemini/answer/15146780].

- **Conocimiento adjunto:** se pueden subir ficheros del ordenador, **añadir ficheros de Google
  Drive** e **importar cuadernos de Gemini Notebook** [V]. El límite documentado por Google en su
  anuncio para Workspace es de **hasta 10 ficheros por Gem**, con los mismos tipos y tamaños que la
  subida de documentos [V, workspace.google.com/blog]. La cifra que circula de "100 MB por fichero"
  es **[S]** y no la he confirmado en la página oficial de límites.
- **Gems compartidos:** existen. Un Gem que te comparten **no se añade solo** a tu gestor de Gems
  [V]. Que su empresa pueda compartir Gems entre compañeros es un dato **[NV]** que depende de la
  configuración del administrador.
- **Herramienta por defecto:** un Gem puede fijar la herramienta que usa — por ejemplo, un Gem de
  investigación que arranca siempre en Deep Research [S].
- **Baja de agosto de 2026:** los Gems **ya no son accesibles desde el panel lateral de Gemini en
  Google Chat** [V, Workspace Updates 08/2026]. Siguen en el resto de sitios. Es un ejemplo perfecto
  de por qué el material no debe apoyarse en un punto de entrada concreto.

#### b) Instrucciones personalizadas (custom instructions) [S]

Distintas de los Gems: se aplican a **todas** las conversaciones, no a una. Es el mecanismo más
barato de "salir del chat" — una vez configuradas, dejan de repetirse en cada mensaje.

#### c) Deep Research [V/S]

Investigación multi-fuente que produce un informe con citas. Límites mensuales por plan de consumo:
**5 informes/mes en gratuito, 20 en AI Pro, 200 en Ultra** [S — cifras coherentes entre varias
fuentes secundarias, no confirmadas en la página oficial de límites]. Para Workspace la web oficial
habla de "acceso ampliado" sin dar número [V, pero sin cifra].

Para su trabajo esto sirve para cosas puntuales (qué pide el consulado de X, qué hace la competencia
en Madrid), no para el día a día. **No es el escalón que le falta.**

#### d) Acciones programadas (Scheduled Actions) [V]

Gemini ejecuta una instrucción de forma recurrente: diaria, semanal, mensual. **Hasta 10 acciones
programadas activas a la vez** [S, coherente entre fuentes; la función es **V**,
support.google.com/gemini/answer/16316416].

Esto es importante para el curso: **es automatización de verdad, dentro del chat que ya usa, sin
instalar nada.** Es el puente natural entre el escalón 1 y el 2.

#### e) Gemini en la barra lateral de Workspace [V]

En Gmail, Docs, Sheets, Slides, Drive, Meet y Chat. Con matices de 2026:

- **Gmail:** "Help me write" en línea, resúmenes de hilos largos, AI Overviews sobre el buzón,
  búsqueda mejorada. Disponible también en las apps móviles [S].
- **Sheets:** genera fórmulas conversacionalmente, y desde junio de 2026 **diagnostica y corrige un
  error de fórmula en un clic** [V, Workspace Updates 06/2026].
- **Sheets Canvas** (13 de agosto de 2026): convierte una hoja en una aplicación interactiva —
  paneles, tableros kanban — describiéndolo en lenguaje natural, con sincronización en tiempo real
  con los datos de origen. Business Standard/Plus, Enterprise Standard/Plus, AI Pro/Ultra [V].
- **Ask Gemini in Chat** (26 de agosto de 2026): línea de comandos unificada que busca en Gmail,
  Drive y Calendar y genera contenido, **sustituyendo** al panel lateral de Gemini en Chat. En
  inglés al principio. Business Standard/Plus, Enterprise Standard/Plus [V].
- **Admin Assist** (17 de agosto de 2026): Gemini dentro de la consola de administración [V]. No es
  para ella, pero es un dato útil: **su administrador tiene ahora ayuda contextual para responderle**
  cuando le pregunte qué plan tienen.

#### f) La función `=AI()` en Google Sheets [V]

**Esta es, con diferencia, la pieza más infravalorada para su caso concreto.**

Se escribe en una celda: `=AI("clasifica este comentario como queja de alojamiento, académica o de
otro tipo", A2)`. Acepta también la sintaxis `=Gemini()`. Genera texto, resume, **categoriza datos**
y extrae información, usando el resto de la hoja como contexto [V,
support.google.com/docs/answer/15877199 y Workspace Updates 06/2025].

Disponible en **español** desde septiembre de 2025 [V, Workspace Updates]. Solo en web, no en móvil
[S].

Por qué importa: el proceso **P27 (encuestas de satisfacción)** son 600–800 respuestas al año con
comentarios en texto libre en 10+ idiomas que, según el propio análisis de dominio, **nunca se
analizan porque nadie tiene tiempo**. Es riesgo bajo, volumen alto, multilingüe y determinista en su
parte tediosa. `=AI()` arrastrado por una columna resuelve exactamente eso. Sin instalar nada, sin
pedir permiso a nadie, en una tarde.

#### g) Gemini Notebook (antes NotebookLM) [V]

Cuadernos con fuentes propias: el modelo responde **solo** sobre lo que le has dado y **cita el
fragmento concreto**. Renombrado el 16/07/2026; los cuadernos, fuentes y enlaces antiguos siguen
funcionando [V, blog.google].

Límites oficiales por plan [V, support.google.com/notebooklm]:

| Plan | Cuadernos | Fuentes por cuaderno | Consultas de chat/día | Audio Overviews/día |
|---|---|---|---|---|
| Gratuito | 100 | 50 | 50 | 3 |
| AI Plus | 200 | 100 | 200 | 6 |
| AI Pro | 500 | 300 | 500 | 20 |
| AI Ultra (20 TB) | 500 | 500 | 2.500 | 100–200 |
| AI Ultra (30 TB) | 500 | 600 | 5.000 | 100–200 |

En Workspace, la página de precios oficial distingue **Starter = acceso básico, hasta 3 Audio
Overviews/día**, y **Standard/Plus = acceso ampliado, hasta 20/día** [V, workspace.google.com/pricing].
El número de fuentes para Workspace lo he visto citado como 400 pero es **[S]**.

Novedad de agosto de 2026: **copiar cuadernos enteros** con sus fuentes, disponible para todos [V].

Para ella: este es el sitio natural de la **base de respuestas con fuente y fecha**. Meter ahí el
tarifario, el calendario académico, las condiciones generales y las políticas de cancelación, y
preguntar en lenguaje natural, obteniendo la cita del documento. Es literalmente el requisito que el
análisis de la referencia marcaba como no negociable en atención al cliente: *citar la fuente y
saber decir "no lo sé"*.

**Aviso de riesgo:** un cuaderno con las condiciones de cancelación del año pasado responde con las
condiciones del año pasado, con toda la confianza del mundo. El control de versiones de las fuentes
es parte del ejercicio, no un detalle.

#### h) Google Workspace Studio — la automatización nativa [V]

Es la respuesta a "¿qué hay de automatización nativa en Google en 2026?", y la respuesta es: **hay
mucho más de lo que había hace un año, y es gratis dentro del plan**.

- **Dónde:** `studio.workspace.google.com`, en ordenador [V].
- **Quién:** cuentas de trabajo con Business Starter/Standard/Plus, Enterprise Standard/Plus,
  Education Fundamentals/Standard/Plus. **El administrador tiene que tener Gemini habilitado** [V,
  support.google.com/workspace-studio/answer/16444479].
- **Cómo se crea:** describiéndolo en lenguaje natural y dejando que Gemini construya el flujo, con
  plantillas predefinidas, o a mano paso a paso [V].
- **Sin código.** Literalmente: "Automate everyday work... no coding required" [V].

**Disparadores (starters) disponibles** [V, support.google.com/workspace-studio/answer/16765661]:
manual con campos de entrada; por horario; cuando llega un email que cumple un criterio; cuando
llega un mensaje de Chat; cuando me mencionan; cuando se añade un elemento a una carpeta de Drive;
cuando se edita un fichero; cuando cambia una hoja de cálculo; **cuando llega una respuesta de
Google Forms**; antes/después de una reunión; cuando están listas las notas de una reunión; cuando
alguien entra en un espacio de Chat; cuando se añade una reacción de emoji.

**Pasos (steps) disponibles** [V, misma fuente]:

- *IA*: Ask Gemini (prompt libre), **Ask a Gem** (usar un Gem propio dentro del flujo), Decide
  (verdadero/falso para bifurcar), Extract (extraer un dato concreto), Summarize, Recap unread
  emails, Create with Gemini (Docs/Slides, beta), **Deep Research (beta)**, **Ask Gemini Notebook**
  (consultar un cuaderno) y **Add a source to Gemini Notebook** (nuevo, 6 de agosto de 2026 [V]).
- *Lógica*: Check if (con AND/OR), Filter a list, Repeat for each.
- *Gmail*: redactar un borrador de respuesta, añadir/quitar etiquetas, marcar leído/no leído,
  destacar, archivar, notificarme por email.
- *Sheets*: añadir fila, actualizar filas, limpiar filas, leer el contenido de una hoja.
- *Docs*: crear documento, añadir contenido.
- *Drive*: guardar adjuntos de email en una carpeta, crear carpeta.
- *Chat*: notificarme. *Calendar*: bloquear tiempo. *Tasks*: crear tarea.
- *Terceros* (cuentas de trabajo): Asana, Confluence, Jira, Mailchimp, Slack, Salesforce [V].

**Y esto es lo decisivo pedagógicamente:** el paso "Ask a Gem" y el paso "Ask Gemini Notebook"
significan que **el trabajo del escalón 1 se reutiliza literalmente en el escalón 2**. El Gem que
escribió en la semana 2 se convierte en un paso de un flujo automático en la semana 5, sin
reescribir nada. No hay salto de herramienta, hay continuidad. Eso vale más que cualquier argumento
motivacional.

**Límites reales y trampas documentadas** [V, mismas páginas de ayuda] — hay que ponerlos por
delante porque son exactamente los que ella se va a encontrar:

1. **Los flujos fallan con unidades compartidas (Shared Drives), carpetas compartidas y hojas con
   `IMPORTRANGE`.** Los ficheros tienen que ser suyos, privados.
2. Cada flujo tiene **un solo disparador**.
3. Solo se muestran **50 etiquetas de Gmail** en la interfaz.
4. Los menores de 18 en cuentas educativas no tienen pasos de IA.
5. En cuentas personales solo está disponible vía "Workspace Experiments".

El punto 1 es **grave para su caso** y tiene que estar en el material desde el primer minuto: el
centro de gravedad de su puesto es **un buzón compartido** (`info@`, `accommodation@`,
`admissions@`) y una **hoja de camas compartida**. Los primeros flujos tienen que construirse sobre
**su propio buzón personal de empresa y sus propias copias**, no sobre los recursos compartidos.
Esto no es un fallo del curso: es la restricción real, y descubrirla en la lección 1 en vez de en el
tercer intento fallido es lo que separa un material honesto de uno que la va a frustrar.

**Controles de empresa (agosto de 2026)** [V, Workspace Updates 17/08/2026]: identidades de agente
con privilegio mínimo, atribución de identidad (beta), panel de administración de accesos, y
**restricciones de pasos, DLP y aprobación humana (human-in-the-loop) configurables por el
administrador**. Esto es bueno para el curso — el "el humano aprueba las escrituras" que la
referencia predicaba ya es una casilla en la consola — y también es un aviso: **su administrador
puede tener pasos desactivados** y ella no tiene forma de saberlo hasta que lo intenta.

#### i) Apps Script asistido por Gemini [V]

El editor de Apps Script (`script.google.com`) tiene panel lateral de Gemini: escribe, modifica y
**depura** scripts a partir de lenguaje natural [V, developers.google.com/apps-script/guides/gemini].
En agosto de 2026 se está desplegando a consumidores en planes de pago de Google AI [S,
AppsScriptPulse].

**Veredicto para ella: no.** No en este curso. Apps Script es código JavaScript aunque lo escriba
Gemini; y en el momento en que falla, hay que leer un stack trace. Es el escalón que se salta
gracias a Workspace Studio. Merece **una caja de "esto existe y qué es"** de media página, para que
sepa que existe y para que reconozca de qué le hablan si alguien de la empresa se lo menciona — no
un módulo.

#### j) Agentes de Google: Gemini Spark, Gemini in Chrome, Project Mariner [V/S]

Ver sección 4. Resumen: existen, y **casi todos están fuera de su alcance por plan**.

### 1.3 Qué viene incluido en el plan de Workspace y qué es un complemento aparte

Esta era una pregunta explícita del encargo, y la respuesta corta es: **desde 2025, casi todo viene
incluido; la era de los complementos de Gemini terminó.**

**Historia mínima, porque explica mucha documentación desactualizada que ella se va a encontrar
buscando en Google:** hasta marzo de 2025 Google vendía "Gemini Business" (20 $/usuario/mes) y
"Gemini Enterprise" (30 $/usuario/mes) como complementos. Los **discontinuó** y metió Gemini dentro
de todos los planes de Workspace, subiendo el precio base entre 2 y 4 $ por usuario [S, coherente
entre varias fuentes]. **Todo tutorial que diga "contrata el add-on de Gemini" es de antes de marzo
de 2025 y está obsoleto.** Es un buen ejemplo para el curso de cómo detectar material caducado.

**INCLUIDO en Workspace de pago** (Business Standard y superiores) [V, workspace.google.com/pricing]:

- Gemini en Gmail, Docs, Sheets, Slides, Drive, Meet y Chat ("acceso ampliado").
- **Gems.**
- **Google Workspace Studio.**
- **Gemini Notebook** con acceso ampliado (hasta 20 Audio Overviews/día).
- Gemini en Sheets, incluida la función `=AI()`.
- Gemini en el editor de Apps Script.
- Sheets Canvas.

**INCLUIDO PERO RECORTADO en Business Starter** [V]: Gemini "limitado" — **excluye Gemini en Docs,
Sheets, Slides, Drive, Meet y Chat**; Gemini Notebook en "acceso básico" con 3 Audio Overviews/día.
Workspace Studio **sí** aparece en la lista de ediciones admitidas para Starter [V], lo cual es una
asimetría curiosa que conviene verificar en la práctica más que en la tabla.

> **Si su empresa está en Business Starter, media sección 1.2 no existe para ella.** Incluida
> `=AI()` en Sheets. Este es el motivo real por el que averiguar el plan es urgente y no un trámite.

**COMPLEMENTO APARTE, es decir, se paga además** [V/S]:

- **AI Expanded Access**: complemento para más límites de generación de imagen, vídeo y de
  automatización en Workspace Studio [S, citado en la web de Google pero sin precio público que haya
  podido verificar → precio **NV**].
- **Assured Controls y AI Classification**: complemento de Enterprise [V].
- **Data Regions (edición Enterprise)**: incluido en Frontline Plus y Enterprise Plus, o como
  complemento [V]. Ojo: **"Fundamental data regions" sí está incluido en Business Standard y Business
  Plus** [V]. Esto importa para el módulo de datos sensibles.
- **Gemini Enterprise** (la plataforma agéntica de Google Cloud, lanzada en octubre de 2025): producto
  distinto, ~21 $/puesto/mes en edición Business y 30 $+ en Standard/Plus [S]. Incluye buscador
  empresarial, agentes prefabricados y un constructor de agentes sin código, y **conectores MCP**
  [V, cloud.google.com y support.google.com/g/answer/17106276]. **Es poco probable que una academia de
  30 empleados lo tenga [NV].** Merece un párrafo en el curso, no un módulo.
- **Google AI Pro / Ultra personales**: no son complementos de Workspace, son suscripciones de
  consumo. Si ella las contrata a título personal, **están fuera del perímetro de datos de la
  empresa**.

### 1.4 Google AI Studio

`aistudio.google.com` es el entorno de desarrollo de la API de Gemini: probar prompts, ajustar
parámetros, obtener claves de API. **[V]** como producto; su posición exacta en 2026 no la he
verificado en detalle porque **no es relevante para ella y recomendar lo contrario sería un error**.

Es gratuito y tentador (modelos potentes, sin límites de la app). Pero: (a) es una superficie de
desarrollador, con temperature, top-p y tokens a la vista; (b) **lo que se mete ahí está bajo los
términos de la API de consumo, no bajo el DPA de Workspace** — y una clave de API en manos de
alguien sin base técnica es un problema de seguridad y de coste; (c) no resuelve ninguna de sus 32
tareas mejor que las herramientas de arriba.

**Veredicto: mencionarlo para que sepa qué es y por qué no va ahí.** Una caja de cinco líneas.

### 1.5 Precios de Workspace (España, 2026)

| Plan | Flexible (mensual) | Anual aprox. (−16 %) | Gemini |
|---|---|---|---|
| Business Starter | **8,10 €**/usuario/mes [S] | ~6,80 € [NV, calculado] | Limitado |
| Business Standard | **16,20 €**/usuario/mes [S] | ~13,60 € [NV, calculado] | Completo |
| Business Plus | **25,30 €**/usuario/mes [S] | ~21,25 € [NV, calculado] | Completo |
| Enterprise | Presupuesto | — | Completo + complementos |

Equivalentes en dólares con compromiso anual, citados de forma consistente: 7 / 14 / 22 $ [S].
La página oficial de precios confirma la estructura de planes, el descuento del **16 % con
compromiso anual** y la prueba de 14 días, pero sirve las cifras por JavaScript y no he podido
extraerlas [V para la estructura, **NV** para las cifras exactas leídas en la web oficial].

**Orden de magnitud para su empresa (30 empleados) [NV, estimación]:** entre ~2.900 €/año en Starter
anual y ~7.700 €/año en Plus anual. Es decir: **la empresa ya paga por esto**. Ninguna de las
recomendaciones del escalón 1 y 2 de este curso implica un euro nuevo.

### 1.6 Averiguar qué tiene su empresa: el diagnóstico de la semana 1

**Dato duro y molesto [V, support.google.com/a/answer/10975849]: un usuario que no es administrador
no puede consultar la edición de Workspace de su organización.** Está en Consola de administración →
Facturación → Suscripciones, y hace falta el privilegio de gestión de facturación. No hay atajo.

Así que el curso necesita **dos vías**, y las dos son ejercicio de la semana 1:

**Vía A — preguntar bien.** Un email de seis líneas al administrador de sistemas o a quien lleve las
licencias. El curso le da el texto literal, porque redactar esto desde cero es una barrera absurda:

> *Asunto: Dos datos sobre nuestro Google Workspace*
> *Estoy organizando mejor mi trabajo con las herramientas de IA que ya tenemos contratadas y
> necesito dos datos para no pedir nada que no tengamos:*
> *1. ¿Qué edición de Google Workspace tenemos? (Business Starter, Standard, Plus o Enterprise)*
> *2. ¿Están habilitados Gemini y Google Workspace Studio para mi cuenta? Y si hay pasos o
> conectores restringidos por política, ¿cuáles?*
> *Como referencia, el dato 1 está en Consola de administración → Facturación → Suscripciones.*
> *Gracias.*

Nótese que la última línea le ahorra al administrador el trabajo de buscarlo, que es lo que hace que
un email así se conteste en vez de quedarse en el fondo del buzón.

**Vía B — diagnóstico empírico, por si no le contestan.** Una lista de cinco comprobaciones que hace
ella sola en diez minutos, y que **infiere el plan a partir de lo que ve**. Es, además, un ejercicio
excelente: es exactamente operacionalizar un constructo en indicadores observables, que es su
formación:

| Comprobación | Si funciona | Si no funciona |
|---|---|---|
| Abrir Gemini logueada con la cuenta de empresa; ver si el pie dice "Workspace" y no muestra el aviso de revisión humana | Gemini de empresa activo | Puede que no le hayan dado Gemini |
| Escribir `=AI("di hola")` en una celda de Sheets | Standard o superior | Probablemente Starter |
| Abrir el panel de Gemini en un Google Doc | Standard o superior | Starter (excluye Docs) |
| Entrar en `studio.workspace.google.com` | Workspace Studio habilitado | El administrador no lo ha activado |
| Abrir Gemini Notebook y mirar cuántos Audio Overviews diarios permite | 20/día → Standard+; 3/día → Starter | — |

Este cuadro es material de curso tal cual, y tiene una virtud pedagógica extra: le enseña que
**la documentación dice una cosa y la instancia concreta dice otra, y manda la instancia.**

---

## 2. Qué significa "salir del chat" sin cambiar de herramienta

El brief dice que lo primero que necesita no es una herramienta nueva sino usar bien la que tiene.
Correcto. Pero "usar mejor el chat" es una consigna vacía si no se nombran los mecanismos. Son
cinco, y cada uno tiene un límite real que hay que decir en voz alta.

### 2.1 Los cinco mecanismos, con sus límites

| Mecanismo | Qué resuelve | Límite real |
|---|---|---|
| **Instrucciones personalizadas** | El contexto que se repite en *todas* las conversaciones: quién es, dónde trabaja, en qué idioma responde, qué tono usa | Es global. Si lo llena de detalles de un proceso concreto, contamina el resto. Sirve para identidad, no para procedimiento. **[S]** |
| **Gems** | Un procedimiento concreto reutilizable: "redactor de respuestas a incidencias de alojamiento", "revisor de presupuestos" | Máx. **10 ficheros de conocimiento** [V]. No se actualizan solos: si cambia el tarifario, el Gem sigue con el viejo. **No tiene memoria entre conversaciones** — recuerda las instrucciones, no lo que pasó ayer. |
| **Ficheros de contexto en Drive** | Que el conocimiento viva en un documento versionable en vez de dentro de un prompt | Hay que volver a adjuntarlos o referenciarlos. Y si el Gem apunta a un Drive compartido, ojo con lo de la sección 1.2.h |
| **Gemini Notebook** | Preguntar sobre un corpus cerrado **con cita del fragmento** | Máx. 300 fuentes en AI Pro, 50 en gratuito [V]. Cita la fuente, pero **no sabe si esa fuente está caducada**. El control de versiones es humano. |
| **Acciones programadas** | Que algo pase sin que ella entre a pedirlo | Máx. ~10 activas [S]. Es un disparador de calendario, no reacciona a eventos. Para eso hace falta Workspace Studio. |

### 2.2 El límite que hay que decir con todas las letras: la memoria

Este es el punto donde la mayoría de la gente se hace una idea equivocada, y donde el material tiene
que ser tajante:

- **Un Gem no recuerda conversaciones anteriores.** Recuerda sus instrucciones. Cada conversación
  empieza en blanco salvo por lo que está escrito en el Gem y sus ficheros.
- **Existe "contexto personal"** en la app de Gemini (usar el historial y datos de otras apps de
  Google), pero es opaco: no se puede auditar qué recuerda ni corregirlo con precisión. **[NV]** en
  cuanto a su comportamiento exacto en cuentas de Workspace en agosto de 2026.
- La conclusión operativa es la buena noticia del webinar de referencia, y hay que quedarse con ella:
  **el contexto que quieras que persista tiene que estar escrito en un sitio que tú controles.** Un
  documento en Drive, un fichero de conocimiento del Gem, una fuente del cuaderno. La memoria fiable
  es un fichero, no una sensación.

### 2.3 La otra mitad de "salir del chat": dejar de copiar y pegar

Hay una diferencia que el curso debe hacer explícita porque es la que ella vive todos los días. Los
tres movimientos, en orden de esfuerzo creciente:

1. **Del chat al sitio donde vive el trabajo.** No abrir `gemini.google.com` para redactar un correo:
   usar el panel de Gemini **dentro de Gmail**, donde ya tiene el hilo delante. No pegar una lista en
   el chat para clasificarla: usar `=AI()` **dentro de la hoja**. El copiar-pegar no es un hábito, es
   un síntoma de estar en la herramienta equivocada.
2. **Del prompt al artefacto.** Un prompt bueno que se escribe una vez y se pierde no vale nada. El
   mismo prompt guardado como Gem, con su tarifario adjunto, es infraestructura.
3. **Del artefacto al disparador.** Cuando el Gem funciona, se mete como paso "Ask a Gem" dentro de
   un flujo de Workspace Studio y deja de necesitar que ella lo abra.

Esa progresión de tres movimientos **es la escalera del curso en miniatura**, y se puede recorrer
entera sin instalar nada ni pedir ninguna licencia. Ese es el argumento más fuerte que tenemos para
la estructura.

---

## 3. Automatización sin código — el escalón 2

### 3.1 Las cinco opciones, evaluadas para su caso concreto

| | **Workspace Studio** | **Make** | **n8n** | **Zapier** | **Power Automate** |
|---|---|---|---|---|---|
| Coste para ella | **0 €** (dentro del plan) [V] | Gratis 1.000 ops/mes; Core 9 $/mes; Pro 16 $/mes [S] | Gratis autoalojado; Cloud desde ~20–24 €/mes [S] | Gratis 100 tareas/mes; Pro ~19,99 $/mes [S] | Premium 15 $/usuario/mes [S] |
| Instalar algo | No | No | Sí si autoaloja (Docker, VPS) | No | No |
| Cuenta nueva / alta | No | Sí | Sí | Sí | Sí |
| ¿Dónde viven sus datos? | Dentro del tenant de Workspace | En un tercero (con conexión OAuth a su Gmail y Drive) | Ídem, o en un servidor que alguien mantiene | En un tercero | En el tenant de Microsoft |
| Encaje con su empresa | Total: la empresa vive en Google | Requiere aprobar un proveedor nuevo | Ídem + alguien que lo mantenga | Ídem | **Ninguno: es el ecosistema Microsoft** |
| Curva para no técnicos | La más suave: se describe el flujo en lenguaje natural [V] | Suave-media, visual | **Empinada; interfaz de desarrollador** [S] | Suave, pero el modelo de precios por *paso* castiga | Media |
| IA integrada | Nativa: Ask Gemini, Ask a Gem, Ask Notebook, Decide, Extract, Deep Research [V] | Vía módulos de IA y agentes (plan Pro) | Muy potente, pero hay que montarla | Vía módulos | Copilot Studio, con créditos aparte (200 $/25.000 créditos) [S] |

### 3.2 La elección correcta para ella, y por qué

**Google Workspace Studio. Sin dudarlo, y sin evaluar alternativas en el curso más allá de una
página.** Cuatro razones, en orden de peso:

1. **Coste marginal cero y fricción de alta cero.** No hay que dar de alta un proveedor, no hay que
   conectar OAuth de terceros al buzón de la empresa, no hay que justificar un gasto. El brief es
   explícito: si en la semana 1 le pedimos que instale algo o pida una licencia, la perdemos.
2. **Continuidad con el escalón 1.** El paso `Ask a Gem` y el paso `Ask Gemini Notebook` reutilizan
   literalmente lo que construyó en las semanas anteriores. En Make o n8n tendría que rehacerlo.
3. **Es la respuesta correcta también en términos de datos.** Conectar Make o Zapier al buzón
   `info@` de una academia significa que los datos de pasaportes y alojamientos de menores pasan por
   un proveedor más. Dentro de Workspace Studio no salen del tenant [V, controles de agosto de 2026].
4. **Su empresa vive en Google.** El criterio general —"automatiza donde ya están tus datos"— apunta
   aquí sin ambigüedad.

**Cuándo dejaría de ser la respuesta correcta**, y esto tiene que estar escrito para que el criterio
sobreviva al producto: cuando el flujo tenga que **tocar un sistema que no está en Workspace** — el
software de gestión académica, la pasarela de pago, WhatsApp Business, un portal de agencia. Ahí
Workspace Studio se queda corto y **Make** es la siguiente parada natural (más barato que Zapier a
volumen, más amable que n8n). **n8n solo si aparece alguien técnico que lo mantenga**; en un puesto de
CX sin base técnica, autoalojar n8n es adoptar un problema, no resolverlo. **Power Automate se
descarta de plano**: es la respuesta correcta para una empresa que vive en Microsoft 365, y la suya
no.

### 3.3 Qué se automatiza de verdad en atención al cliente, y qué no

Cruzando el inventario de 32 procesos con lo que Workspace Studio puede hacer realmente:

**Verde — automatizable ya, riesgo bajo, con revisión humana antes de enviar:**

- **P27 Encuestas de satisfacción.** Riesgo bajo, volumen alto, multilingüe, y hoy **no se hace**.
  El mejor primer proyecto que existe en toda su lista.
- **P01 Respuestas a preguntas repetidas** (70–80 % preguntan lo mismo): **borrador** sugerido, nunca
  envío automático.
- **P30 Parte semanal a dirección académica.** Determinista puro.
- **P32 Detección de plantillas desactualizadas.** El "riesgo alto y silencioso" del inventario: una
  comprobación programada que avisa cuando la versión española cambia y las otras cinco no.
- **P28 Triaje de reseñas** (clasificar y preparar borrador; publicar siempre a mano).

**Ámbar — automatizable la parte mecánica, nunca la decisión:**

- **P02 Presupuestos**: el cálculo es aritmética sobre una tabla y es determinista — pero **eso no
  necesita un modelo de lenguaje, necesita una fórmula**. Este es el ejemplo canónico del árbol de
  decisión de la referencia y hay que usarlo tal cual en el curso.
- **P06 Recordatorios de pago**: la regla de calendario sí; el tono de la reclamación, revisado.
- **P07 Pack de bienvenida** y **P18 Confirmación de alojamiento**: combinación de plantilla y
  variables. Automatizable, pero **el fallo es caro** (un alumno a las 23:40 en Barajas con la
  dirección mal). Revisión humana obligatoria.
- **P20 Incidencias de alojamiento**: clasificar y enrutar sí; responder no.

**Rojo — zona prohibida, y el curso tiene que decir por qué, no solo que no:**

- **P08 Cartas de visado.** Riesgo crítico, normativa que cambia de un año a otro (RD 1155/2024,
  Instrucción SEM 3/2025). Congelar eso dentro de un prompt es fabricar un error futuro.
- **P26 Quejas formales.** Una respuesta que admite responsabilidad por escrito compromete a la
  empresa.
- **P29 Emergencias 24 h.** Personas, menores, responsabilidad civil.
- **P25 Reembolsos**: datos bancarios, riesgo de fraude por suplantación.
- **P17 Matching con familias**: datos de categoría especial del RGPD (salud, religión). Es una
  trampa como primer proyecto precisamente porque *parece* el caso ideal de IA.

### 3.4 Cinco automatizaciones montables en una tarde

Todas con Workspace Studio, sin instalar nada, y todas construidas **sobre su propio buzón y sus
propias copias**, no sobre los recursos compartidos (límite de la sección 1.2.h).

**A) Análisis de las encuestas de satisfacción — el primer proyecto**
- *Disparador:* "When a form response comes in" (Google Forms).
- *Pasos:* `Extract` (idioma y tema) → `Ask Gemini` (traducir el comentario al español y clasificarlo
  en una taxonomía cerrada: académico / alojamiento / instalaciones / actividades / administración) →
  `Check if` (¿es negativo y grave?) → `Add a row` en una hoja + `Notify me in Chat` solo si es grave.
- *Por qué es el primero:* riesgo bajo, hoy no se hace, resultado visible en una semana, y toca el
  proceso más multilingüe de la lista. Y si lo hace mal, no pasa nada.
- *Variante aún más simple, sin Studio:* la columna `=AI()` en la hoja de respuestas. **Media hora.**

**B) Triaje del correo entrante**
- *Disparador:* "When I get an email" (con criterio de remitente/asunto).
- *Pasos:* `Extract` (¿es lead, incidencia, visado, pago, otro?) → `Add or remove labels` → `Star an
  email` si es urgente → `Notify me in Chat` si menciona visado, denegación o menor.
- *Regla de oro que va escrita en el material:* **este flujo no responde a nadie. Solo ordena.**
  Etiquetar es reversible; enviar no.

**C) Borradores para las preguntas repetidas (P01)**
- *Requisito previo:* un cuaderno de Gemini Notebook con el tarifario, el calendario, las condiciones
  y el FAQ de visados. Con fecha de última revisión en cada fuente.
- *Disparador:* "When I get an email" en la carpeta de leads.
- *Pasos:* `Ask Gemini Notebook` (buscar la respuesta **con cita**) → `Check if` (¿ha encontrado
  fuente?) → si sí, `Draft an email`; si no, `Add label` "responder a mano".
- *Lo importante es el "si no":* es el "saber decir no lo sé" de la referencia, convertido en una
  bifurcación de un flujo. **Nunca envía: deja el borrador.**

**D) Vigilante de plantillas desactualizadas (P32)**
- *Disparador:* "When a file is edited" sobre el tarifario maestro, o "On a schedule" mensual.
- *Pasos:* `Get sheet contents` → `Ask Gemini` (comparar los precios del maestro con los de cada
  plantilla de idioma) → `Create a task` con las discrepancias.
- *Por qué mola:* ataca un riesgo real, alto y silencioso, que hoy nadie vigila.

**E) Recordatorio de pagos pendientes (P06)**
- *Disparador:* "On a schedule", cada mañana.
- *Pasos:* `Get sheet contents` (hoja de reservas con fechas de inicio y estado de pago) → `Filter a
  list` (inicio en menos de 15 días y sin pago) → `Draft an email` por cada uno → `Notify me in
  Chat` con el recuento.
- *La condición de parada:* si la lista supera N, no redacta nada y avisa. Un flujo que genera 40
  borradores un lunes de julio no ayuda, entorpece. **Enseñar a poner topes es enseñar diseño.**

### 3.5 El principio que sobrevive a los productos

De los cinco ejemplos, ninguno envía nada a un cliente por su cuenta. Todos **preparan, clasifican,
avisan o redactan un borrador**. Esa es la regla, y es la que hay que enseñar como criterio, no como
precaución:

> **Automatiza la lectura y la preparación. La escritura hacia fuera la firma una persona.**

Se puede relajar más adelante, proceso a proceso, con datos de acierto medidos. Pero se empieza así.

---

## 4. Agentes — el escalón 3

### 4.1 Qué es un agente en 2026 para alguien no técnico

La definición útil, que evita tanto el hype como el desprecio:

> **Automatización** = el mismo camino, siempre. Los pasos los decidiste tú.
> **Agente** = tú defines el objetivo y los límites; **los pasos los decide él sobre la marcha**, y
> puede usar herramientas y consultar cosas para llegar.

Consecuencia directa, y es lo que hay que enseñar: **un agente no es "una automatización mejor". Es
una automatización que ha renunciado a ser predecible a cambio de poder afrontar casos que no
previste.** En atención al cliente, donde el error es visible y a veces caro, esa renuncia hay que
pagarla a conciencia y solo donde compensa.

Y la dirección del error que casi nadie enseña: **un agente puede ser exceso**. Si la tarea tiene
pasos fijos, meterle un agente es peor —más caro, más lento, menos auditable— que un flujo.

### 4.2 Qué agentes puede usar de verdad, sin terminal

| Producto | Qué hace | Puede usarlo ella hoy |
|---|---|---|
| **Workspace Studio con pasos de IA** | Un flujo con `Decide`, `Extract` y `Ask a Gem` ya tiene juicio en puntos concretos, dentro de un camino que tú controlas | **Sí**, incluido en su plan [V]. *Es aquí donde va a hacer su "agente" real.* |
| **Deep Research** | Investiga varias fuentes, decide qué mirar, produce informe con citas | **Sí** [V] |
| **Gemini Spark** | Agente personal 24/7: gestiona correo, calendario, ficheros, navega, reserva; con **conectores MCP personalizados** | **Solo AI Ultra** (99,99–199,99 $/mes), 18+, países seleccionados, y "usuarios de empresa seleccionados" [V, gemini.google/overview/agent/spark]. **Casi con seguridad, no.** |
| **Gemini in Chrome / auto browse** | Agente de navegador: reserva, actualiza pedidos, gestiona trámites | Disponible para Workspace, pero **auto browse requiere AI Pro/Ultra** y arrancó en EE. UU./Android [V, Workspace Updates 06/2026] |
| **Project Mariner** | Prototipo de automatización de navegador | **Solo AI Ultra, EE. UU.** [S]. No. |
| **Gemini Enterprise** | Constructor de agentes sin código + conectores MCP a Gmail, Drive, Docs, Sheets, Calendar, Chat | Solo si su empresa lo tiene contratado aparte [**NV**] |
| **Claude Cowork** | Agente de escritorio/web/móvil, sin terminal, con acceso a ficheros y tareas programadas | Sí, con Claude Pro (20 $/mes) [S] — pero fuera del estándar de su empresa. Ver sección 5. |

### 4.3 MCP y conectores: qué es y por qué le importa poco todavía

**MCP (Model Context Protocol)** es el estándar por el que un modelo se conecta a una fuente de datos
o a una herramienta. En 2026 Google publica servidores MCP oficiales de Workspace para que
aplicaciones como Antigravity o Claude actúen sobre Gmail, Drive, Docs, Sheets, Slides y Calendar
[V, developers.google.com/workspace/guides/configure-mcp-servers].

En la app de Gemini, las "Extensiones" pasaron a llamarse **Connected Apps**, y los **conectores MCP
personalizados están limitados a usuarios con acceso a Gemini Spark, y solo dentro de tareas de
Spark** [S].

**Lo que esto significa para ella, sin adornos:** MCP es hoy, para su perfil, **vocabulario, no
herramienta**. Tiene que saber qué es —le van a hablar de ello— y tiene que entender el concepto de
"conectar el agente solo a lo que necesita". Pero configurar un servidor MCP no es una tarea de este
curso. Media página en el glosario, con un ejemplo de por qué importa (el principio de privilegio
mínimo), y seguir.

### 4.4 La barrera real hoy

No es técnica. Son cuatro barreras, en este orden:

1. **De licencia.** Los agentes de verdad —Spark, Mariner, auto browse— están detrás de AI Ultra o de
   Gemini Enterprise. Su plan de empresa casi con seguridad no los incluye. **Esta es la barrera
   número uno y es de dinero, no de capacidad.**
2. **De permisos.** Un agente útil en su puesto necesitaría tocar el buzón compartido, la hoja de
   camas y el software de gestión. Lo primero y lo segundo son recursos compartidos, que es
   justamente lo que Workspace Studio no soporta [V]. Lo tercero probablemente ni siquiera tiene API.
3. **De datos.** Sus procesos de más volumen mezclan datos de categoría especial del RGPD (salud,
   religión), menores y documentación de identidad. Un agente autónomo ahí no es un problema
   técnico, es un problema jurídico.
4. **De verificación.** Un agente que decide sus propios pasos solo es utilizable si se puede
   comprobar qué hizo. En 2026 la observabilidad de estas cosas para un usuario final sigue siendo
   pobre. **[NV]**, pero es la impresión consistente de toda la documentación revisada.

La conclusión honesta para el curso: **el escalón 3 en su caso es "un flujo con juicio en dos o tres
puntos concretos", no "un agente autónomo que gestiona el buzón".** Y eso hay que decirlo sin
disculparse, porque es lo cierto y porque es alcanzable.

---

## 5. Escalón 4 — Claude Code y equivalentes, con honestidad

### 5.1 Qué hay

- **Claude Code**: herramienta de terminal. Corre sobre el plan de Claude que ya tengas. **No está en
  el plan gratuito**: requiere Pro (20 $/mes) como mínimo [S].
- **Claude Cowork**: la misma arquitectura agéntica de Claude Code envuelta en una interfaz para
  gente no técnica. Preview en enero de 2026, disponibilidad general el 9 de abril de 2026, y desde
  el 7 de julio de 2026 funciona también desde el navegador y desde el móvil [S, TechCrunch y otros].
  Incluido en los planes de pago de Claude desde Pro [S]. **Acceso a ficheros, tareas recurrentes
  programadas, instrucciones globales y por carpeta.**
- **Google Antigravity**: IDE de escritorio y CLI orientado a agentes, con gestor de agentes visual.
  **Sustituye a Gemini CLI**, que dejó de servir peticiones para Pro, Ultra y gratuito el 18 de junio
  de 2026 [V]. Tiene plan gratuito con límites semanales [S].
- **OpenAI Codex** y equivalentes: misma categoría.

### 5.2 El veredicto, sin venderlo

**Para ella, hoy: es una distracción. Y decirlo así es lo único honesto.**

Los argumentos, en orden:

1. **No resuelve ninguno de sus 32 procesos mejor que el escalón 2.** Ninguno. Sus tareas de alto
   volumen viven en Gmail, Sheets, Drive y Forms; Workspace Studio llega a todas ellas sin salir del
   perímetro de datos de la empresa. Claude Code llegaría peor y desde fuera.
2. **Está fuera del estándar de su empresa.** Su empresa recomienda Gemini y en principio solo
   Gemini. Meter una herramienta de Anthropic con acceso a ficheros de trabajo es una conversación
   sobre proveedores y datos que ella no ha pedido tener y que el brief dice expresamente que no
   necesita tener.
3. **Es un coste personal.** 20 $/mes de su bolsillo, sobre un plan de empresa que ya paga por
   capacidades equivalentes para su caso.
4. **La demo de la referencia es de Claude Code, y ese es precisamente el sesgo que estamos
   corrigiendo.** El grafo de Obsidian es atrezzo de webinar. Copiar la herramienta de la demo porque
   la demo era espectacular sería exactamente el error que el análisis de referencia ya identificó.

**Cuándo sí, y esto también hay que escribirlo, porque un "no" sin condiciones de revisión es
dogma:**

- Si acaba con una tarea que exige **procesar decenas de ficheros locales** de forma repetida —por
  ejemplo, revisar 200 contratos de estancia larga buscando cláusulas—, ahí un agente con acceso al
  sistema de ficheros gana de calle.
- Si su pareja, que tiene conocimientos de IA, le monta algo y ella solo tiene que usarlo. **Este es
  un punto de consulta natural**, y de los buenos: media hora con alguien que sabe vale más que un
  módulo entero.
- Si en algún momento le pica la curiosidad. Que la satisfaga, pero **como apéndice del curso, con
  Cowork y no con la terminal**, y sabiendo que es exploración, no plan.

**Cómo debe aparecer en el curso:** un módulo final, explícitamente marcado como **opcional**, de una
sola lección, cuyo objetivo declarado no es que lo use, sino **que sepa qué es y por qué no lo
necesita**. Si termina el curso sin abrirlo, el curso ha funcionado igual.

---

## 6. Costes reales

### 6.1 Lo que su empresa ya paga [S, estimación **NV** en el total]

Entre ~2.900 € y ~7.700 € al año en licencias de Workspace para 30 personas, según edición. **Todo
el escalón 1 y todo el escalón 2 de este curso caben ahí dentro sin un euro adicional.** Ese es el
mensaje que abre el curso: *no vas a tener que pedir nada.*

### 6.2 Qué puede hacer con plan gratuito (si están en Starter, o para practicar en casa)

| Se puede | No se puede |
|---|---|
| Gemini gratuito: chat completo, Gems, subir ficheros | `=AI()` en Sheets (requiere plan de pago) [V] |
| Gemini Notebook: **100 cuadernos, 50 fuentes cada uno, 50 consultas/día, 3 Audio Overviews/día** [V] | Deep Research más allá de 5 informes/mes [S] |
| **5 informes de Deep Research al mes** [S] | Workspace Studio con cuenta personal (solo vía "Workspace Experiments") [V] |
| Acciones programadas [S, límite ~10 activas] | Gemini Spark, auto browse, Mariner |
| Make gratuito: 1.000 operaciones/mes, escenarios multipaso [S] | Claude Code (no está en el plan gratuito de Claude) [S] |
| Zapier gratuito: 100 tareas/mes, flujos de 2 pasos [S] | |
| Antigravity: plan gratuito con límites semanales [S] | |

**El plan gratuito de Gemini Notebook es sorprendentemente generoso para su caso**: 50 fuentes por
cuaderno cubren de sobra un tarifario, un calendario, unas condiciones generales y un FAQ. Si por lo
que sea no puede tocar nada de la empresa, **puede practicar el escalón 1 entero gratis** con
documentos ficticios.

### 6.3 Suscripciones personales, por si se las plantea

| | Precio/mes [S] | ¿Merece la pena para ella? |
|---|---|---|
| Google AI Plus | 4,99 $ (bajado desde 7,99 $ en junio de 2026) | Si su empresa está en Starter y quiere `=AI()` y Notebook decente en casa: quizá |
| Google AI Pro | 19,99 $ | Solo si Deep Research a 20 informes/mes le resulta central. Probablemente no |
| Google AI Ultra | desde 99,99 $ (el tramo de 249,99 $ se dividió en I/O 2026 en 99,99 $ y 199,99 $) | **No.** Es la única puerta a Spark y Mariner, y eso no justifica el precio en su caso |
| Claude Pro | 20 $ | Solo para el escalón 4 opcional |
| ChatGPT Plus | ~20 $ [**NV**, no verificado en esta investigación] | Ya lo usa. El curso debe abordar **el riesgo de datos**, no el precio |

**Recomendación de coste:** **cero euros.** Todo el curso se puede hacer con lo que su empresa ya
paga más los planes gratuitos. Si el curso le acaba costando dinero, hemos fallado en el
diagnóstico.

---

## 7. Recomendación: sobre qué se construye el esqueleto del curso

### 7.1 El principio de diseño

**Cada escalón se construye sobre el artefacto del anterior, y ningún escalón introduce una
herramienta nueva antes de haber agotado la anterior.** No es solo pedagogía: es que Workspace Studio
consume Gems y cuadernos como pasos, así que la continuidad es literal, no metafórica.

Y el corolario que el brief impone: **cero instalaciones y cero peticiones de licencia hasta pasada
la mitad del curso.** Idealmente, nunca.

### 7.2 La escalera, escalón por escalón

**Escalón 0 — Diagnóstico (semana 1). Coste: 0. Instalaciones: 0.**
- Averiguar el plan: email al administrador (Vía A) + las cinco comprobaciones empíricas (Vía B).
- Inventario propio de tareas, corrigiendo el mapa de 32 procesos con su realidad.
- Primera clasificación: chat / automatización / agente / **ni IA**.
- Y la lección de datos sensibles **aquí, no al final**: qué es la cuenta de empresa, qué es la
  personal, qué no se pega nunca en ninguna. Porque es la semana en la que va a empezar a pegar cosas.
- *Entregable:* una ficha de una página con su plan real, sus tres tareas candidatas y el veredicto de
  cada una.

**Escalón 1 — Salir del chat sin cambiar de herramienta (semanas 2–3). Coste: 0.**
- Instrucciones personalizadas.
- Un Gem con ficheros de conocimiento, para su tarea más repetitiva.
- Un cuaderno de Gemini Notebook con las fuentes de verdad de su puesto, **con fecha de revisión en
  cada una**, y la regla de "no lo sé".
- Gemini en Gmail y en Sheets **desde dentro de Gmail y de Sheets**, no desde la ventana de chat.
- *Entregable:* un Gem y un cuaderno que responden preguntas reales de su trabajo citando la fuente.
- *Prueba de que funciona:* diez preguntas reales, cinco que debe acertar, tres límite, dos que debe
  rechazar diciendo que no lo sabe.

**Escalón 1,5 — La primera automatización sin salir de Gemini (semana 4). Coste: 0.**
- Una **acción programada**: un resumen semanal, un recordatorio.
- Una columna `=AI()` en una hoja real: clasificar las respuestas de la última encuesta.
- *Por qué existe este medio escalón:* porque es la primera vez que algo pasa sin que ella lo pida, y
  ese es el momento psicológico del curso. No hay que hacerla esperar a la semana 6 para eso.

**Escalón 2 — Automatización de verdad con Workspace Studio (semanas 5–7). Coste: 0.**
- Flujo A (encuestas) como proyecto guiado.
- Flujo B (triaje de correo) como proyecto propio.
- Reutilizar el Gem y el cuaderno del escalón 1 como pasos `Ask a Gem` / `Ask Gemini Notebook`.
- Diseñar **condiciones de parada y topes**, y el hábito de "esto prepara, no envía".
- Los límites reales por delante: nada de unidades compartidas ni `IMPORTRANGE`.
- *Entregable:* dos flujos activos, con su batería de casos de prueba y su regla de parada.
- *Punto de consulta con la pareja:* aquí. Cuando un flujo falla por un motivo de plataforma y no de
  diseño, diez minutos con alguien que sabe ahorran una tarde.

**Escalón 3 — Juicio dentro del flujo (semanas 8–9). Coste: 0.**
- Qué es un agente, qué no, y por qué en su puesto la respuesta correcta casi siempre es "flujo con
  juicio en dos puntos" y no "agente autónomo".
- Los pasos `Decide` y `Extract` como el sitio donde vive el juicio.
- Glosario honesto: MCP, conectores, agentes de navegador, Gemini Enterprise. Qué son, por qué hoy no
  los usa, y qué tendría que cambiar para que los usara.
- *Entregable:* un flujo que se bifurca según un criterio que ella ha definido y sabe justificar.

**Escalón 4 — Opcional, una sola lección. Coste: 0 si no lo abre.**
- Claude Code, Cowork, Antigravity. Qué son, cuándo ganan, por qué hoy no.
- *Entregable:* ninguno. Es lectura.

### 7.3 Momento de subir cada escalón

El criterio no es el calendario, es el artefacto:

- Se sube al escalón 2 **cuando el Gem del escalón 1 le está ahorrando tiempo de verdad y ella lo
  usa sin que el curso se lo pida**. Si no lo usa, el Gem está mal y no hay que automatizarlo:
  automatizar algo que no funciona es multiplicar el error.
- Se sube al escalón 3 **cuando tenga dos flujos vivos y haya visto uno fallar**. Sin haber visto un
  fallo, no hay criterio para dar autonomía a nada.
- El escalón 4 no se sube. Se lee.

### 7.4 Lo que NO va en el curso

- Apps Script como módulo (caja informativa de media página, y punto).
- Google AI Studio (caja de cinco líneas).
- n8n, Zapier y Power Automate como módulos (una tabla comparativa de una página, para que sepa que
  existen y cuál sería la siguiente parada si algún día lo necesita).
- Cualquier módulo de venta interna, portfolio o landing. El brief es taxativo.
- Cualquier cosa vistosa. Nada de grafos.

---

## 8. Riesgo de caducidad y cómo escribir para sobrevivirlo

### 8.1 Qué va a envejecer mal, ordenado por probabilidad

| Riesgo | Probabilidad a 12 meses | Qué se rompe |
|---|---|---|
| **Nombres de producto** | **Casi segura.** Tres renombrados en 2026: Flows→Studio, NotebookLM→Gemini Notebook, Gemini CLI→Antigravity CLI | Todas las capturas, todas las rutas de menú |
| **Ubicación de los botones** | **Casi segura** | Las instrucciones paso a paso |
| **Límites numéricos** | **Alta.** Los cupos de Notebook y de Deep Research se mueven cada pocos meses | Las tablas de la sección 1 y 6 |
| **Precios** | **Alta.** AI Plus bajó de 7,99 a 4,99 $ en junio de 2026; Ultra se dividió en dos tramos en I/O 2026 | La sección 6 |
| **Qué edición incluye qué** | **Media-alta.** Google ya movió Gemini de complemento a incluido en 2025 | La sección 1.3 |
| **Puntos de entrada** | **Media.** Gems dejaron de estar en el panel de Chat en agosto de 2026 | Los primeros pasos de cada ejercicio |
| **Modelo subyacente** | Alta, e **irrelevante** | Nada, si el material no lo menciona |
| **El árbol de decisión chat/automatización/agente** | **Baja** | Nada |
| **"Automatiza donde ya viven tus datos"** | **Muy baja** | Nada |
| **"Prepara, no envíes"** | **Muy baja** | Nada |
| **Los 32 procesos de su puesto** | **Muy baja** | Nada. Una academia de idiomas en 2030 seguirá emitiendo cartas de visado |

La lectura de esa tabla es el diseño: **lo que caduca es lo que se puede mirar en pantalla; lo que
dura es lo que hay que pensar.** Y el material tiene que reflejar esa frontera físicamente.

### 8.2 La convención propuesta: dos secciones, dos formatos, dos fechas

En **cada lección**, el contenido se parte en dos bloques visualmente distintos y nunca mezclados:

---

**`## El criterio`** *(sin fecha, sin capturas, sin nombres de menú)*

Por qué esto se hace así. Qué problema resuelve. Cómo se decide si toca. Qué se comprueba para saber
si ha salido bien. Qué puede salir mal y cómo lo detectas.

Regla de escritura: **si una frase de esta sección deja de ser cierta porque Google renombró algo, la
frase estaba mal escrita.** Aquí se habla de "un asistente reutilizable con instrucciones guardadas",
no de "un Gem". El nombre propio va entre paréntesis la primera vez y no vuelve a aparecer.

---

**`## Los clics de hoy`** *(con fecha de verificación arriba, en grande)*

> *Verificado el 22 de agosto de 2026. Si algo no coincide con lo que ves, tu pantalla tiene razón y
> este texto no. Salta a la sección "Cuando no coincide".*

Rutas concretas, nombres de botones, capturas, límites numéricos, precios.

---

**`## Cuando no coincide`** *(una vez en todo el curso, referenciada desde cada lección)*

Media página que le enseña **el procedimiento** para cuando el manual y la pantalla discrepan:
buscar el nombre nuevo en el blog de novedades de Workspace, comprobar si es una restricción de su
plan o de su administrador, preguntar a Gemini "¿cómo se llama ahora X y dónde está?", y —solo si
nada de eso funciona— el punto de consulta con su pareja.

Esto convierte la caducidad de un defecto en **una competencia enseñada**. Que es exactamente lo que
necesita alguien que va a seguir usando estas herramientas cinco años después de terminar el curso.

### 8.3 Tres reglas complementarias

1. **Ningún ejercicio depende de una captura.** El texto describe qué busca ("el botón que crea un
   flujo nuevo"), la captura solo ilustra. Si la captura envejece, el ejercicio sigue haciéndose.
2. **Los números viven en un único fichero.** Precios, cupos y límites en `datos-volatiles.md`,
   referenciado desde las lecciones. Actualizar el curso es actualizar un fichero, no veinte.
3. **Cada afirmación volátil lleva su marca de fiabilidad**, igual que este documento. Enseñarle a
   distinguir "esto lo dice Google" de "esto lo dice un blog de precios" es, por sí solo, media
   competencia de alfabetización en IA.

---

## 9. Resumen ejecutivo en diez líneas

1. La herramienta del curso es **Gemini dentro de Google Workspace**, porque es lo que su empresa
   paga y lo que la protege jurídicamente.
2. Lo primero, en la semana 1, es **averiguar qué plan tienen**: un usuario no admin no puede
   consultarlo, así que hacen falta un email y cinco comprobaciones empíricas.
3. **Si están en Business Starter, la mitad de las funciones no existen para ella.** Es el dato que
   condiciona todo.
4. "Salir del chat" son cinco mecanismos concretos —instrucciones, Gems, ficheros, cuadernos,
   acciones programadas— y cada uno tiene un límite que hay que decir en voz alta. El principal:
   **la memoria fiable es un fichero, no una sensación.**
5. La automatización correcta para ella es **Google Workspace Studio**: cero coste, cero instalación,
   y reutiliza literalmente sus Gems y cuadernos como pasos del flujo.
6. Su primer proyecto debe ser **el análisis de las encuestas de satisfacción**: riesgo bajo, volumen
   alto, multilingüe, y hoy no se hace.
7. La regla que atraviesa todo el escalón 2: **automatiza la lectura y la preparación; la escritura
   hacia fuera la firma una persona.**
8. Los agentes de verdad de Google están detrás de AI Ultra o de Gemini Enterprise. Su escalón 3
   realista es **un flujo con juicio en dos o tres puntos**, y eso es honesto y alcanzable.
9. **Claude Code es una distracción para ella.** Una lección opcional que explica qué es y por qué no
   lo necesita, y si no la abre, el curso ha funcionado igual.
10. Todo el curso cuesta **cero euros**. Si acaba costando dinero, el diagnóstico estaba mal.

---

## 10. Lo que no he podido verificar

Listado explícito, para que nadie construya sobre arena:

- **El plan de Workspace de su empresa y su configuración.** El dato más importante del documento.
  Tarea del curso, no de esta investigación.
- **Precios exactos en euros en la web oficial de Google.** La página de precios sirve las cifras por
  JavaScript. Las de 8,10 / 16,20 / 25,30 € (facturación flexible, España) proceden de un revendedor
  y son **[S]**.
- **Precio del complemento "AI Expanded Access".** Aparece citado en material de Google, sin precio
  público localizable.
- **Límites exactos de Deep Research** (5/20/200 al mes): consistentes entre fuentes secundarias,
  no confirmados en una página oficial de límites.
- **Límite de fuentes de Gemini Notebook en Workspace** (se cita 400): **[S]**.
- **Límite de 100 MB por fichero de conocimiento de un Gem:** **[S]**. Lo confirmado oficialmente es
  el máximo de 10 ficheros.
- **Límite de 10 acciones programadas simultáneas:** **[S]**.
- **Si su empresa puede compartir Gems entre compañeros**, y si el administrador tiene pasos de
  Workspace Studio restringidos: depende de su consola.
- **Nombres de modelo de 2026** (Gemini 3.1 Pro, 3.6 Flash, etc.): aparecen en comparadores de
  precios que también inventan nombres de modelos de otros proveedores. **He evitado deliberadamente
  apoyar nada de este documento en el nombre del modelo**, que además es el detalle que menos
  importa: como decía el webinar de referencia, *"da bastante igual qué modelo uses"*.
- **Precio de ChatGPT Plus en 2026.** No investigado: irrelevante para la recomendación.
- **Observabilidad real de los flujos de Workspace Studio** cuando fallan a mitad. No hay
  documentación suficiente y es un riesgo práctico que solo se conocerá usándolo.

---

## Fuentes principales

Primarias (Google): [workspace.google.com/pricing](https://workspace.google.com/pricing) ·
[workspace.google.com/studio](https://workspace.google.com/studio/) ·
[Workspace Updates agosto 2026](https://workspaceupdates.googleblog.com/2026/08/) ·
[Workspace Updates: fórmulas en Sheets](https://workspaceupdates.googleblog.com/2026/06/troubleshoot-formula-errors-in-sheets.html) ·
[Workspace Updates: función AI en Sheets](https://workspaceupdates.googleblog.com/2025/06/generate-data-with-gemini-in-google-sheets.html) ·
[Guía de starters y steps de Workspace Studio](https://support.google.com/workspace-studio/answer/16765661?hl=en) ·
[Empezar con Workspace Studio](https://support.google.com/workspace-studio/answer/16444479?hl=en) ·
[Usar Gems](https://support.google.com/gemini/answer/15146780?hl=en&co=GENIE.Platform%3DDesktop) ·
[Acciones programadas](https://support.google.com/gemini/answer/16316416?hl=en&co=GENIE.Platform%3DDesktop) ·
[Límites de Gemini Notebook](https://support.google.com/notebooklm/answer/16213268?hl=en) ·
[NotebookLM es ahora Gemini Notebook](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook/) ·
[Gemini Apps Privacy Hub](https://support.google.com/gemini/answer/13594961?hl=en) ·
[Privacidad de IA generativa en Workspace](https://support.google.com/a/answer/15706919?hl=en) ·
[Data regions](https://knowledge.workspace.google.com/admin/compliance/choose-a-geographic-location-for-your-data) ·
[Qué edición tengo](https://support.google.com/a/answer/10975849?hl=en) ·
[Gemini en el editor de Apps Script](https://developers.google.com/apps-script/guides/gemini) ·
[Servidores MCP de Workspace](https://developers.google.com/workspace/guides/configure-mcp-servers) ·
[Gemini Spark](https://gemini.google/overview/agent/spark/) ·
[Transición de Gemini CLI a Antigravity CLI](https://github.com/google-gemini/gemini-cli/discussions/27274) ·
[Antigravity o Gemini CLI](https://cloud.google.com/blog/topics/developers-practitioners/choosing-antigravity-or-gemini-cli) ·
[Gemini Enterprise](https://cloud.google.com/gemini-enterprise)

Secundarias: [Reworked sobre Workspace Studio](https://www.reworked.co/digital-workplace/google-launches-workspace-studio-for-no-code-ai-automation/) ·
[Zenphi: Workspace Studio (antes Flows)](https://zenphi.com/what-is-google-workspace-studio-formerly-flows-latest-news/) ·
[9to5Google: renombrado de NotebookLM](https://9to5google.com/2026/07/16/notebooklm-gemini-notebook/) ·
[TechCrunch: Claude Cowork](https://techcrunch.com/2026/07/07/the-coding-agent-wars-are-spilling-into-the-rest-of-the-office-claude-cowork/) ·
[Precios Google Workspace España](https://10atm.com/precios-google-workspace/) ·
[Make pricing 2026](https://smartprocessflow.com/make-com-pricing) ·
[n8n pricing 2026](https://www.nocode.mba/articles/n8n-pricing) ·
[Zapier pricing 2026](https://www.nocode.mba/articles/zapier-pricing-2026) ·
[Power Automate pricing 2026](https://citizendevelopmentacademy.com/power-automate-pricing/) ·
[Gemini Enterprise pricing](https://coworker.ai/blog/gemini-enterprise-pricing)
