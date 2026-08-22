# Dominio — Protección de datos y uso seguro de IA en una academia de idiomas

**Para qué sirve este documento.** Es la materia prima del bloque *"manejar datos sensibles con
seguridad"*, que en el perfil de la alumna es uno de los tres objetivos, no un anexo legal. Aquí está
el marco, el inventario de datos de su empresa, la comparación real entre planes de consumo y planes
de empresa, y — lo más importante — las reglas que puede aplicar el lunes y los ejercicios con los
que se comprueba que las sabe aplicar.

Cubre además el hueco que `dominio-academia.md` deja abierto: aquella nota remite a *"ver sección 6"*
al hablar del matching alumno-familia y del RGPD, y esa sección 6 es esto.

**Fecha del análisis:** 22.08.2026. Todo lo normativo de la sección 1 caduca rápido; ver la nota de
caducidad al final de esa sección.

---

## Advertencia que el material debe llevar impresa

> **Esto no es asesoramiento jurídico y quien lo escribe no es tu abogada.** Es orientación general
> para que sepas qué preguntar, a quién y con qué palabras, y para que no metas la pata por
> desconocimiento en el uso diario. Las decisiones sobre qué base legal aplica a un tratamiento, qué
> contratos hay firmados, si hace falta una evaluación de impacto o cómo se responde a una brecha
> **las toma tu empresa**, normalmente con su asesoría de protección de datos.
>
> Tu papel no es ser la responsable de cumplimiento de la academia. Tu papel es: **no ser tú el
> agujero**, y saber detectar cuándo hay que levantar la mano.

A lo largo del documento se marca explícitamente cada bloque:

| Marca | Significado |
|---|---|
| **[D]** | **Documentado.** Verificado en fuente oficial o primaria en agosto de 2026. Fuentes en la sección 9. |
| **[R]** | **Reconstrucción razonada.** Deducción coherente con lo documentado, pero no publicado como tal. |
| **[V]** | **A verificar por ella** en su empresa. Es el material de los ejercicios. |
| **[NV]** | **No verificable desde fuera.** Depende del contrato concreto de su empresa o de configuración privada. Se dice claramente y no se rellena con suposiciones. |
| **[!]** | **Requiere profesional o decisión de empresa.** No es cosa suya resolverlo. |

---

## 1. El marco aplicable en 2026

### 1.1 Lo que hay, en una frase cada uno

| Norma | Qué regula | Estado en agosto de 2026 |
|---|---|---|
| **RGPD** (Reglamento UE 2016/679) | El tratamiento de datos personales. La columna vertebral. | Plenamente en vigor desde 2018 [D] |
| **LOPDGDD** (LO 3/2018) | Los añadidos españoles al RGPD. | En vigor [D] |
| **Reglamento de IA** (UE 2024/1689) | Los sistemas de IA, por nivel de riesgo. | Aplicación **escalonada**, y recién reordenada [D] |
| **Reglamento Ómnibus de IA** (UE 2026/1744) | Retoca el calendario del anterior. | Publicado en el DOUE el **24.07.2026**, en vigor el **27.07.2026** [D] |
| **Proyecto de Ley Orgánica española de gobernanza de la IA** | Autoridades, sandboxes y sanciones en España. | **Aún no es ley.** Aprobado en Consejo de Ministros el 26.05.2026, publicado en el Congreso el 12.06.2026, en tramitación [D] |

Dos cosas que conviene tener claras desde el principio y que la mayoría de artículos de prensa mezclan:

1. **El RGPD ya se aplica a todo lo que ella hace con IA.** No hace falta esperar a ninguna ley de IA.
   Pegar el pasaporte de un alumno en un chat es un tratamiento de datos personales, y lo era en 2019.
2. **El Reglamento de IA no sustituye al RGPD, se suma.** Regula el *sistema*; el RGPD regula los
   *datos*. Se puede cumplir uno e incumplir el otro.

### 1.2 RGPD: los seis puntos que de verdad tocan a su puesto

No hace falta que se sepa el reglamento. Necesita seis ideas.

**1. Dato personal es cualquier cosa que permita identificar a alguien**, directamente o combinando
piezas. El nombre, sí; pero también "la chica coreana de 19 años que llegó el 3 de julio y está en
casa de la familia de Chamberí". Eso identifica a una persona entre 1.400. [D — art. 4.1 RGPD]

**2. Responsable y encargado no son lo mismo, y esta distinción es la que sostiene todo el documento.** [D — arts. 4.7, 4.8 y 28 RGPD]
- **Responsable del tratamiento**: quien decide para qué y cómo se usan los datos. **Aquí, la academia.**
- **Encargado del tratamiento**: quien trata los datos *por cuenta* del responsable y solo siguiendo sus
  instrucciones. Un proveedor.
- Para que un proveedor sea encargado **tiene que haber un contrato por escrito** con el contenido que
  exige el artículo 28.3. Sin contrato no hay encargado: hay una cesión de datos a un tercero sin
  amparo. Esa es, literalmente, la diferencia entre Gemini con la cuenta de empresa y ChatGPT con la
  cuenta personal.

**3. Minimización.** Solo los datos necesarios para lo que estás haciendo. [D — art. 5.1.c] Es el
principio más útil de todos en el día a día, porque es **operativo**: antes de pegar algo, la pregunta
no es "¿tengo permiso?", es *"¿hace falta esto para lo que le estoy pidiendo?"*. Casi nunca hace falta.

**4. Categorías especiales.** Hay datos que están prohibidos por defecto y solo se pueden tratar si
encaja una de las excepciones tasadas del artículo 9.2. Ver sección 2.2, porque en una academia con
alojamiento hay más de los que parece. [D — art. 9 RGPD]

**5. Transferencias fuera del EEE.** Mandar datos a un servidor de EE. UU. es una transferencia
internacional y necesita cobertura: decisión de adecuación, cláusulas contractuales tipo, etc.
[D — cap. V RGPD] Hoy la cobertura principal con EE. UU. es el **Marco de Privacidad de Datos UE-EE. UU.**
(*Data Privacy Framework*), y sobre su solidez ver 1.5.

**6. Brechas de seguridad.** Si hay una violación de seguridad con riesgo para las personas, el
responsable debe notificarlo a la AEPD **en 72 horas**. [D — art. 33 RGPD] Que un empleado vuelque
datos de clientes en una herramienta no contratada por la empresa **puede constituir una brecha
notificable** [R], y la responsabilidad recae en la empresa, no en el empleado. Este es el argumento
que hace que el punto 5 de este documento no sea un sermón.

### 1.3 LOPDGDD: qué añade España

Poco, pero relevante para una academia:

- **Edad de consentimiento: 14 años.** Por debajo de 14, el consentimiento lo dan quienes ejerzan la
  patria potestad o tutela. [D — art. 7 LOPDGDD] El RGPD deja elegir entre 13 y 16; España eligió 14.
- **Deber de confidencialidad** de quien interviene en el tratamiento, que se mantiene después de
  terminar la relación laboral. [D — art. 5 LOPDGDD]
- **Delegado de protección de datos (DPD).** No es obligatorio para toda pyme; depende de la actividad.
  Los centros educativos sí están en la lista de entidades que deben designarlo. [D — art. 34.1.b
  LOPDGDD] **[V]** ¿Su academia tiene DPD designado y comunicado a la AEPD? Es una pregunta con
  respuesta binaria y muy fácil de hacer, y si la hay, esa persona es su interlocutor natural.

### 1.4 Reglamento de IA: qué está en vigor de verdad hoy

Este es el punto donde más desinformación hay, porque el calendario cambió hace tres semanas.

**Calendario real tras el Ómnibus (Reglamento UE 2026/1744):** [D]

| Fecha | Qué empezó / empieza a aplicarse | Estado |
|---|---|---|
| 02.02.2025 | **Prohibiciones** del art. 5 (usos vedados) y **alfabetización en IA** del art. 4 | **En vigor** |
| 02.08.2025 | Obligaciones de los **modelos de propósito general** (GPAI), gobernanza | **En vigor** |
| **02.08.2026** | **Transparencia del art. 50**: avisar de que se está hablando con una IA, etiquetar contenido sintético, revelar deepfakes | **En vigor desde hace tres semanas** |
| ~~02.08.2026~~ → **02.12.2027** | Sistemas de **alto riesgo del Anexo III** (bloque íntegro) | **Aplazado** |
| ~~02.08.2027~~ → **02.08.2028** | Alto riesgo del **Anexo I** (IA embebida en productos ya regulados) | **Aplazado** |

Tres consecuencias concretas para la academia:

**(a) El artículo 4 ya la obliga, y va sobre ella.** El Reglamento exige a proveedores y a
*responsables del despliegue* —es decir, empresas que usan IA— garantizar un **nivel suficiente de
alfabetización en IA** de su personal. Está en vigor desde febrero de 2025. [D] Dicho de otro modo:
**el curso que está haciendo es, técnicamente, cumplimiento normativo de su empresa.** Es un detalle
que merece salir en el material, porque cambia la posición mental con la que se estudia esto.

**(b) El artículo 50 ya la obliga si automatiza respuestas a clientes.** Desde el 02.08.2026 hay que
informar a la persona de que está interactuando con un sistema de IA, salvo que resulte evidente. [D]
Si mañana monta un asistente que contesta primeros correos del buzón `info@`, **el aviso no es
opcional**. Diseño derivado: la línea de aviso va en la plantilla desde el primer día, no como parche.

**(c) Y esta es la que casi nadie ve: una academia puede acabar en el Anexo III.** El Anexo III incluye
como alto riesgo, en el ámbito de educación y formación profesional, los sistemas destinados a: [D]

- determinar el **acceso o la admisión** a centros educativos;
- **evaluar los resultados del aprendizaje**;
- **evaluar el nivel educativo** adecuado que recibirá una persona o al que podrá acceder;
- **vigilar comportamientos prohibidos durante exámenes**.

Traducido a su inventario de procesos: **P05 (test de nivel y asignación de grupo MCER)** y **P16
(exámenes DELE/SIELE)** están en esa lista. Si algún día se automatiza la nivelación con IA, eso no es
"una automatización más": es un sistema de alto riesgo con obligaciones de documentación, supervisión
humana, registro y calidad de datos. Hoy **no es exigible** —está aplazado al **02.12.2027**— pero la
fecha llega. **[!]** Decisión de empresa, no suya. Lo que sí es suyo es **saber reconocerlo y avisar**.

> **Regla de oro para el curso:** de todo el proceso de la academia, el trocito que decide *el nivel de
> un alumno* es el único que está en la lista de alto riesgo. Todo lo demás —redactar, traducir,
> resumir, clasificar correos, preparar borradores— no lo está. Esa asimetría es fácil de recordar y
> es lo que hay que enseñar.

