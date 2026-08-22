# Dominio — Atención al cliente en una academia de español para extranjeros (Madrid, ~30 empleados)

**Para qué sirve este documento.** Es el mapa del terreno real donde la alumna va a trabajar. El curso
tiene que salir de aquí: los ejercicios, los datos de práctica, el proyecto final y — sobre todo — los
casos en los que hay que decir *"aquí no metas IA"*. Sin este mapa, el curso enseña herramientas en el
vacío.

**Fecha:** 22.08.2026.

---

## Nota metodológica — qué es dato y qué es reconstrucción

Este documento mezcla tres cosas y conviene no confundirlas:

| Marca | Significado |
|---|---|
| **[D]** | **Documentado.** Cifra o norma verificada en fuente pública (FEDELE, Instituto Cervantes, normativa de extranjería, condiciones generales publicadas por escuelas reales). Fuentes en la sección 9. |
| **[R]** | **Reconstrucción razonada.** No está publicado, pero se deduce de los datos [D] y de cómo funciona el sector. Es la parte que la alumna debe **corregir con la realidad de su empresa**. |
| **[V]** | **A verificar por ella.** Punto donde la reconstrucción puede fallar y donde su conocimiento del dominio vale más que cualquier fuente. |

> **Uso pedagógico de esto.** El primer ejercicio real del curso puede ser exactamente este:
> darle la sección 1 y pedirle que tache lo que no ocurre en su empresa, corrija los volúmenes y añada
> los procesos que faltan. Eso es *levantar el contexto de la empresa*, que es el 80 % del trabajo de un
> operador de IA y lo que ningún curso genérico le puede dar hecho.

---

## 0. La empresa modelo

### 0.1 Anclajes reales del sector [D]

- España recibió **160.830 estudiantes de español** en 2025 repartidos en **112 escuelas asociadas a
  FEDELE**, que sumaron **977.490 semanas de curso**. Impacto económico directo e indirecto por encima
  de **715 M€**.
- De ahí salen dos números que ordenan todo lo demás: **~1.400 estudiantes por escuela y año** y
  **~8.700 semanas-alumno por escuela y año** → **estancia media ≈ 6 semanas**.
- **56,4 %** de los estudiantes se alojan en **familia de acogida gestionada por la escuela**.
- Duración de la estancia: **71,3 % menos de 3 meses**, **18,3 % de 3 a 12 meses**, **10,3 % residentes**.
- Procedencia: **Europa 80,3 %**, Asia 9,3 %, Norteamérica 7,7 %, Sudamérica 1,1 %, África 0,8 %.
- **41,5 % viaja en grupo** y 58,5 % individualmente → una escuela media convive con dos negocios muy
  distintos: el alumno individual y el grupo cerrado (colegio, universidad, agencia).
- Perfil: **57,4 % mujeres**, 41,75 % hombres. Curso más demandado: **lengua y cultura general (73 %)**.

Una academia de ~30 empleados en Madrid está exactamente en esa media: no es una escuela de barrio ni
una cadena. Es el tamaño en el que **todo el trabajo administrativo recae en 2–4 personas** y no hay
departamentos especializados. Ese es el punto clave para el curso.

### 0.2 Organigrama plausible [R]

| Área | Personas | Notas |
|---|---|---|
| Dirección / gerencia | 1–2 | Decide precios, convenios y compensaciones |
| Dirección académica + coordinación | 2 | Niveles, horarios, cuadrante de profesores |
| Profesorado ELE | 14–18 | Mezcla de fijos y de refuerzo estacional (junio–septiembre) |
| **Atención al cliente / student services** | **3–4** | ← el puesto de la alumna |
| Alojamiento | 1–2 | A veces es la misma persona de CX; en verano se desborda |
| Marketing / ventas / agencias | 1–2 | Lleva la relación con las agencias intermediarias |
| Administración / contabilidad | 1 | Facturación, remesas, pagos a familias |
| Actividades culturales | 1 (+becarios) | Excursiones, tapas, intercambios |
| Limpieza / mantenimiento del edificio de estancias | externo o 1 | |

**Consecuencia operativa [R]:** en atención al cliente **una misma persona atiende el teléfono, contesta
el buzón compartido, resuelve una incidencia de alojamiento y emite una carta de visado en la misma
hora**. No hay colas separadas. Cualquier solución de IA que exija "dedicar un rato tranquilo" fracasa.

### 0.3 Volúmenes de trabajo del puesto [R, sobre base D]

| Magnitud | Temporada baja (nov–feb) | Media (mar–may, oct) | Pico (jun–sep) |
|---|---|---|---|
| Correos entrantes al buzón compartido | 80–150/día | 150–250/día | **250–400/día** |
| Llamadas atendidas | 20–40/día | 40–60/día | **60–100/día** |
| Mensajes de WhatsApp | 40–80/día | 80–150/día | **150–300/día** |
| Alumnos simultáneos en el centro | 120–180 | 180–260 | **300–450** |
| Matrículas nuevas confirmadas | 10–20/semana | 25–40/semana | **60–90/semana** |
| Reservas de alojamiento activas | 60–100 | 100–160 | **200–300** |

