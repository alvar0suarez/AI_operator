# Lo que REALMENTE se ve en pantalla — análisis visual de los frames

Fuente: `/home/user/AI_operator/materiales/fuentes/webinar-damian-naprawa/frames/` (137 capturas .jpg,
1920×1080), cotejado con `informe.md`, `transcripcion.md` y `web-aioperators/index.txt`.

Método: he **abierto como imagen** los frames, no solo leído su OCR. Frames vistos a tamaño completo:
`0022, 0024, 0026, 0027, 0028, 0029, 0030, 0031, 0032, 0033, 0034, 0035, 0036, 0037, 0038, 0039, 0040,
0041, 0042, 0043, 0046`. Además he recortado y ampliado ×2–×6 con Pillow doce regiones concretas
(barra lateral de Obsidian, tres zonas del grafo, la constelación del artefacto, tres zonas del
dashboard, el indicador de progreso del artefacto, el nodo `mmponline`, la rejilla de la slide 22).

> **Aviso metodológico importante.** La consigna pedía "al menos 20 capturas del tramo 00:26–00:47".
> Ese tramo **solo contiene 15 capturas** (`0027`…`0041`). Las he visto todas, y he añadido seis más
> del entorno inmediato. El propio muestreo de frames es una pista: en 21 minutos de "demo real" el
> extractor solo detectó 15 cambios de pantalla, mientras que en los 4 minutos del pitch de venta
> (01:01–01:05) detectó **33**. La demo es visualmente estática; el cierre comercial no.

---

## 1. Qué software se ve exactamente, y cuándo

**Máquina:** Windows 11 en polaco. Usuario `Lenovo` (todas las rutas son `C:/Users/Lenovo/…`).
Reloj de la barra de tareas: **20.08.2026**, de 20:13 a 20:55 a lo largo del tramo analizado.
Widget de tiempo abajo a la izquierda: *"Cz. słonecznie / Cz. pochmurnie, 20°C"*.

**Apps ancladas en la barra de tareas** (visibles en todos los frames): Explorador de archivos, Edge,
Chrome, **Obsidian** (icono morado) y **Claude** (asterisco naranja de Anthropic). No hay VS Code,
ni Cursor, ni ninguna terminal anclada. En la barra de extensiones de Chrome hay tres iconos, uno de
ellos el mismo asterisco naranja de Claude.

**Chrome tiene siempre 3 pestañas abiertas** (más la pestaña roja de grabación):
1. `System AI, który zna Twoją prac…` → `file:///C:/Users/Lenovo/Desktop/Instagram/prezentacja-system-ai-v21.html#slide=N`
2. `Rentgen agencji w ciemności` → `file:///C:/Users/Lenovo/Desktop/Self-firma/artefakty/prezentacja5.html`
3. `StreamYard - Studio`

Es decir: **todo lo que se proyecta son ficheros HTML locales abiertos con `file://`**, más Obsidian.
No hay ninguna herramienta en la nube, ningún panel de Notion/Airtable/Firecrawl, ningún terminal.

### Cronología exacta del tramo de demo