### 1.5 Transferencias a EE. UU.: por qué esto no está cerrado

Estado a agosto de 2026 [D]:

- La decisión de adecuación del **Marco de Privacidad de Datos UE-EE. UU. (DPF)** de 2023 **sigue
  vigente**. El Tribunal General de la UE desestimó en septiembre de 2025 el recurso de anulación
  (asunto *Latombe*).
- Pero **hay recurso de casación pendiente ante el TJUE** (asunto C-703/25 P, interpuesto el
  31.10.2025), sin fecha de vista anunciada. Los análisis especializados sitúan una sentencia en
  2027 [R].
- El TJUE es el tribunal que ya tumbó *Safe Harbor* (2015) y *Privacy Shield* (2020).

**Qué significa esto en lenguaje llano, y es lo único que ella necesita retener:** hoy es legal apoyarse
en proveedores estadounidenses con las garantías adecuadas, pero **es la tercera vez que se monta este
marco y las dos anteriores se cayeron**. Por eso la opción de procesar en la UE, cuando existe, no es
un capricho: es lo que hace que un cambio de jurisprudencia no te obligue a rediseñarlo todo. [R]

### 1.6 Nota de caducidad

Todo el apartado 1 tiene fecha de caducidad corta. Lo que cambiará previsiblemente antes de un año:
el estado de la ley española de IA, la fecha efectiva del Anexo III (ya se movió una vez y podría
moverse otra), y el DPF si el TJUE resuelve. **El curso no debe congelar estas fechas dentro de un
prompt ni de una plantilla.** Van en un fichero de contexto con fecha visible, y se revisan. Este es,
además, un buen ejemplo pedagógico de la diferencia entre *conocimiento estable* (los seis principios
de 1.2) y *conocimiento volátil* (las fechas), que es exactamente la distinción que hay que enseñar
para construir bases de conocimiento que no envejezcan mal.

---

## 2. Qué datos maneja realmente una academia con estudiantes extranjeros

### 2.1 Inventario, por proceso

Cruzando con el inventario P01–P32 de `dominio-academia.md`:

| Dato | Dónde aparece | Categoría | Nivel |
|---|---|---|---|
| Nombre, apellidos, fecha de nacimiento | Todos | Personal ordinario | Amarillo |
| **Nº de pasaporte, NIE, copia del documento** | P04, P08, P10, P21 | Personal ordinario, pero **identificador oficial** | **Rojo** |
| Nacionalidad y país de origen | P01–P08, P31 | Ordinario, pero puede **revelar origen étnico o racial** por combinación | Rojo si va combinado |
| Dirección en origen y dirección de alojamiento en Madrid | P07, P18, P21 | Ordinario, pero **localiza físicamente a la persona** | **Rojo** |
| Teléfono, email, WhatsApp | Todos | Ordinario | Amarillo |
| Fechas exactas de estancia, vuelo, hora de llegada | P07, P18, P19 | Ordinario, pero **localiza en el tiempo** | Rojo si va con dirección |
| Datos de pago, IBAN, tarjeta, justificantes | P02, P06, P25, P21 | Ordinario, **pero con riesgo de fraude directo** | **Rojo absoluto** |
| Situación económica, becas, impagos | P06, P25 | Ordinario, sensible en la práctica | Rojo |
| **Alergias, intolerancias, dieta médica** | P17, P20, P29 | **Categoría especial: salud** (art. 9) | **Rojo absoluto** |
| **Medicación, condiciones crónicas, ficha médica** | P29 | **Categoría especial: salud** | **Rojo absoluto** |
| **Dieta halal / kosher, prácticas religiosas** | P17 | **Categoría especial: convicciones religiosas** | **Rojo absoluto** |
| **Preferencias de convivencia que revelan orientación sexual** | P17, P20 | **Categoría especial** | **Rojo absoluto** |
| Datos de **menores** (y de sus tutores) | P11, P15, P17, P20, P29 | Ordinario, pero **régimen reforzado** | **Rojo absoluto** |
| Notas, asistencia, nivel MCER | P05, P10, P11 | Ordinario + posible **decisión que afecta** al alumno | Rojo |
| Contenido de quejas y reclamaciones | P26 | Ordinario, pero puede arrastrar salud o convivencia | Rojo |
| Grabaciones de llamadas | P29, atención telefónica | Ordinario (voz); puede contener salud | **Rojo** |
| Datos de **familias de acogida** (dirección, composición del hogar, mascotas, tabaco, historial) | P17, P23 | Ordinario + **datos del hogar de un tercero** | **Rojo** |
| Comentarios libres de encuestas | P27 | Depende; suelen ser anónimos o seudonimizables | **Verde tras limpieza** |
| Tarifas, calendario, condiciones, plantillas | P01, P02, P32 | **No son datos personales** | **Verde** |

Dos observaciones que ordenan todo lo demás:

- **La academia no maneja "algunos" datos sensibles. Maneja el paquete completo.** Identificación
  oficial, salud, religión, menores, dinero y domicilio, todo a la vez y sobre la misma persona. Es un
  perfil de riesgo más parecido al de una pequeña clínica o una agencia de viajes con visados que al de
  una empresa de servicios normal. Conviene decirlo así en el curso, sin dramatismo pero sin rebajarlo.
- **Y a la vez tiene un proceso perfectamente limpio: P27, las encuestas de satisfacción.** Volumen
  alto, multilingüe, riesgo bajo, sin dinero ni plazos legales, y seudonimizable de verdad. En
  `dominio-academia.md` ya se identificaba como el mejor primer proyecto por razones operativas. Desde
  el punto de vista de protección de datos **la conclusión es idéntica**, y esa coincidencia es un
  regalo para el diseño del curso: el primer proyecto es a la vez el más útil y el más seguro.

### 2.2 Categorías especiales: cuáles son y por qué lo cambia todo

El artículo 9.1 del RGPD prohíbe, **por defecto**, tratar datos que revelen: [D]

> origen étnico o racial · opiniones políticas · convicciones religiosas o filosóficas · afiliación
> sindical · datos genéticos · **datos biométricos dirigidos a identificar de manera unívoca a una
> persona** · **datos relativos a la salud** · datos sobre la vida sexual o la orientación sexual.

**Por qué "cambia todo" no es una exageración:**

1. **Se invierte la lógica.** Con un dato normal, buscas una base legal entre las seis del art. 6. Con
   una categoría especial, **primero está prohibido** y solo se levanta la prohibición si encaja una de
   las diez excepciones del art. 9.2 (consentimiento explícito, intereses vitales, etc.). Son dos
   pisos, no uno.
2. **El consentimiento tiene que ser explícito**, no basta el implícito o el "al reservar acepta". [D]
3. **Sube el listón de seguridad y de evaluación previa.** El tratamiento a gran escala de categorías
   especiales es uno de los criterios que empujan hacia una evaluación de impacto (EIPD, art. 35). [D]
   **[!]** Determinar si su academia necesita una EIPD para un proyecto concreto no es cosa suya.
4. **Sube el rango sancionador y el daño reputacional.** Filtrar una lista de emails es feo. Filtrar
   una lista de alergias, medicación y religión de menores extranjeros es otra cosa completamente
   distinta.

**Dónde se cuelan sin que nadie lo note, en su trabajo concreto:**

- **P17, matching con familia de acogida.** El formulario de preferencias del alumno es, en la
  práctica, un formulario de datos de categoría especial disfrazado de logística: "vegetariano / sin
  gluten / alérgico a los gatos / no como cerdo / prefiero una casa sin fumadores / vengo con mi
  pareja". Ahí hay salud, religión y potencialmente orientación sexual, en una misma casilla de texto
  libre. Por eso `dominio-academia.md` marcaba el matching como **trampa** para un primer proyecto de
  IA: es el proceso más goloso (decisión compleja, muchos criterios, dolor real) y el más peligroso.
- **P20, incidencias de alojamiento.** "No come lo que le ponen" puede ser un capricho o una
  intolerancia diagnosticada. "No se encuentra bien" puede ser morriña o un problema de salud mental.
  La incidencia se escribe en texto libre y ahí aterriza todo.
- **P29, emergencias.** Salud pura, y además bajo presión. Zona prohibida para automatización, sin
  matices.
- **Alergia alimentaria comunicada a la familia de acogida.** Esto es además una **comunicación de
  datos de salud a un tercero** (la familia), necesaria y legítima, pero que exige que exista un
  encuadre por escrito. **[!]** Eso ya está resuelto o no en su empresa; no lo resuelve ella.

**Un matiz técnico que evita un error común:** grabar la voz de alguien **no** convierte el dato en
biométrico automáticamente. Es dato biométrico del art. 9 cuando el tratamiento **está dirigido a
identificar de manera unívoca** a la persona (huella de voz, reconocimiento del hablante). Transcribir
una llamada para resumirla no es eso. [D — art. 4.14 RGPD] Ahora bien, **el contenido** de esa llamada
sí puede ser categoría especial, y normalmente lo es en una llamada de incidencia. Ver 6.5.

### 2.3 Menores: el régimen reforzado

Una academia de español con turistas y estudiantes tiene menores con más frecuencia de la que sugiere
el organigrama: programas de verano, grupos escolares (recordemos, **41,5 % viaja en grupo** [D, FEDELE]),
y estancias de 16-17 años en familia.

Lo que cambia [D]:
- Consentimiento propio solo desde los **14 años** (art. 7 LOPDGDD); por debajo, tutores.
- El RGPD pide que la información dirigida a menores esté **en lenguaje claro y adaptado** (art. 12).
- El considerando 38 subraya que los menores merecen **protección específica** porque son menos
  conscientes de los riesgos.
- La AEPD insiste explícitamente en **no usar imágenes de menores** en herramientas de IA.

Regla práctica para el curso, deliberadamente tajante y sin excepciones: **si hay un menor implicado,
sus datos no entran en ninguna herramienta de IA. Ni seudonimizados. Se trabaja con el caso descrito en
abstracto o no se trabaja.** Es más restrictivo de lo que la norma exige en todos los supuestos, y es
a propósito: una regla con excepciones no sobrevive a un martes de julio con 300 correos.

### 2.4 El semáforo: la herramienta operativa

Todo lo anterior tiene que colapsar en algo que quepa en una nota adhesiva al lado de la pantalla.

