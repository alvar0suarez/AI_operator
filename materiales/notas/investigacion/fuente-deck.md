# Reconstrucción del DECK — Webinar "AI Operators" (Damian Naprawa + Aleksandra Zajączkowska)

Fuente: `/home/user/AI_operator/materiales/fuentes/webinar-damian-naprawa/informe.md` (137 capturas + OCR),
`transcripcion.md` (2.148 segmentos), `frames/`, y `web-aioperators/index.txt`.
Duración 01:56:59. Fecha en pantalla del reloj de Windows: 20.08.2026 (el deck dice "DZIŚ 2 WRZEŚNIA" — ver §7).
Material original en polaco; se cita en polaco y se traduce.

---

## 0. Hallazgo previo: no hay UN deck, hay TRES superficies

El OCR revela, por la barra de direcciones del navegador y las cabeceras de página, que lo que se
proyecta son **tres artefactos distintos**, y esa separación es la clave de toda la estructura:

| # | Superficie | Fichero visible en pantalla | Quién la maneja | Función |
|---|---|---|---|---|
| **A** | Deck de encuadre y venta | HTML a pantalla completa; cabecera `AI • Operators / OTWARCIE / 00 : 03` | Damian | Marco + oferta |
| **B** | Deck docente | `C:/Users/Lenovo/Desktop/Instagram/prezentacja-system-ai-v21.html` — **22 slides numeradas** | Ola | Contenido |
| **C** | Demo/artefacto | `C:/Users/Lenovo/Desktop/Self-firma/artefakty/prezentacja5.html` — pestaña titulada *"Rentgen agencji w ciemności"* + Obsidian | Ola | Prueba |

El deck B lleva **cabecera de tres campos**: marca a la izquierda, **sección** en el centro
(`PLAN`, `KROK 01`…`KROK 05`, `PODSUMOWANIE`, `DOMKNIĘCIE`) y **contador `NN / 22`** a la derecha.
Esa arquitectura nunca se menciona en voz: es andamiaje puramente visual.

El emparedado es: **A (encuadre) → B (docencia) + C (prueba) → A (venta) → C/web (cierre)**.
Damian nunca enseña; Ola nunca vende. La separación de roles es deliberada y es el mecanismo
central del embudo: la credibilidad la fabrica una persona y la cobra la otra.

---

## 1. Secuencia ordenada de slides

### BLOQUE A-1 — Apertura de Damian (00:00 – 00:09)

| Frame / t | Kicker (polaco) | Titular reconstruido | Traducción |
|---|---|---|---|
| `0005` 00:00:23 | `AI • Operators` | **Jak zbudować system AI, który zna Twoją pracę** / *i przejmuje jej powtarzalną część* | Cómo construir un sistema de IA que conoce tu trabajo / y asume su parte repetitiva |
| `0006` 00:01:00 | `DLA KOGO JEST TEN WEBINAR?` | **Kierujemy go do dwóch grup osób.** <br>pie: *W obu przypadkach cel jest ten sam: przejść od dorywczego używania AI do systemu pracy.* | ¿Para quién es este webinar? — Lo dirigimos a dos grupos de personas. <br>*En ambos casos el objetivo es el mismo: pasar del uso ocasional de la IA a un sistema de trabajo.* |
| `0007` 00:02:57 | `NIE BĘDZIE` \| `BĘDZIE` | izq: **50 promptów. 20 aplikacji. Jednego magicznego triku.** — der: **System AI, który zna Twoją firmę.** | NO HABRÁ: 50 prompts. 20 apps. Un truco mágico. / HABRÁ: un sistema de IA que conoce tu empresa. |
| `0008` 00:03:51 | `NOWA KOMPETENCJA W FIRMIE` | **Osoba, która potrafi zaprojektować taki system, jest AI Operatorem.** | Nueva competencia en la empresa: quien sabe diseñar ese sistema es un AI Operator. |
| `0009` 00:04:09 | — | **DWIE DROGI. JEDNA ROLA. AI OPERATOR** | Dos caminos. Un solo rol. AI Operator. |
| `0010` 00:04:57 | `DWOJE PRAKTYKÓW. DWIE PERSPEKTYWY.` | **Ola – AI Engineer, 7+ lat doświadczenia.** / **Damian – Architekt systemów + przedsiębiorca.** | Dos profesionales. Dos perspectivas. Ola – AI Engineer, +7 años. Damian – arquitecto de sistemas + empresario. |
| `0011` 00:06:51 | `PRAKTYKA, NIE TEORIA` | **Budujemy z AI. Uczymy tego, czego sami używamy.** | Práctica, no teoría. Construimos con IA. Enseñamos lo que nosotros mismos usamos. |
| `0012` 00:07:48 | `PREZENT DLA OBECNYCH NA ŻYWO` | **Jak zbudować stronę internetową z AI w cztery wieczory.** <br>*Dowiesz się, jak ją opublikować oraz jak znaleźć pierwszego klienta i sprzedać gotową stronę.* <br>mini-flujo: `TWÓJ POMYSŁ → STRONA DO PUBLIKACJI` · `JAK OPUBLIKOWAĆ` · `JAK SPRZEDAĆ` | Regalo para los presentes en directo: cómo construir una web con IA en cuatro tardes. Sabrás publicarla, encontrar el primer cliente y vender la web terminada. TU IDEA → WEB LISTA PARA PUBLICAR · CÓMO PUBLICAR · CÓMO VENDER |
| `0013` 00:08:42 | `CZAS ZBUDOWAĆ SECOND BRAIN` | **Ola pokaże Wam teraz, jak AI zaczyna rozumieć firmę.** <br>`ALEKSANDRA ZAJĄCZKOWSKA · AI ENGINEER` | Hora de construir un Second Brain. Ola os enseñará ahora cómo la IA empieza a entender la empresa. |

### BLOQUE B — Deck docente de Ola, 22 slides (00:09 – 00:56)

