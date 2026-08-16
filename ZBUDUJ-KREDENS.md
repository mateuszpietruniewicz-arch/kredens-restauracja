Pracujesz na już pobranym szablonie Landed (HTML5UP) w tym folderze. Zbuduj
na nim stronę restauracji KREDENS — klasyczna kuchnia polska i europejska,
Kraków. Poniżej masz wszystko: treść, dane, palety, i wnioski z trzech
poprzednich projektów portfolio (Wolska/Astral, Ziarno/Story,
Ognisko/Paradigm Shift) — przeczytaj je zanim zaczniesz, bo to konkretne
błędy, których NIE wolno powtórzyć.

===== WIZUALNE DNA SZABLONU — KONIECZNIE ZACHOWAJ =====
Sprawdziłem żywe demo Landed, nie tylko opis. To NIE jest układ
"zdjęcie-obok-tekstu". Rzeczywista struktura:
1. Hero: ciemne, przyciemnione zdjęcie w tle na pełny ekran + OKRĄGŁE,
   maskowane zdjęcie (idealne koło) jako ozdobny akcent obok nagłówka.
   Zachowaj tę okrągłą maskę — to charakterystyczny detal szablonu.
2. Trzy "rozdziały": każdy to JEDNO zdjęcie na pełną szerokość ekranu
   (edge-to-edge: border-radius:0, box-shadow:none, margin:0, padding:0),
   z tekstem (nagłówek + label + akapit) nałożonym BEZPOŚREDNIO na zdjęcie
   przez ciemny gradient/scrim pod spodem dla czytelności. NIE zamieniaj
   tego na "zdjęcie w boksie z tekstem obok" — to zgubi cały efekt (dokładnie
   ten błąd popełniony przy pierwszym buildzie Paradigm Shift dla Ognisko).
3. Siatka 6 punktów z ikonami na spokojnym, prawie czarnym tle.
4. Zamykający pas CTA w JEDNYM, w pełni nasyconym kolorze akcentu — nie
   przygaszonej, stonowanej wersji. To musi wyglądać odważnie.
Jeśli po zbudowaniu strona wygląda jak wąska kolumna tekstu obok małych
zdjęć w ramkach z cieniem — to źle, cofnij się i popraw zanim pójdziesz dalej.

===== WNIOSKI Z POPRZEDNICH 3 PROJEKTÓW =====
1. Każdy <img>: width/height + object-fit: cover — nic się nie rozciąga.
2. Żadne zdjęcie nie powtarza się dwa razy na stronie.
3. Zmiany CSS w osobnym assets/css/custom.css, ładowanym w <head> PO
   main.css — nie edytuj main.css bezpośrednio.
4. Sprawdź na szerokim ekranie (>1800px) — treść nie może się gubić w
   wąskiej kolumnie na pustym, płaskim tle.
5. Link do Google Maps jako zwykły przycisk/link, NIE osadzaj iframe z
   domyślną, kolorową mapą Google — gryzie się z paletą marki.
6. Stopka z "Wykonanie: widacwas.pl" wbudowana od razu, nie jako poprawka
   na później.
7. Sekcje, których nie ma w oryginalnym szablonie (tu: Menu, Opinie gości)
   buduj w spójnej stylistyce z sąsiednimi blokami, żeby nie wyglądały jak
   doklejka.
8. loading="eager" na hero i pierwszym widocznym zdjęciu, "lazy" na
   pozostałych, fade-in po załadowaniu (klasa .loaded, opacity 0→1).

PALETA: #7A1F3D (bordo/wino — JEDEN odważny akcent, przyciski i CTA) /
#F4EFE6 (kremowy, tło jasnych sekcji i tekst na ciemnym) / #B08D57
(mosiądz/złoto, drugorzędny akcent) / #1C1712 (ciepła, prawie czarna czerń —
scrimy pod tekstem na zdjęciach, tła ciemnych sekcji)

FONTY (Google Fonts, link w <head>): Cormorant Garamond — WYŁĄCZNIE
nagłówki (elegancki, wąski serif). Nunito Sans — cały pozostały tekst
(akapity, menu, kontakt, przyciski).