> **🟢 VERDE — entra sin pensar.**
> Información de la empresa que no identifica a nadie: tarifas, calendario académico, condiciones
> generales, normas de convivencia, plantillas, el texto de la FAQ, políticas de cancelación, tu propio
> borrador redactado en tercera persona, listas de precios, textos de marketing.
>
> **🟡 ÁMBAR — entra solo con la cuenta de empresa y solo si hace falta.**
> Un caso real contado sin identificadores. Un correo de cliente con el nombre, el email, la dirección
> y las fechas ya quitados. Datos agregados ("de 40 respuestas, 12 mencionan el ruido"). Un texto que
> traduces y que no contiene datos de nadie.
>
> **🔴 ROJO — no entra nunca, en ninguna herramienta, ni siquiera en la de empresa, salvo que exista
> una instrucción escrita de tu empresa que lo autorice.**
> Pasaportes y NIE (número o imagen) · IBAN, tarjetas y justificantes de pago · alergias, dietas
> médicas, medicación, cualquier tema de salud · religión y prácticas religiosas · cualquier dato de un
> **menor** · direcciones de alojamiento junto a nombres · datos de las **familias de acogida** ·
> grabaciones de llamadas sin tratar · cualquier documento que **no hayas abierto y leído entero**.

**Por qué el rojo dice "ni siquiera en la de empresa".** Porque el hecho de que la herramienta esté
contratada resuelve la pregunta del *proveedor*, no la del *tratamiento*. Que Google sea encargado del
tratamiento no legitima que la academia pase pasaportes por un chat si su registro de actividades de
tratamiento no lo contempla. **[!]** Ampliar el rojo es una decisión de empresa, y su forma correcta es
una instrucción escrita, no un "me dijeron que sí". El curso enseña a pedirla, no a asumirla.

---

## 3. LA PREGUNTA CENTRAL: consumo frente a empresa

### 3.1 Las cuatro preguntas que definen un plan

Todo el ruido de marketing se reduce a cuatro preguntas. Enseñarle **las preguntas** vale más que
enseñarle la tabla, porque la tabla caduca y las preguntas no.

1. **¿Entrenan sus modelos con lo que yo escribo?**
2. **¿Cuánto tiempo guardan mis conversaciones, y quién decide ese plazo?**
3. **¿Dónde se procesan y se almacenan los datos? ¿Puedo exigir la UE?**
4. **¿El proveedor firma como encargado del tratamiento, con contrato del art. 28?**

Y una quinta que no es del plan sino de la empresa, y que suele ser la que decide de verdad:
**¿mi empresa ha activado y configurado esto, y ha dejado dicho por escrito qué se puede meter?**

### 3.2 Gemini dentro de Google Workspace — su caso probable, en detalle

Es el escenario más probable según el perfil ("en su empresa se usa Gemini de pago"), y también el más
malinterpretado, porque **"Gemini de pago" puede significar al menos cuatro cosas distintas**.

#### 3.2.1 El mecanismo que hay que entender: servicio principal frente a servicio adicional

Esta es la pieza clave y casi nadie la conoce.

Dentro de Google Workspace, una aplicación puede estar disponible de dos maneras: [D]

- Como **servicio principal** (*core service*): queda cubierta por el **acuerdo de Google Workspace** y
  por el **Cloud Data Processing Addendum (CDPA)**. Google actúa como **encargado del tratamiento**,
  con las obligaciones del art. 28.3 del RGPD trasladadas también a sus subencargados, y con cláusulas
  contractuales tipo para las transferencias. [D]
- Como **servicio adicional**: se rige por las **condiciones generales de Google**, no por el acuerdo de
  Workspace. Es, a efectos prácticos, terreno de consumo con una cuenta de trabajo. [D]

Desde octubre de 2024, la aplicación Gemini es **servicio principal con protección de datos de nivel
empresarial** en la mayoría de ediciones de Workspace. [D] Pero un administrador puede además permitir
el acceso a usuarios **sin licencia**, y en ese caso acceden como **servicio adicional**. [D]

**Consecuencia:** dos personas de la misma academia, escribiendo en la misma pantalla de
`gemini.google.com` con la misma cuenta `@academia.es`, pueden estar bajo dos regímenes jurídicos
distintos. Por eso el ejercicio de la sección 4 no es burocracia: es la diferencia entre estar cubierta
y no estarlo.

#### 3.2.2 Los compromisos, cuando sí está cubierta

Con protección de datos de nivel empresarial, Google se compromete a: [D]

- **No usar los datos del cliente para entrenar ni ajustar sus modelos generativos sin permiso o
  instrucción previa del cliente.** Literal de la documentación de Workspace: *"Workspace does not use
  customer data for training models without customer's prior permission or instruction."*
- **Sin revisión humana fuera del dominio.** *"Your chats and uploaded files won't be reviewed by human
  reviewers or otherwise used to train generative AI models outside of your domain without permission."*
- Los prompts se consideran **customer data** bajo el CDPA, y Google *"only accesses and processes
  customer data in accordance with customer instruction as set out in the CDPA"*.
- Certificaciones: SOC 1/2/3, ISO 27001/27017/27018/27701, ISO 42001, BSI C5. [D]

#### 3.2.3 Retención: la decide su administrador, no Google

| Superficie | Retención | Quién decide |
|---|---|---|
| Gemini **en las apps** (panel lateral, "Ayúdame a escribir") | de **90 días a indefinido** | **El administrador** [D] |
| **Aplicación** Gemini (gemini.google.com) | hasta **36 meses**; autoborrado configurable a **3, 18 o 36 meses** | **El administrador** [D] |
| **Gemini Notebook** | no se retiene al terminar la sesión [D] | — |

Léase despacio: **"indefinido" es una opción real y, en muchas organizaciones, la que viene por
defecto**. Si la academia no la ha tocado, todo lo que ella pegue en Gemini puede quedar guardado sin
fecha de caducidad, dentro del dominio, y ser recuperable. Eso no es ilegal —sigue siendo dato del
cliente bajo su control— pero **contradice el principio de limitación del plazo de conservación** si
nadie lo ha pensado, y convierte cada pegado descuidado en un depósito permanente. **[V]** Pregunta
directa para su administrador, y de las que sorprenden por cómo se responden.

#### 3.2.4 Ubicación de los servidores: aquí está el matiz que casi todo el mundo ignora

Google ofrece **regiones de datos** (elegir UE, EE. UU. o ambas). Pero **la cobertura de Gemini por
regiones de datos llegó tarde y no está en todas las ediciones**: [D]

| Superficie | Desde | Ediciones con regiones de datos |
|---|---|---|
| **Funciones** de Gemini en las apps (panel lateral, "Ayúdame a escribir") | 09.06.2025 | **Enterprise Plus**, y clientes con el complemento **Assured Controls / Assured Controls Plus** |
| **Aplicación** Gemini (gemini.google.com) | 29.06.2026 | **Enterprise Plus**, Education Plus, Education Standard (solo almacenamiento), **Frontline Plus** |
| **Gemini Notebook** | — | **Los ajustes de región de la organización NO se aplican** [D] |

**Traducción para una academia de 30 personas, que casi con seguridad está en Business Standard o
Business Plus [R]:**

> Muy probablemente tiene el compromiso de **no entrenamiento** y a Google como **encargado del
> tratamiento** — que es lo importante — pero **NO tiene garantizado el procesamiento en la UE para
> Gemini**. Son dos cosas distintas y conviene no confundirlas. Las "regiones de datos fundamentales"
> que se incluyen en Business Standard y Plus cubren el contenido de Workspace [R, no verificado para
> Gemini]; la cobertura específica de Gemini exige Enterprise Plus o el complemento Assured Controls.

Esto no es un problema legal automático: el DPF y las cláusulas contractuales tipo dan cobertura hoy
(ver 1.5). Es un dato de arquitectura que conviene conocer antes de decidir qué se mete ahí.

#### 3.2.5 Cómo se comprueba desde la pantalla, en 30 segundos

Google publica un método directo y esto es oro para un ejercicio: [D]

1. Entrar en `gemini.google.com` con la cuenta **de trabajo**.
2. Mirar el **distintivo en la parte superior**.

| Lo que ve | Qué significa |
|---|---|
| **Pro**, **Expanded** o **Ultra** | *"Tus conversaciones y los archivos que subas no los examinarán revisores humanos ni se usarán para mejorar modelos de IA generativa"* |
| **Sin distintivo** | Acceso estándar: *"Tus conversaciones... las podrán examinar revisores humanos y se podrán usar para mejorar productos"* — y toca hablar con el administrador |

**Honestidad sobre una tensión que he encontrado en las fuentes [NV]:** el anuncio de octubre de 2024
dice que la app Gemini es servicio principal con protección empresarial para Business Starter,
Standard, Plus, Enterprise Starter, Standard y Plus. La página de ayuda vigente en 2026 describe, en
cambio, niveles por distintivo donde "sin distintivo" **no** lleva esas protecciones. La lectura más
razonable [R] es que "sin distintivo" corresponde a usuarios **sin licencia asignada**, que acceden como
servicio adicional. No puedo verificarlo con certeza desde fuera. **Lo que sí es seguro y es lo que se
enseña: si no ve distintivo, no debe asumir que está protegida — debe preguntar.**

#### 3.2.6 Y una advertencia sobre el nombre "Gemini Enterprise"

Ojo, porque el nombre confunde y va a aparecer en cualquier conversación con IT [D/R]:

- **Gemini incluido en Google Workspace** — lo que casi seguro tiene su empresa. Desde enero de 2025
  Google eliminó los complementos de pago y metió Gemini dentro de los planes de Workspace, subiendo el
  precio base. [D]
- **Gemini Enterprise / Gemini Business** — un **producto distinto de Google Cloud**, con plataforma de
  agentes, y precios por puesto del orden de 21–30 $/mes [R, cifras de fuentes secundarias, no
  verificadas en la lista oficial]. No es lo mismo que "tener Gemini en Workspace".
- **Gemini Advanced / suscripción Google AI personal** — plan de **consumo**, con cuenta personal.
- **Google AI Studio / API de Gemini** — herramienta de desarrollo, con reglas propias y peligrosas en
  su versión gratuita (ver 3.3).

Cuando alguien de la academia diga "tenemos Gemini de pago", **puede referirse a cualquiera de las
cuatro**. Desambiguar eso es literalmente el objetivo del ejercicio de la sección 4.

### 3.3 La tabla comparativa

Estado a agosto de 2026. Las casillas dudosas van marcadas.