| Slide | Frame / t | Sección | Titular reconstruido | Traducción |
|---|---|---|---|---|
| 01–02 | `0016-0017` 00:09:06 | portada | **Jak zbudować system AI, który zna Twoją pracę** *i przejmuje jej powtarzalną część* | (misma portada que A) |
| 02 | `0018` 00:09:30 | — | **Pokażę Ci pięć kroków, żeby to wykonać i wyróżnić się na rynku** | Te enseñaré cinco pasos para hacerlo y destacar en el mercado |
| **03** | `0019` 00:09:42 | `PIĘĆ KROKÓW` | lista de los 5 pasos (→ §3.1) | Cinco pasos |
| **05** | `0021` 00:13:00 | `PLAN` | tarjeta **TEGO SZUKA RYNEK** (→ §3.4) | Esto es lo que busca el mercado |
| **08** | `0023-0024` 00:14:27 | `KROK 01` | **Model, automatyzacja albo agent** + árbol de decisión (→ §3.2) | Modelo, automatización o agente |
| 09–10 | *(no capturadas)* 00:16–00:19 | `KROK 01` | ramas A / B / C del árbol + tabla de herramientas | — |
| **11** | `0026` 00:20:09 | `KROK 02` · `PRZYKŁAD` | **Analiza konkurencji** — *Zbierasz listę firm od marketingu i SEO na polskim rynku, sprawdzasz, jak na ich tle wygląda Twoja agencja, porządkujesz dane i wyciągasz wnioski.* | Ejemplo: análisis de competencia. Reúnes una lista de agencias de marketing y SEO del mercado polaco, compruebas cómo queda tu agencia frente a ellas, ordenas los datos y sacas conclusiones. |
| **13** | `0027` 00:26:15 | `KROK 02` | **Opis zadania, które oddajesz** + diagrama 01–04 (→ §3.3) | La descripción de la tarea que delegas |
| 14 | `0028` 00:26:45 | — | **Teraz pokażę, jak powstaje LLM brain** — *Wygląda na skomplikowane, a złoży go też osoba pracująca na kasie, z zawodem zupełnie spoza biznesu. Programowanie nie jest tu potrzebne.* | Ahora enseñaré cómo nace un LLM brain. Parece complicado, pero lo puede montar hasta una persona que trabaja en una caja registradora, con una profesión totalmente ajena al mundo empresarial. Aquí no hace falta programar. |
| ~14b | `0029` 00:27:33 | `KROK 03` · `TEGO SZUKA RYNEK` | revelado del ítem **Wewnętrzne narzędzia** | Herramientas internas |
| **15** | `0034` / `0041` 00:35:02 | `KROK 03` | **Kontekst i wiedza firmy** — tríada Źródła prawdy / Pamięć / Skill (→ §3.5) | Contexto y conocimiento de la empresa |
| 16–17 | *(no capturadas)* 00:46–00:49 | `KROK 04` | **Dostęp do narzędzi** ↔ ítem *Zdolność prototypowania* | Acceso a herramientas |
| **18** | `0042` 00:49:09 | `KROK 05` · `ZANIM OCENIMY JAKOŚĆ` | **To samo ułożysz dla wielu innych spraw** — rueda de 6 casos (→ §3.6) | Antes de evaluar la calidad: lo mismo lo montas para muchos otros asuntos |
| **19** | `0043` 00:50:27 | `KROK 05` | **Ocena jakości wyniku** — *Każde zdanie ma notatkę* (Klikasz link, otwierasz plik i widzisz to samo źródło oraz datę.) / *Test na znanym przypadku* (Puszczasz zadanie, którego wynik znasz, i porównujesz różnice.) | Evaluación de la calidad del resultado. Cada frase tiene su nota: haces clic en el enlace, abres el fichero y ves la misma fuente y la misma fecha. Test sobre un caso conocido: lanzas una tarea cuyo resultado ya conoces y comparas las diferencias. |
| **20** | `0044` 00:52:12 | `PODSUMOWANIE` | **Podsumujmy** + tarjeta completa TEGO SZUKA RYNEK | Recapitulemos |
| **21** | `0045` 00:55:12 | `DOMKNIĘCIE` | **Teraz powiem wam coś zupełnie szczerze** | Ahora os voy a decir algo con total sinceridad |
| **22** | `0046` 00:56:12 | `DOMKNIĘCIE` | **Widzisz wynik. Za nim stoi kilkadziesiąt podejść.** — retícula de casillas apagadas → 3 verdes → `WYNIK: LLM brain` | Ves el resultado. Detrás hay varias decenas de intentos. |

### BLOQUE C — Demo intercalado (dentro del bloque B)

No son slides: es una segunda pestaña. Aparece dos veces y es la única "prueba" del webinar.

- `0030-0036`, 00:29:32 – 00:41 — **Obsidian** con *Podgląd grafu* (vista de grafo). Barra lateral real:
  `raw · agencies · assets · wiki · analyses · concepts · entities · segments (duzi-marka, duzi-performance, msp-marka, msp-performance) · sources · index · log · overview · CLAUDE`.
  Panel de filtros: `Grupy / Wyświetlanie / Siły` (Grupos / Visualización / Fuerzas).
- `0035`, `0037-0040`, 00:35:03 y 00:41:24 – 00:46 — **`prezentacja5.html`**, cabecera
  `RENTGEN RYNKU AGENCJI` (*Radiografía del mercado de agencias*), ficha `#038 / LEADY DLA MAŁYCH FIRM`.
  Empresa real analizada en pantalla: **Kadrio · Wrocław**, etiqueta `AI SEO i GEO · Poziom 4 z 4: własna technologia`.
  Bloques: `Czym się wyróżnia` (LEPSZA OD RYNKU / SŁABSZA OD RYNKU) · `Co zrobić, żeby się wyróżnić`
  (01 *Idź w głąb* · 02 *Dołóż czwarty dowód* · 03 *Zajmij branżę bez gospodarza`) ·
  `Pozycja na tle rynku` · `Oferta wobec rynku` · `Mapa rynku` (4 cuadrantes: Leady dla małych firm 25 /
  Wyniki dla dużych marek 13 / Marka małych firm 9 / Kampanie dużych marek 12; ejes *Chcę leadów ↔ Chcę marki*
  y *Płaci mała firma ↔ Płaci duża marka`) · `Klienci i własne słowa` (17 marcas citadas).

### BLOQUE A-2 — Giro y venta de Damian (00:56 – 01:23)