| t | Frame | Qué hay en pantalla |
|---|---|---|
| 00:13:39 | `0022` | Deck, slide **06/22**. Transición con el texto gigante *"Każdy z tych kroków wykonasz bez programowania"* ("cada uno de estos pasos lo harás sin programar") |
| 00:15:39 | `0024` | Deck **08/22**, diagrama `ZADANIE → ¿tiene pasos repetibles? → TAK → B/AUTOMATYZACJA` |
| 00:20:09 | `0026` | Deck **11/22**, `PRZYKŁAD — Analiza konkurencji` |
| **00:26:15** | `0027` | Deck **13/22**, `KROK 02 — Opis zadania, które oddajesz`. **Éste es el único sitio donde se ve la arquitectura del sistema, y es un dibujo, no software** (ver §5) |
| 00:26:45 | `0028` | Deck **14/22**, pantalla negra: *"Teraz pokażę, jak powstaje LLM brain"* + *"Wygląda na skomplikowane, a złoży go też osoba pracująca na kasie, z zawodem zupełnie spoza biznesu. Programowanie nie jest tu potrzebne."* |
| 00:27:33 | `0029` | Deck **15/22**, `Kontekst i wiedza firmy`: tres tarjetas *Źródła prawdy / Pamięć (Obsidian, graf notatek) / Skill (analiza konkurencji)* |
| **00:29:32** | `0030` | **Primer cambio a Obsidian.** Vista `Podgląd grafu` (Graph view) |
| 00:29:39 | `0031` | Mismo grafo; entra el recuadro de cámara de Damian (*"¿se ve bien?"*) |
| 00:30:12 | `0032` | Grafo alejado (zoom-out) para "dar perspectiva" |
| 00:35:00 | `0033` | Grafo otra vez + se ve el **preview de Alt-Tab de Chrome** (miniaturas de las dos pestañas) |
| 00:35:02 | `0034` | Vuelta al deck **15/22** durante ~1 s |
| **00:35:03** | `0035` | **Artefacto HTML**, escena **1/8**: la constelación de 6 clústeres |
| 00:40:59 | `0036` | Vuelta a Obsidian, grafo (para explicar "si añado una empresa nueva…") |
| 00:41:24 | `0037` | Artefacto, escena **6/8**: `KONCEPTY — Wzorce, które powtarzają się między firmami` |
| 00:42:15 | `0038` | Artefacto, escena **8/8**: el dashboard `Kadrio`, en scroll |
| 00:44:42 / 00:44:48 | `0039` / `0040` | Dashboard completo, ya asentado |
| 00:46:24 | `0041` | Vuelta al deck **15/22** |
| 00:49:09 | `0042` | Deck **18/22** ("lo mismo sirve para otros usos") |
| 00:50:27 | `0043` | Deck **19/22**, `KROK 05 — Ocena jakości wyniku` |
| 00:56:12 | `0046` | Deck **22/22**, `Widzisz wynik. Za nim stoi kilkadziesiąt podejść.` |

**Contabilidad honesta del tiempo de "producto real" en pantalla:**
Obsidian ≈ 29:32→35:02 y 40:59→41:24 → **~6 minutos**.
Artefacto HTML ≈ 35:03→40:59 y 41:24→46:24 → **~11 minutos**.
Total ≈ **17 minutos de 117**. El resto son diapositivas y venta.

---

## 2. La estructura del vault de Obsidian

Ampliando ×2 la barra lateral del frame `0030` (recorte guardado en scratchpad) el árbol se lee
sin ambigüedad. Está en el mismo estado en `0030`, `0031`, `0032`, `0033` y `0036` — **nunca se
despliega ni una carpeta más durante todo el webinar**.

```
<raíz del vault>              ← casi con seguridad C:\Users\Lenovo\Desktop\Self-firma\
├── artefakty/          ▸ (colapsada, NUNCA se abre)
├── raw/                ▾
│   ├── agencies/       ▸ (colapsada)
│   └── assets/         ▸ (colapsada)
├── wiki/               ▾
│   ├── analyses/       ▸ (colapsada)
│   ├── concepts/       ▸ (colapsada)
│   ├── entities/       ▸ (colapsada)
│   ├── segments/       ▾
│   │   ├── duzi-marka
│   │   ├── duzi-performance
│   │   ├── msp-marka
│   │   └── msp-performance
│   ├── sources/        ▸ (colapsada)
│   ├── index           (index.md)
│   ├── log             (log.md)
│   └── overview        (overview.md)
└── CLAUDE              (CLAUDE.md, en la raíz, al mismo nivel de sangrado que artefakty/raw/wiki)
```