| | ¿Entrena con tus datos? | Retención | Ubicación | ¿Encargado del tratamiento (art. 28)? |
|---|---|---|---|---|
| **Gemini con cuenta personal** (gratis o suscripción de consumo) | **Sí.** Se usan para *"ofrecer, desarrollar y mejorar sus servicios, lo cual incluye entrenar los modelos"* [D] | Configurable; **si un revisor humano lee una conversación, se guarda hasta 3 años** desasociada de la cuenta [D]. Y aunque se desactive la actividad, **72 h** siempre [D] | Global | **No.** Google es responsable de su propio tratamiento |
| **Gemini en Workspace, con licencia** (servicio principal) | **No**, sin permiso previo del cliente [D] | **90 días → indefinido** (apps) / hasta **36 meses** (app), lo fija el **administrador** [D] | UE garantizada **solo en Enterprise Plus / Assured Controls** [D]. En Business, no garantizada | **Sí**, vía **CDPA** [D] |
| **Gemini en Workspace, sin licencia** (servicio adicional) | **[NV]** Se rige por condiciones generales de Google, no por el acuerdo de Workspace [D]. Trátese como consumo | — | — | **No, o no claramente** |
| **Google AI Studio / API — nivel gratuito** | **Sí.** Los términos advierten literalmente: *"No envíes información sensible, confidencial o personal"*, y revisores humanos pueden leer, anotar y procesar entradas y salidas [D] | — | — | **No** |
| **API de Gemini — nivel de pago** | **No** se usan prompts ni respuestas para mejorar productos [D] | Registro limitado para detectar abusos [D] | Configurable | Sí, vía CDPA [R] |
| **ChatGPT gratis / Plus / Pro (personal)** | **Sí por defecto**; hay un interruptor en Ajustes → Controles de datos [D] | Chats borrados y temporales: **30 días** [D] | EE. UU. por defecto | **No** |
| **ChatGPT Business** (antes *Team*) | **No por defecto**, y con respaldo contractual [D] | Del contrato | **Sin opción de residencia europea** [R, fuente secundaria] | **Sí**, DPA con cobertura del art. 28 [D] |
| **ChatGPT Enterprise / Edu** | **No** | Duración del contrato; retención cero solo por contrato [R] | **Residencia europea (EEE + Suiza) disponible** [D] | **Sí** |

**Dos cosas de esta tabla merecen subrayado en el material:**

**(a) El nivel gratuito de AI Studio es la trampa más silenciosa de todo el panorama.** Es de Google,
tiene aspecto profesional, se entra con la cuenta de Google y es gratis. Y sus propios términos dicen
que no metas información personal. Alguien que "está aprendiendo IA" y se topa con AI Studio puede
acabar pegando ahí lo que jamás pegaría en un chat de consumo. **Merece un aviso explícito en el curso.**

**(b) "No entrenamos con tus datos" no significa "tus datos son inaccesibles".** El caso *OpenAI vs.
New York Times* lo demuestra: la orden inicial de preservación indefinida terminó en septiembre de
2025, pero en enero de 2026 un tribunal federal de Nueva York confirmó la obligación de entregar una
muestra de **20 millones de conversaciones de usuarios**, desidentificadas, a la parte demandante, y la
primera remesa se entregó ese mismo mes. [D] Son conversaciones de plan de consumo. La lección para el
curso no es "OpenAI es mala": es que **un chat no es un espacio privado, es un registro que puede
acabar en manos de un tercero por vías que no dependen de la política de privacidad**. Y "desidentificado"
hace mucho trabajo en esa frase — ver la sección 6.2 sobre por qué quitar el nombre no basta.

### 3.4 Lo que no puedo verificar, dicho claramente

Honestidad obligatoria, y además pedagógicamente útil: enseña que la respuesta correcta a veces es
"no lo sé, y así se averigua".

- **[NV] Qué edición exacta de Workspace tiene su academia.** Solo se ve desde la consola de
  administración. Es el ejercicio de la sección 4.
- **[NV] Si su cuenta tiene licencia de Gemini asignada** o accede como servicio adicional.
- **[NV] Cómo está configurada la retención.** El rango va de 90 días a indefinido y lo fija su
  administrador.
- **[NV] Si tienen el complemento Assured Controls** y por tanto procesamiento en la UE para Gemini.
- **[NV] Si existe una política interna escrita** sobre qué se puede meter en la IA, y si hay registro
  de actividades de tratamiento que contemple el uso de IA.
- **[NV] Si hay DPD designado.**
- **[R, no verificado] Los precios y desgloses por edición de la sección 3.2.6** proceden de fuentes
  secundarias (blogs de consultoras), no de la lista oficial de Google. Sirven para orientarse en una
  conversación, no para citarlos como dato.
- **[NV] Si la academia tiene contratado ChatGPT de empresa además de Gemini.** El perfil dice que
  Gemini es *"en principio, la única"* herramienta recomendada, y ese "en principio" es exactamente lo
  que hay que despejar.

---

## 4. EJERCICIO: averiguar qué tiene contratado tu empresa

> **Ejercicio E-01 · "¿Qué tengo yo exactamente?"**
> Momento: **primera semana del curso**, antes de cualquier automatización.
> Tiempo: 25 minutos tuyos + una conversación de 5 minutos con otra persona.
> Se autocorrige con la rúbrica del final. No necesitas que nadie te lo valide.

**Por qué esto va primero y no al final.** Porque de la respuesta depende todo lo demás. Si resulta que
tu cuenta no tiene licencia de Gemini, cambia lo que puedes meter ahí. Si la retención está en
"indefinido", cambia cómo escribes. Si hay una política interna que no conocías, cambia el curso
entero. Montar automatizaciones antes de saber esto es construir sobre un suelo que no has mirado.

**Tono.** No estás pidiendo permiso para nada. **Ya usas Gemini, tu empresa te lo ha dado, y usarlo
está bien visto.** Estás haciendo lo que hace alguien que se toma en serio su herramienta: entender la
configuración antes de apoyarse en ella. Si acaso, esta conversación te deja mejor, no peor. Y si la
academia nunca se lo ha planteado, se lo estás planteando tú, que es aún mejor.

### Fase 1 — Lo que puedes averiguar sola, sin hablar con nadie (10 min)

Anota las respuestas en un fichero. Ese fichero es el entregable.

| # | Qué haces | Qué anotas |
|---|---|---|
| 1 | Entra en `gemini.google.com` **con la cuenta de la academia** (comprueba arriba a la derecha que no es la personal) | Correo con el que has entrado |
| 2 | Mira el **distintivo** arriba: ¿pone **Pro**, **Expanded**, **Ultra**, o no hay nada? | El distintivo exacto, o "ninguno" |
| 3 | Busca en la propia interfaz el aviso sobre datos (suele estar en el pie o en el menú de la conversación) | ¿Dice algo sobre revisión humana o entrenamiento? Cópialo literal |
| 4 | Entra en Gmail o Docs de trabajo y mira si aparece el **panel lateral de Gemini** o "Ayúdame a escribir" | Sí / No, y en qué apps |
| 5 | Comprueba si `admin.google.com` te deja entrar con tu cuenta | Casi seguro que no. Anótalo: **te dice quién manda** |
| 6 | Busca en tu correo, intranet o carpetas compartidas: "protección de datos", "política", "IA", "inteligencia artificial", "confidencialidad", "Workspace" | Lista de lo que encuentres, aunque sea de 2019 |
| 7 | Revisa qué firmaste al entrar en la empresa: ¿había cláusula de confidencialidad o política de uso de sistemas? | Sí / No / No lo encuentro |

**Ya con esto tienes media respuesta**, y no has hablado con nadie.

### Fase 2 — A quién preguntar

En una empresa de 30 personas no hay departamento de IT. La persona que administra Google Workspace es
casi siempre una de estas tres [R]:

| Quién | Probabilidad | Qué sabe |
|---|---|---|
| **Administración / la persona que lleva facturas y proveedores** | Alta | Qué se paga y qué plan es. **Empieza por aquí** |
| **El informático externo o la asesoría que montó los correos** | Alta | La configuración técnica real |
| **Gerencia / dirección** | Media | Quién decidió y qué se firmó |
| **Asesoría legal o DPD**, si existe | Baja pero decisiva | Si hay registro de tratamientos y política de IA |

**Estrategia:** primero administración (sabe qué se factura), y que ella te diga quién toca la consola.

### Fase 3 — Las palabras exactas

Están escritas para copiarlas y pegarlas. Toda la formulación descansa en un mismo movimiento: **tú
aportas algo, no pides algo.**

---

**Mensaje 1 — a administración (email o chat interno)**

> Asunto: Duda rápida sobre nuestro plan de Google Workspace
>
> Hola [nombre]:
>
> Estoy montando un par de cosas con Gemini para agilizar la respuesta de correos de admisiones y
> quiero configurarlo bien desde el principio. Para eso necesito dos datos que seguro que tienes tú a
> mano:
>
> 1. ¿Qué edición de Google Workspace tenemos contratada? (Business Starter, Business Standard,
>    Business Plus, Enterprise…)
> 2. ¿Mi cuenta tiene licencia de Gemini asignada, o accedo sin licencia?
>
> Con eso ya sé qué puedo apoyar en la herramienta y qué no. Gracias.

*Por qué funciona:* abre con trabajo hecho, la pregunta es concreta y de una sola respuesta, y no
menciona ni permiso ni riesgo ni legal.

---

**Mensaje 2 — a quien administre Workspace (el bloque técnico)**

> Hola [nombre]:
>
> Estoy usando Gemini para preparar borradores y quiero asegurarme de que lo estoy usando como toca.
> ¿Me confirmas estos cuatro puntos cuando puedas?
>
> 1. **Edición** de Workspace y **si mi usuario tiene licencia de Gemini** (o si accede como servicio
>    adicional).
> 2. **Retención** de las conversaciones de Gemini en la consola: ¿está en 3, 18 o 36 meses, o en
>    indefinido?
> 3. **Regiones de datos**: ¿tenemos configurada la UE, y aplica también a Gemini? (Por lo que he
>    leído, para Gemini eso solo está disponible en Enterprise Plus o con el complemento Assured
>    Controls.)
> 4. ¿Hay alguna **instrucción escrita** sobre qué tipo de información se puede introducir en Gemini?
>    Si no la hay, te paso encantada el borrador que estoy usando yo, por si sirve de punto de partida.
>
> No corre prisa, es para dejarlo bien montado.

*Por qué funciona:* el punto 3 demuestra que ha hecho los deberes y cambia el registro de la
conversación. El punto 4 ofrece trabajo en vez de pedirlo — y si no existe política, **ella acaba
siendo quien la propone**, que es el mejor resultado posible.

---

**Mensaje 3 — la pregunta incómoda, si hace falta**