Totales anuales de referencia [R]: **1.300–1.500 matrículas**, **~5.000–8.000 solicitudes de información**
(conversión 15–25 %), **~700–800 reservas de alojamiento**, **120–200 cartas de aceptación para visado**,
**120–180 cancelaciones o cambios de fecha**, **80–120 incidencias de alojamiento**, **30–60 quejas
formales**, **600–800 encuestas de satisfacción respondidas**.

### 0.4 Stack de herramientas típico [R]

- **Buzón compartido** (`info@`, `accommodation@`, `admissions@`) en Outlook o Google Workspace. Es el
  centro de gravedad del puesto.
- **Software de gestión académica** tipo ClassLife, OfiELE, LangLion, Acadesoft… o, muy frecuentemente,
  **un Excel maestro + Google Drive** que hace de CRM real aunque exista otro software oficial [V].
- **WhatsApp Business** para alumnos ya llegados y para familias de acogida (grupos incluidos).
- **Hoja de cálculo de camas / calendario de ocupación** para alojamiento — casi siempre separada del
  software académico, y esa separación es el origen de la mitad de los errores [R].
- **Pasarela de pago** (Redsys/TPV, Stripe o PayPal) + transferencias internacionales.
- **Formularios** (Google Forms / Typeform) para test de nivel y encuestas.
- **Carpeta de plantillas** en Word/Drive: cartas, certificados, presupuestos, en varias versiones y
  varios idiomas, sin control de versiones. **Esta carpeta es el yacimiento del curso.**
- Portales de agencias y marketplaces: LanguageCourse.net, ESL, EF, Sprachcaffe, Booking/Spotahome/
  HousingAnywhere/Uniplaces para la parte de estancias largas [R].

---

## 1. Inventario de procesos del puesto

Formato de cada ficha:

- **Disparador / canal** — qué lo inicia y por dónde entra.
- **Volumen** — [R] salvo indicación.
- **Repetitivo** — Alto / Medio / Bajo.
- **Determinista** — ¿los pasos están escritos y siempre son los mismos? Sí / Parcial / No.
- **Consulta** — documentos y fuentes de verdad que hay que mirar (ver sección 2).
- **Idiomas** — en los que se ejecuta realmente.
- **Riesgo** — Bajo / Medio / Alto / **Crítico**, con la consecuencia concreta del error.

---

### Bloque A — Captación, presupuesto y matrícula

#### P01 · Respuesta a solicitud de información entrante (lead)
- **Disparador / canal:** formulario web, email directo, WhatsApp, portal de comparadores, DM de redes.
- **Volumen:** 20–35/día laborable en baja; **80–120/día** en marzo–mayo. 5.000–8.000/año.
- **Repetitivo:** **Alto.** El 70–80 % pregunta lo mismo: precio, fechas de inicio, niveles, si hay
  alojamiento, si dan carta para el visado, si hay descuento por semanas.
- **Determinista:** Parcial. La *información* es determinista (está en el tarifario y el calendario);
  el *tono, idioma y orden* dependen del caso.
- **Consulta:** tarifario vigente, calendario académico con fechas de inicio y festivos, catálogo de
  alojamiento con precios, condiciones generales, FAQ de visados.
- **Idiomas:** inglés (mayoritario), español, alemán, francés, italiano, portugués; y ocasionalmente
  japonés, coreano, chino, ruso, turco, neerlandés, polaco, sueco.
- **Riesgo:** **Medio.** Un precio mal citado por escrito se convierte de facto en una oferta que la
  escuela acaba respetando para no perder la reserva. Un plazo de visado mal dicho pierde al alumno.

#### P02 · Elaboración y envío de presupuesto / proforma
- **Disparador / canal:** lead cualificado, casi siempre por email.
- **Volumen:** 2.500–3.500/año (10–15/día; 30–40/día en pico).
- **Repetitivo:** **Alto**, pero con muchas combinaciones: nº de semanas × tipo de curso × alojamiento ×
  régimen de comidas × traslado de aeropuerto × seguro × tasa de matrícula × descuentos por volumen.
- **Determinista:** **Sí** — es aritmética sobre una tabla de precios. Aquí no hay juicio, hay cálculo.
- **Consulta:** tarifario, tabla de descuentos por semanas, suplementos de verano y de dietas especiales,
  calendario (semanas con festivo), condiciones de pago.
- **Idiomas:** los de P01. El documento suele ir en inglés o español aunque la conversación sea en otro.
- **Riesgo:** **Alto.** Un error de cálculo se descubre al facturar y ya no se puede subir el precio;
  o se descubre al llegar el alumno y produce una queja. Errores típicos: cobrar 4 semanas de alojamiento
  cuando la estancia son 27 noches, olvidar el suplemento de julio-agosto, aplicar un descuento caducado.

#### P03 · Reserva vía agencia intermediaria
- **Disparador / canal:** *booking form* de la agencia por email o su portal.
- **Volumen:** 30–50 % de las matrículas [R, coherente con el 41,5 % de viaje en grupo [D]] → 400–700/año.
- **Repetitivo:** **Alto**, pero **cada agencia tiene su propio formulario, sus tarifas netas, su
  comisión y sus condiciones de cancelación pactadas por convenio**, distintas de las públicas.
