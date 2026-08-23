# Transcripción — LIVE: Jak zbudować system AI, który zna Twoją pracę i przejmuje jej powtarzalną część


**[00:00:25]** Dobry wieczór Państwu, witamy serdecznie na szkoleniu jak zbudować system AI, który zna Twoją pracę i przejmuje jej powtarzalną część.

**[00:00:38]** Ja nazywam się Damian Naprawa i ze mną jest Ola Zajączkowska i mam nadzieję, że razem dzisiaj spędzimy najbliższe 90 minut i że zostaniecie z nami do końca,

**[00:00:50]** ponieważ przygotowaliśmy dla Was specjalne bonusy, no i oczywiście Ola przygotowała kawał merytorycznej wiedzy.

**[00:00:58]** Zatem powoli będziemy sobie zaczynać, wiem, że część osób dołączy jeszcze w trakcie, ale w międzyczasie zrobimy sobie wprowadzenie.

**[00:01:10]** To szkolenie kierujemy do dwóch grup osób, tak naprawdę. Do osób, które dopiero zaczynają z AI i chcą zrozumieć fundamenty, zobaczyć gdzie AI może usprawniać,

**[00:01:21]** jak zbudować pracę, ale także do osób, które już używają AI i chciałyby się czegoś konkretnego nauczyć, czyli to co w tytule jak budować system AI, który rozumie Twoją pracę.

**[00:01:32]** I będzie konkretne demo, za chwilę tutaj oddam Oli głos, która zaprezentuje Wam ciekawe rozwiązanie, które obecnie jest na topie, można by powiedzieć.

**[00:01:43]** Ale zanim jeszcze to zrobimy, to chcę jeszcze porozmawiać o takim czymś, co spotykam na co dzień.

**[00:01:51]** Część osób używa AI jako tylko takiej szybkiej wyszukiwarki, lepszej wyszukiwarki niż Google, piszą coś do tego czata, czy do innego Gemini'a, kopiują, uzyskują jakąś odpowiedź.

**[00:02:06]** Natomiast możliwości dzisiaj są znacznie większe i jeśli pomyśleliście, że jest to kolejny webinar o promptach, albo że pokażą nam znowu jakieś narzędzia, które za miesiąc się zmienią,

**[00:02:21]** albo pokażą coś, co w ogóle nie będzie przydatne w Waszej pracy, to chcemy Was uspokoić, dzisiaj tego nie będzie.

**[00:02:30]** Pokażemy dzisiaj konkrety, jak można budować taki system w różnych dziedzinach.

**[00:02:36]** I on będzie na tyle uniwersalny, że śmiało mogę powiedzieć, iż możecie go wykorzystać w bardzo różnych branżach.

**[00:02:45]** Więc nie będziemy dawać Wam ani 50 magicznych promptów, ani pokazywać jak tworzyć aplikacje.

**[00:02:53]** Ani nie pokażemy Wam jednego tricku, ani nie opowiemy Wam o trzech magicznych sekretach, jak to na webinarach ostatnio często widzę, jakieś trzy magiczne sekrety.

**[00:03:04]** Nie, nie, tutaj tego nie będzie, będzie konkret.

**[00:03:07]** Więc moi drodzy, nie będzie tego, ponieważ przewaga nie leży w jednym promptcie, tylko tak naprawdę praca z AI zaczyna się od dobrze ustawionego kontekstu, który jest zasilony wiedzą, narzędziami i odpowiednimi zasadami.

**[00:03:21]** I na to się składa system.

**[00:03:22]** To oczywiście w bardzo wielkim skrócie.

**[00:03:25]** Nie spytałem na początku, czy nas dobrze widać, czy nas słychać, po prostu wyleciało mi to z głowy, ale na czacie widzę, że nie ma komentarzy, nie słychać, także lecę dalej.

**[00:03:39]** Będziemy budować sobie tzw. LLM Second Brain, gdzie AI rozumie Wasz kontekst, firmy, dokumenty, decyzje, procesy i właśnie Ola to za chwilę zaprezentuje.

**[00:03:51]** I my dzisiaj z Olą widzimy taką nową kompetencję w firmach.

**[00:03:55]** Którą nazwaliśmy AI Operatorem.

**[00:03:59]** I jest to właśnie taka osoba, która potrafi zaprojektować taki system, jaki dzisiaj pokażemy za chwilę i o którym zrobiliśmy małe wprowadzenie.

**[00:04:09]** Więc jeśli jesteś osobą nietechniczną, to spokojnie dzisiaj będziemy mówić w taki sposób, aby rozumieli nas także nietechniczni.

**[00:04:21]** Czyli jeżeli pracujesz poza branżą IT.

**[00:04:23]** Nie masz na co dzień styczności z programowaniem, to spokojnie dzisiaj to szkolenie także jest dla Ciebie.

**[00:04:30]** Ale uwaga, jeśli jesteś z branży IT, wiem, że tutaj sporo takich osób mamy i pozdrawiam wszystkich naszych stałych klientów i obserwujących.

**[00:04:38]** To też wyniesiesz z tego całkiem sporo wiedzy, bo możesz dzięki temu rozwiązaniu, które pokaże Ola za chwilę, projektować swoje narzędzia, integracje i wdrażać takie dodatkowe narzędzia,

**[00:04:51]** które usprawniają pracę w firmie.

**[00:04:52]** Pracę Twojego zespołu lub Twoją.

**[00:04:56]** Więc dlaczego mielibyście nas dzisiaj słuchać?

**[00:05:00]** To może wreszcie teraz oddam głos Oli, bo jeszcze nie dopuściłem jej do słowa.

**[00:05:04]** Tak, dobrze mnie słychać?

**[00:05:06]** Tak, tak.

**[00:05:09]** Super, super. Witam Was wszystkich. Cieszę się, że możemy dla Was poprowadzić ten webinar.

**[00:05:14]** Ja się też krótko przedstawię. Mam na imię Ola Zajączkowska i jestem inżynier z ponad 7-letnim doświadczeniem.

**[00:05:22]** Przeszłam całą tą drogę, żeby wejść właśnie do branży AI i teraz staram się przekazać takie smaczki z wszystkich lat doświadczenia, jak pracowałam w wdrażaniu systemów AI przy różnych branżach.

**[00:05:38]** Także dzisiaj opowiem Wam właśnie, jak LLM Brain może nam pomóc ustawiać kontekst, jak możemy z tym rozwiązaniem budować system,

**[00:05:50]** który jest taką, wiecie, aplikacją, która daje nam bardzo dużo wniosków i po prostu nie mogę się doczekać, że Wam pokażę za chwilę całą część merytoryczną.

**[00:06:02]** Dzięki Ola. To dwa zdania ode mnie. Jestem Damian. Zajmowałem się projektowaniem systemów IT. Od jakiegoś czasu także rozwijam swoje aplikacje i prowadzę też inne biznesy i jestem naprawdę heavy użytkownikiem AI.

**[00:06:20]** Myślę, że spędzam z AI po kilka godzin dziennie albo może nawet i całą moją pracę w ciągu dnia. Jeśli pracuję przy komputerze, to jest to praca z AI z różnych perspektyw.

**[00:06:34]** Od programowania, po tworzenie treści, materiałów marketingowych. No de facto, co tylko się da dzisiaj z AI zrobić, to dotykam tego, więc dzisiaj też większość tematów będzie omawiać Ola,

**[00:06:47]** ale jeśli będziecie mieli do mnie jakieś pytania, to też chętnie na nie odpowiem.

**[00:06:51]** Więc to są nasze jakby statsy, jeśli chodzi o to, dlaczego mielibyście z nami zostać do końca. Ja tylko dodam, że jeżeli ktoś jest pierwszy raz na tym szkoleniu i nie kojarzy nas,

**[00:07:06]** to w naszych szkoleniach ogólnie tutaj pod marką w kontenerach, którą reprezentuję brało udział, no myślę, że grubo ponad 20-30 tysięcy w tych darmowych i jakieś 5 tysięcy w takich szkoleniach,

**[00:07:20]** powiedzmy pełnopłatnych.

**[00:07:22]** Pełnometrażowych. Więc zostańcie z nami dzisiaj do końca, będziemy mieli też dla was specjalny prezent, który myślę, że wam się spodoba.

**[00:07:32]** Więc jak będziecie podchodzić do budowania takich systemów, to trzeba sobie zadać trzy pytania.

**[00:07:38]** Co AI musi wiedzieć o waszej firmie, o waszej pracy? Skąd wie, którym źródłom ufać i gdzie człowiek zachowuje kontrolę? Gdzie człowiek powinien zatwierdzać rzeczy?

**[00:07:48]** I teraz obiecany prezent, który mamy dla was, dla osób, które będą z nami na żywo, będzie to takie szkolenie, poradnik, jak zbudować stronę internetową z AI w 4 wieczory,

**[00:08:01]** czyli nie w godzinę, nie w minutę, tylko w 4 wieczory, usiąść do tego konkretnie i spokojnie i jak opublikować tę stronę w internecie.

**[00:08:10]** Ale jeszcze, żeby to nie było wszystko, to mam dla was też, ponieważ ja dużo sprzedaję różnych rozwiązań,

**[00:08:16]** aplikacji i tak dalej, to mam pewne doświadczenie jak szukać klientów, jak znaleźć pierwszego klienta i zaproponować taką stronę w takim podejściu trochę side hustle,

**[00:08:30]** ale bez żadnego naciągania i bez żadnego hype'u, więc ten poradnik będzie dla was, którzy zostaną z nami dzisiaj na żywo.

**[00:08:40]** Także warto zostać do końca.

**[00:08:43]** Tyle z mojej strony.

**[00:08:44]** Oddaję głos do Oli, która wam pokaże to wszystko, co wcześniej zapowiedzieliśmy.

**[00:08:51]** Tak, tak, teraz proszę cię o przekazanie ekranu i ja nie będę was widzieć na chwilę,

**[00:08:57]** ale myślę, że już możesz włączyć ekran i powiedzieć mi, czy dobrze widać prezentację, jak zbudować system AI.

**[00:09:06]** Tak jest, już prezentacja jest widoczna.

**[00:09:09]** Widać? Ok, super.

**[00:09:11]** Dzisiaj jestem tutaj po to, razem z Damianem, żeby powiedzieć wam właśnie,

**[00:09:14]** jak zbudować system AI, który zna waszą pracę i jest w stanie przejąć jej powtarzalną część.

**[00:09:21]** I to jest też sposób, który ja widzę, że może wyróżnić bardzo wiele osób na rynku pracy.

**[00:09:29]** Ale żeby pokazać wam, jak to zrobić, muszę wspomnieć o pięciu krokach,

**[00:09:34]** które są kluczowe właśnie, żeby się wyróżnić na rynku i żeby wykonać ten system.

**[00:09:38]** I te pięć kroków możecie kojarzyć z opisu webinaru.

**[00:09:42]** Bardzo chcę wam powiedzieć o tym, dlaczego na samym początku musicie wiedzieć, co to jest model,

**[00:09:49]** automatyzacja i agent, jaka jest różnica pomiędzy tym,

**[00:09:53]** jak mamy opisywać zadania, nasze zadania, które oddajemy AI do pracy,

**[00:10:00]** co to jest kontekst i jak możemy z nim pracować, jak możemy opisywać kontekst

**[00:10:06]** i jak operować wiedzą, którą mamy, czy to jest wiedza naszej firmy, czy projektu,

**[00:10:10]** dlaczego ważny jest dostęp do narzędzi i dlaczego ważna jest ocena jakości wyniku z AI.

**[00:10:18]** I dlaczego w ogóle te pięć kroków?

**[00:10:22]** Dlatego, że te pięć kroków szuka rynek.

**[00:10:26]** Razem z Damianem mieliśmy bardzo dużo rozkmin i to jest coś, co ja też widzę

**[00:10:31]** przez ostatnie 8 miesięcy 2026 roku, przez cały rok to obserwuję, jak zmienia się rynek.

**[00:10:37]** Miałam masę konsultacji i widzę,

**[00:10:41]** jeden trend, że rynek obecnie poszukuje ludzi, którzy potrafią płynnie działać w narzędziach AI.

**[00:10:50]** I to się właśnie mapuje do pierwszego kroku, czyli osoba, która potrafi zobaczyć na dany problem,

**[00:10:57]** dane zagadnienie i zastanowić się, jak może je rozwiązać, czy modelem językowym,

**[00:11:02]** czy automatyzacją, czy może jakimś agentem, to jest właśnie osoba, która jest płynna w narzędziach AI.

**[00:11:06]** I od tego zaczniemy.

**[00:11:07]** Potem powiem Wam coś o myśleniu systemami, o takim systemowym myśleniu,

**[00:11:14]** czyli jak już jesteśmy płynni w tych narzędziach AI, to jak możemy zmienić powtarzalny proces w automatyzację.

**[00:11:21]** I do tego są ważne, ważna jest ta umiejętność, ten skill opisania naszego zadania, które oddajemy AI.

**[00:11:28]** Później, jeśli chodzi o kontekst i wiedzę firmy, to oczywiście rynek szuka ludzi,

**[00:11:34]** którzy potrafią spojrzeć na dane firmy, na 10 projektów, na jakich pracowaliśmy,

**[00:11:42]** na wewnętrzne narzędzia, wyciągnąć z nich tą masę nieustrukturyzowanych danych i wyciągnąć z nich wnioski.

**[00:11:48]** I to, słuchajcie, zmienia się bardzo płynnie w taką zdolność prototypowania,

**[00:11:55]** gdzie my mamy jakiś pomysł, że o, tutaj mamy masę projektów i danych z nich

**[00:12:02]** i fajnie by było wyciągnąć z tego jakieś wnioski.

**[00:12:05]** Ale jak wyciągnąć te wnioski? No musimy zbudować system, z którego będziemy mogli czerpać tą wiedzę

**[00:12:10]** i na przykład usprawnić jakiś proces albo zautomatyzować coś, albo zrobić research, wyciągnąć informacje.

**[00:12:17]** I po to musimy mieć zdolność prototypowania, czyli takiego zamieniania pomysłów w działające demo,

**[00:12:22]** żeby wyciągnąć z tego wartość biznesową.

**[00:12:25]** No i oczywiście w tym całym procesie potrzebna jest też ocena jakości wyniku, czyli jak ocenić ten wynik

**[00:12:31]** i czy on faktycznie, realnie rozwiązuje problem biznesowy i czy daje nam wartość.

**[00:12:36]** Bo to, co ja Wam teraz pokażę, to jest rozwiązanie, które jest techniczne.

**[00:12:40]** Ale po tylu latach pracy w branży to, co zawsze staram się przekazywać, to jest to, że fajnie jest mieć tą wiedzę techniczną,

**[00:12:48]** ale i tak finalnie my budujemy rozwiązanie, które ma dać jakąś wartość biznesową i faktycznie rozwiązać jakiś problem,

**[00:12:54]** więc po to się ewaluuje te wyniki, bo to jest tak naprawdę najważniejsza część tego procesu.

**[00:12:58]** I to, co Wam teraz wymieniłam, to jest akurat bardzo ciekawy fakt, faktyczny opis pozycji,

**[00:13:07]** która nazywa się często AI Product Builderem, bardzo często też AI Operatorem.

**[00:13:13]** Tutaj nie chcę, żebyście się przywiązywali do nazwy, bo rynek zmienia się tak dynamicznie,

**[00:13:17]** a każda firma w zależności od potrzeb nazywa to trochę inaczej, więc dlatego to się może pojawiać też czasami pod nazwą Solution Engineer.

**[00:13:24]** I właśnie te wszystkie kroki dokładnie opisują to, czego firmy szukają,

**[00:13:28]** bo naprawdę potrzebują osób, które będą potrafiły cały ten proces przejść płynnie.

**[00:13:35]** I to jest coś, co chcę Wam teraz pokazać.

**[00:13:38]** I tutaj też chcę wspomnieć o tym, że każdy z tych kroków obecnie jesteśmy w stanie wykonać bez programowania.

**[00:13:48]** Bariera wejścia do AI na obecną chwilę, jak sami wiecie, jest bardzo niska.

**[00:13:55]** Ja to mówię z perspektywy 8 lat w tej branży, kiedyś była bardzo wysoka

**[00:13:59]** i naprawdę jakby bez programowania nie dało się pracować z AI.

**[00:14:03]** Teraz tak nie jest, więc wszystko, co Wam tutaj pokażę, da się zrobić pracując z modelami językowymi, tylko językiem naturalnym.

**[00:14:10]** Więc to jest też ciekawy aspekt, że zdecydowanie jakby ten proces, który Wam pokażę jest dla też osób, które potencjalnie są początkujące.

**[00:14:21]** I na początku chcę zacząć od podstaw, po co my w ogóle tego potrzebujemy.

**[00:14:26]** I dlatego przejdziemy sobie do punktu pierwszego,

**[00:14:28]** czyli do płynności w narzędziach AI.

**[00:14:32]** Na samym początku, jak macie jakiś proces w pracy, to musicie wiedzieć, jak możemy rozwiązać dany problem.

**[00:14:42]** Czego możemy użyć? Czy modelu, czy automatyzacji, czy agenta?

**[00:14:46]** I jak możemy w ogóle do tego podejść?

**[00:14:48]** Tutaj teraz dam Wam taki szybki tip, to będzie taki booster, który możecie od razu sobie wykorzystać nawet gdzieś tam w pracy,

**[00:14:56]** czy jak zastanawiacie się nad jakimś swoim rozwiązaniem.

**[00:14:58]** I to jest taki schemat myślowy, który może Was na samym początku, jak myślicie high levelowo, wysokopoziomowo o problemie, który musicie rozwiązać,

**[00:15:08]** doprowadzić do tego, jakiego Wy potrzebujecie rozwiązania, żeby się za to zabrać.

**[00:15:12]** Mamy dane zadanie w pracy i najpierw się zastanawiamy, czy ono ma określone, powtarzalne kroki.

**[00:15:17]** Jeśli tak, to bardzo możliwe, że rozwiązaniem tego problemu w ogóle nie będzie AI, tylko automatyzacja.

**[00:15:26]** I co ja mam tutaj na myśli, jeśli chodzi o określone, powtarzalne kroki?

**[00:15:32]** No na przykład, że macie fakturę, musicie zeskanować dane z tej faktury, przenieść je do jakiegoś Excela i coś obliczyć i za każdym razem to wygląda tak samo.

**[00:15:40]** I nie ma tutaj po prostu żadnej dozy krytycznego myślenia, to jest można by powiedzieć prosty algorytm, można by to krokami rozpisać zawsze identycznie.

**[00:15:48]** W takich sytuacjach bardzo często nie potrzebujecie w ogóle AI, tylko prawdopodobnie rozwiąże to jakaś automatyzacja.

**[00:15:54]** Ale z drugiej strony bardzo często, kiedy takie właśnie Wasze zadanie nie ma określonych, powtarzalnych kroków, to możliwe, że wtedy model językowy będzie dobrym rozwiązaniem.

**[00:16:04]** I mówię tutaj możliwe, bo oczywiście ten schemat jest pomocniczy, ale wiadomo, że jakiś przypadek, nad którym pracujecie, może mieć mnóstwo niuansów, więc czasami to nie jest takie, wiecie, zero-jedynkowe.

**[00:16:13]** Ale fajnie się tym schematem posługiwać, bo on bardzo dużo ułatwia na początku.

**[00:16:17]** Jeśli chodzi o modele językowe, to mamy dwie opcje.

**[00:16:21]** Mamy opcję A, czyli po prostu używamy go w okienku czasu.

**[00:16:24]** Możecie sobie to wyobrazić w ten sposób, że macie na przykład, wchodzicie na stronę czata GPT, na stronę Claude'a i macie tego właśnie czata jako taką wyszukiwarkę, trochę bardziej fancy, skomplikowaną i w ten sposób możecie go używać.

**[00:16:40]** I to jest w ogóle pierwszy poziom używania modeli językowych, żeby rozwiązać jakiś problem.

**[00:16:44]** Można to robić na pytania i na burzę mózgów.

**[00:16:46]** I większość osób się na tym poziomie zatrzymuje.

**[00:16:49]** A możemy pójść o wiele poziomów dalej i użyć agenta.