**Deducción de la raíz:** el artefacto se sirve desde `C:/Users/Lenovo/Desktop/Self-firma/artefakty/prezentacja5.html`
y el vault tiene una carpeta `artefakty` en la raíz → **el vault es `Desktop\Self-firma\` y Claude Code
escribe el HTML dentro del propio vault**. Es una pieza de arquitectura que ellos no verbalizan pero
que se deduce de la barra de direcciones.

### Rol de cada pieza (deducido de lo que se ve + lo que se dice)

| Pieza | Qué es | Rol en el sistema |
|---|---|---|
| `CLAUDE.md` (raíz) | Fichero de instrucciones de Claude Code | El "sistema operativo" del agente: reglas, formato de nota, cómo enlazar. **Nunca se abre en pantalla.** Es literalmente el fichero más importante del montaje y no se enseña ni una línea |
| `raw/agencies/` | Volcado bruto de las webs de las ~60 agencias (Firecrawl) | Materia prima inmutable. Zona de "no tocar" |
| `raw/assets/` | Imágenes/PDF/capturas asociados | Adjuntos del scraping |
| `wiki/sources/` | Una nota por página fuente | Los nodos grises `xxx-pl` / `xxx-com` del grafo. Es la **capa de trazabilidad**: cada afirmación puede volver a su URL y fecha (es exactamente lo que promete la slide 19/22, *"Każde zdanie ma notatkę"*) |
| `wiki/entities/` | Una nota por agencia (59 fichas) | Los nodos de color del grafo. Ficha estructurada: posicionamiento, precios, clientes, claims |
| `wiki/segments/` | **4 notas fijas**: `duzi-marka`, `duzi-performance`, `msp-marka`, `msp-performance` | Los 4 hubs gordos del grafo. Taxonomía 2×2: (grande/pyme) × (marca/rendimiento) |
| `wiki/concepts/` | ~20 notas de patrón transversal | `archetypy-claimow`, `mechanizmy-dowodzenia`, `sygnaly-jakosci-strony`, `szeroka-oferta-jako-ryzyko`, `strony-miastowe-pod-seo`… (leídos directamente del grafo) |
| `wiki/analyses/` | 8 notas de conclusión | Comparativas, matrices de servicios/precios, mapa de posicionamiento, huecos de mercado |
| `wiki/index` | Índice | Punto de entrada del agente al vault |
| `wiki/overview` | Resumen ejecutivo | Vista de conjunto |
| `wiki/log` | Registro | Historial de qué se añadió/actualizó y cuándo — la pieza de "versionado" del contexto |
| `artefakty/` | Salidas HTML | Donde vive `prezentacja5.html` |

**Detalle revelador:** la nomenclatura está **mezclada en dos idiomas**. Carpetas en inglés
(`agencies`, `wiki`, `analyses`, `concepts`, `entities`, `segments`, `sources`, `assets`, `index`,
`log`, `overview`) y contenido en polaco (`duzi-marka`, `msp-performance`, `archetypy-claimow`).
Ola lo justifica de pasada en voz: *"one mi się tutaj zapisały po angielsku… to jest po prostu przez
sposób, w jaki pracowałam"* ("me salieron en inglés, es simplemente por cómo trabajaba"). Traducción
real: **el LLM eligió los nombres, no ella.** No hay una convención de nombres diseñada.

En el raíl de iconos de la izquierda de Obsidian, además de los habituales, hay un icono **`>_`
(terminal)**. Obsidian no lleva terminal de serie: es un plugin de comunidad. Lo más plausible es que
Claude Code se lance desde ahí, dentro del propio vault. Es la única huella de terminal en todo el
webinar, y es un icono de 20 píxeles que nadie menciona.

---

## 3. El grafo: recuento real de nodos y qué significa cada cosa

He contado los nodos **programáticamente** sobre el frame `0032` (el zoom-out limpio), con detección
de componentes conexos + erosión morfológica para descartar aristas y etiquetas, y clasificación por
tono HSV. Resultado reproducible:

| Color | Nodos detectados | Interpretación |
|---|---|---|
| Turquesa | **26** | hub `msp-performance` + **25** agencias |
| Verde lima | **14** | hub `duzi-performance` + **13** agencias |
| Morado | **13** | hub `duzi-marka` + **12** agencias |
| Naranja | **10** | hub `msp-marka` + **9** agencias |
| Blanco | **1** | `mmponline` — sin segmento asignado |
| **Total "brillante"** | **64** | = 4 hubs + 59 agencias + 1 huérfano |
| Grises | ~55–60 | notas `sources` (una `xxx-pl` / `xxx-com` por agencia) + un puñado de `concepts` |
| **Total visible** | **~120** | |

Los 25 / 13 / 12 / 9 **encajan exactamente** con los rótulos del artefacto
(25 + 13 + 12 + 9 = **59** agencias). Esto confirma que las cuatro carpetas de `segments` y los
cuatro clústeres de color son la misma cosa, y que el mapeo es:

| Carpeta `segments/` | Color en el grafo | Etiqueta comercial del artefacto | N |
|---|---|---|---|
| `msp-performance` | turquesa | **Leady dla małych firm** (leads para pymes) | 25 |
| `duzi-performance` | verde lima | **Wyniki dla dużych marek** (resultados para grandes marcas) | 13 |
| `duzi-marka` | morado | **Kampanie dużych marek** (campañas de grandes marcas) | 12 |
| `msp-marka` | naranja | **Marka małych firm** (marca de pymes) | 9 |

### Topología: el "cerebro" es una taxonomía de dos niveles

Ampliando ×4 el frame `0036` se ven las puntas de flecha. La estructura dominante es:

```
   xxx-pl (gris, fuente)  ←──  xxx (color, agencia)  ──→  hub de segmento (color, gordo)
                                    │
                                    └──→  algún concepto (gris)  y algún enlace agencia↔agencia