- **Determinista:** Parcial. Extraer datos del formulario es determinista; aplicar el convenio correcto no.
- **Consulta:** convenio/acuerdo con esa agencia, tarifa neta pactada, % de comisión, condiciones de
  cancelación específicas, calendario de disponibilidad de alojamiento.
- **Idiomas:** inglés casi siempre; italiano, alemán, francés, japonés y coreano según la agencia.
- **Riesgo:** **Alto.** Aplicar la tarifa pública a una agencia con tarifa neta rompe el margen o rompe
  la relación comercial. Y las agencias reservan **volumen**: un error se multiplica por 15 alumnos.

#### P04 · Alta del alumno en el sistema y apertura de expediente
- **Disparador / canal:** reserva confirmada.
- **Volumen:** 1.300–1.500/año.
- **Repetitivo:** **Alto.** Copiar datos de un email/formulario a los campos del sistema.
- **Determinista:** **Sí.** Es transcripción pura.
- **Consulta:** pasaporte/DNI del alumno, formulario de reserva, tarifario, hoja de camas.
- **Idiomas:** los datos llegan en cualquier idioma y alfabeto (cirílico, japonés, árabe, coreano).
- **Riesgo:** **Alto** por acumulación. Un nombre transcrito mal desde el pasaporte reaparece en la carta
  de visado, en el certificado y en la factura, y obliga a rehacerlo todo. Una fecha en formato
  MM/DD frente a DD/MM cambia la llegada de marzo a abril.

#### P05 · Test de nivel y asignación de grupo (MCER A1–C2)
- **Disparador / canal:** enlace enviado antes de llegar; o presencial el lunes.
- **Volumen:** 1.300–1.500/año, concentrados en lunes.
- **Repetitivo:** Alto en la parte administrativa (enviar, recordar, recoger, pasar el resultado a
  académico); **no repetitivo** en el juicio final del nivel.
- **Determinista:** Parcial. El test escrito puntúa solo; la entrevista oral y el encaje en un grupo
  existente los decide el equipo académico.
- **Consulta:** resultados del test, ocupación real de cada grupo, horarios, historial si es repetidor.
- **Idiomas:** instrucciones del test en 4–6 idiomas; la gestión, en el idioma del alumno.
- **Riesgo:** **Medio-Alto.** Un alumno mal nivelado es la **primera causa de queja académica** y suele
  acabar en cambio de grupo en 48 h, con efecto dominó sobre el resto de grupos.

#### P06 · Cobro, seguimiento de pagos pendientes y conciliación
- **Disparador / canal:** vencimiento del plazo (habitualmente **15 días antes del inicio** [D, TANDEM]).
- **Volumen:** ~1.400 cobros/año + 300–500 recordatorios de impago.
- **Repetitivo:** **Alto.**
- **Determinista:** **Sí.** Regla de calendario: si no consta pago X días antes → recordatorio 1 → 2 → aviso.
- **Consulta:** extracto bancario, listado de reservas, condiciones de pago, tabla de comisiones bancarias.
- **Idiomas:** el del alumno; con agencias, inglés.
- **Riesgo:** **Alto.** Reclamar un pago ya hecho enfada al cliente antes de llegar; no reclamarlo hace
  que el alumno aparezca el lunes sin pagar y nadie quiere ser quien lo eche de clase.

#### P07 · Envío del pack de bienvenida / información pre-llegada
- **Disparador / canal:** automático a X días de la llegada, en la práctica manual.
- **Volumen:** 1.300–1.500/año.
- **Repetitivo:** **Alto.** Es el mismo documento con 6–10 variables.
- **Determinista:** **Sí.**
- **Consulta:** dirección y plano del centro, horario del primer día, datos de la familia o del
  alojamiento, instrucciones de transporte desde Barajas, qué traer, contacto de emergencia 24 h.
- **Idiomas:** todos los de trabajo.
- **Riesgo:** **Medio.** Si no se envía, el lunes hay alumnos perdidos por Madrid llamando al móvil de
  emergencia. Si va con la dirección del alojamiento equivocada, el riesgo sube a Alto.

---

### Bloque B — Visados, certificados y documentación oficial

#### P08 · Emisión de carta de aceptación / admisión para visado de estudiante
- **Disparador / canal:** petición del alumno o de la agencia, tras pago **completo** del curso
  (práctica habitual del sector [D, TANDEM: exige transferencia previa del total]).
- **Volumen:** 120–200/año, muy concentradas: **abril–junio** (cursos de septiembre) y **octubre–noviembre**
  (cursos de enero).
- **Repetitivo:** **Alto** en la forma; **bajo** en la casuística (consulados distintos piden cosas
  distintas, el mismo país cambia de criterio de un año a otro).
- **Determinista:** **Sí en la plantilla, No en el criterio.** El documento tiene campos fijos: nombre
  exacto como en el pasaporte, nº de pasaporte, nacionalidad, programa, **fechas exactas de inicio y fin**,
  **nº de horas semanales** (el umbral de referencia es **20 h/semana** [D]), importe pagado, sello y firma.
- **Consulta:** pasaporte, justificante de pago, calendario académico, condiciones de visado del consulado
  correspondiente, acreditación del centro (Instituto Cervantes / registro autonómico).