**[00:16:52]** I agent oczywiście to jest już coś takiego jak na przykład kod, kod albo kodeks.

**[00:16:58]** Będziemy o tym mówić za chwilę trochę więcej.

**[00:17:00]** I to już jest ten wyższy poziom pracy z AI, pracy z modelami językowymi, gdzie możemy wpuścić takiego agenta już nie tylko do zadawania mu pytań i odpowiedzi, do jakiegoś szybkiego pisania maili, tylko użyć go do procesu, który jest złożony, wieloetapowy i często wymaga jakiegoś krytycznego myślenia.

**[00:17:20]** I ja bym powiedziała, że ta płynność w narzędziach AI, bycie takim płynnym właśnie w używaniu modeli językowych, to jest właśnie ta umiejętność tego, że Ty jako taki użytkownik wspierany przez AI wiesz, kiedy użyć modelu językowego, w jakiej formie, bo też nie do wszystkiego agent jest dobry.

**[00:17:43]** Czasami po prostu wystarczy, że rozwiążesz problem zwykłym zapytaniem do LLM-u, zwykłym zapytaniem do kloda.

**[00:17:50]** Ale w ogóle AI nie potrzebujesz i musisz użyć automatyzacji.

**[00:17:54]** To jest krok numer jeden.

**[00:17:57]** I teraz pójdźmy jeszcze troszeczkę więcej, troszeczkę głębiej w podstawy, żeby wyrównać poziom, bo wiem, że bardzo możliwe, że mam tutaj dużo osób, dla których to jest totalnie temat od zera.

**[00:18:11]** Więc chcę troszeczkę wyrównać poziom i powiedzieć Wam jeszcze parę słów więcej o tych trzech rozwiązaniach.

**[00:18:17]** Właśnie jak używamy czata w wyszukiwaniu.

**[00:18:21]** W wyszukiwarce to to jest zazwyczaj takie zadawanie pytań i odpowiadanie jednokierunkowe, czyli mamy pytanie, odpowiedź, pytanie, odpowiedź.

**[00:18:29]** I tutaj przychodzimy z prostymi tematami.

**[00:18:32]** Jak wybieramy automatyzację z drugiej strony, to mamy określone kroki, czyli tak jak mówiłam, ta sama ścieżka za każdym razem.

**[00:18:41]** I tutaj użyjemy takich programów jak AnyTen i Make.

**[00:18:44]** Pokazuję Wam też tą mapę tych trzech różnych poziomów, żeby też zarysować Wam jakie mamy normy.

**[00:18:51]** Narzędzia tutaj, czyli zaznaczyłam właśnie w czacie, że to będą proste zapytania do modeli językowych.

**[00:18:59]** W automatyzacjach to będzie AnyTen lub Make, najbardziej popularne narzędzia do automatyzacji.

**[00:19:04]** A w złożonych procesach, i czym jest złożony proces?

**[00:19:07]** Złożony proces to będzie taki, gdzie mamy dany cel, gdzie musimy dojść do jakiegoś określonego stanu.

**[00:19:13]** Na przykład research, musimy zrobić badania rynku, gdzie musimy wybrać konkretne narzędzia albo połączyć ten proces,

**[00:19:20]** z narzędziami zewnętrznymi i później potrzebujemy krytycznej oceny.

**[00:19:24]** No to taki złożony proces, gdzie kroki w zasadzie układają się w trakcie i nie jesteśmy ich w stanie ułożyć na samym początku,

**[00:19:30]** tak jak właśnie w przypadku automatyzacji, to to jest właśnie rozwiązanie dla agenta, czyli dla kodkoda albo dla kodeksa.

**[00:19:37]** I ja zawsze lubię o tym opowiadać, bo to jest taka podstawa, którą często ludzie pomijają,

**[00:19:42]** a ta świadomość tego już na samym początku może Wam nawet rozwiązać po prostu problem, który macie w pracy i nie wiecie jak się zaniknąć.

**[00:19:50]** Możecie go zabrać.

**[00:19:52]** I pójdźmy teraz o krok dalej, ponieważ ja chcę pokazać Wam kolejny element już na przykładzie.

**[00:20:00]** Teraz powiedziałam troszeczkę o teorii, żeby wyrównać poziom, żeby dać wprowadzenie, a dalej przejdziemy sobie głębiej już na konkretny przykład.

**[00:20:09]** Myślenie systemami.

**[00:20:11]** To jest taki sposób pracy z modelami językowymi, w którym chcemy zamienić powtarzalny proces w jakąś automatyzację, usprawnić sobie proces.

**[00:20:20]** Chcę Wam to pokazać na przykładzie analizy konkurencji.

**[00:20:23]** Chcę, żebyście wyobrazili sobie, że zbieramy listę firm od marketingu i od CEO na polskim rynku, agencji marketingowych.

**[00:20:32]** I ja faktycznie zebrałam listę 60 agencji marketingowych w Polsce i chcemy sprawdzić, jak na tle tych firm wygląda jedna z wybranych agencji,

**[00:20:41]** zrobić research, uporządkować dane, zebrać te dane i wyciągnąć z nich wnioski.

**[00:20:46]** Więc to będzie nasz przykład, który ja będę teraz pokazywać.

**[00:20:49]** Ale...

**[00:20:50]** Chcę, żebyście wiedzieli, że ten jeden sposób, który Wam teraz pokażę, jesteśmy w stanie zastosować tak naprawdę na masie innych pomysłów.

**[00:20:58]** Dlatego, że ten schemat, który ja użyję teraz do pokazania, jak się robi analizę konkurencji, możemy na przykład użyć do nauki nowego tematu.

**[00:21:07]** Czyli wszystko, czego uczymy się na przykład o AI, możemy mieć w jednym miejscu i możemy użyć tego sposobu do takiego pomysłu.

**[00:21:16]** Jeśli pracujecie w jakiejś firmie, możecie zrobić bazę wiedzy działów.

**[00:21:19]** W firmie też tym sposobem.

**[00:21:21]** Czy to są dokumenty, procedury, czy jakieś ustalenia, czy pracujecie w sprzedaży, w HR-ach, w finansach, czy w jakimkolwiek innym dziale,

**[00:21:29]** to też byłoby coś, co da się wykorzystać tym samym sposobem, który za chwilę pokażę.

**[00:21:35]** I jeśli na przykład chcecie to mieć jako swój prywatny użytek i mieć takiego swojego doradcę i po prostu wrzucić w ten system nawet swoje notatki, swoje przemyślenia,

**[00:21:48]** swoje jakieś dokumenty, na których pracujecie i zrobić z tego prywatnego doradcę, który przypomina, podpowiada albo z którym zbijacie myśli,

**[00:21:56]** to tak samo w ten sposób można tutaj wykorzystać.

**[00:21:59]** Więc przejdźmy teraz krok dalej.

**[00:22:04]** O co chodzi w tym myśleniu systemami?

**[00:22:07]** Chodzi o to, żeby opisywać zadanie, które oddajemy w taki sposób do modela językowego, żeby zmapować wszystko po drodze.

**[00:22:17]** I co ja mam tutaj na myśli?

**[00:22:18]** Pokażę wam.

**[00:22:19]** Pokażę wam to teraz na przykładzie.

**[00:22:21]** Jeśli robimy analizę konkurencji, to na samym początku musimy się zastanowić, czego my potrzebujemy.

**[00:22:27]** Potrzebujemy informacji ze stron internetowych, potrzebujemy cenników, potrzebujemy na przykład iluś tam konkurentów i dane o nich.

**[00:22:35]** Więc musimy się zastanowić w takim opisie pracy, przekazywaniu kontekstu do agenta, na jakich danych będziemy pracować.

**[00:22:43]** Później musimy się zastanowić, skąd te dane weźmiemy i jakich narzędzi potrzebujemy.

**[00:22:48]** Na przykład pracujemy w jakiejś firmie, korzystamy z Notion.

**[00:22:52]** I w Notion są informacje o różnych agencjach marketingowych, które już zresearchowaliśmy.

**[00:22:57]** Mamy jakieś dane z CRM-u z Airtable.

**[00:23:00]** Potrzebujemy danych z internetu, więc tu musimy się zastanowić, ok, będzie mi potrzebny FireCrawl.

**[00:23:05]** I tu już możecie zobaczyć, że wracając do poprzedniego punktu, to myślenie systemami już nam się układa w taki proces, że widzimy, ok, mamy tutaj wiele narzędzi.

**[00:23:16]** Research to będzie proces wieloetapowy.

**[00:23:19]** Musimy się połączyć z narzędziami wewnętrznymi, gdzie jest jakaś wiedza, pobrać coś z internetu, spisać cały ten proces.

**[00:23:28]** I tutaj też nam to pokazuje, które rozwiązanie będzie najlepsze najprawdopodobniej.

**[00:23:32]** W takim zadaniu to będzie właśnie agent, czyli krotkot.

**[00:23:35]** Ja tu jeszcze zapisałam skill, o którym za chwilę trochę więcej powiem.

**[00:23:38]** Potem musimy się zastanowić, czy ten nasz proces potrzebuje decyzji.

**[00:23:43]** Tutaj wiemy na przykład, że...

**[00:23:45]** Jeśli dane są starsze, to będą musiały być update'owane.

**[00:23:49]** Trzeba jakoś nad nimi iterować.

**[00:23:51]** Musimy też mieć tą dozę krytycznego myślenia przy takim researchu i wyciąganiu wniosków.

**[00:23:57]** Więc to już nas doprowadza do tego, że ok, w takim wypadku to jest proces niedeterministyczny.

**[00:24:02]** Kroki będą ustalane w trakcie, więc agent jest dobrym rozwiązaniem do tego konkretnego zadania.

**[00:24:10]** I słuchajcie, kolejnym elementem takiej pracy jest to, że ok,

**[00:24:14]** wiemy już, że mamy te dane i co teraz z tymi danymi możemy zrobić?

**[00:24:19]** Nie ma czegoś takiego praktycznie, jak się faktycznie pracuje z modelami językowymi,

**[00:24:24]** jak praca z modelami bez pamięci.

**[00:24:27]** Jeśli używacie czata GPT w przeglądarce, to dobrze wiecie,

**[00:24:30]** że w pewnym momencie jest tak, że to wasze okienko czatu już jest takie długie,

**[00:24:35]** kontekst się gubi i on na przykład zaczyna odpowiadać po jakimś czasie gorzej.

**[00:24:39]** W związku z tym, żeby zaprojektować taki naprawdę użyteczny i dobry system,

**[00:24:44]** pracy z modelami językowymi, to trzeba się zastanowić nad tym,

**[00:24:47]** jak my mu zaprojektujemy pamięć.

**[00:24:50]** I jest kilka sposobów, tutaj teraz się odnoszę do osób technicznych,

**[00:24:54]** że jest wiele sposobów, jak możemy to przedstawić.

**[00:24:57]** Ja pokażę teraz jeden z nich, który nazywam LLM Brain.

**[00:25:03]** Jest to baza danych dla osób technicznych, grafowa baza danych,

**[00:25:06]** o której zaraz powiem troszeczkę więcej, która właśnie pełni rolę takiej pamięci dla modelu.

**[00:25:14]** Potrzebujemy tego, ponieważ mamy bardzo dużo danych, bardzo dużo informacji.

**[00:25:18]** Chcemy zrobić research 60 agencji marketingowych w Polsce

**[00:25:22]** i jak my te dane mamy przechować.

**[00:25:24]** No nie wrzucimy tego wszystkiego do jednego okienka czatu,

**[00:25:26]** bo zrobi się z tego jeden wielki bałagan, zaraz skończy nam się okno kontekstu

**[00:25:32]** i będzie problem.

**[00:25:32]** Więc po to właśnie wykorzystuje się takie bazy danych,

**[00:25:36]** żeby stworzyć taki dynamiczny mózg, który właśnie będzie sam się usprawniał

**[00:25:42]** i widział połączenia pomiędzy przeróżnymi danymi, które mu tam damy do środka.

**[00:25:48]** I po co to robimy?

**[00:25:48]** Robimy to po to, żeby nasz model językowy miał podstawę do tego,

**[00:25:54]** żeby naprawdę bardzo dużo dowiedzieć się o naszym projekcie z różnych stron,

**[00:25:58]** żeby to bardzo dobrze opisać.

**[00:26:00]** To jest właśnie też część przekazywania kontekstu

**[00:26:04]** i na podstawie tego zrobimy sobie taki bardzo dobry fundament do tego,

**[00:26:08]** żeby nasz model językowy, żeby nasz agent,

**[00:26:12]** wyciągnął wnioski i dał nam analizę, taką analizę konkurencji,

**[00:26:18]** która jest naprawdę poparta na ogromnej ilości danych,

**[00:26:22]** na połączeniach i wnioskach z tych właśnie plików, które mu damy,

**[00:26:28]** które sami zapewne albo robilibyśmy dniami, godzinami,

**[00:26:32]** albo właśnie byłoby to nawet niemożliwe do zauważenia,

**[00:26:38]** co możemy zrobić dzięki temu, że korzystamy z modeli językowych.

**[00:26:42]** I teraz Wam pokażę, jak właśnie działa i powstaje taki LLM Brain

**[00:26:49]** i to, co teraz zobaczycie, może wyglądać na jakąś czarną magię

**[00:26:54]** i naprawdę na skomplikowane, ale chcę Wam tutaj powiedzieć

**[00:26:57]** i Was zapewnić, że to, co ja Wam teraz pokazuję,

**[00:27:01]** jest tak naprawdę w stanie złożyć nawet osoba pracująca na kasie

**[00:27:06]** i tutaj daję przykład takiej osoby, bo chodzi mi po prostu o wymienienie zawodu,

**[00:27:10]** który jest zupełnie spoza niszy biznesowej.

**[00:27:13]** Naprawdę jakby jest to proces, w którym programowanie nie jest potrzebne

**[00:27:17]** i jedyne, co jest potrzebne, to zrozumienie działania tego

**[00:27:21]** i odpowiednie przekazanie kontekstu, które macie Wy jako specjaliści

**[00:27:26]** z wiedzą ekspercką w danej dziedzinie.

**[00:27:28]** I teraz Wam, tak, za chwilę Wam pokażę, jak wygląda ten LLM Brain,

**[00:27:34]** ale czego my potrzebujemy, żeby w ogóle go stworzyć.

**[00:27:38]** Więc tak, tutaj teraz przechodzimy do kolejnego elementu, czego szuka rynek,

**[00:27:42]** czyli rynek potrzebuje ludzi, którzy potrafią pobrać tę wiedzę z wewnętrznych narzędzi,

**[00:27:51]** zebrać dane firmy i ułożyć taki system prawdy,

**[00:27:55]** który właśnie będzie dostosowany do pracy z modelem językowym.

**[00:27:59]** Więc jak to powstaje?

**[00:28:00]** Najpierw pobieramy informacje i teraz tak, mamy informacje z internetu,

**[00:28:05]** na przykład mamy pobrane wszystkie informacje ze stron internetowych

**[00:28:08]** z tych właśnie agencji marketingowych.

**[00:28:12]** Robimy to za pomocą połączenia właśnie klockoda z FireCrawlem.

**[00:28:16]** Później pobieramy, jeśli pracujemy w jakiejś firmie z CRM-ów, z Airtable,

**[00:28:21]** robimy to za pomocą połączenia konektorów z klockodem właśnie z tymi narzędziami

**[00:28:28]** i pobieramy te wszystkie informacje i to są nasze źródła prawdy.

**[00:28:31]** I później wybieramy sobie narzędzie i w tym wypadku ja wybrałam Obsidian,

**[00:28:37]** który pozwala nam stworzyć grafową bazę danych.

**[00:28:40]** Dlaczego graf?

**[00:28:41]** Zaraz Wam pokażę, jak ten graf działa, ale generalnie one są bardzo fajne

**[00:28:46]** do pracy z modelami językowymi, ponieważ one pozwalają na to,

**[00:28:50]** żeby model językowy sam stworzył bazę danych, w którym sam zobaczy połączenia

**[00:28:54]** pomiędzy różnymi źródłami i to jest właśnie ten klucz.

**[00:28:57]** I potem kolejnym elementem, po tym jak już weźmiemy te źródła prawdy,

**[00:29:02]** jak już wstawimy je do Obsidiana, jak już ustawimy odpowiednio,

**[00:29:07]** właśnie napiszemy odpowiednio sposób, w jaki klockod ma,

**[00:29:11]** jak ma uporządkować te dane w Obsidianie dla nas,

**[00:29:14]** to wtedy tworzymy z tego skill, tworzymy z tego umiejętność,

**[00:29:18]** czyli opisujemy mu, o czym są te dane, nasz sposób pracy,

**[00:29:22]** jakie informacje on ma wyciągnąć i jak ma je uporządkować,

**[00:29:25]** żeby on stworzył dla nas taką właśnie bazę danych.

**[00:29:29]** Jak ta baza danych wygląda?

**[00:29:30]** Ja się teraz przełączę do Obsidiana i teraz Damian pytanie,

**[00:29:34]** czy widać dobrze teraz Obsidiana?

**[00:29:37]** Widać.

**[00:29:43]** Widać.

**[00:29:44]** Czy dobrze? To ciężko stwierdzić.

**[00:29:47]** Mogłabyś troszkę powiększyć, myślę, jakby się da.

**[00:29:52]** Może Shift, Ctrl+, o lepiej, no.

**[00:29:58]** Tak.

**[00:30:00]** Także jak widzicie, faktycznie, teraz może trochę pomniejszę i powiększę,

**[00:30:03]** żeby dać wam perspektywę.

**[00:30:05]** Faktycznie wygląda to jak mózg.

**[00:30:07]** Możecie tutaj zobaczyć przeróżne klastry, ja je za chwilę powiększę,

**[00:30:10]** to jest żeby pokazać wam perspektywę, w których widzicie,

**[00:30:14]** mamy takie centra i one coś oznaczają.

**[00:30:17]** I teraz wam opiszę, o co tutaj chodzi.

**[00:30:20]** Słuchajcie, to jest tak, że dajemy do modelu językowego,

**[00:30:26]** właśnie w takiej grafowej bazie wiedzy, gołe pliki.

**[00:30:30]** I te pliki mamy tutaj w tym folderze, gdzie mamy dosłownie,

**[00:30:34]** faktycznie prawdziwe agencje marketingowe z Polski.

**[00:30:39]** Mamy 60 agencji marketingowych.

**[00:30:41]** Tylko, że ja zrobiłam anonimizację ich nazw,

**[00:30:46]** żeby nikogo tu nie reklamować,

**[00:30:48]** więc możecie tam zobaczyć poprzekręcane nazwy,

**[00:30:51]** ale dane są faktycznie prawdziwe.

**[00:30:55]** I strukturyzujemy taki sposób właśnie pracy w tej bazie danych

**[00:31:00]** i to, co model językowy robi dla nas,

**[00:31:03]** czyli co Cloud Code robi dla nas w takiej bazie danych,

**[00:31:05]** to on sam wyciąga segmenty i grupuje nam te firmy,

**[00:31:11]** więc tworzy taką bazę danych, w której na przykład możemy zobaczyć,

**[00:31:15]** że mamy tutaj zebrany klaster.

**[00:31:17]** Mamy zebrany klaster firm, które są skupione na tym,

**[00:31:22]** że to są małe, średnie przedsiębiorstwa

**[00:31:25]** i one działają w taki sposób, że zapewniają innym firmom performance.

**[00:31:30]** Tutaj na przykład mamy takie, które zapewniają,

**[00:31:33]** są to duże firmy, które zapewniają visibility marki.

**[00:31:36]** Tutaj mamy analogicznie małe, średnie przedsiębiorstwa,

**[00:31:40]** które zapewniają visibility marki, widoczność marki

**[00:31:43]** i tak samo analogicznie mamy duże firmy,

**[00:31:46]** które właśnie dają wynik sprzedażowy firmom.

**[00:31:50]** I jak widzicie model językowy sam sobie tworzy te klastry

**[00:31:53]** i sam to grupuje, to nie jest coś, co my musimy zrobić.

**[00:31:56]** I oprócz tego to, co jest tutaj też interesujące,

**[00:32:00]** to to, że w takiej bazie wiedzy mamy te wszystkie połączenia,

**[00:32:05]** mamy też koncepty, czyli model językowy sam wyciąga koncepty,