```

Sobre los cuatro hubs convergen decenas de flechas entrantes; ése es todo el efecto "cerebro". Hay
**algunos** enlaces agencia↔agencia y agencia→concepto, pero son minoría frente a los
agencia→segmento y agencia→fuente. Es decir: lo que en voz se vende como *"el modelo ve conexiones
entre datos que tú no verías"* es, en la imagen, mayoritariamente **una clasificación en 4 cajones
más un enlace a la fuente**. Un `GROUP BY` renderizado con física de muelles.

Y el propio panel lateral lo delata: `Filtry / Grupy / Wyświetlanie / Siły` es el panel de ajustes
del Graph View de Obsidian. **"Grupy" es la función de colorear nodos por consulta, y se configura a
mano.** El LLM generó las notas y los `[[enlaces]]`; los cuatro colores bonitos que hacen que "los
clústeres salgan solos" son una preferencia de visualización que puso un humano. La frase *"model
językowy sam sobie tworzy te klastry"* ("el modelo se crea los clústeres solo") es cierta en cuanto
a la clasificación, y engañosa en cuanto a lo que el espectador está viendo.

### Dos anomalías que nadie caza en directo

1. **Existe un nodo llamado `%s`** (visible arriba a la izquierda en `0036`, ampliación ×3). `%s` es
   un marcador de formato de cadena. Es, con casi total seguridad, **un fichero basura generado por
   una plantilla que falló**. Lleva ahí durante toda la demo.
2. **`mmponline` es el único nodo blanco**, sin color de segmento, colgando en la periferia con dos
   aristas. Ola dice en voz *"zebrałam listę 60 agencji"* ("recopilé 60 agencias") y el artefacto
   dice **59** por todas partes. **60 − 59 = 1.** La hipótesis más económica es que `mmponline` es la
   agencia que el agente nunca clasificó, y que el artefacto la descartó en silencio. No es un error
   grave; es exactamente el tipo de cosa que el "humano supervisor" del que habla la slide 19 debería
   detectar — y en 17 minutos de demo, no se detecta.

---

## 4. El artefacto HTML: `Rentgen rynku agencji`

Pestaña titulada **"Rentgen agencji w ciemności"** (radiografía de la agencia a oscuras); el H1 de la
página dice **`RENTGEN RYNKU AGENCJI`** (radiografía del mercado de agencias). Fichero:
`C:/Users/Lenovo/Desktop/Self-firma/artefakty/prezentacja5.html`.

### Forma general

No es un informe: es un **scrollytelling** (presentación que avanza con el scroll) sobre un fondo de
campo de estrellas oscuro con estética terminal (verde lima `#c8f000`-ish sobre negro, tipografía
monoespaciada para los metadatos, sans para los titulares).

- **Barra fija superior**: `■ RENTGEN RYNKU AGENCJI` a la izquierda; `#038 / LEADY DLA MAŁYCH FIRM`
  a la derecha (id + segmento de la agencia seleccionada).
- **Barra de progreso** de línea completa bajo la cabecera, que se llena al hacer scroll.
- **Indicador de 8 segmentos** (recortado y ampliado ×4 desde `0035` y `0037`): la página tiene
  **8 escenas**. En `0035` está activa la 1ª; en `0037`, la 6ª.

### Las 8 escenas reconstruidas

| # | Escena | Contenido visual | Titular |
|---|---|---|---|
| **1** | Constelación | 6 nodos-icono orbitando un cúmulo de partículas central | *"To jest baza wiedzy, z której wyszła cała analiza"* ("Ésta es la base de conocimiento de la que salió todo el análisis") |
| **2–5** | Los 4 clústeres de agencias | Zoom/paneo del campo de estrellas hacia cada cúmulo; rótulos de cuadrante al fondo (`MAŁE FIRMY`, `DUŻE MARKI`) | Un titular + descripción por segmento |
| **6** | Koncepty | Enjambre de ~20 puntos verdes bajo el icono `KONCEPTY` | *"Wzorce, które powtarzają się między firmami"* — subtítulo: *"Archetypy claimów, mechanizmy dowodu, jawność ceny, gwarancje, nazwane metody, edukacja jako sposób pozyskiwania klientów"* |
| **7** | Analizy | Enjambre bajo el icono `ANALIZY` (visible desenfocado a la derecha en `0037`) | Las conclusiones cruzadas |
| **8** | Dashboard | La ficha interactiva por agencia (ver abajo) | — |