- **Idiomas:** español obligatoriamente; muy a menudo también inglés, y a veces bilingüe en el mismo folio.
- **Riesgo:** **CRÍTICO.** Un dato mal puesto = **visado denegado** = viaje cancelado, reembolso, reseña
  demoledora y posible reclamación. Además hay exposición reputacional y legal: el centro certifica hechos
  ante una administración. **Contexto normativo vivo [D]:** el Reglamento de Extranjería (RD 1155/2024, en
  vigor desde el 20.05.2025) y la Instrucción SEM 3/2025 han reordenado la estancia/residencia por estudios
  — se exige presencialidad mínima, centro autorizado/registrado, solicitud con antelación (referencia:
  2 meses) y el idioma estudiado debe ser distinto de la lengua materna u oficial del país de origen.
  **Esto cambia de un año para otro: es exactamente el tipo de conocimiento que NO se debe congelar dentro
  de un prompt.**

#### P09 · Seguimiento de expedientes de visado, denegaciones y cambios de fecha
- **Disparador / canal:** el alumno avisa de cita consular, retraso o denegación.
- **Volumen:** 80–150 interacciones/año; 10–25 denegaciones o retrasos reales.
- **Repetitivo:** Medio. Cada caso tiene su historia.
- **Determinista:** Parcial. La política de "si hay denegación oficial documentada se aplica X" está
  escrita [D: TANDEM aplica las mismas condiciones de cancelación con denegación acreditada]; el resto
  es negociación y contención emocional.
- **Consulta:** condiciones generales, expediente del alumno, carta emitida, política de reembolso por
  denegación, calendario para reubicar en otra fecha.
- **Idiomas:** el del alumno; documentos consulares en cualquier idioma.
- **Riesgo:** **Alto.** Dinero real en juego y un alumno frustrado que ya ha pagado vuelos.

#### P10 · Emisión de certificados (asistencia, matrícula, notas, nivel alcanzado)
- **Disparador / canal:** petición del alumno, normalmente el último viernes; también para renovaciones
  de autorización y para su universidad de origen.
- **Volumen:** ~1.200 certificados de fin de curso + 200–400 ad hoc/año.
- **Repetitivo:** **Muy alto.** Es una plantilla con 5–8 variables.
- **Determinista:** **Sí.**
- **Consulta:** registro de asistencia, notas del profesor, expediente, calendario.
- **Idiomas:** español y/o inglés; a veces con exigencia de traducción jurada (que la escuela **no** hace).
- **Riesgo:** **Alto** si el certificado alimenta un trámite oficial (renovación de estancia, convalidación
  de créditos, beca). Certificar horas o asistencia que no se han producido es falsedad documental.
  **Medio** si es solo un recuerdo para el alumno.

#### P11 · Control de asistencia y avisos por faltas
- **Disparador / canal:** parte diario del profesor.
- **Volumen:** diario, ~300–450 alumnos en pico.
- **Repetitivo:** **Alto.**
- **Determinista:** **Sí.** Umbral escrito (p. ej. <80 % → aviso; faltas continuadas → notificación).
- **Consulta:** partes de asistencia, condiciones del curso, obligaciones asociadas al visado.
- **Idiomas:** español/inglés interno; el aviso, en el idioma del alumno.
- **Riesgo:** **Alto** en alumnos con visado (la asistencia sostiene la autorización) y en menores
  (hay que avisar a la familia el mismo día). **Bajo** en un turista de dos semanas.

---

### Bloque C — Operativa semanal del centro

#### P12 · Check-in del lunes / gestión del primer día
- **Disparador / canal:** presencial, cada lunes del año.
- **Volumen:** 15–30 alumnos nuevos/lunes en baja; **60–90/lunes** en julio.
- **Repetitivo:** **Alto** y siempre igual: acoger, test, carnet, wifi, aulas, horarios, normas, cobro de
  pendientes, foto para el carnet, formulario de datos, entrega de material.
- **Determinista:** **Sí**, es una lista de comprobación.
- **Consulta:** listado de llegadas, asignación de grupos, plano de aulas, hoja de alojamiento.
- **Idiomas:** todos a la vez, en la misma sala, con alumnos de nivel A0.
- **Riesgo:** **Medio.** No es irreversible, pero **es el momento que fija la percepción de calidad de
  toda la estancia** y donde se generan las reseñas.

#### P13 · Cambios de nivel, de grupo y de horario
- **Disparador / canal:** alumno o profesor, típicamente martes-miércoles de la primera semana.
- **Volumen:** 5–12 % de los alumnos → 80–170/año.
- **Repetitivo:** Medio.
- **Determinista:** No. Depende de plazas libres, del criterio del profesor y de la insistencia del alumno.
- **Consulta:** ocupación de grupos, informe del profesor, resultado del test.
- **Idiomas:** el del alumno.
- **Riesgo:** **Medio.** Mover a uno descoloca a un grupo entero.

#### P14 · Altas, bajas y ampliaciones de curso en marcha
- **Disparador / canal:** el alumno quiere quedarse 2 semanas más, o irse antes.
- **Volumen:** 200–350/año. Las ampliaciones son de los momentos más rentables del negocio.
- **Repetitivo:** **Alto.**
- **Determinista:** **Sí** en la parte de precio (tarifa por semanas adicionales) y **encadenado**: tocar
  el curso obliga a tocar el alojamiento, la factura, el grupo y, si hay visado, las fechas certificadas.