**[00:32:10]** one mi się tutaj zapisały po angielsku,

**[00:32:12]** ale oczywiście może to być też po polsku,

**[00:32:15]** to jest po prostu przez sposób, w jaki pracowałam.

**[00:32:18]** Więc mamy tutaj na przykład metodologię,

**[00:32:21]** które firmy marketingowe używają jakiego CEO,

**[00:32:25]** jakie mają CEO na landing page'ach,

**[00:32:27]** jak oni kwalifikują osoby, które mogą zostać ich właśnie klientami,

**[00:32:33]** czy mają branding, który jest oparty na założycielu,

**[00:32:38]** jaką mają edukację.

**[00:32:41]** Jest bardzo, bardzo dużo konceptów,

**[00:32:43]** które właśnie sam nam model językowy stąd wyciągnął.

**[00:32:49]** I to, co widzicie teraz, może wydawać wam się bardzo skomplikowane,

**[00:32:55]** ponieważ możecie sobie zapewne, zgaduję, że może być tak teraz,

**[00:33:01]** że widzicie tą bazę grafową i macie takie,

**[00:33:04]** kurczę, ale jak ja będę z tego korzystać?

**[00:33:06]** Przecież to wygląda na tak skomplikowane.

**[00:33:09]** Tych danych tutaj jest masa.

**[00:33:11]** Ja nie wiem, jak się po tym poruszać.

**[00:33:13]** Może to jest długi czas, żeby to ogarnąć, żeby się tego nauczyć.

**[00:33:18]** I teraz chcę wam powiedzieć, że to wygląda w ten sposób,

**[00:33:21]** ale to nie jest dla nas.

**[00:33:23]** To nie jest dla nas jako dla człowieka,

**[00:33:26]** w sensie dla mnie jako dla Oli,

**[00:33:28]** bo ta baza danych wygląda w ten sposób,

**[00:33:31]** ponieważ ona jest dostosowana do naszego agenta.

**[00:33:34]** To jest zrobione specjalnie w taki sposób,

**[00:33:36]** żeby na przykład kod, kod albo kodeks,

**[00:33:40]** nieważne, co sobie wybierzecie do pracy,

**[00:33:42]** był w stanie właśnie przechodzić przez te informacje,

**[00:33:46]** szybko znajdować sobie tutaj połączenia pomiędzy tymi informacjami

**[00:33:50]** i na podstawie tego wyciągać wnioski.

**[00:33:53]** Więc to, co widzicie tutaj, jest dla agenta,

**[00:33:55]** a to, co pokażę wam zaraz, to jest coś, co robicie

**[00:33:58]** i widzicie wy po zbudowaniu takiego systemu.

**[00:34:02]** I tutaj jeszcze zanim przejdę, powiem wam, że no,

**[00:34:06]** to jest to taki bardzo złożony system notatek,

**[00:34:08]** tak działa ta baza danych,

**[00:34:10]** że na przykład możemy sobie wejść w jakąś konkretną agencję

**[00:34:14]** i tutaj tagami będzie oznaczona,

**[00:34:16]** będą informacje, będzie jej pozycjonowanie,

**[00:34:19]** jak oni, co oni o siebie mówią

**[00:34:22]** i będą przeróżne, przeróżne właśnie informacje,

**[00:34:25]** więc można teoretycznie wejść i zobaczyć, co się tutaj znajduje,

**[00:34:29]** czyli tak jak wam mówiłam, analogicznie,

**[00:34:31]** gdybyście mieli taki system na przykład do nauki,

**[00:34:34]** no to moglibyście zobaczyć,

**[00:34:36]** że tutaj jest jakieś zagadnienie,

**[00:34:38]** uczycie się na przykład AI

**[00:34:39]** i na przykład teraz uczycie się grafowych baz danych

**[00:34:42]** i macie notatkę o grafowych bazach danych

**[00:34:44]** i wszystko w takim systemie jest zawarte.

**[00:34:48]** Tak samo możecie mieć konkretne koncepty

**[00:34:51]** i właśnie konkretne analizy.

**[00:34:54]** Więc tak jak mówiłam, to jest coś, co widzi model językowy,

**[00:34:57]** a teraz wam pokażę, co konkretnie widzicie wy.

**[00:35:01]** I to, co ja przygotowałam teraz dla was,

**[00:35:05]** to są takie wnioski, które dostarczył mi mój agent,

**[00:35:10]** ponieważ to był jego mózg, to jest jego baza,

**[00:35:13]** na której on pracuje i to, co on dostarcza mi,

**[00:35:16]** to jest właśnie analiza, to są wyniki,

**[00:35:19]** to są wnioski, które on wyciągnął z tych klastrów.

**[00:35:23]** I teraz wam pokażę, co widzę ja,

**[00:35:26]** jako właśnie taki specjalista wspierany przez AI,

**[00:35:30]** który zarządza takim agentem, który ma dostęp do takich informacji.

**[00:35:35]** To, co chcę wam tutaj przekazać, to jest to,

**[00:35:39]** że kiedy zaczynamy pracować z takim agentem jak KlotKot

**[00:35:42]** i zaczynamy przekazywać mu ten kontekst i naszą wiedzę,

**[00:35:45]** to nasza praca się zmienia

**[00:35:48]** z tej wykonawczej pracy na bardziej nadzorującą

**[00:35:52]** i to, co teraz wam pokażę, to jest właśnie proces tego nadzoru.

**[00:35:55]** Czyli KlotKot wykonał dla mnie coś, co ja bym robiła ze 2 miesiące,

**[00:36:00]** bo żeby zmapować, zrobić taki research

**[00:36:03]** i zmapować takie połączenia i zobaczyć,

**[00:36:06]** jak to wszystko ze sobą współgra,

**[00:36:08]** no to ja bym siedziała nad tym, nad taką manualną robotą

**[00:36:11]** bardzo, bardzo długo i on mi dostarcza wynik tego

**[00:36:14]** i jakby to teraz w moim krytycznym myśleniu jest jakby w moim,

**[00:36:20]** że tak powiem, moim obowiązkiem jest teraz to sprawdzić,

**[00:36:24]** nadzorować, zobaczyć, co on mi tutaj przyniósł

**[00:36:26]** i poiterować go, czy idziemy w dobrym kierunku,

**[00:36:29]** czy dalej ma nad tym pracować.

**[00:36:31]** Więc teraz sprawdźmy sobie, jakie on mi przygotował tutaj klastry.

**[00:36:37]** Na analizie konkurencji tu możecie zobaczyć,

**[00:36:40]** że to jest wizualne przedstawienie tego, co on mi dał.

**[00:36:42]** On mi dał 6 różnych klastrów i 4 z nich dotyczą firm,

**[00:36:46]** a 2 z nich dotyczą samych wniosków i analiz.

**[00:36:50]** Na samym początku Klot zobaczył, że przeanalizował,

**[00:36:56]** że 25 agencji to są agencje, które robią leady dla małych firm

**[00:37:01]** i opisuje mi tutaj, co one mówią wprost,

**[00:37:04]** że one mówią wprost do właściciela małej firmy,

**[00:37:07]** to są firmy, które robią telefony, zapytania, zamówienia,

**[00:37:10]** mają jawne ceny i gwarancje na rynku

**[00:37:13]** i zgrupował mi taki jeden klaster.

**[00:37:15]** Kolejna grupa z analizy konkurencji to są firmy,

**[00:37:19]** które właśnie robią wyniki dla dużych marek

**[00:37:21]** i ja pokazywałam Wam te klastry na samym grafie,

**[00:37:24]** tylko teraz pokazuję Wam już same wnioski z nich,

**[00:37:27]** bo nie chodzi o to, żebyśmy my przeglądali teraz

**[00:37:30]** każde z tych notatek i sami łapali wnioski,

**[00:37:33]** tylko my to dostajemy jako gotowy wynik.

**[00:37:35]** Kolejny klaster to jest na przykład

**[00:37:37]** agencji, które zajmują się wynikami dla dużych marek

**[00:37:40]** i to są właśnie agencje, które mają opisane procesy,

**[00:37:44]** mają własne narzędzia, rozliczają się z ROAS-u,

**[00:37:47]** czyli z wyniku tego, ile przyniosą reklamy

**[00:37:51]** i bardzo, bardzo liczy się dla nich

**[00:37:54]** koszt pozyskanego klienta.

**[00:37:56]** Kolejny klaster, jaki Claude zauważył,

**[00:37:59]** to są marki małych firm,

**[00:38:03]** czyli tutaj mamy małe firmy, które chcą wyglądać i brzmieć,

**[00:38:06]** jak większa marka i co one dostają od tych agencji,

**[00:38:10]** dostają estetykę i portfolio,

**[00:38:13]** czyli na przykład zarządzanie contentem.

**[00:38:15]** Kolejny klaster, jaki zauważył,

**[00:38:20]** to jest 12 agencji marketingowych,

**[00:38:23]** które głównie robią kampanie dla dużych marek,

**[00:38:25]** czyli na przykład przychodzi do nich dyrektor marketingu,

**[00:38:28]** kupuje kreację, kupuje wizerunek

**[00:38:30]** i mamy tutaj, często takie agencje nie podają ceny,

**[00:38:35]** ale za to mają dużą listę klientów,

**[00:38:38]** którzy są zazwyczaj znani i duzi.

**[00:38:42]** I oprócz tego, że Claude wziął mi te gołe dane

**[00:38:45]** i tak je pogrupował i zrobił naprawdę bardzo głęboką analizę konkurencji,

**[00:38:49]** to zwrócił mi coś jeszcze,

**[00:38:52]** zwrócił mi właśnie te koncepty

**[00:38:54]** i tutaj on mi zwraca wzorce,

**[00:38:56]** które powtarzają się pomiędzy firmami.

**[00:38:59]** Mamy tutaj archetypy tego, jak działają te firmy,

**[00:39:04]** mamy mechanizmy tego, jak one dowożą wartość,

**[00:39:11]** czy cena jest jawna, czy dają gwarancję,

**[00:39:15]** mamy nazwane ich metody,

**[00:39:17]** jak one działają, jeśli chodzi o edukację,

**[00:39:19]** jaki mają sposób pozyskiwania klientów

**[00:39:21]** i to zostało wyodrębnione jako koncepty.

**[00:39:24]** I mamy też kolejną rzecz, czyli analizy,

**[00:39:27]** czyli już wnioski, które Claude wyniósł na podstawie tego,

**[00:39:33]** jak zobaczył te wszystkie połączenia pomiędzy tymi właśnie danymi.

**[00:39:41]** I tutaj możemy mieć gotowe odpowiedzi, notatki,

**[00:39:45]** możemy mieć porównanie,

**[00:39:47]** czasami nawet tworzy macierze usług, cenników, warunków

**[00:39:51]** i tu na podstawie tego można zrobić taką mapę pozycjonowania

**[00:39:56]** oraz zobaczyć, jakie w ogóle mamy luki na rynku i szanse.

**[00:40:01]** I teraz tutaj też odniosę się do tego,

**[00:40:03]** że gdybyśmy używali tego systemu dla czegoś innego

**[00:40:05]** niż analiza konkurencji,

**[00:40:07]** no to tak samo mielibyśmy na przykład pogrupowane nasze dane

**[00:40:11]** w różne klastry, na temat czego zbieramy informacje,

**[00:40:15]** tak samo mielibyśmy wyodrębnione koncepty,

**[00:40:18]** nad którymi pracujemy i tak samo mielibyśmy analizy.

**[00:40:21]** I teraz sobie pomyślicie pewnie,

**[00:40:23]** kurczę, ale jak zarządzać tą bazą danych

**[00:40:26]** i co, jeśli ja dorzucę kolejne informacje?

**[00:40:30]** No właśnie, jeśli pracujemy skutecznie

**[00:40:32]** z modelami językowymi,

**[00:40:33]** to jesteśmy w stanie ustawić ten system w taki sposób właśnie,

**[00:40:36]** że dodając nową analizę, dodając nawet nowy koncept,

**[00:40:41]** to Claude przejdzie przez całą bazę danych

**[00:40:45]** i zobaczy, czy ten nowy koncept, czy ta nowa analiza,

**[00:40:47]** czy może nowa dorzucona firma łączy się

**[00:40:50]** ze wszystkimi innymi danymi, które tu mamy

**[00:40:53]** i sam zupdate'uje wszystkie połączenia w bazie danych.

**[00:40:57]** Zaraz wrócę sobie do Obsidiana.

**[00:40:59]** Gdybym dorzuciła tutaj,

**[00:41:02]** tutaj nową firmę, to agent zacząłby od tego,

**[00:41:07]** że nie zostawiłby jej sobie jako takie osobne kółeczko,

**[00:41:10]** które sobie tutaj wisi,

**[00:41:11]** tylko przeszedłby przez wszystkie te pliki

**[00:41:14]** i zobaczył, czy ona się z czymkolwiek nie łączy

**[00:41:17]** i zrobił nowe połączenia, które by tutaj na tym grafie

**[00:41:20]** zaczęły widnieć jako po prostu nowe strzałki.

**[00:41:25]** I teraz odniosę się jeszcze raz,

**[00:41:26]** jeśli mamy tutaj osoby techniczne,

**[00:41:28]** że oczywiście jest to jeden tylko sposób,

**[00:41:32]** w jaki możemy tworzyć bazę danych,

**[00:41:34]** dla modeli językowych.

**[00:41:36]** On jest bardzo skuteczny.

**[00:41:38]** Są też inne sposoby,

**[00:41:39]** także to nie jest tak, że to jest jeden możliwy

**[00:41:44]** i jeden jedyny, za którym trzeba obecnie iść,

**[00:41:47]** ale jest to na pewno taki uniwersalny sposób,

**[00:41:50]** który w wielu przypadkach bardzo dużo Wam pomoże uzyskać

**[00:41:55]** i który też na pewno jest czymś fajnym do pokazania

**[00:42:00]** i nadaje się do bardzo, bardzo wielu firm.

**[00:42:03]** I jak mamy już te wnioski,

**[00:42:06]** widzimy właśnie te wzorce, analizę,

**[00:42:09]** to właśnie z tego może nam powstać

**[00:42:13]** taka prawdziwa analiza konkurencji.

**[00:42:17]** Bo możemy też wziąć te nagie dane,

**[00:42:21]** pobrane ze stron internetowych

**[00:42:23]** i po prostu wrzucić je do Claude'a.

**[00:42:25]** I jak zapewne wiecie, pracując z modelami językowymi,

**[00:42:29]** jak czasem wrzucicie mu 5, 10 plików, nie wiadomo co,

**[00:42:32]** no to on zrobi to bardzo pobieżnie,

**[00:42:35]** zwróci Wam coś generycznego,

**[00:42:37]** nie zauważy szczegółów,

**[00:42:39]** będziecie musieli rozbijać zadanie na małe etapy,

**[00:42:43]** no i tak się pracuje iteracyjnie i różnie to wychodzi.

**[00:42:46]** A jeśli pracujemy na takiej bazie danych,

**[00:42:48]** no to już mamy z góry bardziej opisany kontekst,

**[00:42:52]** mamy sposoby pracy,

**[00:42:54]** bo tam możemy naprawdę wszystko wrzucić.

**[00:42:55]** Możemy mu też wrzucić informacje,

**[00:42:57]** w jaki sposób on ma w ogóle korzystać z tej bazy danych.

**[00:42:59]** Jeśli byśmy robili na przykład bazę jakiegoś procesu firmowego,

**[00:43:01]** to też możemy to tak ustawić,

**[00:43:04]** żeby on w taki sposób działał.

**[00:43:06]** I wtedy na przykład,

**[00:43:07]** ja teraz Wam pokazuję wnioski

**[00:43:09]** dla jednej przykładowej agencji marketingowej,

**[00:43:12]** wtedy takie wnioski są o wiele bardziej skuteczne.

**[00:43:20]** One mogą pozwolić nam zauważyć coś,

**[00:43:23]** czego normalnie byśmy nie zauważyli

**[00:43:26]** bez tak dogłębnej analizy,

**[00:43:29]** która po prostu łączy,

**[00:43:31]** bo to są takie kropki.

**[00:43:33]** I wiem, że bardzo wiele osób spotyka się też z takim problemem właśnie,

**[00:43:36]** że pracuje na modelach językowych

**[00:43:38]** i ma takie kurczę, ale przecież on nie wie,

**[00:43:40]** na przykład jak ja piszę teraz ten raport,

**[00:43:42]** to on nie wie, że ja potrzebuję jakichś wniosków

**[00:43:45]** z raportu sprzed trzech miesięcy.

**[00:43:47]** No to właśnie w takiej sytuacji

**[00:43:49]** można stworzyć sobie później taką analizę,

**[00:43:51]** taki dashboard, który będzie widział te połączenia,

**[00:43:53]** bo ten graf po prostu to zapewni i zadba o to.

**[00:43:57]** No i zobaczmy,

**[00:43:59]** jak to wygląda dla agencji marketingowej,

**[00:44:02]** która właśnie,

**[00:44:04]** oczywiście nazwę sobie gdzieś tam wymyśliłam

**[00:44:06]** i w sensie zanimizowałam ją,

**[00:44:08]** ale dane są prawdziwe

**[00:44:10]** i możemy tutaj zobaczyć,

**[00:44:12]** że ta na przykład agencja mega się wyróżnia

**[00:44:14]** na tle innych na rynku,

**[00:44:16]** ponieważ właśnie robi AACO

**[00:44:18]** i widać, że robi to tylko 8 firm z 59.

**[00:44:23]** Możemy właśnie zobaczyć, co jest jej wyróżnikiem

**[00:44:27]** i mamy od razu podane wnioski,

**[00:44:29]** czym ona jest lepsza od rynku,

**[00:44:31]** że na przykład mówi o cenie,

**[00:44:32]** a to nie jest takie oczywiste,

**[00:44:33]** bo wiele firm nie mówi o cenie,

**[00:44:35]** to wynika tutaj z tych danych,

**[00:44:36]** że ma wiele klientów,

**[00:44:38]** czym jest słabsza

**[00:44:39]** i od razu mamy podane,

**[00:44:40]** co możemy w ogóle zrobić,

**[00:44:42]** żeby się wyróżnić,

**[00:44:43]** co ta agencja może zrobić,

**[00:44:45]** żeby się wyróżnić.

**[00:44:46]** No i taki sposób może też być potencjalnie po to,

**[00:44:50]** żeby na przykład pozyskiwać klientów

**[00:44:55]** albo można uderzyć do danej firmy

**[00:44:57]** i powiedzieć hej,

**[00:44:58]** zauważyłem takie luki u was,

**[00:44:59]** możecie to usprawnić.

**[00:45:00]** To też taki mały tip dla osób,

**[00:45:02]** które szukają pracy,

**[00:45:03]** że możecie zrobić takie research o firmie,

**[00:45:05]** do której uderzacie

**[00:45:06]** i zaproponować im coś,

**[00:45:08]** jak wbijacie na jakąś daną pozycję.

**[00:45:10]** Można też zobaczyć z takiej analizy właśnie,

**[00:45:12]** jak ta firma konkretnie się pozycjonuje właśnie wobec rynku,

**[00:45:19]** jeśli chodzi o jej ofertę

**[00:45:21]** i możemy sprawdzić też właśnie,

**[00:45:24]** jaka jest jej pozycja,

**[00:45:25]** taka bardziej związana z samymi danymi

**[00:45:28]** i też są jakieś,

**[00:45:30]** mam tutaj informacje na temat klientów,

**[00:45:32]** na temat tego, co można znaleźć na ich stronie

**[00:45:34]** i jak oni siebie pozycjonują.

**[00:45:37]** I ja z własnego doświadczenia pracy na danych,

**[00:45:40]** co mam bardzo wiele lat,

**[00:45:42]** robiłam to w przeróżnych branżach,

**[00:45:45]** wiem, że czasami ten proces wyciągania wniosków

**[00:45:49]** jest taki bardzo mozolny,

**[00:45:51]** a tutaj jakby w modele językowe to nam ułatwiają,

**[00:45:54]** że jesteśmy w stanie wyciągać wnioski,

**[00:45:56]** które faktycznie dają wartość.

**[00:45:58]** I to, co chcę tutaj też przekazać,