| Frame / t | Kicker | Titular | Traducción |
|---|---|---|---|
| `0048-0049` 00:56:47 | `PREZENT DLA OBECNYCH NA ŻYWO` | (repetición del slide del regalo) | — |
| `0050` 00:57:12 | `WRÓĆMY DO POCZĄTKU` | **Przewagą nie jest lepszy prompt.** | Volvamos al principio. La ventaja no es un prompt mejor. |
| `0051` 00:57:48 | `PROBLEM NIE LEŻY W MODELU AI` | **Za każdym razem tłumaczysz AI firmę od początku.** | El problema no está en el modelo de IA. Cada vez le explicas la empresa a la IA desde cero. |
| `0052` 00:59:12 | `I TU POJAWIA SIĘ LUKA` | **Kto przygotuje firmę do realnej pracy z AI?** | Y aquí aparece el hueco. ¿Quién va a preparar la empresa para trabajar de verdad con IA? |
| `0053-0057` 01:01:06 | `Ostatnie 50 minut` | **Czy zgodzisz się ze mną, że to szkolenie to dobrze spędzony czas?** *Daj znać na czacie.* (con comentarios del chat superpuestos en el slide) | Los últimos 50 minutos. ¿Estás de acuerdo conmigo en que esta formación ha sido tiempo bien invertido? Dilo en el chat. |
| `0059` 01:01:54 | `MAM JESZCZE JEDNĄ RZECZ` | **Czy chcecie usłyszeć krótką propozycję dla osób, które chcą nauczyć się budować takie systemy?** | Tengo una cosa más. ¿Queréis oír una propuesta breve para quien quiera aprender a construir estos sistemas? |
| `0060-0078` 01:02:11–01:03:17 | *(VSL, marca `GŁOS WŁĄCZONY`)* | Vídeo con rótulos: *Nie wie, jak pracują zespoły.* / *Gdzie jest wiedza i którym źródłom ufać.* / *AI Operator rozmawia z zespołami.* / *Nie musisz być programistą, żeby wejść w tę rolę.* / *kontekst* | No sabe cómo trabajan los equipos. Dónde está el conocimiento y en qué fuentes confiar. El AI Operator habla con los equipos. No hace falta ser programador para entrar en este rol. |
| `0079-0081` 01:03:24 | `DZIŚ OTWIERAMY PRZEDSPRZEDAŻ` | **AI-Operators** — *5-tygodniowy program, który uczy delegować AI realne procesy.* | Hoy abrimos la preventa. AI-Operators: programa de 5 semanas que enseña a delegar procesos reales a la IA. |
| `0082` 01:04:03 | `TWOJA TRANSFORMACJA` | `DZIŚ` **Używasz AI dorywczo. (np. ChataGPT)** → `PO 5 TYGODNIACH` **Projektujesz system AI, który zna Twoją pracę.** | Tu transformación. HOY: usas la IA de forma ocasional (p. ej. ChatGPT). TRAS 5 SEMANAS: diseñas un sistema de IA que conoce tu trabajo. |
| `0083-0084` 01:04:33 | `TEN PROBLEM MA DWIE ODSŁONY` | `DLA NIETECHNICZNYCH` **W firmie są wiedza i procesy, ale brakuje osoby, która przygotuje je pod AI.** — `DLA TECHNICZNYCH` **Masz systemy i API, ale agent potrzebuje bezpiecznych narzędzi, żeby z nich korzystać.** | Este problema tiene dos caras. NO TÉCNICOS: en la empresa hay conocimiento y procesos, pero falta la persona que los prepare para la IA. TÉCNICOS: tienes sistemas y APIs, pero el agente necesita herramientas seguras para usarlos. |
| `0085` 01:05:12 | `REZULTAT ŚCIEŻKI DLA NIETECHNICZNYCH` | **Możesz zostać osobą od AI, która przygotowuje firmę do pracy z AI.** | Resultado de la vía no técnica: puedes convertirte en la persona de la IA, la que prepara la empresa para trabajar con IA. |
| `0086` 01:06:42 | `JEDEN PROGRAM` | **Wspólny fundament. Dwie równorzędne ścieżki.** — `TYGODNIE 1-4` → `DLA NIETECHNICZNYCH` / `DLA TECHNICZNYCH`; pie: *Masz dostęp do obu. Wybierasz projekt dopiero w 5. tygodniu.* | Un solo programa. Base común. Dos vías equivalentes. Semanas 1-4 → para no técnicos / para técnicos. Tienes acceso a ambas. Eliges proyecto solo en la 5ª semana. |
| `0087` 01:06:54 | `TYDZIEŃ 1` | **Wybierasz proces, który naprawdę warto oddać AI.** *Rozmowa, workflow czy agent? Podejmujesz decyzje na podstawie wartości, ryzyka i kosztu.* `REZULTAT: Mapa własnego procesu` | Semana 1: eliges el proceso que de verdad merece la pena delegar a la IA. ¿Conversación, workflow o agente? Decides según valor, riesgo y coste. RESULTADO: mapa de tu propio proceso. |
| `0088` 01:08:30 | `TYDZIEŃ 2` | **Budujesz agenta, który przejmuje powtarzalne zadanie.** *Dajesz mu rolę, narzędzia, granice działania i sposób oceny wyniku.* `REZULTAT: Działający, przetestowany agent` | Semana 2: construyes un agente que asume la tarea repetitiva. Le das rol, herramientas, límites de actuación y forma de evaluar el resultado. RESULTADO: agente funcionando y probado. |
| `0089` 01:09:24 | `TYDZIEŃ 3` | **Twój sposób pracy staje się kontekstem dla AI.** *Zapisujesz źródła prawdy, instrukcje, przykłady i procedury, aby agent nie zgadywał.* `REZULTAT: Wersjonowany kontekst i własny skill` | Semana 3: tu forma de trabajar se convierte en contexto para la IA. Registras fuentes de verdad, instrucciones, ejemplos y procedimientos para que el agente no adivine. RESULTADO: contexto versionado y skill propio. |
| — *(no capturada)* 01:10:10 | `TYDZIEŃ 4` | **Bazy danych / baza wiedzy dla agenta** (grafos, RAG) | Semana 4: bases de datos / base de conocimiento para el agente. |
| `0090` 01:11:18 | `PRZYKŁAD DLA NIETECHNICZNYCH` | **Co składa się na ten projekt?** | Ejemplo para no técnicos: ¿de qué se compone este proyecto? |
| `0091` 01:16:33 | `„CZY TO MI SIĘ PRZYDA W PRACY?"` | **Jeśli w Twojej pracy są informacje, decyzje i powtarzalne zadania, masz co oddać AI.** — fila `MARKETING · SPRZEDAŻ · OPERACJE · HR · IT · ANALIZA` | "¿Esto me va a servir en mi trabajo?" Si en tu trabajo hay información, decisiones y tareas repetitivas, tienes qué delegar a la IA. |
| `0092` 01:16:57 | `NIE MASZ POMYSŁU NA PROJEKT?` | **Nie musisz przychodzić z gotowym.** *Pomożemy Ci znaleźć proces w Twojej pracy i pokażemy kompletny przykład.* | ¿No tienes idea para el proyecto? No hace falta que vengas con una lista. Te ayudamos a encontrar el proceso en tu trabajo y te enseñamos un ejemplo completo. |
| `0093` 01:17:12 | — | **PROGRAM ZAPROJEKTOWANY DLA OSÓB NA ETACIE** (recuadro central vacío en la captura) | Programa diseñado para personas con empleo por cuenta ajena. |
| `0094` 01:17:45 | `NIE ZOSTAJESZ SAM Z MATERIAŁAMI` | **Budujesz z nami. Dostajesz feedback.** | No te quedas solo con los materiales. Construyes con nosotros. Recibes feedback. |
| `0095` 01:17:57 | `UCZESTNICZKA NASZYCH SZKOLEŃ` | **Katarzyna Kot** — *Audytor Jakości Produkcji Żywności* — „*Wiedzę wcześniej zarezerwowaną dla programistów przełożyliście na język zrozumiały dla człowieka spoza branży IT.*" | Participante de nuestras formaciones. Auditora de calidad en producción alimentaria: "Habéis traducido a un lenguaje comprensible para alguien de fuera de IT un conocimiento antes reservado a programadores." |
| `0096` 01:18:30 | `PIERWSZA EDYCJA` | **Cena?** | Primera edición. ¿Precio? |
| `0097` 01:18:33 | `NAJPIERW ZDEJMIJMY RYZYKO` | **Masz 7 dni od startu, żeby spokojnie sprawdzić czy to dla Ciebie.** *Jeśli nie, prosisz o zwrot.* | Primero quitemos el riesgo. Tienes 7 días desde el arranque para comprobar con calma si es para ti. Si no, pides la devolución. |
| `0098` 01:19:06 | `PRZEDSPRZEDAŻ` | **Ta cena nie wróci już nigdy.** `DZIŚ 2 WRZEŚNIA` *Kolejne ceny będą wyższe.* | Preventa. Este precio no volverá nunca. HOY, 2 DE SEPTIEMBRE. Los siguientes precios serán más altos. |
| `0099` 01:19:24 | `WAŻNE – zanim podamy cenę...` | **Potrzebujemy minimum 100 osób w przedsprzedaży.** | IMPORTANTE, antes de dar el precio... Necesitamos un mínimo de 100 personas en la preventa. |
| `0100` 01:20:00 | `DODATKOWY KURS ONLINE` / `BEZ PROGRAMOWANIA · DLA NIETECHNICZNYCH` | **Zbuduj głosowego asystenta AI, który odbiera telefony.** *Potrafi odebrać połączenie, także gdy nie odbierasz własnego telefonu, i prowadzić rozmowę głosem brzmiącym jak człowiek.* — `FIRMY PŁACĄ ZA TAKIE ROZWIĄZANIA 500-1200 zł / mies. W ABONAMENCIE` | Curso online adicional. Sin programar · para no técnicos. Construye un asistente de voz con IA que contesta el teléfono. Puede coger la llamada, también cuando tú no coges tu propio teléfono, y mantener la conversación con una voz que suena humana. LAS EMPRESAS PAGAN POR ESTAS SOLUCIONES 500-1200 zł / mes EN SUSCRIPCIÓN. |
| `0101-0103` 01:21:24 | `WARUNEK OTRZYMANIA BONUSU` | **Tylko osoby, które kupią dzisiaj do 23:59, otrzymają dodatkowy kurs online.** | Condición para recibir el bonus: solo quienes compren hoy hasta las 23:59 recibirán el curso online adicional. |
| **`0104`** 01:23:15 | **slide de oferta** (permanece en pantalla ~35 min, hasta el final) | ver §1.1 | |