- **Consulta:** tarifario, disponibilidad de alojamiento, ocupación de grupos, expediente.
- **Riesgo:** **Alto** por la cadena: es el proceso donde más se olvida actualizar *una* de las cinco cosas.

#### P15 · Programación e inscripción en actividades culturales
- **Disparador / canal:** calendario semanal publicado los lunes.
- **Volumen:** 3–5 actividades/semana, 15–40 inscritos cada una; 150–250 actividades/año.
- **Repetitivo:** **Alto.** Mismo ciclo cada semana: publicar, inscribir, cobrar extras, confirmar aforo,
  recordar punto de encuentro, gestionar lluvia o cierre del museo.
- **Determinista:** **Sí.**
- **Consulta:** calendario de actividades, aforos, precios de extras, contactos de proveedores.
- **Idiomas:** cartel en español fácil + inglés; recordatorios en el idioma del alumno.
- **Riesgo:** **Bajo-Medio.** Salvo aforo, dinero cobrado o menores implicados.

#### P16 · Gestión de exámenes oficiales (DELE, SIELE, CCSE)
- **Disparador / canal:** convocatorias fijas anuales del Instituto Cervantes.
- **Volumen:** 2–4 convocatorias/año; 40–120 candidatos/año [R].
- **Repetitivo:** Medio, pero con **plazos rígidos e inamovibles**.
- **Determinista:** **Sí, y con reglas ajenas:** la inscripción y el pago de tasas se hacen **en la
  plataforma del Instituto Cervantes**, no en la escuela [D]; la escuela pone sala, coordinación y a veces
  el papel de centro examinador.
- **Consulta:** calendario de convocatorias, tasas por nivel (orden de 100–200 € según nivel [D]),
  instrucciones del centro examinador, listado de candidatos.
- **Idiomas:** español; comunicación con candidatos en su idioma.
- **Riesgo:** **Alto.** Un plazo de inscripción perdido no se recupera: el alumno espera a la siguiente
  convocatoria, meses después, y a veces se queda sin el certificado que necesitaba para una universidad.

---

### Bloque D — Alojamiento (familias, residencia y estancias de larga duración)

Este bloque es, en una escuela con alojamiento propio, **la mitad del trabajo de CX y el 80 % de las
incidencias**. Y es donde la escuela deja de ser una academia y se comporta como un pequeño hotel.

#### P17 · Asignación alumno ↔ familia de acogida / habitación (*matching*)
- **Disparador / canal:** reserva de alojamiento confirmada.
- **Volumen:** 700–800/año [R, coherente con el 56,4 % en familia [D]]. En julio, 60–80 asignaciones/semana.
- **Repetitivo:** Medio. El *procedimiento* se repite; la *decisión* no.
- **Determinista:** **No.** Hay que cruzar: disponibilidad real, zona y distancia al centro, edad y sexo
  del alumno, si hay niños o mascotas en casa, tabaco, **alergias y dieta** (vegetariana, vegana, sin
  gluten, halal, kosher), religión, idioma que se habla en casa, si el alumno viene con un amigo, si es
  menor, y el histórico de esa familia con alumnos anteriores.
- **Consulta:** fichero de familias colaboradoras, calendario de ocupación, ficha del alumno, historial de
  incidencias de cada familia, tarifas por régimen.
- **Idiomas:** con la familia **siempre español**; con el alumno, su idioma.
- **Riesgo:** **Alto.** Un mal encaje genera cambio de alojamiento en 48 h, coste directo y una reseña
  negativa. Y se manejan **datos de categoría especial del RGPD**: salud (alergias), creencias religiosas,
  a veces orientación sexual. *(Ver sección 6: por eso es una trampa como primer proyecto de IA.)*

#### P18 · Confirmación de alojamiento e instrucciones de llegada
- **Disparador / canal:** hecha la asignación, ~2 semanas antes de la llegada.
- **Volumen:** 700–800/año.
- **Repetitivo:** **Muy alto.** Plantilla con: nombre y teléfono del anfitrión, dirección exacta, metro más
  cercano, hora de llegada acordada, qué incluye el régimen, normas de la casa, contacto de emergencia.
- **Determinista:** **Sí.**
- **Consulta:** ficha de la familia/piso, hoja de camas, instrucciones de llegada, normas de convivencia.
- **Idiomas:** el del alumno; la dirección **siempre también en español** para que pueda enseñársela al taxista.
- **Riesgo:** **Alto.** Es el documento que un alumno lee a las 23:40 en Barajas. Un portal o un piso mal
  escrito es una emergencia nocturna garantizada.

#### P19 · Coordinación de llegadas y salidas (check-in/check-out, traslados)
- **Disparador / canal:** vuelo del alumno; salidas los sábados/domingos.
- **Volumen:** 700–800 llegadas + 700–800 salidas/año; **domingo es el día crítico**.
- **Repetitivo:** **Alto.**
- **Determinista:** **Sí**, pero con excepciones costosas: llegadas de madrugada, vuelos retrasados,
  check-in fuera de horario, entrega de llaves, suplemento por llegada nocturna.