Zdjęcia dodasz później ręcznie — zostaw placeholdery z komentarzem HTML
`<!-- TODO ZDJĘCIE: opis -->` bezpośrednio nad każdym <img>, dokładny opis
potrzebnego kadru podany niżej przy każdej sekcji.

===== HERO =====
Tło (TODO ZDJĘCIE: przyciemniona sala restauracji, świece, obrus, pełny
ekran): img/hero-sala.jpg
Okrągłe zdjęcie (TODO ZDJĘCIE: zbliżenie na eleganckie danie na talerzu,
albo kieliszek wina przy świecy): img/hero-detal.jpg
Nagłówek: KREDENS
Podtytuł: "Klasyczna kuchnia polska i europejska w sercu Krakowa. Bez
fajerwerków na pokaz — tylko sprawdzone receptury, sezonowe składniki i
uważna obsługa."
Strzałka w dół → scroll do rozdziału 1.

===== ROZDZIAŁ 1 (pełnoekranowe zdjęcie + tekst nałożony) =====
Zdjęcie (TODO ZDJĘCIE: wnętrze restauracji — kamienne ściany, świece,
wysokie sufity, pełny ekran): img/rozdzial-1-wnetrze.jpg
Label: NASZA HISTORIA
Nagłówek: Kredens, który pamięta trzy pokolenia
Akapit 1: "Nazwa nie jest przypadkowa — w sali stoi prawdziwy kredens z
porcelaną, którą przekazywano w rodzinie od babci. Otworzyliśmy to miejsce,
żeby serwować dania, które się pamięta, w przestrzeni, która ma duszę."
Akapit 2: "Kamienica przy Kanoniczej ma się dobrze — wysokie sufity,
kamienne ściany, świece zamiast jarzeniówek. To sala, w której chce się
zostać dłużej niż planowano."

===== ROZDZIAŁ 2 (pełnoekranowe zdjęcie + tekst nałożony) =====
Zdjęcie (TODO ZDJĘCIE: danie główne z bliska, np. kaczka lub polędwiczki,
elegancko podane, pełny ekran): img/rozdzial-2-danie.jpg
Label: FILOZOFIA KUCHNI
Nagłówek: Klasyka wymaga precyzji, nie fajerwerków
Akapit: "Karta zmienia się z sezonem, ale zasady zostają te same: dobry
wywar warzy się dwa dni, mięso odpoczywa tyle, ile trzeba, a talerz wygląda
tak, jak sam obiad powinien smakować — spokojnie i dopracowanie."
Przycisk: "Zobacz menu" → scroll do sekcji Menu.

===== ROZDZIAŁ 3 (pełnoekranowe zdjęcie + tekst nałożony) =====
Zdjęcie (TODO ZDJĘCIE: detal sali — kredens z porcelaną, świecznik,
nakrycie stołu, pełny ekran): img/rozdzial-3-detal.jpg
Label: SALA I ATMOSFERA
Nagłówek: Miejsce na wieczór, który ma zostać w pamięci
Akapit: "Osiemnaście stolików, cisza, która sprzyja rozmowie, i obsługa,
która pamięta, jak lubisz swój stek wysmażony. To sala na rocznicę,
kolację biznesową albo po prostu wieczór, na który warto się ubrać
odrobinę lepiej."
Przycisk: "Zarezerwuj stolik" → scroll do sekcji Kontakt.

===== MENU (nowa sekcja, dodaj po rozdziale 3, PRZED siatką 6 punktów) =====
Tło: jasne, kremowe #F4EFE6 — świadomy kontrast wobec ciemnych rozdziałów
powyżej, czysta typografia bez wielkiego zdjęcia w tle.
Nagłówek: Menu
Podtytuł: "Karta zmienia się z sezonem — to wybór naszych stałych pozycji."

Przystawki:
- Tatar z polędwicy wołowej, żółtko, kapary — 42 zł
- Krem z pieczonych buraków, chrzan, kozi ser — 26 zł
- Śledź w oleju lnianym, cebula, jabłko — 28 zł