#### 1.1 El slide de oferta (frame `0104`, en pantalla de 01:23:15 a 01:56:03)

```
AI • Operators                              ┌ PRZEDSPRZEDAŻ DO 02.09 ┐
                                            │  995  zł netto         │
Zostań                                      │       + 23% VAT        │
AI Operatorem. Deleguj                      ├────────────────────────┤
powtarzalne zadania do AI.                  │ EXTRA  DLA NIETECHNICZNYCH
                                            │ KUP DO  23:59
• 5 tygodni nauki i dostęp do obu ścieżek   │ Bez programowania: zbuduj
• Spotkania na żywo oraz feedback           │ głosowego asystenta AI, który
• 12 miesięcy dostępu                       │ odbiera telefony i brzmi jak
• Certyfikat i 7 dni gwarancji              │ człowiek. Firmy płacą za takie
• Start 26 października – ale teraz          │ rozwiązania 500-1200 zł
  w przedsprzedaży najtaniej                │ miesięcznie.
                                            ├────────────────────────┤
                                            │ DOŁĄCZ TERAZ →
                                            │ aioperators.pl/teraz
                                            └ Do 10 rat 0% z PayU Raty
```
*Traducción:* "Conviértete en AI Operator. Delega tareas repetitivas a la IA. · 5 semanas de formación
y acceso a ambas vías · encuentros en directo y feedback · 12 meses de acceso · certificado y 7 días
de garantía · empieza el 26 de octubre, pero ahora en preventa es lo más barato. — PREVENTA HASTA EL
02.09: 995 zł netos + 23% IVA. EXTRA para no técnicos, COMPRA HASTA LAS 23:59… ÚNETE AHORA
aioperators.pl/teraz. Hasta 10 plazos al 0% con PayU Raty."

### BLOQUE A-3 — Cierre (01:49 – 01:56)

| Frame / t | Contenido | Traducción |
|---|---|---|
| `0125-0127` 01:49:15 | **Reprise de la apertura olvidada**: cabecera `AI • Operators / OTWARCIE / 00 : 03`, banda `OD CHAOSU ————— DO PROCESU`, ilustración de un hombre ante papeles volando. Rótulos: *AI pomaga Ci dorywczo.* → *Kolejne zadanie znów zaczynasz od początku.* | Del caos al proceso. La IA te ayuda de forma ocasional. La siguiente tarea la vuelves a empezar desde cero. |
| `0129` 01:49:57 | `WYBIERZ ZDANIE, KTÓRE OPISUJE CIEBIE` — `01` **Chcę wejść głębiej w AI, ale nie wiem, od czego zacząć.** | Elige la frase que te describe. 01: Quiero profundizar en la IA, pero no sé por dónde empezar. |
| `0130` 01:50:27 | **Zostań osobą od AI w swojej firmie.** `aioperators.pl` | Conviértete en la persona de la IA en tu empresa. |
| `0131-0136` hasta 01:56:03 | vuelta permanente al slide de oferta | — |

---

## 2. ESTRUCTURA ARGUMENTAL DEL DECK

El deck ejecuta una **doble espiral**: Damian abre y cierra un bucle de venta, y en medio inserta
un bloque docente de 47 minutos que funciona como *aval*. El argumento completo:

**Fase 1 — Inoculación (00:00–00:04, slides A0-A4).**
No empieza por la promesa, empieza por **desactivar objeciones antes de que se formulen**. El slide
`NIE BĘDZIE / BĘDZIE` es una vacuna: nombra en voz alta los tres formatos de infoproducto que el
espectador ya desprecia ("50 prompts", "20 apps", "un truco mágico") y se coloca fuera de ellos.
Sólo después nombra el producto: *un sistema de IA que conoce tu empresa*. Inmediatamente crea una
**categoría nueva y vacía** (`NOWA KOMPETENCJA W FIRMIE → AI Operator`) — no vende un curso, vende
una identidad profesional que aún no existe y de la que ellos son los definidores. `DWIE DROGI. JEDNA
ROLA.` amplía el mercado direccionable a la vez: técnicos y no técnicos, sin excluir a nadie.