> Una cosa más, y es por prudencia mía: en el buzón de admisiones manejamos copias de pasaporte, datos
> de pago y a veces alergias del alojamiento. ¿Hay algo de eso que **no** debamos meter en Gemini
> aunque sea la cuenta de empresa? Yo por defecto no lo meto, pero prefiero que quede dicho por
> alguien y no depender de mi criterio.

*Por qué funciona:* declara que ya actúa con prudencia (no está confesando nada), y traslada la
decisión a quien le corresponde. Si nadie contesta, **su regla por defecto sigue siendo no meterlo**,
que es la correcta.

---

**Mensaje 4 — si la respuesta es "no sé" o "pregunta a X"**

> Sin problema. ¿Me dices quién lleva la consola de administración de Google y le escribo yo
> directamente? Así no te lo cargo a ti.

---

### Fase 4 — Qué hacer con cada respuesta

| Lo que te contestan | Lo que significa | Lo que haces |
|---|---|---|
| "Business Standard/Plus, y sí tienes licencia" | Escenario más probable [R]. No entrenan con tus datos, Google es encargado. Sin garantía de procesamiento en la UE para Gemini | Verde y ámbar sí, rojo no. **Sigue adelante con el curso** |
| "Enterprise Plus" | Lo mejor que puede pasar. Además con regiones de datos disponibles | Igual, y pregunta si la UE está activada |
| "No tienes licencia, entras sin más" | **Puede que estés en servicio adicional** | **Trátalo como consumo hasta que te lo aclaren.** Solo verde |
| "La retención está en indefinido" | Todo lo que pegues se queda | Cambia cómo escribes. Y coméntalo: es una pregunta legítima |
| "No hay ninguna política escrita" | Lo más frecuente en una empresa de 30 personas [R] | **Oportunidad.** Ofrece tu semáforo de la sección 2.4 como borrador |
| "No sé / no me consta" | Nadie se lo ha planteado | Fase 1 + tu criterio + escríbelo tú. **Documentar que preguntaste ya te protege** |
| "Eso no lo puedo contar" | Raro, pero pasa | No insistas. Regla por defecto: solo verde y ámbar |

### Rúbrica de autocorrección — E-01

Está bien resuelto si tu fichero contiene, sin ayuda de nadie:

- [ ] El **correo exacto** con el que entras en Gemini, y comprobado que no es el personal.
- [ ] El **distintivo** que ves (Pro / Expanded / Ultra / ninguno), copiado literal.
- [ ] La **edición** de Workspace, con nombre exacto — **o**, si no la has conseguido, la frase *"pregunté
      a [nombre] el [fecha] y no obtuve respuesta"*. Eso también es un resultado válido.
- [ ] Si tu usuario **tiene licencia de Gemini** — o la constancia de haberlo preguntado.
- [ ] El **plazo de retención**, o la constancia de haberlo preguntado.
- [ ] Si existe o no **política escrita** de uso de IA.
- [ ] **A quién** hay que preguntarle esto en el futuro (un nombre y un puesto).
- [ ] Tu **semáforo personal** de la sección 2.4, adaptado con los datos concretos de tu academia.

**Está mal resuelto si** en algún punto has escrito "creo que", "supongo que" o "me suena que". En este
ejercicio **"no lo sé y lo he preguntado" vale; "creo que sí" no vale.** Ese estándar —distinguir lo
que sabes de lo que supones— es el mismo que vas a necesitar para evaluar respuestas de una IA, y por
eso este ejercicio va el primero.

**Señal de que has ido más allá de lo pedido:** que alguien de la empresa te haya respondido
*"pues buena pregunta, no lo habíamos mirado"*. Ocurre a menudo [R], y significa que acabas de aportar
algo, no de consumir tiempo de nadie.

---

## 5. Gemini con la cuenta de empresa frente a ChatGPT con la cuenta personal

Ella hoy hace lo segundo. Este apartado tiene que corregirlo **sin moralina**, porque la moralina no
cambia hábitos y además sería injusta: lo que hace es lo que hace casi todo el mundo, y lo hace porque
ChatGPT le funciona y lo conoce.

### 5.1 Lo que cambia, punto por punto

| | ChatGPT con cuenta personal | Gemini con la cuenta de la academia (con licencia) |
|---|---|---|
| **Quién responde ante la AEPD** | La **academia**, como responsable del tratamiento — aunque tú no le hayas dicho a nadie que lo usas [R] | La academia, pero **con contrato y garantías detrás** |
| **Contrato de encargado (art. 28)** | **No existe** | **Sí**, vía CDPA [D] |
| **Entrenamiento** | Sí por defecto; hay interruptor [D] | **No**, sin permiso previo [D] |
| **Retención** | Bajo tu control personal, y **hasta ahí llega tu control** | Bajo el control de tu empresa, que puede borrar |
| **Si un cliente ejerce el derecho de supresión** | La academia **no puede borrar** lo que está en tu cuenta personal [R] | La empresa puede actuar sobre su dominio |
| **Si te vas de la empresa** | Los datos de clientes se van **contigo**, en tu cuenta | Se quedan en el dominio de la empresa |
| **Si hay un litigio del proveedor** | Tus conversaciones son de consumo — ver el caso de los 20 millones de logs [D] | Bajo régimen empresarial |
| **Auditoría** | La empresa **no sabe** que ocurre. Es lo que se llama *shadow AI* | Trazable y gobernable |

### 5.2 El argumento que de verdad convence

No es "es ilegal". Es este, y conviene que esté escrito casi con estas palabras:

> **Si mañana un alumno ejerce su derecho de supresión y la academia tiene que certificar que ha
> borrado sus datos de todos los sitios, tu cuenta personal de ChatGPT es un sitio que la academia no
> puede tocar y del que ni siquiera sabe que existe.**
>
> No es que hayas hecho nada malo. Es que has creado, sin querer, un almacén de datos de clientes que
> está fuera del alcance de la empresa. Y ese es exactamente el tipo de cosa que, cuando aparece en una
> inspección o en una reclamación, no tiene arreglo posible: no se puede desandar.

Y el remate operativo, que es lo que hace que el cambio ocurra de verdad:

> Cambiar esto no te cuesta calidad. **Gemini con el plan de tu empresa es un modelo de la misma
> generación.** Lo que te cuesta es dos semanas de incomodidad mientras te acostumbras a otra
> interfaz. Y a cambio dejas de ser tú la que responde si algo sale mal.

### 5.3 La transición honesta

No hay que pedirle que borre ChatGPT de su vida. Hay que trazar una línea limpia y fácil de recordar:

| Sigue usando ChatGPT personal para | Pasa a Gemini de empresa para |
|---|---|
| Aprender, probar cosas, entender conceptos | **Cualquier cosa que venga de un correo, una llamada o un expediente de un cliente** |
| Textos genéricos sin nada de la academia | Borradores de respuestas a alumnos y agencias |
| Redactar tu currículum, cosas tuyas | Traducciones de comunicaciones reales |
| Practicar prompts con casos **inventados** | Análisis de encuestas, incidencias, quejas |

**Y una tarea de higiene, para hacer una vez y olvidarse** [D]: entrar en la cuenta personal de ChatGPT
→ Ajustes → Controles de datos → desactivar la mejora del modelo; y en la cuenta personal de Google →
Datos y privacidad → Actividad de las aplicaciones Gemini → desactivar. Ojo: incluso desactivado,
Google retiene **72 horas** [D]. Es decir, **desactivarlo reduce el daño pero no lo elimina**, y por eso
no sustituye a la regla de no meter datos de clientes.

---

## 6. Reglas prácticas aplicables el lunes

Todo lo anterior tiene que caber en unas pocas frases que se puedan seguir un martes de julio con 300
correos sin abrir. Si una regla necesita que te pares a pensar, no sobrevive a julio.

### 6.1 Qué se puede pegar y qué no

Ya está en el **semáforo de 2.4**. Tres reglas de decisión que lo hacen operativo:

**Regla del titular de prensa.** Antes de darle a enviar: *si esto que estoy pegando apareciera mañana
en un periódico junto al nombre de mi academia, ¿me importaría?* Si la respuesta es sí, no lo pegues.

**Regla del "¿para qué lo necesita?".** Si le pides que traduzca una queja al español, **no necesita el
nombre**, ni el email, ni el número de reserva. Si le pides que calcule un presupuesto, **no necesita
el pasaporte**. Casi siempre la mitad de lo que ibas a pegar sobra. Esto es minimización, pero
formulada como pregunta y no como principio, que es lo que la hace utilizable.

**Regla de los cinco segundos.** Si dudas más de cinco segundos sobre si algo puede entrar, **no
entra**. Ya lo preguntarás mañana con calma. La duda es la señal, no el problema.

### 6.2 Seudonimizar de verdad: por qué "quitar el nombre" no basta

**El error de fondo.** El RGPD dice explícitamente que **los datos seudonimizados siguen siendo datos
personales** [D — considerando 26 y art. 4.5]. Solo dejan de estarlo si están **anonimizados de verdad**,
es decir, si ya no es posible reidentificar a la persona por ningún medio razonable. Quitar el nombre
no anonimiza: **desplaza la identificación al resto del texto.**

**El ejemplo que hay que usar en el curso, porque es de su casa:**

> ❌ *"La alumna coreana de 19 años que llegó el 3 de julio y está alojada con la familia de Chamberí
> dice que la comida no le sienta bien y que es celíaca."*

Aquí no hay ni un solo nombre. Y sin embargo, **cualquiera de sus tres compañeras de atención al
cliente sabe exactamente de quién se habla**, en dos segundos. Con 1.400 alumnos al año, la combinación
nacionalidad + edad + fecha de llegada + barrio del alojamiento deja **una sola persona**. Eso se llama
*singularización*, y es lo que hace que "quitar el nombre" sea una falsa sensación de seguridad. Y
encima el texto contiene un dato de salud, que es categoría especial.

**Cómo se hace bien:**

> ✅ *"Un alumno de nivel A2 comunica una intolerancia alimentaria no registrada en su ficha inicial y
> pide cambio de régimen de comidas. Redáctame un correo a la familia de acogida explicando el cambio,
> en español, tono cordial y directo, máximo 120 palabras."*

Qué se ha hecho, y son cinco movimientos que se pueden enseñar como lista:

1. **Fuera los identificadores directos**: nombre, email, teléfono, pasaporte, nº de reserva.
2. **Fuera los cuasi-identificadores**, que son los que de verdad delatan: nacionalidad concreta, edad
   exacta, fecha exacta, barrio, nombre de la familia. Se **generalizan**: "coreana de 19 años" →
   "alumno"; "3 de julio" → "esta semana" o nada; "familia de Chamberí" → "familia de acogida".