Dania główne:
- Kaczka pieczona, purée z pietruszki, wiśnie — 78 zł
- Polędwiczki wieprzowe, kasza gryczana, borowiki — 64 zł
- Sandacz na maśle, szpinak, beurre blanc — 72 zł
- Risotto z dynią i szałwią (wege) — 48 zł

Desery:
- Sernik na zimno wg przepisu babci — 24 zł
- Szarlotka na ciepło, lody waniliowe — 26 zł

Podpis pod menu: "Karta win dostępna na miejscu — zapytaj o dobór do
dania." Pod menu dodaj przycisk "Zarezerwuj stolik" (bordo #7A1F3D) →
scroll do sekcji Kontakt.

===== OPINIE GOŚCI (mały blok tuż pod menu, to samo jasne tło) =====
Dwa cytaty, kursywa, cienka bordowa kreska z lewej strony każdego:

"Najlepszy sernik w Krakowie, mówię to bez przesady. Obsługa pamiętała
naszą rocznicę z zeszłego roku." — Anna i Piotr, Kraków

"Miejsce na poważną kolację biznesową — cicho, elegancko, karta win
dobrana z głową." — Tomasz, gość biznesowy

===== SIATKA 6 PUNKTÓW (zostaje w oryginalnej pozycji szablonu, po menu) =====
Nagłówek: Dlaczego Kredens
Label: NASZE ZASADY
1. Rezerwacja telefoniczna lub mailowa — bez systemów, po prostu zadzwoń
2. Karta win dobrana przez sommeliera do każdego dania
3. Kolacje prywatne i degustacyjne na zamówienie
4. Sezonowe menu — zmienia się co kwartał
5. 18 stolików — kameralnie, bez pośpiechu
6. Miejsce dostępne dla osób na wózkach

===== ZAMYKAJĄCY CTA (pełnoszerokości pas, kolor #7A1F3D w pełnym nasyceniu) =====
Nagłówek: Zarezerwuj stolik na wieczór, który zapamiętasz
Podtytuł: "Zadzwoń albo napisz — odpowiadamy tego samego dnia."
Przycisk: "Zadzwoń: +48 12 345 67 89" → href="tel:+48123456789"

===== KONTAKT / STOPKA =====
Adres: ul. Kanonicza 8, 31-002 Kraków
Telefon: +48 12 345 67 89 (href="tel:+48123456789")
E-mail: rezerwacje@kredens-restauracja.pl
Godziny: Wt–Nd 13:00–22:00 · Poniedziałki nieczynne
Link "Otwórz w Google Maps" → href
"https://www.google.com/maps/search/?api=1&query=ul.+Kanonicza+8%2C+31-002+Krak%C3%B3w"
target="_blank" rel="noopener" (zwykły link, NIE osadzaj iframe)
Social: Instagram @kredens.krakow, Facebook

Stopka: "© 2026 KREDENS. Wszelkie prawa zastrzeżone. Design: HTML5 UP."
Druga linia: "Wykonanie: widacwas.pl" → link do https://widacwas.pl,
target="_blank" rel="noopener", ten sam rozmiar/kolor co linia powyżej.

===== SEO / META =====
title: "KREDENS — klasyczna restauracja | Kraków"
meta description: "KREDENS — klasyczna kuchnia polska i europejska w sercu
Krakowa. Sezonowe menu, kameralna sala, rezerwacje telefoniczne."

===== README.md — TODO dla mnie =====
- [ ] Dodać 5 zdjęć (patrz komentarze TODO w HTML): hero-sala.jpg,
      hero-detal.jpg, rozdzial-1-wnetrze.jpg, rozdzial-2-danie.jpg,
      rozdzial-3-detal.jpg
- [ ] Podmienić realny adres e-mail jeśli inny niż podany
- [ ] Sprawdzić kartę win / dodać jeśli ma być osobna sekcja

Po zakończeniu pokaż mi diff plików i potwierdź, że strona działa lokalnie
(python3 -m http.server) bez błędów w konsoli, a rozdziały nadal wyglądają
jak pełnoekranowe zdjęcia z tekstem nałożonym (nie boksy obok siebie).
