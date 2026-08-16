# KREDENS — strona restauracji

Statyczna strona jednostronicowa dla restauracji **KREDENS** (klasyczna kuchnia
polska i europejska, Kraków), zbudowana na bazie szablonu [Landed](https://html5up.net/landed)
(HTML5 UP).

## Podgląd lokalny

```bash
python3 -m http.server 8000
```

i wejdź na `http://localhost:8000`.

## Struktura

- `index.html` — cała strona (hero, 3 rozdziały pełnoekranowe, galeria, menu,
  opinie, siatka 6 punktów, CTA, kontakt/stopka)
- `assets/css/main.css` — oryginalny CSS szablonu (nie edytować)
- `assets/css/custom.css` — nadpisania: paleta KREDENS, fonty, style sekcji
  menu/opinii/kontaktu
- `images/` — zdjęcia strony (patrz sekcja niżej — do uzupełnienia)
- `kredens-restauracja-brief.md`, `ZBUDUJ-KREDENS.md` — brief projektowy

## Zdjęcia do dodania

Strona ma placeholdery `<!-- TODO ZDJĘCIE: ... -->` w `index.html` nad każdym
miejscem, gdzie brakuje zdjęcia. Wgraj pliki o dokładnie tych nazwach do
folderu `images/`:

| Plik | Wymiary (orientacyjnie) | Co ma przedstawiać |
|---|---|---|
| `images/hero-sala.jpg` | 1920×1080 lub większe, poziome | Przyciemniona sala restauracji — świece, obrus, pełny kadr na tło hero (zdjęcie będzie ściemnione gradientem, więc może być nawet jasne w oryginale) |
| `images/hero-detal.jpg` | min. 800×800, zdjęcie **kwadratowe** lub centrowane na środku (będzie przycięte do koła) | Zbliżenie na eleganckie danie na talerzu albo kieliszek wina przy świecy |
| `images/rozdzial-1-wnetrze.jpg` | 1920×1080 lub większe, poziome | Wnętrze restauracji — kamienne ściany, świece, wysokie sufity, pełny kadr sali |
| `images/rozdzial-2-danie.jpg` | 1920×1080 lub większe, poziome | Danie główne z bliska (np. kaczka, polędwiczki), elegancko podane |
| `images/rozdzial-3-detal.jpg` | 1920×1080 lub większe, poziome | Detal sali — kredens z porcelaną, świecznik, nakrycie stołu |

### Galeria (sekcja `#gallery`, opcjonalna)

Siatka 6 zdjęć między rozdziałem 3 a menu. Dopóki plików nie ma, sekcja sama
pokazuje czytelny placeholder (nazwa pliku + opis kadru) zamiast zepsutej
ikonki obrazka — wystarczy wgrać plik o właściwej nazwie do `images/`, bez
zmian w kodzie, a placeholder automatycznie zniknie i pojawi się zdjęcie.

| Plik | Co ma przedstawiać |
|---|---|
| `images/dania-02.jpg` | Danie z bliska, inny kadr niż w rozdziale 2 |
| `images/dania-03.jpg` | Deser lub przystawka, elegancko podana |
| `images/dania-04.jpg` | Kieliszek wina albo detal nakrycia stołu |
| `images/wnetrze-02.jpg` | Sala z innego kąta, stoliki |
| `images/wnetrze-03.jpg` | Kredens z porcelaną, zbliżenie |
| `images/wnetrze-04.jpg` | Detal wystroju albo wejście do lokalu |

Po wgraniu zdjęć (hero/rozdziały i/lub galeria) zrób
`git add images && git commit -m "Dodaj zdjęcia" && git push`
— strona na GitHub Pages zaktualizuje się automatycznie.

Źródła darmowych zdjęć: [unsplash.com](https://unsplash.com), [pexels.com](https://pexels.com).

## Licencja

Szablon Landed by HTML5 UP — wolny do użytku osobistego i komercyjnego na
licencji CCA 3.0 (patrz `LICENSE.txt`), z zachowaniem linku "Design: HTML5 UP"
w stopce.