3. **El dato de salud se degrada al mínimo funcional**: "celíaca" → "una intolerancia alimentaria".
   Si el correo lo requiere de verdad, lo escribes tú a mano al final; la IA no necesita saberlo para
   redactar el marco.
4. **Si necesitas seguir el hilo entre varios casos, usa códigos estables** (`ALU-01`, `FAM-03`) y
   **guarda la equivalencia en un fichero aparte que nunca entra en la herramienta**. Esa tabla es la
   "clave"; mientras exista, esto es seudonimización, no anonimización, y sigue bajo el RGPD.
5. **Prueba final antes de enviar** — la única que hay que memorizar:

> **"¿Podría una compañera mía saber de quién hablo leyendo esto?"**
> Si la respuesta es sí, no está seudonimizado. Da igual que no aparezca el nombre.

**Aviso importante para no crear una falsa seguridad:** seudonimizar bien reduce mucho el riesgo, pero
**no convierte el rojo en verde**. Un pasaporte seudonimizado sigue siendo un pasaporte. Las alergias de
un menor seudonimizadas siguen siendo datos de salud de un menor. La seudonimización es la técnica que
te permite trabajar con **ámbar**; no es una llave que abra el rojo.

### 6.3 Adjuntos: la regla más incómoda y la más necesaria

**El problema.** Al pegar texto ves lo que envías. Al adjuntar un fichero, **no**. Y lo que va dentro
suele ser mucho más de lo que crees:

- Un **PDF de pasaporte** va entero: foto, firma, lugar de nacimiento, nombres de los padres en algunos
  países, y la banda legible por máquina con todo repetido.
- Un **Excel** va **completo**: todas las filas, incluidas las 900 que no estás mirando; todas las
  columnas, incluidas las ocultas; **todas las hojas**, incluida la que se llama "datos antiguos"; y a
  menudo comentarios y control de cambios.
- Una **foto** lleva metadatos EXIF: fecha, hora, modelo de cámara y, muy a menudo, **coordenadas GPS**.
- Un **Word** puede llevar **cambios no aceptados, comentarios y autor**, es decir, el borrador anterior
  con lo que se decidió no decir.

**Las reglas:**

1. **Documentos oficiales de identidad: nunca.** Ni pasaporte, ni NIE, ni DNI, ni tarjeta de
   residencia, ni imagen ni PDF. Si necesitas un dato de ahí, **lo escribes tú a mano**, y solo ese.
2. **Antes de adjuntar cualquier hoja de cálculo, haz una copia y bórrale lo que no hace falta.**
   Filas, columnas, hojas. Adjunta la copia. Nunca el maestro.
3. **Si no lo has abierto y mirado entero, no lo adjuntas.** Sin excepciones. Es la regla que evita el
   90 % de los accidentes.
4. **Prefiere pegar texto a adjuntar ficheros** siempre que puedas. Pegar te obliga a ver lo que envías,
   y esa fricción es una función de seguridad, no un inconveniente.
5. **Capturas de pantalla: cuidado con lo que hay alrededor.** La bandeja de entrada de fondo, la
   pestaña abierta, el nombre en la barra de título, la notificación que entró justo entonces.

### 6.4 Un apunte sobre Gemini y los ficheros de Drive

Cuando Gemini está integrado en Workspace **puede acceder a los ficheros de Drive y a los correos a los
que tú ya tienes acceso**. Eso es una función, no un fallo: no ve nada que tú no pudieras ver. Pero
tiene dos consecuencias prácticas [R]:

- Si tienes acceso a una carpeta compartida que contiene cosas que **no deberías estar mirando**,
  Gemini puede traértelas a la respuesta sin que las hayas buscado.
- Un prompt del tipo *"resume todo lo que tengamos de este alumno"* puede recopilar y juntar en un solo
  sitio información que estaba dispersa a propósito.

**Regla:** pide por documento concreto, no por barrido general. **[V]** Y si detecta que tiene acceso a
carpetas que no le corresponden por su puesto, eso se comunica — es un hallazgo valioso y no le mete a
ella en ningún problema.

### 6.5 Grabaciones de llamadas

Es el punto donde más gente mete la pata al empezar a usar IA, porque transcribir llamadas es de lo
primero que a uno se le ocurre y parece inocuo.

**Lo que hay que saber:** [D]

- Grabar una llamada exige **informar previamente** de la grabación, de su finalidad concreta y del
  resto de la información básica de protección de datos (responsable, base legal, destinatarios, plazo
  de conservación, derechos). La AEPD ha sancionado a empresas por grabar sin informar correctamente.
- El plazo de conservación debe ser **proporcionado y limitado** a lo necesario.
- El cliente tiene **derecho de acceso a la grabación** de su propia llamada (art. 15 RGPD).
- **Meter la grabación en una herramienta de transcripción es un tratamiento nuevo y un destinatario
  nuevo.** La información que se dio al cliente al empezar la llamada probablemente **no lo cubre**, y
  el proveedor de transcripción debe ser encargado del tratamiento con contrato.

**Y el contenido:** una llamada de incidencia de alojamiento de una academia contiene, con altísima
probabilidad, **datos de salud** ("no puedo comer eso", "me encuentro mal", "estoy con ansiedad"),
convivencia, y a veces menores. Una transcripción convierte lo que era audio efímero en **texto
buscable, copiable y reenviable**, que es un salto de riesgo enorme y que casi nadie contabiliza.

**Las reglas, en orden:**

1. **Una grabación de una llamada con un cliente no se sube nunca a una herramienta personal.** Nunca.
   Ni a la tuya, ni a una app gratuita de transcripción, ni a un servicio "que lo hace en el navegador".
2. **Con la cuenta de empresa, antes de subir nada:** comprueba que el aviso que se da al cliente al
   inicio de la llamada menciona la transcripción o el tratamiento automatizado. **[!]** Si no lo
   menciona, esto no lo decides tú: lo pregunta.
3. **Alternativa que resuelve el 90 % de los casos sin tocar nada de esto:** no transcribas la
   grabación. **Escribe tú un resumen de cuatro líneas al colgar, ya seudonimizado**, y trabaja con ese
   resumen. Es más rápido que subir un audio de doce minutos, no genera un tratamiento nuevo, y de paso
   piensas el caso. Este es el ejemplo perfecto de que **la opción segura suele ser también la más
   eficiente**, que es el tono que debe llevar todo el bloque.
4. **Reuniones internas con notas automáticas:** aplica lo mismo. Todos los asistentes deben saber que
   se está grabando o transcribiendo.

### 6.6 La tarjeta del lunes

Lo que va impreso al lado de la pantalla:

```
ANTES DE PEGAR ALGO EN UNA IA
1. ¿Es de la cuenta de la ACADEMIA?          si no → para
2. ¿Hay nombre, pasaporte, NIE, dirección,
   IBAN, salud, religión o un MENOR?         si sí  → quítalo o no lo hagas
3. ¿Lo necesita de verdad para responderme?  si no  → fuera
4. ¿Una compañera sabría de quién hablo?     si sí  → sigue quitando
5. ¿Es un adjunto que no he abierto entero?  si sí  → no lo adjuntes
6. ¿Dudo más de 5 segundos?                  si sí  → no entra

Grabaciones de llamadas → NUNCA en herramienta personal.
Menores → NUNCA, en ninguna.
Pasaportes y datos de pago → NUNCA, en ninguna.
```

---

## 7. El riesgo operativo y reputacional

El riesgo legal es el que sale en los titulares. **El que se materializa un martes es el otro.** Y para
su puesto —atención al cliente— el operativo es más probable, más frecuente y más caro que la multa.

### 7.1 Qué pasa realmente cuando un sistema contesta mal a un cliente

Cruzando con los procesos de `dominio-academia.md`:

| Fallo | Proceso | Qué pasa de verdad |
|---|---|---|
| **Cita un precio que ya no está vigente** | P01, P02 | Por escrito, se convierte de facto en una oferta que la escuela acaba respetando para no perder la reserva. **Pérdida directa de margen** |
| **Afirma algo sobre plazos o requisitos de visado** | P08, P09 | El alumno organiza su viaje con esa información. Si es falsa: **visado denegado, vuelos perdidos, reembolso y reseña demoledora** |
| **Aplica la política de cancelación equivocada** | P24 | Devolver de más = pérdida. Devolver de menos = reclamación de consumo |
| **Confunde condiciones de curso con las de alojamiento** | P24 | El error clásico del proceso, ahora a escala y en segundos |
| **Admite responsabilidad por escrito en una queja** | P26 | **Compromete a la empresa.** Riesgo crítico |
| **Menciona datos de un alumno al responder una reseña pública** | P28 | Confirmar públicamente que alguien fue alumno y tuvo un problema **ya es una cesión de datos**. Doble golpe: brecha + reputación |
| **Contesta en el idioma equivocado o con tono equivocado** | Todos | Daño menor, pero erosiona la percepción de calidad |
| **Inventa una cita del reglamento o una fecha** | P08, P16 | La alucinación con formato de dato oficial es la más peligrosa: **parece verdad** |
| **No dice que es una IA** | Todos | Desde el **02.08.2026**, incumplimiento del art. 50 del Reglamento de IA [D] |

**Y el fallo que casi nadie anticipa:** el sistema acierta el 95 % de las veces, la gente se relaja, y
el 5 % restante pasa sin revisión. **La degradación no viene del error; viene de la confianza.** Esto
conecta directamente con el paso 5 del método de la referencia (evaluación) y con su pregunta sobre si
el sistema empeora al crecer.

### 7.2 Las salvaguardas, y por qué son de diseño y no de disciplina

La regla de fondo, que ordena todas las demás:

> **La confianza no es una salvaguarda.** Si la seguridad de un sistema depende de que alguien se
> acuerde de revisar, el sistema no es seguro: es seguro *hasta el primer día de mucho trabajo*. Y en
> una academia, el día de mucho trabajo es predecible: se llama julio.

**Las siete salvaguardas, ordenadas de más a menos importante:**

**1. Nada sale al cliente sin que un humano le dé a enviar.**
La única salvaguarda que no falla. Todo lo demás es un refuerzo de esta. Se diseña como **borrador en
la bandeja**, nunca como envío automático. Coste: cinco segundos por correo. Beneficio: elimina de
golpe la categoría entera de fallos del apartado 7.1.

**2. La lista de temas prohibidos, explícita en el sistema.**
Escrita en el fichero de contexto, en negativo y sin matices: *"nunca respondas sobre requisitos o
plazos de visado; nunca cites importes; nunca confirmes disponibilidad de alojamiento; nunca respondas
a una queja formal; nunca menciones salud; si el tema aparece, escribe SOLO: **DERIVAR A PERSONA** y
para."* Los temas prohibidos coinciden exactamente con los procesos de riesgo **CRÍTICO** y **Alto** del
inventario, lo cual da un criterio objetivo para construir la lista en vez de improvisarla.