- **Consulta:** listado de llegadas con nº de vuelo y hora, contactos de anfitriones, proveedor de traslados,
  hoja de camas.
- **Idiomas:** todos; y a menudo por WhatsApp, en tiempo real, fuera de horario laboral.
- **Riesgo:** **Alto** — es el proceso con más probabilidad de generar una crisis en horario no laboral.

#### P20 · Incidencias en el alojamiento
- **Disparador / canal:** WhatsApp o presencial, en cualquier momento.
- **Volumen:** 80–120/año; 1 de cada 8–10 reservas. Se concentran en julio y agosto (calor + convivencia).
- **Repetitivo:** Medio. El catálogo de motivos sí se repite: **ruido, temperatura (aire acondicionado y
  calefacción), comida escasa o distinta a lo esperado, limpieza, wifi, convivencia con otros inquilinos,
  llaves, horarios, sensación de aislamiento, distancia real al centro**.
- **Determinista:** Parcial. Hay un protocolo (escuchar → verificar con el anfitrión → mediar → si no,
  reubicar) pero cada caso mezcla hechos y expectativas culturales.
- **Consulta:** protocolo de incidencias, condiciones de alojamiento, ficha e histórico de la familia,
  disponibilidad para reubicar, política de compensaciones.
- **Idiomas:** el del alumno + español con la familia. **Traducir la queja es media resolución.**
- **Riesgo:** **Alto.** Mal gestionada escala a reseña pública, reclamación de la agencia y pérdida de una
  familia colaboradora (que cuesta meses conseguir). Puede haber menores.

#### P21 · Estancias de larga duración: contratos, mensualidades y fianzas
- **Disparador / canal:** reserva de 1 a 9 meses en alojamiento propio.
- **Volumen:** 40–60 plazas propias [R]; 100–200 contratos/año; ~150 cobros mensuales recurrentes.
- **Repetitivo:** **Alto** (mensual y previsible).
- **Determinista:** **Sí.** Contrato de temporada, **fianza** (la referencia legal en alquiler de temporada
  en la Comunidad de Madrid son **dos mensualidades** [D]), suministros, calendario de pagos, prórrogas,
  devolución de fianza tras inventario de salida.
- **Consulta:** contrato tipo, normas de convivencia, inventario de la habitación, tabla de suministros,
  calendario de vencimientos.
- **Idiomas:** contrato en español (validez legal) + versión de cortesía en inglés.
- **Riesgo:** **Alto.** Es dinero recurrente y una relación contractual: retener una fianza sin justificar
  es una reclamación de consumo; no cobrar una mensualidad se descubre tarde.

#### P22 · Gestión de disponibilidad y ocupación (calendario de camas)
- **Disparador / canal:** continuo; cada reserva, cambio o ampliación lo toca.
- **Volumen:** decenas de actualizaciones al día en pico.
- **Repetitivo:** **Muy alto.**
- **Determinista:** **Sí.** Es un calendario de recursos.
- **Consulta:** hoja de camas, reservas confirmadas, bloqueos por mantenimiento, vacaciones de las familias.
- **Idiomas:** interno, español.
- **Riesgo:** **CRÍTICO en su versión mala: el *overbooking*.** Dos alumnos asignados a la misma habitación
  un domingo de julio es el peor día del año del puesto. Casi siempre nace de la **desincronización entre
  la hoja de camas y el software académico**.

#### P23 · Alta, seguimiento y pago a familias de acogida
- **Disparador / canal:** captación continua; refuerzo antes de verano.
- **Volumen:** cartera de 35–60 familias [R]; 10–20 altas/bajas al año; pago mensual a cada una.
- **Repetitivo:** Medio-Alto.
- **Determinista:** Parcial. La visita, la entrevista y la decisión de admitir una familia no lo son.
- **Consulta:** ficha de familia, tarifas de pago a anfitriones, checklist de visita domiciliaria,
  historial de valoraciones de alumnos.
- **Idiomas:** español.
- **Riesgo:** **Alto.** Las familias son el activo escaso del negocio: en agosto se van de vacaciones y la
  capacidad se hunde. Un pago tardío o un trato descuidado y se pasan a la escuela de al lado.

---

### Bloque E — Postventa, incidencias y satisfacción

#### P24 · Cancelaciones y cambios de fecha
- **Disparador / canal:** email o llamada del alumno o de la agencia.
- **Volumen:** 120–180/año (8–12 % de las reservas).
- **Repetitivo:** **Alto** en la mecánica.
- **Determinista:** **Sí, totalmente** — si la política está escrita. Es una tabla de tramos. Ejemplos
  reales publicados [D]: reembolso total salvo inscripción si se cancela **≥15 días** antes y **cero
  devolución** por debajo (TANDEM Madrid, con inscripción de 50 € en intensivos / 30 € en extensivos y
  **depósito de 200 € no reembolsable**); 60 % si ≥30 días y 40 % si <30 días (Alcalingua); y para
  **alojamiento**, escalados del tipo **50 % entre 30 y 20 días, 75 % entre 20 y 5 días, 100 % con menos
  de 5 días** antes de la llegada. Además existe el **derecho de desistimiento de 14 días naturales** en
  contratación a distancia si el curso no ha empezado [D].