**Escena 1, leída con precisión (recorte ×2 de `0035`):** seis nodos etiquetados con su conteo.

```
   ⟋ LEADY DLA MAŁYCH FIRM              ⟍  WYNIKI DLA DUŻYCH MAREK
        25 AGENCJI                              13 AGENCJI
                        ✦ (cúmulo de partículas)
  ◇ MARKA MAŁYCH FIRM                      ✳ KAMPANIE DUŻYCH MAREK
        9 AGENCJI                                12 AGENCJI

        ◔ KONCEPTY              ⊞ ANALIZY
         20 NOTATEK              8 NOTATEK
```

Cada nodo tiene su propio color: verde-agua, violeta, amarillo-lima, coral, verde y amarillo, con
halo de luz. **Los cuatro primeros son los mismos cuatro clústeres del grafo de Obsidian, repintados
con otra paleta.** Esto importa: la coherencia visual entre grafo y artefacto es cosmética, no
estructural.

### Escena 8 — el dashboard por agencia (frames `0038`, `0039`, `0040`)

Es la única pieza verdaderamente "producto" de todo el webinar. Estructura reconstruida:

```
┌───────────────────────────────────────────────────────────────────────────────────────┐
│ Kadrio   #038 · WROCŁAW · LEADY DLA MAŁYCH FIRM  │▎AI SEO i GEO · Poziom 4 z 4:        │
│                                                   │  własna technologia                 │
│                                                   │  agent treści pod odpowiedzi AI     │
│                                                   │  i monitoring botów · robi to 8     │
│                                                   │  firm z 59                          │
│                                        [ ▾ #038 Kadrio · Wrocław ★ AI SEO ]  [ LOSOWA ] │
├─────────────────────────────┬─────────────────────────────────────────────────────────┤
│ ⌂ GRUPA                     │ ((•)) DOWÓD                │  Mapa rynku                 │
│   Leady dla małych firm     │   Zasięgi kampanii         │  ┌───────────┬───────────┐  │
│   25 firm w grupie          │   tak samo 7 z 59          │  │Leady dla  │Wyniki dla │  │
│ ────────────────────────────┼────────────────────────────┤  │małych firm│dużych     │  │
│ ⌂ CENA                      │ ✦ WYRÓŻNIK                 │  │ 25        │marek  13  │  │
│   Cennik na stronie         │   AI i widoczność w AI     │  ├───────────┼───────────┤  │
│   tak samo 5 z 59           │   oraz 2 inne              │  │Marka      │Kampanie   │  │
├─────────────────────────────┬────────────────────────────┤  │małych     │dużych     │  │
│ Czym się wyróżnia           │ Co zrobić, żeby się        │  │firm    9  │marek   12 │  │
│                             │ wyróżnić                   │  └───────────┴───────────┘  │
│ LEPSZA OD RYNKU             │ 01 ⟲ Idź w głąb            │   eje Y: Chce leadów /      │
│  ✓ Mówi o cenie             │      Cena, dowód i wyróżnik│          Chce marki         │
│    Cennik na stronie,       │      są na miejscu.        │   eje X: Płaci mała firma / │
│    a 43 firmy milczą.       │      Kolejny krok to       │          Płaci duża marka   │
│  ✓ Długa lista klientów     │      wyceniony, powtarzalny│   leyenda con los 4 conteos │
│    Pokazuje 17 marek        │      program.              │   + "wybrana" (destacada)   │
│    z nazwy. Typowa          │ 02 ♛ Dołóż czwarty dowód   ├─────────────────────────────┤
│    agencja dziesięć.        │ 03 ◎ Zajmij branżę bez     │  Klienci i własne słowa     │
│                             │      gospodarza            │   MARKI NA STRONIE          │
│ SŁABSZA OD RYNKU            │      B2B SaaS, sprzedaż na │   17                        │
│  ⊘ Węższa oferta            │      marketplace'ach       │   [Fotoforma][Nakrywamy]    │
│    Sprzedaje 2 z 12         │      i employer branding   │   [Blikle][Mercedes][Benz]  │
│    kategorii usług.         │      nie mają tu jeszcze   │   [Duda][Cars][Imker]       │
│    Typowa agencja pięć.     │      właściciela.          │   ❝ „SEO na luzie"          │
├─────────────────────────────┼────────────────────────────┤   ❝ „SEO traktujemy serio,  │
│ Pozycja na tle rynku        │ Oferta wobec rynku         │     choć przy pracy aż      │
│  Szerokość oferty      2    │  Social media       32     │     cieszy nam się micha"   │
│  ▓░░░░░░  POD RYNKIEM       │  Strony i sklepy    32 ◄   │                             │
│  mediana rynku 5            │  SEO i widoczność   32 ◄   │                             │
│  Jawność ceny          3    │  Reklamy płatne     29     │                             │
│  ▓▓▓▓▓▓▓  NAD RYNKIEM       │  Wideo i foto       19     │                             │
│  mediana rynku 0            │  Automatyzacja i AI 13     │                             │
│  Znane marki na stronie 17  │  Strategia          27     │                             │
│  ▓▓▓▓▓░░  NAD RYNKIEM       │  Content            29     │                             │
│  mediana rynku 10           │  Kampanie i eventy  31     │                             │
│                             │  Analityka          15     │                             │
│                             │  Branding           16     │                             │
│                             │  PR i influencerzy  11     │                             │
└─────────────────────────────┴────────────────────────────┴─────────────────────────────┘
```

