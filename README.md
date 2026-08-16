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

- `index.html` — cała strona (hero, 3 rozdziały pełnoekranowe, menu, opinie,
  siatka 6 punktów, CTA, kontakt/stopka)
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

Po wgraniu zdjęć zrób `git add images && git commit -m "Dodaj zdjęcia" && git push`
— strona na GitHub Pages zaktualizuje się automatycznie.

Źródła darmowych zdjęć: [unsplash.com](https://unsplash.com), [pexels.com](https://pexels.com).

## Licencja

Szablon Landed by HTML5 UP — wolny do użytku osobistego i komercyjnego na
licencji CCA 3.0 (patrz `LICENSE.txt`), z zachowaniem linku "Design: HTML5 UP"
w stopce.