- **Consulta:** condiciones generales vigentes **en la fecha de la reserva** (no las de hoy), convenio de
  la agencia si aplica, expediente y justificantes de pago, calendario.
- **Idiomas:** el del cliente. La versión que prevalece jurídicamente es la española.
- **Riesgo:** **Alto.** Devolver de más es pérdida directa; devolver de menos es una reclamación de consumo
  y una reseña. Y las condiciones **de alojamiento y de curso son distintas entre sí** — confundirlas es
  el error clásico.

#### P25 · Reembolsos y notas de crédito
- **Disparador / canal:** cancelación aceptada, denegación de visado, doble cobro.
- **Volumen:** 60–100/año.
- **Repetitivo:** Alto.
- **Determinista:** **Sí.** Cálculo → autorización → orden de pago → justificante al cliente.
- **Consulta:** política de reembolso, factura original, datos bancarios, comisiones y tipo de cambio.
- **Idiomas:** el del cliente.
- **Riesgo:** **Alto.** Dinero irreversible + datos bancarios (**nunca deben pasar por una herramienta de
  IA**) + riesgo de fraude por suplantación en el cambio de cuenta.

#### P26 · Quejas y reclamaciones formales
- **Disparador / canal:** email, presencial, agencia, o la **hoja de reclamaciones oficial** de la
  Comunidad de Madrid.
- **Volumen:** 30–60 quejas/año; 2–5 hojas oficiales.
- **Repetitivo:** Bajo-Medio.
- **Determinista:** **No.** Requiere investigar, decidir si hay compensación y con qué importe, y redactar.
- **Consulta:** expediente completo, histórico de comunicaciones, condiciones generales, protocolo de
  incidencias, límites de compensación que puede autorizar cada persona.
- **Idiomas:** el del cliente; con la administración, español.
- **Riesgo:** **CRÍTICO.** Consecuencia legal, económica y reputacional. Una respuesta que admite
  responsabilidad por escrito compromete a la empresa.

#### P27 · Encuestas de satisfacción y análisis de resultados
- **Disparador / canal:** a mitad de curso y el último día; formulario online o en papel.
- **Volumen:** ~1.400 envíos/año, **600–800 respuestas** con **comentarios en texto libre en 10+ idiomas**.
- **Repetitivo:** **Alto** en el envío; **el análisis casi nunca se hace** porque nadie tiene tiempo [R][V].
- **Determinista:** Sí en el envío y en las medias numéricas; **no** en la lectura de los comentarios.
- **Consulta:** cuestionario, listado de alumnos que terminan, histórico de resultados, requisitos de
  calidad del sello de acreditación.
- **Idiomas:** todos. Es el proceso **más multilingüe de todos**.
- **Riesgo:** **Bajo.** Equivocarse aquí no rompe nada: no hay dinero, no hay plazo legal, el resultado es
  un informe interno. **← Retener este dato: es la razón por la que es el mejor primer proyecto.**

#### P28 · Gestión y respuesta a reseñas online
- **Disparador / canal:** Google, LanguageCourse.net, Trustpilot, portales de alojamiento.
- **Volumen:** 100–250 reseñas/año; se responden las negativas y algunas positivas.
- **Repetitivo:** Alto en el formato de respuesta.
- **Determinista:** No.
- **Consulta:** expediente del alumno (¿quién es?, ¿qué pasó de verdad?), protocolo de tono, histórico.
- **Idiomas:** se responde **en el idioma de la reseña**.
- **Riesgo:** **Medio-Alto.** Es público y permanente. Y **no se pueden dar datos del alumno en la
  respuesta** (RGPD): confirmar públicamente que alguien fue alumno y tuvo un problema de salud o de
  convivencia ya es una cesión de datos.

#### P29 · Emergencias y asistencia 24 h
- **Disparador / canal:** llamada o WhatsApp, casi siempre fuera de horario.
- **Volumen:** 15–40/año [R]: urgencias médicas, pérdida de pasaporte, robo, accidente en excursión,
  alumno menor que no aparece, conflicto grave en el alojamiento.
- **Repetitivo:** **Bajo.**
- **Determinista:** Parcial. Existe un protocolo, pero se aplica con juicio y bajo presión.
- **Consulta:** protocolo de emergencias, póliza del seguro del alumno, contactos de la familia y del
  consulado, ficha médica si la hay.
- **Idiomas:** el que haga falta, con un alumno en estado de shock y probablemente en nivel A1.
- **Riesgo:** **CRÍTICO.** Integridad de personas, menores, responsabilidad civil. **Zona prohibida para
  cualquier automatización.**

---

### Bloque F — Coordinación interna y reporting

#### P30 · Parte semanal a dirección académica y a profesorado
- **Disparador / canal:** cada viernes/lunes.
- **Volumen:** 52 ciclos/año, más los cambios diarios.
- **Repetitivo:** **Muy alto.** Listas de altas, bajas, cambios de grupo, alumnos nuevos por nivel.
- **Determinista:** **Sí.**
- **Consulta:** sistema de gestión, hoja de camas, reservas de la semana.
- **Riesgo:** **Medio.** Un profesor con la lista mal recibe a un alumno que no existe o pierde a uno que sí.