**Fase 2 — Autoridad + gancho de retención (00:04–00:09, slides A5-A8).**
Credenciales (`DWOJE PRAKTYKÓW`) y prueba de suelo moral (`PRAKTYKA, NIE TEORIA — enseñamos lo que
nosotros mismos usamos`). Inmediatamente después, **el gancho de permanencia**: el regalo por estar
en directo (web con IA en cuatro tardes + cómo publicarla + cómo venderla). Nótese que el regalo
**no es del mismo tema que el webinar**: es un side-hustle monetizable. Se coloca en el minuto 8 y se
vuelve a mencionar en el 56 — es el mecanismo que sostiene la audiencia durante el bloque docente.

**Fase 3 — Docencia real (00:09–00:56, deck B, 22 slides).**
Aquí sí se enseña. La arquitectura es rígida y explícita: *5 pasos* (§3.1) mapeados uno a uno contra
*5 competencias que "busca el mercado"* (§3.4). Cada slide de paso muestra a la izquierda la tarjeta
de competencias con **una sola fila iluminada** — el oyente ve en todo momento cuánto le falta.
Ese es el verdadero motor persuasivo del bloque docente: **la tarjeta no es un índice, es una barra
de progreso de una carencia**. Se ilumina 5 veces y en el slide 20 (`Podsumujmy`) aparece entera y
sin resaltar: *ahora ya sabes lo que el mercado busca, y sabes que no lo tienes entero*.