**[00:46:01]** to jest to, że generalnie wiadomo,

**[00:46:06]** że ten proces jest bardzo iteracyjny,

**[00:46:09]** więc jakby to też nie chodzi o to,

**[00:46:12]** że raz ustawimy taki system

**[00:46:14]** i właśnie on nam da od razu dobry wynik,

**[00:46:17]** tylko że będziemy nad tym iterować.

**[00:46:20]** I teraz przejdę sobie dalej

**[00:46:24]** i to był właśnie ten element tego kontekstu

**[00:46:28]** i wiedzy firmy,

**[00:46:30]** że jesteśmy w stanie stworzyć taką bazę danych,

**[00:46:32]** ustawić tą bazę danych do właśnie agentowi,

**[00:46:36]** jak on ma z niej korzystać

**[00:46:38]** i później to nam wszystko się mapuje

**[00:46:42]** właśnie do tej zdolności prototypowania.

**[00:46:47]** Dlatego, że ten system,

**[00:46:49]** który Wam teraz pokazałam,

**[00:46:51]** to jest tak naprawdę prototyp systemu

**[00:46:53]** albo wewnętrznie dla danej firmy,

**[00:46:56]** albo dla Was do Waszej konkretnej pracy.

**[00:46:59]** No i to jest właśnie ten taki proces,

**[00:47:01]** w którym Wy możecie pokazać,

**[00:47:03]** że hej, ja przecież jestem w stanie pracować

**[00:47:08]** z modelami językowymi,

**[00:47:10]** mam tą właśnie wiedzę,

**[00:47:11]** bo wiem, jakie wybrać rozwiązanie,

**[00:47:13]** potrafię zaprojektować taki system,

**[00:47:15]** potrafię pobrać te dane,

**[00:47:16]** potrafię zaprojektować te dane dla modelu językowego,

**[00:47:19]** a potem potrafię jeszcze zaproponować rozwiązanie,

**[00:47:22]** z którego możemy naprawdę wyciągnąć wnioski,

**[00:47:25]** które są wartościowe dla biznesu,

**[00:47:27]** na przykład robiąc właśnie taki artefakt,

**[00:47:29]** jaki Wam pokazałam,

**[00:47:30]** który Wam te wnioski uporządkuje.

**[00:47:33]** Dlatego tutaj właśnie tak mówię

**[00:47:36]** w tej zdolności prototypowania o tym,

**[00:47:38]** że bardzo ważne jest ogarnięcie dostępu do narzędzi

**[00:47:42]** i żeby cloud sięgał generalnie tylko tam,

**[00:47:46]** gdzie naprawdę jakby musimy pobrać te informacje.

**[00:47:50]** No i w jaki sposób to robimy?

**[00:47:52]** Teraz podsumowując już tak,

**[00:47:54]** wybieramy do tego clouda,

**[00:47:55]** łączymy go tylko z tymi narzędziami przez konektory,

**[00:47:58]** które są konieczne,

**[00:48:00]** wybieramy mu jeden konkretny folder

**[00:48:03]** i jeszcze w tej zdolności właśnie prototypowania

**[00:48:06]** i robienia tego całego procesu muszę zaznaczyć,

**[00:48:09]** że najważniejszy jesteśmy my,

**[00:48:13]** najważniejsza jest ta nasza tutaj wiedza ekspercka

**[00:48:19]** i to nasze działanie krytyczne,

**[00:48:21]** gdzie my będziemy tą osobą,

**[00:48:23]** która będzie sprawdzać jego wynik,

**[00:48:25]** będzie zatwierdzać jego wynik

**[00:48:27]** i będzie ewentualnie iterować nad tym wynikiem

**[00:48:29]** i kierować go w dobrą stronę

**[00:48:31]** i to jest to prawdziwe przekazywanie kontekstu.

**[00:48:34]** Teraz się mówi o tym,

**[00:48:35]** że kontekst jest trochę tak jak ropa.

**[00:48:38]** Kiedyś się mówiło, że dane są jak ropa,

**[00:48:40]** teraz mówi się o tym,

**[00:48:41]** że kontekst jest jak ropa,

**[00:48:43]** czyli że ta wiedza ekspercka,

**[00:48:47]** którą my jesteśmy w stanie po prostu przełożyć na proces pracy

**[00:48:52]** i na proces taki,

**[00:48:53]** który będzie czytelny dla modela językowego,

**[00:48:55]** żeby on właśnie odciążył nas z jakiegoś konkretnego zadania

**[00:49:00]** i to jest właśnie to.

**[00:49:03]** Jest jeszcze ostatni element,

**[00:49:05]** o którym chcę tutaj wspomnieć

**[00:49:07]** i to jest właśnie ewaluacja,

**[00:49:10]** a przepraszam,

**[00:49:11]** jeszcze tutaj właśnie chciałam jeszcze raz wspomnieć,

**[00:49:13]** że zanim przejdę do ewaluacji,

**[00:49:16]** to chciałam jeszcze tak troszeczkę podsumować,

**[00:49:19]** że podałam Wam przykład analizy konkurencji,

**[00:49:22]** no a jeszcze raz przypominając,

**[00:49:26]** że generalnie taki proces,

**[00:49:28]** jaki Wam teraz pokazałam,

**[00:49:29]** możemy wykorzystać do nauki danego tematu,

**[00:49:32]** możemy tu wrzucić materiały z YouTube,

**[00:49:35]** kursy, artykuły

**[00:49:36]** i możemy sobie mieć taką bazę wiedzy,

**[00:49:38]** która będzie po prostu nam pomagać w nauce,

**[00:49:40]** możemy tu przekazać wiedzę z danego działu,

**[00:49:42]** możemy zrobić z tego osobistego doradcę,

**[00:49:45]** jeśli pracujecie w HR-ach,

**[00:49:46]** to to może być taki materiał,

**[00:49:48]** gdzie mamy po prostu całą rekrutację,

**[00:49:52]** możemy mieć tu cenniki,

**[00:49:54]** cenniki oferty,

**[00:49:55]** jeśli na przykład pracujecie w dziale sprzedażowym

**[00:49:57]** i patrzycie, jak się zmienia rynek,

**[00:49:59]** to może być też użyte do customer service,

**[00:50:02]** do obsługi klienta,

**[00:50:03]** gdzie mamy powtarzalne pytania

**[00:50:04]** i taki agent będzie sobie wyciągał z tej bazy wiedzy

**[00:50:06]** i odpowiadał właśnie klientom

**[00:50:09]** na podstawie już innych case'ów rozwiązanych,

**[00:50:12]** innych pytań

**[00:50:13]** i całej masy po prostu danych zebranych tutaj.

**[00:50:17]** Więc tutaj też chcę podkreślić,

**[00:50:19]** że jesteśmy w stanie ułożyć ten sam system

**[00:50:22]** dla wielu innych spraw.

**[00:50:24]** I teraz wrócę właśnie do tego ostatniego elementu,

**[00:50:27]** czyli do oceny jakości wyniku,

**[00:50:29]** dlatego że tutaj chciałam Wam powiedzieć,

**[00:50:31]** że ta ocena jakości wyniku,

**[00:50:32]** ona nie tylko odnosi się i do tego systemu,

**[00:50:35]** który Wam pokazałam,

**[00:50:36]** nie tylko do konkretnego case'a,

**[00:50:38]** ale też tak naprawdę do wszystkiego,

**[00:50:40]** do czego bylibyście w stanie użyć ten system.

**[00:50:42]** To jest taki krytyczny punkt pracy z modelami językowymi,

**[00:50:46]** że zawsze musimy oceniać,

**[00:50:48]** jak ten model językowy właśnie zwraca nam te odpowiedzi.

**[00:50:52]** No i tutaj taka grafika,

**[00:50:54]** grafowa baza danych działa w taki sposób,

**[00:50:57]** że widzimy źródło,

**[00:51:00]** widzimy kiedy powstała dana notatka,

**[00:51:03]** jesteśmy w stanie wejść,

**[00:51:05]** zawsze jakoś zweryfikować,

**[00:51:07]** jakie informacje mu wrzuciliśmy,

**[00:51:09]** jak one zostały połączone

**[00:51:11]** i taki system będzie wymagał czegoś takiego,

**[00:51:15]** jak testowe przypadki,

**[00:51:17]** czyli zawsze powinniśmy mieć jakiś taki przypadek,

**[00:51:20]** na przykład jakiegoś połączenia,

**[00:51:22]** jakiegoś konceptu,

**[00:51:23]** który on powinien wyłapać,

**[00:51:25]** który taki system powinien wyłapać

**[00:51:27]** i powinniśmy mieć konkretne zapytanie,

**[00:51:30]** w którym zawsze możemy zapytać

**[00:51:32]** i zobaczyć, czy on na przykład wyłapie dalej te połączenia,

**[00:51:35]** czy jak na przykład dodamy mu 15 innych plików,

**[00:51:38]** czy on nie zacznie się gubić

**[00:51:39]** i nie zacznie nagle na przykład odpowiadać gorzej,

**[00:51:42]** więc powinniśmy mieć zawsze takie testowe przypadki

**[00:51:45]** i prowadzić taką ewaluację,

**[00:51:46]** żeby być w stanie oceniać jakość tej naszej bazy danych

**[00:51:49]** i czy ona nie degraduje z czasem,

**[00:51:51]** czy ona faktycznie się ulepsza

**[00:51:52]** i czy ten kontekst pozostaje zachowany.

**[00:51:56]** Więc tutaj też mamy właśnie taki aspekt,

**[00:52:00]** który chciałam Wam poruszyć na sam koniec.

**[00:52:05]** I jak widzicie,

**[00:52:07]** przeszliśmy sobie te wszystkie elementy,

**[00:52:11]** więc ja tutaj chcę jeszcze raz podsumować,

**[00:52:15]** że żeby stworzyć system pracy z AI,

**[00:52:19]** który pracuje razem z Wami

**[00:52:21]** i odciąża Was w części zadań,

**[00:52:23]** musimy przejść przez 5 elementów.

**[00:52:26]** Na samym początku musicie być naprawdę płynni w narzędziach AI

**[00:52:30]** i wiedzieć, kiedy ten model językowy się nadaje,

**[00:52:34]** a kiedy się nie nadaje do pracy,

**[00:52:37]** kiedy możemy użyć agenta,

**[00:52:39]** a kiedy agent to będzie za dużo,

**[00:52:41]** to będzie tak zwany overkill,

**[00:52:43]** no bo jeśli chcemy po prostu zrobić prosty brainstorm,

**[00:52:45]** no to może nie musimy angażować do tego żadnego kodkoda albo kodeksa.

**[00:52:49]** Potem musimy,

**[00:52:51]** żeby potrafić dobrze opisać sposób naszej pracy,

**[00:52:55]** czyli nauczyć się myśleć systemem

**[00:52:57]** i to jest właśnie to przekazywanie kontekstu,

**[00:53:00]** czy my bardzo dobrze zmapujemy tą naszą wiedzę ekspercką

**[00:53:04]** i czy my jesteśmy w stanie to ustrukturyzować,

**[00:53:06]** czy jesteśmy z tego w stanie wyizolować poszczególne etapy,

**[00:53:10]** powiedzieć z jakich danych korzystamy,

**[00:53:12]** jak korzystamy z tych danych,

**[00:53:13]** w jakiej kolejności,

**[00:53:15]** ile my tego potrzebujemy,

**[00:53:16]** czy my potrzebujemy to update'ować

**[00:53:18]** i zaprojektować właśnie, rozpisać sobie taki system,

**[00:53:21]** potem zastanowić się,

**[00:53:22]** czy my jesteśmy w stanie właśnie dostać się do tych danych,

**[00:53:26]** jak mamy je uporządkować,

**[00:53:27]** ile projektów musimy w to zaangażować

**[00:53:30]** i te trzy elementy są kluczowe,

**[00:53:33]** bo modele językowe też pracują na danych,

**[00:53:36]** nie mogą polegać tylko na swojej własnej wiedzy.

**[00:53:39]** No i później kolejny element to jest,

**[00:53:42]** jak stworzyć już rozwiązanie,

**[00:53:44]** czyli jak tak naprawdę dobrze pokierować tego kodkoda,

**[00:53:47]** żeby on nam zrobił po prostu,

**[00:53:51]** zmienił nasze pomysły w jakiś namacalny artefakt,

**[00:53:55]** w prototyp,

**[00:53:56]** który będzie dla nas narzędziem do wyciągania wniosków

**[00:53:59]** i jak mamy taki system,

**[00:54:01]** no to wtedy właśnie przestajemy wykonywać dane zadanie

**[00:54:06]** i możemy je oddelegować do agenta,

**[00:54:08]** stajemy się takim specjalistą wspieranym przez AI

**[00:54:12]** i to co my robimy,

**[00:54:13]** to jest właśnie ocena tego,

**[00:54:15]** krytyczne myślenie i takie bardziej strategiczne działanie,

**[00:54:19]** w którą stronę dalej mamy iść,

**[00:54:20]** jakie wnioski z tego wyciągnąć,

**[00:54:22]** skoro już oddaliśmy te powtarzalne,

**[00:54:25]** nudne czy też trudne i żmudne zadania do agenta,

**[00:54:28]** to jak my możemy teraz naprawdę na tych danych zrobić coś,

**[00:54:32]** co ma sens i przyniesie wartość

**[00:54:34]** i to się właśnie na samym końcu mapuje do tego,

**[00:54:37]** że musimy potrafić oceniać wyniki takiego systemu

**[00:54:42]** i widzieć, czy on realnie rozwiązuje problem,

**[00:54:45]** bo tutaj chcę wspomnieć o tym,

**[00:54:47]** że jest bardzo duży hype teraz na AI

**[00:54:49]** i myślimy, że ono jest w stanie rozwiązać wszystko,

**[00:54:51]** ale to jest tylko technologia

**[00:54:52]** i finalnie i tak jak projektujemy jakieś rozwiązanie,

**[00:54:55]** to ono jest po to, żeby rozwiązać jakiś dany problem,

**[00:54:57]** więc czy faktycznie rozwiązuje ten problem,

**[00:54:59]** czy może nie daje nam jakiejś konkretnej wartości.

**[00:55:04]** Tak i jeśli chodzi o wiedzę merytoryczną,

**[00:55:07]** to jest tak naprawdę wszystko,

**[00:55:09]** ale na sam koniec chcę wam jeszcze powiedzieć coś zupełnie szczerze

**[00:55:14]** i tutaj to, co chcę wam przekazać,

**[00:55:16]** to jest to, że teraz zobaczyliście naprawdę dobrze działający,

**[00:55:21]** system, w którym wiecie, macie piękną bazę danych,

**[00:55:25]** ona wygląda naprawdę jak mózg,

**[00:55:27]** są połączenia, dane są pobrane,

**[00:55:29]** ona się update'uje sama, sama się usprawnia,

**[00:55:32]** mamy też podane konkretne wnioski,

**[00:55:35]** mamy ten zbudowany artefakt

**[00:55:37]** i możecie sobie teraz pomyśleć,

**[00:55:41]** że to będzie jak magiczna różdżka

**[00:55:45]** i taki system będziemy mieć

**[00:55:47]** i ja zawsze bardzo lubię obalać hype

**[00:55:50]** i chcę wam powiedzieć tylko o tym,

**[00:55:52]** że ja lubię przekazywać to,

**[00:55:54]** że praca z modelem językowym to jest zawsze praca iteracyjna,

**[00:55:59]** zawsze będzie tak, że trzeba będzie go tam popromptować,

**[00:56:02]** pokierować i poiterować, jeśli chodzi o pracę z nim

**[00:56:05]** i po takich wiecie, falach iteracji

**[00:56:08]** w końcu będziemy mieli naprawdę dobrze działający system,

**[00:56:11]** tak było zawsze, taka jest natura modeli językowych,

**[00:56:14]** to prawda, że jest coraz łatwiej z nimi pracować,

**[00:56:16]** ale chcę zakończyć właśnie tą prezentację takim zabiciem tego hype'u,

**[00:56:21]** bo strasznie mnie on denerwuje,

**[00:56:23]** że ludzie myślą właśnie, że to jest nie wiadomo co

**[00:56:26]** i że tylko taką magiczną różdżką będziemy mieli niesamowity wynik

**[00:56:29]** i zapominają o naturze tego, jak działają modele językowe

**[00:56:33]** i że one właśnie wymagają iteracji.

**[00:56:35]** No tak, więc to będzie wszystko z mojej strony

**[00:56:40]** i teraz myślę, że oddam właśnie ekran i głos Damianowi.

**[00:56:47]** Dzięki Ola, ja sam się bardzo dużo nauczyłem dzisiaj,

**[00:56:53]** więc sądząc po komentarzach nasi widzowie także,

**[00:56:58]** więc ja przypominam, że już za chwilę będziemy rozdawać prezent,

**[00:57:02]** o który wam obiecaliśmy, czyli jak zbudować stronę internetową

**[00:57:05]** za 4 wieczory, ale jeszcze ja mam parę słów do dodania od siebie,

**[00:57:10]** więc pozwólcie, że wrócę do swojej części prezentacji

**[00:57:15]** i to co na początku dziś zapowiadaliśmy,

**[00:57:18]** to dzisiaj promptowanie już nie ma sensu na pewno,

**[00:57:21]** w sensie inaczej, sam prompt nie rozwiązuje takich problemów,

**[00:57:28]** o których uczono nas chociażby rok temu,

**[00:57:30]** gdzie mówiono nam, że prompty i prompt engineering jest najważniejszy.

**[00:57:36]** Dzisiaj już ta zasada jest troszkę passé.

**[00:57:41]** Przewagą jest zbudowanie systemu i przykład takiego systemu

**[00:57:45]** widzieliście przed chwilą na prezentacji Oli.

**[00:57:50]** Więc problem nie jest też w jakimś wyborze modeli AI,

**[00:57:54]** bo dzisiaj zobaczcie, że też wiele osób pyta się,

**[00:57:58]** a jakiego to modelu AI użyłeś?

**[00:58:01]** Do mnie czasami tak się ludzie pytają.

**[00:58:04]** Ja odpowiadam często, że to nie ma większego znaczenia,

**[00:58:07]** którego modelu używasz, dopóki naprawdę nie wydajesz setek tysięcy

**[00:58:14]** albo tysięcy na te tokeny, to prawdopodobnie nie ma znaczenia,

**[00:58:17]** jakiego modelu użyjesz.

**[00:58:19]** Tylko problem jest w tym, że za każdym razem większość ludzi

**[00:58:23]** tłumaczy wszystko do tego AI od początku,

**[00:58:27]** a to, że ludzie są leniwi, ja też jestem leniwy

**[00:58:30]** i nie chce mi się za każdym razem tłumaczyć wszystkiego,

**[00:58:33]** to powoduje, że mam gorsze wyniki, jeśli bym nie miał takiego systemu,

**[00:58:37]** gdzie nie mam zabranej wiedzy w jednym miejscu,

**[00:58:40]** nie mam tego kontekstu dobrze ustawionego i tak dalej.

**[00:58:43]** Więc to są najczęstsze problemy, że AI nie zna tego, co my mamy w głosie.

**[00:58:48]** Więc to są najczęstsze problemy, że AI nie zna tego, co my mamy w głosie.

**[00:58:50]** My byśmy chcieli, że my napiszemy jedno zdanie

**[00:58:53]** i od razu wszystko będzie pięknie,

**[00:58:54]** ale jak my tego dobrze nie opiszemy wcześniej,

**[00:58:56]** no to wyniki też są kiepskie, bo są brane ze statystyki.

**[00:58:59]** Przypominam, że AI to jest to technologia oparta trochę o statystyce.

**[00:59:06]** Prawdopodobieństwo, to jest lepsze słowo.

**[00:59:11]** I tu się właśnie pojawia luka, kto przygotuje firmę do realnej pracy z AI.

**[00:59:18]** Wiemy już, że nie muszą być to programiści.

**[00:59:20]** Ja też potrafię programować, ale dzisiaj już nie programuję.

**[00:59:23]** I dzisiaj największy mój skill to jest to, że potrafię łączyć kropki

**[00:59:28]** i ustawiać dobrze kontekst, tak bym powiedział.

**[00:59:31]** Plus jeszcze parę innych rzeczy.