#### P31 · Informe mensual de KPIs a gerencia
- **Disparador / canal:** cierre de mes.
- **Volumen:** 12/año.
- **Repetitivo:** Alto.
- **Determinista:** **Sí.** Matrículas, semanas vendidas, ocupación de alojamiento, origen de los alumnos,
  ingresos por canal (directo vs agencia), incidencias, satisfacción media.
- **Consulta:** todo lo anterior.
- **Riesgo:** **Medio.** Es una decisión de negocio la que se toma con esos números.

#### P32 · Mantenimiento de las plantillas, la web y el FAQ
- **Disparador / canal:** cambio de precios, de calendario, de política o de normativa.
- **Volumen:** 2–6 revisiones grandes/año + parches continuos.
- **Repetitivo:** Medio.
- **Determinista:** Parcial.
- **Consulta:** tarifario nuevo, calendario nuevo, condiciones actualizadas, web, plantillas en 6 idiomas.
- **Idiomas:** **todos** — y aquí está el problema: se actualiza la versión española y **las otras cinco
  se quedan viejas**.
- **Riesgo:** **Alto y silencioso.** Una plantilla desactualizada en alemán sigue mandando durante meses un
  precio del año pasado. Nadie se entera hasta que un cliente lo reclama.

---

### 1.1 Tabla resumen del inventario

| # | Proceso | Volumen/año | Repet. | Determinista | Idiomas | Riesgo |
|---|---|---|---|---|---|---|
| P01 | Respuesta a solicitud de información | 5.000–8.000 | Alto | Parcial | 6–12 | Medio |
| P02 | Presupuesto / proforma | 2.500–3.500 | Alto | **Sí** | 6–12 | Alto |
| P03 | Reserva vía agencia | 400–700 | Alto | Parcial | 3–6 | Alto |
| P04 | Alta en sistema y expediente | 1.300–1.500 | Alto | **Sí** | todos | Alto |
| P05 | Test de nivel y asignación de grupo | 1.300–1.500 | Alto/Bajo | Parcial | 4–6 | Medio-Alto |
| P06 | Cobros y seguimiento de impagos | ~1.900 | Alto | **Sí** | 6–12 | Alto |
| P07 | Pack de bienvenida pre-llegada | 1.300–1.500 | Alto | **Sí** | 6–12 | Medio |
| P08 | Carta de aceptación para visado | 120–200 | Alto | Sí (plantilla) | 2 | **CRÍTICO** |
| P09 | Seguimiento de visados y denegaciones | 80–150 | Medio | Parcial | 6–12 | Alto |
| P10 | Certificados | ~1.500 | Muy alto | **Sí** | 2 | Alto |
| P11 | Control de asistencia y avisos | diario | Alto | **Sí** | 6–12 | Alto |
| P12 | Check-in del lunes | 52 ciclos | Alto | **Sí** | todos | Medio |
| P13 | Cambios de nivel/grupo | 80–170 | Medio | No | 6–12 | Medio |
| P14 | Altas/bajas/ampliaciones en curso | 200–350 | Alto | Sí (encadenado) | 6–12 | Alto |
| P15 | Actividades culturales | 150–250 | Alto | **Sí** | 2–4 | Bajo-Medio |
| P16 | Exámenes DELE/SIELE/CCSE | 2–4 conv. | Medio | Sí (reglas ajenas) | 2 | Alto |
| P17 | Matching alumno ↔ familia/habitación | 700–800 | Medio | **No** | 6–12 | Alto |
| P18 | Confirmación de alojamiento | 700–800 | Muy alto | **Sí** | 6–12 | Alto |
| P19 | Llegadas, salidas y traslados | ~1.500 mov. | Alto | Sí (con excepciones) | todos | Alto |
| P20 | Incidencias de alojamiento | 80–120 | Medio | Parcial | 6–12 | Alto |
| P21 | Larga estancia: contratos y fianzas | 100–200 | Alto | **Sí** | 2 | Alto |
| P22 | Calendario de camas / ocupación | continuo | Muy alto | **Sí** | ES | **CRÍTICO** (overbooking) |
| P23 | Familias de acogida: alta y pagos | 10–20 altas | Medio-Alto | Parcial | ES | Alto |
| P24 | Cancelaciones y cambios de fecha | 120–180 | Alto | **Sí** | 6–12 | Alto |
| P25 | Reembolsos y notas de crédito | 60–100 | Alto | **Sí** | 6–12 | Alto |
| P26 | Quejas y reclamaciones formales | 30–60 | Bajo-Medio | **No** | 6–12 | **CRÍTICO** |
| P27 | Encuestas de satisfacción | 600–800 resp. | Alto | Parcial | **10+** | **Bajo** |
| P28 | Reseñas online | 100–250 | Alto | No | 6–12 | Medio-Alto |
| P29 | Emergencias 24 h | 15–40 | Bajo | Parcial | todos | **CRÍTICO** |
| P30 | Parte semanal a académico | 52 | Muy alto | **Sí** | ES | Medio |
| P31 | Informe mensual de KPIs | 12 | Alto | **Sí** | ES | Medio |
| P32 | Mantenimiento de plantillas y FAQ | 2–6 + parches | Medio | Parcial | **todos** | Alto silencioso |