**Fase 4 — Anticlímax honesto (00:55–00:56, slides 21-22).**
Golpe deliberado de sinceridad justo antes de vender: `Teraz powiem wam coś zupełnie szczerze` →
`Widzisz wynik. Za nim stoi kilkadziesiąt podejść.` Una retícula de decenas de casillas apagadas y
sólo tres verdes. Ola desmonta su propio demo ("*ja zawsze bardzo lubię obalać hype*" — "siempre me
gusta echar abajo el hype"). **Función real:** eliminar la última objeción posible ("esto es marketing
mágico") y, a la vez, argumentar implícitamente que hacer esto solo cuesta decenas de intentos —
premisa exacta que el programa de pago promete ahorrar. Es el pivote docencia→venta más elegante del
deck y está construido con el material de la honestidad.

**Fase 5 — El pivote (00:57–01:01, slides A10-A12).**
Tres slides encadenados en cadena lógica cerrada:
1. `Przewagą nie jest lepszy prompt.` (invalida la alternativa barata)
2. `Za każdym razem tłumaczysz AI firmę od początku.` (nombra el dolor con la 2ª persona)
3. `Kto przygotuje firmę do realnej pracy z AI?` (**el hueco**) — pregunta cuya única respuesta
   disponible es la identidad inventada en la Fase 1: *el AI Operator*.
El argumento se ha cerrado sobre sí mismo: se creó una categoría en el minuto 3, se demostró su
dificultad en los minutos 9-56, y en el minuto 59 se abre el vacío que sólo esa categoría llena.

**Fase 6 — Micro-compromiso y permiso (01:01–01:02, slides A13-A14).**
Antes del pitch, dos slides que piden consentimiento: `¿Estás de acuerdo en que ha sido tiempo bien
invertido? Dilo en el chat` (compromiso público que genera consistencia) y `¿Queréis oír una propuesta
breve?` — pregunta que **él mismo responde**: *"ale w sumie odpowiem sobie sam i pójdę dalej"*
("en realidad me contesto yo solo y sigo"). El permiso es ritual, no real.

**Fase 7 — Pitch (01:03–01:23).**
Orden: apertura de preventa → transformación antes/después → el problema en dos caras → resultado por
vía → estructura del programa (base común 4 semanas + bifurcación en la 5ª) → semana a semana →
"¿me sirve a mí?" → "¿y si no tengo idea?" → "¿y si trabajo por cuenta ajena?" → "no te quedo solo" →
testimonio → **y sólo entonces** el precio. Antes del precio, **tres slides de desactivación de riesgo
en cadena**: garantía de 7 días → "este precio no volverá" → "necesitamos 100 personas o devolvemos
todo". Ese tercero es un movimiento inusual: convierte una condición de negocio en prueba de
integridad *y* en presión social simultáneamente.

**Fase 8 — Escasez apilada (01:20–01:23).**
Dos relojes distintos y superpuestos: preventa **hasta el 02.09** (precio) y bonus **hasta las 23:59
de hoy** (asistente de voz). El bonus lleva su propia promesa de ingresos (500-1200 zł/mes) — es
decir, un ROI declarado que hace que el precio de 995 zł parezca amortizable en un mes.

**Fase 9 — Sostenido (01:23–01:56).**
El slide de oferta ya no se quita. Los 33 minutos de Q&A transcurren **sobre el precio**: cada
respuesta técnica se ve con el CTA y el contador debajo. La venta deja de ser un momento y pasa a ser
el fondo de pantalla.

**Fase 10 — Cierre y bucle (01:49–01:56).**
Damian recuerda que se saltó la apertura de su propio deck (`OD CHAOSU DO PROCESU`, contador 00/03) y
la proyecta **al final**. El efecto es que el webinar se cierra con la misma metáfora con la que la web
abre — y con el slide `WYBIERZ ZDANIE, KTÓRE OPISUJE CIEBIE`, un test de auto-identificación que
devuelve al espectador al punto de partida, ya convertido en segmento.

---

## 3. FRAMEWORKS VISUALES (reproducidos con exactitud)

### 3.1 Los CINCO PASOS — `PIĘĆ KROKÓW` (slide 3, frame `0019`)

```
PIĘĆ KROKÓW
────────────────────────────────────────────
01   Model, automatyzacja albo agent
02   Opis zadania, które oddajesz
03   Kontekst i wiedza firmy
04   Dostęp do narzędzi
05   Ocena jakości wyniku
```
**Traducción:**
```
CINCO PASOS
01   Modelo, automatización o agente
02   La descripción de la tarea que delegas
03   Contexto y conocimiento de la empresa
04   Acceso a herramientas
05   Evaluación de la calidad del resultado
```

### 3.2 EL ÁRBOL DE DECISIÓN — `KROK 01` (slide 8, frames `0023`/`0024` + voz 00:15:12–00:19:37)

En pantalla sólo se capturó la rama TAK; el resto está reconstruido con la locución, que la describe
íntegra. Reconstrucción completa:

```
                                              ┌──────────────────────────┐
                                        TAK → │ B / AUTOMATYZACJA        │
                                              │ Ta sama ścieżka          │
                                              │ (n8n · Make)             │
              ┌───────────────────────┐       └──────────────────────────┘
 ZADANIE ───► │ Ma określone,         │──┤
              │ powtarzalne kroki?    │       ┌──────────────────────────┐
              └───────────────────────┘  NIE→│ MODEL JĘZYKOWY (LLM)     │
                                              └──────────┬───────────────┘
                                          ┌──────────────┴───────────────┐
                              ┌───────────────────────┐   ┌──────────────────────────┐
                              │ A / CZAT              │   │ C / AGENT                │
                              │ okienko czatu         │   │ proces złożony,          │
                              │ pytania i burza       │   │ wieloetapowy, wymaga     │
                              │ mózgów                │   │ krytycznej oceny         │
                              │ (ChatGPT · Claude)    │   │ (Claude Code · Codex)    │
                              └───────────────────────┘   └──────────────────────────┘
```
**Traducción:** TAREA → *¿Tiene pasos definidos y repetibles?* — **SÍ** → B/AUTOMATIZACIÓN, *el mismo
camino siempre* (n8n, Make). **NO** → MODELO DE LENGUAJE, y de ahí dos salidas: **A/CHAT** (ventana de
chat, preguntas y lluvia de ideas — ChatGPT, Claude) y **C/AGENTE** (proceso complejo, multietapa, que
exige juicio crítico — Claude Code, Codex).

Cita literal de la locución (00:15:17): *"Jeśli tak, to bardzo możliwe, że rozwiązaniem tego problemu
w ogóle nie będzie AI, tylko automatyzacja"* — "Si es que sí, es muy posible que la solución a ese
problema no sea IA en absoluto, sino automatización." Y en 00:16:46: *"I większość osób się na tym
poziomie zatrzymuje"* — "Y la mayoría de la gente se queda en ese nivel [el chat]."

*(Nota de transcripción: el ASR escribe "AnyTen" por **n8n**, y "kodkod / kodeks" por **Claude Code /
Codex**.)*

### 3.3 EL DIAGRAMA DE LA TAREA DELEGADA — `KROK 02` (slide 13, frame `0027`)

Numeración desordenada a propósito (01 → 03 → 02 → 04), leyendo en zigzag:

```
01 / WEJŚCIA              03 / NARZĘDZIA               02 / DECYZJE
┌──────────────────┐      ┌──────────────────────┐     ┌──────────────────┐
│ Strony i cenniki │ ───► │ Claude + skill       │ ──► │ Dane starsze     │
│ 8 konkurentów    │      │ Notion·Airtable·     │     │ niż 30 dni?      │
└──────────────────┘      │ Firecrawl            │     └──────────────────┘
        ▲                 └──────────────────────┘              │
        └───────────  TAK → POBIERZ ŚWIEŻE  ────────────────────┘
                                   │
04 / REZULTAT · LLM BRAIN          ▼            NA TEJ PODSTAWIE
┌────────────────────────────────────┐        ┌────────────────────────┐
│ [grafo de nodos]  Baza danych      │  ───►  │ Analiza z wnioskami    │
│                   pamięć dla modelu│        │ [captura del informe]  │
│                   tabela konkurentów│       └────────────────────────┘
│                   zmiany w czasie,  │
│                   format karty      │
└────────────────────────────────────┘
```
**Traducción:** 01/ENTRADAS: webs y tarifas de 8 competidores. 03/HERRAMIENTAS: Claude + skill;
Notion · Airtable · Firecrawl. 02/DECISIONES: *¿datos con más de 30 días?* — **SÍ → descarga datos
frescos** (bucle de vuelta a las entradas). 04/RESULTADO · LLM BRAIN: base de datos, *memoria para el
modelo*; tabla de competidores, cambios en el tiempo, formato de ficha. SOBRE ESA BASE: análisis con
conclusiones.

### 3.4 EL MAPA DE COMPETENCIAS — `TEGO SZUKA RYNEK` (tarjeta persistente, slides 5, 8, 11, 13, 15, 19, 20)

```
TEGO SZUKA RYNEK
(◉)  ══════════════════════════

✓  Płynność w narzędziach AI
   wiesz, kiedy przełączyć narzędzie
✓  Myślenie systemami
   powtarzalny proces zamieniasz w automatyzację
✓  Wewnętrzne narzędzia
   na danych firmy, na przykład z 10 projektów
✓  Zdolność prototypowania
   pomysł zmieniasz w działające demo
✓  Wynik realnie rozwiązuje problem
   ocena, czy narzędzie trafia w problem
```
**Traducción — ESTO ES LO QUE BUSCA EL MERCADO:**
```
✓  Fluidez en las herramientas de IA
   sabes cuándo cambiar de herramienta
✓  Pensamiento en sistemas
   conviertes un proceso repetitivo en automatización
✓  Herramientas internas
   sobre datos de la empresa, por ejemplo de 10 proyectos
✓  Capacidad de prototipar
   conviertes una idea en una demo que funciona
✓  El resultado resuelve el problema de verdad
   evaluación de si la herramienta acierta con el problema
```

**Emparejamiento paso ↔ competencia** (deducido del resaltado verde de cada slide):

| Paso | Competencia iluminada |
|---|---|
| KROK 01 · Model, automatyzacja albo agent | Płynność w narzędziach AI |
| KROK 02 · Opis zadania, które oddajesz | Myślenie systemami |
| KROK 03 · Kontekst i wiedza firmy | Wewnętrzne narzędzia |
| KROK 04 · Dostęp do narzędzi | Zdolność prototypowania |
| KROK 05 · Ocena jakości wyniku | Wynik realnie rozwiązuje problem |

### 3.5 LA TRÍADA DE CONTEXTO — `KROK 03 · Kontekst i wiedza firmy` (slide 15, frame `0034`)

```
┌─────────────────────────┐ ┌─────────────────────────┐ ┌─────────────────────────┐
│ Źródła prawdy           │ │ Pamięć                  │ │ Skill                   │
│                         │ │                         │ │            (resaltado)  │
│ Fakty z jednego adresu. │ │ Ustalenia, które zostają│ │ Sposób pracy:           │
│                         │ │                         │ │ kroki i format.         │
│ 📄 💲                   │ │ 🔷 Obsidian             │ │ 🗒                       │
│ 📄 tabela konkurentów   │ │ 🕸 graf notatek         │ │ ✳ analiza konkurencji   │
└─────────────────────────┘ └─────────────────────────┘ └─────────────────────────┘
```
**Traducción:**
- **Fuentes de verdad** — *Hechos desde una sola dirección.* → tabla de competidores.
- **Memoria** — *Acuerdos que permanecen.* → Obsidian, grafo de notas.
- **Skill** — *La forma de trabajar: pasos y formato.* → análisis de competencia.

Es el núcleo conceptual del webinar entero y la tesis que la web repite: *dato ≠ memoria ≠
procedimiento*, y las tres capas hay que construirlas por separado.

### 3.6 LA RUEDA DE APLICACIONES — `KROK 05 · ZANIM OCENIMY JAKOŚĆ` (slide 18, frame `0042`)

Seis satélites alrededor de un icono de cerebro (`LLM brain`), titular
**"To samo ułożysz dla wielu innych spraw"** ("Lo mismo lo montas para muchos otros asuntos"):

```
                       Nauka tematu
                       kursy i artykuły
        Obsługa klienta          Wiedza działu
        powtarzalne pytania      procedury i ustalenia
                    ⟨ LLM brain ⟩
        Cenniki i oferty         Osobisty doradca
        zmiany na rynku          twoje notatki
                       Rekrutacja
                       kandydaci w jednym formacie
```
**Traducción:** Aprender un tema (cursos y artículos) · Atención al cliente (preguntas repetitivas) ·
Conocimiento del departamento (procedimientos y acuerdos) · Tarifas y ofertas (cambios en el mercado) ·
Asesor personal (tus notas) · Selección de personal (candidatos en un mismo formato).

### 3.7 LA BIFURCACIÓN DEL PROGRAMA — `JEDEN PROGRAM` (frame `0086`)

```
JEDEN PROGRAM
Wspólny fundament. Dwie równorzędne ścieżki.

                       ┌──────────────────────────┐
   TYGODNIE 1-4 ───────┤ DLA NIETECHNICZNYCH      │
                       ├──────────────────────────┤
                       │ DLA TECHNICZNYCH         │
                       └──────────────────────────┘

   Masz dostęp do obu. Wybierasz projekt dopiero w 5. tygodniu.
```
**Traducción:** UN SOLO PROGRAMA. Base común. Dos vías equivalentes. SEMANAS 1-4 → para no técnicos /
para técnicos. Tienes acceso a ambas. Eliges proyecto solo en la 5ª semana.
*(Función comercial: elimina la objeción "¿cuál compro?" y elimina la posibilidad de que alguien
decida que ninguna de las dos es la suya.)*

### 3.8 LA ESCALERA DE ENTREGABLES SEMANALES (frames `0087-0089` + voz)

| Semana | Titular | `REZULTAT` (entregable) |
|---|---|---|
| 1 | Wybierasz proces, który naprawdę warto oddać AI | Mapa własnego procesu |
| 2 | Budujesz agenta, który przejmuje powtarzalne zadanie | Działający, przetestowany agent |
| 3 | Twój sposób pracy staje się kontekstem dla AI | Wersjonowany kontekst i własny skill |
| 4 | *(no capturada)* bazy danych / baza wiedzy dla agenta: grafos y RAG | — |
| 5 | Proyecto por vía: 05A proceso de negocio / 05B servidor MCP + agente diagnóstico | Proyecto de portfolio |

Cada semana cierra con un artefacto nombrado. Es la contrapartida estructural del anticlímax de Ola
("decenas de intentos"): el programa se presenta como el atajo que convierte esos intentos en cinco
entregables datados.

---

## 4. QUÉ SLIDES SON DOCENCIA Y CUÁLES SON VENTA

### 4.1 Docencia pura (contenido que sirve aunque no compres)

| Slides | Por qué es docencia |
|---|---|
| B03 `PIĘĆ KROKÓW` | Taxonomía completa, entregada entera y sin retención |
| B08 `KROK 01` + árbol | **La pieza de mayor valor del webinar.** Ola la llama explícitamente *"taki booster, który możecie od razu sobie wykorzystać"* ("un booster que podéis usar ya mismo"). Enseña a decidir cuándo NO usar IA — argumento que va contra su propio interés comercial |
| B11 `PRZYKŁAD` | Enunciado del caso, verificable |
| B13 diagrama de la tarea | Arquitectura reutilizable: entradas / herramientas / decisiones / resultado + regla de frescura |
| B15 tríada `Źródła prawdy / Pamięć / Skill` | Modelo conceptual transferible a cualquier stack |
| B18 rueda de 6 casos | Generalización honesta del método |
| B19 `Ocena jakości wyniku` | Trazabilidad + casos de test: la parte que los infoproductos suelen omitir |
| B21-B22 anticlímax | Desmontaje del hype, cuantificado ("decenas de intentos") |
| C (Obsidian + Rentgen) | Demo real, navegable, con datos concretos |

### 4.2 Venta disfrazada de docencia (zona gris — la parte más interesante)

| Slides | Mecanismo |
|---|---|
| **La tarjeta `TEGO SZUKA RYNEK`** | Presentada como mapa de competencias del mercado, funciona como **auditoría de carencias**. Nadie la cita, nadie la fundamenta: es una afirmación de mercado sin fuente que legitima el producto. Aparece 7 veces |
| A2 `NIE BĘDZIE / BĘDZIE` | Parece transparencia, es inoculación de objeciones |
| A3 `NOWA KOMPETENCJA W FIRMIE` | Parece observación de mercado, es creación de categoría propietaria |
| A6 `PRAKTYKA, NIE TEORIA` | Parece principio pedagógico, es prueba de autoridad |
| B14 "*lo puede montar hasta quien trabaja en una caja*" | Parece inclusividad, es eliminación de la objeción "yo no sé programar" |
| B22 `Za nim stoi kilkadziesiąt podejść` | Parece honestidad (y lo es), pero simultáneamente **justifica el precio**: el atajo vale dinero |
| C `Rentgen agencji` | Parece demo educativa; es sobre todo prueba de resultado — no se enseña cómo se genera el HTML |

### 4.3 Venta explícita

Todo el bloque A-2 desde `0050` (00:57:12) en adelante: el pivote (A10-A12), el micro-compromiso
(A13-A14), el VSL, el pitch (A15-A28), el precio y la escasez (A29-A34), el slide de oferta
persistente (A35) y el cierre (A36-A38). **28 de las 137 capturas (20%) son literalmente el mismo
slide de oferta** (`0104`-`0124`, `0127`, `0131`-`0136`), sostenido durante 33 minutos.

### 4.4 Reparto real del tiempo

| Bloque | Duración | % |
|---|---|---|
| Encuadre + gancho (A-1) | 00:00–00:09 | 8% |
| Docencia + demo (B + C) | 00:09–00:56 | **40%** |
| Pivote + pitch (A-2) | 00:57–01:23 | 22% |
| Q&A **sobre el slide de oferta** | 01:23–01:56 | 30% |

Es decir: **el 52% del webinar transcurre con material de venta en pantalla**, y sólo el 40% enseña.
Pero el 40% que enseña es genuino y de calidad, y ahí está la eficacia del embudo.

---

## 5. IDEAS QUE APARECEN **SOLO EN PANTALLA** Y NO SE DICEN EN VOZ ALTA

Verificado por búsqueda directa sobre `transcripcion.md`.

**5.1 La regla de los 30 días.** El diagrama del slide 13 contiene el nodo `02 / DECYZJE — Dane
starsze niż 30 dni? · TAK → POBIERZ ŚWIEŻE` ("¿Datos con más de 30 días? Sí → descarga datos
frescos"). `grep "30 dni"` sobre la transcripción **no devuelve nada**. Es la única política de
caducidad de datos de todo el webinar y se entrega en silencio.

**5.2 La numeración desordenada 01→03→02→04** del mismo diagrama (entradas, luego herramientas, luego
decisiones) codifica un orden de diseño distinto al de ejecución. Nunca se comenta.

**5.3 El certificado.** `Certyfikat i 7 dni gwarancji` está en el slide de oferta durante 33 minutos.
`grep -i "certyfikat"` → **cero apariciones habladas**. Se menciona la garantía largamente; el
certificado, jamás.

**5.4 Los subtítulos de la tarjeta de competencias.** *"na danych firmy, na przykład z 10 projektów"*
y *"pomysł zmieniasz w działające demo"* se leen en cada slide pero nunca se enuncian como tales.

**5.5 "W ABONAMENCIE".** El slide del bonus remata la cifra 500-1200 zł con `W ABONAMENCIE` ("en
suscripción" — es decir, recurrente). En voz sólo se dice *"między 500 a 1200 złotych miesięcznie"*.
La palabra que convierte un ingreso puntual en renta mensual está solo escrita.

**5.6 La arquitectura del propio deck.** Secciones (`PLAN`, `KROK 01-05`, `PODSUMOWANIE`, `DOMKNIĘCIE`,
`OTWARCIE`) y contador `NN / 22`. Nunca se nombran; funcionan como promesa silenciosa de que "queda
poco" durante los 47 minutos docentes.

**5.7 Metadatos filtrados por la barra de direcciones.** Visibles en una veintena de capturas y jamás mencionados:
- el deck docente es **`prezentacja-system-ai-v21.html`** → versión **21** de la presentación;
- vive en `Desktop/**Instagram**/` → carpeta de producción de contenido para redes;
- el demo estrella es **`artefakty/prezentacja5.html`**, dentro de `Desktop/Self-firma/` → "artefacto
  nº 5" de un directorio llamado *auto-empresa*.
  El demo que se presenta como salida orgánica del LLM brain está guardado como un artefacto numerado
  en la carpeta de material propio.

**5.8 El título de la pestaña del demo: "Rentgen agencji w ciemności"** ("Radiografía de agencias a
oscuras"). Es el nombre interno del proyecto y no se pronuncia nunca.

**5.9 Una empresa real con nombre y juicio.** El demo muestra **Kadrio · Wrocław** con veredictos
`LEPSZA OD RYNKU` / `SŁABSZA OD RYNKU: Węższa oferta` ("oferta más estrecha") y citas literales de su
web ("«SEO na luzie»"). En voz se habla de "una de las agencias elegidas" sin nombrarla.

**5.10 La frase-tesis del segundo slide.** `W obu przypadkach cel jest ten sam: przejść od dorywczego
używania AI do systemu pracy` — la formulación más limpia de toda la propuesta de valor está a pie de
página del slide A1 y Damian no la lee.

**5.11 El formato de la garantía.** El slide dice *7 dni **od startu*** (7 días **desde el arranque**,
no desde la compra). Damian sí lo aclara en voz, pero sólo una vez y 5 minutos después; la letra que
convierte "7 días" en "7 días a partir del 26 de octubre" está sobre todo en pantalla.

**5.12 `PROGRAM ZAPROJEKTOWANY DLA OSÓB NA ETACIE`** ("programa diseñado para gente con empleo por
cuenta ajena") aparece con un recuadro central **vacío** en la captura: el contenido que justificaba
la afirmación no llegó a cargar/mostrarse, y en voz no se sustituye.

**5.13 El slide olvidado.** La apertura `OD CHAOSU DO PROCESU` (contador `00 : 03`) **no se proyectó al
principio**: Damian la descubre en el minuto 109 (*"O właśnie jeszcze zapomniałem tego pokazać"* — "Ah,
justo se me olvidó enseñar esto"). Es el eje narrativo que la web usa como hero (`Od chaosu do
procesu`, pasos 01-05 en `index.txt`) y en el webinar apareció por accidente y al final.

**5.14 Desalineación slide ↔ voz en el minuto 71.** En pantalla `PRZYKŁAD DLA NIETECHNICZNYCH`, mientras
Damian anuncia *"najpierw teraz opowiem o ścieżce dla technicznych"* ("primero hablaré de la vía
técnica"). El deck y el discurso van en direcciones opuestas durante ese tramo.

---

## 6. RELACIÓN CON LA WEB (aioperators.pl)

La web es la **versión estable** del mismo argumento; el deck es su versión temporizada.

| Elemento | Web (`index.txt`) | Deck |
|---|---|---|
| Narrativa maestra | `Od chaosu do procesu` 01-05, con scroll | slide de apertura `OD CHAOSU ——— DO PROCESU` (mostrado al final) |
| Rol | *Kim jest AI Operator?* | `NOWA KOMPETENCJA W FIRMIE` |
| Tríada | *Plik kontekstowy / Pamięć / Skill / Baza wiedzy* | `Źródła prawdy / Pamięć / Skill` |
| Bifurcación | *Wspólny start / tygodnie 1-4 → 05A / 05B* | `JEDEN PROGRAM · TYGODNIE 1-4` |
| Prueba social | Klaudia Szewczuk (abogada, "30 h/mes ahorradas") | Katarzyna Kot (auditora alimentaria) — **testimonios distintos en cada canal** |
| Escasez | *Przedsprzedaż do 2 września* | `PRZEDSPRZEDAŻ DO 02.09` + `KUP DO 23:59` |
| Precio | no aparece en el texto capturado | **995 zł netto + 23% VAT**, solo en el webinar |

El precio vive únicamente detrás del webinar. Ese es el sello de que el webinar no es contenido: es la
puerta de precio.

---

## 7. LAGUNAS Y CAVEATS DE LA RECONSTRUCCIÓN

- **Slides no capturadas** del deck docente: 4, 6, 7, 9, 10, 12, 14, 16, 17, 21 parcialmente
  (el muestreo de frames tiene huecos de hasta 4 minutos). Las ramas A y C del árbol de decisión
  (§3.2) y el bloque `KROK 04 · Dostęp do narzędzi` están reconstruidos **desde la locución**, no
  desde OCR. Están marcados como tales.
- **Deck A sin numeración visible** salvo en el frame `0126` (`00 : 03`), por lo que su recuento total
  de slides no es determinable; el orden aquí es cronológico, no de índice.
- **Discrepancia de fecha:** el reloj de Windows en las capturas marca `20.08.2026`, mientras el deck
  anuncia `DZIŚ 2 WRZEŚNIA` y `PRZEDSPRZEDAŻ DO 02.09`. O el reloj de la máquina está desajustado, o
  la grabación es de un ensayo/reemisión distinta de la fecha comercial anunciada. **No se ha podido
  resolver con el material disponible** y conviene no dar por buena ninguna de las dos fechas.
- **El OCR de tesseract** carece de diacríticos polacos y confunde sistemáticamente `AI`→`Al`,
  `ż/ź`→`z`, `ć`→`c`, `ę`→`e`. Todas las citas de este documento están re-normalizadas a polaco
  correcto y contrastadas contra la imagen original o la transcripción cuando la reconstrucción no era
  obvia.