**3. "No lo sé" como respuesta válida y deseable.**
Hay que instruirlo explícitamente y **probarlo a propósito**, con preguntas cuya respuesta no está en
las fuentes. Un sistema que nunca dice "no lo sé" no es que lo sepa todo: es que no lo has probado bien.
La referencia lo señala como uno de sus mejores aportes y en atención al cliente no es un refinamiento,
es el requisito mínimo.

**4. Cita de la fuente y de su fecha.**
Toda afirmación con un dato —precio, fecha, condición— tiene que venir con de dónde sale y de cuándo es.
Esto convierte la revisión humana en algo de cinco segundos en lugar de una investigación, que es lo que
hace que la revisión se siga haciendo en julio. Y ataca el problema de **P32** (plantillas caducadas en
otros idiomas), que es el riesgo "alto y silencioso" del inventario.

**5. Condiciones de parada.**
Cuándo el sistema **debe** detenerse: cliente enfadado, mención de abogado o de hoja de reclamaciones,
mención de salud o de accidente, menor implicado, importe por encima de X, cualquier cosa relacionada
con visados, o simplemente que no encuentre la respuesta en sus fuentes. La condición de parada es lo
que separa un asistente de un problema.

**6. Registro de qué se generó y quién lo aprobó.**
No para culpar a nadie: para poder reconstruir qué pasó cuando algo salga mal, y para poder decirle a un
cliente qué se le dijo exactamente y cuándo.

**7. El aviso de IA, desde el primer día.**
Si el cliente interactúa con el sistema, debe saberlo (art. 50, en vigor). Si el sistema solo prepara
borradores que revisa y firma una persona, **no hay interacción directa** y el aviso no aplica del mismo
modo [R] **[!]** — pero esa línea la marca la empresa, no ella.

### 7.3 El plan para cuando falle — porque va a fallar

La referencia insiste en que detrás de una demo hay decenas de intentos. En producción, detrás de un
sistema bueno hay un plan para el día malo:

1. **Detectar.** Alguien tiene que darse cuenta. Normalmente el cliente. Que exista una vía por la que
   una queja de "me dijisteis otra cosa" llegue a quien puede parar el sistema.
2. **Parar.** Saber **cómo se apaga**, y haberlo probado. Un sistema que no sabes apagar no está
   terminado.
3. **Reparar con la persona.** Llamada, no correo. Y la academia asume el error sin cargárselo a "el
   sistema": para el cliente, el sistema **es** la academia.
4. **Corregir el sistema.** Añadir ese caso concreto a la batería de pruebas para que no vuelva a pasar.
   Así es como una batería de pruebas se hace buena: creciendo con los fallos reales.
5. **Valorar si hay brecha de datos.** **[!]** Si el fallo implicó revelar datos de un cliente a otro,
   eso puede ser una brecha notificable en 72 h. **No lo decide ella.** Lo escala el mismo día.

### 7.4 El riesgo reputacional específico de este sector

Merece apartado propio porque su negocio tiene una asimetría poco común [R, sobre datos D del
inventario]:

- **Los clientes son extranjeros que se juegan mucho**: un visado, un semestre, un viaje pagado. La
  tolerancia al error administrativo es baja porque las consecuencias para ellos son enormes.
- **Las agencias intermediarias son el 30-50 % de las matrículas** y reservan por volumen: un error se
  multiplica por quince alumnos y por una relación comercial entera.
- **Las reseñas son el canal de captación**: LanguageCourse.net, Google, Trustpilot. Una reseña que diga
  *"me contestaba un robot y me dio información falsa sobre el visado"* hace un daño desproporcionado y
  permanente, y es exactamente el tipo de frase que un cliente frustrado escribe.
- **Y hay una asimetría cultural cruel:** el ahorro de tiempo se nota en la oficina, en silencio; el
  fallo se nota en internet, en público y en el idioma del alumno.

Conclusión para el diseño del curso, y es la razón de que la escalera del perfil empiece por donde
empieza: **empezar por lo interno.** Análisis de encuestas (P27), partes semanales (P30), informes de
KPIs (P31), mantenimiento de plantillas (P32). Ahí el error es barato, se detecta rápido y no lo ve
ningún cliente. El contacto con el cliente llega después, y siempre con humano en el medio.

---

## 8. Traducción a contenido de curso

### 8.1 Principio de diseño

Esto **no es un módulo de protección de datos**. Si fuera un módulo, se leería una vez, se aprobaría y
se olvidaría. Es una **capa que atraviesa el curso**, con tres apariciones en momentos donde el
contenido **desbloquea** lo siguiente en vez de frenarlo:

| Momento | Aparición | Por qué ahí |
|---|---|---|
| **Antes de tocar nada** | Saber qué tienes y qué no puedes pegar | Sin esto, todo lo demás se construye sobre un suelo sin mirar |
| **Antes de la primera automatización** | Seudonimizar y adjuntos | Automatizar multiplica el volumen de datos que pasan por la herramienta |
| **Antes del primer agente** | Salvaguardas, condiciones de parada, art. 50 | Un agente actúa sin que tú mires cada paso |

### 8.2 Qué tiene que saber hacer, y en qué orden

**Nivel 1 — Antes de tocar nada (semana 1)**

| Competencia | Verificable por |
|---|---|
| Saber **qué cuenta y qué plan** usa, y qué protecciones lleva | E-01 (sección 4) |
| Distinguir **verde / ámbar / rojo** en su propio material real | E-02 |
| Saber que **el RGPD ya se aplica** y que la ley de IA es otra capa | E-05 |
| Saber **quién es el responsable** (la academia) y **quién el encargado** (Google, si hay contrato) | E-05 |

**Nivel 2 — Antes de automatizar (semanas 2-3)**

| Competencia | Verificable por |
|---|---|
| **Seudonimizar de verdad**, con la prueba de la compañera | E-03 |
| Tratar adjuntos: copia limpia, nunca el maestro, nunca el pasaporte | E-03 |
| Elegir **el proceso adecuado para empezar**, con criterio de riesgo, no de ganas | E-04 |
| Escribir un **prompt que no necesite datos personales** para hacer su trabajo | E-03 |

**Nivel 3 — Antes de dejar que algo actúe solo (semana 4+)**

| Competencia | Verificable por |
|---|---|
| Escribir **condiciones de parada** para su proceso | E-06 |
| Escribir la **lista de temas prohibidos**, derivada de los procesos críticos | E-06 |
| Diseñar el **punto de revisión humana** y defender por qué está ahí | E-06 |
| Reconocer que la nivelación de alumnos (P05) toca el **Anexo III** y hay que escalarla | E-05 |
| Saber **qué escala inmediatamente** y a quién | E-06 |

### 8.3 Los ejercicios autocorregibles

Cada uno con rúbrica de sí/no, sin juicio de valor y sin necesitar a nadie.

---

**E-01 · "¿Qué tengo yo exactamente?"** — desarrollado íntegro en la sección 4.
Momento: semana 1. Rúbrica: la lista de 8 casillas de la sección 4.

---

**E-02 · El semáforo de tu bandeja de entrada**

> Abre tu buzón de trabajo y coge **los 10 últimos correos de clientes** que has respondido. Para cada
> uno, sin pegar nada en ninguna parte, escribe: qué le pedirías a una IA que hiciera con él, y **qué
> parte exacta tendrías que quitar** antes.

*Autocorrección — está bien si:*
- [ ] En al menos 7 de los 10 has identificado **algún** dato que hay que quitar. Si en menos de 7 no
      has encontrado nada, **estás mirando por encima**: vuelve.
- [ ] Has encontrado al menos un correo que es **rojo entero** y que no debe entrar de ninguna manera.
      (En una academia, en 10 correos de cliente aparece uno. Si no aparece, cambia la muestra por
      correos de admisiones o alojamiento.)
- [ ] Has encontrado al menos un correo **verde**: una consulta genérica sin nada personal.
- [ ] En cada caso ámbar has escrito qué es lo que **sí** necesita la IA para hacer su trabajo.

*Trampa deliberada del ejercicio:* la mayoría, la primera vez, quitan el nombre y creen que ya está.
La rúbrica no lo dice; lo descubre en E-03. Está puesto a propósito para que el error ocurra antes en
el ejercicio que en la vida real.

---

**E-03 · La prueba de la compañera**

> Coge 3 casos ámbar del E-02 y reescríbelos seudonimizados. Después, para cada uno, contesta:
> **¿podría [nombre de una compañera concreta] saber de quién hablo leyendo esto?**
>
> Si la respuesta es sí, sigue quitando. Repite hasta que sea no.

*Autocorrección — está bien si:*
- [ ] En los 3 casos has quitado, además del nombre, **al menos dos cuasi-identificadores** (fecha
      exacta, nacionalidad concreta, edad exacta, barrio, nombre del alojamiento, número de reserva).
- [ ] Has **generalizado** en lugar de borrar: "coreana de 19 años" → "alumno", no un hueco vacío. Si
      has dejado huecos, el texto pierde sentido y la respuesta será mala.
- [ ] El prompt resultante **sigue sirviendo**: pruébalo. Si la respuesta que te da es útil, has
      seudonimizado bien. Si es inservible, has quitado contexto que no era identificador — **ese es el
      error del otro lado y también hay que verlo.**
- [ ] Si alguno de los 3 casos contenía salud, religión o un menor, has concluido que **no debía entrar
      en absoluto**, ni seudonimizado. Si has "arreglado" un caso de alergia de un menor
      seudonimizándolo, **eso está mal** y es el fallo más importante que puede cometer el ejercicio.

*Punto de consulta con su pareja (marcado como tal, y uno de los pocos del curso):*
Enseñarle dos o tres de sus casos ya seudonimizados y preguntar: *"¿tú sabrías de quién hablo?"*.
Alguien que no trabaja en la academia y sí sabe de IA es **el evaluador ideal** para esta prueba
concreta, porque tiene el punto de vista de fuera que ella no puede tener sobre su propio material.
Diez minutos. Es de los pocos sitios del curso donde ese recurso rinde de verdad.

---

**E-04 · Elegir el proceso de partida**