**[00:59:34]** Więc dzisiaj to humaniści, czy też ludzie nietechniczni

**[00:59:37]** często będą mieli przewagę nad programistami.

**[00:59:41]** Gdybym powiedział to 5 lat temu, albo 3 lata temu,

**[00:59:45]** to by mnie wszyscy wyśmiali, zlinczowali.

**[00:59:47]** Co? Programiści?

**[00:59:51]** Dzisiaj to się dzieje, moi drodzy.

**[00:59:53]** I mam nadzieję, że część z Was już to dostrzega.

**[00:59:55]** Że specjaliści, którzy mają wiedzę domenową,

**[00:59:58]** często potrafią lepiej opisać dany problem

**[01:00:01]** i wrzucić go do AI niż osoby techniczne.

**[01:00:05]** Więc dzisiaj tak naprawdę drzwi stoją otworem przed osobami,

**[01:00:12]** które chcą się uczyć i chcą w ten świat AI wejść.

**[01:00:17]** Bo dzisiaj potrzebujemy ludzi, którzy będą potrafili uporządkować jakąś wiedzę.

**[01:00:21]** I zamienić ją w procesy.

**[01:00:23]** I przede wszystkim przygotować kontekst do tego AI.

**[01:00:28]** Więc taki szybki czek, sprawdzenie, czy ostatnie 50 minut,

**[01:00:34]** czy zgodzicie się, że to był dobrze spędzony dla Was czas.

**[01:00:38]** Dajcie znać na czacie.

**[01:00:40]** To też nam pomoże przygotowywać kolejne prezentacje.

**[01:00:43]** Wasz feedback bardzo szanujemy, stąd też o niego prosimy.

**[01:00:48]** Dobrze.

**[01:01:09]** Cieszymy się bardzo.

**[01:01:10]** Bardzo się cieszymy.

**[01:01:11]** Bardzo się cieszymy.

**[01:01:14]** Dziękuję bardzo.

**[01:01:22]** Dobra, dzięki wszystkim.

**[01:01:35]** Jakby coś, to możecie też dać znać, co Wam gdzieś szczególnie utrwiło w pamięci na czacie.

**[01:01:40]** Ja będę miał dla Was krótką propozycję.

**[01:01:44]** I mam tutaj pytanie, czy chcecie ją usłyszeć.

**[01:01:47]** Ale w sumie odpowiem sobie sam i pójdę dalej.

**[01:01:51]** Więc chcę Wam puścić taki krótki, krótki filmik.

**[01:01:55]** I ta propozycja zajmie dosłownie 15 minut maksymalnie.

**[01:01:57]** I po tym wszystkim będę miał dla Was ten prezent, który Wam obiecałem.

**[01:02:02]** Więc na początek króciutki filmik, który Wam zrobi takie wprowadzenie do tematu, o czym chcę odpowiedzieć.

**[01:02:09]** AI potrafi zrobić bardzo dużo, tylko jest jeden problem.

**[01:02:14]** Nie zna Twojej firmy.

**[01:02:16]** Nie wie, jak pracują zespoły, gdzie jest wiedza, a niektórym źródłom można ufać.

**[01:02:20]** AI operator rozmawia z zespołami, porządkuje wiedzę firmy, przygotowuje kontekst i pokazuje, które zadania naprawdę warto przekazać AI.

**[01:02:28]** Nie musisz być programistą, żeby wejść w tę rolę.

**[01:02:31]** Bo dziś humaniści i osoby z wiedzą domenową mogą być bardziej przydatni niż programiści, bo będą potrafić opisać dobrze AI kontekst firmy.

**[01:02:40]** A jeśli pracujesz w IT, możesz pójść dalej.

**[01:02:43]** Możesz tworzyć własne MCP i łączyć AI z systemami firmy.

**[01:02:47]** AI operator potrafi wziąć problem od zespołu i z pomocą AI samodzielnie dowieźć konkretny rezultat.

**[01:02:54]** Analizę, raport, stronę, prototyp albo usprawnienie prototypu.

**[01:02:58]** Wie jak przygotować kontekst, dobrać narzędzia i doprowadzić temat do czegoś, co zespół może wykorzystać.

**[01:03:05]** Na szkoleniu AI operators przez 5 tygodni nie tylko nauczysz się skutecznie korzystać z AI,

**[01:03:11]** ale zbudujesz projekt do portfolio, a co tydzień spotykamy się na żywo, żeby omówić Twoje pytania i postępy.

**[01:03:17]** Zapraszamy Cię serdecznie na pokład.

**[01:03:20]** Ok, więc przedstawiamy Wam dzisiaj program AI operators.

**[01:03:30]** Jest to 5 tygodniowy program edukacyjny, który poprowadzimy wspólnie z Olą.

**[01:03:37]** I dzisiaj otwieramy do niego przedsprzedaż.

**[01:03:40]** Będzie to program, który będzie uczyć jak projektować kontekst firmowy.

**[01:03:47]** Niezależnie od tego czy jesteście osobami technicznymi czy nietechnicznymi.

**[01:03:51]** Czy pracujecie w logistyce, marketingu, sprzedaży czy innych działach.

**[01:03:55]** To jest program dla osób, które są po prostu ciekawe tego świata AI.

**[01:03:59]** I chcą do tego świata wejść.

**[01:04:03]** Więc przed tym programem ja sobie wyobrażam, że osoba, która dzisiaj korzysta dorywczo z czata GPT,

**[01:04:10]** prosi go o jakieś pytanie, to to wystarczy, żeby wejść w to szkolenie.

**[01:04:16]** Nie potrzebujemy wcześniej jakiejś skomplikowanej wiedzy, aby przejść przez ten program.

**[01:04:21]** Ale skończymy go z umiejętnościami projektowania systemów AI, które będą znały Waszą pracę.

**[01:04:28]** Czy to Waszą osobiście, czy pracę jaką robicie na co dzień w firmie.

**[01:04:33]** I ten program kierujemy do dwóch grup osób.

**[01:04:36]** Do osób nietechnicznych, czyli osób, które chciałyby ułożyć procesy w firmie.

**[01:04:44]** I na przykład wejść do branży AI lub wyróżnić się wśród obecnego pracodawcy.

**[01:04:53]** I mamy też specjalną ścieżkę dla technicznych.

**[01:04:58]** Dla osób, które chciałyby budować jakieś własne integracje z istniejącymi systemami.

**[01:05:04]** Bo na przykład zależy Wam na bezpieczeństwie danych.

**[01:05:07]** Więc to będą dwie ścieżki. Jest nas dwóch prowadzących i dwie osoby będą odpowiadać za różne rzeczy.

**[01:05:13]** Więc jeśli chodzi o ścieżkę nietechniczną, tutaj za nią będzie odpowiadać Ola bardziej.

**[01:05:22]** Ja będę tylko gdzieś tam z boku.

**[01:05:26]** Tutaj zadbamy o to, aby to było w porządku.

**[01:05:27]** Tutaj zadbamy o to, aby to było w porządku.

**[01:05:28]** Żebyście wynieśli taką wiedzę jak porządkować firmowy kontekst i procesy.

**[01:05:35]** Usprawniać pracę swoją, ale także innych ludzi.

**[01:05:39]** Jak inicjować jakieś swoje projekty wewnątrz firmowe, żeby budować jakieś prototypy na potrzeby firmowe.

**[01:05:49]** A także jak zbudować sobie portfolio, jeśli chcecie wejść dopiero do branży AI.

**[01:05:54]** W ścieżce nietechnicznej nauczymy Was jak łączyć agentów z systemami firmy.

**[01:05:58]** Więc przede wszystkim zbudujemy własny serwer MCP, do którego podepniecie agenta i ten serwer MCP będzie zintegrowany z jakimiś Waszymi systemami firmowymi.

**[01:06:10]** To wszystko oczywiście z wykorzystaniem takich otwartych protokołów i standardów, jakie są obecnie na rynku.

**[01:06:19]** I to rozwiązanie będziecie w stanie wdrożyć w swojej pracy.

**[01:06:24]** I to jest jakby cel, za który ja odpowiadam w ścieżce dla technicznych osób.

**[01:06:28]** Będziemy budować coś, co realnie będziecie mogli wykorzystać w pracy.

**[01:06:34]** Więc szkolenie jest właśnie podzielone na takie dwie ścieżki, zarówno dla osób nietechnicznych i technicznych.

**[01:06:41]** Ale mamy też jeden wspólny fundament, czyli ustawianie kontekstu.

**[01:06:47]** I tutaj nad tym się będziemy najbardziej skupiać.

**[01:06:51]** Przejdę sobie troszkę szybciej przez ten slajd.

**[01:06:56]** I teraz opowiemy Wam.

**[01:06:57]** Co będzie Was czekać w konkretnym tygodniu.

**[01:07:00]** Bo będzie 5 tygodni.

**[01:07:02]** I teraz oddam głos Oli, żeby opowiedziała Wam co będzie w poszczególnych tygodniach.

**[01:07:10]** Na samym początku będziemy mieli tą właśnie wspólną bazę skierowaną i do osób technicznych i do nietechnicznych.

**[01:07:16]** I od pierwszych tygodni ja będę też mentorem.

**[01:07:21]** I ja tam postaram się Wam przekazać takie też zasady po prostu pracy z modelami językowymi.

**[01:07:26]** Ponieważ to jest moja specjalizacja.

**[01:07:29]** I od pierwszego tygodnia zaczniemy od wybrania procesów, które właśnie warto oddać.

**[01:07:35]** O tym, żebyście wiedzieli kiedy naprawdę...

**[01:07:38]** Teraz mieliście tego taki malutki przesmak.

**[01:07:41]** Kiedy wybrać proces deterministyczny, niedeterministyczny.

**[01:07:44]** Kiedy nadaje się właśnie rozwiązanie oparte o plot-code'a.

**[01:07:50]** Kiedy trzeba zrobić prototyp.

**[01:07:51]** Kiedy automatyzacja.

**[01:07:53]** Bo jak...

**[01:07:54]** Ja to...

**[01:07:55]** W zasadzie zaprojektowaliśmy to z taką myślą, że po prostu widzę co się dzieje w firmach.

**[01:08:01]** Nie zawsze będzie tak, że wszystko da się rozwiązać modelami językowymi.

**[01:08:05]** I po prostu trzeba być płynnym w tym.

**[01:08:08]** Więc pierwszy tydzień będzie skupiony na tym, żeby faktycznie dobrać dobre rozwiązanie do konkretnego przypadku.

**[01:08:18]** I kiedy zastosować te modele językowe i w jaki sposób.

**[01:08:23]** I na tym skupimy się w tygodniu pierwszym.

**[01:08:25]** Ok.

**[01:08:28]** To ja opowiem teraz może dla odmiany o tygodniu drugim.

**[01:08:31]** Więc w tygodniu drugim będziemy budować agentów.

**[01:08:37]** Czyli już będziemy oddawać jakieś powtarzalne zadania.

**[01:08:41]** Będą tu takie tematy jak MCP, jak skille.

**[01:08:45]** Czyli wszystkie te fundamenty, które dzisiaj każdy AI operator musi mieć.

**[01:08:50]** Będziemy uczyć się jak tworzyć skille od zera.

**[01:08:54]** Jak wykorzystywać istniejące serwery MCP.

**[01:08:56]** Tu jeszcze nie będziemy budować serwerów MCP, bo jest to troszkę bardziej skomplikowane.

**[01:09:02]** I to bym zostawił dla ścieżki technicznej.

**[01:09:04]** Ale to też taka ciekawostka, że osoby nietechniczne mają też dostęp do ścieżki technicznej.

**[01:09:10]** Bo nie rozdzielamy tego.

**[01:09:12]** Dostajecie dostęp do wszystkiego.

**[01:09:14]** Sami decydujecie w którą ścieżkę idziecie.

**[01:09:16]** Więc jak ktoś będzie ambitny z osób nietechnicznych to też będzie mógł skorzystać z tworzenia serwerów MCP.

**[01:09:24]** Tak, teraz tydzień trzeci.

**[01:09:28]** Czyli przekazywanie kontekstu.

**[01:09:31]** I tutaj będziemy faktycznie pracować nad tym, żeby dobrze ustawić ten tak zwany kontekst engineering.

**[01:09:41]** To jest umiejętność właśnie opisywania tych procesów dla modelu językowego.

**[01:09:47]** Będziemy mieli różne przykłady.

**[01:09:50]** I będziemy pokazywać jak właśnie też wersjonować ten kontekst.

**[01:09:55]** I tworzyć skille, które wspierają nam te procesy ustawiania kontekstu dla agenta.

**[01:10:02]** To jeszcze może Cię poproszę o czwarty tydzień.

**[01:10:10]** Tak, i czwarty tydzień to są bazy danych.

**[01:10:13]** Teraz też Wam pokazałam tego przedsmak.

**[01:10:15]** Ponieważ pokazałam Wam grafową bazę wiedzy.

**[01:10:18]** Ale tak naprawdę to zależy mi na szerszym pokazaniu tego.

**[01:10:22]** Ponieważ tworzenie bazy wiedzy dla agenta to nie tylko są grafy.

**[01:10:26]** I nie tylko są takie fajne kolorowe właśnie LLM brainy, mózgi.

**[01:10:29]** Ale też są systemy ragowe.

**[01:10:32]** Też są bardzo proste systemy ragowe, które da się robić bez tworzenia ich samemu.

**[01:10:38]** I po prostu chcę pokazać cały taki przekrój tego.

**[01:10:42]** Jak wygląda cały przekrój.

**[01:10:44]** Jaka może być baza wiedzy dla naszego agenta.

**[01:10:47]** Jaką może z niej korzystać.

**[01:10:49]** I które rozwiązanie mamy wybrać.

**[01:10:51]** No bo znowu taka jest potrzeba.

**[01:10:53]** To nie jest tak, że taki LLM brain jest rozwiązaniem na wszystko.

**[01:10:56]** Tylko jest konkretny przykład w firmie.

**[01:10:58]** Czy u Was prywatnie, czy w firmie dla której pracujecie.

**[01:11:01]** I nie zawsze LLM brain się nada.

**[01:11:03]** Czasami to będzie inne rozwiązanie.

**[01:11:05]** Więc po prostu żeby mieć taki przekrój i wiedzieć co zastosować.

**[01:11:10]** No i teraz przechodzimy już do konkretów dla poszczególnych ścieżek.

**[01:11:17]** Więc ja najpierw teraz opowiem o ścieżce dla technicznych.

**[01:11:21]** I za chwilę się cofniemy dla nietechnicznych.

**[01:11:23]** Więc w ścieżce dla osób technicznych.

**[01:11:25]** Zbudujemy bezpieczną warstwę.

**[01:11:27]** Zbudujemy bezpieczną warstwę między agentem AI a wewnętrznym API.

**[01:11:31]** Czy logami, czy dokumentacją firmową.

**[01:11:34]** Następnie wykorzystamy ją do sprawdzenia statusu systemów chociażby.

**[01:11:39]** Będzie to jakaś dobra wiedza dla devopsów.

**[01:11:42]** I nie tylko.

**[01:11:44]** Więc tu jaki problem rozwiążemy.

**[01:11:47]** Często gotowe integracje się kończą wtedy gdy zaczynają się jakieś wewnętrzne systemy firmowe.

**[01:11:53]** Mamy jakiś wewnętrzny system firmowy, który sami zbudowaliśmy.

**[01:11:56]** No i ciężko żeby mieć do tego jakiś gotowy konektor MCP.

**[01:12:00]** Dlatego też trzeba będzie się troszkę pogłowić i zbudować sobie na przykład taki serwer MCP.

**[01:12:06]** Aby połączyć agenta w sposób bezpieczny z istniejącym systemem.

**[01:12:10]** I tym się również zajmiemy właśnie w ścieżce dla technicznych w tygodniu piątym.

**[01:12:15]** A teraz przykład dla nietechnicznych.

**[01:12:18]** Oddaję Ci głos.

**[01:12:20]** Jeśli chodzi o przykład dla osób nietechnicznych.

**[01:12:22]** To tutaj zależy nam na tym żeby zrobić właśnie taki system.

**[01:12:26]** Który usprawni wewnętrzny proces w firmie.

**[01:12:28]** Na przykład właśnie taką analizę konkurencji.

**[01:12:31]** Tylko, że ten proces może być o wiele bardziej złożony.

**[01:12:35]** I chodzi tutaj też o to żeby mieć taki projekt dla osób, które chcą wejść do branży AI.

**[01:12:42]** I żeby mogły pokazać go w swoim portfolio.

**[01:12:45]** Ponieważ ja wiem, że jest bardzo wiele specjalistów.

**[01:12:49]** Którzy właśnie mają tą wiedzę ekspercką.

**[01:12:51]** I wiedzą, że jak dołożą do tego ten skill AI.

**[01:12:54]** To mogą wtedy na przykład ze swojej pozycji.

**[01:12:57]** Project managera, product managera, sprzedawcy.

**[01:13:00]** Czy może właśnie jakichś takich zawodów biznesowych.

**[01:13:04]** Wejść na rolę, która jest takim operatorem AI.

**[01:13:08]** Solution właśnie inżynierem.

**[01:13:11]** Czy product builderem.

**[01:13:13]** Jest bardzo wiele ludzi, które ma pokrewne umiejętności.

**[01:13:17]** I tu chodzi o to żebyście wy byli w stanie zrobić coś.

**[01:13:20]** Co będzie tym właśnie takim waszym projektem do portfolio.

**[01:13:22]** Że hej wziąłem moją wiedzę ekspercką.

**[01:13:24]** Zrobiłem rozwiązanie AI.

**[01:13:26]** I zobacz co mam w swoim CV teraz.

**[01:13:29]** I jakby ja naprawdę potrafię używać tego AI plus mojej wiedzy eksperckiej.

**[01:13:33]** Więc jakby tutaj celem będzie zrobić taki system.

**[01:13:38]** Ja tutaj tylko dodam, że ta analiza konkurencji jest tylko wybranym przykładem.

**[01:13:42]** Ponieważ w tym tygodniu skupimy się także na takich rzeczach.

**[01:13:47]** Jak prototyp aplikacji.

**[01:13:49]** Czyli osoba, product manager będzie w stanie zrobić szybki prototyp aplikacji.

**[01:13:53]** Która mogłaby usprawnić jakieś procesy wewnątrz firmowe.

**[01:13:58]** Nie będziemy tu oczywiście mówić o sprzedawaniu aplikacji, budowaniu pod sprzedaż.

**[01:14:02]** Bo jest to uważam na dzień dzisiejszy zarezerwany temat dla inżynierów, dla programistów.

**[01:14:07]** Więc nie mydlimy wam tu oczu, że nauczycie się budować aplikacje i potem je sprzedawać.

**[01:14:12]** Absolutnie nie.

**[01:14:13]** Chociaż wiem, że są w internecie ludzie, którzy w ten sposób mydlą oczy ludziom.

**[01:14:17]** I bardzo ich nie szanuję.

**[01:14:19]** To my wam tutaj pokażemy bardziej jak robić coś.

**[01:14:22]** Co możecie wykorzystać na potrzeby firmowe.

**[01:14:25]** Bo zbudowanie czegoś na potrzeby wewnętrzne, a udostępnienie tego do internetu.

**[01:14:31]** To są w ogóle dwie różne światy i dwie różne ścieżki.

**[01:14:35]** Więc nie będziemy tego robić.

**[01:14:37]** Ja też pokażę wam jak tworzyć strony internetowe.

**[01:14:42]** Za chwilę zobaczycie stronę AI Operators chociażby.

**[01:14:45]** Która gdzieś ostatnio była tworzona przez nas.

**[01:14:48]** I to też było tworzone z AI.

**[01:14:51]** Na podstawie dobrego kontekstu.

**[01:14:53]** Uwierzcie mi bardzo dobrego, rozwijanego już od ponad roku.

**[01:14:56]** No i też podzielę się tym doświadczeniem z wami.

**[01:15:00]** Jak tworzyć strony, które nie wyglądają jak AI generated.

**[01:15:03]** Tylko wyglądają jakby wyszły od designera.

**[01:15:06]** Więc to tyle pokrótce jeśli chodzi o program.

**[01:15:11]** Wszystkie szczegóły będą na stronie.