**Métricas que muestra realmente:**
- 4 tarjetas-resumen: **grupo**, **prueba social** (`Zasięgi kampanii`, "igual que 7 de 59"),
  **precio** (`Cennik na stronie`, "igual que 5 de 59"), **diferenciador** (`AI i widoczność w AI`,
  "y 2 más").
- Etiqueta de nivel en la cabecera: `Poziom 4 z 4: własna technologia` — una escala de madurez 1–4.
- 3 barras de posición con **mediana del mercado** como referencia (2 vs 5 · 3 vs 0 · 17 vs 10) y
  veredicto `POD RYNKIEM` / `NAD RYNKIEM`.
- Un **mapa 2×2** `Chce leadów↔Chce marki` × `Płaci mała firma↔Płaci duża marka`, con las 59 agencias
  como puntos y la seleccionada resaltada con anillo.
- 12 categorías de oferta con conteo absoluto sobre 59, y las de la agencia resaltadas.
- Recuento y lista de marcas-cliente nombradas en la web + citas literales de la propia web.
- Un selector desplegable con las 59 agencias y un botón **`LOSOWA`** (aleatoria).

**Es un producto de datos de verdad**, no una maqueta: cruza cada agencia contra medianas del
conjunto y contra conteos absolutos coherentes. Eso hay que reconocerlo.

**Pero el "mapa de mercado" no mapea nada.** Cada cuadrante *es* uno de los cuatro segmentos, así
que la posición de un punto no aporta información nueva sobre la que ya da su etiqueta de clúster;
dentro de cada cuadrante los puntos se apelotonan en dos o tres bandas verticales. Es una leyenda
disfrazada de scatter plot. La voz lo vende como *"mapa pozycjonowania"*.

---

## 5. Lo que se enseña de la *construcción* del sistema: exactamente una diapositiva

Todo el "cómo se hace" está en el frame `0027` (00:26:15), deck slide 13/22 — **un dibujo, no una
pantalla**:

```
01 / WEJŚCIA              03 / NARZĘDZIA                   02 / DECYZJE
Strony i cenniki    →     Claude + skill            →      Dane starsze niż 30 dni?
8 konkurentów             Notion · Airtable · Firecrawl     └─ TAK → POBIERZ ŚWIEŻE ──┐
                                       ↑                                              │
                                       └──────────────────────────────────────────────┘
04 / REZULTAT · LLM BRAIN                          NA TEJ PODSTAWIE
[miniatura del grafo]  Baza danych                 [miniatura del dashboard]
                       pamięć dla modelu           Analiza z wnioskami
                       tabela konkurentów,
                       zmiany w czasie,
                       format karty
```