> De la lista de tus tareas repetitivas, elige **una** para automatizar primero. Puntúa cada candidata:
>
> | Criterio | +2 | 0 | −3 |
> |---|---|---|---|
> | Datos que maneja | solo verde | ámbar seudonimizable | rojo |
> | Consecuencia del error | interna, se arregla | molesta a un cliente | dinero, plazo legal o visado |
> | ¿Lo ve un cliente? | no | indirectamente | sí, directamente |
> | ¿Cuántas veces al mes? | más de 20 | 5-20 | menos de 5 |
> | ¿Sabes cómo se hace bien? | perfectamente | más o menos | depende de otros |

*Autocorrección — está bien si:*
- [ ] La ganadora tiene **puntuación positiva** y **ningún −3**.
- [ ] **Ninguna tarea con −3 ha ganado**, por mucho que te apetezca. Si te apetece mucho, es señal de
      que duele mucho, no de que sea buena para empezar.
- [ ] Has descartado explícitamente el **matching de alojamiento (P17)**, aunque sea el que más duele.
      Motivo: es el que más categorías especiales concentra de todo tu trabajo.
- [ ] Has descartado **cualquier cosa con visados (P08, P09)** y **emergencias (P29)**.

*Solución comentada:* si el ganador ha sido el **análisis de encuestas de satisfacción (P27)** o el
**mantenimiento de plantillas (P32)**, has llegado a la misma conclusión que el análisis del dominio
por un camino distinto, y eso significa que el criterio funciona. Si ha ganado otra cosa que cumple los
requisitos, también está bien: **el criterio es lo que se evalúa, no la respuesta.**

---

**E-05 · Verdadero o falso** (autocorrección instantánea)

| # | Afirmación | |
|---|---|---|
| 1 | "Como mi empresa paga Gemini, puedo meter cualquier cosa" | **F.** Pagar resuelve quién es el proveedor, no qué tratamientos están amparados |
| 2 | "Si quito el nombre, ya no son datos personales" | **F.** Siguen siéndolo si se puede reidentificar. Considerando 26 |
| 3 | "El Reglamento de IA todavía no se aplica" | **F.** Prohibiciones y alfabetización desde feb-2025; transparencia del art. 50 desde el 02.08.2026 |
| 4 | "Los sistemas de alto riesgo ya son exigibles" | **F.** El Anexo III se aplazó al 02.12.2027 por el Ómnibus |
| 5 | "Si uso mi ChatGPT personal, el problema es mío" | **F.** El responsable ante la AEPD es la academia |
| 6 | "Google AI Studio es de Google, así que es seguro" | **F.** El nivel gratuito advierte literalmente de no enviar información personal |
| 7 | "Una alergia alimentaria es un dato normal" | **F.** Es dato de salud, categoría especial del art. 9 |
| 8 | "Grabar la voz de alguien es siempre dato biométrico" | **F.** Solo si el tratamiento busca identificar unívocamente a la persona |
| 9 | "Si el sistema no habla con el cliente, no hace falta avisar de que es IA" | **V** (con matices) **[!]** La línea la marca la empresa |
| 10 | "Nivelar alumnos con IA sería un uso de alto riesgo" | **V.** Anexo III, ámbito de educación. Aplazado, no cancelado |
| 11 | "Con la cuenta de empresa, Gemini se procesa siempre en la UE" | **F.** Solo con Enterprise Plus o Assured Controls |
| 12 | "Si desactivo la actividad, no queda nada guardado" | **F.** Google retiene 72 h en cualquier caso |

*Autocorrección:* menos de 10 aciertos → releer secciones 1 y 3. Fallar la 5 u 11 es lo más común.

---

**E-06 · La lista de temas prohibidos de tu propio sistema**

> Para el proceso que elegiste en E-04, escribe: (a) la lista de temas sobre los que el sistema **nunca**
> debe pronunciarse, (b) las condiciones de parada, (c) quién revisa antes de que salga, (d) cómo se
> apaga.

*Autocorrección — está bien si:*
- [ ] La lista de (a) incluye **importes, plazos de visado, disponibilidad y salud**, aunque tu proceso
      no los toque hoy. Los sistemas se expanden solos; la lista se escribe para el sistema de dentro de
      seis meses.
- [ ] Las condiciones de parada incluyen al menos: **no encuentro la respuesta en mis fuentes**,
      **el cliente está enfadado**, **hay un menor**, **se menciona salud** y **se menciona abogado,
      reclamación u hoja de reclamaciones**.
- [ ] La respuesta a (c) es **una persona con nombre**, no "se revisa". Si no hay nombre, no hay revisión.
- [ ] La respuesta a (d) la has **probado de verdad**, no imaginado.
- [ ] Ninguna salida llega a un cliente sin que alguien le dé a enviar. Si tu diseño lo permite,
      **vuelve al principio.**

---

### 8.4 Los puntos de consulta con su pareja

El perfil pide reservar este recurso y no gastarlo en lo que el material puede resolver. En todo el
bloque de datos hay exactamente **dos** que lo merecen:

1. **La prueba de la compañera en E-03.** Necesita una mirada externa que ella, por definición, no
   puede tener sobre sus propios casos. Diez minutos y resuelve el concepto más difícil del bloque.
2. **La revisión del diseño de salvaguardas de E-06, la primera vez.** Alguien con criterio técnico ve
   en dos minutos si el punto de revisión humana está donde tiene que estar o es decorativo. Es el
   error de diseño más caro y el más difícil de ver desde dentro.

Todo lo demás —el semáforo, el verdadero/falso, la elección del proceso, el ejercicio de averiguar el
plan— se corrige solo con las rúbricas.

### 8.5 Lo que este bloque NO debe hacer

- **No debe ser un módulo de "avisos legales"** que se lee una vez. Va repartido y siempre pegado a la
  acción que desbloquea.
- **No debe asustar.** El objetivo es que use más la IA, no menos: que la use **en el sitio correcto**.
  Un bloque de protección de datos que produce parálisis ha fallado.
- **No debe convertirla en responsable de cumplimiento.** Cada vez que aparece una decisión que no es
  suya, va marcada **[!]** y con el nombre de a quién se escala.
- **No debe congelar fechas dentro de prompts ni plantillas.** Todo lo de la sección 1 vive en un
  fichero de contexto con fecha visible y se revisa.
- **No debe prometer certezas que no tiene.** Los **[NV]** de la sección 3.4 se quedan como están, y
  eso es parte de lo que se enseña.

---

## 9. Fuentes

**Marco normativo**
- Reglamento (UE) 2016/679, RGPD — arts. 4, 5, 6, 9, 12, 15, 28, 33, 35, cap. V; considerandos 26 y 38.
- Ley Orgánica 3/2018, LOPDGDD — arts. 5, 7, 34.
- Reglamento (UE) 2024/1689, Reglamento de IA — arts. 4, 5, 50, 99; Anexo III.
- Reglamento (UE) 2026/1744, Ómnibus digital sobre IA — DOUE 24.07.2026, en vigor 27.07.2026.
- Proyecto de Ley Orgánica para el buen uso y la gobernanza de la IA — Consejo de Ministros 26.05.2026;
  publicado en el Congreso 12.06.2026; en tramitación.
  https://www.lamoncloa.gob.es/consejodeministros/resumenes/paginas/2026/260526-rueda-prensa-ministros.aspx

**AEPD**
- Decálogo *"Cuidado con lo que le confIAs"*, 27.01.2026 — https://www.aepd.es/guias/recomendaciones-ia-aepd.pdf
- Orientaciones sobre **IA agéntica**, 18.02.2026 — https://www.aepd.es/guias/orientaciones-ia-agentica.pdf
- Nota de prensa del decálogo — https://www.aepd.es/prensa-y-comunicacion/notas-de-prensa/aepd-publica-decalogo-recomendaciones-proteger-privacidad-al-usar-ia

**Google — fuentes oficiales**
- Privacy Hub de IA generativa en Workspace — https://knowledge.workspace.google.com/admin/generative-ai/generative-ai-in-google-workspace-privacy-hub
- Seguridad y privacidad de la IA generativa en Workspace — https://workspace.google.com/security/ai-privacy/
- FAQ de Google Workspace con Gemini — https://knowledge.workspace.google.com/admin/gemini/gemini-for-google-workspace-faq
- Usar Gemini con una cuenta de trabajo o centro educativo (**los distintivos Pro/Expanded/Ultra**) — https://support.google.com/gemini/answer/14620100
- Privacy Hub de las aplicaciones Gemini (consumo) — https://support.google.com/gemini/answer/13594961
- Gemini pasa a ser servicio principal con protección empresarial (10.2024) — https://workspaceupdates.googleblog.com/2024/10/gemini-app-enterprise-data-protection-core-service-expansion.html
- Regiones de datos para **funciones** de Gemini (09.06.2025) — https://workspaceupdates.googleblog.com/2025/06/data-regions-support-for-gemini-features-in-google-workspace.html
- Regiones de datos para la **app** Gemini (29.06.2026) — https://workspaceupdates.googleblog.com/2026/06/gemini-app-data-regions-support.html
- Funciones de Gemini incluidas en las suscripciones de Workspace — https://knowledge.workspace.google.com/admin/generative-ai/workspace-with-gemini/gemini-ai-features-now-included-in-google-workspace-subscriptions
- Cloud Data Processing Addendum — https://cloud.google.com/terms/data-processing-addendum
- RGPD y Google Cloud — https://cloud.google.com/privacy/gdpr
- Términos adicionales de la API de Gemini (**Unpaid vs Paid Services**) — https://ai.google.dev/gemini-api/terms

**OpenAI**
- Residencia de datos en Europa — https://openai.com/index/introducing-data-residency-in-europe/
- Respuesta a las demandas de datos del NYT — https://openai.com/index/response-to-nyt-data-demands/
- FAQ del cambio de nombre de Team a Business — https://help.openai.com/en/articles/12111915-chatgpt-business-rename-faq

**Transferencias internacionales**
- IAPP, el Tribunal General desestima el recurso *Latombe* — https://iapp.org/news/a/european-general-court-dismisses-latombe-challenge-upholds-eu-us-data-privacy-framework
- Recurso de casación C-703/25 P, pendiente ante el TJUE.

**Contexto sectorial**
- FEDELE, datos del sector 2025 (recogidos en `dominio-academia.md`).
- Anexo III del Reglamento de IA aplicado al ámbito educativo — análisis especializado, agosto 2026.

**Nota sobre la calidad de las fuentes.** Todo lo marcado **[D]** procede de fuente oficial o primaria
consultada el 22.08.2026. Los precios y desgloses por edición de la sección 3.2.6, y la ausencia de
residencia europea en ChatGPT Business, proceden de consultoras y blogs especializados; van marcados
**[R]** y no deben citarse como dato firme. Todo lo marcado **[NV]** no es verificable desde fuera de la
empresa y es, precisamente, el objeto del ejercicio E-01.