**[01:15:13]** Więc za chwilę wam je udostępnimy.

**[01:15:16]** I teraz jeśli ktoś ma jakieś pytania.

**[01:15:19]** W sensie takim, że nie wiem.

**[01:15:21]** Jest laikiem, boi się, że sobie nie poradzi.

**[01:15:23]** To mamy taki warunek.

**[01:15:28]** Mianowicie macie 7 dni na przetestowanie kursu.

**[01:15:31]** Przetestowanie naszego programu.

**[01:15:34]** Wbicie na spotkania z nami na żywo.

**[01:15:37]** Sprawdzenie czy to jest fajne czy nie.

**[01:15:39]** W razie czego możecie zwrócić 100% kasy, odzyskać.

**[01:15:43]** Więc jakby nie ma tu żadnego ryzyka, że kupicie.

**[01:15:46]** A potem się okaże, że sobie nie dacie rady.

**[01:15:48]** Natomiast przypominam, że też kierujemy ten program.

**[01:15:50]** Do nietechnicznych.

**[01:15:52]** Więc będzie to przedstawione w sposób taki.

**[01:15:55]** Aby osoba nietechniczna to zrozumiała.

**[01:15:58]** Jeśli boicie się, że nie macie wiedzy eksperckiej.

**[01:16:03]** Bo tutaj na przykład wymienialiśmy często.

**[01:16:05]** Że ktoś ma wiedzę domenową, ekspercką.

**[01:16:07]** I może zostać właśnie takim solution inżynierem.

**[01:16:10]** Czy coś w tym stylu.

**[01:16:12]** To też się nie bójcie.

**[01:16:14]** Jeśli na przykład wasza w tej chwili praca jest powtarzalna.

**[01:16:16]** To my wam zaproponujemy jakiś projekt.

**[01:16:19]** Tutaj w szkoleniu.

**[01:16:20]** Gdzie tą wiedzę będziecie mogli sobie przetestować.

**[01:16:25]** I tutaj też nie ma o to obaw.

**[01:16:29]** Jeśli wybieracie ścieżkę techniczną.

**[01:16:32]** To też nie ma dużych wymagań wstępnych.

**[01:16:35]** Proste rzeczy typu Bash, Git, API itd.

**[01:16:38]** Ale to podkreślam tylko dla ścieżki technicznej.

**[01:16:41]** Czy to wam się przyda z pracy?

**[01:16:45]** Możecie sobie pomyśleć.

**[01:16:46]** Więc jeśli z waszej pracy są jakieś informacje.

**[01:16:49]** A każda firma chyba ma informacje.

**[01:16:51]** Jakieś powtarzalne zadania.

**[01:16:53]** To na pewno macie co usprawniać.

**[01:16:55]** I będziecie mogli się wykazać.

**[01:16:57]** Jak nie macie pomysłu na swój projekt.

**[01:16:59]** To my wam podsuniemy taki pomysł.

**[01:17:01]** Który będziecie mogli zrobić.

**[01:17:03]** A jak będziecie mieli pomysł na swój.

**[01:17:05]** To jesteśmy happy żeby wam dać feedback.

**[01:17:07]** Jak to ogarnąć.

**[01:17:15]** Więc program wygląda w ten sposób.

**[01:17:17]** Że uczycie się wtedy kiedy macie czas.

**[01:17:19]** Jest to program dostosowany do osób pracujących na etacie.

**[01:17:21]** Którzy rano najczęściej są w pracy.

**[01:17:23]** I mają czas tylko popołudniami.

**[01:17:25]** Mamy też spotkania na żywo.

**[01:17:27]** Też w godzinach popołudniowych one będą.

**[01:17:29]** Ale dla osób które nie mogą być w danym dniu.

**[01:17:31]** To będzie nagrywane wszystko.

**[01:17:33]** I udostępnione.

**[01:17:35]** I przechodzicie to wszystko razem z grupą.

**[01:17:37]** Więc macie motywację.

**[01:17:39]** Nie odłożycie tego na półkę na pewno.

**[01:17:41]** Tylko będziecie pracować.

**[01:17:43]** Będziecie pracować z grupą.

**[01:17:45]** I wszystko razem z naszym wsparciem.

**[01:17:47]** Macie dostęp do forum.

**[01:17:49]** Do spotkań na żywo.

**[01:17:51]** Więc możecie liczyć na naszą pomoc.

**[01:17:53]** Poprzednie nasze programy.

**[01:17:55]** Z zadowoleniem.

**[01:17:57]** Kończyły osoby nietechniczne.

**[01:18:00]** Tu widzicie przykład Kasi.

**[01:18:02]** Która ukończyła jedno z naszych szkoleń.

**[01:18:04]** I było to szkolenie.

**[01:18:06]** Które pokrywało taką wiedzę.

**[01:18:08]** Też z AI.

**[01:18:10]** I Kasia tu mówi.

**[01:18:12]** Że wiedzę wcześniej zarezerwowaną dla programistów.

**[01:18:15]** Przełożyliście na język zrozumiały.

**[01:18:17]** Dla człowieka spoza branży IT.

**[01:18:19]** I to jest bardzo ważne.

**[01:18:21]** I to jest bardzo ważne.

**[01:18:23]** Więcej opinii znajdziecie na stronie.

**[01:18:25]** Ja tylko już podsumuję.

**[01:18:27]** I przechodzę do konkretów.

**[01:18:29]** Czyli do ceny.

**[01:18:31]** Natomiast zanim jeszcze.

**[01:18:33]** To przypomnę 7 dni gwarancji.

**[01:18:35]** Niezależnie od tego czy.

**[01:18:37]** Cokolwiek wam się nie spodoba.

**[01:18:39]** Czy na przykład będziecie potrzebować.

**[01:18:41]** Odzyskać pieniądze.

**[01:18:43]** To aż do 2 listopada możecie to zrobić.

**[01:18:45]** Program startuje nie teraz.

**[01:18:47]** Nie dzisiaj.

**[01:18:49]** Startuje w październiku.

**[01:18:51]** A dzisiaj mamy otwarcie projektu.

**[01:18:53]** Na najlepszą możliwą cenę.

**[01:18:55]** Najniższą jaką się tylko dało.

**[01:18:57]** I nigdy nie będzie taniej.

**[01:18:59]** Ale jeszcze dodatkowo możecie tą cenę rozłożyć.

**[01:19:01]** Nawet na 10 rat 0%.

**[01:19:03]** Mamy w koszyku pay uraty.

**[01:19:05]** Wszystko tam sobie wyklikujecie samodzielnie.

**[01:19:07]** Ja tylko podkreślę, że dzisiaj jest najlepszy moment.

**[01:19:09]** I ta cena nie wróci już nigdy.

**[01:19:11]** Bo zawsze będzie później drożej.

**[01:19:13]** Tak to działa.

**[01:19:15]** Przed sprzedaż jak kupujecie bilet na koncert.

**[01:19:17]** Wcześniej to macie taniej.

**[01:19:19]** Tak samo działa to u nas.

**[01:19:21]** Tyle.

**[01:19:23]** Nie będę się nad tym rozwodził.

**[01:19:25]** Mam jeden ważny temat.

**[01:19:27]** Potrzebujemy.

**[01:19:29]** Albo raczej określiliśmy sobie takie minimum.

**[01:19:31]** Że musi do nas dołączyć minimum 100 osób.

**[01:19:35]** Przed sprzedaży.

**[01:19:37]** Jeśli nie uzbieramy tych 100 osób.

**[01:19:39]** To anulujemy projekt całkowicie.

**[01:19:41]** Wszystkim którzy dołączyli.

**[01:19:43]** Oddajemy kasę.

**[01:19:45]** I się rozchodzimy.

**[01:19:47]** Ale wierzę, że ten limit przekroczymy.

**[01:19:49]** I to grubo.

**[01:19:51]** Ale gdyby nie.

**[01:19:53]** To tak jak mówiłem.

**[01:19:55]** Oddajemy 100% kasy.

**[01:19:57]** I nie ma żadnego problemu.

**[01:19:59]** Dodatkowo dla wszystkich osób.

**[01:20:01]** Które zdecydują się.

**[01:20:03]** Dzisiaj do północy.

**[01:20:05]** Na dołączenie.

**[01:20:07]** Będzie dodatkowy kurs online.

**[01:20:09]** Który udostępnimy wam we wrześniu.

**[01:20:11]** Będzie to kurs.

**[01:20:13]** Zbuduj głosowego asystenta AI.

**[01:20:15]** Który odbiera telefony.

**[01:20:17]** Potrafi odbierać połączenia.

**[01:20:19]** I możecie to nawet ustawić tak.

**[01:20:21]** Jest tam instrukcja.

**[01:20:23]** Jak na przykład przekierować.

**[01:20:25]** Takiego asystenta z iPhone'a.

**[01:20:27]** Czyli ktoś dzwoni na waszego iPhone'a.

**[01:20:29]** I odbiera wasz taki asystent AI.

**[01:20:31]** Takie rozwiązania.

**[01:20:34]** Dzisiaj są na rynku.

**[01:20:36]** Jakby.

**[01:20:38]** Już powoli standardem.

**[01:20:40]** I coraz więcej firm.

**[01:20:42]** Decyduje się na wdrożenie.

**[01:20:44]** I to nie jest taka sekretarka.

**[01:20:46]** Wciśnij jeden.

**[01:20:48]** To połącze cię z działem tym.

**[01:20:50]** Jakby to człowiek odbierał telefon.

**[01:20:52]** Podobnie.

**[01:20:54]** Bardzo podobnie.

**[01:20:56]** Oczywiście nie jest to człowiek.

**[01:20:58]** Ale brzmi to bardzo podobnie.

**[01:21:00]** Firmy dzisiaj za takie rozwiązania płacą.

**[01:21:02]** Między 500 złotych a 1200 złotych miesięcznie.

**[01:21:04]** Dzisiaj mi się wyświetliła reklama.

**[01:21:06]** Dwóch takich firm.

**[01:21:08]** Które oferują takie usługi.

**[01:21:10]** Nie będę tutaj reklamował.

**[01:21:12]** Ale możecie sobie poszukać.

**[01:21:14]** Jak wpiszecie w Google.

**[01:21:16]** To na pewno zobaczycie takie firmy.

**[01:21:18]** Za miesiąc.

**[01:21:20]** Oczywiście zależy od wolumenu połączeń.

**[01:21:22]** Jeszcze tutaj chciałam jedną rzecz powiedzieć.

**[01:21:24]** Że zawsze jak ktoś się mnie pytał.

**[01:21:26]** Jaki jest największy właśnie zwrot.

**[01:21:28]** Z inwestycji.

**[01:21:30]** Jak na przykład wybieracie sobie jakiś projekt.

**[01:21:32]** Do portfolio na przykład.

**[01:21:34]** Co firmy chętne są wdrażać.

**[01:21:36]** No to zawsze mówiłam.

**[01:21:38]** Że to jest asystent głosowy.

**[01:21:40]** Bo to właśnie łatwo.

**[01:21:42]** Bardzo dużo firm to chce na przykład restauracje.

**[01:21:44]** Salony beauty.

**[01:21:46]** Więc zawsze mówiłam.

**[01:21:48]** Że jeśli chcesz być publiczny.

**[01:21:50]** To taki asystent głosowy.

**[01:21:55]** To jest świetny wybór.

**[01:21:57]** Więc tak.

**[01:21:59]** Ten bonus dzisiejszy.

**[01:22:01]** To jeszcze raz przypomnę dla osób.

**[01:22:03]** Które dołączą do północy.

**[01:22:05]** Ten dodatkowy kurs online.

**[01:22:07]** I teraz tutaj jest pytanie od razu na czacie.

**[01:22:09]** Czy to dotyczy również Androida czy iPhone.

**[01:22:11]** Generalnie ja mam sprawdzone.

**[01:22:13]** Ja wiem że w iPhone się da przekierować połączenie.

**[01:22:15]** I można to zrobić z poziomu telefonu.

**[01:22:17]** Nie jestem pewien czy się da to zrobić.

**[01:22:19]** Z poziomu Androida.

**[01:22:21]** To mówię bo to przetestowałem.

**[01:22:23]** Na nie wiem.

**[01:22:25]** Strzelam że na 80% też się da.

**[01:22:27]** No bo dzisiaj Android to praktycznie ma wszystko.

**[01:22:29]** To co iPhone.

**[01:22:31]** Ale 100% pewności nie mam.

**[01:22:33]** W każdym bądź razie.

**[01:22:35]** Jesteś w stanie wykupić sobie dodatkowy numer specjalny.

**[01:22:37]** I po prostu jak ktoś zadzwoni pod ten numer telefonu.

**[01:22:39]** Bo o tym iPhone to ja mówię na tej zasadzie.

**[01:22:41]** Że masz swój numer telefonu.

**[01:22:43]** Który masz od lat zarejestrowany.

**[01:22:45]** I na ten numer kierujesz tego asystenta.

**[01:22:47]** I jak ktoś do ciebie dzwoni.

**[01:22:49]** To on odbiera.

**[01:22:51]** Natomiast jak chciałbyś to założyć.

**[01:22:53]** Na osobny numer telefonu.

**[01:22:55]** To niezależnie od tego czy masz Androida czy cokolwiek innego.

**[01:22:57]** To to zadziała.

**[01:22:59]** Jak weźmiesz nowy numer telefonu.

**[01:23:01]** I chcesz na przykład skonfigurować to dla jakiejś nowej firmy.

**[01:23:03]** Czy cokolwiek.

**[01:23:09]** Więc ten bonus dzisiaj do 23.

**[01:23:16]** Cena wygląda następująco.

**[01:23:18]** W przedsprzedaży najniższa możliwa cena.

**[01:23:20]** 995 zł netto.

**[01:23:22]** Plus podatek VAT.

**[01:23:24]** 23%.

**[01:23:26]** Wystawiamy faktury.

**[01:23:28]** 23% VAT.

**[01:23:30]** I wszystko.

**[01:23:32]** Przychodzi wam od razu po zakupie na maila.

**[01:23:34]** Przypominam.

**[01:23:36]** Zero ryzyka.

**[01:23:38]** Macie 7 dni gwarancji od startu.

**[01:23:40]** Czyli jak sprawdzicie materiały.

**[01:23:42]** Zobaczycie o co chodzi.

**[01:23:44]** Uznacie że to jest nie dla was.

**[01:23:46]** Albo że was wkurzamy.

**[01:23:48]** Albo wam nie pasujemy.

**[01:23:50]** To piszecie jednego maila.

**[01:23:52]** I w ciągu 3 dni roboczych odzyskujecie 100% kasy.

**[01:23:54]** Bo przelew wychodzi jeden dzień roboczy.

**[01:23:56]** Odczytamy maila.

**[01:23:58]** I najczęściej robimy to tego samego dnia.

**[01:24:00]** Ale dajemy sobie taki bufor.

**[01:24:02]** 3 dni robocze.

**[01:24:04]** Więc zapraszamy serdecznie.

**[01:24:07]** I teraz przechodzimy do sekcji pytań.

**[01:24:09]** I przechodzimy do obiecanego bonusu.

**[01:24:11]** Który też obiecaliśmy.

**[01:24:13]** Wrzucam tylko link na czat.

**[01:24:21]** I tutaj też zaznaczę od razu.

**[01:24:24]** Że tą przedsprzedaż nie ukrywam.

**[01:24:27]** Kierujemy do stałych klientów.

**[01:24:29]** Jak zawsze.

**[01:24:31]** Powiem szczerze że.

**[01:24:33]** W reklamę wrzuciliśmy dosłownie parę groszy.

**[01:24:35]** Jak na nasze standardy.

**[01:24:37]** Specjalnie po to żeby dołączyli.

**[01:24:39]** Nasi stali klienci.

**[01:24:41]** Stąd też nie przewidujemy tutaj żadnych rabatów.

**[01:24:43]** To jest najniższa możliwa cena.

**[01:24:45]** I ona nigdy się nie powtórzy.

**[01:24:47]** Zawsze będzie drożej.

**[01:24:55]** Jeszcze ważna uwaga.

**[01:24:57]** Jak ktoś już się zdecydował na dołączenie.

**[01:24:59]** To ten dostęp do tego kursu.

**[01:25:01]** O tym asystencie.

**[01:25:03]** Jaj będzie we wrześniu przydzielany.

**[01:25:05]** Postaramy się.

**[01:25:07]** Jak najszybciej to przydzielić.

**[01:25:09]** Ale to też zaznaczam.

**[01:25:11]** Że dzisiaj tego jeszcze nie będzie.

**[01:25:13]** Ale ten bonus jest tylko dzisiaj.

**[01:25:15]** Więc jutro jak ktoś będzie chciał dołączyć.

**[01:25:17]** To już go nie dostanie.

**[01:25:22]** Dobra to my przechodzimy do pytań.

**[01:25:24]** I zróbmy sobie dwa pytania.

**[01:25:26]** I rozdamy ten bonus.

**[01:25:28]** O który obiecaliśmy.

**[01:25:30]** Ja mam tutaj polajkowane.

**[01:25:32]** Zaznaczone pytania.

**[01:25:35]** Pytania.

**[01:25:37]** Do części merytorycznej.

**[01:25:39]** Więc Ola.

**[01:25:41]** Pytanie do Ciebie.

**[01:25:43]** Tutaj było w trakcie prezentacji.

**[01:25:45]** Dlaczego Obsidian?

**[01:25:47]** I czy może być coś innego?

**[01:25:49]** Może być coś innego.

**[01:25:51]** Zdecydowanie jest dużo rozwiązań grafowych.

**[01:25:53]** To nie jest jedyna.

**[01:25:55]** Jest w ogóle cała masa.

**[01:25:57]** Tak samo jak wektorowych baz danych.

**[01:25:59]** Wybrałam Obsidian dlatego.

**[01:26:01]** Że chciałam Wam zobrazować koncept.

**[01:26:03]** I on jest bardzo dobrze dostępny.

**[01:26:05]** Na szkoleniu też.

**[01:26:07]** Obsidiana na pewno.

**[01:26:09]** Też dlatego, że to rozwiązanie jest darmowe.

**[01:26:11]** I żeby nie generować.

**[01:26:13]** Niepotrzebnych kosztów.

**[01:26:15]** Więc.

**[01:26:17]** Wybór był głównie po to.

**[01:26:19]** Żeby pokazać Wam.

**[01:26:21]** Zobrazować Wam koncept.

**[01:26:23]** I dobrze go wytłumaczyć.

**[01:26:25]** A to narzędzie pozwala na to też wizualnie.

**[01:26:27]** Więc też taka moja preferencja była.

**[01:26:29]** Ale nie ma tutaj jakiejś takiej.

**[01:26:31]** Przewagi wielkiej.

**[01:26:33]** Bo ja też mam takie podejście do tych narzędzi.

**[01:26:35]** Że bardzo często jest tak, że.

**[01:26:37]** Jak na przykład pracujecie w firmie.

**[01:26:39]** To nie będziecie mogli za bardzo.

**[01:26:41]** Wybrać sobie czegoś co lubicie bardziej.

**[01:26:43]** Albo nie bardziej.

**[01:26:45]** Tylko czasami są pewne ograniczenia.

**[01:26:47]** Czasami jedno rozwiązanie jest lepsze do danego use case.

**[01:26:49]** Więc ja nigdy staram się tak nie podchodzić.

**[01:26:51]** Do tego na zasadzie, że coś jest lepsze, gorsze.

**[01:26:53]** Dlatego, że.

**[01:26:55]** To bardzo mocno zależy od tego jaki macie przypadek.

**[01:26:57]** I do czego musicie to użyć.

**[01:26:59]** I bardzo wiele rozwiązań.

**[01:27:01]** Daje nam to samo.

**[01:27:03]** Bo wiadomo nawet jest wiecie.

**[01:27:05]** Jak używamy kod koda a kodeksa.

**[01:27:07]** Niektóre firmy nie mają w ogóle dostęp do kod koda.

**[01:27:09]** I muszą używać copilota.

**[01:27:11]** I tu nie o to chodzi tak naprawdę.

**[01:27:13]** Nie chodzi o model.

**[01:27:15]** Tak jak to mówił Damian na początku.

**[01:27:17]** Tylko chodzi o sposób pracy.