Esto es **todo**. Nunca se ve:
- el fichero `CLAUDE.md` abierto (ni una línea);
- el *skill* del que se habla durante todo el webinar (ni su nombre de fichero);
- un prompt escrito por un humano;
- Claude Code ejecutándose, ni su salida, ni un plan, ni una llamada a herramienta;
- Firecrawl, Notion o Airtable (se nombran, no se abren);
- **ni una sola nota del vault abierta.** Ola dice literalmente *"możemy sobie wejść w jakąś konkretną
  agencję i tutaj tagami będzie oznaczona…"* ("podemos entrar en una agencia concreta y estará
  etiquetada con tags…") — y **no entra**. El grafo nunca se convierte en un fichero.

---

## 6. Honestidad: ¿respalda lo que se ve la afirmación "esto lo monta alguien sin conocimientos técnicos"?

La afirmación literal, en la slide 14/22 (frame `0028`), es:
> *"Wygląda na skomplikowane, a złoży go też osoba pracująca na kasie, z zawodem zupełnie spoza
> biznesu. Programowanie nie jest tu potrzebne."*
> ("Parece complicado, pero también lo montaría alguien que trabaja en una caja registradora, con
> una profesión totalmente ajena al mundo empresarial. Aquí no hace falta programar.")

Mi lectura, con lo que hay en pantalla: **la afirmación es literalmente cierta y prácticamente
engañosa.** Argumentos, todos apoyados en frames concretos:

**A favor de la afirmación (hay que ser justos):**
1. En pantalla no aparece ni una línea de código escrita a mano. Cierto.
2. Todo lo visible son piezas de consumo: Obsidian gratuito, Chrome, ficheros locales. Ninguna
   infraestructura, ningún despliegue, ninguna base de datos que administrar.
3. Ola es honesta en tres momentos que un vendedor puro habría cortado: dice que Obsidian se eligió
   *"dlatego, że to rozwiązanie jest darmowe"* (porque es gratis) y para "ilustrar el concepto";
   admite que el LLM no hace el grafo solo (*"trzeba dostarczyć LLM-owi dobrze opisany sposób i
   kontekst"*); y en el bloque de oferta dice explícitamente que **no** enseñarán a construir apps
   para vender porque *"jest to zarezerwany temat dla inżynierów"* y que *"nie mydlimy wam tu oczu"*
   ("no os estamos echando arena a los ojos").

**En contra, y pesa más:**

4. **La propia slide 22/22 desmiente la 14/22.** Frame `0046`: una rejilla de **15×5 = 75 casillas**,
   de las que solo las **3 últimas** están encendidas en verde, junto al titular *"Widzisz wynik.
   Za nim stoi kilkadziesiąt podejść."* ("Ves el resultado. Detrás hay decenas de intentos."). El
   propio deck cuantifica 72 intentos fallidos por 3 buenos. Eso no es "una cajera lo monta"; eso es
   el perfil de esfuerzo de un especialista iterando.
5. **Los nombres de fichero son el registro de esas iteraciones y están a la vista todo el rato.**
   El deck es `prezentacja-system-ai-v21.html` — **v21**. El artefacto es `prezentacja5.html` — **la
   quinta**. La barra de direcciones de Chrome, visible en 20 frames, lleva el contador de intentos
   escrito.
6. **El artefacto es software.** Un scrollytelling con campo de estrellas animado, transiciones por
   scroll, indicador de 8 escenas, scatter de 59 puntos, selector con 59 entradas y botón aleatorio,
   barras normalizadas contra medianas. Eso son miles de líneas de HTML/CSS/JS. Que las escriba
   Claude no elimina el conocimiento técnico: lo desplaza. Convierte al usuario en alguien que tiene
   que **revisar** algo que no sabe leer. Y la slide 19/22 (`Ocena jakości wyniku`) le asigna
   justamente ese trabajo: *"Test na znanym przypadku — puszczasz zadanie, którego wynik znasz, i
   porównujesz różnice"*. Una cajera no tiene un caso conocido contra el que contrastar 59 fichas.
7. **La cadena de herramientas no visible es la parte técnica.** Firecrawl (API de pago con clave),
   conectores MCP a Notion/Airtable, Claude Code (que se instala y se lanza desde una terminal — y el
   único indicio en pantalla es un icono `>_` en un plugin de comunidad de Obsidian), y un
   `CLAUDE.md` en la raíz del vault que gobierna todo el comportamiento del agente. Nada de eso se
   demuestra. Se dibuja en una caja de la slide 13/22 y se sigue adelante.
8. **La propia web rebaja la promesa.** `aioperators.pl` dice, en la ruta *no técnica*:
   *"Zmapujesz własny rynek, **3-5 konkurentów** i źródła, którym można zaufać"*. Tres a cinco
   competidores. La demo enseña sesenta. Es una diferencia de dos órdenes de magnitud entre lo que
   se exhibe y lo que se vende. Y la lista de herramientas del programa incluye **Git y API**.
9. **Los errores que quedan en pantalla son la prueba de que hace falta criterio técnico.** El nodo
   `%s`, el nodo blanco `mmponline` sin clasificar, el desfase 60 (voz) / 59 (artefacto) /
   "8 konkurentów" (slide 13), y una incoherencia aritmética dentro del propio dashboard:
   `Cennik na stronie — tak samo 5 z 59` frente a `Mówi o cenie — Cennik na stronie, a 43 firmy
   milczą` (5 + 43 = 48, no 59; faltan 11 empresas por explicar). Ninguna de esas cuatro cosas se
   detecta en directo. Son exactamente las que tendría que cazar el "supervisor humano" que el propio
   webinar dice que eres.
10. **El caso elegido es el más fácil que existe.** Webs públicas de agencias de marketing: texto
    homogéneo, sin permisos, sin datos sensibles, sin conflictos de versión, sin ambigüedad
    semántica. El curso promete aplicar el mismo método a *"dokumenty, decyzje i procedury firmy"*,
    que es un problema cualitativamente distinto (autoridad de la fuente, caducidad, contradicciones).
    La demo no toca ese problema en ningún momento.
11. **La demo es de solo lectura.** Nunca se añade un fichero, nunca se relanza el agente, nunca se
    ve el grafo actualizarse. Cuando Ola explica que si añadiese una empresa el agente recorrería
    todo el vault y crearía enlaces nuevos, está describiendo un futuro condicional
    (*"gdybym dorzuciła… agent zacząłby…"*) sobre una pantalla estática. Es la afirmación de mayor
    valor comercial del bloque y es la única que no se demuestra.

**Veredicto.** Lo que se ve en pantalla demuestra que **el resultado es real**: 59 fichas, medianas
calculadas, trazabilidad a las fuentes, un artefacto interactivo funcional. Lo que **no** demuestra
en absoluto es la afirmación sobre quién puede montarlo. La demo enseña el *output* y esconde el
*proceso* — y el propio deck, en su última diapositiva, admite que el proceso fueron 72 intentos
fallidos. La frase honesta sería: *"esto no requiere escribir código, pero sí requiere pensar como
alguien que diseña sistemas de datos, y a mí me costó decenas de iteraciones"*. Ola casi la dice.
El titular de la slide 14 dice otra cosa.

---

## 7. Anexo: detalles pequeños que sirven de evidencia

- **`0033` (00:35:00)** captura por accidente el **preview de Alt-Tab de Chrome**, con las miniaturas
  de las dos pestañas. Confirma que no hay más ventanas escondidas: el escritorio entero durante la
  demo son dos HTML locales + Obsidian + StreamYard.
- **`0031` (00:29:39)** es el único frame con las **dos cámaras** (Damian y Ola). Coincide con
  *"¿se ve bien Obsidian?"*. El cambio a la herramienta real es también el único momento en que hace
  falta coordinación técnica en directo, y hay un pequeño tropiezo (*"może Shift, Ctrl+, o lepiej"*).
- **`0038` vs `0040`**: la misma pantalla con 2:33 de diferencia y la barra de progreso superior en
  distinta posición. Confirma que la escena 8 es larga y que Ola la recorre con scroll, no con clics.
- El botón **`LOSOWA`** ("aleatoria") junto al selector de agencia es un detalle de diseño de demo:
  está pensado para que en directo cualquiera pueda pedir "enséñame otra" y la ficha se rellene. Es
  el gesto que probaría que el sistema es general — y **no se usa**.
- Las citas del bloque `Klienci i własne słowa` son texto literal raspado de la web de la agencia
  (*„SEO na luzie"*, *„SEO traktujemy serio, choć przy pracy aż cieszy nam się micha"*). Es la prueba
  más convincente de todo el artefacto de que los datos son reales: nadie inventa esas frases.
- Precio del programa (web, no frames): **995 zł netos / 1.223,85 zł brutos**, preventa hasta el 2 de
  septiembre, inicio 26 de octubre, 7 días de garantía. El webinar dura 117 minutos, de los cuales
  ~17 son producto y ~55 son oferta y cierre.
