# KREDENS — podsumowanie projektu

Strona jednostronicowa dla restauracji KREDENS (Kraków), zbudowana na
szablonie [Landed](https://html5up.net/landed) (HTML5 UP). Projekt zamknięty
— to plik kontekstowy, żeby wznowienie pracy (w tej albo nowej rozmowie) nie
wymagało odtwarzania historii od zera.

**Strona live:** https://mateuszpietruniewicz-arch.github.io/kredens-restauracja/
**Repo:** https://github.com/mateuszpietruniewicz-arch/kredens-restauracja
(GitHub Pages, branch `main`, root — publikuje się automatycznie po każdym
pushu, przebudowa trwa ok. 30–90 s)

## Co jest na stronie

Hero → 3 pełnoekranowe rozdziały (historia / filozofia kuchni / sala) →
galeria (6 zdjęć) → menu → opinie gości → siatka 6 punktów "Dlaczego
Kredens" → pas CTA (bordo) → kontakt/stopka. Wszystkie zdjęcia (5 hero/
rozdziały + 6 galeria = 11) są już wgrane i skompresowane.

**Paleta:** #7A1F3D (bordo, jeden odważny akcent) / #F4EFE6 (kremowy) /
#B08D57 (mosiądz) / #1C1712 (ciemna czerń, tylko jako scrim na zdjęciach —
sekcje "Dlaczego Kredens" i stopka są jasne/kremowe, nie czarne).
**Fonty:** Cormorant Garamond (nagłówki) + Nunito Sans (reszta).

## Struktura plików

- `index.html` — cała strona
- `assets/css/main.css` — oryginalny CSS szablonu, **nie edytować**
- `assets/css/custom.css` — wszystkie nadpisania (paleta, fonty, layout,
  media query dla ekranów ≥1800px)
- `images/` — wszystkie zdjęcia, już uzupełnione
- `README.md` — instrukcja podglądu lokalnego i (nieaktualna już w części
  o zdjęciach, bo wszystkie są wgrane) lista wymagań co do kadrów
- `kredens-restauracja-brief.md`, `ZBUDUJ-KREDENS.md` — pierwotny brief
  projektowy, historyczne, nie aktualizowane w trakcie iteracji

## Historia iteracji (skrót)

1. Zbudowano całą stronę wg briefu na szablonie Landed, z placeholderami
   TODO zamiast zdjęć.
2. Dodano zdjęcia hero + 3 rozdziałów → skompresowane (~15MB → ~2,4MB).
3. Linki social (Instagram/Facebook) w stopce zmienione na strony główne
   fb.com / instagram.com — to strona pokazowa, nie ma realnego profilu.
4. Poprawki wyglądu: usunięto okrągłe zdjęcie z hero (było błędnie
   wykadrowane, ostatecznie usunięte na życzenie, nie naprawiane), złagodzono
   ciemny scrim na zdjęciach, rozjaśniono sekcje "Dlaczego Kredens" i stopkę
   z czarnego na kremowe, usunięto frazę "fajerwerki" z copy, dodano sekcję
   galerii z automatycznym fallbackiem dla brakujących zdjęć.
5. Zdjęcia rozdziału 1 i 3 były pierwotnie pionowe → przy pełnoekranowym
   `background-size:cover` gubiły kontekst kadru (widać było tylko wąski,
   mocno przybliżony fragment). Podmienione na poziome — naprawione.
6. Naprawiono wyścig w fallbacku galerii (obrazki `loading="lazy"` czasem
   nie zdążyły wykryć braku pliku przed wejściem w viewport przy szybkim
   scrollu) — dodano niezależną, natychmiastową sondę JS (`new Image()`
   poza DOM) uruchamianą od razu po `DOMContentLoaded`.
7. Naprawiono zbyt wąską kolumnę treści na ekranach ≥1800px (`.container`
   miał sztywny limit 70em) — poszerzono kontener i panele boczne w media
   query dla szerokich ekranów.
8. Dodano i skompresowano 6 zdjęć galerii (dania-02/03/04, wnetrze-02/03/04)
   — placeholdery zniknęły automatycznie, bez zmian w kodzie.

## Otwarte drobiazgi (nie krytyczne, nie zmieniane bez decyzji właściciela)

- **Facebook w stopce** — link prowadzi na `facebook.com` (stronę główną),
  nie na realny profil — nie ma takiego profilu, to celowe dla strony
  pokazowej.
- **`images/wnetrze-02.jpg`** — w tle widoczny fragment neonu/szyldu innego
  lokalu (górny prawy róg zdjęcia).
- **`images/wnetrze-04.jpg`** — na fasadzie budynku widoczny numer "57",
  niespójny z adresem podanym na stronie (ul. Kanonicza 8).
- `images/hero-detal.jpg` leży w repo, ale nie jest już nigdzie użyty (koło
  w hero zostało usunięte) — można go usunąć albo zostawić na potem.

## Jak wznowić pracę

Lokalny podgląd: `python3 -m http.server 8000` w katalogu projektu, potem
`http://localhost:8000`. Zmiany w stylach → `assets/css/custom.css` (ładowany
po `main.css`, nie edytować oryginału). Po zmianach: `git add`, `git commit`,
`git push origin main` — strona aktualizuje się automatycznie przez
GitHub Pages.