**[01:27:19]** Więc narzędzie jest drugorzędne.

**[01:27:23]** To tu jest jeszcze pytanie.

**[01:27:25]** Też w trakcie prezentacji padło.

**[01:27:29]** Czy ten graf się robi sam?

**[01:27:32]** Czy trzeba mu go.

**[01:27:34]** Czy LLM robi sam ten graf?

**[01:27:36]** Czy trzeba mu jakoś dostarczyć?

**[01:27:38]** LLM robi.

**[01:27:40]** Ale trzeba dostarczyć LLM-owi dobrze opisany sposób i kontekst.

**[01:27:42]** Ale LLM go dla ciebie zrobi.

**[01:27:44]** Nie robi się go samemu.

**[01:27:46]** Czyli po prostu dosłownie daje się LLM-owi pliki.

**[01:27:48]** Które są w folderze.

**[01:27:50]** Daje się dostęp do folderu.

**[01:27:52]** I musisz po prostu w dobry sposób to.

**[01:27:54]** Przedstawić ten kontekst.

**[01:27:56]** I wtedy LLM robi go dla ciebie.

**[01:27:59]** Rozumiem, że w szkoleniu AI Operators.

**[01:28:01]** Będzie to wytłumaczone.

**[01:28:03]** Krok po kroku.

**[01:28:05]** Dokładnie.

**[01:28:07]** Długo by było żeby to wyjaśnić.

**[01:28:09]** Ale tak będzie to dokładnie opisane.

**[01:28:11]** Dobra.

**[01:28:14]** Tak jak obiecałem.

**[01:28:16]** Dwa pytania poszły.

**[01:28:21]** Wrzucam teraz.

**[01:28:23]** Ten poradnik o który Kamil prosi.

**[01:28:25]** Ten bonus.

**[01:28:27]** Więc już teraz wam to wrzucam na czat.

**[01:28:29]** I jest on do odebrania dla was.

**[01:28:31]** Już kopię link.

**[01:28:34]** Więc link macie na czacie.

**[01:28:37]** I jest to.

**[01:28:39]** To co obiecywałem od początku.

**[01:28:41]** A my lecimy z kolejnymi pytaniami.

**[01:28:57]** Jeśli macie jeszcze jakieś pytania.

**[01:28:59]** O sam program.

**[01:29:03]** To też zachęcamy.

**[01:29:05]** My tutaj mamy zebraną.

**[01:29:07]** Sporą ilość pytań.

**[01:29:10]** Jeszcze w trakcie prezentacji.

**[01:29:13]** Tu jest pytanie takie.

**[01:29:16]** Czy da się jakoś pobierać te dane.

**[01:29:18]** By mogły się aktualizować codziennie.

**[01:29:20]** By być na bieżąco ze zmienami.

**[01:29:22]** To podejrzewam, że chodzi o.

**[01:29:24]** O takie update'owanie.

**[01:29:27]** Dane tych agencji chyba.

**[01:29:29]** Tak, tak, tak.

**[01:29:31]** Oczywiście da się to.

**[01:29:33]** Da się ustawić to żeby się w ogóle.

**[01:29:35]** Automatycznie wszystko pobierały te dane.

**[01:29:37]** Jeśli masz jakieś miejsca.

**[01:29:39]** Z których chcesz je pobierać.

**[01:29:41]** Czy to są dostępy do wewnętrznych narzędzi firmowych.

**[01:29:43]** Czy pobieranie z internetu.

**[01:29:45]** To jak najbardziej.

**[01:29:47]** Da się w ogóle całkowicie zautomatyzować ten proces.

**[01:29:49]** Żeby one się właśnie automatycznie pobierały.

**[01:29:51]** I ta baza usprawniła się sama.

**[01:29:53]** To pytanie od Agnieszki.

**[01:29:56]** Więc odpowiemy od razu.

**[01:29:58]** Czy można kurs zrobić wcześniej niż w październiku.

**[01:30:00]** To jest taki.

**[01:30:02]** Program edukacyjny.

**[01:30:04]** W którym uczymy się.

**[01:30:06]** Też na spotkaniach na żywo.

**[01:30:08]** Więc to jest tak, że to startuje.

**[01:30:10]** W październiku.

**[01:30:12]** I w trakcie tego.

**[01:30:14]** Tego intensywnego sprintu.

**[01:30:16]** Są dodatkowe spotkania.

**[01:30:18]** Jest dodatkowe nasze wsparcie.

**[01:30:20]** Też jest taka motywacja.

**[01:30:22]** Dzięki temu żeby to ukończyć.

**[01:30:27]** Mamy już z powodzeniem przeprowadzony program.

**[01:30:29]** Poprzedni dla programistów.

**[01:30:31]** Z wykorzystaniem AI.

**[01:30:33]** I to się bardzo dobrze sprawdziło.

**[01:30:35]** Ponieważ.

**[01:30:37]** Mamy wysoki poziom ukończeń tych szkoleń.

**[01:30:39]** Czyli ludzie po prostu.

**[01:30:41]** Nie odkładają tych szkoleń na półkę.

**[01:30:43]** Tylko je przerabiają.

**[01:30:45]** A na tym nam zależy żebyście.

**[01:30:47]** Tu i teraz.

**[01:30:49]** Jakąś wiedzę wynieśli.

**[01:30:51]** Bo jak się kupuje kolejne kursy.

**[01:30:53]** To ja wiem sam z praktyki.

**[01:30:55]** Jak to jest od razu dostępne.

**[01:30:57]** Wejdę a tam jest 150 filmików.

**[01:30:59]** I 150 wideo.

**[01:31:01]** To jest za dużo.

**[01:31:03]** Za dużo dla mnie.

**[01:31:05]** I najczęściej to ląduje na półce wstydu.

**[01:31:07]** A tutaj mam nadzieję.

**[01:31:09]** Że tak nie będzie.

**[01:31:11]** Bo będzie to wszystko prowadzone w taki sposób.

**[01:31:13]** Żebyście.

**[01:31:15]** Mieli też motywację do tego.

**[01:31:18]** Żeby to ukończyć.

**[01:31:20]** Razem z całą grupą.

**[01:31:23]** I też grupa nakręca się.

**[01:31:25]** Bo jak idzie cała grupa.

**[01:31:27]** To też.

**[01:31:29]** Nie tylko jesteśmy my jako mentorzy.

**[01:31:31]** Ale są też inni ludzie.

**[01:31:33]** Którzy dzielą się swoim feedbackiem.

**[01:31:35]** Co tam udało się skończyć.

**[01:31:37]** I mamy to po prostu już przetestowane.

**[01:31:39]** Sprawdzane na innym programie.

**[01:31:41]** Tylko ten program był kierowany do programistów.

**[01:31:43]** I mamy to przetestowane.

**[01:31:45]** I w ten sam sposób to będzie realizowane.

**[01:31:51]** Tutaj Ola do ciebie pytanko.

**[01:31:55]** Możesz traktować.

**[01:31:57]** Cloud Master Class jako podstawę.

**[01:31:59]** A to będzie bardzo rozszerzone.

**[01:32:01]** Więc nie będzie to powtórzenie.

**[01:32:04]** Tego samego.

**[01:32:06]** A już na pewno nie Cloud Content.

**[01:32:09]** Bo takie materiały.

**[01:32:11]** Tam w ogóle nie będzie.

**[01:32:13]** Jeśli chodzi o Cloud Business.

**[01:32:15]** To możesz traktować.

**[01:32:17]** Jako taką bardzo dużą podstawę.

**[01:32:21]** Cały kurs będzie prowadzony.

**[01:32:23]** Na platformie Circle.

**[01:32:25]** Która jest bardzo wygodna.

**[01:32:27]** Ma super aplikację mobilną.

**[01:32:29]** Wszyscy ogólnie chwalą tą platformę.

**[01:32:31]** Jeśli ktoś ma nasze inne szkolenia.

**[01:32:33]** I nie była to ewolucja dewelopera.

**[01:32:35]** Bo ewolucja też była na Circle.

**[01:32:37]** To to właśnie jest zmiana.

**[01:32:39]** Będzie to właśnie na platformie Circle.

**[01:32:41]** Jest tam chat.

**[01:32:43]** Są live.

**[01:32:45]** Wszystko tam macie w jednym miejscu.

**[01:32:47]** Ogłoszenia, dyskusje.

**[01:32:49]** Fajny podział.

**[01:32:51]** Jakby tej wiedzy.

**[01:32:53]** Na różne materiały.

**[01:32:55]** Czy to tekstowe, graficzne.

**[01:32:57]** Video, quizy.

**[01:32:59]** Także jest to nowoczesna platforma.

**[01:33:01]** Dostosowana do 2.26.

**[01:33:03]** I tam to się będzie wszystko.

**[01:33:05]** Wszystko odbywać.

**[01:33:07]** Przypominam, że będą te spotkania na żywo.

**[01:33:09]** Że to też wyróżnia.

**[01:33:11]** Kurs online kolejny jak na Udemy.

**[01:33:13]** Czy gdziekolwiek indziej.

**[01:33:15]** Tylko na tych spotkaniach my będziemy.

**[01:33:17]** Nie nasze klony AI tylko my.

**[01:33:19]** I będziemy wam pomagać.

**[01:33:21]** Czy serwer MCP.

**[01:33:27]** Tutaj domyślam się Marcin.

**[01:33:29]** Że pytasz o ścieżkę dla technicznych.

**[01:33:31]** To też podkreślę, że.

**[01:33:33]** Jeśli o to pytasz.

**[01:33:35]** Jak nie to sprostuj mnie proszę.

**[01:33:37]** Odniosę się do ścieżki dla technicznych.

**[01:33:39]** Więc ja wykryłem sobie taki problem.

**[01:33:41]** I to też wyszło z moich use case.

**[01:33:43]** Podczas rozwoju swoich.

**[01:33:45]** Aplikacji SAS.

**[01:33:47]** Że napotkałem problem.

**[01:33:49]** Z połączeniem.

**[01:33:51]** Z połączeniem AI.

**[01:33:53]** Z moimi wewnętrznymi systemami.

**[01:33:55]** Gdzie np. nie było gotowego MCP.

**[01:33:57]** Serwera.

**[01:33:59]** Trzeba było coś szyć.

**[01:34:01]** I tak samo jest w firmach.

**[01:34:03]** Które mają wewnętrzne systemy różne.

**[01:34:05]** Napisane albo nie udostępnione.

**[01:34:07]** Na zewnątrz.

**[01:34:09]** No i po prostu trzeba coś dorobić.

**[01:34:11]** Jakiś plugin do tego wszystkiego.

**[01:34:13]** I bezpiecznie tam wpuścić agenta.

**[01:34:15]** Albo nie narobił kuku.

**[01:34:17]** Czyli zadbać o to żeby agent np.

**[01:34:19]** Miał dostęp tylko read-only itd.

**[01:34:21]** Więc będziemy się takimi tematami.

**[01:34:23]** W ścieżce dla technicznych zajmować.

**[01:34:25]** I nie będzie tutaj tworzenia aplikacji programowania.

**[01:34:27]** Tylko tak jak np. jest w evolucji.

**[01:34:29]** Tylko tutaj będziemy bardziej robić takie rzeczy.

**[01:34:31]** Dla admina.

**[01:34:33]** Dla devopsa.

**[01:34:35]** Programista też oczywiście skorzysta.

**[01:34:37]** Ale to są takie rzeczy bardziej.

**[01:34:39]** Do usprawniania pracy zespołu IT.

**[01:34:41]** Niż budowania aplikacji.

**[01:34:49]** Jeszcze raz poproszę o nazwę.

**[01:34:51]** Platformy.

**[01:34:53]** Może mój angielski nie jest rewelacyjny.

**[01:34:55]** Więc napiszę na czacie.

**[01:34:57]** Circle.

**[01:34:59]** Tak to jest kółko.

**[01:35:01]** Circle.

**[01:35:03]** No to taka platforma kursowa.

**[01:35:05]** Ja też robiłam w zeszłym roku na niej.

**[01:35:07]** Jedno szkolenie kohortowe.

**[01:35:09]** I to się sprawdza bardzo dobrze.

**[01:35:11]** Także zgadzam się z tym.

**[01:35:16]** Że to jest najlepsza platforma dostępna na rynku.

**[01:35:18]** Do tego typu formatu.

**[01:35:22]** Tu się domyślam.

**[01:35:24]** Że chodzi o programowanie stricte.

**[01:35:26]** Kojarzę tą metodykę.

**[01:35:29]** Więc generalnie.

**[01:35:31]** My się nie będziemy skupiać na tworzeniu aplikacji.

**[01:35:33]** Za bardzo w tym szkoleniu.

**[01:35:35]** Prototypy tylko dla osób nietechnicznych.

**[01:35:37]** Więc w ścieżce dla nietechnicznych.

**[01:35:39]** Będziemy uczyć.

**[01:35:41]** Jak tworzyć prototypy.

**[01:35:43]** I gdzieś tam szybko je może wdrożyć.

**[01:35:45]** Testowo.

**[01:35:47]** Ale nie będziemy się skupiać.

**[01:35:49]** Na takim pełnym.

**[01:35:51]** AI Assisted Engineering.

**[01:35:53]** To jest przekazywane w ewolucji dewelopera.

**[01:35:55]** Tak.

**[01:36:03]** Przewidzieliśmy rabaty dla zespołów.

**[01:36:05]** Prosimy o kontakt mailowy.

**[01:36:07]** Zamieszczę na czacie.

**[01:36:23]** Czy na kursie będą omawiane kwestie.

**[01:36:25]** Bezpieczeństwa pracy na danych firmach.

**[01:36:27]** Oczywiście, że tak.

**[01:36:29]** Nie może tego zabraknąć.

**[01:36:31]** To jest fundament dzisiaj.

**[01:36:33]** Patrząc na kolejne wycieki.

**[01:36:35]** Nie wiem czy słyszeliście ostatnio.

**[01:36:37]** Jak wyciekły dane z jakiegoś systemu.

**[01:36:39]** Gdzie poleciały Pesele chyba 19 milionów osób.

**[01:36:41]** To to.

**[01:36:43]** Dzisiaj.

**[01:36:45]** Dzisiaj jest praktycznie.

**[01:36:47]** Na samej górze listy priorytetów.

**[01:36:49]** W pracy z AI.

**[01:36:51]** I ogólnej pracy przy komputerze.

**[01:36:53]** Ja bym tak powiedział.

**[01:36:55]** Bo ten incydent pokazuje.

**[01:36:57]** Że dzisiaj dane.

**[01:36:59]** Dane to są po prostu.

**[01:37:01]** Narażone na wyciek.

**[01:37:03]** W każdej chwili.

**[01:37:05]** A taki wyciek prowadzi do różnych konsekwencji.

**[01:37:07]** Tutaj jest podobne pytanie.

**[01:37:17]** Więc już nie będziemy.

**[01:37:19]** Drugi raz chyba odpowiadać.

**[01:37:34]** Idę sobie do kolejnych pytań.

**[01:37:36]** Tu jest znowuże pytanie.

**[01:37:47]** O bezpieczeństwo.

**[01:37:51]** Wiesz co.

**[01:37:53]** Zależy na jakich danych pracujesz.

**[01:37:55]** I tutaj generalnie.

**[01:37:57]** Pytanie jest.

**[01:38:00]** Czy twoja.

**[01:38:02]** Czy firma dla której pracujesz.

**[01:38:04]** Czy ona np.

**[01:38:06]** Ma cloda wewnętrznie.

**[01:38:08]** Ja zakładam że w bardzo wielu korporacjach.

**[01:38:10]** Jest tak że albo.

**[01:38:12]** Trzeba skorzystać jednak z tej.

**[01:38:14]** Subskrypcji którą macie.

**[01:38:16]** Wykupioną no bo wtedy.

**[01:38:18]** Oni pewnie korzystają z.

**[01:38:20]** Konkretnych serwerów w Europie.

**[01:38:22]** Jeśli to jest Microsoft.

**[01:38:24]** Ale tutaj chcemy też zaznaczyć.

**[01:38:26]** Że klockot nie będzie.

**[01:38:28]** Jedynym rozwiązaniem.

**[01:38:30]** O którym będziemy opowiadać.

**[01:38:32]** Bo my chcemy przekazać.

**[01:38:34]** Sposób pracy.

**[01:38:36]** Który jest niezależny od tego.

**[01:38:38]** Czy ty masz w firmie.

**[01:38:40]** Kodeksa koda.

**[01:38:42]** Co pilota.

**[01:38:44]** Więc to będzie głównym celem.

**[01:38:49]** Tak dokładnie tak.

**[01:38:51]** I tutaj jest jeszcze.

**[01:38:53]** Też fajne pytanie.

**[01:38:56]** Ja jeszcze dopowiem.

**[01:38:58]** Zanim przełączymy się na kolejne.

**[01:39:00]** Nie traktujcie tego szkolenia.

**[01:39:02]** Jako przywiązanie się do cloda.

**[01:39:04]** Czy do czata.

**[01:39:06]** Bo szkolenie będzie agnostyczne.

**[01:39:08]** Jeżeli w waszej firmie.

**[01:39:10]** Macie copailota.

**[01:39:12]** To będziecie mogli sobie korzystać.

**[01:39:14]** W trakcie szkolenia z copailota.

**[01:39:16]** W ogóle nie wiem.

**[01:39:18]** Kupować specjalnie cloda.

**[01:39:20]** Bo to nie jest kurs cloda.

**[01:39:22]** To jest szkolenie o tym.

**[01:39:24]** Jak budować systemy.

**[01:39:26]** Jak ustawiać kontekst.

**[01:39:28]** I po prostu być tym AI operatorem.

**[01:39:30]** A taki AI operator.

**[01:39:32]** Jest w stanie pracować.

**[01:39:34]** Niezależnie od narzędzia.

**[01:39:36]** I też wam pokażemy.

**[01:39:38]** Te różnice między narzędziami.

**[01:39:40]** Jakie są niuanse.

**[01:39:42]** Między np. kodeksem a clodem.

**[01:39:44]** Czy copilotem.

**[01:39:49]** Tak.

**[01:39:53]** Można zadawać.

**[01:39:55]** I jeszcze ciekawostka.

**[01:39:57]** Mamy taki proces.

**[01:39:59]** Jak ktoś nie może być na spotkaniu.

**[01:40:01]** To pisze na czacie.

**[01:40:03]** Przed spotkaniem.

**[01:40:05]** I odpowiadamy w trakcie spotkania.

**[01:40:07]** Potem sobie odsłuchuje nagranie.

**[01:40:14]** Bo szkolenia są nagrywane.

**[01:40:16]** Czy szkolenie będzie praktyczne.

**[01:40:18]** Dla przedsiębiorców.

**[01:40:20]** Którzy chcą zautomatyzować.

**[01:40:22]** Powtarzalne procesy.

**[01:40:24]** Dla swojej firmy.

**[01:40:26]** I ten kontekst.

**[01:40:28]** Który buduje sobie już od roku.

**[01:40:30]** To dzisiaj pozwala mi.

**[01:40:32]** Powiem to zupełnie szczerze.

**[01:40:34]** Pracować nad trzema różnymi projektami.

**[01:40:36]** Jednocześnie.

**[01:40:38]** I tak najczęściej wygląda mój dzień pracy.

**[01:40:43]** Więc jak najbardziej tak.

**[01:40:45]** Ja tutaj mogę się podzielić.

**[01:40:47]** Będę się dzielił.

**[01:40:49]** Bo to też będzie w czwartym tygodniu.

**[01:40:51]** Budowa landing page.

**[01:40:53]** Budowa prototypu w aplikacji.

**[01:40:55]** Jakby łączenie się.

**[01:40:57]** Chyba w drugim Ola będzie MCP.

**[01:40:59]** Więc tam pokażemy jak na przykład.

**[01:41:01]** Łączyć się przez MCP.

**[01:41:03]** Z jakimiś różnymi systemami.

**[01:41:05]** Co pozwoli Ci na przykład.

**[01:41:07]** Wykonać jakieś powtarzalne zadania za Ciebie.

**[01:41:09]** Czyli po prostu agent będzie klikał Ci.

**[01:41:11]** Po jakiejś stronie.

**[01:41:13]** Ty będziesz to mogła obserwować.

**[01:41:15]** Jak on klika.

**[01:41:17]** Albo po prostu odejść od komputera.

**[01:41:19]** I jak wyklika to wrócić.

**[01:41:21]** Więc to też będzie.

**[01:41:24]** No ja też z tego korzystam na co dzień.

**[01:41:26]** Z przedsiębiorcami.

**[01:41:28]** Którzy są AI native.

**[01:41:30]** Bo ja też tylko pracuję.

**[01:41:32]** Z cold codem.

**[01:41:34]** Więc wiemy z jakimi problemami się borykacie.

**[01:41:36]** Będą też takie case.

**[01:41:38]** Które będą dla Was użyteczne.

**[01:41:40]** Tylko po prostu.

**[01:41:42]** Ja tu też mam taki background.

**[01:41:44]** Że pracowałam jako AI inżynier.

**[01:41:46]** Przy różnych projektach.

**[01:41:48]** Więc osoby które pracują na etacie.

**[01:41:50]** Mogę się z nimi też utożsamić.

**[01:41:52]** Więc mam jedną i drugą stronę.

**[01:41:54]** Przedsiębiorczynią.

**[01:41:56]** Od dwóch lat.

**[01:42:00]** Czy dla technicznych i nietechnicznych.

**[01:42:02]** Cena jest taka sama.

**[01:42:04]** W przedsprzedaży dajemy dostęp do wszystkiego.

**[01:42:06]** W tej samej cenie.

**[01:42:08]** Zobaczymy jak będzie później.

**[01:42:10]** Przedsprzedaż to jest duże zaufanie też.

**[01:42:12]** Więc my oddzięczamy się tym.

**[01:42:14]** Dajemy dostęp do wszystkiego.

**[01:42:16]** Do obu ścieżek.

**[01:42:18]** A to jest też dobre.

**[01:42:20]** Nie tylko dla osób technicznych.

**[01:42:22]** Ale uważam, że dla nietechnicznych jest spoko.

**[01:42:24]** Możemy wbić w te materiały.

**[01:42:26]** Dla technicznych.

**[01:42:28]** I zobaczyć na ile je rozumiemy.

**[01:42:30]** A może jak nóż będziemy rozumieć wszystko.

**[01:42:32]** I nauczymy się jeszcze więcej.

**[01:42:34]** Niż się spodziewaliśmy.

**[01:42:36]** Dostęp do materiałów.

**[01:42:39]** Macie na 12 miesięcy.

**[01:42:41]** Jak przejdziecie sobie przez swoją ścieżkę nietechniczną.

**[01:42:43]** Bo zakładam, że.

**[01:42:48]** Znaczy nie zakładam nic.

**[01:42:50]** Jeszcze raz przeczytam komentarz.

**[01:42:52]** Więc możecie przejść przez jedną i drugą.

**[01:42:56]** Techniczny to nie jest rozwinięty.

**[01:42:58]** Nie.

**[01:43:00]** Techniczny to nie jest rozwinięty kurs dla nietechnicznych.

**[01:43:02]** Tam są po prostu inne tematy poruszone.

**[01:43:04]** Inne case.

**[01:43:06]** Bo dla nietechnicznych na przykład będziemy bardziej robić coś w stylu.

**[01:43:08]** Nie wiem.

**[01:43:10]** Analiza konkurencji.

**[01:43:12]** Przestzelam.

**[01:43:14]** A dla technicznych będziemy robić na przykład własny serwer MCP.

**[01:43:16]** Żeby połączyć go z istniejącymi narzędziami firmowymi.

**[01:43:18]** Czy procesami.

**[01:43:28]** Jak zapłacisz kartą to raczej tak.

**[01:43:30]** Bo jest płatność kartą.

**[01:43:32]** Mamy w systemie płatność kartą przez Stripe.

**[01:43:34]** Więc w koszyku.

**[01:43:36]** Wybierz proszę płatność za pośrednictwem Stripe.

**[01:43:40]** I tam jest płatność kartą.

**[01:43:42]** I można jak najbardziej zapłacić kartą.

**[01:43:44]** Co tydzień będą spotkania.

**[01:44:14]** Patrzę sobie jeszcze na pytania z poprzedniej części.

**[01:44:25]** Tu jest jeszcze pytanie chyba do części tej.

**[01:44:27]** Merytorycznej.

**[01:44:37]** Na obecną chwilę powstają sasy na wszystko.

**[01:44:39]** Więc.

**[01:44:41]** Może już ktoś zrobił.

**[01:44:43]** Może już ktoś zrobił.

**[01:44:45]** Jak najbardziej.

**[01:44:47]** Ale słuchajcie.

**[01:44:49]** To jest tak, że macie jakiś proces w firmie.

**[01:44:51]** I jest 99% szans.

**[01:44:53]** Że albo już jest firma, która jest całkiem rozwinięta.

**[01:44:55]** Albo ktoś próbuje to zrobić.

**[01:44:57]** Jakby z obecnym.

**[01:44:59]** Takim wiecie.

**[01:45:01]** Niskim progiem wejścia.

**[01:45:03]** Po prostu ludzie naprawdę.

**[01:45:05]** Niskim progiem wejścia do AI.

**[01:45:07]** Obniżył się próg budowania właśnie software'u.

**[01:45:09]** Po ich sił.

**[01:45:11]** Więc powstają aplikacje absolutnie na wszystko.

**[01:45:13]** Więc możliwe, że już ktoś to zrobił.

**[01:45:15]** Tylko pytanie na ile ta aplikacja jest użyteczna.

**[01:45:17]** Tylko pytanie na ile ta aplikacja jest użyteczna.

**[01:45:19]** A tutaj nie chodzi w zasadzie o to,

**[01:45:21]** A tutaj nie chodzi w zasadzie o to,

**[01:45:23]** że jakiś case jest już zrobiony przez.

**[01:45:25]** Jest już zaadresowany przez jakiś software.

**[01:45:27]** No bo tak jak mówię.

**[01:45:29]** Wszystko jest już zaadresowane przez jakiś software.

**[01:45:31]** Tylko chodzi o to, żebyście wy się nauczyli.

**[01:45:33]** Tylko chodzi o to, żebyście wy się nauczyli.

**[01:45:35]** Zmieniać pomysły w.

**[01:45:37]** Zmieniać pomysły w.

**[01:45:39]** Namacalnego co można przetestować.

**[01:45:41]** To chodzi o ten skill.

**[01:45:43]** Że wy nie musicie czekać na zespół techniczny.

**[01:45:45]** Żeby coś wykonać.

**[01:45:47]** Tylko możecie zrobić to sami.

**[01:45:49]** I to jest też w ogóle taka umiejętność.

**[01:45:51]** Że jak nawet sami będziecie mieli jakikolwiek pomysł na coś.

**[01:45:53]** Jeśli na przykład pracujecie na etacie.

**[01:45:55]** A będziecie chcieli w przyszłości robić biznes.

**[01:45:57]** A będziecie chcieli w przyszłości robić biznes.

**[01:45:59]** To żeby sobie po prostu przetestować coś.

**[01:46:01]** I zobaczyć czy to daje wartość biznesową.

**[01:46:03]** To jakby o to chodzi żeby to przekazać.

**[01:46:16]** Tutaj z mojej strony tak.

**[01:46:21]** Tutaj z mojej strony tak.

**[01:46:23]** W sensie zależy.

**[01:46:28]** W sensie zależy.

**[01:46:31]** No bo na przykład.

**[01:46:33]** Też mogłabyś mieć taką usługę.

**[01:46:35]** W której ustawiasz komuś kontekst w firmie.

**[01:46:37]** Więc.

**[01:46:39]** No ja o tym samym pomyślałem.

**[01:46:41]** Że po prostu.

**[01:46:44]** To co nauczysz się w kursie.

**[01:46:46]** Czyli jakby ustawiać kontekst.

**[01:46:48]** Na przykład idziesz do firmy która zajmuje się logistyką.

**[01:46:50]** I tam oni nie mają żadnej osoby od AI.

**[01:46:52]** I ty jesteś osobą która.

**[01:46:54]** Im to konfiguruje.

**[01:46:56]** Po prostu wchodzi w temat.

**[01:46:58]** Wgryza się jakie mają procesy.

**[01:47:00]** I przekłada to na kontekst.

**[01:47:02]** Dokładnie.

**[01:47:04]** No dokładnie.

**[01:47:06]** No też o tym pomyślałam.

**[01:47:14]** SAS ma jeszcze sens.

**[01:47:17]** Ja robię.

**[01:47:19]** Ja robię jak coś kolejny.

**[01:47:21]** Więc chyba ma.

**[01:47:24]** Myślę że tak.

**[01:47:27]** Mamy tego przykłady.

**[01:47:29]** Możemy być dumnymi Polakami.

**[01:47:31]** Bardzo dużo SASów.

**[01:47:33]** Naszych rodaków rośnie w siłę.

**[01:47:35]** Więc chyba mają sens.

**[01:47:37]** Mogłabym rzucić z kaptura.

**[01:47:39]** Przynajmniej 5 firm.

**[01:47:41]** Które naprawdę dobrze sobie radzi za granicą.

**[01:47:45]** Ja odpalam nowy.

**[01:47:47]** Który jeszcze nie jest publicznie dostępny.

**[01:47:49]** Ale już ma klienta.

**[01:47:51]** Więc też niebawem będę dawał znać.

**[01:47:53]** Ale zapowiada się też obiecująco.

**[01:47:55]** Właśnie mi tutaj na boku.

**[01:47:57]** Na drugim monitorze.

**[01:47:59]** Kodeks koduje.

**[01:48:01]** Jakieś dodatkowe rzeczy.

**[01:48:03]** A raczej poprawki już takie finalizujące.

**[01:48:05]** No więc.

**[01:48:07]** Chyba ma.

**[01:48:09]** Będziecie też tak.

**[01:48:11]** W przyszłości.

**[01:48:14]** Mieć sobie agenta który działa.

**[01:48:16]** Całą dobę.

**[01:48:19]** Tak.

**[01:48:22]** No dzisiaj u mnie to jest codzienność.

**[01:48:24]** Że zostawiam coś na nockę.

**[01:48:26]** Albo gdzieś biorę komputer do domu.

**[01:48:28]** I kładę go gdzieś tam w jakimś miejscu.

**[01:48:30]** I coś tam się robi.

**[01:48:32]** No i takie jest założenie tego programu.

**[01:48:34]** Żebyście mieli na tyle kontekst ustawiony.

**[01:48:36]** Że on może działać autonomicznie bez was.

**[01:48:38]** Nie ma złotych gór oczywiście.

**[01:48:40]** Że on tam nie wiadomo co wam zrobi.

**[01:48:42]** Ale.

**[01:48:44]** Dobrze ustawiony kontekst.

**[01:48:46]** Pozwala na to.

**[01:48:48]** I odpowiednie podejście.

**[01:48:50]** Pozwala na to żeby coś się robiło.

**[01:48:52]** Przez ileś tam godzin.

**[01:48:54]** Bez waszego udziału.

**[01:48:56]** Ja tak działam na co dzień.

**[01:49:07]** To mogę szczerze powiedzieć.

**[01:49:14]** Takie mamy czasy teraz.

**[01:49:17]** O właśnie jeszcze zapomniałem tego pokazać.

**[01:49:19]** Więc może cofnijmy się.

**[01:49:21]** Z tym slajdem.

**[01:49:23]** To jest szkolenie AI operators.

**[01:49:25]** Od kiedy zaczynacie.

**[01:49:27]** Czyli dorywczo AI wam pomaga.

**[01:49:29]** Zaczynacie od początku.

**[01:49:31]** A będąc tym operatorem łączycie kontekst.

**[01:49:33]** Wyznaczacie granice.

**[01:49:35]** I zatwierdzacie rzeczy.

**[01:49:37]** I to wszystko zaczyna się układać.

**[01:49:39]** W jakiś taki spójny system.

**[01:49:41]** A nie chaos.

**[01:49:43]** Na którym mieliście na początku.

**[01:49:45]** Porozrzucane różne rzeczy gdzieś.

**[01:49:47]** I to wszystko za każdym razem.

**[01:49:49]** Wrzucane do kolejnego okienka w czacie.

**[01:49:51]** I tak dalej.

**[01:49:56]** Więc.

**[01:49:58]** Może zrobię mały przerwnik od pytań.

**[01:50:00]** I podkreślę raz jeszcze.

**[01:50:02]** Że ten program edukacyjny.

**[01:50:04]** Kierujemy do osób.

**[01:50:06]** Które chcą wejść głębiej w AI.

**[01:50:08]** Nie wiedzą od czego zacząć.

**[01:50:10]** Także do osób które używają AI.

**[01:50:12]** Ale zaczynają za każdym razem.

**[01:50:15]** Od zera.

**[01:50:17]** Nowy czad i tak dalej.

**[01:50:19]** I do osób też na ścieżce technicznej.

**[01:50:21]** Które pracują w IT.

**[01:50:23]** I chcą budować bezpieczne narzędzia dla agentów.

**[01:50:25]** Więc zapraszamy Was serdecznie.

**[01:50:27]** I naszym celem jest to.

**[01:50:29]** Byście mogli.

**[01:50:31]** Gdzieś w rozmówkach.

**[01:50:33]** W biurze przy kawce.

**[01:50:35]** Też błysnąć.

**[01:50:37]** Jakimś takim fajnym.

**[01:50:39]** Nie newsem.

**[01:50:42]** Ale nie wiem.

**[01:50:44]** Takim skillem.

**[01:50:46]** Że rozumiecie jak z tym AI gadać.

**[01:50:48]** I pracować mimo że jesteście osobami nietechnicznymi.

**[01:50:50]** I to też jest nasz cel.

**[01:50:52]** Żebyście po tym szkoleniu.

**[01:50:54]** Takie umiejętności też nabyli.

**[01:51:07]** Dobra.

**[01:51:09]** Czy są jeszcze jakieś pytania?

**[01:51:11]** Bo już mamy prawie dwie godziny.

**[01:51:14]** I się zastanawiam czy jeszcze coś mamy.

**[01:51:41]** Dzięki Paweł.

**[01:51:45]** Dziękujemy.

**[01:51:53]** Bardzo się cieszymy.

**[01:51:55]** Tu jest jeszcze pytanie jakieś.

**[01:51:57]** Czy jako mentorzy zajmujemy się tworzeniem aplikacji?

**[01:52:01]** No ja się zajmuję.

**[01:52:03]** Więc poproszę o kolejne pytanie.

**[01:52:05]** Ja już nie.

**[01:52:07]** Ale też się zajmowałam wcześniej.

**[01:52:09]** I nawet zbierałam rundę na własny startup.

**[01:52:11]** Zatrzymaliśmy projekt.

**[01:52:13]** Więc to też była moja historia.

**[01:52:15]** W zeszłym roku.

**[01:52:17]** Więc było tak.

**[01:52:19]** Ja też miałam swoją przygodę z SASem.

**[01:52:23]** I wbijałam jako CTO.

**[01:52:25]** Do projektu.

**[01:52:27]** Czyli byłam odpowiedzialna za kodowanie

**[01:52:29]** agenta od A do Z.

**[01:52:32]** Bo SAS był oczywiście agentem.

**[01:52:34]** No tak.

**[01:52:37]** U mnie teraz podobnie.

**[01:52:39]** Ten nowy SAS który tworzę to jest bardziej agent niż SAS.

**[01:52:41]** Więc dzisiaj chyba

**[01:52:43]** to ma bardziej sens

**[01:52:45]** niż takie klasyczne krudy, sasy

**[01:52:47]** które gdzieś tam zapisują dane.

**[01:52:49]** No ale to długo by o tym gadać.

**[01:52:51]** Nie temat na dzisiaj myślę.

**[01:52:53]** Tu jeszcze pytanie ważne.

**[01:52:55]** Czy są konsultacje jedyne w pakiecie?

**[01:52:57]** To od razu mówimy, że

**[01:52:59]** to są konsultacje grupowe.

**[01:53:01]** Jeden na jeden.

**[01:53:03]** To znaczy możesz zadać pytanie

**[01:53:05]** na czacie, na grupie.

**[01:53:07]** W ostateczności napisać nam brief wiadomość.

**[01:53:09]** Jak się wstydzisz tego pytania

**[01:53:11]** i nie chcesz żeby było na publicznie

**[01:53:13]** to też napisz na forum

**[01:53:15]** na sirklu

**[01:53:17]** na platformie możesz nam napisać.

**[01:53:19]** Musiałbyś mi powiedzieć

**[01:53:35]** oczekiwania jakie są twoje.

**[01:53:37]** Bo co już potrafisz

**[01:53:41]** co chciałbyś się nauczyć

**[01:53:43]** to tutaj pewnie wtedy doradzimy.

**[01:53:45]** Bo tak za mało danych

**[01:53:47]** żeby odpowiedzieć.

**[01:54:15]** Dobrze.

**[01:54:18]** Czy Ola ty masz jeszcze coś do dodania może?

**[01:54:20]** Coś nie powiedzieliśmy a mieliśmy powiedzieć.

**[01:54:22]** Myślę, że nie.

**[01:54:24]** Ale jeśli będziecie mieli jakieś pytania

**[01:54:26]** dalsze

**[01:54:28]** to zawsze możecie uderzyć do mnie na Instagramie.

**[01:54:30]** Ja jestem bardzo aktywna

**[01:54:32]** na tym Instagramie i chętnie odpowiem.

**[01:54:34]** Także w razie czego

**[01:54:36]** możecie pisać pod AI Zajączkowska.

**[01:54:38]** Być może niektórzy z was

**[01:54:40]** mnie kojarzą z tego profilu.

**[01:54:42]** Ja tam prowadzę.

**[01:54:44]** Mam bardzo dużo treści edukacyjnych

**[01:54:46]** o AI, o kodzie, ustawianiu kontekstu.

**[01:54:48]** Więc jakbyście mieli jakiekolwiek pytania

**[01:54:50]** to zawsze odsyłam do mojego Instagrama.

**[01:54:52]** Okej dobra.

**[01:54:58]** To jak zróbmy sobie może

**[01:55:00]** dwie minutki na ostatnie pytanie

**[01:55:02]** i jeśli

**[01:55:05]** będzie to będzie, jeśli nie to będziemy

**[01:55:07]** sobie kończyć.

**[01:55:09]** W międzyczasie dzięki wszystkim, którzy już

**[01:55:11]** zdecydowali się dołączyć.

**[01:55:13]** Bardzo doceniamy, że

**[01:55:15]** ufacie już nam na tym etapie.

**[01:55:17]** A my się odwdzięczymy najniższą ceną

**[01:55:19]** i tym dodatkowym bonusem,

**[01:55:21]** który widzicie tutaj

**[01:55:23]** na czerwono-pomarańczowo.

**[01:55:25]** Tak cieszymy się bardzo.

**[01:55:27]** No jest tutaj jakiś komentarz.

**[01:55:39]** Branża recyklingu

**[01:55:43]** w obszarze software'u nabiera znaczenia.

**[01:55:45]** Firmowa konsolidacja usług

**[01:55:47]** w ramach własnego

**[01:55:49]** jednego systemu

**[01:55:52]** lub redukcja

**[01:55:54]** softu u klienta.

**[01:55:57]** Chyba nie dokończyło się pytanie.

**[01:55:59]** Albo to był komentarz

**[01:56:01]** może do czegoś co mówiłeś.

**[01:56:03]** Może coś mówiliśmy.

**[01:56:28]** Dobra to myślę, że

**[01:56:30]** będziemy sobie kończyć.

**[01:56:32]** Dzięki Wam jeszcze raz za obecność.

**[01:56:34]** Przespędziliście z nami

**[01:56:36]** ten wieczór.

**[01:56:40]** Bardzo się cieszymy.

**[01:56:42]** Ja się cieszę, że mogłam Wam przekazać

**[01:56:44]** trochę wiedzy.

**[01:56:46]** Zawsze chętnie się nią dzielę.

**[01:56:50]** Tak jest. To co?

**[01:56:52]** Do zobaczenia jeszcze gdzieś kiedyś w internecie

**[01:56:54]** w razie czego jesteśmy w kontakcie mailowym

**[01:56:56]** lub na Instagramie.

**[01:56:58]** Do zobaczenia.